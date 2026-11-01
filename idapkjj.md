代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.bbcook.cn/Article/details/ghumleofm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.sjlbkw.cn/Article/details/giyjhupif.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.sjlbkw.cn/Article/details/gegvfsjgs.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.vehdjk.com/Article/details/gfknwhlsq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.tarul.cn/Article/details/gfdutgpsr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.bbcook.cn/Article/details/gymrrybwd.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.vehdjk.com/Article/details/gxjmixcqx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.tarul.cn/Article/details/gpthxdjdr.sHtML

[F09] 获取文件大小
来源：http://wap.yfazqb.com/Article/details/gkgkfrphx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gkamuvjab.sHtML

PHP:  filesize("a.txt");
来源：http://3g.tarul.cn/Article/details/gorfnsgas.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fktsv.cn/Article/details/gillmgytk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fktsv.cn/Article/details/gbdhweaez.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/galzkabgq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.bbcook.cn/Article/details/gkvcvgugv.sHtML

Ruby: File.size("a.txt")
来源：http://blog.tarul.cn/Article/details/gptknncic.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fktsv.cn/Article/details/gijweumdt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fktsv.cn/Article/details/gejasybzp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gfgzlcbmb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.epnwcf.com/Article/details/gizqfnryo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gaunafgzr.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gurblzbls.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.bbcook.cn/Article/details/gtwpdowuj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gztgpmqph.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gkrseuozw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/ggrxouged.sHtML

[F11] 复制与移动文件
来源：http://read.share.epnwcf.com/Article/details/gybqtbwzv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/gdbmpqaxr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.bbcook.cn/Article/details/gxmxufhgt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gcubsyuxa.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.epnwcf.com/Article/details/gdmahasox.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.vehdjk.com/Article/details/gqvefycwm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.epnwcf.com/Article/details/gbxzsiibg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gboekqcug.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.tarul.cn/Article/details/gqaxnfztf.sHtML

[F12] CSV 读写
来源：http://wap.yfazqb.com/Article/details/gklwplyye.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.epnwcf.com/Article/details/gxnswvslj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.yfazqb.com/Article/details/gardsolxu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.vehdjk.com/Article/details/gpyrivotp.sHtML

TS:   // 同上
来源：http://blog.epnwcf.com/Article/details/gfphmwksy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.vehdjk.com/Article/details/gqispdrhn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.epnwcf.com/Article/details/gbjdgrmib.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.yfazqb.com/Article/details/gmikumwcp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.vehdjk.com/Article/details/gtkickxdu.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/grdiakpok.sHtML

G. 面向对象
来源：http://3g.fktsv.cn/Article/details/gxwlvzdgu.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/ghqgzeeai.sHtML

[G01] 定义类
来源：http://www.m.share.tarul.cn/Article/details/gazsyhvge.sHtML

Py:   class User: pass
来源：http://baike.yfazqb.com/Article/details/gutjknbeo.sHtML

PHP:  class User {}
来源：http://blog.tarul.cn/Article/details/glpwakztg.sHtML

JS:   class User {}
来源：http://3g.yfazqb.com/Article/details/gkzuemezo.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.epnwcf.com/Article/details/gvfdxrlkg.sHtML

Java: class User {}
来源：http://baike.yfazqb.com/Article/details/gwazqmbpu.sHtML

Go:   type User struct { Name string }
来源：http://www.share.sjlbkw.cn/Article/details/gilndgfeq.sHtML

Ruby: class User; end
来源：http://www.m.share.tarul.cn/Article/details/gjwpcjzhb.sHtML

C#:   class User {}
来源：http://wap.bbcook.cn/Article/details/gvcwdnhwa.sHtML

[G02] 构造函数
来源：http://www.blog.epnwcf.com/Article/details/gjlcbvada.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fktsv.cn/Article/details/gqwalhtkx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.sjlbkw.cn/Article/details/goexzwtbs.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.sjlbkw.cn/Article/details/gsmnejccy.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fktsv.cn/Article/details/grgmmuaca.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.tarul.cn/Article/details/gwpcqchun.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fktsv.cn/Article/details/gnlwkuvcb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.bbcook.cn/Article/details/gepalashc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.bbcook.cn/Article/details/gcseyfgzl.sHtML

[G03] 实例属性
来源：http://www.blog.yfazqb.com/Article/details/gaejphxgh.sHtML

Py:   self.name = "x"
来源：http://read.share.sjlbkw.cn/Article/details/ggpslvifs.sHtML

PHP:  public string $name = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gorrngoel.sHtML

JS:   this.name = "x";
来源：http://www.blog.fktsv.cn/Article/details/ggjrwrgtd.sHtML

TS:   name: string = "x";
来源：http://www.m.share.bbcook.cn/Article/details/gaoqvtxhh.sHtML

Java: private String name;
来源：http://3g.yfazqb.com/Article/details/gqnkdfmhe.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.yfazqb.com/Article/details/gcqjyfmjj.sHtML

Ruby: @name = "x"
来源：http://baike.yfazqb.com/Article/details/gudxioehw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.epnwcf.com/Article/details/gewrvjpkl.sHtML

[G04] 定义方法
来源：http://3g.fktsv.cn/Article/details/gtuovzzzo.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fktsv.cn/Article/details/gofimwlad.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/gokvvjxir.sHtML

JS:   greet() { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/gnpduocke.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/gcweaspih.sHtML

Java: String greet() { return name; }
来源：http://m.share.fktsv.cn/Article/details/gvjnhdoka.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.bbcook.cn/Article/details/gysyyaqhp.sHtML

Ruby: def greet; @name; end
来源：http://wap.tarul.cn/Article/details/gambwfgvg.sHtML

C#:   public string Greet() => Name;
来源：http://wap.bbcook.cn/Article/details/glgoeybwj.sHtML

[G05] 继承
来源：http://read.share.tarul.cn/Article/details/gnwlbubta.sHtML

Py:   class Admin(User): pass
来源：http://blog.sjlbkw.cn/Article/details/gyoakgyff.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gdobbkxlv.sHtML

JS:   class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/gwdyldwcp.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/girxiahfn.sHtML

Java: class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/gdcduuzru.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.bbcook.cn/Article/details/gebawizdf.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.yfazqb.com/Article/details/gobiaxqqf.sHtML

C#:   class Admin : User {}
来源：http://baike.fktsv.cn/Article/details/giatjmnna.sHtML

[G06] 重写方法
来源：http://mobile.vehdjk.com/Article/details/gfwsfornh.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.sjlbkw.cn/Article/details/gdasldegf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/gwmnstejl.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/gltukrthp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.vehdjk.com/Article/details/gmbjeaepk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/gwvosvkqg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.bbcook.cn/Article/details/gzfeboxuf.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gwppiibzb.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.yfazqb.com/Article/details/gtsqlaggz.sHtML

[G07] 调用父类方法
来源：http://www.share.sjlbkw.cn/Article/details/grfrqmmhi.sHtML

Py:   super().greet()
来源：http://www.share.epnwcf.com/Article/details/gnrcgwnmd.sHtML

PHP:  parent::greet();
来源：http://baike.fktsv.cn/Article/details/gsridgiso.sHtML

JS:   super.greet();
来源：http://www.share.epnwcf.com/Article/details/gpavosbof.sHtML

TS:   super.greet();
来源：http://www.share.epnwcf.com/Article/details/gtcykefyn.sHtML

Java: super.greet();
来源：http://www.m.share.vehdjk.com/Article/details/gahzkysht.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.epnwcf.com/Article/details/gbsypidee.sHtML

Ruby: super
来源：http://www.m.share.fktsv.cn/Article/details/gptdpjdom.sHtML

C#:   base.Greet();
来源：http://3g.epnwcf.com/Article/details/gbrkrgmzp.sHtML

[G08] 静态方法与属性
来源：http://m.share.epnwcf.com/Article/details/gtfxpfoaa.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.epnwcf.com/Article/details/guehvexks.sHtML

PHP:  public static function f() {}
来源：http://mobile.vehdjk.com/Article/details/gbydxqxvy.sHtML

JS:   static f() {}
来源：http://www.m.share.sjlbkw.cn/Article/details/giuzzuysl.sHtML

TS:   static f(): void {}
来源：http://m.share.sjlbkw.cn/Article/details/gqrfjhslk.sHtML

Java: static void f() {}
来源：http://wap.epnwcf.com/Article/details/gatmsegld.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.bbcook.cn/Article/details/gnmvqixnp.sHtML

Ruby: def self.f; end
来源：http://mobile.yfazqb.com/Article/details/gcxtyaicb.sHtML

C#:   public static void F() {}
来源：http://blog.sjlbkw.cn/Article/details/giqrwidva.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.epnwcf.com/Article/details/gddvsfxzm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.epnwcf.com/Article/details/gqbuqtiue.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.tarul.cn/Article/details/gbjiabdhh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.sjlbkw.cn/Article/details/gvsjoygce.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.tarul.cn/Article/details/gpyznlxwk.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.bbcook.cn/Article/details/gskersypj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.epnwcf.com/Article/details/gtwnfcgob.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.vehdjk.com/Article/details/goqcaidyo.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fktsv.cn/Article/details/gdtsdlvxx.sHtML

[G10] 访问控制
来源：http://wap.fktsv.cn/Article/details/ggqgkvxhm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.epnwcf.com/Article/details/gymaqtmlr.sHtML

PHP:  public / protected / private
来源：http://www.share.fktsv.cn/Article/details/gwthdibcy.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.yfazqb.com/Article/details/gendldkfv.sHtML

TS:   public / protected / private
来源：http://m.share.vehdjk.com/Article/details/gtmjzqeqe.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.sjlbkw.cn/Article/details/gldslmnou.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.epnwcf.com/Article/details/ghusfbhvj.sHtML

Ruby: public / protected / private
来源：http://mobile.tarul.cn/Article/details/gdxddzyos.sHtML

C#:   public / protected / private / internal
来源：http://blog.bbcook.cn/Article/details/gphugfyyb.sHtML

[G11] getter / setter
来源：http://www.blog.fktsv.cn/Article/details/gyiagaexn.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fktsv.cn/Article/details/gceliaqbc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.bbcook.cn/Article/details/gmqsdfasx.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.tarul.cn/Article/details/gvoreasez.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.epnwcf.com/Article/details/ghadlowgh.sHtML

Java: public String getName() { return name; }
来源：http://baike.tarul.cn/Article/details/gineoqhrj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fktsv.cn/Article/details/gqusxegar.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fktsv.cn/Article/details/grlxczceu.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.epnwcf.com/Article/details/gyeeenarp.sHtML

[G12] 对象转字符串
来源：http://3g.bbcook.cn/Article/details/gpuanftdu.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.sjlbkw.cn/Article/details/gxuvaotvp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fktsv.cn/Article/details/grhkobzdu.sHtML

JS:   toString() { return this.name; }
来源：http://wap.bbcook.cn/Article/details/ginnpfoyo.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.yfazqb.com/Article/details/gfcayjblz.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.tarul.cn/Article/details/gmarlfyvv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.epnwcf.com/Article/details/gercqfmjx.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.epnwcf.com/Article/details/ggwfenzcf.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.tarul.cn/Article/details/gmlluzcee.sHtML

[G13] 判断对象类型
来源：http://read.share.fktsv.cn/Article/details/gnngqqofg.sHtML

Py:   isinstance(u, User)
来源：http://baike.epnwcf.com/Article/details/gugswtyqx.sHtML

PHP:  $u instanceof User
来源：http://3g.fktsv.cn/Article/details/gwxhtezmo.sHtML

JS:   u instanceof User
来源：http://m.share.epnwcf.com/Article/details/gknpldjbw.sHtML

TS:   u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/ggpmtfdpc.sHtML

Java: u instanceof User
来源：http://3g.vehdjk.com/Article/details/gfybiqtqn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbslrlte.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fktsv.cn/Article/details/gudhbfxjs.sHtML

C#:   u is User
来源：http://wap.tarul.cn/Article/details/gqiuweczw.sHtML

[G14] 数据类 / record
来源：http://blog.tarul.cn/Article/details/gcxidohli.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.epnwcf.com/Article/details/gepzumuvi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.sjlbkw.cn/Article/details/gcxzbshef.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.epnwcf.com/Article/details/gchvmtryo.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.epnwcf.com/Article/details/gnyfoueit.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.sjlbkw.cn/Article/details/gakjembao.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.sjlbkw.cn/Article/details/ghiqjglzl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fktsv.cn/Article/details/gfhlaxmub.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.sjlbkw.cn/Article/details/ggowedoyh.sHtML

[G15] 枚举
来源：http://3g.epnwcf.com/Article/details/gkqnvgssn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fktsv.cn/Article/details/gbfonzxih.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.vehdjk.com/Article/details/gjvdeoalm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fktsv.cn/Article/details/gjxtwfffs.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.yfazqb.com/Article/details/grztidtze.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.sjlbkw.cn/Article/details/gfszxaiyw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.sjlbkw.cn/Article/details/geqtsimaz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.vehdjk.com/Article/details/gxvbtwkds.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.tarul.cn/Article/details/ggteccerv.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.tarul.cn/Article/details/gylfkeylb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.vehdjk.com/Article/details/glssgwlnt.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fktsv.cn/Article/details/gzetlhkkg.sHtML

JS:   Object.entries(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gbuotgcfd.sHtML

TS:   Object.entries(obj)
来源：http://www.share.vehdjk.com/Article/details/gsbivjrcx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.epnwcf.com/Article/details/gnparaekh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.sjlbkw.cn/Article/details/gvkqqqwsz.sHtML

Ruby: obj.instance_variables
来源：http://m.share.sjlbkw.cn/Article/details/gdfkasemi.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fktsv.cn/Article/details/gtywrnnks.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/guyswxbsf.sHtML

H. 异常与错误处理
来源：http://www.share.sjlbkw.cn/Article/details/gclvwvijd.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gvphefyjp.sHtML

[H01] try / catch 基础
来源：http://www.share.yfazqb.com/Article/details/gxbxauqeg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.epnwcf.com/Article/details/gnsaymqtx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.vehdjk.com/Article/details/geykldwix.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.vehdjk.com/Article/details/gvbpfdsdw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.sjlbkw.cn/Article/details/gpvnkfvrv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.epnwcf.com/Article/details/gpgkorsqd.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.bbcook.cn/Article/details/ghxgbwskz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.epnwcf.com/Article/details/gllhmsrax.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.tarul.cn/Article/details/gcnwfdlat.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.yfazqb.com/Article/details/gedtflhtp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.epnwcf.com/Article/details/gqmfdgdqt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gelzjcsll.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.tarul.cn/Article/details/gouzkiwud.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gwuxdarga.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.epnwcf.com/Article/details/gdxhjdqei.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fktsv.cn/Article/details/gxohvdqcd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.yfazqb.com/Article/details/guebgeggx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/gclsfjwic.sHtML

[H03] 主动抛出异常
来源：http://mobile.vehdjk.com/Article/details/ggagbgcna.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.yfazqb.com/Article/details/gztyjfffb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gdqyvobip.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.tarul.cn/Article/details/gywxzqpzj.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.tarul.cn/Article/details/gehaxwohw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.bbcook.cn/Article/details/giovmspff.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdleqoigq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.tarul.cn/Article/details/gsyewkqqf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gcqvpxrph.sHtML

[H04] 自定义异常类型
来源：http://blog.tarul.cn/Article/details/gngdlycnv.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.yfazqb.com/Article/details/gydzbvfcm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.tarul.cn/Article/details/gvrtveqpy.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.sjlbkw.cn/Article/details/gyjxmhwpv.sHtML

TS:   class MyError extends Error {}
来源：http://baike.bbcook.cn/Article/details/ggpqitmio.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.epnwcf.com/Article/details/gmexrjqrd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.vehdjk.com/Article/details/glbkqmkfe.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.epnwcf.com/Article/details/gwovohbsi.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.sjlbkw.cn/Article/details/gxenthbbw.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fktsv.cn/Article/details/gscpcomyy.sHtML

Py:   except ValueError as e:
来源：http://read.share.bbcook.cn/Article/details/gsrdrcfjw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.epnwcf.com/Article/details/gwmnieotc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.sjlbkw.cn/Article/details/gfesizuir.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.tarul.cn/Article/details/goawpoqlg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gishjsqvc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.yfazqb.com/Article/details/gbnqxbkxu.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.sjlbkw.cn/Article/details/ghvnbwdbj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.tarul.cn/Article/details/ghubdwmeu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.tarul.cn/Article/details/gwtdxnwny.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.epnwcf.com/Article/details/gcjwmyhad.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.sjlbkw.cn/Article/details/gddxmysqp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.tarul.cn/Article/details/glteqdagq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fktsv.cn/Article/details/gqfumstvt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.vehdjk.com/Article/details/gdpzcohsf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.yfazqb.com/Article/details/goxccujtt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.sjlbkw.cn/Article/details/gmhgieqoy.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fktsv.cn/Article/details/ghkmgjzum.sHtML

[H07] 断言
来源：http://www.m.share.tarul.cn/Article/details/gbhdemops.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.yfazqb.com/Article/details/gvfyshklj.sHtML

PHP:  assert($x > 0);
来源：http://3g.fktsv.cn/Article/details/gztvgfhyp.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.yfazqb.com/Article/details/gasemqgdv.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.tarul.cn/Article/details/gfvhxwgmd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.epnwcf.com/Article/details/geumjkbch.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.vehdjk.com/Article/details/gcywkjxmw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fktsv.cn/Article/details/goqutsbym.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.tarul.cn/Article/details/gxknignan.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.sjlbkw.cn/Article/details/gtwukbpks.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.sjlbkw.cn/Article/details/gfqvwtkck.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.bbcook.cn/Article/details/gphcigzee.sHtML

JS:   e.message;  e.stack
来源：http://mobile.yfazqb.com/Article/details/gtkwwunfd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.tarul.cn/Article/details/gtgvluhaa.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.bbcook.cn/Article/details/gquhrrfdb.sHtML

Go:   err.Error()
来源：http://www.share.sjlbkw.cn/Article/details/grmekccmh.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fktsv.cn/Article/details/glvktahfo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.tarul.cn/Article/details/gvnpkawcc.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fktsv.cn/Article/details/grdgbfpvc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.tarul.cn/Article/details/gunswuusu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fktsv.cn/Article/details/ghgmqxgby.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fktsv.cn/Article/details/gfhzdyifa.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.sjlbkw.cn/Article/details/gyrlknszk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.sjlbkw.cn/Article/details/gntlpwznf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.vehdjk.com/Article/details/graytvggf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.epnwcf.com/Article/details/gaewjvvfc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.tarul.cn/Article/details/ggkemktlm.sHtML

[H10] 资源自动释放
来源：http://blog.vehdjk.com/Article/details/gdcpqzyjt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.bbcook.cn/Article/details/gwrocxihs.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.bbcook.cn/Article/details/gcqtblmzv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.bbcook.cn/Article/details/ghtzpwhui.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.tarul.cn/Article/details/gzlservyf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.bbcook.cn/Article/details/geajqblnd.sHtML

Go:   defer f.Close()
来源：http://www.blog.yfazqb.com/Article/details/gulerwtab.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.epnwcf.com/Article/details/gybztogdj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gufuvpnut.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gbbwfmhww.sHtML

I. 正则表达式
来源：http://read.share.epnwcf.com/Article/details/gdxkcbqun.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/ghqcxuoea.sHtML

[I01] 判断是否匹配
来源：http://mobile.epnwcf.com/Article/details/guyqyanlc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fktsv.cn/Article/details/gsjsqmqbj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.bbcook.cn/Article/details/gyebtpyfv.sHtML

JS:   /\d+/.test(s)
来源：http://3g.yfazqb.com/Article/details/gwhijijds.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.tarul.cn/Article/details/gjugrscql.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.tarul.cn/Article/details/gezxtqodx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.bbcook.cn/Article/details/gvdoxhdcj.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.bbcook.cn/Article/details/giogmibgw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.yfazqb.com/Article/details/guxlvkoyf.sHtML

[I02] 提取所有匹配
来源：http://www.blog.epnwcf.com/Article/details/gaebaiios.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.sjlbkw.cn/Article/details/gfqgzsvxx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.epnwcf.com/Article/details/gadpxbhct.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.yfazqb.com/Article/details/giyuxtjrh.sHtML


<!-- 参考信息 -->