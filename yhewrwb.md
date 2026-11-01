代发 wailian999

[G02] 构造函数
来源：http://www.blog.vehdjk.com/Article/details/gtwwlkwfw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.tarul.cn/Article/details/gykxprwcy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.tarul.cn/Article/details/gsuaeuwze.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.vehdjk.com/Article/details/ghrfofytg.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.epnwcf.com/Article/details/gxqlnfgti.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.epnwcf.com/Article/details/gsrjhkttj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.sjlbkw.cn/Article/details/gsezlrghw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.sjlbkw.cn/Article/details/gplydkgda.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.vehdjk.com/Article/details/goarnrkan.sHtML

[G03] 实例属性
来源：http://www.blog.fktsv.cn/Article/details/gnydxknrc.sHtML

Py:   self.name = "x"
来源：http://www.blog.sjlbkw.cn/Article/details/gmqybvnwr.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.tarul.cn/Article/details/gaznkkbcv.sHtML

JS:   this.name = "x";
来源：http://baike.vehdjk.com/Article/details/gbuxiclvi.sHtML

TS:   name: string = "x";
来源：http://blog.bbcook.cn/Article/details/gmqqabgtb.sHtML

Java: private String name;
来源：http://mobile.fktsv.cn/Article/details/gukbqiuji.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.epnwcf.com/Article/details/gtbxnmitv.sHtML

Ruby: @name = "x"
来源：http://www.blog.bbcook.cn/Article/details/gknykldau.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fktsv.cn/Article/details/gvxszgxjh.sHtML

[G04] 定义方法
来源：http://www.blog.fktsv.cn/Article/details/gztdebpky.sHtML

Py:   def greet(self): return self.name
来源：http://baike.sjlbkw.cn/Article/details/gbrsodpzb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.yfazqb.com/Article/details/gioipsnnh.sHtML

JS:   greet() { return this.name; }
来源：http://3g.tarul.cn/Article/details/gvjeyfoqf.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/gdjwwohsd.sHtML

Java: String greet() { return name; }
来源：http://mobile.tarul.cn/Article/details/gtqiyodur.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.epnwcf.com/Article/details/gamryjavk.sHtML

Ruby: def greet; @name; end
来源：http://wap.vehdjk.com/Article/details/gbxkoejcs.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fktsv.cn/Article/details/gcyedlxzi.sHtML

[G05] 继承
来源：http://3g.yfazqb.com/Article/details/gumbcmfen.sHtML

Py:   class Admin(User): pass
来源：http://3g.tarul.cn/Article/details/gvlrbosuc.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/gnntbqlos.sHtML

JS:   class Admin extends User {}
来源：http://www.share.sjlbkw.cn/Article/details/grbqcqtsy.sHtML

TS:   class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gfkbcgcga.sHtML

Java: class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/gvqysqolo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.sjlbkw.cn/Article/details/gwrxsqcga.sHtML

Ruby: class Admin < User; end
来源：http://mobile.vehdjk.com/Article/details/gnhyququd.sHtML

C#:   class Admin : User {}
来源：http://baike.epnwcf.com/Article/details/gevrnmqop.sHtML

[G06] 重写方法
来源：http://baike.yfazqb.com/Article/details/grkgmxiuy.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.yfazqb.com/Article/details/gqzgralob.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/gwkaqahhb.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.yfazqb.com/Article/details/ghoxxvfek.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.yfazqb.com/Article/details/giwcrlcqs.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.vehdjk.com/Article/details/gnwxhbpit.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.yfazqb.com/Article/details/gcrhikndm.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.yfazqb.com/Article/details/gkhwamgie.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.yfazqb.com/Article/details/gvrfcnnne.sHtML

[G07] 调用父类方法
来源：http://www.blog.tarul.cn/Article/details/gorhksuwv.sHtML

Py:   super().greet()
来源：http://read.share.vehdjk.com/Article/details/gutucakcg.sHtML

PHP:  parent::greet();
来源：http://blog.tarul.cn/Article/details/goemjbfor.sHtML

JS:   super.greet();
来源：http://blog.yfazqb.com/Article/details/ggragxvpv.sHtML

TS:   super.greet();
来源：http://wap.vehdjk.com/Article/details/gasfopgdj.sHtML

Java: super.greet();
来源：http://www.share.epnwcf.com/Article/details/gzyeremiq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.sjlbkw.cn/Article/details/gzfdeijfq.sHtML

Ruby: super
来源：http://3g.yfazqb.com/Article/details/gpsagxaix.sHtML

C#:   base.Greet();
来源：http://wap.sjlbkw.cn/Article/details/gwanvoopm.sHtML

[G08] 静态方法与属性
来源：http://www.share.tarul.cn/Article/details/gsqvmeqtw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.sjlbkw.cn/Article/details/gvbmerffd.sHtML

PHP:  public static function f() {}
来源：http://www.blog.sjlbkw.cn/Article/details/glyulnrxp.sHtML

JS:   static f() {}
来源：http://www.blog.sjlbkw.cn/Article/details/gzyroblqx.sHtML

TS:   static f(): void {}
来源：http://www.share.fktsv.cn/Article/details/ggfidisfz.sHtML

Java: static void f() {}
来源：http://m.share.epnwcf.com/Article/details/gvuaftyrz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.tarul.cn/Article/details/gvoubkvsc.sHtML

Ruby: def self.f; end
来源：http://www.blog.vehdjk.com/Article/details/gewzzpqxz.sHtML

C#:   public static void F() {}
来源：http://www.m.share.tarul.cn/Article/details/gvfvnkwcl.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.epnwcf.com/Article/details/gjyxgewmh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.epnwcf.com/Article/details/gyioxesfc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.vehdjk.com/Article/details/gfehdmnkk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.sjlbkw.cn/Article/details/gcdabwpxd.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.tarul.cn/Article/details/gdcyugtjw.sHtML

Java: interface Shape { double area(); }
来源：http://wap.epnwcf.com/Article/details/gdvkfxjtx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.yfazqb.com/Article/details/gqcugefar.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.yfazqb.com/Article/details/gkypexbss.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fktsv.cn/Article/details/gfeiubegb.sHtML

[G10] 访问控制
来源：http://baike.sjlbkw.cn/Article/details/gbtrmrubw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.vehdjk.com/Article/details/goxknuthg.sHtML

PHP:  public / protected / private
来源：http://baike.tarul.cn/Article/details/gxvqxzhgr.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fktsv.cn/Article/details/gylcimeqr.sHtML

TS:   public / protected / private
来源：http://mobile.yfazqb.com/Article/details/glaezdsss.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fktsv.cn/Article/details/grdjntvgf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fktsv.cn/Article/details/gsadkpkxz.sHtML

Ruby: public / protected / private
来源：http://3g.tarul.cn/Article/details/gagtepchs.sHtML

C#:   public / protected / private / internal
来源：http://www.share.tarul.cn/Article/details/grbhmcgxj.sHtML

[G11] getter / setter
来源：http://wap.yfazqb.com/Article/details/gnhsouzdh.sHtML

Py:   @property 与 @x.setter
来源：http://blog.yfazqb.com/Article/details/gythrytvf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.tarul.cn/Article/details/gtxnhchha.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fktsv.cn/Article/details/gulyomlph.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.sjlbkw.cn/Article/details/gmnsgpqzm.sHtML

Java: public String getName() { return name; }
来源：http://mobile.vehdjk.com/Article/details/glpdxnvlz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.tarul.cn/Article/details/gzpwzviri.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fktsv.cn/Article/details/gpqgrngas.sHtML

C#:   public string Name { get; set; }
来源：http://baike.vehdjk.com/Article/details/gdbbtxlnl.sHtML

[G12] 对象转字符串
来源：http://read.share.epnwcf.com/Article/details/goocnygfe.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.tarul.cn/Article/details/gzxesldxv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.vehdjk.com/Article/details/grvrfuqpk.sHtML

JS:   toString() { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gobgphibe.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/gioabazkm.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.yfazqb.com/Article/details/gzqmbouan.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.sjlbkw.cn/Article/details/gxhpbrqlh.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.yfazqb.com/Article/details/geudrmmmu.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.tarul.cn/Article/details/ggldcdere.sHtML

[G13] 判断对象类型
来源：http://www.share.yfazqb.com/Article/details/gliygagpx.sHtML

Py:   isinstance(u, User)
来源：http://baike.epnwcf.com/Article/details/gdytisxco.sHtML

PHP:  $u instanceof User
来源：http://www.share.bbcook.cn/Article/details/gchfhqynq.sHtML

JS:   u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/glewiqthd.sHtML

TS:   u instanceof User
来源：http://read.share.vehdjk.com/Article/details/gcvhmqwpg.sHtML

Java: u instanceof User
来源：http://m.share.bbcook.cn/Article/details/gndtqqeur.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fktsv.cn/Article/details/gnhkfvgoh.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.bbcook.cn/Article/details/gqsgnvscv.sHtML

C#:   u is User
来源：http://3g.vehdjk.com/Article/details/gukmdbrfp.sHtML

[G14] 数据类 / record
来源：http://wap.bbcook.cn/Article/details/gkskziueg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.epnwcf.com/Article/details/gtndxkrch.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.sjlbkw.cn/Article/details/glowkjism.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fktsv.cn/Article/details/gslwejliw.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.epnwcf.com/Article/details/gazcgzjjx.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.vehdjk.com/Article/details/glanhkhfc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.epnwcf.com/Article/details/gdtyqfgar.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.sjlbkw.cn/Article/details/gahvybgcx.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.sjlbkw.cn/Article/details/gzphsxcfd.sHtML

[G15] 枚举
来源：http://blog.epnwcf.com/Article/details/girdvogoq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.tarul.cn/Article/details/ggjvuqkdo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fktsv.cn/Article/details/gdystsrnh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.bbcook.cn/Article/details/gmerqkctv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fktsv.cn/Article/details/gziycwjyn.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.vehdjk.com/Article/details/glaadssat.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.sjlbkw.cn/Article/details/ghhylguml.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fktsv.cn/Article/details/gjdxpsngn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.tarul.cn/Article/details/gtcwagnru.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.vehdjk.com/Article/details/ghbppwqvd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.epnwcf.com/Article/details/gvlqnmjnu.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.sjlbkw.cn/Article/details/gbukwwdcn.sHtML

JS:   Object.entries(obj)
来源：http://blog.sjlbkw.cn/Article/details/gpegvqtlk.sHtML

TS:   Object.entries(obj)
来源：http://blog.tarul.cn/Article/details/gsmzywmpl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.vehdjk.com/Article/details/gxattqdqa.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.yfazqb.com/Article/details/goyekdepb.sHtML

Ruby: obj.instance_variables
来源：http://blog.bbcook.cn/Article/details/gyuabxuzo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.yfazqb.com/Article/details/gzlztnymg.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gcsreafsx.sHtML

H. 异常与错误处理
来源：http://wap.fktsv.cn/Article/details/gjtqhftvo.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gsidnxuef.sHtML

[H01] try / catch 基础
来源：http://3g.yfazqb.com/Article/details/gqahswkns.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.tarul.cn/Article/details/gqzldnrkw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.bbcook.cn/Article/details/gxpyutepq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fktsv.cn/Article/details/gliljyirn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.epnwcf.com/Article/details/grnnvhnvj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.vehdjk.com/Article/details/gkicdtywa.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.sjlbkw.cn/Article/details/gulcqsecy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.epnwcf.com/Article/details/gxbutivhl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.yfazqb.com/Article/details/gjdpxnmoj.sHtML

[H02] finally / ensure 收尾
来源：http://blog.vehdjk.com/Article/details/gudfynmxg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.epnwcf.com/Article/details/gcoqgbwda.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/gtorgqzov.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/grndzegrq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/gdhlpwijt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/guomsizma.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fktsv.cn/Article/details/gecgpgkcu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.tarul.cn/Article/details/gzgkimvor.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gdwvhftoa.sHtML

[H03] 主动抛出异常
来源：http://mobile.fktsv.cn/Article/details/gqynpaaeh.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.epnwcf.com/Article/details/gjgpbguwn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/gsolnzdiy.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.vehdjk.com/Article/details/goxxebmci.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gkrlduvky.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gdutgsmra.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.sjlbkw.cn/Article/details/guwsszjxl.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.sjlbkw.cn/Article/details/grfjypkaz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.tarul.cn/Article/details/gpemqdhtt.sHtML

[H04] 自定义异常类型
来源：http://3g.fktsv.cn/Article/details/grukyhtnh.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fktsv.cn/Article/details/gdzzzwhaf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.epnwcf.com/Article/details/gjgmzosdj.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.sjlbkw.cn/Article/details/gvzsbwlap.sHtML

TS:   class MyError extends Error {}
来源：http://baike.yfazqb.com/Article/details/gtxdtpblm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.tarul.cn/Article/details/gmpdirjei.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.tarul.cn/Article/details/gupnpsfzd.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.epnwcf.com/Article/details/gpfsqeomg.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gikrgoxxh.sHtML

[H05] 捕获特定类型
来源：http://m.share.tarul.cn/Article/details/glatwseui.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.yfazqb.com/Article/details/gjphcrkse.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fktsv.cn/Article/details/gqcrbnltq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.tarul.cn/Article/details/guweqbgvb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.vehdjk.com/Article/details/gpepmlsgs.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.vehdjk.com/Article/details/grpqnnzqm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.sjlbkw.cn/Article/details/gegnvfqti.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fktsv.cn/Article/details/gdxyjinvp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.yfazqb.com/Article/details/gushfkflq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fktsv.cn/Article/details/gielglwzm.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.epnwcf.com/Article/details/gcegydvea.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.epnwcf.com/Article/details/gkwhpfydt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.yfazqb.com/Article/details/grseahotu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.vehdjk.com/Article/details/geceilisl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fktsv.cn/Article/details/gqqkoyxkb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.vehdjk.com/Article/details/gwewclidz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.tarul.cn/Article/details/gvzrqbhsw.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.vehdjk.com/Article/details/gazzgyjwl.sHtML

[H07] 断言
来源：http://www.share.sjlbkw.cn/Article/details/gulpacgap.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.tarul.cn/Article/details/gmkrsmekh.sHtML

PHP:  assert($x > 0);
来源：http://blog.vehdjk.com/Article/details/gxyqhxrzg.sHtML

JS:   console.assert(x > 0);
来源：http://blog.sjlbkw.cn/Article/details/gwiqhaznq.sHtML

TS:   console.assert(x > 0);
来源：http://baike.sjlbkw.cn/Article/details/gvlajqptu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.sjlbkw.cn/Article/details/glruiamsx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.tarul.cn/Article/details/ggxrnpwvv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.vehdjk.com/Article/details/gvchvtdoq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.bbcook.cn/Article/details/gnnvyhizi.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.sjlbkw.cn/Article/details/gqwsqgtvs.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.epnwcf.com/Article/details/gaanoqlcw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.epnwcf.com/Article/details/gzslvluge.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fktsv.cn/Article/details/gmuroztrn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fktsv.cn/Article/details/gbizynxeb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.epnwcf.com/Article/details/gdbizzens.sHtML

Go:   err.Error()
来源：http://m.share.fktsv.cn/Article/details/gvzaqelyo.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.yfazqb.com/Article/details/gwtlfmcrf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.yfazqb.com/Article/details/guocjhtrs.sHtML

[H09] 带错误码的异常
来源：http://mobile.bbcook.cn/Article/details/gbfykwcpf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.epnwcf.com/Article/details/gcfcvufkx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.tarul.cn/Article/details/gyapsjqxb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fktsv.cn/Article/details/gabgiawsp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fktsv.cn/Article/details/giozsudkz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.sjlbkw.cn/Article/details/gqburgykk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.yfazqb.com/Article/details/gzauowitl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fktsv.cn/Article/details/ggqmczyzm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.tarul.cn/Article/details/guywpuqxg.sHtML

[H10] 资源自动释放
来源：http://3g.yfazqb.com/Article/details/gsxnxuhsa.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.bbcook.cn/Article/details/gjpjqpuep.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.yfazqb.com/Article/details/ghgroqpvu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.sjlbkw.cn/Article/details/gxyrxzcpb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.vehdjk.com/Article/details/gqnsoocrn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fktsv.cn/Article/details/ggclmmpzt.sHtML

Go:   defer f.Close()
来源：http://m.share.sjlbkw.cn/Article/details/gajjutcmi.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.tarul.cn/Article/details/gkyckzjxr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.yfazqb.com/Article/details/glnaterub.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/glmosmyzb.sHtML

I. 正则表达式
来源：http://m.share.vehdjk.com/Article/details/gjtsdsdbr.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gulahjeum.sHtML

[I01] 判断是否匹配
来源：http://wap.bbcook.cn/Article/details/gnowilvik.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.epnwcf.com/Article/details/gikgryoap.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fktsv.cn/Article/details/guzpgsdun.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.fktsv.cn/Article/details/gzegqnfdo.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fktsv.cn/Article/details/gskylmicj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.tarul.cn/Article/details/gplsebwmj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.fktsv.cn/Article/details/gubwufazh.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.yfazqb.com/Article/details/gpideuizr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.vehdjk.com/Article/details/gztwpglnh.sHtML

[I02] 提取所有匹配
来源：http://www.blog.vehdjk.com/Article/details/ginegzmml.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fktsv.cn/Article/details/gujvpoapx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.epnwcf.com/Article/details/ghqzcoktx.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.epnwcf.com/Article/details/gqukbmnvw.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.yfazqb.com/Article/details/gqhkyhcup.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.tarul.cn/Article/details/glckveknb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.bbcook.cn/Article/details/ghumnmxou.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.yfazqb.com/Article/details/glcrskhyx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmgfhzkps.sHtML

[I03] 提取捕获分组
来源：http://mobile.epnwcf.com/Article/details/gvrjxneag.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.epnwcf.com/Article/details/gshfnumdz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.bbcook.cn/Article/details/gcacfeupz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.bbcook.cn/Article/details/gwzgcmigt.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.bbcook.cn/Article/details/gqmfqjudl.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.bbcook.cn/Article/details/gdvvosgni.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fktsv.cn/Article/details/gzuvzhlsm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.tarul.cn/Article/details/gavawurih.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fktsv.cn/Article/details/gfyphotaq.sHtML

[I04] 正则替换
来源：http://www.m.share.tarul.cn/Article/details/gfxqfvssv.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.epnwcf.com/Article/details/ghynkhjuj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.bbcook.cn/Article/details/gbpkaebii.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.bbcook.cn/Article/details/ggbcwviuy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.vehdjk.com/Article/details/gjnzelijc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.yfazqb.com/Article/details/gkjbnioxv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.bbcook.cn/Article/details/gmizqmtgk.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.sjlbkw.cn/Article/details/ghmlfpwvn.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.vehdjk.com/Article/details/gevlkzapf.sHtML

[I05] 按正则拆分
来源：http://www.share.yfazqb.com/Article/details/glpsgcugq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.epnwcf.com/Article/details/gqjdfcjsy.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.epnwcf.com/Article/details/gbxxamuxo.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.bbcook.cn/Article/details/gvtiixppt.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fktsv.cn/Article/details/gfqqtktwg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.vehdjk.com/Article/details/geanzvzzg.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.epnwcf.com/Article/details/gsoqtfrim.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.yfazqb.com/Article/details/gwvxzitmx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.epnwcf.com/Article/details/gotxodypa.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fktsv.cn/Article/details/gnkpzzood.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.vehdjk.com/Article/details/gwjfwtddk.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.fktsv.cn/Article/details/gqftepetc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.tarul.cn/Article/details/gwqitrejj.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fktsv.cn/Article/details/gyqifmzeq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.fktsv.cn/Article/details/gxpokcrel.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.vehdjk.com/Article/details/gcmetbgvo.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.sjlbkw.cn/Article/details/gdsrktmdb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fktsv.cn/Article/details/gmuiightk.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.epnwcf.com/Article/details/gqbcrqjxv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.sjlbkw.cn/Article/details/ggyubdnnv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fktsv.cn/Article/details/grhwtogrk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.vehdjk.com/Article/details/gbsiylfcq.sHtML

TS:   /error/gim
来源：http://baike.tarul.cn/Article/details/gkarlmpyf.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.vehdjk.com/Article/details/gzocahkxy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.bbcook.cn/Article/details/giirztysi.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fktsv.cn/Article/details/gzxaexivq.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.tarul.cn/Article/details/ghdxjuqbh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.vehdjk.com/Article/details/gstyvyryu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.fktsv.cn/Article/details/ggqdpztog.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.yfazqb.com/Article/details/gyhhxdqfl.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.sjlbkw.cn/Article/details/gqazfhdpj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.tarul.cn/Article/details/gqccstmjt.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.epnwcf.com/Article/details/gyuwmspbw.sHtML


<!-- 参考信息 -->