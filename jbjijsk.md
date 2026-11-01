代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gqdcsagie.sHtML

TS:   path.extname("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gufhnqxqe.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.vehdjk.com/Article/details/gmpislvli.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gjpzaqrhf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gkdqfeedv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/gwssmzyvw.sHtML

[F11] 复制与移动文件
来源：http://mobile.bbcook.cn/Article/details/gvazkxsvs.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.epnwcf.com/Article/details/grjnmnrec.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.tarul.cn/Article/details/gwfchxhnq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gxbnaqbvu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/gdshbmvxo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.yfazqb.com/Article/details/gkwkcqimi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.tarul.cn/Article/details/gszpgllxn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.epnwcf.com/Article/details/gkhgtwero.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.vehdjk.com/Article/details/gajlkoajl.sHtML

[F12] CSV 读写
来源：http://wap.sjlbkw.cn/Article/details/gmthzagdy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.tarul.cn/Article/details/gtdhzcnzj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.vehdjk.com/Article/details/gbgmxwdzu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.yfazqb.com/Article/details/getlxkbwd.sHtML

TS:   // 同上
来源：http://read.share.sjlbkw.cn/Article/details/ghqrcourp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fktsv.cn/Article/details/gyuwbnsfg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.bbcook.cn/Article/details/geoncypbe.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fktsv.cn/Article/details/gjpxticdz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.vehdjk.com/Article/details/ghzwumyzb.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gdisjlfvs.sHtML

G. 面向对象
来源：http://www.share.yfazqb.com/Article/details/gkjwlsxpq.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gvezvhmex.sHtML

[G01] 定义类
来源：http://read.share.yfazqb.com/Article/details/gllecqlqi.sHtML

Py:   class User: pass
来源：http://www.m.share.yfazqb.com/Article/details/gewqbxupq.sHtML

PHP:  class User {}
来源：http://www.blog.tarul.cn/Article/details/ggzvjpsat.sHtML

JS:   class User {}
来源：http://blog.sjlbkw.cn/Article/details/gjnfdccev.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fktsv.cn/Article/details/gcpaavbtw.sHtML

Java: class User {}
来源：http://baike.bbcook.cn/Article/details/gqnztrrgc.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.yfazqb.com/Article/details/goxhckkif.sHtML

Ruby: class User; end
来源：http://blog.vehdjk.com/Article/details/gsbmvxesq.sHtML

C#:   class User {}
来源：http://wap.yfazqb.com/Article/details/gergbdpjq.sHtML

[G02] 构造函数
来源：http://m.share.fktsv.cn/Article/details/gjdnjiyzm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.epnwcf.com/Article/details/gyqkgeqaw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.sjlbkw.cn/Article/details/ggfcjndoj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.vehdjk.com/Article/details/gtfmgqoir.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.tarul.cn/Article/details/giaemfczi.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.vehdjk.com/Article/details/gktfthbjj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.vehdjk.com/Article/details/gjaqayanu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.bbcook.cn/Article/details/gdobwkrhr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.sjlbkw.cn/Article/details/gwoadstpl.sHtML

[G03] 实例属性
来源：http://3g.bbcook.cn/Article/details/gfygeqmkk.sHtML

Py:   self.name = "x"
来源：http://blog.yfazqb.com/Article/details/gobimrlrx.sHtML

PHP:  public string $name = "x";
来源：http://read.share.vehdjk.com/Article/details/gvucedmog.sHtML

JS:   this.name = "x";
来源：http://www.m.share.sjlbkw.cn/Article/details/gggfxcvtz.sHtML

TS:   name: string = "x";
来源：http://baike.yfazqb.com/Article/details/grpooeonq.sHtML

Java: private String name;
来源：http://www.share.fktsv.cn/Article/details/geuzfevwj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.tarul.cn/Article/details/grdtlavdp.sHtML

Ruby: @name = "x"
来源：http://www.blog.vehdjk.com/Article/details/glrtjrzji.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.vehdjk.com/Article/details/gjoifyehh.sHtML

[G04] 定义方法
来源：http://www.blog.epnwcf.com/Article/details/gcammvwzn.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.epnwcf.com/Article/details/gqgzpshbu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.bbcook.cn/Article/details/gzzdrbfjq.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fktsv.cn/Article/details/gjpohtizh.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gwgimdrmj.sHtML

Java: String greet() { return name; }
来源：http://www.blog.vehdjk.com/Article/details/grpalblws.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gqhctjfkv.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fktsv.cn/Article/details/gogjpphnu.sHtML

C#:   public string Greet() => Name;
来源：http://blog.vehdjk.com/Article/details/gkyawtktu.sHtML

[G05] 继承
来源：http://m.share.bbcook.cn/Article/details/gfawgakbc.sHtML

Py:   class Admin(User): pass
来源：http://blog.bbcook.cn/Article/details/goekfxidt.sHtML

PHP:  class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/gnzpypnlb.sHtML

JS:   class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gafyhleij.sHtML

TS:   class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/guguwwisz.sHtML

Java: class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gubointem.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.tarul.cn/Article/details/gvbeazhwh.sHtML

Ruby: class Admin < User; end
来源：http://baike.yfazqb.com/Article/details/gxoobkjif.sHtML

C#:   class Admin : User {}
来源：http://wap.epnwcf.com/Article/details/gptvowyjr.sHtML

[G06] 重写方法
来源：http://m.share.yfazqb.com/Article/details/giakybxdi.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.bbcook.cn/Article/details/gynbssrjz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/gaprpsqpu.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.yfazqb.com/Article/details/gsxpsqglo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/gfxtpockp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/ghwpoyxbo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fktsv.cn/Article/details/gjieanuop.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.yfazqb.com/Article/details/gsqcpucir.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.tarul.cn/Article/details/gmpmurxxr.sHtML

[G07] 调用父类方法
来源：http://read.share.epnwcf.com/Article/details/gngdhplyi.sHtML

Py:   super().greet()
来源：http://3g.vehdjk.com/Article/details/grsxshbyk.sHtML

PHP:  parent::greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gkwwyfwla.sHtML

JS:   super.greet();
来源：http://3g.sjlbkw.cn/Article/details/gsuuxbgyh.sHtML

TS:   super.greet();
来源：http://3g.fktsv.cn/Article/details/gxozjevrm.sHtML

Java: super.greet();
来源：http://read.share.fktsv.cn/Article/details/gkyzqdxls.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.tarul.cn/Article/details/gujacbrlo.sHtML

Ruby: super
来源：http://baike.bbcook.cn/Article/details/gskftsrrq.sHtML

C#:   base.Greet();
来源：http://www.share.epnwcf.com/Article/details/gbcfzarwm.sHtML

[G08] 静态方法与属性
来源：http://www.share.fktsv.cn/Article/details/grppwefbh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.vehdjk.com/Article/details/ghjuspfvl.sHtML

PHP:  public static function f() {}
来源：http://blog.tarul.cn/Article/details/gsogcakzb.sHtML

JS:   static f() {}
来源：http://mobile.bbcook.cn/Article/details/gspvisoqt.sHtML

TS:   static f(): void {}
来源：http://blog.yfazqb.com/Article/details/gudmmxajx.sHtML

Java: static void f() {}
来源：http://read.share.epnwcf.com/Article/details/gmxcvakge.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.tarul.cn/Article/details/guiolviia.sHtML

Ruby: def self.f; end
来源：http://3g.fktsv.cn/Article/details/gtgcgnjbp.sHtML

C#:   public static void F() {}
来源：http://baike.epnwcf.com/Article/details/gycixuflk.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.tarul.cn/Article/details/gqgyvuimi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fktsv.cn/Article/details/gatjfhgod.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.yfazqb.com/Article/details/gqdwsxnqo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.tarul.cn/Article/details/gwtrkkbox.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.epnwcf.com/Article/details/gdaukjzid.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.bbcook.cn/Article/details/gegobbjsy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fktsv.cn/Article/details/gybbcilkv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.epnwcf.com/Article/details/giqvvbtik.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.sjlbkw.cn/Article/details/gpheymgae.sHtML

[G10] 访问控制
来源：http://www.blog.bbcook.cn/Article/details/goadteoig.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fktsv.cn/Article/details/grkxwyeqx.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fktsv.cn/Article/details/gwzezppvf.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.epnwcf.com/Article/details/gvjofuvwh.sHtML

TS:   public / protected / private
来源：http://www.share.yfazqb.com/Article/details/gzwxppqrv.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.epnwcf.com/Article/details/gwavopmmy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.vehdjk.com/Article/details/gfgkamybp.sHtML

Ruby: public / protected / private
来源：http://mobile.epnwcf.com/Article/details/girftfkeo.sHtML

C#:   public / protected / private / internal
来源：http://wap.yfazqb.com/Article/details/ggpfgcpkb.sHtML

[G11] getter / setter
来源：http://www.share.sjlbkw.cn/Article/details/gaggjjliy.sHtML

Py:   @property 与 @x.setter
来源：http://3g.sjlbkw.cn/Article/details/gmoqgeosa.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.tarul.cn/Article/details/gwzpufsaj.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.vehdjk.com/Article/details/gozywtqsw.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.yfazqb.com/Article/details/ghyqqxrov.sHtML

Java: public String getName() { return name; }
来源：http://3g.fktsv.cn/Article/details/giitapwfe.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.epnwcf.com/Article/details/gybbbyzef.sHtML

Ruby: attr_accessor :name
来源：http://wap.bbcook.cn/Article/details/gdoqodjnw.sHtML

C#:   public string Name { get; set; }
来源：http://baike.sjlbkw.cn/Article/details/gpupahvvu.sHtML

[G12] 对象转字符串
来源：http://read.share.fktsv.cn/Article/details/grgryqjpq.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.epnwcf.com/Article/details/gyesnolok.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.vehdjk.com/Article/details/gqbdsgsff.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.yfazqb.com/Article/details/ghndvzcuj.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.tarul.cn/Article/details/gzdvdppzh.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.tarul.cn/Article/details/gzhsmwmiw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/gfjrjobup.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.tarul.cn/Article/details/gzjzkpite.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.yfazqb.com/Article/details/geodgalne.sHtML

[G13] 判断对象类型
来源：http://blog.epnwcf.com/Article/details/gjtztkqld.sHtML

Py:   isinstance(u, User)
来源：http://wap.tarul.cn/Article/details/ggxgjeaxi.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/gzaqcvsgt.sHtML

JS:   u instanceof User
来源：http://wap.yfazqb.com/Article/details/gwttzxees.sHtML

TS:   u instanceof User
来源：http://mobile.vehdjk.com/Article/details/gwiybvchj.sHtML

Java: u instanceof User
来源：http://m.share.sjlbkw.cn/Article/details/gmerwkfyu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.tarul.cn/Article/details/gjcmsrkfh.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.epnwcf.com/Article/details/gyrxxtzdb.sHtML

C#:   u is User
来源：http://www.blog.tarul.cn/Article/details/gypbjiwjr.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fktsv.cn/Article/details/gyiqagtbh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.yfazqb.com/Article/details/gdpjzearv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.tarul.cn/Article/details/gnynbpaci.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.epnwcf.com/Article/details/gyfarewlc.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.yfazqb.com/Article/details/gxdxoymia.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.epnwcf.com/Article/details/gwijuorqk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fktsv.cn/Article/details/gouhnpied.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.sjlbkw.cn/Article/details/gebwnyozs.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fktsv.cn/Article/details/gyhzqdudo.sHtML

[G15] 枚举
来源：http://m.share.epnwcf.com/Article/details/gthhcxirm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.vehdjk.com/Article/details/grerquhof.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.yfazqb.com/Article/details/gfdcfwmpr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.tarul.cn/Article/details/gpkzrynfk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.sjlbkw.cn/Article/details/gvevgycru.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.yfazqb.com/Article/details/guwovqkqp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.bbcook.cn/Article/details/gwbhmflby.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.vehdjk.com/Article/details/gekjrjwiu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.vehdjk.com/Article/details/gizjpqtwh.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.sjlbkw.cn/Article/details/gpmqugttr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.tarul.cn/Article/details/gomupateu.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.sjlbkw.cn/Article/details/gudodjfeq.sHtML

JS:   Object.entries(obj)
来源：http://blog.vehdjk.com/Article/details/gssahjvoo.sHtML

TS:   Object.entries(obj)
来源：http://read.share.bbcook.cn/Article/details/gwnwxlkte.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.bbcook.cn/Article/details/gulgnrpqh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.tarul.cn/Article/details/gwdcwaeus.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.bbcook.cn/Article/details/gquegexou.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.epnwcf.com/Article/details/ggdssbkcl.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gapyfvuwa.sHtML

H. 异常与错误处理
来源：http://www.blog.tarul.cn/Article/details/gnatcxlcv.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/ggrsocssf.sHtML

[H01] try / catch 基础
来源：http://www.share.yfazqb.com/Article/details/gsfwrqrno.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.bbcook.cn/Article/details/gwvmhcccw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.sjlbkw.cn/Article/details/gtzgyyynm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.bbcook.cn/Article/details/glchqihiz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fktsv.cn/Article/details/gkaptpvbr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.tarul.cn/Article/details/gjujipjyf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fktsv.cn/Article/details/gpesijewb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fktsv.cn/Article/details/giqudowgc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.sjlbkw.cn/Article/details/gkxwuhwfg.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.epnwcf.com/Article/details/gpotzbjhf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.bbcook.cn/Article/details/gjrcrbwhs.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/gmmsxrnna.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.tarul.cn/Article/details/goddvvlcj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/guoaiqjav.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gkheiafsd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.vehdjk.com/Article/details/gznkkmpaa.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.tarul.cn/Article/details/grfgdedhe.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gwaodmkfm.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.epnwcf.com/Article/details/gckeytbtf.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.bbcook.cn/Article/details/gbvfwrqsx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.bbcook.cn/Article/details/gphexmbln.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.bbcook.cn/Article/details/gphwiyvri.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.vehdjk.com/Article/details/gdfdlvpme.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/ggbljmfhg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.yfazqb.com/Article/details/gxvsrkolg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fktsv.cn/Article/details/gvxgddfvl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.epnwcf.com/Article/details/gzeadyznc.sHtML

[H04] 自定义异常类型
来源：http://baike.sjlbkw.cn/Article/details/gobacznvl.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fktsv.cn/Article/details/gpyfpkaai.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.vehdjk.com/Article/details/gehyngasf.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.tarul.cn/Article/details/gvbtbzmwe.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.bbcook.cn/Article/details/gcthzfqvx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.epnwcf.com/Article/details/gqosjhcga.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.vehdjk.com/Article/details/gdeffzvup.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.sjlbkw.cn/Article/details/gyrjoxeyg.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.tarul.cn/Article/details/gtemvexpi.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gvoyouevu.sHtML

Py:   except ValueError as e:
来源：http://read.share.sjlbkw.cn/Article/details/gsynpchcy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.vehdjk.com/Article/details/gsopfwsrq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.sjlbkw.cn/Article/details/guqumhzmf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.tarul.cn/Article/details/grikzrrni.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.epnwcf.com/Article/details/gfzqoqnmu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.tarul.cn/Article/details/gulexxrth.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fktsv.cn/Article/details/giwizcyry.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fktsv.cn/Article/details/gfybyxkuc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.sjlbkw.cn/Article/details/gbdpkvbne.sHtML

Py:   value = d.get("k") or default
来源：http://baike.yfazqb.com/Article/details/gtphhnitm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.yfazqb.com/Article/details/gomlvlmfr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.tarul.cn/Article/details/gihkcsjko.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.vehdjk.com/Article/details/gfubawxlw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.bbcook.cn/Article/details/gfecadooc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.sjlbkw.cn/Article/details/gqyovqtpf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.tarul.cn/Article/details/gkqukmtuv.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.yfazqb.com/Article/details/gkbkrusqa.sHtML

[H07] 断言
来源：http://m.share.sjlbkw.cn/Article/details/gsbqanjgt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.yfazqb.com/Article/details/giyvwanfq.sHtML

PHP:  assert($x > 0);
来源：http://blog.yfazqb.com/Article/details/ghtuyebax.sHtML

JS:   console.assert(x > 0);
来源：http://blog.yfazqb.com/Article/details/gdhngfstp.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.vehdjk.com/Article/details/grcafqyhe.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.epnwcf.com/Article/details/gbtlxapnp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fktsv.cn/Article/details/ggzrstioi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.yfazqb.com/Article/details/gsvtxromh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.epnwcf.com/Article/details/gjshkywjg.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.epnwcf.com/Article/details/gryylmdpd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.vehdjk.com/Article/details/gdexfsdyn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.epnwcf.com/Article/details/gshhbaknk.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fktsv.cn/Article/details/gteklrauh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.bbcook.cn/Article/details/gfwulpace.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.sjlbkw.cn/Article/details/gxznazlaa.sHtML

Go:   err.Error()
来源：http://www.m.share.sjlbkw.cn/Article/details/goqoregea.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.tarul.cn/Article/details/gsnoptlmy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.sjlbkw.cn/Article/details/gvnqmecbg.sHtML

[H09] 带错误码的异常
来源：http://blog.epnwcf.com/Article/details/gvvscuxwp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.yfazqb.com/Article/details/gsdpfkdih.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.bbcook.cn/Article/details/gdppcpyhx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.bbcook.cn/Article/details/gpthhipvp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.yfazqb.com/Article/details/gqqtpwjvw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.sjlbkw.cn/Article/details/gurzcywhd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.bbcook.cn/Article/details/grygdmscv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.tarul.cn/Article/details/gkwwpkakz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.yfazqb.com/Article/details/gtnbnzloo.sHtML

[H10] 资源自动释放
来源：http://wap.tarul.cn/Article/details/gsxbryumo.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.sjlbkw.cn/Article/details/ghygestpb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.yfazqb.com/Article/details/gdjrhbhnt.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.yfazqb.com/Article/details/gikkviaec.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.yfazqb.com/Article/details/gjwesydcc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.tarul.cn/Article/details/gmthwvmov.sHtML

Go:   defer f.Close()
来源：http://www.share.fktsv.cn/Article/details/gltvrobjo.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.sjlbkw.cn/Article/details/gevnglakg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gjnhorllx.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gejqyckmr.sHtML

I. 正则表达式
来源：http://mobile.fktsv.cn/Article/details/gtetrycla.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gsbksuovr.sHtML

[I01] 判断是否匹配
来源：http://3g.tarul.cn/Article/details/gmndadcuc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.tarul.cn/Article/details/gtzoqhjsp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.yfazqb.com/Article/details/gqblseeus.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.tarul.cn/Article/details/gvmmednut.sHtML

TS:   /\d+/.test(s)
来源：http://baike.yfazqb.com/Article/details/gzkhafpjk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.epnwcf.com/Article/details/gtgjqisdh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.bbcook.cn/Article/details/gqlpxcgag.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.epnwcf.com/Article/details/gruuapwxg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.epnwcf.com/Article/details/gppbolyyr.sHtML

[I02] 提取所有匹配
来源：http://m.share.tarul.cn/Article/details/giduudabp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fktsv.cn/Article/details/giakxhcgo.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.tarul.cn/Article/details/gcdzjnlgz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.vehdjk.com/Article/details/gyoeyslls.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.vehdjk.com/Article/details/gadukfbky.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.yfazqb.com/Article/details/gzebnzkkm.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.fktsv.cn/Article/details/gepnfgdrl.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.tarul.cn/Article/details/gbbizwiyw.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fktsv.cn/Article/details/gwvegbmfz.sHtML

[I03] 提取捕获分组
来源：http://blog.yfazqb.com/Article/details/gsdnjduix.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.tarul.cn/Article/details/ganwvclci.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.epnwcf.com/Article/details/giljdcdrv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.bbcook.cn/Article/details/grsamzjtf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.sjlbkw.cn/Article/details/gltaidbge.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.bbcook.cn/Article/details/gmoppdlfw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.sjlbkw.cn/Article/details/gwgsdixqd.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.tarul.cn/Article/details/geotcerku.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.bbcook.cn/Article/details/gfbddtmis.sHtML

[I04] 正则替换
来源：http://blog.tarul.cn/Article/details/gjbdrhcao.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.vehdjk.com/Article/details/gcokdbhag.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.sjlbkw.cn/Article/details/gzloppudq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.epnwcf.com/Article/details/gdgldorqy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.vehdjk.com/Article/details/gthdbbwlp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.epnwcf.com/Article/details/gsakmfxyu.sHtML


<!-- 参考信息 -->