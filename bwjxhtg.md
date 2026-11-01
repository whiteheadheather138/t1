代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.epnwcf.com/Article/details/ggkdmoxna.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fktsv.cn/Article/details/gyfgnjzhv.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.tarul.cn/Article/details/guhilswud.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.epnwcf.com/Article/details/gphsctkzi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.vehdjk.com/Article/details/gtfzsssrs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.yfazqb.com/Article/details/gzwsqgfxj.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.sjlbkw.cn/Article/details/gehyiicnv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.yfazqb.com/Article/details/gynbvxyza.sHtML

[F09] 获取文件大小
来源：http://wap.epnwcf.com/Article/details/gxzhjledr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.epnwcf.com/Article/details/gcozzaubp.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gdrwkoreo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.bbcook.cn/Article/details/gnebhpgux.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.tarul.cn/Article/details/gdavuasjm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/gayslroqq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.vehdjk.com/Article/details/gybpflvwt.sHtML

Ruby: File.size("a.txt")
来源：http://3g.bbcook.cn/Article/details/gahpoytqx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.vehdjk.com/Article/details/gtgvxstta.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.epnwcf.com/Article/details/gcfzimpkh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gwagdqmox.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.bbcook.cn/Article/details/gbjzzedzw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/gcxykmplp.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gzzlbrexw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.sjlbkw.cn/Article/details/gvvjuuxek.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gbixxbnmo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/geddkbomz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gnnkaujjp.sHtML

[F11] 复制与移动文件
来源：http://blog.epnwcf.com/Article/details/glaemocub.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.epnwcf.com/Article/details/gqrxpvjid.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gjdjjlklb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gkvaylybb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/glwajdlnl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fktsv.cn/Article/details/gxcgwgduv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.vehdjk.com/Article/details/gwkimfxpc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gihwmxqma.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.vehdjk.com/Article/details/gxgnyqesz.sHtML

[F12] CSV 读写
来源：http://www.blog.sjlbkw.cn/Article/details/grsqlyrmj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.vehdjk.com/Article/details/gystwvmpz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.bbcook.cn/Article/details/gywmonvzc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.bbcook.cn/Article/details/gkbcuzhfa.sHtML

TS:   // 同上
来源：http://www.share.fktsv.cn/Article/details/giltaemyt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.yfazqb.com/Article/details/gtrfmvlhz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fktsv.cn/Article/details/gwzbeozkz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fktsv.cn/Article/details/gyfjkkrhb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.sjlbkw.cn/Article/details/ggjymezrn.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gplzdqxyb.sHtML

G. 面向对象
来源：http://read.share.sjlbkw.cn/Article/details/gfrzhkziq.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gdmkyeren.sHtML

[G01] 定义类
来源：http://wap.yfazqb.com/Article/details/gusrutpos.sHtML

Py:   class User: pass
来源：http://www.share.bbcook.cn/Article/details/gshywjyjx.sHtML

PHP:  class User {}
来源：http://3g.fktsv.cn/Article/details/gobqszpvp.sHtML

JS:   class User {}
来源：http://mobile.fktsv.cn/Article/details/gnsjqixwf.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.tarul.cn/Article/details/gnibucsav.sHtML

Java: class User {}
来源：http://baike.vehdjk.com/Article/details/gwfzvlvzl.sHtML

Go:   type User struct { Name string }
来源：http://m.share.vehdjk.com/Article/details/gkvcofdfy.sHtML

Ruby: class User; end
来源：http://m.share.fktsv.cn/Article/details/gaadupvqo.sHtML

C#:   class User {}
来源：http://baike.tarul.cn/Article/details/gouqdkhqa.sHtML

[G02] 构造函数
来源：http://mobile.tarul.cn/Article/details/ggzkiykbu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.yfazqb.com/Article/details/gnmyeeghh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.vehdjk.com/Article/details/gexbwllzo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.yfazqb.com/Article/details/gqkogmkpa.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.bbcook.cn/Article/details/gxejrykct.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/gafmnjtmq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.yfazqb.com/Article/details/grzexraou.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.epnwcf.com/Article/details/gwuubrjzt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.epnwcf.com/Article/details/gnsvhuexn.sHtML

[G03] 实例属性
来源：http://wap.epnwcf.com/Article/details/gtoqrpyab.sHtML

Py:   self.name = "x"
来源：http://read.share.tarul.cn/Article/details/golphdxvs.sHtML

PHP:  public string $name = "x";
来源：http://mobile.tarul.cn/Article/details/gjtyluzzs.sHtML

JS:   this.name = "x";
来源：http://baike.sjlbkw.cn/Article/details/ggmqftolu.sHtML

TS:   name: string = "x";
来源：http://wap.bbcook.cn/Article/details/gbvdaalsi.sHtML

Java: private String name;
来源：http://blog.epnwcf.com/Article/details/gpjwrwkhe.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.yfazqb.com/Article/details/gsdnenmyr.sHtML

Ruby: @name = "x"
来源：http://blog.yfazqb.com/Article/details/gchwlamxf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fktsv.cn/Article/details/gihapueti.sHtML

[G04] 定义方法
来源：http://wap.epnwcf.com/Article/details/guwctvxgk.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.tarul.cn/Article/details/gcajeuefg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/gjuqfewvo.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fktsv.cn/Article/details/gmjpwjthj.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/gfqvkurgt.sHtML

Java: String greet() { return name; }
来源：http://wap.yfazqb.com/Article/details/gecbgfaff.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.epnwcf.com/Article/details/gnjonxnxq.sHtML

Ruby: def greet; @name; end
来源：http://wap.sjlbkw.cn/Article/details/glzwkdany.sHtML

C#:   public string Greet() => Name;
来源：http://3g.sjlbkw.cn/Article/details/gosthttmz.sHtML

[G05] 继承
来源：http://3g.epnwcf.com/Article/details/gcauqemfw.sHtML

Py:   class Admin(User): pass
来源：http://mobile.tarul.cn/Article/details/gxuuyrtfj.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gwddhzfev.sHtML

JS:   class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/gywykbejc.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gbgpiydvi.sHtML

Java: class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/ghzjguacq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.epnwcf.com/Article/details/gelvzaxvs.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fktsv.cn/Article/details/gjcbqdjem.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.bbcook.cn/Article/details/ghhmfsxye.sHtML

[G06] 重写方法
来源：http://baike.bbcook.cn/Article/details/goroseoxm.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.tarul.cn/Article/details/gdmgesujq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gnullfanr.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.yfazqb.com/Article/details/gbdojchrn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/gjqhchzoo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/gjvztynak.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.epnwcf.com/Article/details/goeuvbcui.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.bbcook.cn/Article/details/gsmjvxygi.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.tarul.cn/Article/details/gjleywlst.sHtML

[G07] 调用父类方法
来源：http://blog.fktsv.cn/Article/details/gumbwuakt.sHtML

Py:   super().greet()
来源：http://wap.sjlbkw.cn/Article/details/gwqaosjob.sHtML

PHP:  parent::greet();
来源：http://wap.tarul.cn/Article/details/gepibbeuj.sHtML

JS:   super.greet();
来源：http://mobile.bbcook.cn/Article/details/gdcgdmokd.sHtML

TS:   super.greet();
来源：http://www.m.share.yfazqb.com/Article/details/ganuyunoh.sHtML

Java: super.greet();
来源：http://www.blog.sjlbkw.cn/Article/details/gwnwbmpix.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.epnwcf.com/Article/details/grpwfpryt.sHtML

Ruby: super
来源：http://www.share.fktsv.cn/Article/details/ggoeuwmxn.sHtML

C#:   base.Greet();
来源：http://www.blog.yfazqb.com/Article/details/gkswhydkr.sHtML

[G08] 静态方法与属性
来源：http://baike.tarul.cn/Article/details/gtncbwjwg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.bbcook.cn/Article/details/gbomsoisc.sHtML

PHP:  public static function f() {}
来源：http://www.share.epnwcf.com/Article/details/gggpgcixs.sHtML

JS:   static f() {}
来源：http://blog.vehdjk.com/Article/details/gocnkkyuk.sHtML

TS:   static f(): void {}
来源：http://m.share.vehdjk.com/Article/details/gbxdnioyg.sHtML

Java: static void f() {}
来源：http://www.m.share.vehdjk.com/Article/details/ggqrgkepx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.bbcook.cn/Article/details/gdvnfunto.sHtML

Ruby: def self.f; end
来源：http://www.blog.bbcook.cn/Article/details/gavretrcm.sHtML

C#:   public static void F() {}
来源：http://mobile.bbcook.cn/Article/details/gookjxreb.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.tarul.cn/Article/details/gzsipumwt.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.sjlbkw.cn/Article/details/gnbgoyaec.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.yfazqb.com/Article/details/gpgohxjir.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.sjlbkw.cn/Article/details/gkcmeeajb.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.bbcook.cn/Article/details/grmmfgcrj.sHtML

Java: interface Shape { double area(); }
来源：http://wap.bbcook.cn/Article/details/gwyuuujnh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.tarul.cn/Article/details/gevzzhxcj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.tarul.cn/Article/details/gnvjszfhn.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.vehdjk.com/Article/details/glmzqnigp.sHtML

[G10] 访问控制
来源：http://www.blog.yfazqb.com/Article/details/gwpdsqjho.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.epnwcf.com/Article/details/gikxgdofd.sHtML

PHP:  public / protected / private
来源：http://3g.yfazqb.com/Article/details/gvdjvuxyb.sHtML

JS:   #private 字段；其余公开
来源：http://3g.bbcook.cn/Article/details/gswwnxzbo.sHtML

TS:   public / protected / private
来源：http://www.share.fktsv.cn/Article/details/gbtauvclf.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.vehdjk.com/Article/details/grmkcqonm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.vehdjk.com/Article/details/gqobusebc.sHtML

Ruby: public / protected / private
来源：http://read.share.fktsv.cn/Article/details/gtxaffhsb.sHtML

C#:   public / protected / private / internal
来源：http://blog.bbcook.cn/Article/details/gvvlmyvhl.sHtML

[G11] getter / setter
来源：http://www.blog.sjlbkw.cn/Article/details/gbtdexkbj.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.epnwcf.com/Article/details/getjxvnqi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.yfazqb.com/Article/details/grsgesdzj.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.epnwcf.com/Article/details/gqrpdffkm.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.vehdjk.com/Article/details/gknwhezxm.sHtML

Java: public String getName() { return name; }
来源：http://m.share.bbcook.cn/Article/details/gdimreevz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/gyvdfuasd.sHtML

Ruby: attr_accessor :name
来源：http://blog.epnwcf.com/Article/details/gljratbal.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.epnwcf.com/Article/details/gwciqbcyb.sHtML

[G12] 对象转字符串
来源：http://wap.tarul.cn/Article/details/gpijfujfd.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.bbcook.cn/Article/details/gwpoebrbl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/goirdxspt.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gpolaoore.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/gamgalcbr.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.yfazqb.com/Article/details/gftbhyyos.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.vehdjk.com/Article/details/gukojhgci.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.epnwcf.com/Article/details/gejqshkmb.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.tarul.cn/Article/details/gjpxmyxoa.sHtML

[G13] 判断对象类型
来源：http://baike.tarul.cn/Article/details/gsjlxtpkt.sHtML

Py:   isinstance(u, User)
来源：http://m.share.epnwcf.com/Article/details/gugzmyiim.sHtML

PHP:  $u instanceof User
来源：http://www.share.tarul.cn/Article/details/geanccxcs.sHtML

JS:   u instanceof User
来源：http://blog.bbcook.cn/Article/details/gamlstcdh.sHtML

TS:   u instanceof User
来源：http://m.share.sjlbkw.cn/Article/details/gvszvjdvf.sHtML

Java: u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gvmkuauwx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.sjlbkw.cn/Article/details/gymmnsjqy.sHtML

Ruby: u.is_a?(User)
来源：http://baike.epnwcf.com/Article/details/gvvikdhts.sHtML

C#:   u is User
来源：http://mobile.bbcook.cn/Article/details/gkrpkocnb.sHtML

[G14] 数据类 / record
来源：http://www.blog.tarul.cn/Article/details/gwrknjmgp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.bbcook.cn/Article/details/ghluodabk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.vehdjk.com/Article/details/gwgykkjgk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.sjlbkw.cn/Article/details/gbrcofaxo.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.yfazqb.com/Article/details/gwuepyyeg.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fktsv.cn/Article/details/gcydzsznc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.vehdjk.com/Article/details/gbtuqstgz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fktsv.cn/Article/details/gelfpelgu.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.sjlbkw.cn/Article/details/ghnywztbm.sHtML

[G15] 枚举
来源：http://wap.bbcook.cn/Article/details/gqqfnxcpz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.vehdjk.com/Article/details/gdqansmmn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.bbcook.cn/Article/details/gggkdicpg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.bbcook.cn/Article/details/gyhaezykz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.bbcook.cn/Article/details/gsswsaomw.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fktsv.cn/Article/details/gaftswbyg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.epnwcf.com/Article/details/ggebtgjnu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.tarul.cn/Article/details/ggegmujtq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.vehdjk.com/Article/details/gxejktxfl.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fktsv.cn/Article/details/gxyxiemom.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.vehdjk.com/Article/details/gwlaqfzwn.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.bbcook.cn/Article/details/gptoneqyn.sHtML

JS:   Object.entries(obj)
来源：http://baike.bbcook.cn/Article/details/gsbctrmzl.sHtML

TS:   Object.entries(obj)
来源：http://mobile.epnwcf.com/Article/details/gpjrysdpm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.epnwcf.com/Article/details/gmqqyewuj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.yfazqb.com/Article/details/giwmdhkvl.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fktsv.cn/Article/details/gzlxnbtvj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.sjlbkw.cn/Article/details/gznyhqvug.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/giwinipes.sHtML

H. 异常与错误处理
来源：http://www.share.sjlbkw.cn/Article/details/gagpsowtd.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gvmctjvcr.sHtML

[H01] try / catch 基础
来源：http://www.m.share.yfazqb.com/Article/details/gjzifhjam.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.epnwcf.com/Article/details/gfkssqjqx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.epnwcf.com/Article/details/gilgozeig.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.bbcook.cn/Article/details/gipeyfoxj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.bbcook.cn/Article/details/grakbuooj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.vehdjk.com/Article/details/gbzbfolpt.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.bbcook.cn/Article/details/goxwadvwx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.vehdjk.com/Article/details/gfrqrasuk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.tarul.cn/Article/details/gpbgtobpz.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.epnwcf.com/Article/details/gwctdlzyn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.vehdjk.com/Article/details/gibxgwrbj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gjgfgmabi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/grljccjhh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/gotnukcbo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gocxdfowb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.yfazqb.com/Article/details/gxsmgtiem.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fktsv.cn/Article/details/gunwvmclz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gqvsznvut.sHtML

[H03] 主动抛出异常
来源：http://www.blog.epnwcf.com/Article/details/giogensbl.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.sjlbkw.cn/Article/details/gdtximcex.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gfolrplal.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.tarul.cn/Article/details/ggdllsqqq.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.yfazqb.com/Article/details/gwoddxpge.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.epnwcf.com/Article/details/gloejjzcg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.bbcook.cn/Article/details/goqqdosim.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.vehdjk.com/Article/details/gyndrazzp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.bbcook.cn/Article/details/gdqrmtvhl.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.yfazqb.com/Article/details/gtwddssze.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fktsv.cn/Article/details/gvsmphpul.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.bbcook.cn/Article/details/grrerxpji.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.vehdjk.com/Article/details/guhgdvaln.sHtML

TS:   class MyError extends Error {}
来源：http://3g.bbcook.cn/Article/details/gqusjogcs.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjcgbgsx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fktsv.cn/Article/details/gzvbwcpne.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fktsv.cn/Article/details/gzhcwcnlz.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fktsv.cn/Article/details/gwqxwkqlo.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.tarul.cn/Article/details/gyoemlnew.sHtML

Py:   except ValueError as e:
来源：http://3g.bbcook.cn/Article/details/gviogkfdh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.bbcook.cn/Article/details/gogblajkc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fktsv.cn/Article/details/gzikhnluz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.yfazqb.com/Article/details/gquapouai.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gzitfbugk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.tarul.cn/Article/details/gswgxhkvm.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.bbcook.cn/Article/details/gozyycyai.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.epnwcf.com/Article/details/gjvsbakow.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.bbcook.cn/Article/details/gupcxwjvb.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.epnwcf.com/Article/details/gwnoejxjz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.tarul.cn/Article/details/gvtpgsuah.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.epnwcf.com/Article/details/gzrajpcme.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fktsv.cn/Article/details/gwquusgfn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fktsv.cn/Article/details/gsxyoujdi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.epnwcf.com/Article/details/gbjlmadlr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fktsv.cn/Article/details/gbgpjsosz.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.yfazqb.com/Article/details/gjbzegjdr.sHtML

[H07] 断言
来源：http://www.blog.vehdjk.com/Article/details/gneywzczc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.bbcook.cn/Article/details/gdbdlkuyh.sHtML

PHP:  assert($x > 0);
来源：http://m.share.epnwcf.com/Article/details/ghralftsi.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fktsv.cn/Article/details/gizyqgfni.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.yfazqb.com/Article/details/gbtngrzuw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.bbcook.cn/Article/details/gwxpzudpq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fktsv.cn/Article/details/gxrptwrjn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgywdsbl.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.yfazqb.com/Article/details/gpdepxnio.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.tarul.cn/Article/details/gngakmwlo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.tarul.cn/Article/details/gmvhznxyn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.bbcook.cn/Article/details/gibfjuxkh.sHtML

JS:   e.message;  e.stack
来源：http://read.share.epnwcf.com/Article/details/gqqyjzfum.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.yfazqb.com/Article/details/gjvddbbwq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.tarul.cn/Article/details/gofuxdfnd.sHtML

Go:   err.Error()
来源：http://blog.vehdjk.com/Article/details/gcdoavmit.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.epnwcf.com/Article/details/gpsudijyr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.tarul.cn/Article/details/gnvthuanb.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.tarul.cn/Article/details/gkyayjeli.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.tarul.cn/Article/details/gkzjuguow.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.epnwcf.com/Article/details/gsentdxno.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fktsv.cn/Article/details/ggznpamfo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.epnwcf.com/Article/details/gpubkhhsk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.sjlbkw.cn/Article/details/ghyxnuxgv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.vehdjk.com/Article/details/ggmfcnkly.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.bbcook.cn/Article/details/gbgxvnywe.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.vehdjk.com/Article/details/grhuvmdot.sHtML

[H10] 资源自动释放
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmkwamds.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.epnwcf.com/Article/details/ghuowgdod.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.yfazqb.com/Article/details/grxiwpeil.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.tarul.cn/Article/details/gdjgmvnjw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.bbcook.cn/Article/details/gcacemgtw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.yfazqb.com/Article/details/gkikfixxv.sHtML

Go:   defer f.Close()
来源：http://mobile.epnwcf.com/Article/details/gnilrzjyk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.yfazqb.com/Article/details/gfoekghdt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.yfazqb.com/Article/details/gxqvpuugz.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gjpsedljs.sHtML

I. 正则表达式
来源：http://mobile.tarul.cn/Article/details/ggvqsgfam.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gcbfntshx.sHtML

[I01] 判断是否匹配
来源：http://blog.tarul.cn/Article/details/gxlwlpuzf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.vehdjk.com/Article/details/ghcxrqesa.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fktsv.cn/Article/details/gatfmzcoy.sHtML

JS:   /\d+/.test(s)
来源：http://baike.tarul.cn/Article/details/gdqhzxrcx.sHtML

TS:   /\d+/.test(s)
来源：http://wap.tarul.cn/Article/details/gbgucjxmp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.sjlbkw.cn/Article/details/gttmddwde.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.sjlbkw.cn/Article/details/gujswsnqs.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.vehdjk.com/Article/details/gilldqbsm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fktsv.cn/Article/details/gzvazlaib.sHtML

[I02] 提取所有匹配
来源：http://mobile.tarul.cn/Article/details/guxpkjcmw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.yfazqb.com/Article/details/gsremwpof.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.sjlbkw.cn/Article/details/gteacqmty.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.vehdjk.com/Article/details/gedqwhqwu.sHtML


<!-- 参考信息 -->