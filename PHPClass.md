# কিভাবে আমরা ক্লাস লিখবো ?

# Example Class
        <?php
        
        class Fruit
        {
        
#            //properties
            
            public $name;
            public $color;
            
#            //Methods
            
            public function set_name($name)
            {
                $this->name = $name;
            }
        
            public function get_name()
            {
                return $this->name;
            }
        
            public function set_color($color)
            {
                $this->color = $color;
            }
        
            public function get_color()
            {
                return $this->color;
            }
        
        }
        
#        // Object make
        
        $apple = new Fruit();
        $banana = new Fruit();
        
#        // Assign a value in Methods

        $apple->set_color('Reza');
        $banana->set_color('Prince');
        
        $apple->set_name('Apple');
        $banana->set_name('Banana');

#        // Print all assign value 
        echo $apple->get_name();
        echo "<br>";
        echo $banana->get_name();
        echo "<br>";
        echo $apple->get_color();
        echo "<br>";
        echo $banana->get_color();
        echo "<br>";
        ?>


* ক্লাসের (Class) ভিতর {

    ভেরিয়েবল ($name) কে বলে প্রপার্টি (Properties) ;
    
    ফাংশন (function) কে বলে মেথড (Methods);

  }
