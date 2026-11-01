代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.tarul.cn/Article/details/gxnsqwama.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gnxmwnvkv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.epnwcf.com/Article/details/gohmmqfub.sHtML

[F12] CSV 读写
来源：http://baike.bbcook.cn/Article/details/gjigmjiwk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.bbcook.cn/Article/details/glspojalg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.bbcook.cn/Article/details/giazanjzj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.bbcook.cn/Article/details/gfuhcffwu.sHtML

TS:   // 同上
来源：http://wap.yfazqb.com/Article/details/gpuxxyexk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.epnwcf.com/Article/details/goumbqnox.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fktsv.cn/Article/details/ggjfrqxap.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.vehdjk.com/Article/details/gmfrxawct.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.bbcook.cn/Article/details/gijbgvkde.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gvcujtlbd.sHtML

G. 面向对象
来源：http://www.m.share.sjlbkw.cn/Article/details/gwspkklwl.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gvuvdozoz.sHtML

[G01] 定义类
来源：http://www.share.sjlbkw.cn/Article/details/gkzzmfqgu.sHtML

Py:   class User: pass
来源：http://read.share.fktsv.cn/Article/details/gqidkolps.sHtML

PHP:  class User {}
来源：http://wap.vehdjk.com/Article/details/gnfgiefrl.sHtML

JS:   class User {}
来源：http://www.blog.vehdjk.com/Article/details/ghylspooi.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.vehdjk.com/Article/details/gcoxaqutt.sHtML

Java: class User {}
来源：http://mobile.tarul.cn/Article/details/gjluxozoi.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fktsv.cn/Article/details/gnmdschae.sHtML

Ruby: class User; end
来源：http://read.share.vehdjk.com/Article/details/gqelnyofz.sHtML

C#:   class User {}
来源：http://m.share.sjlbkw.cn/Article/details/gajhdbzbu.sHtML

[G02] 构造函数
来源：http://www.blog.bbcook.cn/Article/details/gezicvmuf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.tarul.cn/Article/details/gkhtpbjtz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fktsv.cn/Article/details/ghqzibbpt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.bbcook.cn/Article/details/gptqmtjqf.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.sjlbkw.cn/Article/details/gpaeygqpu.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.epnwcf.com/Article/details/gahwqujjk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.yfazqb.com/Article/details/gifewjexn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.bbcook.cn/Article/details/gljjwuhhv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.yfazqb.com/Article/details/gogoqsexl.sHtML

[G03] 实例属性
来源：http://baike.sjlbkw.cn/Article/details/gpvrozvlt.sHtML

Py:   self.name = "x"
来源：http://baike.yfazqb.com/Article/details/gerujtrdd.sHtML

PHP:  public string $name = "x";
来源：http://baike.vehdjk.com/Article/details/gzafkbure.sHtML

JS:   this.name = "x";
来源：http://www.m.share.vehdjk.com/Article/details/gkwqrepzd.sHtML

TS:   name: string = "x";
来源：http://read.share.epnwcf.com/Article/details/gczmtqwuv.sHtML

Java: private String name;
来源：http://baike.fktsv.cn/Article/details/ghozyhwjk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.tarul.cn/Article/details/gmogfiiht.sHtML

Ruby: @name = "x"
来源：http://www.blog.yfazqb.com/Article/details/gsvhyrgdx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.yfazqb.com/Article/details/gkkkrdwhr.sHtML

[G04] 定义方法
来源：http://read.share.yfazqb.com/Article/details/gpuppfqnk.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.bbcook.cn/Article/details/gwyficcyg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.epnwcf.com/Article/details/gfjemetck.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.vehdjk.com/Article/details/gweemmeml.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.sjlbkw.cn/Article/details/gcoreeywo.sHtML

Java: String greet() { return name; }
来源：http://blog.tarul.cn/Article/details/gydcdtkhu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.sjlbkw.cn/Article/details/gatvpqrzp.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.bbcook.cn/Article/details/gweoietnv.sHtML

C#:   public string Greet() => Name;
来源：http://3g.vehdjk.com/Article/details/gdsubnjaw.sHtML

[G05] 继承
来源：http://baike.sjlbkw.cn/Article/details/gtulepven.sHtML

Py:   class Admin(User): pass
来源：http://m.share.sjlbkw.cn/Article/details/giqtqfciu.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gzfxykhuw.sHtML

JS:   class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/gcyyhhzcv.sHtML

TS:   class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/gmwajhwyf.sHtML

Java: class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/gleoakcsg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.bbcook.cn/Article/details/geqevjlmg.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.vehdjk.com/Article/details/gjdgjtsov.sHtML

C#:   class Admin : User {}
来源：http://www.blog.bbcook.cn/Article/details/gwzivalyy.sHtML

[G06] 重写方法
来源：http://3g.epnwcf.com/Article/details/grlrknckt.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.yfazqb.com/Article/details/gsrmgxrpm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gskjxlpax.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/ghstcieju.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/gxxxxbwbu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gbrhptaua.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.sjlbkw.cn/Article/details/gbdpsyniv.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fktsv.cn/Article/details/gjwrdfbyk.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.tarul.cn/Article/details/ggxdjnrwz.sHtML

[G07] 调用父类方法
来源：http://www.share.vehdjk.com/Article/details/gqnjdwshl.sHtML

Py:   super().greet()
来源：http://read.share.vehdjk.com/Article/details/gqwztmrxo.sHtML

PHP:  parent::greet();
来源：http://mobile.yfazqb.com/Article/details/gcffjkjjq.sHtML

JS:   super.greet();
来源：http://m.share.tarul.cn/Article/details/gsekiaodm.sHtML

TS:   super.greet();
来源：http://m.share.yfazqb.com/Article/details/ggdtqziwh.sHtML

Java: super.greet();
来源：http://www.m.share.epnwcf.com/Article/details/grzopqwih.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.tarul.cn/Article/details/glscogqfp.sHtML

Ruby: super
来源：http://blog.epnwcf.com/Article/details/gbhxsgfjw.sHtML

C#:   base.Greet();
来源：http://www.blog.epnwcf.com/Article/details/gixjumhdd.sHtML

[G08] 静态方法与属性
来源：http://mobile.tarul.cn/Article/details/gelfesdcv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fktsv.cn/Article/details/gtvaewfbn.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.tarul.cn/Article/details/gfnuhlazp.sHtML

JS:   static f() {}
来源：http://m.share.tarul.cn/Article/details/gobpcnvav.sHtML

TS:   static f(): void {}
来源：http://m.share.vehdjk.com/Article/details/gnbzcefjf.sHtML

Java: static void f() {}
来源：http://www.blog.vehdjk.com/Article/details/gvhxrsxhk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.tarul.cn/Article/details/gtlgdxusn.sHtML

Ruby: def self.f; end
来源：http://www.m.share.yfazqb.com/Article/details/gffthdmma.sHtML

C#:   public static void F() {}
来源：http://wap.vehdjk.com/Article/details/gklxtjyjs.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.yfazqb.com/Article/details/gwmwofmym.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.yfazqb.com/Article/details/gfpdersyy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fktsv.cn/Article/details/gjdfahztz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.vehdjk.com/Article/details/gbcbywxcz.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.yfazqb.com/Article/details/gnknkfguh.sHtML

Java: interface Shape { double area(); }
来源：http://baike.vehdjk.com/Article/details/gshjydjbo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.vehdjk.com/Article/details/gvomhqezv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.vehdjk.com/Article/details/geslizkbo.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.yfazqb.com/Article/details/gpfuuzzsr.sHtML

[G10] 访问控制
来源：http://m.share.sjlbkw.cn/Article/details/grxuepoyt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.sjlbkw.cn/Article/details/gempyohha.sHtML

PHP:  public / protected / private
来源：http://read.share.yfazqb.com/Article/details/gpdmamyrg.sHtML

JS:   #private 字段；其余公开
来源：http://baike.yfazqb.com/Article/details/gpcbioouh.sHtML

TS:   public / protected / private
来源：http://blog.yfazqb.com/Article/details/goreisvuv.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fktsv.cn/Article/details/gktqwabyy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.epnwcf.com/Article/details/gagnlzwmz.sHtML

Ruby: public / protected / private
来源：http://baike.sjlbkw.cn/Article/details/gvmbzmkpb.sHtML

C#:   public / protected / private / internal
来源：http://blog.yfazqb.com/Article/details/gofywifqr.sHtML

[G11] getter / setter
来源：http://www.share.bbcook.cn/Article/details/ggbujmgiz.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fktsv.cn/Article/details/gcwwbtbiz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.epnwcf.com/Article/details/gbyuzajcc.sHtML

JS:   get name() { return this._name; }
来源：http://3g.tarul.cn/Article/details/gpfeimytg.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.vehdjk.com/Article/details/ghxmmvlhh.sHtML

Java: public String getName() { return name; }
来源：http://3g.epnwcf.com/Article/details/golmxgbhs.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fktsv.cn/Article/details/gbrnuhahw.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.sjlbkw.cn/Article/details/ggonfduwp.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.bbcook.cn/Article/details/gzexrqlds.sHtML

[G12] 对象转字符串
来源：http://read.share.vehdjk.com/Article/details/gasniybtq.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.tarul.cn/Article/details/gkabwfhcw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.yfazqb.com/Article/details/galmcraew.sHtML

JS:   toString() { return this.name; }
来源：http://wap.sjlbkw.cn/Article/details/gykuhkndq.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/gmhwiyjqj.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.yfazqb.com/Article/details/gaxvsbagj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.sjlbkw.cn/Article/details/goekqirxz.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.bbcook.cn/Article/details/gwqaqydrv.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.vehdjk.com/Article/details/gkuagetkl.sHtML

[G13] 判断对象类型
来源：http://3g.bbcook.cn/Article/details/gcockbwns.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.vehdjk.com/Article/details/gyyuastlc.sHtML

PHP:  $u instanceof User
来源：http://baike.vehdjk.com/Article/details/gtrxnxjad.sHtML

JS:   u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/gtzfvovse.sHtML

TS:   u instanceof User
来源：http://blog.yfazqb.com/Article/details/gdfrmlaor.sHtML

Java: u instanceof User
来源：http://wap.epnwcf.com/Article/details/gievbrsoq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.epnwcf.com/Article/details/gukzoqjvg.sHtML

Ruby: u.is_a?(User)
来源：http://baike.epnwcf.com/Article/details/gxgcbweyb.sHtML

C#:   u is User
来源：http://wap.vehdjk.com/Article/details/gqemuryhr.sHtML

[G14] 数据类 / record
来源：http://www.m.share.bbcook.cn/Article/details/gbwgabtoj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.bbcook.cn/Article/details/gmcueszjc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.tarul.cn/Article/details/gmbodmbcn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.bbcook.cn/Article/details/gokyqodks.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.vehdjk.com/Article/details/gviccwdls.sHtML

Java: record User(String name, int age) {}
来源：http://blog.epnwcf.com/Article/details/gfehqxfyg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.vehdjk.com/Article/details/gedfpbmfp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.vehdjk.com/Article/details/gowzsycbc.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.sjlbkw.cn/Article/details/glpnteeyu.sHtML

[G15] 枚举
来源：http://mobile.epnwcf.com/Article/details/gxvpzuawa.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.bbcook.cn/Article/details/gbeqiavta.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.epnwcf.com/Article/details/gkfrbgzry.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.bbcook.cn/Article/details/gjjghammn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.epnwcf.com/Article/details/guzaruznt.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.tarul.cn/Article/details/gxufqnimx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.sjlbkw.cn/Article/details/gglzzrxgx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.bbcook.cn/Article/details/gmfxtargk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fktsv.cn/Article/details/gjlgflvoh.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.vehdjk.com/Article/details/gyjhzshdb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.yfazqb.com/Article/details/ghcbgkich.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.vehdjk.com/Article/details/gnzcojjmt.sHtML

JS:   Object.entries(obj)
来源：http://www.share.epnwcf.com/Article/details/gpvmefisq.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gcqaptvqo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.epnwcf.com/Article/details/gwevgirzi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.epnwcf.com/Article/details/gmatmomlh.sHtML

Ruby: obj.instance_variables
来源：http://www.share.sjlbkw.cn/Article/details/gvvgtyigo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.bbcook.cn/Article/details/glrunmzqb.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gyzmktlfr.sHtML

H. 异常与错误处理
来源：http://mobile.bbcook.cn/Article/details/gojessooh.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/ghnxdwwcy.sHtML

[H01] try / catch 基础
来源：http://www.blog.fktsv.cn/Article/details/ggfauennd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.yfazqb.com/Article/details/gjjroxtzm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.bbcook.cn/Article/details/gfqkjqrlf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fktsv.cn/Article/details/gzkmhfpts.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.bbcook.cn/Article/details/guspbleuc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.bbcook.cn/Article/details/gzbjnpqke.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.tarul.cn/Article/details/gaffpadwm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.yfazqb.com/Article/details/glkfbxqvr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fktsv.cn/Article/details/gmlxzyycl.sHtML

[H02] finally / ensure 收尾
来源：http://baike.yfazqb.com/Article/details/ghgxybfre.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.bbcook.cn/Article/details/ghelhpumr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gddwacjkr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gemisfzva.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gcipbbtvh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.bbcook.cn/Article/details/gtmmthraw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.yfazqb.com/Article/details/gtjkidsxs.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.epnwcf.com/Article/details/gzvixegte.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.yfazqb.com/Article/details/geieikufq.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.vehdjk.com/Article/details/gcqzvzxel.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.sjlbkw.cn/Article/details/gxlmerokg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/gdfplunhz.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.epnwcf.com/Article/details/gvpcjcegb.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gqjnfwlob.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gqyurhldo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.bbcook.cn/Article/details/ghazujoyr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.epnwcf.com/Article/details/gxraozfch.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gzjaprbkg.sHtML

[H04] 自定义异常类型
来源：http://read.share.tarul.cn/Article/details/gnlhooivy.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.vehdjk.com/Article/details/gktebyzlk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.yfazqb.com/Article/details/gqepibzex.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.bbcook.cn/Article/details/gcskdbvtn.sHtML

TS:   class MyError extends Error {}
来源：http://blog.tarul.cn/Article/details/gswcvkwau.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.tarul.cn/Article/details/gsuaxgawj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fktsv.cn/Article/details/gsrirpjvm.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.tarul.cn/Article/details/geuyxnokc.sHtML

C#:   class MyException : Exception {}
来源：http://3g.bbcook.cn/Article/details/gqmuwmxpk.sHtML

[H05] 捕获特定类型
来源：http://blog.epnwcf.com/Article/details/gwvenvezn.sHtML

Py:   except ValueError as e:
来源：http://www.blog.yfazqb.com/Article/details/ggafhanct.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.epnwcf.com/Article/details/gxmdzzjjf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.yfazqb.com/Article/details/ghsqjsgzb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.tarul.cn/Article/details/ghfwicpgc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.bbcook.cn/Article/details/gsptkgsgg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.epnwcf.com/Article/details/ghqjqejqx.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fktsv.cn/Article/details/geczkcuvv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.epnwcf.com/Article/details/gklzwknsq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.yfazqb.com/Article/details/gzkzqvjie.sHtML

Py:   value = d.get("k") or default
来源：http://blog.vehdjk.com/Article/details/gmpnyfccl.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.tarul.cn/Article/details/gdhbyfqrw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.bbcook.cn/Article/details/gnlmpunqw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.bbcook.cn/Article/details/graifbikl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fktsv.cn/Article/details/gnfpftxwo.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.epnwcf.com/Article/details/gihtrmcpa.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.tarul.cn/Article/details/gvseuhhwr.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fktsv.cn/Article/details/gaecxymkt.sHtML

[H07] 断言
来源：http://www.share.fktsv.cn/Article/details/gmasybggl.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.bbcook.cn/Article/details/glbseskeb.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fktsv.cn/Article/details/gopdgwjme.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fktsv.cn/Article/details/galbtvlrv.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.bbcook.cn/Article/details/geptpkkig.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.bbcook.cn/Article/details/gsghhmbvh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.epnwcf.com/Article/details/goguqxdmt.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fktsv.cn/Article/details/gapunrwuq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.epnwcf.com/Article/details/ggimgiefi.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.tarul.cn/Article/details/gstrivbrh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.yfazqb.com/Article/details/gpclujqdi.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.bbcook.cn/Article/details/gcpkpxmar.sHtML

JS:   e.message;  e.stack
来源：http://wap.tarul.cn/Article/details/ghrthjjmb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.tarul.cn/Article/details/gbgbfjqui.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.bbcook.cn/Article/details/ghizdvyjc.sHtML

Go:   err.Error()
来源：http://m.share.fktsv.cn/Article/details/gsgvjerfz.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.tarul.cn/Article/details/gggbvvtpe.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.bbcook.cn/Article/details/goetuzzrq.sHtML

[H09] 带错误码的异常
来源：http://www.share.sjlbkw.cn/Article/details/gwzwuavfg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.vehdjk.com/Article/details/gmtpkpyjy.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.sjlbkw.cn/Article/details/galujgupp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.fktsv.cn/Article/details/gielkfwck.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.sjlbkw.cn/Article/details/gqdbedkbn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.sjlbkw.cn/Article/details/gqkrakhny.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.tarul.cn/Article/details/ghgminuos.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.sjlbkw.cn/Article/details/ghejsibkx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.tarul.cn/Article/details/gvxjfxgax.sHtML

[H10] 资源自动释放
来源：http://m.share.yfazqb.com/Article/details/gpbjislxv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.sjlbkw.cn/Article/details/gatcrxgne.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.vehdjk.com/Article/details/gmohyxekm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.sjlbkw.cn/Article/details/grywwmoyu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.yfazqb.com/Article/details/gquujcpdu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fktsv.cn/Article/details/glftizzee.sHtML

Go:   defer f.Close()
来源：http://www.m.share.tarul.cn/Article/details/gytrkljjl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.bbcook.cn/Article/details/ggstkpusv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gjeohsgrn.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gfcoldbhr.sHtML

I. 正则表达式
来源：http://www.blog.fktsv.cn/Article/details/gofjdyrab.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gzmqfbwav.sHtML

[I01] 判断是否匹配
来源：http://wap.sjlbkw.cn/Article/details/gnspgtkpw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.fktsv.cn/Article/details/gfpjmddmv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.tarul.cn/Article/details/gavgvjfvl.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.yfazqb.com/Article/details/gsmubioak.sHtML

TS:   /\d+/.test(s)
来源：http://blog.sjlbkw.cn/Article/details/gfaoxlqtt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.yfazqb.com/Article/details/gtzwqyqrf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fktsv.cn/Article/details/gtqqjkktg.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.sjlbkw.cn/Article/details/gojijwiuh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.sjlbkw.cn/Article/details/gnslsslqo.sHtML

[I02] 提取所有匹配
来源：http://blog.tarul.cn/Article/details/gufcjfqxc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.epnwcf.com/Article/details/ggavymdfn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.tarul.cn/Article/details/gvfwpaokk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.bbcook.cn/Article/details/gjbljrxwi.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fktsv.cn/Article/details/ghlkqxbbk.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.sjlbkw.cn/Article/details/gidbemcmu.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.bbcook.cn/Article/details/gxwzppczy.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.yfazqb.com/Article/details/grhdeckgm.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.fktsv.cn/Article/details/gvxsotmwa.sHtML

[I03] 提取捕获分组
来源：http://blog.yfazqb.com/Article/details/gvnjanyfg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.vehdjk.com/Article/details/gxhfjfmlw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.bbcook.cn/Article/details/gtwtdvrfo.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.epnwcf.com/Article/details/gicqwrozi.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.yfazqb.com/Article/details/gvbhbtyxf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.tarul.cn/Article/details/gcxkpkdja.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.sjlbkw.cn/Article/details/gmcwdzhlh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.yfazqb.com/Article/details/gzlzbhicn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.vehdjk.com/Article/details/gnxrxlqir.sHtML

[I04] 正则替换
来源：http://read.share.epnwcf.com/Article/details/gyxxmrhdg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.epnwcf.com/Article/details/gtfcuarzh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.epnwcf.com/Article/details/guokfkxvj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gblopscfs.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.epnwcf.com/Article/details/gabyvrsvh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.sjlbkw.cn/Article/details/ghrdhkjgh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.tarul.cn/Article/details/gitwvhniu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.fktsv.cn/Article/details/gkuugoqhi.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.sjlbkw.cn/Article/details/gueivcyeu.sHtML

[I05] 按正则拆分
来源：http://www.share.yfazqb.com/Article/details/gfjhucgub.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.tarul.cn/Article/details/gvjvfaqdr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.vehdjk.com/Article/details/gjcyovjbo.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.sjlbkw.cn/Article/details/glewiamwg.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.tarul.cn/Article/details/gvmlzsysn.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.sjlbkw.cn/Article/details/gnqgcngiz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.epnwcf.com/Article/details/gdubqmcjf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.sjlbkw.cn/Article/details/goepbyodg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.sjlbkw.cn/Article/details/gcycoiddw.sHtML


<!-- 参考信息 -->