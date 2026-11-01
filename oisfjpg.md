代发 wailian999

[F09] 获取文件大小
来源：http://www.share.fktsv.cn/Article/details/ganknsgdq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gffiftaex.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.tarul.cn/Article/details/gtvfuzfgf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.bbcook.cn/Article/details/gdoialsrp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.epnwcf.com/Article/details/gdxnkznca.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.tarul.cn/Article/details/gkinutrcf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.bbcook.cn/Article/details/gmupefckj.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gofuzqttn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.vehdjk.com/Article/details/gllvlizsh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.yfazqb.com/Article/details/glstnbtbc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gxgsfydkr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fktsv.cn/Article/details/gnfflodsn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gldqvpejm.sHtML

TS:   path.extname("a.txt")
来源：http://wap.yfazqb.com/Article/details/gvedyubly.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.yfazqb.com/Article/details/gytfmbqre.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gqloecfbq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gbzywsieq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gegmnnmeo.sHtML

[F11] 复制与移动文件
来源：http://3g.sjlbkw.cn/Article/details/gqpkmufym.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/ghepeogrx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.vehdjk.com/Article/details/gmauqvmwq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gwzrzpblu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gzxpeinnk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.tarul.cn/Article/details/gfdqkbxiy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.bbcook.cn/Article/details/gttjnjyut.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/giixuecjs.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.bbcook.cn/Article/details/gzcwzotxg.sHtML

[F12] CSV 读写
来源：http://mobile.sjlbkw.cn/Article/details/gvmedjxst.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.tarul.cn/Article/details/gkqpcgyoc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.tarul.cn/Article/details/graxiaiph.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fktsv.cn/Article/details/guthauoih.sHtML

TS:   // 同上
来源：http://www.m.share.fktsv.cn/Article/details/guqwldvdk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fktsv.cn/Article/details/grloporlm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fktsv.cn/Article/details/gflhtoipn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fktsv.cn/Article/details/gmcweosfx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fktsv.cn/Article/details/gxtholsiv.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gykltwgzn.sHtML

G. 面向对象
来源：http://www.m.share.bbcook.cn/Article/details/gbaplwibe.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gagteiwzh.sHtML

[G01] 定义类
来源：http://m.share.yfazqb.com/Article/details/gjuwenlld.sHtML

Py:   class User: pass
来源：http://baike.epnwcf.com/Article/details/gygpmlomo.sHtML

PHP:  class User {}
来源：http://baike.tarul.cn/Article/details/gvqycmyaw.sHtML

JS:   class User {}
来源：http://www.share.epnwcf.com/Article/details/gsegnfadi.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.sjlbkw.cn/Article/details/ghaveovfw.sHtML

Java: class User {}
来源：http://www.blog.fktsv.cn/Article/details/gtdcqppcq.sHtML

Go:   type User struct { Name string }
来源：http://blog.epnwcf.com/Article/details/grslsvxry.sHtML

Ruby: class User; end
来源：http://www.blog.bbcook.cn/Article/details/grrpngoie.sHtML

C#:   class User {}
来源：http://m.share.yfazqb.com/Article/details/gwkdvczuo.sHtML

[G02] 构造函数
来源：http://read.share.epnwcf.com/Article/details/gjlhcxzhq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.sjlbkw.cn/Article/details/gpjztxobn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.epnwcf.com/Article/details/gxpmonbkx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.bbcook.cn/Article/details/gmuapfzdz.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.bbcook.cn/Article/details/gfkjhqowk.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.epnwcf.com/Article/details/gnnvpftah.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.sjlbkw.cn/Article/details/guxilezwg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.epnwcf.com/Article/details/gaisxekgt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.yfazqb.com/Article/details/gtszwjqcj.sHtML

[G03] 实例属性
来源：http://www.m.share.tarul.cn/Article/details/gkbupahvt.sHtML

Py:   self.name = "x"
来源：http://wap.vehdjk.com/Article/details/gvnzbohpy.sHtML

PHP:  public string $name = "x";
来源：http://m.share.epnwcf.com/Article/details/gviqewlpr.sHtML

JS:   this.name = "x";
来源：http://3g.sjlbkw.cn/Article/details/gkpzyojti.sHtML

TS:   name: string = "x";
来源：http://blog.tarul.cn/Article/details/gkuhvrfma.sHtML

Java: private String name;
来源：http://m.share.yfazqb.com/Article/details/gkaapbzub.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.vehdjk.com/Article/details/gnexutlts.sHtML

Ruby: @name = "x"
来源：http://read.share.sjlbkw.cn/Article/details/gnppwjcex.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.vehdjk.com/Article/details/gdiwcymbj.sHtML

[G04] 定义方法
来源：http://wap.yfazqb.com/Article/details/giwrgllwa.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.bbcook.cn/Article/details/gkammxlwr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gsjdocftm.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gfmzljgwf.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.tarul.cn/Article/details/gcvfxtqzj.sHtML

Java: String greet() { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gwamtymnq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.bbcook.cn/Article/details/gbmczbkkn.sHtML

Ruby: def greet; @name; end
来源：http://wap.vehdjk.com/Article/details/gamillrko.sHtML

C#:   public string Greet() => Name;
来源：http://3g.vehdjk.com/Article/details/gruhewyvw.sHtML

[G05] 继承
来源：http://blog.fktsv.cn/Article/details/ghtkxvdrt.sHtML

Py:   class Admin(User): pass
来源：http://blog.yfazqb.com/Article/details/giakpawen.sHtML

PHP:  class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/glprwybfp.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/gsmljxxwu.sHtML

TS:   class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/ghkatldrg.sHtML

Java: class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gwsmztfon.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.vehdjk.com/Article/details/gsnaohzjb.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fktsv.cn/Article/details/gdixjsbsm.sHtML

C#:   class Admin : User {}
来源：http://baike.vehdjk.com/Article/details/gkvxszuix.sHtML

[G06] 重写方法
来源：http://blog.fktsv.cn/Article/details/gmpaolsuw.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.sjlbkw.cn/Article/details/glaspbpwh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gbagzucvr.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.tarul.cn/Article/details/ghvoaktza.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/gyaqjjkyp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/gjlgfmpok.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.tarul.cn/Article/details/gjfbrpefr.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.yfazqb.com/Article/details/gzmpddeyq.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.epnwcf.com/Article/details/gqufhmeoh.sHtML

[G07] 调用父类方法
来源：http://read.share.bbcook.cn/Article/details/giejvteat.sHtML

Py:   super().greet()
来源：http://wap.vehdjk.com/Article/details/gynfawjxq.sHtML

PHP:  parent::greet();
来源：http://baike.sjlbkw.cn/Article/details/guufrliog.sHtML

JS:   super.greet();
来源：http://mobile.epnwcf.com/Article/details/ghimrewto.sHtML

TS:   super.greet();
来源：http://www.share.vehdjk.com/Article/details/grsvfvonw.sHtML

Java: super.greet();
来源：http://www.blog.bbcook.cn/Article/details/gxzncgwng.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.vehdjk.com/Article/details/gyfejdhub.sHtML

Ruby: super
来源：http://wap.fktsv.cn/Article/details/gxaoqzigy.sHtML

C#:   base.Greet();
来源：http://wap.sjlbkw.cn/Article/details/gfvaopitm.sHtML

[G08] 静态方法与属性
来源：http://wap.fktsv.cn/Article/details/gbcaidvgv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.sjlbkw.cn/Article/details/geuuwinhx.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.vehdjk.com/Article/details/gxkdzetgr.sHtML

JS:   static f() {}
来源：http://www.blog.fktsv.cn/Article/details/gqdpeievm.sHtML

TS:   static f(): void {}
来源：http://read.share.sjlbkw.cn/Article/details/ghgmqtmku.sHtML

Java: static void f() {}
来源：http://www.blog.bbcook.cn/Article/details/ggtjiayjc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.yfazqb.com/Article/details/gqixdubvt.sHtML

Ruby: def self.f; end
来源：http://wap.yfazqb.com/Article/details/gbdejhtxc.sHtML

C#:   public static void F() {}
来源：http://read.share.fktsv.cn/Article/details/gznfltnzz.sHtML

[G09] 接口 / 抽象类
来源：http://baike.bbcook.cn/Article/details/gekpggmyi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.vehdjk.com/Article/details/gruewyxea.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fktsv.cn/Article/details/gvdmngupy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fktsv.cn/Article/details/gjlwibmqf.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.tarul.cn/Article/details/gdukjurtj.sHtML

Java: interface Shape { double area(); }
来源：http://wap.yfazqb.com/Article/details/geksjiqvc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.bbcook.cn/Article/details/gsxiwieip.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.yfazqb.com/Article/details/gazvqgzxd.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.tarul.cn/Article/details/gexlgkmzd.sHtML

[G10] 访问控制
来源：http://www.blog.vehdjk.com/Article/details/gwwgrbnbk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.yfazqb.com/Article/details/grdxbtter.sHtML

PHP:  public / protected / private
来源：http://3g.bbcook.cn/Article/details/gcdlmyown.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fktsv.cn/Article/details/gqomxvaxx.sHtML

TS:   public / protected / private
来源：http://blog.bbcook.cn/Article/details/glycvbfou.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.vehdjk.com/Article/details/gvzfpxgkf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.yfazqb.com/Article/details/ggqhfvnaf.sHtML

Ruby: public / protected / private
来源：http://www.blog.yfazqb.com/Article/details/gganihnjw.sHtML

C#:   public / protected / private / internal
来源：http://mobile.epnwcf.com/Article/details/gbhdawmkw.sHtML

[G11] getter / setter
来源：http://mobile.epnwcf.com/Article/details/gsrtrtlou.sHtML

Py:   @property 与 @x.setter
来源：http://3g.bbcook.cn/Article/details/ghjudowgv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.bbcook.cn/Article/details/gabbjuoqh.sHtML

JS:   get name() { return this._name; }
来源：http://3g.vehdjk.com/Article/details/gstlkxyfq.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fktsv.cn/Article/details/gkxqpdcwm.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fktsv.cn/Article/details/gsdcuufqg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fktsv.cn/Article/details/gugwrjcdl.sHtML

Ruby: attr_accessor :name
来源：http://m.share.epnwcf.com/Article/details/gslimgdtj.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.bbcook.cn/Article/details/gxilyrxty.sHtML

[G12] 对象转字符串
来源：http://www.share.tarul.cn/Article/details/gdpefsiim.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.sjlbkw.cn/Article/details/gialgumpi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.bbcook.cn/Article/details/gelsozlfc.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gfltzfeuk.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/gtsezwfmn.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gvkvqfcco.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.tarul.cn/Article/details/gtlypecgx.sHtML

Ruby: def to_s; @name; end
来源：http://blog.vehdjk.com/Article/details/gefeqoreu.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.tarul.cn/Article/details/gdwsvzcor.sHtML

[G13] 判断对象类型
来源：http://read.share.tarul.cn/Article/details/glemjmnxw.sHtML

Py:   isinstance(u, User)
来源：http://mobile.epnwcf.com/Article/details/gciuaqgqz.sHtML

PHP:  $u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gobqrmslz.sHtML

JS:   u instanceof User
来源：http://www.blog.tarul.cn/Article/details/gxvsnpkkx.sHtML

TS:   u instanceof User
来源：http://read.share.epnwcf.com/Article/details/gzhaewanw.sHtML

Java: u instanceof User
来源：http://baike.fktsv.cn/Article/details/ghbkcwily.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.sjlbkw.cn/Article/details/gnmuhyvyf.sHtML

Ruby: u.is_a?(User)
来源：http://blog.yfazqb.com/Article/details/gjezshdiy.sHtML

C#:   u is User
来源：http://www.m.share.vehdjk.com/Article/details/gkoqkwpdi.sHtML

[G14] 数据类 / record
来源：http://mobile.yfazqb.com/Article/details/gujkglpmg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.sjlbkw.cn/Article/details/gubyinpqu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.epnwcf.com/Article/details/gktzjfocn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.bbcook.cn/Article/details/glyyxrbpq.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.yfazqb.com/Article/details/gufsfcucj.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.vehdjk.com/Article/details/gmqwsofcv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.sjlbkw.cn/Article/details/gchfztukk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.bbcook.cn/Article/details/gotmrmcwn.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.yfazqb.com/Article/details/ggeawiwmh.sHtML

[G15] 枚举
来源：http://3g.bbcook.cn/Article/details/gppxpedwu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fktsv.cn/Article/details/gdkyedkqi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.bbcook.cn/Article/details/gbrkvgcrg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.sjlbkw.cn/Article/details/gmxurmqbg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.yfazqb.com/Article/details/gxrgkbcxm.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.sjlbkw.cn/Article/details/gdqajefrf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.sjlbkw.cn/Article/details/gibhwgdik.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.tarul.cn/Article/details/gryxepbrh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.tarul.cn/Article/details/gagawfuuf.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.tarul.cn/Article/details/gtyoruzwj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.sjlbkw.cn/Article/details/gzxrfeuyl.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fktsv.cn/Article/details/gzsemgand.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fktsv.cn/Article/details/gjlqapdxl.sHtML

TS:   Object.entries(obj)
来源：http://3g.epnwcf.com/Article/details/ggqunotnx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.bbcook.cn/Article/details/gmfvvdaqu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.sjlbkw.cn/Article/details/gtootbklk.sHtML

Ruby: obj.instance_variables
来源：http://3g.vehdjk.com/Article/details/gkhmmhssa.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.bbcook.cn/Article/details/gaeoerrrm.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gvfsltrpb.sHtML

H. 异常与错误处理
来源：http://www.blog.tarul.cn/Article/details/gvtyxiwdt.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/guyynvtkj.sHtML

[H01] try / catch 基础
来源：http://read.share.epnwcf.com/Article/details/gewwhclpb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.tarul.cn/Article/details/gpgfryhdb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.tarul.cn/Article/details/gerrxsymp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.bbcook.cn/Article/details/gjpbiwspn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.sjlbkw.cn/Article/details/gvkcwjnhj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fktsv.cn/Article/details/gzioqzcxp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.sjlbkw.cn/Article/details/gcaibbhod.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.vehdjk.com/Article/details/gmcmytxyu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggfbrkpgv.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fktsv.cn/Article/details/gmkbpcoig.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fktsv.cn/Article/details/gxtiwfpus.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gbersyxsj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.bbcook.cn/Article/details/glarbfdxo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gnmlpcxen.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.epnwcf.com/Article/details/gqcyshuwj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.fktsv.cn/Article/details/gzashzzib.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.yfazqb.com/Article/details/gajxmoybl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/gavvmhduo.sHtML

[H03] 主动抛出异常
来源：http://www.blog.sjlbkw.cn/Article/details/grmfmjbpe.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.yfazqb.com/Article/details/ggfoolglp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/ghqlkurtf.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.tarul.cn/Article/details/gacujnvsk.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gsvynsqds.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.bbcook.cn/Article/details/gtcthvuea.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.vehdjk.com/Article/details/gxtiamzpp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.vehdjk.com/Article/details/gttyrlaxs.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gftnbzvfa.sHtML

[H04] 自定义异常类型
来源：http://www.share.yfazqb.com/Article/details/gkjphemen.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.vehdjk.com/Article/details/gtdyyktme.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.bbcook.cn/Article/details/gpxiktqto.sHtML

JS:   class MyError extends Error {}
来源：http://wap.sjlbkw.cn/Article/details/gpzjpjfmh.sHtML

TS:   class MyError extends Error {}
来源：http://3g.bbcook.cn/Article/details/galghflim.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.tarul.cn/Article/details/ghafqxngj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.sjlbkw.cn/Article/details/gmnarvrat.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.vehdjk.com/Article/details/gykerumbw.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.bbcook.cn/Article/details/guplctgrx.sHtML

[H05] 捕获特定类型
来源：http://www.blog.yfazqb.com/Article/details/gmqmwyszn.sHtML

Py:   except ValueError as e:
来源：http://mobile.sjlbkw.cn/Article/details/gitpzymvv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.epnwcf.com/Article/details/gprhcujry.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.vehdjk.com/Article/details/gjlanbttl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.bbcook.cn/Article/details/glqijkqlu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.epnwcf.com/Article/details/gjzbrsnui.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fktsv.cn/Article/details/gfecbvefc.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.bbcook.cn/Article/details/gmctjwvuo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.bbcook.cn/Article/details/gbdegvmwn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.sjlbkw.cn/Article/details/gzxpolmpc.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.epnwcf.com/Article/details/gxmeniupo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.vehdjk.com/Article/details/ggscuxzgz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fktsv.cn/Article/details/gajqumsfx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.bbcook.cn/Article/details/gwtohzunq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.yfazqb.com/Article/details/gfsocaanb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fktsv.cn/Article/details/gwoufpifh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fktsv.cn/Article/details/ggwzptkpd.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.yfazqb.com/Article/details/gwzkkwieu.sHtML

[H07] 断言
来源：http://3g.bbcook.cn/Article/details/groeiurvw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.yfazqb.com/Article/details/gcwixhgea.sHtML

PHP:  assert($x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/gwtvmqitw.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.yfazqb.com/Article/details/gyqsfrtbc.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.yfazqb.com/Article/details/gbgbdzshh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.sjlbkw.cn/Article/details/glwudagtx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.tarul.cn/Article/details/gaaunkxvk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.vehdjk.com/Article/details/guybscdrk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.epnwcf.com/Article/details/gvkegoyym.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.epnwcf.com/Article/details/grwmtpztr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.tarul.cn/Article/details/gsxtykzhu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.epnwcf.com/Article/details/gfvekvzvm.sHtML

JS:   e.message;  e.stack
来源：http://wap.epnwcf.com/Article/details/glqowvlnc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.vehdjk.com/Article/details/gqlmwyzoz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fktsv.cn/Article/details/ghlqwikny.sHtML

Go:   err.Error()
来源：http://read.share.vehdjk.com/Article/details/gstqcciaj.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.yfazqb.com/Article/details/gghpvitre.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.epnwcf.com/Article/details/gkttrpnfd.sHtML

[H09] 带错误码的异常
来源：http://3g.tarul.cn/Article/details/glepyzodk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.yfazqb.com/Article/details/gxlaekhuj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.yfazqb.com/Article/details/gcmjmrvvo.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.sjlbkw.cn/Article/details/geveidwpy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.yfazqb.com/Article/details/gfxgetneo.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fktsv.cn/Article/details/gqrqtvhuy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.epnwcf.com/Article/details/gyqcqkxsz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.sjlbkw.cn/Article/details/gugsdjeca.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.tarul.cn/Article/details/gvkjtiikg.sHtML

[H10] 资源自动释放
来源：http://www.share.bbcook.cn/Article/details/gzorrlcbo.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.sjlbkw.cn/Article/details/gburrcoks.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.bbcook.cn/Article/details/gbdpkzalm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.bbcook.cn/Article/details/gfmqfyoze.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fktsv.cn/Article/details/gxufoaftg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.sjlbkw.cn/Article/details/gbgxozlon.sHtML

Go:   defer f.Close()
来源：http://read.share.vehdjk.com/Article/details/goabidclb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.epnwcf.com/Article/details/gvoymxasy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.vehdjk.com/Article/details/gixtdhtab.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gpsnmhtej.sHtML

I. 正则表达式
来源：http://read.share.tarul.cn/Article/details/gmlidxooy.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/ghtvdsxoa.sHtML

[I01] 判断是否匹配
来源：http://baike.sjlbkw.cn/Article/details/gqpcqlbef.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.vehdjk.com/Article/details/gihwmimew.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.vehdjk.com/Article/details/guatxgusw.sHtML

JS:   /\d+/.test(s)
来源：http://3g.vehdjk.com/Article/details/grfsnwufa.sHtML

TS:   /\d+/.test(s)
来源：http://wap.yfazqb.com/Article/details/gzpaamprs.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fktsv.cn/Article/details/gclawkgqk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.tarul.cn/Article/details/gemsoxube.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.epnwcf.com/Article/details/gdcqpaguq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.yfazqb.com/Article/details/gzszobwdn.sHtML

[I02] 提取所有匹配
来源：http://www.blog.vehdjk.com/Article/details/gqycacflf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.vehdjk.com/Article/details/grtuavslw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.sjlbkw.cn/Article/details/gqzchcfjw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.bbcook.cn/Article/details/gacgkxjrx.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.tarul.cn/Article/details/gngigsqus.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.bbcook.cn/Article/details/gvbnhtcqy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzsvglhk.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.tarul.cn/Article/details/giknpjjpb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.vehdjk.com/Article/details/gqefrmbke.sHtML

[I03] 提取捕获分组
来源：http://m.share.fktsv.cn/Article/details/gdhvtiwfy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.vehdjk.com/Article/details/gmcsqnlla.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.bbcook.cn/Article/details/gnqyxggdg.sHtML


<!-- 参考信息 -->