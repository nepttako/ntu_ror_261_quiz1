1. 請說明 Fixnum (整數) 和 Float (浮點數) 之間的差異
Fixnum 為整數，例如：1, 299, 312。
Float 為有小數點的數字，例如：3.14, 0.01。

2. 今天有兩個字串：
  ```ruby 
  str1 = "Hallo Welt!" 
  str2 = " NTU Rails 261!"
  ```
請說明以下兩個印出字串的方式的不同處：
  ```ruby
  puts str1 + str2
  puts "#{str1}#{str2}"
  ```
結果相同但 + 號耗記憶體

3. 請解釋 array 和 hash 的不同處
array 為陣列，例如：[1,2,3,4,5]，可儲存數字、文字及其它資料。
hash 為雜湊，由Key & Value 所組合成，例如：{"cat" => "Dobby", "dog" => "Lucky"} 每一個Key有一個value.

4. 請寫一段 code 從 [1, "a string", 3.14, [1,2,3,4]] 這個陣列找出所有非字串的值
  ```ruby
  array = [1, "a string", 3.14, [1,2,3,4]]
  array.each do |item|
	unless item.kind_of?(Array) == true
		puts item
	end
  end
  ```

5. 請列出兩種產出亂數的方法
use shuffle.last or sample.
For example: array.shuffle.last or array.sample.

6. 請把 hoemowrk1 程式碼裡的裡面的使用者輸入兩個數字的方式和輸贏的判斷式改寫成 method
https://github.com/nepttako/test/blob/master/homework2a.rb

7. 以下這段程式碼：
  ```ruby
  ((1 > 3)&&(true == true))||(!!!false)
  ```
  會執行出什麼結果？ 請試試不用 irb 算出結果
首先 （1>3) 為 false, （true == true） 為 true, (!!!false) 為 true, 所以此題為true.

8. 請問 binding.pry 是什麼？ 要如何使用它？
pry 為除錯的 gem, 需安裝 gem install pry


9. 下面的一段程式碼，請嘗試用其他方法把 if...else...end 簡化成一行

  ```ruby
  var = 5

  puts var >= 5? "var is greater than or equal to 5" : "var is less than 5"
  
  ```


