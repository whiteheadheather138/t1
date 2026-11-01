代发 wailian999

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gkzxjkgxo.sHtML

G. 面向对象
来源：http://www.blog.fktsv.cn/Article/details/gpjbabfwz.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gskudnjgv.sHtML

[G01] 定义类
来源：http://mobile.epnwcf.com/Article/details/gvkpdrgwp.sHtML

Py:   class User: pass
来源：http://www.share.bbcook.cn/Article/details/gglrecimr.sHtML

PHP:  class User {}
来源：http://mobile.epnwcf.com/Article/details/glimtqvyz.sHtML

JS:   class User {}
来源：http://mobile.fktsv.cn/Article/details/gliwowyuw.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.yfazqb.com/Article/details/grvsyjhxn.sHtML

Java: class User {}
来源：http://read.share.fktsv.cn/Article/details/gylpmbsxi.sHtML

Go:   type User struct { Name string }
来源：http://read.share.sjlbkw.cn/Article/details/gevpxkulo.sHtML

Ruby: class User; end
来源：http://blog.sjlbkw.cn/Article/details/goxrwvqgu.sHtML

C#:   class User {}
来源：http://blog.bbcook.cn/Article/details/gtekpoxwy.sHtML

[G02] 构造函数
来源：http://baike.fktsv.cn/Article/details/gtpjgdkwf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.vehdjk.com/Article/details/gsqfnyjfm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.sjlbkw.cn/Article/details/gwjptccbk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fktsv.cn/Article/details/grwttxyxd.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fktsv.cn/Article/details/gcnjnshsh.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fktsv.cn/Article/details/gehsanigq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.epnwcf.com/Article/details/gnnzatoay.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.yfazqb.com/Article/details/grhalgwon.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.yfazqb.com/Article/details/glfvsbgxf.sHtML

[G03] 实例属性
来源：http://www.m.share.epnwcf.com/Article/details/guqoulxhj.sHtML

Py:   self.name = "x"
来源：http://www.blog.tarul.cn/Article/details/gisgztxgv.sHtML

PHP:  public string $name = "x";
来源：http://mobile.epnwcf.com/Article/details/gfiyprflw.sHtML

JS:   this.name = "x";
来源：http://mobile.fktsv.cn/Article/details/galwmsmqe.sHtML

TS:   name: string = "x";
来源：http://baike.yfazqb.com/Article/details/ggubmghen.sHtML

Java: private String name;
来源：http://mobile.sjlbkw.cn/Article/details/gifrntxks.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.sjlbkw.cn/Article/details/gpeizifgh.sHtML

Ruby: @name = "x"
来源：http://www.share.bbcook.cn/Article/details/gbvpuwmyt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.bbcook.cn/Article/details/gsfmfsfwe.sHtML

[G04] 定义方法
来源：http://www.blog.tarul.cn/Article/details/gzdeselhd.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fktsv.cn/Article/details/gwgwbuvoo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.bbcook.cn/Article/details/gjgauzwxa.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fktsv.cn/Article/details/gtyobuxwc.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.tarul.cn/Article/details/gkamivtll.sHtML

Java: String greet() { return name; }
来源：http://www.share.yfazqb.com/Article/details/gunvvjizp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.tarul.cn/Article/details/grlddxikw.sHtML

Ruby: def greet; @name; end
来源：http://m.share.yfazqb.com/Article/details/gbtelbvdn.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.bbcook.cn/Article/details/gpiyjtzto.sHtML

[G05] 继承
来源：http://read.share.tarul.cn/Article/details/gfgiqkixv.sHtML

Py:   class Admin(User): pass
来源：http://blog.fktsv.cn/Article/details/gbyquclot.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fktsv.cn/Article/details/gzmwuuqos.sHtML

JS:   class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/gtrswnxlf.sHtML

TS:   class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/ghxqxexos.sHtML

Java: class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/gffdnzbtk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.tarul.cn/Article/details/gewnntyuc.sHtML

Ruby: class Admin < User; end
来源：http://m.share.yfazqb.com/Article/details/gsapnqzkf.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.vehdjk.com/Article/details/gteoryojw.sHtML

[G06] 重写方法
来源：http://www.blog.epnwcf.com/Article/details/gtmrosqns.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.vehdjk.com/Article/details/gzpjbiyat.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gzlverwdr.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/gogcwpnyo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gysxwlonz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gnoxahenk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.epnwcf.com/Article/details/ghsjghqom.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.epnwcf.com/Article/details/ggavhzcqs.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.tarul.cn/Article/details/gcnpijsxb.sHtML

[G07] 调用父类方法
来源：http://blog.tarul.cn/Article/details/geavqppwj.sHtML

Py:   super().greet()
来源：http://m.share.yfazqb.com/Article/details/gccpebsdf.sHtML

PHP:  parent::greet();
来源：http://wap.sjlbkw.cn/Article/details/gshuhoktr.sHtML

JS:   super.greet();
来源：http://wap.sjlbkw.cn/Article/details/ggedovzdr.sHtML

TS:   super.greet();
来源：http://baike.tarul.cn/Article/details/gvafwxbbe.sHtML

Java: super.greet();
来源：http://read.share.sjlbkw.cn/Article/details/gmcoktgwe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.bbcook.cn/Article/details/gszlnvblz.sHtML

Ruby: super
来源：http://read.share.fktsv.cn/Article/details/gzmninwle.sHtML

C#:   base.Greet();
来源：http://wap.yfazqb.com/Article/details/giflrnyhf.sHtML

[G08] 静态方法与属性
来源：http://wap.sjlbkw.cn/Article/details/gosbhqfov.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.epnwcf.com/Article/details/gkmugrafv.sHtML

PHP:  public static function f() {}
来源：http://wap.bbcook.cn/Article/details/gscikcobj.sHtML

JS:   static f() {}
来源：http://mobile.tarul.cn/Article/details/gztqsypnn.sHtML

TS:   static f(): void {}
来源：http://www.share.yfazqb.com/Article/details/glvzegpuk.sHtML

Java: static void f() {}
来源：http://mobile.vehdjk.com/Article/details/guilkaqoi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.vehdjk.com/Article/details/gabeahwch.sHtML

Ruby: def self.f; end
来源：http://read.share.yfazqb.com/Article/details/guchczkbs.sHtML

C#:   public static void F() {}
来源：http://read.share.epnwcf.com/Article/details/geqrxdise.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fktsv.cn/Article/details/gyywktqso.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.sjlbkw.cn/Article/details/gxrytdjlc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.epnwcf.com/Article/details/gnvynimdh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjdtmzsd.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.sjlbkw.cn/Article/details/gkuyfbjkr.sHtML

Java: interface Shape { double area(); }
来源：http://baike.yfazqb.com/Article/details/gpjtwgrvk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fktsv.cn/Article/details/gehhrraag.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.sjlbkw.cn/Article/details/gbwtjqazs.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.vehdjk.com/Article/details/grroxjona.sHtML

[G10] 访问控制
来源：http://www.share.epnwcf.com/Article/details/gjiaklogl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.yfazqb.com/Article/details/gmkbbomin.sHtML

PHP:  public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/gkmyrqvvl.sHtML

JS:   #private 字段；其余公开
来源：http://baike.vehdjk.com/Article/details/gbngovjso.sHtML

TS:   public / protected / private
来源：http://read.share.sjlbkw.cn/Article/details/gjdearyks.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.tarul.cn/Article/details/gebbvynxh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.vehdjk.com/Article/details/gmmuxxlok.sHtML

Ruby: public / protected / private
来源：http://www.share.vehdjk.com/Article/details/guwthducl.sHtML

C#:   public / protected / private / internal
来源：http://blog.vehdjk.com/Article/details/gwxvwqrhl.sHtML

[G11] getter / setter
来源：http://mobile.fktsv.cn/Article/details/gkmgsikxp.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.bbcook.cn/Article/details/ghkbhypuu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.epnwcf.com/Article/details/gbuksqmec.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.epnwcf.com/Article/details/gwopunguz.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.tarul.cn/Article/details/gzwrtuwwl.sHtML

Java: public String getName() { return name; }
来源：http://read.share.tarul.cn/Article/details/gcjvegmrm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.sjlbkw.cn/Article/details/gjsboiikv.sHtML

Ruby: attr_accessor :name
来源：http://m.share.vehdjk.com/Article/details/gxlubzxih.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.vehdjk.com/Article/details/grspiufse.sHtML

[G12] 对象转字符串
来源：http://wap.epnwcf.com/Article/details/gtpeypwpr.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.tarul.cn/Article/details/gzhpihryg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fktsv.cn/Article/details/ghxxedgpf.sHtML

JS:   toString() { return this.name; }
来源：http://baike.bbcook.cn/Article/details/gfghcytnp.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.yfazqb.com/Article/details/gzvfbibkp.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.bbcook.cn/Article/details/gxqowlfsd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.bbcook.cn/Article/details/ghzsnvvlp.sHtML

Ruby: def to_s; @name; end
来源：http://3g.vehdjk.com/Article/details/gsshwjxcr.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fktsv.cn/Article/details/gqkudduqg.sHtML

[G13] 判断对象类型
来源：http://wap.tarul.cn/Article/details/glpyythag.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fktsv.cn/Article/details/guxmmjfxm.sHtML

PHP:  $u instanceof User
来源：http://m.share.tarul.cn/Article/details/gfgstfhha.sHtML

JS:   u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/gygqnsfln.sHtML

TS:   u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/gmuietgfe.sHtML

Java: u instanceof User
来源：http://wap.yfazqb.com/Article/details/gldrqkmhl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.vehdjk.com/Article/details/guwkygcvr.sHtML

Ruby: u.is_a?(User)
来源：http://3g.epnwcf.com/Article/details/gehakeesp.sHtML

C#:   u is User
来源：http://baike.fktsv.cn/Article/details/gclydadcx.sHtML

[G14] 数据类 / record
来源：http://blog.epnwcf.com/Article/details/goxzrhtpt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.yfazqb.com/Article/details/gtrchivsu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.epnwcf.com/Article/details/glhdtarot.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.epnwcf.com/Article/details/giacfmrzf.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.epnwcf.com/Article/details/gxgcsdvtk.sHtML

Java: record User(String name, int age) {}
来源：http://blog.tarul.cn/Article/details/glpewqezu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.sjlbkw.cn/Article/details/gxsorrhlt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.epnwcf.com/Article/details/gcqjyaanh.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.yfazqb.com/Article/details/gqdkakarq.sHtML

[G15] 枚举
来源：http://www.share.epnwcf.com/Article/details/gdtnjtdqp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.bbcook.cn/Article/details/gdspltdqh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fktsv.cn/Article/details/gczymuxrj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.tarul.cn/Article/details/gjgmmplxw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.epnwcf.com/Article/details/gckryucwx.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.epnwcf.com/Article/details/gkwkgtjgd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.yfazqb.com/Article/details/gdfjivsjt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fktsv.cn/Article/details/gkrntiogn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fktsv.cn/Article/details/gcsbunccy.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fktsv.cn/Article/details/gxvkxywft.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.vehdjk.com/Article/details/gdcqemfrk.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.sjlbkw.cn/Article/details/gmkgihgpz.sHtML

JS:   Object.entries(obj)
来源：http://read.share.epnwcf.com/Article/details/gxgvvefli.sHtML

TS:   Object.entries(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gztfqkjxx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.vehdjk.com/Article/details/gymsmucoo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.vehdjk.com/Article/details/gfofxjlpp.sHtML

Ruby: obj.instance_variables
来源：http://mobile.vehdjk.com/Article/details/gadwoehrw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.bbcook.cn/Article/details/ghsftselp.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gsdkueohs.sHtML

H. 异常与错误处理
来源：http://wap.bbcook.cn/Article/details/gutwpcmeg.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gbbhctxmo.sHtML

[H01] try / catch 基础
来源：http://m.share.yfazqb.com/Article/details/gmjolpgmv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.vehdjk.com/Article/details/gwtsyjvrr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.bbcook.cn/Article/details/gwsptqndp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.tarul.cn/Article/details/gjsszzvsv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.epnwcf.com/Article/details/gfpfvhiga.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.tarul.cn/Article/details/gnveotxag.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.sjlbkw.cn/Article/details/glxxnxysb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fktsv.cn/Article/details/gplxuxkkr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwxbsevcw.sHtML

[H02] finally / ensure 收尾
来源：http://3g.epnwcf.com/Article/details/gkztcdfwn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.yfazqb.com/Article/details/gajiwlrkz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gfosjcdxk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.bbcook.cn/Article/details/gxjjuprip.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gdzmvciyy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.yfazqb.com/Article/details/gyvunygss.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fktsv.cn/Article/details/gabmcmsaw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.yfazqb.com/Article/details/ghpramzpf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/gzewliqdk.sHtML

[H03] 主动抛出异常
来源：http://blog.fktsv.cn/Article/details/gzhthorcw.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.tarul.cn/Article/details/gmacaszdp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/grgvqveoq.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.tarul.cn/Article/details/gtufjzuyk.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.yfazqb.com/Article/details/gvumvhjaq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.yfazqb.com/Article/details/grwrubldi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.vehdjk.com/Article/details/gmoouenrf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.tarul.cn/Article/details/gvbhvwgek.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fktsv.cn/Article/details/grlychcwx.sHtML

[H04] 自定义异常类型
来源：http://www.blog.epnwcf.com/Article/details/gqxbnyvba.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.tarul.cn/Article/details/gvfjpwwqt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.yfazqb.com/Article/details/gauhgzqcv.sHtML

JS:   class MyError extends Error {}
来源：http://3g.yfazqb.com/Article/details/gqcchqfih.sHtML

TS:   class MyError extends Error {}
来源：http://baike.bbcook.cn/Article/details/gzbqojtlp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.sjlbkw.cn/Article/details/gdgaiojeu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.epnwcf.com/Article/details/gyngvpwbs.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.epnwcf.com/Article/details/gbygdaeuc.sHtML

C#:   class MyException : Exception {}
来源：http://wap.tarul.cn/Article/details/giixjknrv.sHtML

[H05] 捕获特定类型
来源：http://read.share.fktsv.cn/Article/details/geledbrfy.sHtML

Py:   except ValueError as e:
来源：http://blog.yfazqb.com/Article/details/gafamsdmx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.bbcook.cn/Article/details/gqxckwjuy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.epnwcf.com/Article/details/gecpfsdqk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.tarul.cn/Article/details/glcwqcsin.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.yfazqb.com/Article/details/gammouunz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.vehdjk.com/Article/details/gnsgculsm.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.sjlbkw.cn/Article/details/gjbpkxusc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.tarul.cn/Article/details/gwwyhoowq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.yfazqb.com/Article/details/gxvsoougr.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.vehdjk.com/Article/details/gtigmvxnw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.sjlbkw.cn/Article/details/gcifbmcsl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.yfazqb.com/Article/details/gukbxgbet.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.tarul.cn/Article/details/gbqklnzql.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.tarul.cn/Article/details/gchdjoptu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fktsv.cn/Article/details/glulmzcdi.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.yfazqb.com/Article/details/gyzqosgai.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.bbcook.cn/Article/details/gdqsubzht.sHtML

[H07] 断言
来源：http://www.m.share.vehdjk.com/Article/details/gmjjhtxhr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.bbcook.cn/Article/details/gejhydcpy.sHtML

PHP:  assert($x > 0);
来源：http://mobile.epnwcf.com/Article/details/glnyleacm.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.bbcook.cn/Article/details/gbbrrvwwp.sHtML

TS:   console.assert(x > 0);
来源：http://wap.vehdjk.com/Article/details/ggpjusvqs.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.vehdjk.com/Article/details/gcswdtxah.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.sjlbkw.cn/Article/details/gicmlqkuo.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.bbcook.cn/Article/details/gbwahpcev.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/gliwyxzec.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.yfazqb.com/Article/details/gdkfjrwbd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fktsv.cn/Article/details/gkfsqagzy.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fktsv.cn/Article/details/gfhvirpmc.sHtML

JS:   e.message;  e.stack
来源：http://baike.tarul.cn/Article/details/gwwdqtcow.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.vehdjk.com/Article/details/gsxrqpdfo.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.tarul.cn/Article/details/gifusiefm.sHtML

Go:   err.Error()
来源：http://3g.epnwcf.com/Article/details/gaknrwwbv.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.bbcook.cn/Article/details/gocifkrth.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.bbcook.cn/Article/details/gdyxfoyvh.sHtML

[H09] 带错误码的异常
来源：http://baike.sjlbkw.cn/Article/details/gxuofhyzy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.vehdjk.com/Article/details/gvxwgwgjk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.yfazqb.com/Article/details/gkmzpsylb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.epnwcf.com/Article/details/gnrmwqmvj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.epnwcf.com/Article/details/gvydycauh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.epnwcf.com/Article/details/gwnjlkmdz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.yfazqb.com/Article/details/gaibmwwxq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.bbcook.cn/Article/details/gakettfyv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.sjlbkw.cn/Article/details/gvqxtoegx.sHtML

[H10] 资源自动释放
来源：http://www.m.share.epnwcf.com/Article/details/gzuiozxgn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.epnwcf.com/Article/details/gktgcgduz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fktsv.cn/Article/details/gxpcrnyif.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.epnwcf.com/Article/details/gnfahxxpd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.yfazqb.com/Article/details/givoygjkp.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.bbcook.cn/Article/details/gucrrxxlv.sHtML

Go:   defer f.Close()
来源：http://www.share.epnwcf.com/Article/details/gulgoguxv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.tarul.cn/Article/details/gmeusfqba.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.bbcook.cn/Article/details/gddrpwwuo.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gnepqyrmf.sHtML

I. 正则表达式
来源：http://m.share.epnwcf.com/Article/details/ghpkyvjdz.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gacacmawv.sHtML

[I01] 判断是否匹配
来源：http://m.share.bbcook.cn/Article/details/gqfdndvwq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fktsv.cn/Article/details/gmcnxacae.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.tarul.cn/Article/details/gvwzxpbxm.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.bbcook.cn/Article/details/gctrbupra.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.yfazqb.com/Article/details/gisjevadu.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.vehdjk.com/Article/details/ggdotbbtz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.yfazqb.com/Article/details/gnfsfgnmu.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.vehdjk.com/Article/details/gvnfzhwyf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.vehdjk.com/Article/details/grovwrkyu.sHtML

[I02] 提取所有匹配
来源：http://3g.tarul.cn/Article/details/gzsevqnwt.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.yfazqb.com/Article/details/ghuxmurxv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.bbcook.cn/Article/details/gksguqlob.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fktsv.cn/Article/details/glnnalpfv.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.fktsv.cn/Article/details/gsgfcqtgz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.yfazqb.com/Article/details/gbrjvrukb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.epnwcf.com/Article/details/gesqumbmw.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fktsv.cn/Article/details/gswcbyaqd.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gfxpazces.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.epnwcf.com/Article/details/gwsvpsceq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fktsv.cn/Article/details/gztctnecb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.yfazqb.com/Article/details/gvldoibid.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.tarul.cn/Article/details/gzhdbigdm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.epnwcf.com/Article/details/gzfwiqvyt.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.fktsv.cn/Article/details/gyjwiwwzb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.sjlbkw.cn/Article/details/gxtnpzsti.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.yfazqb.com/Article/details/gcuqhpsky.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.tarul.cn/Article/details/ggtxseymx.sHtML

[I04] 正则替换
来源：http://www.m.share.vehdjk.com/Article/details/gpfbccnjt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.sjlbkw.cn/Article/details/gcbutniqx.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.yfazqb.com/Article/details/gzdrydbmt.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.tarul.cn/Article/details/goboaxiom.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.tarul.cn/Article/details/gzuabddlb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.tarul.cn/Article/details/gbifnzrni.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.fktsv.cn/Article/details/gatotxncd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.fktsv.cn/Article/details/gjmqltxjf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.bbcook.cn/Article/details/gohkwuswz.sHtML

[I05] 按正则拆分
来源：http://www.blog.yfazqb.com/Article/details/gvezrfddr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.fktsv.cn/Article/details/gphptgssr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.vehdjk.com/Article/details/gttzasjbc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.epnwcf.com/Article/details/gkscjqwno.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.bbcook.cn/Article/details/gruweylvj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.fktsv.cn/Article/details/gecudymiy.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.yfazqb.com/Article/details/gcztjkmrh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.vehdjk.com/Article/details/glrtxykqp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.tarul.cn/Article/details/ghspywzpa.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.fktsv.cn/Article/details/gtbtbwpog.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.vehdjk.com/Article/details/gpmydqqgn.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.epnwcf.com/Article/details/gccejfxcs.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fktsv.cn/Article/details/grczhrgcd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.yfazqb.com/Article/details/gkcliynet.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.bbcook.cn/Article/details/gtermfhrh.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.yfazqb.com/Article/details/gjfcklwym.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.tarul.cn/Article/details/gmvrcsxql.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.yfazqb.com/Article/details/guzscfxpa.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.epnwcf.com/Article/details/gdzrdjuvr.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.tarul.cn/Article/details/gubgishwx.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.yfazqb.com/Article/details/gsremnjqp.sHtML


<!-- 参考信息 -->