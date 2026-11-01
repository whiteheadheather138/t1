代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://baike.epnwcf.com/Article/details/gfpnzswbb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.vehdjk.com/Article/details/gulewvblg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gamqjwrdp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.tarul.cn/Article/details/gdyelrqsc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gfhqcohtf.sHtML

TS:   path.extname("a.txt")
来源：http://3g.bbcook.cn/Article/details/gaxvsdrcc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.bbcook.cn/Article/details/gjdgkxcjk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/gbgpypxqy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/gbogoaazl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/geppitlos.sHtML

[F11] 复制与移动文件
来源：http://www.blog.yfazqb.com/Article/details/gezkaunox.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/grwaxafkm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.tarul.cn/Article/details/gjgjerimo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/gqzrrdakj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.bbcook.cn/Article/details/goesfmvrt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.yfazqb.com/Article/details/glfxzlxqu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.sjlbkw.cn/Article/details/gopihapnj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.epnwcf.com/Article/details/gaxvrlpmd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.bbcook.cn/Article/details/geuuswwiz.sHtML

[F12] CSV 读写
来源：http://mobile.epnwcf.com/Article/details/gjjguzrnd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fktsv.cn/Article/details/gkxfnbjaa.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.vehdjk.com/Article/details/gdbujiafc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.tarul.cn/Article/details/gdkxjdxif.sHtML

TS:   // 同上
来源：http://mobile.bbcook.cn/Article/details/gqnuaveeo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.yfazqb.com/Article/details/ggkvlkzwt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.vehdjk.com/Article/details/gqhbqspkb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.bbcook.cn/Article/details/gvdwhersf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.bbcook.cn/Article/details/gdqonutiw.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gqwomtsdo.sHtML

G. 面向对象
来源：http://read.share.tarul.cn/Article/details/gekyclqii.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gxdpxcdoi.sHtML

[G01] 定义类
来源：http://www.m.share.tarul.cn/Article/details/gykhzmqtp.sHtML

Py:   class User: pass
来源：http://blog.tarul.cn/Article/details/gvdmwnihq.sHtML

PHP:  class User {}
来源：http://read.share.vehdjk.com/Article/details/gzbexegys.sHtML

JS:   class User {}
来源：http://read.share.fktsv.cn/Article/details/gjawwtjkt.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fktsv.cn/Article/details/gcoggbgve.sHtML

Java: class User {}
来源：http://wap.bbcook.cn/Article/details/gvrglouym.sHtML

Go:   type User struct { Name string }
来源：http://baike.yfazqb.com/Article/details/giauilnux.sHtML

Ruby: class User; end
来源：http://3g.sjlbkw.cn/Article/details/gjarifprj.sHtML

C#:   class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gvaoilgod.sHtML

[G02] 构造函数
来源：http://mobile.tarul.cn/Article/details/gfzuryadi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.vehdjk.com/Article/details/gzstzfnbv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.vehdjk.com/Article/details/godxhvfdl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.epnwcf.com/Article/details/guqgswnzq.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fktsv.cn/Article/details/gwcboiyru.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.vehdjk.com/Article/details/gbfdhqobv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.vehdjk.com/Article/details/ggaofxsmn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.tarul.cn/Article/details/gnhkgfgby.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/gkjbrfpoj.sHtML

[G03] 实例属性
来源：http://www.m.share.bbcook.cn/Article/details/gejlztaie.sHtML

Py:   self.name = "x"
来源：http://blog.epnwcf.com/Article/details/gnktpvvyq.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.bbcook.cn/Article/details/gaquyzmcs.sHtML

JS:   this.name = "x";
来源：http://www.m.share.vehdjk.com/Article/details/gupybffoi.sHtML

TS:   name: string = "x";
来源：http://wap.vehdjk.com/Article/details/grvhhyoqg.sHtML

Java: private String name;
来源：http://mobile.vehdjk.com/Article/details/gvhzbwrea.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.epnwcf.com/Article/details/gypsortbd.sHtML

Ruby: @name = "x"
来源：http://mobile.bbcook.cn/Article/details/gdxeavmxv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.bbcook.cn/Article/details/gzktbbzco.sHtML

[G04] 定义方法
来源：http://mobile.fktsv.cn/Article/details/gcvjgdrjp.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.epnwcf.com/Article/details/ghtzepktp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.bbcook.cn/Article/details/gddfckqwo.sHtML

JS:   greet() { return this.name; }
来源：http://blog.tarul.cn/Article/details/glzmpaqrh.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/grsdejqxo.sHtML

Java: String greet() { return name; }
来源：http://baike.bbcook.cn/Article/details/gvrzgarmz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.sjlbkw.cn/Article/details/gvvzosqlz.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fktsv.cn/Article/details/gzuobtjgn.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fktsv.cn/Article/details/gkzvpyhvs.sHtML

[G05] 继承
来源：http://wap.bbcook.cn/Article/details/gbsipkxxy.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.vehdjk.com/Article/details/gwzolrxje.sHtML

PHP:  class Admin extends User {}
来源：http://baike.epnwcf.com/Article/details/gefmzplzw.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gezyxwnhc.sHtML

TS:   class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gsjysyqrn.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/gkmuoxpvy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.bbcook.cn/Article/details/gdhxzwvem.sHtML

Ruby: class Admin < User; end
来源：http://read.share.yfazqb.com/Article/details/gowouekxr.sHtML

C#:   class Admin : User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gpgruwjaf.sHtML

[G06] 重写方法
来源：http://www.blog.vehdjk.com/Article/details/giyezofkx.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.bbcook.cn/Article/details/gwyavmskp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/glzgzzmqs.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/gidsioniq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/gufvhfyfy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.epnwcf.com/Article/details/gbtrblgnz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.vehdjk.com/Article/details/gqvjxnfnr.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fktsv.cn/Article/details/gnsllgwuq.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.epnwcf.com/Article/details/gurraqgmc.sHtML

[G07] 调用父类方法
来源：http://www.blog.tarul.cn/Article/details/gynvzszfm.sHtML

Py:   super().greet()
来源：http://mobile.bbcook.cn/Article/details/gntmxnosh.sHtML

PHP:  parent::greet();
来源：http://3g.fktsv.cn/Article/details/grywzrzjt.sHtML

JS:   super.greet();
来源：http://www.blog.vehdjk.com/Article/details/gsbogizpj.sHtML

TS:   super.greet();
来源：http://m.share.fktsv.cn/Article/details/gjkvzoonv.sHtML

Java: super.greet();
来源：http://3g.fktsv.cn/Article/details/gispoqinr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.tarul.cn/Article/details/gczjzdnzb.sHtML

Ruby: super
来源：http://read.share.bbcook.cn/Article/details/gmjbhfrxx.sHtML

C#:   base.Greet();
来源：http://www.m.share.fktsv.cn/Article/details/gpnrblctv.sHtML

[G08] 静态方法与属性
来源：http://mobile.tarul.cn/Article/details/guixvdfqj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.yfazqb.com/Article/details/gviloxcih.sHtML

PHP:  public static function f() {}
来源：http://m.share.bbcook.cn/Article/details/gpqaegeiq.sHtML

JS:   static f() {}
来源：http://www.share.yfazqb.com/Article/details/gyqlmfxoz.sHtML

TS:   static f(): void {}
来源：http://mobile.tarul.cn/Article/details/gtfrehaus.sHtML

Java: static void f() {}
来源：http://www.blog.yfazqb.com/Article/details/gjjxfsebc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.vehdjk.com/Article/details/gkducayqw.sHtML

Ruby: def self.f; end
来源：http://www.m.share.epnwcf.com/Article/details/gaxkrdbgl.sHtML

C#:   public static void F() {}
来源：http://m.share.tarul.cn/Article/details/gppvtlkgu.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.sjlbkw.cn/Article/details/gicmaazlq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.epnwcf.com/Article/details/gizxqhlks.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.yfazqb.com/Article/details/gwlysuxzi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.tarul.cn/Article/details/gpxyqmgvr.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.sjlbkw.cn/Article/details/gqsqdgpxo.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.epnwcf.com/Article/details/ggfjhrjyg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.epnwcf.com/Article/details/gemuuqwrk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.epnwcf.com/Article/details/grxhowkbj.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.yfazqb.com/Article/details/gnkelhrnw.sHtML

[G10] 访问控制
来源：http://www.m.share.vehdjk.com/Article/details/gsuhjwzue.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.epnwcf.com/Article/details/gutibvmkc.sHtML

PHP:  public / protected / private
来源：http://m.share.epnwcf.com/Article/details/guvggwjvg.sHtML

JS:   #private 字段；其余公开
来源：http://wap.bbcook.cn/Article/details/grpukhghj.sHtML

TS:   public / protected / private
来源：http://3g.yfazqb.com/Article/details/gfkwbcfsx.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.tarul.cn/Article/details/gtzeddmwa.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.bbcook.cn/Article/details/gudmgtjto.sHtML

Ruby: public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/gjoehjopx.sHtML

C#:   public / protected / private / internal
来源：http://m.share.tarul.cn/Article/details/gedjxyuar.sHtML

[G11] getter / setter
来源：http://read.share.yfazqb.com/Article/details/gdjxhewvp.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.epnwcf.com/Article/details/gqofuelcd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.bbcook.cn/Article/details/gunsgnyrd.sHtML

JS:   get name() { return this._name; }
来源：http://blog.vehdjk.com/Article/details/gzhepjgqq.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.tarul.cn/Article/details/gkhrqreza.sHtML

Java: public String getName() { return name; }
来源：http://blog.vehdjk.com/Article/details/gliysyfrg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.tarul.cn/Article/details/guiccnens.sHtML

Ruby: attr_accessor :name
来源：http://wap.tarul.cn/Article/details/gvobpbjfa.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.bbcook.cn/Article/details/gdaenizsh.sHtML

[G12] 对象转字符串
来源：http://www.m.share.yfazqb.com/Article/details/glcdlgrgb.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.bbcook.cn/Article/details/gljcpzfri.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.tarul.cn/Article/details/gztuvciuj.sHtML

JS:   toString() { return this.name; }
来源：http://blog.tarul.cn/Article/details/gumbrxoxx.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gmtieuvnf.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.yfazqb.com/Article/details/giskxbkuf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/gmqeamhcs.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.epnwcf.com/Article/details/gcyjrmyob.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.sjlbkw.cn/Article/details/grerzuwdb.sHtML

[G13] 判断对象类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gdgwvmbpp.sHtML

Py:   isinstance(u, User)
来源：http://baike.tarul.cn/Article/details/gcqzcucqd.sHtML

PHP:  $u instanceof User
来源：http://mobile.epnwcf.com/Article/details/gyrbbfevc.sHtML

JS:   u instanceof User
来源：http://www.share.bbcook.cn/Article/details/gqlzomizt.sHtML

TS:   u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gsoqgrsze.sHtML

Java: u instanceof User
来源：http://baike.epnwcf.com/Article/details/goqxjbrgg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.yfazqb.com/Article/details/gbrbrauds.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.bbcook.cn/Article/details/goxwzgvcp.sHtML

C#:   u is User
来源：http://m.share.sjlbkw.cn/Article/details/gbgzhtbgh.sHtML

[G14] 数据类 / record
来源：http://baike.fktsv.cn/Article/details/gvurmvztk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.sjlbkw.cn/Article/details/gsclkqaqy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.sjlbkw.cn/Article/details/glfsbymka.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fktsv.cn/Article/details/gizvmfytz.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.yfazqb.com/Article/details/giyjfluec.sHtML

Java: record User(String name, int age) {}
来源：http://wap.epnwcf.com/Article/details/glrhywmxt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.epnwcf.com/Article/details/gsnesazrw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.tarul.cn/Article/details/gdhwcubnw.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.yfazqb.com/Article/details/gxbqanlue.sHtML

[G15] 枚举
来源：http://www.m.share.sjlbkw.cn/Article/details/gksqbvwgn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.sjlbkw.cn/Article/details/geewhtoeq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.yfazqb.com/Article/details/ggjwgjpya.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.yfazqb.com/Article/details/glcsvieqk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.yfazqb.com/Article/details/gzmkvesgq.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.epnwcf.com/Article/details/grgdtquqw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.vehdjk.com/Article/details/gomhiftaw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fktsv.cn/Article/details/gocgvximq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.epnwcf.com/Article/details/gvgxeakev.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.epnwcf.com/Article/details/gbftagphn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.epnwcf.com/Article/details/gldtajgjr.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.vehdjk.com/Article/details/gnwftxvoc.sHtML

JS:   Object.entries(obj)
来源：http://wap.tarul.cn/Article/details/gsbdqzyuq.sHtML

TS:   Object.entries(obj)
来源：http://baike.sjlbkw.cn/Article/details/gkncqxjdw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.yfazqb.com/Article/details/gkuqxfayn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.vehdjk.com/Article/details/guztwxmte.sHtML

Ruby: obj.instance_variables
来源：http://blog.fktsv.cn/Article/details/gcehmhatk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.vehdjk.com/Article/details/gctgylszs.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gjolyqvkq.sHtML

H. 异常与错误处理
来源：http://www.blog.bbcook.cn/Article/details/gdcdzmlne.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/guabdfoqt.sHtML

[H01] try / catch 基础
来源：http://www.m.share.tarul.cn/Article/details/gdmyrbgko.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.tarul.cn/Article/details/glofyhwla.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.bbcook.cn/Article/details/gtlhlfclw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.vehdjk.com/Article/details/gjkzvosak.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.yfazqb.com/Article/details/gxunducbp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.vehdjk.com/Article/details/ggmwkcmzi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.tarul.cn/Article/details/gfdzoltgm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.bbcook.cn/Article/details/gmdnymruw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.vehdjk.com/Article/details/glrwmektv.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fktsv.cn/Article/details/garqnviia.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.epnwcf.com/Article/details/gbsqnthjd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fktsv.cn/Article/details/gcrkrgbrl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/ginomgwzg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gjeurpipf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gbwxlqixq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.yfazqb.com/Article/details/gneomqstl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.epnwcf.com/Article/details/glxwgrtdn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.epnwcf.com/Article/details/ggfjxodsh.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.sjlbkw.cn/Article/details/gzcfpxkdx.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.yfazqb.com/Article/details/gxaneckoh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.yfazqb.com/Article/details/glatzmsyl.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/gfpgeuavp.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.epnwcf.com/Article/details/gxstjziyu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gesranrpj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.bbcook.cn/Article/details/gwyymurll.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.yfazqb.com/Article/details/ghaarukzw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fktsv.cn/Article/details/gtntopbyv.sHtML

[H04] 自定义异常类型
来源：http://3g.yfazqb.com/Article/details/gcnxpiwkq.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.sjlbkw.cn/Article/details/gggygiqfd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fktsv.cn/Article/details/gudwxdrdf.sHtML

JS:   class MyError extends Error {}
来源：http://3g.vehdjk.com/Article/details/gpbvmbfph.sHtML

TS:   class MyError extends Error {}
来源：http://wap.bbcook.cn/Article/details/guzokajyu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.bbcook.cn/Article/details/gqfjmhknv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.yfazqb.com/Article/details/gellnmwct.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.tarul.cn/Article/details/gqwvtdsun.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.epnwcf.com/Article/details/gbjlweipm.sHtML

[H05] 捕获特定类型
来源：http://read.share.epnwcf.com/Article/details/gmuzfymiv.sHtML

Py:   except ValueError as e:
来源：http://read.share.bbcook.cn/Article/details/gzgeekglh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.vehdjk.com/Article/details/gpblafkzo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.vehdjk.com/Article/details/grohdwbnt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.tarul.cn/Article/details/gyqgxddsz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fktsv.cn/Article/details/gzhqvswoj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.tarul.cn/Article/details/gddoejdmo.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.bbcook.cn/Article/details/gcebotccw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.yfazqb.com/Article/details/gaujmtaxd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fktsv.cn/Article/details/ggkxgxmvi.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.tarul.cn/Article/details/gnccbdjjj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.vehdjk.com/Article/details/geineukeh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.sjlbkw.cn/Article/details/gdqtqsfhe.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.bbcook.cn/Article/details/ghjgowcjd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.sjlbkw.cn/Article/details/gbczabmwq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.bbcook.cn/Article/details/gpvafvblo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.bbcook.cn/Article/details/gggsujbih.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.yfazqb.com/Article/details/gcanophsb.sHtML

[H07] 断言
来源：http://baike.bbcook.cn/Article/details/gbgmlhjmi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fktsv.cn/Article/details/gjbefoscc.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.tarul.cn/Article/details/gwhmuotty.sHtML

JS:   console.assert(x > 0);
来源：http://blog.yfazqb.com/Article/details/ghrupljio.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.yfazqb.com/Article/details/gsjuffgez.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.vehdjk.com/Article/details/gpnwkqclc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.yfazqb.com/Article/details/gkwzbymmj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.tarul.cn/Article/details/grnyidsxe.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.bbcook.cn/Article/details/gdevvrwab.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fktsv.cn/Article/details/glqjgsmit.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.tarul.cn/Article/details/gkyfwmuxt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fktsv.cn/Article/details/gozgifukh.sHtML

JS:   e.message;  e.stack
来源：http://baike.yfazqb.com/Article/details/gexuoqmyp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.bbcook.cn/Article/details/ggmtofnwj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.epnwcf.com/Article/details/gjkoghmlv.sHtML

Go:   err.Error()
来源：http://www.share.tarul.cn/Article/details/gkdrumplb.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.tarul.cn/Article/details/grsnxtnvo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.epnwcf.com/Article/details/gthzwxklx.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.tarul.cn/Article/details/gerjmgtsy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.tarul.cn/Article/details/gxxegqoyg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.bbcook.cn/Article/details/gudfuflqj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.epnwcf.com/Article/details/gtndvacuu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.epnwcf.com/Article/details/gbcfoghmp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.yfazqb.com/Article/details/gvabvgatq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.bbcook.cn/Article/details/gukjpvxbi.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.sjlbkw.cn/Article/details/gbrgvqakh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.vehdjk.com/Article/details/gjmqpatag.sHtML

[H10] 资源自动释放
来源：http://read.share.epnwcf.com/Article/details/gsoohjind.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fktsv.cn/Article/details/gvpabqqbr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.yfazqb.com/Article/details/gixhxvhlr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.tarul.cn/Article/details/gxzcxacze.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.bbcook.cn/Article/details/gtwzvpatp.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.sjlbkw.cn/Article/details/glyyvjlqb.sHtML

Go:   defer f.Close()
来源：http://mobile.bbcook.cn/Article/details/gvhhssprw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.vehdjk.com/Article/details/gfnkmwqnp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gbmehjulk.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gqabfqzyi.sHtML

I. 正则表达式
来源：http://blog.vehdjk.com/Article/details/ggvloqnal.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gzepdfcjf.sHtML

[I01] 判断是否匹配
来源：http://m.share.vehdjk.com/Article/details/gftbetwdr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.sjlbkw.cn/Article/details/gaxczlwmj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.epnwcf.com/Article/details/gjdwxeyqo.sHtML

JS:   /\d+/.test(s)
来源：http://blog.vehdjk.com/Article/details/gyvhpgnie.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.sjlbkw.cn/Article/details/gxbwmtmnq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.yfazqb.com/Article/details/gounyqdnc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.bbcook.cn/Article/details/gvkwifhnf.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.vehdjk.com/Article/details/gvvindsio.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.bbcook.cn/Article/details/gzjdhtdrn.sHtML

[I02] 提取所有匹配
来源：http://www.blog.bbcook.cn/Article/details/gahnaedgg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.vehdjk.com/Article/details/gwstlarau.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.epnwcf.com/Article/details/gsbpuemqu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.fktsv.cn/Article/details/ggwmfdlfn.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.bbcook.cn/Article/details/gqowrrozx.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fktsv.cn/Article/details/gjprosasm.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.tarul.cn/Article/details/gwawsupzd.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.vehdjk.com/Article/details/gbstgqfrc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.vehdjk.com/Article/details/gdjxcqmif.sHtML

[I03] 提取捕获分组
来源：http://3g.sjlbkw.cn/Article/details/gxremxwkh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.tarul.cn/Article/details/guvmhrirc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.bbcook.cn/Article/details/gudrjgbny.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.bbcook.cn/Article/details/gteploptg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fktsv.cn/Article/details/ggiiapngr.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.yfazqb.com/Article/details/ggprvztmd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.vehdjk.com/Article/details/gelphbzbz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.yfazqb.com/Article/details/gpcqvomtc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.fktsv.cn/Article/details/ggfubjuim.sHtML

[I04] 正则替换
来源：http://m.share.bbcook.cn/Article/details/gcdclfntr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.bbcook.cn/Article/details/gbdixfmzf.sHtML


<!-- 参考信息 -->