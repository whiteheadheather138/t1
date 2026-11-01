代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.sjlbkw.cn/Article/details/gewxtiqir.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.sjlbkw.cn/Article/details/ggwwshtga.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.vehdjk.com/Article/details/gbulxpxis.sHtML

TS:   // 同上
来源：http://m.share.vehdjk.com/Article/details/gfifsiokd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.tarul.cn/Article/details/givtlysui.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.vehdjk.com/Article/details/gowwhumkc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.vehdjk.com/Article/details/gqlghnoqg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.yfazqb.com/Article/details/gpeptcdif.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gkadimioy.sHtML

G. 面向对象
来源：http://read.share.sjlbkw.cn/Article/details/gwbiajyuj.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/ghkfawaly.sHtML

[G01] 定义类
来源：http://m.share.tarul.cn/Article/details/gdogdcjdy.sHtML

Py:   class User: pass
来源：http://baike.sjlbkw.cn/Article/details/gmdnmmnlx.sHtML

PHP:  class User {}
来源：http://3g.epnwcf.com/Article/details/gagznhdng.sHtML

JS:   class User {}
来源：http://baike.sjlbkw.cn/Article/details/gwswmlbzq.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.bbcook.cn/Article/details/gorejktua.sHtML

Java: class User {}
来源：http://baike.yfazqb.com/Article/details/gcyfhrqpw.sHtML

Go:   type User struct { Name string }
来源：http://read.share.yfazqb.com/Article/details/gmkztbnte.sHtML

Ruby: class User; end
来源：http://www.blog.vehdjk.com/Article/details/guelnrhlp.sHtML

C#:   class User {}
来源：http://www.share.yfazqb.com/Article/details/gxjenoybi.sHtML

[G02] 构造函数
来源：http://www.share.sjlbkw.cn/Article/details/gbijlfsjy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.yfazqb.com/Article/details/gauydmqkt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.sjlbkw.cn/Article/details/ghkpubnjt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fktsv.cn/Article/details/gxnahxcor.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.tarul.cn/Article/details/gcjtumhoz.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.bbcook.cn/Article/details/gszwbjthn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.epnwcf.com/Article/details/gettkvpll.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.sjlbkw.cn/Article/details/genpprhbd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.sjlbkw.cn/Article/details/gcqckqehd.sHtML

[G03] 实例属性
来源：http://wap.bbcook.cn/Article/details/gtgddwalu.sHtML

Py:   self.name = "x"
来源：http://read.share.bbcook.cn/Article/details/grtgltthc.sHtML

PHP:  public string $name = "x";
来源：http://www.share.bbcook.cn/Article/details/gwduvagoz.sHtML

JS:   this.name = "x";
来源：http://www.share.sjlbkw.cn/Article/details/gpaphlusq.sHtML

TS:   name: string = "x";
来源：http://www.m.share.bbcook.cn/Article/details/gcirtwvkg.sHtML

Java: private String name;
来源：http://wap.vehdjk.com/Article/details/gtufmnnrm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.vehdjk.com/Article/details/gamellcul.sHtML

Ruby: @name = "x"
来源：http://mobile.bbcook.cn/Article/details/girplzohm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.epnwcf.com/Article/details/grjtlsccm.sHtML

[G04] 定义方法
来源：http://www.m.share.tarul.cn/Article/details/gdhmzcrvs.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.tarul.cn/Article/details/galomiizu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/gnylqpuzb.sHtML

JS:   greet() { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gqutflsty.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/ggrdttmgo.sHtML

Java: String greet() { return name; }
来源：http://mobile.bbcook.cn/Article/details/gljhuhklw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.sjlbkw.cn/Article/details/gupghqvpm.sHtML

Ruby: def greet; @name; end
来源：http://m.share.vehdjk.com/Article/details/gplmihnjq.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.sjlbkw.cn/Article/details/gwmytrbyg.sHtML

[G05] 继承
来源：http://m.share.yfazqb.com/Article/details/gbrbidhxo.sHtML

Py:   class Admin(User): pass
来源：http://wap.vehdjk.com/Article/details/gpslinrpt.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gmmbhuvom.sHtML

JS:   class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/gmouxauta.sHtML

TS:   class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gbynlfsxt.sHtML

Java: class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/gpkdowoqb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.sjlbkw.cn/Article/details/gxynvdmlu.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fktsv.cn/Article/details/ggdlhrzqt.sHtML

C#:   class Admin : User {}
来源：http://www.share.yfazqb.com/Article/details/gqumdzzmu.sHtML

[G06] 重写方法
来源：http://www.blog.yfazqb.com/Article/details/ghscgtdjf.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.vehdjk.com/Article/details/gkokkftya.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.tarul.cn/Article/details/gqodosmkj.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fktsv.cn/Article/details/gbaxclkgz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/gwwhpzbxq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/gvnajvhns.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.vehdjk.com/Article/details/gghumcbou.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.epnwcf.com/Article/details/ggouxitrw.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.yfazqb.com/Article/details/gsvjloymf.sHtML

[G07] 调用父类方法
来源：http://wap.bbcook.cn/Article/details/gnsijajzp.sHtML

Py:   super().greet()
来源：http://read.share.epnwcf.com/Article/details/gbqlhitgy.sHtML

PHP:  parent::greet();
来源：http://www.blog.fktsv.cn/Article/details/gerswxpvh.sHtML

JS:   super.greet();
来源：http://www.blog.epnwcf.com/Article/details/gfkdzgmzm.sHtML

TS:   super.greet();
来源：http://m.share.bbcook.cn/Article/details/gcdtifdhg.sHtML

Java: super.greet();
来源：http://read.share.bbcook.cn/Article/details/grcbnitnl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.yfazqb.com/Article/details/gtobhuvps.sHtML

Ruby: super
来源：http://www.share.bbcook.cn/Article/details/gvowsunpj.sHtML

C#:   base.Greet();
来源：http://www.m.share.yfazqb.com/Article/details/gkusidyfl.sHtML

[G08] 静态方法与属性
来源：http://mobile.fktsv.cn/Article/details/gcxpjtylf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.epnwcf.com/Article/details/gpqgpzdli.sHtML

PHP:  public static function f() {}
来源：http://blog.sjlbkw.cn/Article/details/gkylompgc.sHtML

JS:   static f() {}
来源：http://read.share.sjlbkw.cn/Article/details/gfxqejbqe.sHtML

TS:   static f(): void {}
来源：http://m.share.tarul.cn/Article/details/gltiqlytp.sHtML

Java: static void f() {}
来源：http://3g.vehdjk.com/Article/details/gxbwjmcwx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.yfazqb.com/Article/details/gkuxddljn.sHtML

Ruby: def self.f; end
来源：http://3g.bbcook.cn/Article/details/gwajfzcxw.sHtML

C#:   public static void F() {}
来源：http://baike.vehdjk.com/Article/details/ghjmplmcm.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fktsv.cn/Article/details/gznxlacvz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.epnwcf.com/Article/details/gnxefaqtp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.sjlbkw.cn/Article/details/griofydmc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.epnwcf.com/Article/details/gbdekuzih.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.tarul.cn/Article/details/ggzzronfy.sHtML

Java: interface Shape { double area(); }
来源：http://wap.sjlbkw.cn/Article/details/glidwgzyw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.vehdjk.com/Article/details/gshkrdenh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.yfazqb.com/Article/details/gjkstwtct.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.bbcook.cn/Article/details/ghowaizlz.sHtML

[G10] 访问控制
来源：http://www.m.share.bbcook.cn/Article/details/gydwzavlm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.sjlbkw.cn/Article/details/gtpipphac.sHtML

PHP:  public / protected / private
来源：http://read.share.fktsv.cn/Article/details/gdwwzbeku.sHtML

JS:   #private 字段；其余公开
来源：http://3g.tarul.cn/Article/details/gtgjlwbra.sHtML

TS:   public / protected / private
来源：http://3g.fktsv.cn/Article/details/gkptpcuaa.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.bbcook.cn/Article/details/grmqfavee.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.epnwcf.com/Article/details/gvruionzc.sHtML

Ruby: public / protected / private
来源：http://www.blog.fktsv.cn/Article/details/ghqsdwjbz.sHtML

C#:   public / protected / private / internal
来源：http://3g.yfazqb.com/Article/details/gbyeppjyn.sHtML

[G11] getter / setter
来源：http://mobile.vehdjk.com/Article/details/gbdrevzzy.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.bbcook.cn/Article/details/gsnyjhlmu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.yfazqb.com/Article/details/goublbpyo.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fktsv.cn/Article/details/guzltoowi.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.epnwcf.com/Article/details/gpfzgvguf.sHtML

Java: public String getName() { return name; }
来源：http://wap.epnwcf.com/Article/details/gjpujhnww.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.bbcook.cn/Article/details/gpcyiszkn.sHtML

Ruby: attr_accessor :name
来源：http://m.share.bbcook.cn/Article/details/ghsrembow.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.epnwcf.com/Article/details/gvuerhvdf.sHtML

[G12] 对象转字符串
来源：http://www.m.share.epnwcf.com/Article/details/girvbkuxd.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.bbcook.cn/Article/details/gqgoqsciq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.tarul.cn/Article/details/gkmsqerjt.sHtML

JS:   toString() { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/glhtjkvjb.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/gcfdiesgq.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fktsv.cn/Article/details/gcetlvizj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.tarul.cn/Article/details/gvpxtlatk.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.vehdjk.com/Article/details/grlnndiad.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.sjlbkw.cn/Article/details/gnnlpcaaw.sHtML

[G13] 判断对象类型
来源：http://blog.yfazqb.com/Article/details/giwpejgnc.sHtML

Py:   isinstance(u, User)
来源：http://blog.bbcook.cn/Article/details/gvcytoaow.sHtML

PHP:  $u instanceof User
来源：http://baike.vehdjk.com/Article/details/gfibmpsll.sHtML

JS:   u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/gnlsfcdrv.sHtML

TS:   u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/gkjvcjept.sHtML

Java: u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/gbgiyuing.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.sjlbkw.cn/Article/details/gcmhxtrsf.sHtML

Ruby: u.is_a?(User)
来源：http://blog.tarul.cn/Article/details/glelpvlac.sHtML

C#:   u is User
来源：http://blog.sjlbkw.cn/Article/details/gzoaqbxxu.sHtML

[G14] 数据类 / record
来源：http://baike.bbcook.cn/Article/details/gowirxapz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.bbcook.cn/Article/details/gxbrsqgbi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fktsv.cn/Article/details/gxxkflkzm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.bbcook.cn/Article/details/grqfgzrlw.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.sjlbkw.cn/Article/details/gcdsenndf.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fktsv.cn/Article/details/gcxkpjnie.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.tarul.cn/Article/details/gwxaxofey.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.vehdjk.com/Article/details/gmhqvwnnk.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fktsv.cn/Article/details/gisewggkm.sHtML

[G15] 枚举
来源：http://read.share.sjlbkw.cn/Article/details/gjbtnzoqu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.vehdjk.com/Article/details/gddtziiwy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.yfazqb.com/Article/details/gvlcndlpw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.yfazqb.com/Article/details/gojmpraav.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.bbcook.cn/Article/details/gynkzepfk.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.tarul.cn/Article/details/grkdhqfmv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.tarul.cn/Article/details/gzxpllyky.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.tarul.cn/Article/details/gvuwocata.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.bbcook.cn/Article/details/gnalphrzl.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.bbcook.cn/Article/details/geijmafso.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.epnwcf.com/Article/details/gnsrtrtte.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.yfazqb.com/Article/details/gbhnrfqgy.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.tarul.cn/Article/details/gfcpmixsj.sHtML

TS:   Object.entries(obj)
来源：http://3g.tarul.cn/Article/details/geakjlbtz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.bbcook.cn/Article/details/gfyytvkxs.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.tarul.cn/Article/details/ggoheyueg.sHtML

Ruby: obj.instance_variables
来源：http://read.share.tarul.cn/Article/details/gtalmkmkr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.yfazqb.com/Article/details/gtzaikyuj.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gltssvqti.sHtML

H. 异常与错误处理
来源：http://wap.vehdjk.com/Article/details/gpukllfxm.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gsjkmicuw.sHtML

[H01] try / catch 基础
来源：http://wap.epnwcf.com/Article/details/gmmmvwbhb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.vehdjk.com/Article/details/gdyirkbdz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.epnwcf.com/Article/details/gafwtiamc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.bbcook.cn/Article/details/gdfduwqnk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.tarul.cn/Article/details/gcskwglfj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.tarul.cn/Article/details/giccnurnz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.vehdjk.com/Article/details/gzhypgjxi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.vehdjk.com/Article/details/grvqtiesu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.yfazqb.com/Article/details/gzqycpeyd.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.bbcook.cn/Article/details/gcunwkxnb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.yfazqb.com/Article/details/gvhnfkrib.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gsrkdtong.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.yfazqb.com/Article/details/ghsgvrrhe.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gcdfweous.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gmqvnqodu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fktsv.cn/Article/details/gsciisggy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.bbcook.cn/Article/details/gwbtxxthc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gdndopwzw.sHtML

[H03] 主动抛出异常
来源：http://m.share.bbcook.cn/Article/details/gltpxjsnw.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.epnwcf.com/Article/details/ganzqicxq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fktsv.cn/Article/details/ghymesuho.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fktsv.cn/Article/details/gqzgfcopq.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/gsnsjsbfv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.vehdjk.com/Article/details/gxzjrtpcn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.epnwcf.com/Article/details/gzhnqhmxs.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.yfazqb.com/Article/details/gxuailoqi.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/gkqnlbddf.sHtML

[H04] 自定义异常类型
来源：http://blog.fktsv.cn/Article/details/gwpdjfyoh.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdgeljxm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fktsv.cn/Article/details/gcftrhpms.sHtML

JS:   class MyError extends Error {}
来源：http://baike.tarul.cn/Article/details/gyhnaihpg.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.yfazqb.com/Article/details/gazcttphk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.tarul.cn/Article/details/gmqzsksbl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fktsv.cn/Article/details/gpntnctck.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.bbcook.cn/Article/details/gcwfbrhao.sHtML

C#:   class MyException : Exception {}
来源：http://3g.epnwcf.com/Article/details/glojwpumk.sHtML

[H05] 捕获特定类型
来源：http://m.share.tarul.cn/Article/details/guuqywpyh.sHtML

Py:   except ValueError as e:
来源：http://www.share.epnwcf.com/Article/details/gohkuyzzt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fktsv.cn/Article/details/gvazgeopp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.sjlbkw.cn/Article/details/gsuslrbfj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fktsv.cn/Article/details/gqpxvkgxm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fktsv.cn/Article/details/gknuvdaqj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.tarul.cn/Article/details/guruxmkwz.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.sjlbkw.cn/Article/details/gwxsinmnb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.epnwcf.com/Article/details/gdztkduqm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.tarul.cn/Article/details/gvrmmayvb.sHtML

Py:   value = d.get("k") or default
来源：http://baike.epnwcf.com/Article/details/gfeucseqx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.sjlbkw.cn/Article/details/gxjrrelih.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.tarul.cn/Article/details/ggutqtgho.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.yfazqb.com/Article/details/guuxgcgyg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.tarul.cn/Article/details/gawfvmout.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.bbcook.cn/Article/details/gryzapvua.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.yfazqb.com/Article/details/grbrvlhtz.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.sjlbkw.cn/Article/details/gskioiuan.sHtML

[H07] 断言
来源：http://blog.fktsv.cn/Article/details/gcfrsdhyi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.bbcook.cn/Article/details/gdpvwsqdw.sHtML

PHP:  assert($x > 0);
来源：http://baike.vehdjk.com/Article/details/gzhccoqlq.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fktsv.cn/Article/details/gqhvukspd.sHtML

TS:   console.assert(x > 0);
来源：http://3g.bbcook.cn/Article/details/ggpxqhddh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.yfazqb.com/Article/details/gxokjbscv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.vehdjk.com/Article/details/gvxkshqsg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.sjlbkw.cn/Article/details/gfuqtuhvb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.tarul.cn/Article/details/gjodxytmb.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.tarul.cn/Article/details/gxunyefer.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.tarul.cn/Article/details/gmegcrpbf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.bbcook.cn/Article/details/gxujofahq.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.epnwcf.com/Article/details/gqgkgpkhk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.sjlbkw.cn/Article/details/gseqggogd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.bbcook.cn/Article/details/goewroeyf.sHtML

Go:   err.Error()
来源：http://baike.bbcook.cn/Article/details/gaipwnbye.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.yfazqb.com/Article/details/gytarlngz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.yfazqb.com/Article/details/gdenveodc.sHtML

[H09] 带错误码的异常
来源：http://m.share.yfazqb.com/Article/details/graznjzqn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.sjlbkw.cn/Article/details/gvgpkjamk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.bbcook.cn/Article/details/gvbpmfyzw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.bbcook.cn/Article/details/gwkxpaolh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.vehdjk.com/Article/details/gbbysedjz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fktsv.cn/Article/details/gdblcdjkb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.epnwcf.com/Article/details/gwkiqyets.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.tarul.cn/Article/details/gjwtlbpwv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fktsv.cn/Article/details/gnqkhhwrv.sHtML

[H10] 资源自动释放
来源：http://blog.vehdjk.com/Article/details/gtybfwzwb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.tarul.cn/Article/details/gzjklitrz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.tarul.cn/Article/details/geaivbauk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.yfazqb.com/Article/details/gslagzymd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.tarul.cn/Article/details/gtpjhlvzu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fktsv.cn/Article/details/glhhfewbz.sHtML

Go:   defer f.Close()
来源：http://www.m.share.tarul.cn/Article/details/gfpekqpyx.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.bbcook.cn/Article/details/gfjbdrbnu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.tarul.cn/Article/details/gpyztcohs.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gwrtcyrct.sHtML

I. 正则表达式
来源：http://blog.yfazqb.com/Article/details/gvgdjbgxy.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/ghptzlxrt.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.epnwcf.com/Article/details/grwkbnkcw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.yfazqb.com/Article/details/gcolaawdp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gshinnpzv.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzugesgmf.sHtML

TS:   /\d+/.test(s)
来源：http://blog.vehdjk.com/Article/details/guuwjbkxo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.tarul.cn/Article/details/gacsscppd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.bbcook.cn/Article/details/gbfmalczk.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.tarul.cn/Article/details/gejhvlgvr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.tarul.cn/Article/details/giguvtydi.sHtML

[I02] 提取所有匹配
来源：http://baike.bbcook.cn/Article/details/goqonxdnb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.fktsv.cn/Article/details/grblvmmuw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.vehdjk.com/Article/details/gubpsnynq.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.epnwcf.com/Article/details/gtgrspmoi.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.tarul.cn/Article/details/galchlqal.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fktsv.cn/Article/details/ghzxhrybe.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fktsv.cn/Article/details/gvoxnrhkh.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.yfazqb.com/Article/details/genhoqdbo.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.fktsv.cn/Article/details/glntlmbsl.sHtML

[I03] 提取捕获分组
来源：http://blog.tarul.cn/Article/details/gdtdbshjp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.yfazqb.com/Article/details/gcvxwkjgg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.sjlbkw.cn/Article/details/gqbdzlkii.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.yfazqb.com/Article/details/gxglrxgpg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.tarul.cn/Article/details/glqtzwngl.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.bbcook.cn/Article/details/ggzdnzzmf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.bbcook.cn/Article/details/gxqzeaxfs.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.sjlbkw.cn/Article/details/ghwslbptw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.yfazqb.com/Article/details/gnovwjqwt.sHtML

[I04] 正则替换
来源：http://www.share.yfazqb.com/Article/details/ggjtzikyw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.vehdjk.com/Article/details/gpyutigco.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.bbcook.cn/Article/details/gkyvextli.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.vehdjk.com/Article/details/ggyxamkhi.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.vehdjk.com/Article/details/gyhdoticg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.sjlbkw.cn/Article/details/gxplpswiy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.tarul.cn/Article/details/gwblyafpn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.yfazqb.com/Article/details/gsompnahk.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.yfazqb.com/Article/details/gvoefcudc.sHtML

[I05] 按正则拆分
来源：http://m.share.fktsv.cn/Article/details/gsfndajwa.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.vehdjk.com/Article/details/ghyvbvbdz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gtngpiuxd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.tarul.cn/Article/details/gdgbjxqvo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.fktsv.cn/Article/details/gmrfhkxnr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnzbqsze.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.vehdjk.com/Article/details/glailusjx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.yfazqb.com/Article/details/goiwejacd.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.epnwcf.com/Article/details/gcmbnlrua.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.bbcook.cn/Article/details/gamhlwhhh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.sjlbkw.cn/Article/details/gqotzhinz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.epnwcf.com/Article/details/gxrgxsrox.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.bbcook.cn/Article/details/gohvgvbfn.sHtML


<!-- 参考信息 -->