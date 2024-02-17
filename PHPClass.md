# কিভাবে আমরা ক্লাস লিখবো ?

** PHP তে অবজেক্ট ওরিয়েন্টেড প্রোগ্রামিং লেখার জন্য 'Class' KeyWord ব্যবহার করতে হয় .

* ক্লাসের (Class) ভিতর {

    ভেরিয়েবল ($name) কে বলে প্রপার্টি (Properties) ;
    
    ফাংশন (function) কে বলে মেথড (Methods);

  }

# Example Class
        <?php
        
        class Fruit
        {
        
            //Properties
            
            public $name;
            public $color;
            
            //Methods
            
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
        
        // Object make
        
        $apple = new Fruit();
        $banana = new Fruit();
        
        // Assign a value in Methods

        $apple->set_color('Reza');
        $banana->set_color('Prince');
        
        $apple->set_name('Apple');
        $banana->set_name('Banana');

        // Print all assign value 
        
        echo $apple->get_name();
        echo "<br>";
        echo $banana->get_name();
        echo "<br>";
        echo $apple->get_color();
        echo "<br>";
        echo $banana->get_color();
        echo "<br>";
        ?>

# new KeyWord দিয়ে কি করা হয় ?

** new কিওয়ার্ড টা বোঝার আগে আমাদের বুঝতে হবে অবজেক্ট কি ?

-> Object ছাড়া Class অচল! আমরা একটি ক্লাস থেকে একাধিক অবজেক্ট তৈরি করতে পারি। প্রত্যেকটি অবজেক্ট এর ভেতর Class এ 
বিদ্যমান Methods এবং Properties এর সকল বৈশিষ্ট্য রয়েছে।

        // Object make
        
        $apple = new Fruit();
        $banana = new Fruit();
        
* এখানে new KeyWord দিয়ে নতুন একটি অবজেক্ট তৈরি করা হয়েছে।

# $this OR '->' দিয়ে কি করা হয় ?
        
# এখানে ব্যবহারকৃত KeyWords
*new
*class
