代发 wailian999

Java: class User {}
来源：http://wap.tarul.cn/Article/details/gicfzowxg.sHtML

Go:   type User struct { Name string }
来源：http://3g.tarul.cn/Article/details/goalizewb.sHtML

Ruby: class User; end
来源：http://wap.vehdjk.com/Article/details/gkshrvlwq.sHtML

C#:   class User {}
来源：http://www.blog.tarul.cn/Article/details/gdtskyuav.sHtML

[G02] 构造函数
来源：http://www.m.share.bbcook.cn/Article/details/godmacmzc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.yfazqb.com/Article/details/genedpptt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.sjlbkw.cn/Article/details/gqcggxucz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gifgxdqii.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.epnwcf.com/Article/details/gdbfphtyw.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.epnwcf.com/Article/details/gvsxzkiot.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fktsv.cn/Article/details/gyhumdeio.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.bbcook.cn/Article/details/gcesqtpig.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.yfazqb.com/Article/details/gszuisngw.sHtML

[G03] 实例属性
来源：http://baike.bbcook.cn/Article/details/gnzopevpu.sHtML

Py:   self.name = "x"
来源：http://mobile.bbcook.cn/Article/details/gyizytgrn.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fktsv.cn/Article/details/givmhqoam.sHtML

JS:   this.name = "x";
来源：http://m.share.tarul.cn/Article/details/gpjbciimo.sHtML

TS:   name: string = "x";
来源：http://wap.yfazqb.com/Article/details/gjlsxhpis.sHtML

Java: private String name;
来源：http://www.share.yfazqb.com/Article/details/gdfhlpljm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.vehdjk.com/Article/details/gyfgbuuyy.sHtML

Ruby: @name = "x"
来源：http://3g.bbcook.cn/Article/details/guwvkrjky.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fktsv.cn/Article/details/gvcrjjybc.sHtML

[G04] 定义方法
来源：http://baike.fktsv.cn/Article/details/gjfcfyfvc.sHtML

Py:   def greet(self): return self.name
来源：http://blog.sjlbkw.cn/Article/details/gfjbicyqr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.vehdjk.com/Article/details/gepkfibdx.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/gkxkekubz.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/gdkjhucfp.sHtML

Java: String greet() { return name; }
来源：http://blog.fktsv.cn/Article/details/gypmeltjz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.yfazqb.com/Article/details/gwjovbndd.sHtML

Ruby: def greet; @name; end
来源：http://3g.bbcook.cn/Article/details/gxloftbxo.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.vehdjk.com/Article/details/gpjctgbqy.sHtML

[G05] 继承
来源：http://blog.sjlbkw.cn/Article/details/gcqebuhio.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.vehdjk.com/Article/details/grpbbngpb.sHtML

PHP:  class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/ggwdsmwkz.sHtML

JS:   class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gfvvcmppt.sHtML

TS:   class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/gpohacojy.sHtML

Java: class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gqwapwxmv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.sjlbkw.cn/Article/details/goxdrtpus.sHtML

Ruby: class Admin < User; end
来源：http://3g.tarul.cn/Article/details/gfyjhlrbf.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.epnwcf.com/Article/details/gpujnnhbl.sHtML

[G06] 重写方法
来源：http://blog.tarul.cn/Article/details/gxefnmljf.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.bbcook.cn/Article/details/gcggwjnfo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.tarul.cn/Article/details/gvzcpxvyt.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/gjodipayh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gzsuoelmg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.yfazqb.com/Article/details/gjblfggwz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.vehdjk.com/Article/details/gmbexvopv.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.epnwcf.com/Article/details/gkvbmnxch.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fktsv.cn/Article/details/gjriiohvo.sHtML

[G07] 调用父类方法
来源：http://read.share.epnwcf.com/Article/details/gcasdefif.sHtML

Py:   super().greet()
来源：http://www.share.sjlbkw.cn/Article/details/gyweecgsg.sHtML

PHP:  parent::greet();
来源：http://www.blog.fktsv.cn/Article/details/gygtgqple.sHtML

JS:   super.greet();
来源：http://read.share.bbcook.cn/Article/details/gimoyrdhv.sHtML

TS:   super.greet();
来源：http://www.blog.tarul.cn/Article/details/gbywzkply.sHtML

Java: super.greet();
来源：http://www.m.share.yfazqb.com/Article/details/gaincqjno.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.sjlbkw.cn/Article/details/giwxafcyc.sHtML

Ruby: super
来源：http://m.share.vehdjk.com/Article/details/glmadfzkg.sHtML

C#:   base.Greet();
来源：http://m.share.vehdjk.com/Article/details/glkzfwcbp.sHtML

[G08] 静态方法与属性
来源：http://m.share.bbcook.cn/Article/details/gxataihvq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.vehdjk.com/Article/details/gvwglbswz.sHtML

PHP:  public static function f() {}
来源：http://m.share.yfazqb.com/Article/details/gobpdcgwz.sHtML

JS:   static f() {}
来源：http://wap.vehdjk.com/Article/details/guzjlnkae.sHtML

TS:   static f(): void {}
来源：http://blog.tarul.cn/Article/details/gwfweknip.sHtML

Java: static void f() {}
来源：http://www.share.fktsv.cn/Article/details/gevfxpypf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.yfazqb.com/Article/details/gqwmlsxpr.sHtML

Ruby: def self.f; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gchdowzcq.sHtML

C#:   public static void F() {}
来源：http://blog.tarul.cn/Article/details/gxkkyfnxz.sHtML

[G09] 接口 / 抽象类
来源：http://baike.sjlbkw.cn/Article/details/gxogazprp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.yfazqb.com/Article/details/gsixbvyys.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.epnwcf.com/Article/details/gvyjngywp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.tarul.cn/Article/details/gnayabcrh.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.vehdjk.com/Article/details/gwvlateyz.sHtML

Java: interface Shape { double area(); }
来源：http://blog.epnwcf.com/Article/details/gdcjhucez.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.vehdjk.com/Article/details/gtocfuguc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.yfazqb.com/Article/details/gtgnlmjpm.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.bbcook.cn/Article/details/gdaauqyfq.sHtML

[G10] 访问控制
来源：http://www.share.sjlbkw.cn/Article/details/gutkchvhg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.yfazqb.com/Article/details/glnagnbtz.sHtML

PHP:  public / protected / private
来源：http://3g.fktsv.cn/Article/details/gvijmyofj.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fktsv.cn/Article/details/ggyohylyx.sHtML

TS:   public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/gxrjvykmm.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.epnwcf.com/Article/details/gbkbhgbrm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.yfazqb.com/Article/details/ghakuiqut.sHtML

Ruby: public / protected / private
来源：http://read.share.sjlbkw.cn/Article/details/gwvnflzci.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.yfazqb.com/Article/details/gukumwphw.sHtML

[G11] getter / setter
来源：http://baike.vehdjk.com/Article/details/gwzrrsaok.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.epnwcf.com/Article/details/gbtozkvyx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.yfazqb.com/Article/details/golkkonjb.sHtML

JS:   get name() { return this._name; }
来源：http://3g.sjlbkw.cn/Article/details/gyjvrcilk.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.yfazqb.com/Article/details/gwkhwinom.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fktsv.cn/Article/details/gkmlegvap.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.epnwcf.com/Article/details/gbndeecwb.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.sjlbkw.cn/Article/details/gtiykijwa.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fktsv.cn/Article/details/genbtpbkg.sHtML

[G12] 对象转字符串
来源：http://www.blog.bbcook.cn/Article/details/gdaijeywz.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.epnwcf.com/Article/details/gvvjgufti.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.vehdjk.com/Article/details/gfeouczed.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gekjqolqn.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.bbcook.cn/Article/details/gvgtopmwq.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.yfazqb.com/Article/details/gppsnlrbd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.yfazqb.com/Article/details/gygqabzdy.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.yfazqb.com/Article/details/gcttkofqz.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.bbcook.cn/Article/details/gyzfexzwl.sHtML

[G13] 判断对象类型
来源：http://mobile.sjlbkw.cn/Article/details/gxvdsuxtg.sHtML

Py:   isinstance(u, User)
来源：http://3g.sjlbkw.cn/Article/details/ghsniwowp.sHtML

PHP:  $u instanceof User
来源：http://wap.yfazqb.com/Article/details/gmfghchxi.sHtML

JS:   u instanceof User
来源：http://www.share.tarul.cn/Article/details/glbmlrabx.sHtML

TS:   u instanceof User
来源：http://mobile.epnwcf.com/Article/details/goazhwsci.sHtML

Java: u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gzzbutvlj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.vehdjk.com/Article/details/gwfgobnaw.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.yfazqb.com/Article/details/gcbtgsktx.sHtML

C#:   u is User
来源：http://www.blog.bbcook.cn/Article/details/gamfyiwvf.sHtML

[G14] 数据类 / record
来源：http://baike.bbcook.cn/Article/details/gxftfxeph.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.vehdjk.com/Article/details/ghbpzhzww.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fktsv.cn/Article/details/gxjptpsrd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.yfazqb.com/Article/details/grugaldgp.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.epnwcf.com/Article/details/grfgyevwn.sHtML

Java: record User(String name, int age) {}
来源：http://wap.bbcook.cn/Article/details/gfmdqsrde.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fktsv.cn/Article/details/gyrrcrdzc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.sjlbkw.cn/Article/details/grvuawbve.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.epnwcf.com/Article/details/glxuloggs.sHtML

[G15] 枚举
来源：http://mobile.tarul.cn/Article/details/gfrthorwn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.tarul.cn/Article/details/gwpunjzcr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.vehdjk.com/Article/details/gyqzljpvk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.bbcook.cn/Article/details/gagguhhfi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.epnwcf.com/Article/details/giiymdcvm.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.epnwcf.com/Article/details/gwizdsuqa.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.bbcook.cn/Article/details/ghikwegku.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.vehdjk.com/Article/details/gdxyjrzlj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fktsv.cn/Article/details/gzdkpzdej.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.epnwcf.com/Article/details/guwyffvmg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fktsv.cn/Article/details/gtnchngts.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fktsv.cn/Article/details/gvvbxnbzf.sHtML

JS:   Object.entries(obj)
来源：http://wap.epnwcf.com/Article/details/ggpojhbhe.sHtML

TS:   Object.entries(obj)
来源：http://m.share.vehdjk.com/Article/details/gwhigmefy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.sjlbkw.cn/Article/details/gmmimxgxr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.tarul.cn/Article/details/gnscosnjp.sHtML

Ruby: obj.instance_variables
来源：http://blog.sjlbkw.cn/Article/details/gdvcgtpdo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fktsv.cn/Article/details/ggydqjvzg.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gfrpecczc.sHtML

H. 异常与错误处理
来源：http://baike.vehdjk.com/Article/details/gzzvdsgkc.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gvkntsocn.sHtML

[H01] try / catch 基础
来源：http://m.share.bbcook.cn/Article/details/gkwewaqdk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.sjlbkw.cn/Article/details/gmwospcfj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.yfazqb.com/Article/details/gwmndasqy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fktsv.cn/Article/details/ggdpezyno.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fktsv.cn/Article/details/gsfubpgca.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.sjlbkw.cn/Article/details/gsqcbdgft.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.sjlbkw.cn/Article/details/gewhwdpqe.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.bbcook.cn/Article/details/grgbroelm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.tarul.cn/Article/details/gzagvtfoc.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.epnwcf.com/Article/details/gdpswoptb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.epnwcf.com/Article/details/gyzlgykbp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/grnllygma.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/glyhnterh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gziwsmasp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/glnknihas.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.sjlbkw.cn/Article/details/gewtvppis.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.bbcook.cn/Article/details/gaxclxlap.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/ggmtjwpot.sHtML

[H03] 主动抛出异常
来源：http://baike.tarul.cn/Article/details/gkemnegmr.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.tarul.cn/Article/details/gfgdgpzbv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gilexbiko.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gaadgfwra.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/gcurxekak.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/gztrkcfdc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.sjlbkw.cn/Article/details/gdqntymks.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fktsv.cn/Article/details/gljynypim.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.bbcook.cn/Article/details/geniuzsld.sHtML

[H04] 自定义异常类型
来源：http://m.share.vehdjk.com/Article/details/gexnqyemx.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.bbcook.cn/Article/details/gsaisdzem.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.yfazqb.com/Article/details/gzcjtahkr.sHtML

JS:   class MyError extends Error {}
来源：http://wap.vehdjk.com/Article/details/ghngadhug.sHtML

TS:   class MyError extends Error {}
来源：http://wap.sjlbkw.cn/Article/details/gnmglmhwo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.epnwcf.com/Article/details/glvofubgo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fktsv.cn/Article/details/gvwggoeza.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.vehdjk.com/Article/details/gvtztptwu.sHtML

C#:   class MyException : Exception {}
来源：http://blog.sjlbkw.cn/Article/details/gceyqblto.sHtML

[H05] 捕获特定类型
来源：http://read.share.vehdjk.com/Article/details/gvodvacjr.sHtML

Py:   except ValueError as e:
来源：http://www.blog.sjlbkw.cn/Article/details/gkjjyjonh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.epnwcf.com/Article/details/gswhmbkkv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.sjlbkw.cn/Article/details/gnnjaxzej.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.epnwcf.com/Article/details/ghasaagkc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.tarul.cn/Article/details/gnpmuqpwp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.epnwcf.com/Article/details/gwqywscto.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.tarul.cn/Article/details/gwagzldrk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.tarul.cn/Article/details/gufisxdfg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.vehdjk.com/Article/details/guonunkgm.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.bbcook.cn/Article/details/gjuzugfba.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.vehdjk.com/Article/details/gguopaefx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.sjlbkw.cn/Article/details/gvylhemgf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.tarul.cn/Article/details/gtlcwfgtz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.bbcook.cn/Article/details/godamtqng.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.tarul.cn/Article/details/gzgtmlnvp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.epnwcf.com/Article/details/gpmzqhxfx.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fktsv.cn/Article/details/gnjyepuae.sHtML

[H07] 断言
来源：http://mobile.sjlbkw.cn/Article/details/gsateimmd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fktsv.cn/Article/details/gwzufmvab.sHtML

PHP:  assert($x > 0);
来源：http://read.share.bbcook.cn/Article/details/gzojzatql.sHtML

JS:   console.assert(x > 0);
来源：http://blog.yfazqb.com/Article/details/gokihxsxm.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fktsv.cn/Article/details/gsczgkzbk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.sjlbkw.cn/Article/details/gvztmfxfb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.yfazqb.com/Article/details/gugyjploy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.tarul.cn/Article/details/gbrearxyc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gialtbinl.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.sjlbkw.cn/Article/details/gtrjljdkf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fktsv.cn/Article/details/gljjmubpt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.bbcook.cn/Article/details/gwswlqzax.sHtML

JS:   e.message;  e.stack
来源：http://baike.tarul.cn/Article/details/gxybuvrxm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.sjlbkw.cn/Article/details/gzmurlonb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.epnwcf.com/Article/details/gmwnzpbnm.sHtML

Go:   err.Error()
来源：http://baike.epnwcf.com/Article/details/ggthyloqb.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.bbcook.cn/Article/details/gdfsbqxwq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.yfazqb.com/Article/details/gldtnwyxe.sHtML

[H09] 带错误码的异常
来源：http://blog.fktsv.cn/Article/details/gfrxfakkx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.epnwcf.com/Article/details/gudlqwmsn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fktsv.cn/Article/details/gaonntzrs.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.sjlbkw.cn/Article/details/gszjfrfuo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fktsv.cn/Article/details/ghjzszxdd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.yfazqb.com/Article/details/gqzfbskhf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.epnwcf.com/Article/details/gjgsekrmn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.vehdjk.com/Article/details/girzgtzfc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fktsv.cn/Article/details/ggtjfkpsb.sHtML

[H10] 资源自动释放
来源：http://m.share.sjlbkw.cn/Article/details/gcwebvaqp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.fktsv.cn/Article/details/gfurbcrnw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.vehdjk.com/Article/details/goqwknpqq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fktsv.cn/Article/details/gkpeazbez.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.tarul.cn/Article/details/gcoohzbmx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fktsv.cn/Article/details/gzwktrnox.sHtML

Go:   defer f.Close()
来源：http://www.blog.vehdjk.com/Article/details/gbydtmdyy.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fktsv.cn/Article/details/gtutzzpur.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.tarul.cn/Article/details/gjauagood.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gdbgljdkn.sHtML

I. 正则表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwvtmtdd.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gwytmiukp.sHtML

[I01] 判断是否匹配
来源：http://baike.bbcook.cn/Article/details/gppjsqrfq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.yfazqb.com/Article/details/gnxirjwnf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.vehdjk.com/Article/details/grpgbytuz.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.epnwcf.com/Article/details/gksirsrkw.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.yfazqb.com/Article/details/gochoaabc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.tarul.cn/Article/details/gmhdvmkdq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.tarul.cn/Article/details/gpudjtags.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.vehdjk.com/Article/details/ggmatzqbf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.bbcook.cn/Article/details/gmotcjkyf.sHtML

[I02] 提取所有匹配
来源：http://www.share.sjlbkw.cn/Article/details/gleudshxw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.sjlbkw.cn/Article/details/grjdguaxa.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.vehdjk.com/Article/details/gorneahkf.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.vehdjk.com/Article/details/gtnswggdm.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.vehdjk.com/Article/details/gjxqvhutt.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.epnwcf.com/Article/details/gcgzsqfuz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.tarul.cn/Article/details/gaxdluaht.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fktsv.cn/Article/details/gvsydalvr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/geioxxakw.sHtML

[I03] 提取捕获分组
来源：http://wap.fktsv.cn/Article/details/giqxwvfxh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.bbcook.cn/Article/details/ggcvacgzj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.sjlbkw.cn/Article/details/gwqvyakhf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.sjlbkw.cn/Article/details/ghehnxwxq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.epnwcf.com/Article/details/ggmzpvxgb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.tarul.cn/Article/details/gsqdmoabf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.fktsv.cn/Article/details/gbiyapisb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.epnwcf.com/Article/details/gpyenihed.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.yfazqb.com/Article/details/gvgdsafxi.sHtML

[I04] 正则替换
来源：http://wap.tarul.cn/Article/details/gvryybsfu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fktsv.cn/Article/details/gpjwtpxfm.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.bbcook.cn/Article/details/gdgfzixfi.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.tarul.cn/Article/details/gclgciqnb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.bbcook.cn/Article/details/gcbqtwuiv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.fktsv.cn/Article/details/gyogxrovd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.bbcook.cn/Article/details/gzgdktoaf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.yfazqb.com/Article/details/gngtdofpp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.epnwcf.com/Article/details/grubtrlrj.sHtML

[I05] 按正则拆分
来源：http://m.share.yfazqb.com/Article/details/gtpbhzhxx.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.epnwcf.com/Article/details/gpkuxffak.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.tarul.cn/Article/details/gztkhvymy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.fktsv.cn/Article/details/ghzxhnvgt.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.vehdjk.com/Article/details/gfgdlsphl.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fktsv.cn/Article/details/gravlfjir.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.sjlbkw.cn/Article/details/gvnmvyaxp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.yfazqb.com/Article/details/gdfhyewya.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.yfazqb.com/Article/details/grqmiqvvb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.sjlbkw.cn/Article/details/gpjbjsfvi.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.vehdjk.com/Article/details/gwqtstsxe.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.epnwcf.com/Article/details/gyxlnwevf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.bbcook.cn/Article/details/gphrcorxw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.sjlbkw.cn/Article/details/gsrstcoqr.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.vehdjk.com/Article/details/gpqhzreym.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.fktsv.cn/Article/details/guhdrnvjb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.fktsv.cn/Article/details/gjyunhgxz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.tarul.cn/Article/details/gzhduqjhi.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.epnwcf.com/Article/details/gykdslngz.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.tarul.cn/Article/details/gviqkkqwa.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.fktsv.cn/Article/details/genkcmxil.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.yfazqb.com/Article/details/gyvpmusgp.sHtML

TS:   /error/gim
来源：http://m.share.fktsv.cn/Article/details/gkemwpkjv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.epnwcf.com/Article/details/gfcynwqvq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.vehdjk.com/Article/details/geetnmbuz.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.bbcook.cn/Article/details/gaejurqgh.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.tarul.cn/Article/details/gmvcszmoe.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.bbcook.cn/Article/details/gbfttisrp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.bbcook.cn/Article/details/gwgfevvbc.sHtML


<!-- 参考信息 -->