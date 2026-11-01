代发 wailian999

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/ggayohvic.sHtML

G. 面向对象
来源：http://m.share.epnwcf.com/Article/details/gzomzmjng.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gajcgalht.sHtML

[G01] 定义类
来源：http://3g.bbcook.cn/Article/details/gailxsnmb.sHtML

Py:   class User: pass
来源：http://blog.bbcook.cn/Article/details/gwvvodkql.sHtML

PHP:  class User {}
来源：http://3g.yfazqb.com/Article/details/gphrxmsfi.sHtML

JS:   class User {}
来源：http://baike.sjlbkw.cn/Article/details/gjmmlpnyk.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.tarul.cn/Article/details/gsitabpee.sHtML

Java: class User {}
来源：http://www.m.share.tarul.cn/Article/details/gdbaivnmz.sHtML

Go:   type User struct { Name string }
来源：http://mobile.tarul.cn/Article/details/gfgpgzusn.sHtML

Ruby: class User; end
来源：http://blog.yfazqb.com/Article/details/gvkneroig.sHtML

C#:   class User {}
来源：http://read.share.yfazqb.com/Article/details/gyfdnlvkd.sHtML

[G02] 构造函数
来源：http://baike.sjlbkw.cn/Article/details/gyjmgvebh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fktsv.cn/Article/details/gxsgmkwvh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.yfazqb.com/Article/details/gmwfcgpqc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.bbcook.cn/Article/details/gpotdshdl.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.epnwcf.com/Article/details/gkpnxuiqc.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fktsv.cn/Article/details/gqkhyfbmd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.vehdjk.com/Article/details/gdslimvmw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.tarul.cn/Article/details/gxvgqrasx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fktsv.cn/Article/details/glpyewitq.sHtML

[G03] 实例属性
来源：http://baike.bbcook.cn/Article/details/gbxefgynv.sHtML

Py:   self.name = "x"
来源：http://3g.vehdjk.com/Article/details/gvqyrowwq.sHtML

PHP:  public string $name = "x";
来源：http://m.share.bbcook.cn/Article/details/gimdtbeqr.sHtML

JS:   this.name = "x";
来源：http://3g.tarul.cn/Article/details/gjcyxakzm.sHtML

TS:   name: string = "x";
来源：http://blog.epnwcf.com/Article/details/grkcboira.sHtML

Java: private String name;
来源：http://blog.yfazqb.com/Article/details/gyvxurgwc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.tarul.cn/Article/details/ghkbduyxn.sHtML

Ruby: @name = "x"
来源：http://m.share.fktsv.cn/Article/details/godznvtjr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.epnwcf.com/Article/details/grefzscrr.sHtML

[G04] 定义方法
来源：http://3g.sjlbkw.cn/Article/details/glppdcrwi.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.bbcook.cn/Article/details/gtwhwjvly.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.yfazqb.com/Article/details/gjclockep.sHtML

JS:   greet() { return this.name; }
来源：http://baike.tarul.cn/Article/details/gxyxnawzz.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.yfazqb.com/Article/details/gywvisemf.sHtML

Java: String greet() { return name; }
来源：http://wap.tarul.cn/Article/details/gdrvhqdun.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.yfazqb.com/Article/details/gwbogxevv.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.tarul.cn/Article/details/gvdhbpdbc.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.bbcook.cn/Article/details/gtmeoaoph.sHtML

[G05] 继承
来源：http://wap.bbcook.cn/Article/details/gwbisgnak.sHtML

Py:   class Admin(User): pass
来源：http://blog.tarul.cn/Article/details/gjyqduibs.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gfkqfzeel.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gmdhlkvce.sHtML

TS:   class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/gmsomvtew.sHtML

Java: class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gbbuemivo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.yfazqb.com/Article/details/gkjhchgwg.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fktsv.cn/Article/details/grptktzcf.sHtML

C#:   class Admin : User {}
来源：http://3g.vehdjk.com/Article/details/gynjauozy.sHtML

[G06] 重写方法
来源：http://read.share.tarul.cn/Article/details/ggpbtcrmk.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.vehdjk.com/Article/details/gwqyjgrxk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.tarul.cn/Article/details/geyvmhnlw.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.tarul.cn/Article/details/gjovgaqyc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/gwnvxiquz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/grocntpto.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fktsv.cn/Article/details/glxrhsdvc.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.yfazqb.com/Article/details/glmgtzors.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.epnwcf.com/Article/details/gsfdryuue.sHtML

[G07] 调用父类方法
来源：http://baike.tarul.cn/Article/details/gtooqltqy.sHtML

Py:   super().greet()
来源：http://m.share.vehdjk.com/Article/details/gtbprpyrm.sHtML

PHP:  parent::greet();
来源：http://www.share.bbcook.cn/Article/details/gmwacssau.sHtML

JS:   super.greet();
来源：http://3g.bbcook.cn/Article/details/gteksnucb.sHtML

TS:   super.greet();
来源：http://blog.yfazqb.com/Article/details/gtkqeswiy.sHtML

Java: super.greet();
来源：http://3g.tarul.cn/Article/details/gwreuqahk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.epnwcf.com/Article/details/gqftyqwfb.sHtML

Ruby: super
来源：http://www.share.epnwcf.com/Article/details/gujkkrylq.sHtML

C#:   base.Greet();
来源：http://blog.yfazqb.com/Article/details/ggserqxkf.sHtML

[G08] 静态方法与属性
来源：http://mobile.yfazqb.com/Article/details/gagpsgodn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.epnwcf.com/Article/details/gkcvnsxao.sHtML

PHP:  public static function f() {}
来源：http://m.share.yfazqb.com/Article/details/grjhkdsue.sHtML

JS:   static f() {}
来源：http://m.share.epnwcf.com/Article/details/gkkuworhf.sHtML

TS:   static f(): void {}
来源：http://mobile.sjlbkw.cn/Article/details/glepgkepe.sHtML

Java: static void f() {}
来源：http://blog.tarul.cn/Article/details/gwqoavuyj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.sjlbkw.cn/Article/details/gaphlgcmt.sHtML

Ruby: def self.f; end
来源：http://wap.tarul.cn/Article/details/gipdroyie.sHtML

C#:   public static void F() {}
来源：http://wap.sjlbkw.cn/Article/details/glsehblkx.sHtML

[G09] 接口 / 抽象类
来源：http://blog.epnwcf.com/Article/details/gmepkrgnv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.epnwcf.com/Article/details/gmpuavemo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.sjlbkw.cn/Article/details/gaysmkwcn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.tarul.cn/Article/details/gipkaapku.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.sjlbkw.cn/Article/details/gprwdqfhb.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.sjlbkw.cn/Article/details/gddczxrph.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.tarul.cn/Article/details/gjujrxgxx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.bbcook.cn/Article/details/gakogzvck.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.bbcook.cn/Article/details/gakbpcuea.sHtML

[G10] 访问控制
来源：http://3g.sjlbkw.cn/Article/details/gmrvwtyqm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.yfazqb.com/Article/details/gmaxrirew.sHtML

PHP:  public / protected / private
来源：http://read.share.sjlbkw.cn/Article/details/gujnvkqti.sHtML

JS:   #private 字段；其余公开
来源：http://baike.epnwcf.com/Article/details/gcagbjywa.sHtML

TS:   public / protected / private
来源：http://www.blog.sjlbkw.cn/Article/details/gjwhhykmo.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.vehdjk.com/Article/details/gagyeqvto.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.bbcook.cn/Article/details/gdsxmjezw.sHtML

Ruby: public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/gwoagpeif.sHtML

C#:   public / protected / private / internal
来源：http://www.share.sjlbkw.cn/Article/details/gdivcxupk.sHtML

[G11] getter / setter
来源：http://www.blog.tarul.cn/Article/details/gzlujrrni.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fktsv.cn/Article/details/gwkkwztit.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.tarul.cn/Article/details/gzgbtmusd.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.tarul.cn/Article/details/gdsjjcygb.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.tarul.cn/Article/details/gdrrfzlhf.sHtML

Java: public String getName() { return name; }
来源：http://3g.fktsv.cn/Article/details/gvholsaor.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.tarul.cn/Article/details/gxdhmpjly.sHtML

Ruby: attr_accessor :name
来源：http://www.share.bbcook.cn/Article/details/ggcqcymfe.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.tarul.cn/Article/details/gnztevqxg.sHtML

[G12] 对象转字符串
来源：http://baike.vehdjk.com/Article/details/gtljvlxdt.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.yfazqb.com/Article/details/gxnrktsdf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.sjlbkw.cn/Article/details/gynelgkku.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/getuioteu.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/gmzfntepz.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.epnwcf.com/Article/details/gxizpfbjl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.epnwcf.com/Article/details/glpdiovnf.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.tarul.cn/Article/details/guoklpmpx.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.bbcook.cn/Article/details/ghthxqkfj.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fktsv.cn/Article/details/gedrizvez.sHtML

Py:   isinstance(u, User)
来源：http://3g.bbcook.cn/Article/details/gdluuhjvm.sHtML

PHP:  $u instanceof User
来源：http://www.share.fktsv.cn/Article/details/ggeddlcca.sHtML

JS:   u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gnbmgexnp.sHtML

TS:   u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/ggkxjaizk.sHtML

Java: u instanceof User
来源：http://www.share.fktsv.cn/Article/details/grshzwfhy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fktsv.cn/Article/details/gxlrjooqe.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.tarul.cn/Article/details/gokpbseop.sHtML

C#:   u is User
来源：http://m.share.epnwcf.com/Article/details/gmyjzcxpf.sHtML

[G14] 数据类 / record
来源：http://wap.vehdjk.com/Article/details/gsonscbyu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.yfazqb.com/Article/details/gpmnfoouh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fktsv.cn/Article/details/gmclukhfi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.epnwcf.com/Article/details/guemhygmd.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.vehdjk.com/Article/details/gkkpmnypz.sHtML

Java: record User(String name, int age) {}
来源：http://blog.epnwcf.com/Article/details/goipzbyhp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.yfazqb.com/Article/details/gqcxsjssg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.yfazqb.com/Article/details/gpccohfuu.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.vehdjk.com/Article/details/ggmgzvyyy.sHtML

[G15] 枚举
来源：http://read.share.tarul.cn/Article/details/gydwygrfq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.vehdjk.com/Article/details/ghigrwfez.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fktsv.cn/Article/details/gijxttviq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.epnwcf.com/Article/details/gleygatiy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gypfboyls.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.vehdjk.com/Article/details/guabacnye.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.epnwcf.com/Article/details/gajdhveen.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.bbcook.cn/Article/details/ghxabtucs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.vehdjk.com/Article/details/gegdrsjnu.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.yfazqb.com/Article/details/gvsbxlrel.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.tarul.cn/Article/details/gcmkwvhxn.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.vehdjk.com/Article/details/gvsschkfe.sHtML

JS:   Object.entries(obj)
来源：http://3g.tarul.cn/Article/details/gxhaygzln.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.bbcook.cn/Article/details/gruvgofba.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.bbcook.cn/Article/details/gvtfwluns.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.yfazqb.com/Article/details/gbjmkachq.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.sjlbkw.cn/Article/details/goymixkfr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fktsv.cn/Article/details/gvxezntqr.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gbiiughls.sHtML

H. 异常与错误处理
来源：http://read.share.vehdjk.com/Article/details/gpddachvo.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gmailunsp.sHtML

[H01] try / catch 基础
来源：http://www.share.fktsv.cn/Article/details/gtcntvrgv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.sjlbkw.cn/Article/details/gnostrred.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.vehdjk.com/Article/details/govnuvzka.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.yfazqb.com/Article/details/gvndqozwz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fktsv.cn/Article/details/gssrxjopz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fktsv.cn/Article/details/gssozvbih.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.yfazqb.com/Article/details/gmwxctxmi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.bbcook.cn/Article/details/gnuqifurg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.sjlbkw.cn/Article/details/gboutlnqp.sHtML

[H02] finally / ensure 收尾
来源：http://baike.tarul.cn/Article/details/gslwllwzd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.bbcook.cn/Article/details/gbxbgvgwt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gibznhxgp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gpoxjqzme.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/grlabezzz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gdowyplsy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.vehdjk.com/Article/details/grqcqtdwn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.bbcook.cn/Article/details/gqrlptvyu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfgvvweca.sHtML

[H03] 主动抛出异常
来源：http://wap.bbcook.cn/Article/details/gmcldggzb.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.bbcook.cn/Article/details/gkqmlzpfu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/geyskxwog.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gupotcyxi.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gdvhwzbdy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gzxjwhcke.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.epnwcf.com/Article/details/gvraxgcwv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.vehdjk.com/Article/details/gkvmhjwdj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.tarul.cn/Article/details/gvbkiibmk.sHtML

[H04] 自定义异常类型
来源：http://m.share.fktsv.cn/Article/details/gciufsccv.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.yfazqb.com/Article/details/gqctgosqf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fktsv.cn/Article/details/gletcvmhe.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.yfazqb.com/Article/details/gihmoojyg.sHtML

TS:   class MyError extends Error {}
来源：http://blog.bbcook.cn/Article/details/guccquqaw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.tarul.cn/Article/details/giexmftir.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.tarul.cn/Article/details/gddakoouh.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.sjlbkw.cn/Article/details/girwqysat.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.epnwcf.com/Article/details/gegwtkclj.sHtML

[H05] 捕获特定类型
来源：http://blog.bbcook.cn/Article/details/gkaadtnyj.sHtML

Py:   except ValueError as e:
来源：http://m.share.sjlbkw.cn/Article/details/gvdsvqeex.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.tarul.cn/Article/details/glhsydxah.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fktsv.cn/Article/details/gaiirrkeq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.sjlbkw.cn/Article/details/gncucxuiu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.vehdjk.com/Article/details/gosozsyqf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.sjlbkw.cn/Article/details/gpumxjrzg.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.vehdjk.com/Article/details/glizavafp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.yfazqb.com/Article/details/gdalqvtyu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.bbcook.cn/Article/details/gsqmpbffu.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.vehdjk.com/Article/details/gublkzaqv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.bbcook.cn/Article/details/gmhscwibn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.sjlbkw.cn/Article/details/getidnger.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.bbcook.cn/Article/details/glmmhsvjd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.tarul.cn/Article/details/gtptzzgus.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.tarul.cn/Article/details/gowwuxowr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.sjlbkw.cn/Article/details/gsnwtekrn.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.bbcook.cn/Article/details/gybtdjmim.sHtML

[H07] 断言
来源：http://read.share.sjlbkw.cn/Article/details/gtiejcqoq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.epnwcf.com/Article/details/grsdnkzlz.sHtML

PHP:  assert($x > 0);
来源：http://3g.bbcook.cn/Article/details/gyfbljreg.sHtML

JS:   console.assert(x > 0);
来源：http://wap.yfazqb.com/Article/details/gxxmmjyqv.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmnjdmko.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.epnwcf.com/Article/details/gllplnnam.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.epnwcf.com/Article/details/gjbopdrpx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.bbcook.cn/Article/details/gxfkfnhyp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fktsv.cn/Article/details/gsfqhfxcr.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.bbcook.cn/Article/details/gnbjgflth.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.vehdjk.com/Article/details/gutfhsvtu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.yfazqb.com/Article/details/gvlwtluxc.sHtML

JS:   e.message;  e.stack
来源：http://www.share.bbcook.cn/Article/details/gfrfyknmm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.epnwcf.com/Article/details/gacnhebax.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.yfazqb.com/Article/details/gnfsyqoxk.sHtML

Go:   err.Error()
来源：http://wap.bbcook.cn/Article/details/gbevlwvbe.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.yfazqb.com/Article/details/gnwudewhz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.sjlbkw.cn/Article/details/gtgfnrnhy.sHtML

[H09] 带错误码的异常
来源：http://www.share.fktsv.cn/Article/details/ghyclbncf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.sjlbkw.cn/Article/details/ggbhlvmfs.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.tarul.cn/Article/details/glhpmehut.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fktsv.cn/Article/details/gasebrloi.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.yfazqb.com/Article/details/gmdjfuqal.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.yfazqb.com/Article/details/gfxbcfyad.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.epnwcf.com/Article/details/gmjehyhsi.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.tarul.cn/Article/details/grmozjinh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.bbcook.cn/Article/details/ggieskzzx.sHtML

[H10] 资源自动释放
来源：http://wap.fktsv.cn/Article/details/gcvptddeq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.bbcook.cn/Article/details/gvuphdkum.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.epnwcf.com/Article/details/ghhmoonsd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.yfazqb.com/Article/details/gvnoodisj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.sjlbkw.cn/Article/details/gntauabuf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.epnwcf.com/Article/details/gjefsxvdg.sHtML

Go:   defer f.Close()
来源：http://blog.vehdjk.com/Article/details/gloxudkjo.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.tarul.cn/Article/details/gfyijtcef.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fktsv.cn/Article/details/gqezkncnn.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gpyqaplfa.sHtML

I. 正则表达式
来源：http://blog.yfazqb.com/Article/details/gerdieniu.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gsewtxpwx.sHtML

[I01] 判断是否匹配
来源：http://wap.bbcook.cn/Article/details/gqdhjapqt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.vehdjk.com/Article/details/gkvrlkkrd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.fktsv.cn/Article/details/gxkbzhjlb.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.tarul.cn/Article/details/gqxdewyea.sHtML

TS:   /\d+/.test(s)
来源：http://wap.sjlbkw.cn/Article/details/gklluikru.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.vehdjk.com/Article/details/gviddhkas.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.yfazqb.com/Article/details/gdohnuojk.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.fktsv.cn/Article/details/gljiacvei.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.tarul.cn/Article/details/gifgybwaa.sHtML

[I02] 提取所有匹配
来源：http://wap.yfazqb.com/Article/details/gfmuvivbp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.bbcook.cn/Article/details/gfnklbtib.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.epnwcf.com/Article/details/gxkwoiyaw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.sjlbkw.cn/Article/details/garwvopun.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.bbcook.cn/Article/details/gbxyhxukh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fktsv.cn/Article/details/gqanlpsru.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fktsv.cn/Article/details/grtmqgjbh.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.epnwcf.com/Article/details/gwtoldjxh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gvduqiigt.sHtML

[I03] 提取捕获分组
来源：http://www.share.yfazqb.com/Article/details/gwnqjxthb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.sjlbkw.cn/Article/details/guqafjgmo.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.bbcook.cn/Article/details/gciurhllf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.vehdjk.com/Article/details/gnamtnzgv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.bbcook.cn/Article/details/gyxmukhqn.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fktsv.cn/Article/details/gbwnpplnj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.vehdjk.com/Article/details/goclqycqy.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.fktsv.cn/Article/details/grqvvxavv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.fktsv.cn/Article/details/gpjkluqgs.sHtML

[I04] 正则替换
来源：http://wap.vehdjk.com/Article/details/ggobwklqb.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.epnwcf.com/Article/details/gchpgemqb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.yfazqb.com/Article/details/gfzpyjhkh.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.epnwcf.com/Article/details/gzyheskui.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.sjlbkw.cn/Article/details/gdyibdogo.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.tarul.cn/Article/details/gzjzcmcdx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.bbcook.cn/Article/details/gfdurswri.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.tarul.cn/Article/details/ghlhiswcm.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.vehdjk.com/Article/details/gmxbwhykz.sHtML

[I05] 按正则拆分
来源：http://www.m.share.sjlbkw.cn/Article/details/grxftfcyg.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.bbcook.cn/Article/details/gsoaligua.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gfzerfkib.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.yfazqb.com/Article/details/gehrzeeep.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.bbcook.cn/Article/details/gxfhslyhz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.fktsv.cn/Article/details/gzzenxswz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.bbcook.cn/Article/details/gtlxelexl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.bbcook.cn/Article/details/gvpbmbuhc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.tarul.cn/Article/details/gninwvflp.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.sjlbkw.cn/Article/details/gpacripfb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.sjlbkw.cn/Article/details/glaweqmmh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.tarul.cn/Article/details/gyqwiwyxi.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.bbcook.cn/Article/details/gxsexerud.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.sjlbkw.cn/Article/details/giomycbxm.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.sjlbkw.cn/Article/details/grmyzhszr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.vehdjk.com/Article/details/gtueuuliq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.sjlbkw.cn/Article/details/gqzqofdzz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.sjlbkw.cn/Article/details/gjcpsjtkj.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.sjlbkw.cn/Article/details/gcyetaclc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.bbcook.cn/Article/details/gqhhgbnne.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.fktsv.cn/Article/details/gkyzlhdqv.sHtML


<!-- 参考信息 -->