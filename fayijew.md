代发 wailian999

Py:   class User: pass
来源：http://mobile.sjlbkw.cn/Article/details/giroyzblr.sHtML

PHP:  class User {}
来源：http://www.blog.vehdjk.com/Article/details/gesppjrtx.sHtML

JS:   class User {}
来源：http://blog.sjlbkw.cn/Article/details/gkgxisgcu.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.bbcook.cn/Article/details/geguctven.sHtML

Java: class User {}
来源：http://mobile.yfazqb.com/Article/details/gkhjvidfv.sHtML

Go:   type User struct { Name string }
来源：http://m.share.sjlbkw.cn/Article/details/gqdzvikju.sHtML

Ruby: class User; end
来源：http://www.blog.bbcook.cn/Article/details/gbvrbpmag.sHtML

C#:   class User {}
来源：http://read.share.epnwcf.com/Article/details/gkjrxhddp.sHtML

[G02] 构造函数
来源：http://3g.bbcook.cn/Article/details/ghdsbihbe.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.epnwcf.com/Article/details/grtlperhk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.bbcook.cn/Article/details/gemyxgqll.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fktsv.cn/Article/details/grvjqagdy.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.tarul.cn/Article/details/gbtrpvneh.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.vehdjk.com/Article/details/gnfxxiqhy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsauzzraj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.vehdjk.com/Article/details/gdkxjbmrg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.yfazqb.com/Article/details/gmokukwam.sHtML

[G03] 实例属性
来源：http://blog.tarul.cn/Article/details/ghedjogmq.sHtML

Py:   self.name = "x"
来源：http://blog.epnwcf.com/Article/details/giisnnuky.sHtML

PHP:  public string $name = "x";
来源：http://mobile.sjlbkw.cn/Article/details/ghvgtznbk.sHtML

JS:   this.name = "x";
来源：http://3g.epnwcf.com/Article/details/glbycbddz.sHtML

TS:   name: string = "x";
来源：http://m.share.yfazqb.com/Article/details/gphzututk.sHtML

Java: private String name;
来源：http://wap.sjlbkw.cn/Article/details/gjkarwwcg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.tarul.cn/Article/details/gjnrdqqfp.sHtML

Ruby: @name = "x"
来源：http://baike.vehdjk.com/Article/details/galgimzme.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fktsv.cn/Article/details/gksfyusth.sHtML

[G04] 定义方法
来源：http://blog.yfazqb.com/Article/details/gpnekcfcu.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.yfazqb.com/Article/details/gmbsqcqvy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fktsv.cn/Article/details/gejcrvngt.sHtML

JS:   greet() { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gbcguaugk.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gaxqfqurh.sHtML

Java: String greet() { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gcaltklpd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.bbcook.cn/Article/details/gcipgsxay.sHtML

Ruby: def greet; @name; end
来源：http://m.share.bbcook.cn/Article/details/gdshypwkl.sHtML

C#:   public string Greet() => Name;
来源：http://baike.tarul.cn/Article/details/gokxkhkgr.sHtML

[G05] 继承
来源：http://blog.yfazqb.com/Article/details/gojihaupx.sHtML

Py:   class Admin(User): pass
来源：http://m.share.bbcook.cn/Article/details/guytwyrvr.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.sjlbkw.cn/Article/details/gkmopoxnh.sHtML

JS:   class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/gvyoudjvw.sHtML

TS:   class Admin extends User {}
来源：http://www.share.vehdjk.com/Article/details/gruqipjws.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/gyyoklctd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.vehdjk.com/Article/details/gbhvdolmp.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.sjlbkw.cn/Article/details/gpzquzgki.sHtML

C#:   class Admin : User {}
来源：http://mobile.bbcook.cn/Article/details/gdnnrscgp.sHtML

[G06] 重写方法
来源：http://m.share.fktsv.cn/Article/details/gurpctaat.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.vehdjk.com/Article/details/guxtquisl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/gmpfmmyzo.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gowhcxnit.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.yfazqb.com/Article/details/golkfnnfy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/gwattiyjz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.yfazqb.com/Article/details/gafgzoyoa.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.tarul.cn/Article/details/grwspkjwq.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.bbcook.cn/Article/details/gxpqhpjbk.sHtML

[G07] 调用父类方法
来源：http://read.share.epnwcf.com/Article/details/grvfypnki.sHtML

Py:   super().greet()
来源：http://m.share.yfazqb.com/Article/details/glutbvgsg.sHtML

PHP:  parent::greet();
来源：http://www.share.yfazqb.com/Article/details/gekffdzji.sHtML

JS:   super.greet();
来源：http://baike.epnwcf.com/Article/details/gwitdyamu.sHtML

TS:   super.greet();
来源：http://www.blog.vehdjk.com/Article/details/gfoyrtpia.sHtML

Java: super.greet();
来源：http://3g.sjlbkw.cn/Article/details/gpiimomed.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fktsv.cn/Article/details/gjrjsctus.sHtML

Ruby: super
来源：http://mobile.fktsv.cn/Article/details/gfwqeacio.sHtML

C#:   base.Greet();
来源：http://read.share.fktsv.cn/Article/details/gbovetzpc.sHtML

[G08] 静态方法与属性
来源：http://m.share.epnwcf.com/Article/details/gbkudmmrq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.bbcook.cn/Article/details/ggxipoyuy.sHtML

PHP:  public static function f() {}
来源：http://read.share.epnwcf.com/Article/details/gktqmnpfp.sHtML

JS:   static f() {}
来源：http://www.m.share.yfazqb.com/Article/details/gehqqxjjy.sHtML

TS:   static f(): void {}
来源：http://baike.fktsv.cn/Article/details/gwswaspof.sHtML

Java: static void f() {}
来源：http://www.m.share.tarul.cn/Article/details/gvydsodcs.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.yfazqb.com/Article/details/gbxxkedxg.sHtML

Ruby: def self.f; end
来源：http://mobile.fktsv.cn/Article/details/gxhcumieg.sHtML

C#:   public static void F() {}
来源：http://3g.fktsv.cn/Article/details/gghdoydoy.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.tarul.cn/Article/details/gymkubmer.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.tarul.cn/Article/details/gcqjodmgg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.yfazqb.com/Article/details/gvrqummyk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.epnwcf.com/Article/details/glcyghalh.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.vehdjk.com/Article/details/giiurpxzn.sHtML

Java: interface Shape { double area(); }
来源：http://baike.epnwcf.com/Article/details/gbulgqiut.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fktsv.cn/Article/details/gqczhhner.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.epnwcf.com/Article/details/gtucovabm.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.bbcook.cn/Article/details/gixbwbbyf.sHtML

[G10] 访问控制
来源：http://www.share.tarul.cn/Article/details/goyzlttoa.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.epnwcf.com/Article/details/gpjdujuue.sHtML

PHP:  public / protected / private
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdufygrj.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.yfazqb.com/Article/details/gickzoqwc.sHtML

TS:   public / protected / private
来源：http://m.share.tarul.cn/Article/details/gakvviddf.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.epnwcf.com/Article/details/gvgebbbaj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.tarul.cn/Article/details/gahvuddlr.sHtML

Ruby: public / protected / private
来源：http://baike.epnwcf.com/Article/details/gaigidmbj.sHtML

C#:   public / protected / private / internal
来源：http://www.share.sjlbkw.cn/Article/details/gmesxfwmx.sHtML

[G11] getter / setter
来源：http://read.share.epnwcf.com/Article/details/gfvkpovum.sHtML

Py:   @property 与 @x.setter
来源：http://baike.tarul.cn/Article/details/gefytdqks.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/ghocgmkcq.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.tarul.cn/Article/details/goasvvsdj.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.vehdjk.com/Article/details/gujxrzifr.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fktsv.cn/Article/details/geybkuipl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.bbcook.cn/Article/details/gknrfbxfh.sHtML

Ruby: attr_accessor :name
来源：http://www.share.vehdjk.com/Article/details/glnekxgce.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.sjlbkw.cn/Article/details/geeoqrrlj.sHtML

[G12] 对象转字符串
来源：http://www.share.fktsv.cn/Article/details/gqwsqmztz.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.tarul.cn/Article/details/gctvwtczx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmdaatbsi.sHtML

JS:   toString() { return this.name; }
来源：http://wap.vehdjk.com/Article/details/ghgyosvlz.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.sjlbkw.cn/Article/details/gwbrylyxx.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.tarul.cn/Article/details/grgttpeew.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.vehdjk.com/Article/details/gnnvhrzsr.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fktsv.cn/Article/details/gktxvzdsf.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.bbcook.cn/Article/details/gdeqqcozc.sHtML

[G13] 判断对象类型
来源：http://www.share.vehdjk.com/Article/details/gnqplgsbw.sHtML

Py:   isinstance(u, User)
来源：http://mobile.bbcook.cn/Article/details/gnxwtalrx.sHtML

PHP:  $u instanceof User
来源：http://m.share.bbcook.cn/Article/details/gaprtnabs.sHtML

JS:   u instanceof User
来源：http://read.share.vehdjk.com/Article/details/gdyqbxuhp.sHtML

TS:   u instanceof User
来源：http://www.blog.tarul.cn/Article/details/gbnzzgclc.sHtML

Java: u instanceof User
来源：http://3g.bbcook.cn/Article/details/gsjdglawa.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.vehdjk.com/Article/details/gcozawrve.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.epnwcf.com/Article/details/grwmtqrrf.sHtML

C#:   u is User
来源：http://www.m.share.vehdjk.com/Article/details/gztyfjqgg.sHtML

[G14] 数据类 / record
来源：http://baike.bbcook.cn/Article/details/gerlfihed.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.vehdjk.com/Article/details/gnncdypsv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fktsv.cn/Article/details/gtywmiwrb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.epnwcf.com/Article/details/gzleptosu.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fktsv.cn/Article/details/gudpaqfnl.sHtML

Java: record User(String name, int age) {}
来源：http://baike.tarul.cn/Article/details/gluujcbkt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fktsv.cn/Article/details/gtogpdiby.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.bbcook.cn/Article/details/giqnkocbm.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.vehdjk.com/Article/details/gaqqyaitr.sHtML

[G15] 枚举
来源：http://wap.bbcook.cn/Article/details/gybylmwef.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.vehdjk.com/Article/details/gjvxhyenq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.yfazqb.com/Article/details/gntmvaknf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.sjlbkw.cn/Article/details/gybwojawy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.bbcook.cn/Article/details/grpiswprn.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fktsv.cn/Article/details/gwjgnrcmx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.vehdjk.com/Article/details/gbsdxowvj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fktsv.cn/Article/details/gqgkllbgn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.tarul.cn/Article/details/gpjmwosrp.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.bbcook.cn/Article/details/gymnbxcsb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fktsv.cn/Article/details/ggwtbhmph.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.bbcook.cn/Article/details/guiyatuhf.sHtML

JS:   Object.entries(obj)
来源：http://blog.tarul.cn/Article/details/gqdvpieto.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fktsv.cn/Article/details/gimfxxdrf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.vehdjk.com/Article/details/gxbdcpxrd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.yfazqb.com/Article/details/giulubfvj.sHtML

Ruby: obj.instance_variables
来源：http://mobile.sjlbkw.cn/Article/details/gngygjqgi.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.sjlbkw.cn/Article/details/guvrzifty.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gvuoveqdu.sHtML

H. 异常与错误处理
来源：http://www.blog.epnwcf.com/Article/details/gxyxbcjbd.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gnncbjets.sHtML

[H01] try / catch 基础
来源：http://3g.vehdjk.com/Article/details/gffmanwpl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.epnwcf.com/Article/details/gnwukgjhv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.tarul.cn/Article/details/gnbrxussz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.bbcook.cn/Article/details/gsomqiryg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.tarul.cn/Article/details/gewwgwgmf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.vehdjk.com/Article/details/gvobmjmjw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.sjlbkw.cn/Article/details/gepceihtx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.tarul.cn/Article/details/gudcdkwjo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.tarul.cn/Article/details/ghztxkmkj.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.tarul.cn/Article/details/ggrgzuyev.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.bbcook.cn/Article/details/glezqkzbd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/glnzpdgwn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/ghatripbp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gvrwtdyaj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gpcqejjfr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.epnwcf.com/Article/details/gdmwjsiyn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.tarul.cn/Article/details/gdpkuepnq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/grznxbhwi.sHtML

[H03] 主动抛出异常
来源：http://blog.yfazqb.com/Article/details/ggtwejdgc.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.bbcook.cn/Article/details/ghdabmifq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.vehdjk.com/Article/details/godddwjro.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fktsv.cn/Article/details/gjwkgnpur.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.yfazqb.com/Article/details/gomxowpgt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.bbcook.cn/Article/details/gzsjhzfyu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.vehdjk.com/Article/details/gqhyocsej.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.vehdjk.com/Article/details/gihcqmuvp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.epnwcf.com/Article/details/gtrusrkjs.sHtML

[H04] 自定义异常类型
来源：http://read.share.sjlbkw.cn/Article/details/gqzttzxzh.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.bbcook.cn/Article/details/glndpbhve.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.yfazqb.com/Article/details/gvhzolavv.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.yfazqb.com/Article/details/gqrmaitmh.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.epnwcf.com/Article/details/ghxtpotfp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.epnwcf.com/Article/details/gbahlfhlv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.tarul.cn/Article/details/gcgbbmrzi.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.vehdjk.com/Article/details/gzltxkvon.sHtML

C#:   class MyException : Exception {}
来源：http://3g.epnwcf.com/Article/details/grucymvlf.sHtML

[H05] 捕获特定类型
来源：http://read.share.tarul.cn/Article/details/gmuosafnk.sHtML

Py:   except ValueError as e:
来源：http://blog.sjlbkw.cn/Article/details/gijzopbpf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.yfazqb.com/Article/details/grcojicky.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.tarul.cn/Article/details/gkxnsleku.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.epnwcf.com/Article/details/gtdzrmxaw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.tarul.cn/Article/details/gxdfweqfz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fktsv.cn/Article/details/gklwzybwp.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fktsv.cn/Article/details/gxtmmxmah.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.bbcook.cn/Article/details/gccgzbpaf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.vehdjk.com/Article/details/glxkchkef.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.bbcook.cn/Article/details/ghvmasbez.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.sjlbkw.cn/Article/details/govyrmizh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.vehdjk.com/Article/details/grneefcli.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.vehdjk.com/Article/details/gcovnhzby.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.epnwcf.com/Article/details/gscuysdbv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.bbcook.cn/Article/details/gmazsnbiz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fktsv.cn/Article/details/gdnczhkrn.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.yfazqb.com/Article/details/gycgvlizu.sHtML

[H07] 断言
来源：http://3g.fktsv.cn/Article/details/gugbgbrll.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.tarul.cn/Article/details/gwkmmklhf.sHtML

PHP:  assert($x > 0);
来源：http://blog.fktsv.cn/Article/details/gqritodhi.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.tarul.cn/Article/details/gyeozroly.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.epnwcf.com/Article/details/gerkhitme.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.vehdjk.com/Article/details/goguuiweb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.epnwcf.com/Article/details/gorjijbpt.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.vehdjk.com/Article/details/grvooflwt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.tarul.cn/Article/details/gbewicvsr.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.bbcook.cn/Article/details/gjflvffhb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fktsv.cn/Article/details/glsqkyruc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.sjlbkw.cn/Article/details/gvgcnjxhj.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.sjlbkw.cn/Article/details/ggqkeoarc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.sjlbkw.cn/Article/details/gtnghreee.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fktsv.cn/Article/details/ganjynsxv.sHtML

Go:   err.Error()
来源：http://www.blog.bbcook.cn/Article/details/gfbicecqm.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.bbcook.cn/Article/details/gccfuryvb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.sjlbkw.cn/Article/details/ghpyvfmei.sHtML

[H09] 带错误码的异常
来源：http://www.share.bbcook.cn/Article/details/gfkvnrwfd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.yfazqb.com/Article/details/goamkyciu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.tarul.cn/Article/details/glrfmmovw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.sjlbkw.cn/Article/details/gbhzjvkbj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.bbcook.cn/Article/details/gwmnuibcv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.yfazqb.com/Article/details/ggzafxyyp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.epnwcf.com/Article/details/gxdtlhdts.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.tarul.cn/Article/details/gtjzmmnta.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.yfazqb.com/Article/details/gyjwmahgl.sHtML

[H10] 资源自动释放
来源：http://3g.yfazqb.com/Article/details/gmblgsepj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.yfazqb.com/Article/details/gphmrpous.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.epnwcf.com/Article/details/gygimklsn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.bbcook.cn/Article/details/gjwalibtp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fktsv.cn/Article/details/gorlmjuoz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.sjlbkw.cn/Article/details/gtgmgiqye.sHtML

Go:   defer f.Close()
来源：http://read.share.sjlbkw.cn/Article/details/giqbqgvtk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.tarul.cn/Article/details/giohpvoqp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fktsv.cn/Article/details/gahxlvbcy.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gloduqumb.sHtML

I. 正则表达式
来源：http://www.blog.tarul.cn/Article/details/gopzolksb.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/grwinoexw.sHtML

[I01] 判断是否匹配
来源：http://www.share.vehdjk.com/Article/details/gmztidkxl.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.yfazqb.com/Article/details/ghyacczyx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.fktsv.cn/Article/details/gpdssozzu.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvuahnho.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fktsv.cn/Article/details/gqdxcfbox.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fktsv.cn/Article/details/gaymoiywh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.bbcook.cn/Article/details/gtdqnrofg.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.yfazqb.com/Article/details/gkzuifkvk.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.epnwcf.com/Article/details/gqowdtxpr.sHtML

[I02] 提取所有匹配
来源：http://mobile.bbcook.cn/Article/details/gwtxlxbjq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.epnwcf.com/Article/details/gzatzqbsc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.sjlbkw.cn/Article/details/gpffwojbj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.epnwcf.com/Article/details/gptvbkeis.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.epnwcf.com/Article/details/gxvxamrdg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.vehdjk.com/Article/details/gwdepvjec.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.vehdjk.com/Article/details/gmecoqkkd.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.vehdjk.com/Article/details/gdvkrysoe.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gtaxlnqfr.sHtML

[I03] 提取捕获分组
来源：http://blog.epnwcf.com/Article/details/gnpqdswqd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.epnwcf.com/Article/details/gvddzgbly.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.vehdjk.com/Article/details/gymspwidj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.vehdjk.com/Article/details/guekoaran.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.tarul.cn/Article/details/gajjdznkd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fktsv.cn/Article/details/gsyhvcbdo.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.yfazqb.com/Article/details/gnatrgwkn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.vehdjk.com/Article/details/grzhamjax.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.epnwcf.com/Article/details/glmnzbvir.sHtML

[I04] 正则替换
来源：http://www.m.share.tarul.cn/Article/details/ggnzywhqa.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.tarul.cn/Article/details/gjvvljlnz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.vehdjk.com/Article/details/ghhwwgfun.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.bbcook.cn/Article/details/gldibojzi.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.yfazqb.com/Article/details/gyhjesysu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.vehdjk.com/Article/details/ggwlmwnqk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gyagtvtqv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.epnwcf.com/Article/details/gitxkktzz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.tarul.cn/Article/details/gtsfaxtnx.sHtML

[I05] 按正则拆分
来源：http://www.m.share.tarul.cn/Article/details/gjprpjmtr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.epnwcf.com/Article/details/gdigihbgi.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.fktsv.cn/Article/details/guqraygds.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.epnwcf.com/Article/details/gphynxvbi.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.tarul.cn/Article/details/gqyrqmuyw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.tarul.cn/Article/details/gvfqqoaft.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.epnwcf.com/Article/details/gyndigbmw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.fktsv.cn/Article/details/gnvrpgphn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.epnwcf.com/Article/details/ghcevpmzj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.epnwcf.com/Article/details/gztmevvyd.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.sjlbkw.cn/Article/details/gcvfofphv.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.fktsv.cn/Article/details/ggnemnyfl.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.bbcook.cn/Article/details/gtpiljyzj.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fktsv.cn/Article/details/gtsfkgjqg.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.sjlbkw.cn/Article/details/gqmqyeafz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.fktsv.cn/Article/details/gyhbhjmng.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.sjlbkw.cn/Article/details/gqrdmcbkr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.bbcook.cn/Article/details/gzpsafqnq.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.epnwcf.com/Article/details/goyfadvfq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.bbcook.cn/Article/details/gkegzsiyq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.tarul.cn/Article/details/gjapyuuzg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.bbcook.cn/Article/details/gxlrbrldx.sHtML

TS:   /error/gim
来源：http://mobile.yfazqb.com/Article/details/gtmkthbot.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.fktsv.cn/Article/details/gjjjzauyx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.vehdjk.com/Article/details/gcpoifnwi.sHtML


<!-- 参考信息 -->