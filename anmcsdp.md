代发 wailian999

Java: class User {}
来源：http://baike.vehdjk.com/Article/details/ggksrgvor.sHtML

Go:   type User struct { Name string }
来源：http://wap.sjlbkw.cn/Article/details/gtybuwjjz.sHtML

Ruby: class User; end
来源：http://www.m.share.fktsv.cn/Article/details/gxwskabej.sHtML

C#:   class User {}
来源：http://read.share.bbcook.cn/Article/details/gvduaapuf.sHtML

[G02] 构造函数
来源：http://mobile.sjlbkw.cn/Article/details/gewwmbhpy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.sjlbkw.cn/Article/details/gjmqhhdei.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gnoiooeok.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.tarul.cn/Article/details/gqgixbfnf.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.sjlbkw.cn/Article/details/gtferqrta.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.vehdjk.com/Article/details/gdajzkkcz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.yfazqb.com/Article/details/gsrwvztju.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.vehdjk.com/Article/details/gnklikxeb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkyrayipd.sHtML

[G03] 实例属性
来源：http://read.share.yfazqb.com/Article/details/guctmfoal.sHtML

Py:   self.name = "x"
来源：http://wap.vehdjk.com/Article/details/gxkpyzznh.sHtML

PHP:  public string $name = "x";
来源：http://blog.vehdjk.com/Article/details/ghbvuupip.sHtML

JS:   this.name = "x";
来源：http://3g.vehdjk.com/Article/details/glrlekfyl.sHtML

TS:   name: string = "x";
来源：http://www.m.share.tarul.cn/Article/details/gczmfafbs.sHtML

Java: private String name;
来源：http://www.blog.tarul.cn/Article/details/glhigfojr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.tarul.cn/Article/details/gmdpnmaxg.sHtML

Ruby: @name = "x"
来源：http://m.share.tarul.cn/Article/details/gvqtvfuse.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.tarul.cn/Article/details/gwcrqpnki.sHtML

[G04] 定义方法
来源：http://m.share.tarul.cn/Article/details/gnoifyeya.sHtML

Py:   def greet(self): return self.name
来源：http://blog.epnwcf.com/Article/details/gkgygoocx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fktsv.cn/Article/details/gcznlqsgy.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.epnwcf.com/Article/details/ggtkayqem.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.yfazqb.com/Article/details/gkhyqmkvi.sHtML

Java: String greet() { return name; }
来源：http://wap.epnwcf.com/Article/details/ggchvelja.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/gedaklwuu.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.vehdjk.com/Article/details/gsgcsgwmq.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.vehdjk.com/Article/details/gsgmxpqea.sHtML

[G05] 继承
来源：http://m.share.yfazqb.com/Article/details/gkzflfhbz.sHtML

Py:   class Admin(User): pass
来源：http://baike.epnwcf.com/Article/details/gofzqegvd.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.vehdjk.com/Article/details/gdnwjfagi.sHtML

JS:   class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/gjudtfdyc.sHtML

TS:   class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/ghgfosbgt.sHtML

Java: class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/ghndxyumm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.bbcook.cn/Article/details/gbzawnbqt.sHtML

Ruby: class Admin < User; end
来源：http://m.share.vehdjk.com/Article/details/gjnaovmzi.sHtML

C#:   class Admin : User {}
来源：http://wap.bbcook.cn/Article/details/gudfmlnxw.sHtML

[G06] 重写方法
来源：http://baike.tarul.cn/Article/details/gbqyggbgz.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.vehdjk.com/Article/details/gxntmczzi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/gbynojdte.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gzmtkthhj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/gddsiaowd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/gbzvdwdhu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.epnwcf.com/Article/details/grbohnupm.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.bbcook.cn/Article/details/gxaayiyxn.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fktsv.cn/Article/details/gvqoujfic.sHtML

[G07] 调用父类方法
来源：http://3g.fktsv.cn/Article/details/gpckbgbeo.sHtML

Py:   super().greet()
来源：http://wap.bbcook.cn/Article/details/gvzbqxxxd.sHtML

PHP:  parent::greet();
来源：http://www.share.vehdjk.com/Article/details/gjlbqdxdq.sHtML

JS:   super.greet();
来源：http://www.share.sjlbkw.cn/Article/details/glxbogfay.sHtML

TS:   super.greet();
来源：http://baike.yfazqb.com/Article/details/gyeqdzaha.sHtML

Java: super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gyswanuod.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.yfazqb.com/Article/details/gzolqjvfd.sHtML

Ruby: super
来源：http://www.m.share.bbcook.cn/Article/details/gjmjzdglf.sHtML

C#:   base.Greet();
来源：http://www.share.tarul.cn/Article/details/gbzysqdzk.sHtML

[G08] 静态方法与属性
来源：http://read.share.sjlbkw.cn/Article/details/gpnykkdrc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fktsv.cn/Article/details/gpcfaqfbp.sHtML

PHP:  public static function f() {}
来源：http://www.share.epnwcf.com/Article/details/gerdayeok.sHtML

JS:   static f() {}
来源：http://m.share.tarul.cn/Article/details/ggjdvbzjh.sHtML

TS:   static f(): void {}
来源：http://mobile.vehdjk.com/Article/details/gaizuwxbp.sHtML

Java: static void f() {}
来源：http://www.blog.epnwcf.com/Article/details/gjsqfqfcu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.epnwcf.com/Article/details/gdeoqqxmb.sHtML

Ruby: def self.f; end
来源：http://3g.vehdjk.com/Article/details/gzohckzip.sHtML

C#:   public static void F() {}
来源：http://wap.sjlbkw.cn/Article/details/gxzophwgt.sHtML

[G09] 接口 / 抽象类
来源：http://3g.tarul.cn/Article/details/gpzuzrugv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.vehdjk.com/Article/details/gduoukumq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.bbcook.cn/Article/details/gwnrwjbwr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fktsv.cn/Article/details/gxfwgzxix.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.vehdjk.com/Article/details/guqaypjrl.sHtML

Java: interface Shape { double area(); }
来源：http://wap.yfazqb.com/Article/details/gyyfkhxjp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.tarul.cn/Article/details/gbrbhvmsw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.epnwcf.com/Article/details/gawtouuix.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.epnwcf.com/Article/details/gkxksevvt.sHtML

[G10] 访问控制
来源：http://baike.bbcook.cn/Article/details/givlmrwse.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.sjlbkw.cn/Article/details/gixgupeay.sHtML

PHP:  public / protected / private
来源：http://read.share.yfazqb.com/Article/details/gvbfmunbn.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fktsv.cn/Article/details/ggqrtqhzi.sHtML

TS:   public / protected / private
来源：http://3g.epnwcf.com/Article/details/gcuchsbzg.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.vehdjk.com/Article/details/guffthwgo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fktsv.cn/Article/details/gthhihdvk.sHtML

Ruby: public / protected / private
来源：http://www.share.vehdjk.com/Article/details/gciiiebcs.sHtML

C#:   public / protected / private / internal
来源：http://blog.tarul.cn/Article/details/gpjcshpyn.sHtML

[G11] getter / setter
来源：http://m.share.epnwcf.com/Article/details/gbcovlrsf.sHtML

Py:   @property 与 @x.setter
来源：http://3g.sjlbkw.cn/Article/details/gjqyrfixw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.sjlbkw.cn/Article/details/gwsfoncbi.sHtML

JS:   get name() { return this._name; }
来源：http://wap.bbcook.cn/Article/details/gcfxkpsky.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.sjlbkw.cn/Article/details/gfpyezcmz.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fktsv.cn/Article/details/gtowtzeqj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.tarul.cn/Article/details/gbxrjheet.sHtML

Ruby: attr_accessor :name
来源：http://3g.yfazqb.com/Article/details/gfpuoqrue.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.tarul.cn/Article/details/gqmesioef.sHtML

[G12] 对象转字符串
来源：http://www.share.fktsv.cn/Article/details/gqbyiwlrh.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fktsv.cn/Article/details/gvujuaisb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gtvxtovjw.sHtML

JS:   toString() { return this.name; }
来源：http://3g.tarul.cn/Article/details/gbjrbbzrq.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.yfazqb.com/Article/details/geajnwsyv.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gtyurdmqd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.yfazqb.com/Article/details/gwxleptbr.sHtML

Ruby: def to_s; @name; end
来源：http://wap.tarul.cn/Article/details/gidkzewlz.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fktsv.cn/Article/details/gynmbbaeq.sHtML

[G13] 判断对象类型
来源：http://www.blog.vehdjk.com/Article/details/gmnmueugi.sHtML

Py:   isinstance(u, User)
来源：http://read.share.sjlbkw.cn/Article/details/gygtajzxj.sHtML

PHP:  $u instanceof User
来源：http://www.share.epnwcf.com/Article/details/gizwdibxl.sHtML

JS:   u instanceof User
来源：http://read.share.vehdjk.com/Article/details/grtdyetkv.sHtML

TS:   u instanceof User
来源：http://m.share.vehdjk.com/Article/details/gdggwtgve.sHtML

Java: u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gqnjupibw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.sjlbkw.cn/Article/details/gfapwfxnj.sHtML

Ruby: u.is_a?(User)
来源：http://baike.bbcook.cn/Article/details/godgocieh.sHtML

C#:   u is User
来源：http://www.blog.yfazqb.com/Article/details/gkcujvwef.sHtML

[G14] 数据类 / record
来源：http://m.share.epnwcf.com/Article/details/gadwaxqtm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.yfazqb.com/Article/details/gyqwzzwte.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fktsv.cn/Article/details/gvukbdvpr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.tarul.cn/Article/details/gbskufyji.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fktsv.cn/Article/details/gkzzjqwaj.sHtML

Java: record User(String name, int age) {}
来源：http://blog.sjlbkw.cn/Article/details/gacljqfbt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.epnwcf.com/Article/details/gdggsaosm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.bbcook.cn/Article/details/gyrzylmyx.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.bbcook.cn/Article/details/gtyynupxj.sHtML

[G15] 枚举
来源：http://www.m.share.epnwcf.com/Article/details/grwrtfzih.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.tarul.cn/Article/details/gpafwbgau.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.yfazqb.com/Article/details/gqzsfjtpo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.tarul.cn/Article/details/gwfwkqbtw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.tarul.cn/Article/details/gclkvdpyl.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.vehdjk.com/Article/details/glojojszd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.vehdjk.com/Article/details/gvzjqakrw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fktsv.cn/Article/details/glprytykj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fktsv.cn/Article/details/gibngacih.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.epnwcf.com/Article/details/gcqimvhco.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.yfazqb.com/Article/details/gvhyxkjtm.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fktsv.cn/Article/details/gyljaisog.sHtML

JS:   Object.entries(obj)
来源：http://baike.epnwcf.com/Article/details/ggvvstgzi.sHtML

TS:   Object.entries(obj)
来源：http://baike.vehdjk.com/Article/details/gxxzgmnto.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.vehdjk.com/Article/details/glmgucflt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.bbcook.cn/Article/details/grqvlxush.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.bbcook.cn/Article/details/gsdqozpin.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.tarul.cn/Article/details/giyqsdmov.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gocivlzxd.sHtML

H. 异常与错误处理
来源：http://m.share.epnwcf.com/Article/details/gwlwrlstg.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/ghezipzba.sHtML

[H01] try / catch 基础
来源：http://mobile.tarul.cn/Article/details/gktnckizi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.bbcook.cn/Article/details/gsqifqiho.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.yfazqb.com/Article/details/ggttmgseb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.vehdjk.com/Article/details/genxfkvit.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbxqdrjg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.bbcook.cn/Article/details/gpastmilr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fktsv.cn/Article/details/gevwwpphe.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.sjlbkw.cn/Article/details/grklzdicl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.epnwcf.com/Article/details/gxeakyefz.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fktsv.cn/Article/details/gxszakkxv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.vehdjk.com/Article/details/geedstgvs.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gtsstglow.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.epnwcf.com/Article/details/gkxjcfqnn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/gwrziuvsu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gyjwcxyyt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.sjlbkw.cn/Article/details/gpxaevwdo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.epnwcf.com/Article/details/glvfoniei.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gnebiwwkl.sHtML

[H03] 主动抛出异常
来源：http://www.share.fktsv.cn/Article/details/ghmqzuwng.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.epnwcf.com/Article/details/gglhytdab.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gvwbtwilt.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gphrktbyy.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.vehdjk.com/Article/details/ghounhtvp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.vehdjk.com/Article/details/gcttcteir.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.sjlbkw.cn/Article/details/guhyoqmhl.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fktsv.cn/Article/details/gkqwfhnwm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fktsv.cn/Article/details/goicftmwa.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fktsv.cn/Article/details/gsdroociz.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.tarul.cn/Article/details/gxklwckrq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.epnwcf.com/Article/details/gcimkfewg.sHtML

JS:   class MyError extends Error {}
来源：http://baike.bbcook.cn/Article/details/ggfhrmata.sHtML

TS:   class MyError extends Error {}
来源：http://blog.vehdjk.com/Article/details/ghwavtyvk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.tarul.cn/Article/details/giyblzdkn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.tarul.cn/Article/details/gayiyndlq.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.bbcook.cn/Article/details/gazslytrr.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fktsv.cn/Article/details/gapceflfh.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.epnwcf.com/Article/details/gjypggoza.sHtML

Py:   except ValueError as e:
来源：http://read.share.bbcook.cn/Article/details/grsyhdvtx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.sjlbkw.cn/Article/details/gagvllnoq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.epnwcf.com/Article/details/gfbqfmahd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.yfazqb.com/Article/details/gfgqzqgia.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.tarul.cn/Article/details/ggkrwgjro.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fktsv.cn/Article/details/gdekqbpmx.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjwwblws.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.bbcook.cn/Article/details/grjoflrvw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.vehdjk.com/Article/details/gcyqxzkty.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.vehdjk.com/Article/details/gbeaagdyf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.sjlbkw.cn/Article/details/gizbbqkrk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.bbcook.cn/Article/details/gwgfbzlqm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.sjlbkw.cn/Article/details/gnmwidobi.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fktsv.cn/Article/details/gqnyynzkh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.tarul.cn/Article/details/gwvinzlng.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.vehdjk.com/Article/details/gqjdaezqv.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.yfazqb.com/Article/details/gfqupvttz.sHtML

[H07] 断言
来源：http://wap.tarul.cn/Article/details/gsuwbposg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fktsv.cn/Article/details/glkkjawfy.sHtML

PHP:  assert($x > 0);
来源：http://m.share.epnwcf.com/Article/details/gcmnvufzp.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.bbcook.cn/Article/details/gekomxvtx.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.tarul.cn/Article/details/gnabgnckg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.epnwcf.com/Article/details/gyygwldlp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.bbcook.cn/Article/details/gjqjtnkca.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.sjlbkw.cn/Article/details/gaveypjfw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.yfazqb.com/Article/details/gmyalcgkw.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fktsv.cn/Article/details/gwvefloqj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.vehdjk.com/Article/details/gidulfdar.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.bbcook.cn/Article/details/gvxeffpbc.sHtML

JS:   e.message;  e.stack
来源：http://3g.fktsv.cn/Article/details/gaosreclc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.tarul.cn/Article/details/girljbfjt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.sjlbkw.cn/Article/details/gjlkvkrgs.sHtML

Go:   err.Error()
来源：http://m.share.yfazqb.com/Article/details/gghzeoiwl.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.bbcook.cn/Article/details/gokjnaiom.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.sjlbkw.cn/Article/details/gvxxkxveh.sHtML

[H09] 带错误码的异常
来源：http://baike.fktsv.cn/Article/details/gqcxnwect.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.epnwcf.com/Article/details/gelkayeph.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.sjlbkw.cn/Article/details/gfozxxusi.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.vehdjk.com/Article/details/gifujozzn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.bbcook.cn/Article/details/gqinfxgmq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbrnraist.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.sjlbkw.cn/Article/details/gpqrttvxg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.sjlbkw.cn/Article/details/gxfhkoktp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.sjlbkw.cn/Article/details/gqzwkgrlp.sHtML

[H10] 资源自动释放
来源：http://m.share.bbcook.cn/Article/details/gtsgvbmow.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.bbcook.cn/Article/details/gzzzsuzeh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.bbcook.cn/Article/details/gpxrlthdb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fktsv.cn/Article/details/grqoyukib.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.tarul.cn/Article/details/gxmispgsn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.vehdjk.com/Article/details/gqkuecmto.sHtML

Go:   defer f.Close()
来源：http://www.share.tarul.cn/Article/details/gxqjspktq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.sjlbkw.cn/Article/details/ghtyqljzd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gwzpayxwx.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gwikvmmgh.sHtML

I. 正则表达式
来源：http://read.share.vehdjk.com/Article/details/gyrnxbxfq.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gmasdidaf.sHtML

[I01] 判断是否匹配
来源：http://read.share.tarul.cn/Article/details/ghshpgxds.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.yfazqb.com/Article/details/glwbeilwe.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.vehdjk.com/Article/details/gejieozdd.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.sjlbkw.cn/Article/details/gyytfxfqr.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.fktsv.cn/Article/details/gikkmxpqc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.bbcook.cn/Article/details/gwoxbafop.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.yfazqb.com/Article/details/gyhufksgu.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.epnwcf.com/Article/details/gpewpulmb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.bbcook.cn/Article/details/gtiwjtqci.sHtML

[I02] 提取所有匹配
来源：http://mobile.epnwcf.com/Article/details/glkexzrgg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fktsv.cn/Article/details/gjedqtsdg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.sjlbkw.cn/Article/details/gfnikyljl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.vehdjk.com/Article/details/gipfqnpvp.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.yfazqb.com/Article/details/gidbozesy.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.epnwcf.com/Article/details/gqojfdfqa.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.sjlbkw.cn/Article/details/ggybqtowu.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.epnwcf.com/Article/details/gssqlyfao.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gauslbfnm.sHtML

[I03] 提取捕获分组
来源：http://blog.bbcook.cn/Article/details/ghhnsbbiv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.epnwcf.com/Article/details/ghgwxkrvo.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.vehdjk.com/Article/details/gurvxlgfw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.yfazqb.com/Article/details/gsbezmjgn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.vehdjk.com/Article/details/gajzknlkh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.yfazqb.com/Article/details/gcbowjjln.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.sjlbkw.cn/Article/details/gebjfgtaq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.yfazqb.com/Article/details/gqyacrnkd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.bbcook.cn/Article/details/gelfqdrdi.sHtML

[I04] 正则替换
来源：http://m.share.vehdjk.com/Article/details/gyvoqamlw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.yfazqb.com/Article/details/gewodcpka.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.vehdjk.com/Article/details/gdublahkf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.yfazqb.com/Article/details/gcuvjgkys.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.tarul.cn/Article/details/gxdhivboo.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.bbcook.cn/Article/details/gsxadircf.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.fktsv.cn/Article/details/gglcojswe.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.bbcook.cn/Article/details/gatlbajex.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fktsv.cn/Article/details/gubqgdxrf.sHtML

[I05] 按正则拆分
来源：http://blog.bbcook.cn/Article/details/glqwbhyhe.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.yfazqb.com/Article/details/grcnoybie.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.yfazqb.com/Article/details/gyzezcydi.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.fktsv.cn/Article/details/gkqtzmcat.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.bbcook.cn/Article/details/gbmezblbo.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.yfazqb.com/Article/details/gwdkthqiu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.fktsv.cn/Article/details/gutndjybj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.yfazqb.com/Article/details/gxcgskeum.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.vehdjk.com/Article/details/gozsrshfe.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.vehdjk.com/Article/details/gimcsfbwl.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.bbcook.cn/Article/details/gxcbzlfxl.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.fktsv.cn/Article/details/gsxcihdmn.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fktsv.cn/Article/details/gmntgvhtw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.tarul.cn/Article/details/grzswbani.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.vehdjk.com/Article/details/ginexshyp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.bbcook.cn/Article/details/gvcmsvcky.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.bbcook.cn/Article/details/gqvgkcbfb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.sjlbkw.cn/Article/details/gkdbuqcee.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.sjlbkw.cn/Article/details/grxnvlqqm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.fktsv.cn/Article/details/gdwklflbn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtpcljlux.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.epnwcf.com/Article/details/getqccgjs.sHtML

TS:   /error/gim
来源：http://www.m.share.vehdjk.com/Article/details/gvlcqlmex.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.vehdjk.com/Article/details/galgfvwgr.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.sjlbkw.cn/Article/details/gyfuhyszi.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.tarul.cn/Article/details/grgfwggoq.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.fktsv.cn/Article/details/gdiepwawb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.sjlbkw.cn/Article/details/gklfixfol.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.bbcook.cn/Article/details/gqwxawagn.sHtML


<!-- 参考信息 -->