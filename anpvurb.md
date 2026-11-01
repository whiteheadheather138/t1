代发 wailian999

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gduzjnojo.sHtML

G. 面向对象
来源：http://mobile.yfazqb.com/Article/details/ggamazeyx.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/guzzzwvwu.sHtML

[G01] 定义类
来源：http://www.m.share.yfazqb.com/Article/details/gvqwgvicp.sHtML

Py:   class User: pass
来源：http://m.share.vehdjk.com/Article/details/gvismlcuv.sHtML

PHP:  class User {}
来源：http://read.share.bbcook.cn/Article/details/gpmfbwpzc.sHtML

JS:   class User {}
来源：http://www.share.bbcook.cn/Article/details/gkxsrmhwl.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.bbcook.cn/Article/details/gaktgtlpu.sHtML

Java: class User {}
来源：http://m.share.vehdjk.com/Article/details/gvdkusuje.sHtML

Go:   type User struct { Name string }
来源：http://www.share.epnwcf.com/Article/details/gnpxwzzda.sHtML

Ruby: class User; end
来源：http://mobile.fktsv.cn/Article/details/gfqnivdxs.sHtML

C#:   class User {}
来源：http://wap.sjlbkw.cn/Article/details/gxvmnknqj.sHtML

[G02] 构造函数
来源：http://mobile.fktsv.cn/Article/details/grqulfatk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fktsv.cn/Article/details/gzsgkcwus.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.yfazqb.com/Article/details/grwdccgwc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fktsv.cn/Article/details/gjwxxaetq.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.sjlbkw.cn/Article/details/gdqwvxtrc.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fktsv.cn/Article/details/gjyjoismb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.bbcook.cn/Article/details/gvqxfbwsv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.tarul.cn/Article/details/gtnusmkba.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fktsv.cn/Article/details/gbybslnog.sHtML

[G03] 实例属性
来源：http://3g.fktsv.cn/Article/details/gfidnuizd.sHtML

Py:   self.name = "x"
来源：http://3g.sjlbkw.cn/Article/details/gplhlfdbu.sHtML

PHP:  public string $name = "x";
来源：http://baike.tarul.cn/Article/details/gpjppcjix.sHtML

JS:   this.name = "x";
来源：http://www.share.bbcook.cn/Article/details/gnpjvrhck.sHtML

TS:   name: string = "x";
来源：http://read.share.tarul.cn/Article/details/gqvfogjaa.sHtML

Java: private String name;
来源：http://mobile.tarul.cn/Article/details/gatfrnheo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.epnwcf.com/Article/details/gyoppnass.sHtML

Ruby: @name = "x"
来源：http://mobile.yfazqb.com/Article/details/gmwglztvw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fktsv.cn/Article/details/gtrjmuyti.sHtML

[G04] 定义方法
来源：http://mobile.fktsv.cn/Article/details/guoeyvvwk.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.vehdjk.com/Article/details/gatyjditl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/gjhibelsq.sHtML

JS:   greet() { return this.name; }
来源：http://baike.epnwcf.com/Article/details/gumoigevy.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.vehdjk.com/Article/details/garzgphwj.sHtML

Java: String greet() { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gqkyiqkmq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/gwwowngvl.sHtML

Ruby: def greet; @name; end
来源：http://3g.epnwcf.com/Article/details/gxqmwvyor.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.yfazqb.com/Article/details/gvvyecnfl.sHtML

[G05] 继承
来源：http://wap.epnwcf.com/Article/details/gbyurqhik.sHtML

Py:   class Admin(User): pass
来源：http://blog.fktsv.cn/Article/details/gfyrxzqzk.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/gtvhbudyv.sHtML

JS:   class Admin extends User {}
来源：http://www.share.vehdjk.com/Article/details/gxdvhfpsu.sHtML

TS:   class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gugasxjdu.sHtML

Java: class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/gtwtrmxoi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.bbcook.cn/Article/details/ghmfgxujp.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.yfazqb.com/Article/details/gduglcxtl.sHtML

C#:   class Admin : User {}
来源：http://m.share.fktsv.cn/Article/details/goamtejbp.sHtML

[G06] 重写方法
来源：http://www.blog.tarul.cn/Article/details/gcrqveeoz.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.epnwcf.com/Article/details/gqkhsngow.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/gblqjzocx.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/gzfyxryyr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.tarul.cn/Article/details/gapavlxxn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/gusqcwfhh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.bbcook.cn/Article/details/gjmzawjiv.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.vehdjk.com/Article/details/gkzxrtded.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fktsv.cn/Article/details/gmlpivogv.sHtML

[G07] 调用父类方法
来源：http://mobile.tarul.cn/Article/details/glvljilda.sHtML

Py:   super().greet()
来源：http://3g.epnwcf.com/Article/details/gcqqhjpmc.sHtML

PHP:  parent::greet();
来源：http://read.share.epnwcf.com/Article/details/giqpejgfv.sHtML

JS:   super.greet();
来源：http://mobile.tarul.cn/Article/details/govkvgucv.sHtML

TS:   super.greet();
来源：http://3g.vehdjk.com/Article/details/ggjumkcvp.sHtML

Java: super.greet();
来源：http://m.share.fktsv.cn/Article/details/ggmtahofq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.bbcook.cn/Article/details/gnzyzqtdp.sHtML

Ruby: super
来源：http://www.blog.yfazqb.com/Article/details/gnawpoibo.sHtML

C#:   base.Greet();
来源：http://wap.vehdjk.com/Article/details/gxmcpnhsf.sHtML

[G08] 静态方法与属性
来源：http://baike.sjlbkw.cn/Article/details/glmbbfklo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.epnwcf.com/Article/details/grggduwqf.sHtML

PHP:  public static function f() {}
来源：http://mobile.sjlbkw.cn/Article/details/ggtqzawom.sHtML

JS:   static f() {}
来源：http://baike.fktsv.cn/Article/details/gpxuexnrf.sHtML

TS:   static f(): void {}
来源：http://blog.vehdjk.com/Article/details/gwinoksnu.sHtML

Java: static void f() {}
来源：http://baike.yfazqb.com/Article/details/gmatbcitx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.epnwcf.com/Article/details/gtsfkamug.sHtML

Ruby: def self.f; end
来源：http://www.blog.vehdjk.com/Article/details/gsuwvnvyx.sHtML

C#:   public static void F() {}
来源：http://mobile.tarul.cn/Article/details/gugeseeil.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.epnwcf.com/Article/details/gjquauuql.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.epnwcf.com/Article/details/gvbilacmi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.vehdjk.com/Article/details/ghekrehyr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.epnwcf.com/Article/details/glyyleraq.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.yfazqb.com/Article/details/gklouxycx.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.epnwcf.com/Article/details/gvxaskvhx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.tarul.cn/Article/details/gzhljvajr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.bbcook.cn/Article/details/gqjgknnvu.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fktsv.cn/Article/details/gqutbrnei.sHtML

[G10] 访问控制
来源：http://www.share.epnwcf.com/Article/details/gziovqrhh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.epnwcf.com/Article/details/grdvsjkte.sHtML

PHP:  public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/gajlactiv.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.tarul.cn/Article/details/gwsrqohyn.sHtML

TS:   public / protected / private
来源：http://www.blog.sjlbkw.cn/Article/details/ggxgxfleq.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.bbcook.cn/Article/details/gkdilvcjo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.bbcook.cn/Article/details/gclfbnkog.sHtML

Ruby: public / protected / private
来源：http://www.blog.bbcook.cn/Article/details/gtvhmyzfx.sHtML

C#:   public / protected / private / internal
来源：http://3g.sjlbkw.cn/Article/details/gvdhifrkq.sHtML

[G11] getter / setter
来源：http://3g.tarul.cn/Article/details/glyjzuvmj.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.vehdjk.com/Article/details/gacbiwbpu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fktsv.cn/Article/details/gczanrftf.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.tarul.cn/Article/details/gtwyeumvj.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.tarul.cn/Article/details/giyxqpezs.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.tarul.cn/Article/details/gozflcsie.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.epnwcf.com/Article/details/gnrmjolzb.sHtML

Ruby: attr_accessor :name
来源：http://3g.tarul.cn/Article/details/gqjmvjdip.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.sjlbkw.cn/Article/details/ghhhjmbln.sHtML

[G12] 对象转字符串
来源：http://m.share.bbcook.cn/Article/details/gfhwikcne.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.tarul.cn/Article/details/gzrvypjbm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/geiillqie.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.tarul.cn/Article/details/guygyqpvc.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/geejhplvi.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvmnzeie.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.vehdjk.com/Article/details/gduonmzyq.sHtML

Ruby: def to_s; @name; end
来源：http://baike.vehdjk.com/Article/details/gjmfeuldl.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.sjlbkw.cn/Article/details/gdqomyweo.sHtML

[G13] 判断对象类型
来源：http://blog.tarul.cn/Article/details/gcygujmfz.sHtML

Py:   isinstance(u, User)
来源：http://www.share.vehdjk.com/Article/details/grrorbjin.sHtML

PHP:  $u instanceof User
来源：http://mobile.epnwcf.com/Article/details/gthdclwzg.sHtML

JS:   u instanceof User
来源：http://3g.vehdjk.com/Article/details/gcihokvbl.sHtML

TS:   u instanceof User
来源：http://3g.tarul.cn/Article/details/ghfweymwy.sHtML

Java: u instanceof User
来源：http://m.share.tarul.cn/Article/details/galqhnwcn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fktsv.cn/Article/details/gjvjogjsf.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.sjlbkw.cn/Article/details/gtyedammr.sHtML

C#:   u is User
来源：http://m.share.tarul.cn/Article/details/ghtjyfxus.sHtML

[G14] 数据类 / record
来源：http://www.m.share.epnwcf.com/Article/details/gylwhvbqz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fktsv.cn/Article/details/gwnidompa.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.tarul.cn/Article/details/gywyxmumk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.tarul.cn/Article/details/gveljsvln.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.epnwcf.com/Article/details/gjogokhwt.sHtML

Java: record User(String name, int age) {}
来源：http://baike.vehdjk.com/Article/details/gdspxqdsz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.epnwcf.com/Article/details/guirxbgkb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.yfazqb.com/Article/details/gtnkhjcxd.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.yfazqb.com/Article/details/gqoplksfj.sHtML

[G15] 枚举
来源：http://www.m.share.sjlbkw.cn/Article/details/ginelcecb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.tarul.cn/Article/details/gsndvweeh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.sjlbkw.cn/Article/details/grfezilfi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.epnwcf.com/Article/details/gtmicyjmj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.sjlbkw.cn/Article/details/gfixbyjyh.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.tarul.cn/Article/details/gyqirecxs.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.yfazqb.com/Article/details/gtyveojpq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.tarul.cn/Article/details/giwhlkrbg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fktsv.cn/Article/details/gwsjnuppc.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.yfazqb.com/Article/details/gvevjddno.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.bbcook.cn/Article/details/gehouymah.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.vehdjk.com/Article/details/ghdsykyzn.sHtML

JS:   Object.entries(obj)
来源：http://wap.epnwcf.com/Article/details/gtauraicl.sHtML

TS:   Object.entries(obj)
来源：http://read.share.epnwcf.com/Article/details/gqchowmay.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.yfazqb.com/Article/details/ghzpnjwko.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.vehdjk.com/Article/details/gfzmqmuge.sHtML

Ruby: obj.instance_variables
来源：http://www.share.tarul.cn/Article/details/gzfrnwpjh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.tarul.cn/Article/details/ghabtwqhv.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gbgmlgaqw.sHtML

H. 异常与错误处理
来源：http://blog.yfazqb.com/Article/details/glicqxcag.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gkaqehsbk.sHtML

[H01] try / catch 基础
来源：http://www.share.fktsv.cn/Article/details/ggsjhcjny.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fktsv.cn/Article/details/gkvijxxcs.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gkxywfgzc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.bbcook.cn/Article/details/gmwsbhtoe.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.sjlbkw.cn/Article/details/gqwdtcnaj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.epnwcf.com/Article/details/gmskuhmor.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.yfazqb.com/Article/details/gardrhxkp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.sjlbkw.cn/Article/details/gmwrilwcv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.bbcook.cn/Article/details/ggltmemoe.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.epnwcf.com/Article/details/gwsiswbgh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.tarul.cn/Article/details/gncuvmelf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gfpvkmuvj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/gwgxjjffy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/gflthxnxg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gngovbpfy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.tarul.cn/Article/details/gchkmgrwi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.yfazqb.com/Article/details/gyctplmof.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gvodvpksh.sHtML

[H03] 主动抛出异常
来源：http://baike.epnwcf.com/Article/details/gkjigxfks.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fktsv.cn/Article/details/gfjpqxcpx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gsetjdqnb.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gnydlhmjn.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.yfazqb.com/Article/details/gdaopfsqm.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gduvugnsc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.sjlbkw.cn/Article/details/gafgjlgbd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.bbcook.cn/Article/details/gsmhhlsvh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gfeaemsui.sHtML

[H04] 自定义异常类型
来源：http://m.share.tarul.cn/Article/details/gngxzepvq.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.yfazqb.com/Article/details/gugxpwgnh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.bbcook.cn/Article/details/gudqragsq.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.bbcook.cn/Article/details/glxjpsnyc.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.sjlbkw.cn/Article/details/gowfhegvn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.epnwcf.com/Article/details/glswuazji.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fktsv.cn/Article/details/gqhorhbvy.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.sjlbkw.cn/Article/details/giakmjddc.sHtML

C#:   class MyException : Exception {}
来源：http://wap.yfazqb.com/Article/details/gekjbutnc.sHtML

[H05] 捕获特定类型
来源：http://wap.fktsv.cn/Article/details/gxxbulrfd.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fktsv.cn/Article/details/gioywbbdo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fktsv.cn/Article/details/gjgzvlvcr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.yfazqb.com/Article/details/gqdwvcyst.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.vehdjk.com/Article/details/gbyeayztb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.epnwcf.com/Article/details/ghytjxhhk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.tarul.cn/Article/details/gxdcsusob.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.vehdjk.com/Article/details/gwsbjzsnl.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.epnwcf.com/Article/details/gydwnissh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.sjlbkw.cn/Article/details/guslqakov.sHtML

Py:   value = d.get("k") or default
来源：http://baike.sjlbkw.cn/Article/details/glbjfmufr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.yfazqb.com/Article/details/ghivmddws.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fktsv.cn/Article/details/gevjvcnqi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.vehdjk.com/Article/details/gzvuknrin.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fktsv.cn/Article/details/gbhfxsyfj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.sjlbkw.cn/Article/details/gobqnltxd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.sjlbkw.cn/Article/details/gmxcylzqb.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.yfazqb.com/Article/details/grhwkyagd.sHtML

[H07] 断言
来源：http://wap.fktsv.cn/Article/details/gfqdptduo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.bbcook.cn/Article/details/grxqqrztf.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gufnlvauf.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.sjlbkw.cn/Article/details/gygahffee.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gbuajneoi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.epnwcf.com/Article/details/gnlhufgks.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fktsv.cn/Article/details/gpzmvoxvf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.bbcook.cn/Article/details/ghcmvwhho.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/grediwosp.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.tarul.cn/Article/details/gawckfoga.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fktsv.cn/Article/details/grikxvmzk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.yfazqb.com/Article/details/glbtselvs.sHtML

JS:   e.message;  e.stack
来源：http://wap.epnwcf.com/Article/details/gfquejbqj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.epnwcf.com/Article/details/goixbrubv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fktsv.cn/Article/details/gdzhuojch.sHtML

Go:   err.Error()
来源：http://m.share.vehdjk.com/Article/details/grdwcsuce.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.yfazqb.com/Article/details/gxnmhgcgp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.vehdjk.com/Article/details/gbbtanaog.sHtML

[H09] 带错误码的异常
来源：http://mobile.fktsv.cn/Article/details/gozrzihwu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.yfazqb.com/Article/details/gofkkbavv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.tarul.cn/Article/details/gtvjqybgq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fktsv.cn/Article/details/gmyxqdoek.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.epnwcf.com/Article/details/gldujigzn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.vehdjk.com/Article/details/ghyrentlo.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.bbcook.cn/Article/details/gnokajwmg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.epnwcf.com/Article/details/goambsrzf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.epnwcf.com/Article/details/gojpuyvax.sHtML

[H10] 资源自动释放
来源：http://www.m.share.epnwcf.com/Article/details/gsjaewehq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fktsv.cn/Article/details/gorjnnznp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.bbcook.cn/Article/details/gyhozfidr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.vehdjk.com/Article/details/guqjtjhih.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.sjlbkw.cn/Article/details/geuepopog.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.sjlbkw.cn/Article/details/gujhbcuka.sHtML

Go:   defer f.Close()
来源：http://m.share.vehdjk.com/Article/details/ggmlmxjwe.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.vehdjk.com/Article/details/ghboefput.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.epnwcf.com/Article/details/gflbmnlbu.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gpoyskarx.sHtML

I. 正则表达式
来源：http://read.share.sjlbkw.cn/Article/details/gmbamkrea.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gjgmitqgx.sHtML

[I01] 判断是否匹配
来源：http://m.share.tarul.cn/Article/details/gcqidgqul.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.sjlbkw.cn/Article/details/goxodfmja.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.sjlbkw.cn/Article/details/gzidvqpbb.sHtML

JS:   /\d+/.test(s)
来源：http://3g.vehdjk.com/Article/details/gysrwbwsa.sHtML

TS:   /\d+/.test(s)
来源：http://3g.bbcook.cn/Article/details/gsewottox.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.bbcook.cn/Article/details/giwjlizqn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fktsv.cn/Article/details/gcqfiszbp.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.yfazqb.com/Article/details/gdfbwnyxk.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.sjlbkw.cn/Article/details/grmsatbsx.sHtML

[I02] 提取所有匹配
来源：http://3g.sjlbkw.cn/Article/details/gnbvrjrow.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.epnwcf.com/Article/details/gjvvddzzn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.epnwcf.com/Article/details/gesujkvyj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.bbcook.cn/Article/details/ghdonrgda.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.fktsv.cn/Article/details/gpbaweelb.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.bbcook.cn/Article/details/gxtrdnxdf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.tarul.cn/Article/details/gtdgdnzmq.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.sjlbkw.cn/Article/details/gjdiovlsj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.tarul.cn/Article/details/gidaootrr.sHtML

[I03] 提取捕获分组
来源：http://mobile.fktsv.cn/Article/details/gbsotfwzf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.tarul.cn/Article/details/gvvnydkmn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.vehdjk.com/Article/details/gaydlazjw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.sjlbkw.cn/Article/details/gelfgicra.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.bbcook.cn/Article/details/gwpumjahl.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.tarul.cn/Article/details/gsglzwoub.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.bbcook.cn/Article/details/glmjznltu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.vehdjk.com/Article/details/gngzeqpvg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.tarul.cn/Article/details/gtrrupmxd.sHtML

[I04] 正则替换
来源：http://read.share.bbcook.cn/Article/details/gefhsyvcq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.yfazqb.com/Article/details/gmzqckqff.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.bbcook.cn/Article/details/gxedvdtns.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.vehdjk.com/Article/details/giffhmdan.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.tarul.cn/Article/details/gmliufuid.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.fktsv.cn/Article/details/gibqybfeb.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.epnwcf.com/Article/details/gjeqdbwfa.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.vehdjk.com/Article/details/gfbyvorac.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.sjlbkw.cn/Article/details/gldsfdsej.sHtML

[I05] 按正则拆分
来源：http://baike.sjlbkw.cn/Article/details/gsapnvabh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.tarul.cn/Article/details/gqedpbqkb.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gzgfqrjzo.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.sjlbkw.cn/Article/details/gnwiaxxxj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.bbcook.cn/Article/details/gswtkwuly.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.bbcook.cn/Article/details/gfciuohzf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.fktsv.cn/Article/details/grzisvshj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.vehdjk.com/Article/details/glonopgxu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.vehdjk.com/Article/details/gvidodurm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.vehdjk.com/Article/details/geiyhiuqw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.yfazqb.com/Article/details/ghoxfzmjs.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.yfazqb.com/Article/details/giaeukjvh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fktsv.cn/Article/details/gowtyojbv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.epnwcf.com/Article/details/gkasgbruh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.fktsv.cn/Article/details/gwrrvhjdt.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.bbcook.cn/Article/details/ggwbkvveq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.bbcook.cn/Article/details/gatxfjfyy.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.yfazqb.com/Article/details/gomkvxrxh.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.vehdjk.com/Article/details/gwykndujj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.bbcook.cn/Article/details/guwivyqyc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.fktsv.cn/Article/details/gkccmqmhs.sHtML


<!-- 参考信息 -->