代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://m.share.bbcook.cn/Article/details/ghpvfwmom.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gluudvxgo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.vehdjk.com/Article/details/gvpeattyb.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/glxfxcozh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.yfazqb.com/Article/details/gwqncjywd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.vehdjk.com/Article/details/gkmveojzb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gnmprrtpx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.tarul.cn/Article/details/gsgranpwm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gdbwzddww.sHtML

TS:   path.extname("a.txt")
来源：http://wap.epnwcf.com/Article/details/gevbepafw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.yfazqb.com/Article/details/ghrlfhwxb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gpnjdmkin.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gnrdymqwg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gvevotwnq.sHtML

[F11] 复制与移动文件
来源：http://mobile.vehdjk.com/Article/details/gfvabbreb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/gggbxjlre.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.vehdjk.com/Article/details/gnfvcraqo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/gfsgmfhxh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gurtfsomp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.tarul.cn/Article/details/ggdhkpjzj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.bbcook.cn/Article/details/ghhznuyxm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/giwsqecsz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.yfazqb.com/Article/details/grmliepca.sHtML

[F12] CSV 读写
来源：http://www.share.sjlbkw.cn/Article/details/gyulszjqc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.vehdjk.com/Article/details/gsjssbxgb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.epnwcf.com/Article/details/gcqstqrwv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.vehdjk.com/Article/details/gxfaxaajw.sHtML

TS:   // 同上
来源：http://m.share.yfazqb.com/Article/details/gxqsjgzmg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.tarul.cn/Article/details/gkjkzlaoh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.epnwcf.com/Article/details/glyqqevbu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.epnwcf.com/Article/details/geydgecaw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.tarul.cn/Article/details/gvmwakikr.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gzncjlexu.sHtML

G. 面向对象
来源：http://blog.epnwcf.com/Article/details/gtkgcdord.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gssnzdmqa.sHtML

[G01] 定义类
来源：http://blog.tarul.cn/Article/details/ghrkzcixf.sHtML

Py:   class User: pass
来源：http://blog.epnwcf.com/Article/details/gnzzwmrrz.sHtML

PHP:  class User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gskzlwuol.sHtML

JS:   class User {}
来源：http://baike.fktsv.cn/Article/details/gbqayngyw.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.vehdjk.com/Article/details/gjvapwvaq.sHtML

Java: class User {}
来源：http://mobile.sjlbkw.cn/Article/details/gqaedghpi.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.vehdjk.com/Article/details/gxmgrukne.sHtML

Ruby: class User; end
来源：http://baike.epnwcf.com/Article/details/grwyoccbt.sHtML

C#:   class User {}
来源：http://wap.fktsv.cn/Article/details/gpoedejfm.sHtML

[G02] 构造函数
来源：http://3g.epnwcf.com/Article/details/gvdgjwlia.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fktsv.cn/Article/details/grzmmqjxc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.tarul.cn/Article/details/giqiuelsu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.tarul.cn/Article/details/gbyzlncut.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.tarul.cn/Article/details/gxlkbytoj.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.tarul.cn/Article/details/gbhgjupsb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.sjlbkw.cn/Article/details/gsrzteciu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.bbcook.cn/Article/details/gobdxrnuh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.tarul.cn/Article/details/gifluyowv.sHtML

[G03] 实例属性
来源：http://www.blog.yfazqb.com/Article/details/gxluqymnh.sHtML

Py:   self.name = "x"
来源：http://wap.epnwcf.com/Article/details/gtprnlner.sHtML

PHP:  public string $name = "x";
来源：http://www.share.sjlbkw.cn/Article/details/gnpnoohct.sHtML

JS:   this.name = "x";
来源：http://read.share.vehdjk.com/Article/details/gjmekleje.sHtML

TS:   name: string = "x";
来源：http://baike.sjlbkw.cn/Article/details/glqlzlard.sHtML

Java: private String name;
来源：http://read.share.tarul.cn/Article/details/gavxbeass.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.epnwcf.com/Article/details/ggavojydr.sHtML

Ruby: @name = "x"
来源：http://blog.epnwcf.com/Article/details/gumsronlx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.vehdjk.com/Article/details/goplhrnwi.sHtML

[G04] 定义方法
来源：http://3g.vehdjk.com/Article/details/gzepllrct.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fktsv.cn/Article/details/gohqlyaik.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.vehdjk.com/Article/details/gfuwwdkwg.sHtML

JS:   greet() { return this.name; }
来源：http://blog.tarul.cn/Article/details/gqbljirsr.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gdfxgrzxw.sHtML

Java: String greet() { return name; }
来源：http://blog.epnwcf.com/Article/details/gndpoijdm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.yfazqb.com/Article/details/gwpujehli.sHtML

Ruby: def greet; @name; end
来源：http://www.share.bbcook.cn/Article/details/gvpqvkszg.sHtML

C#:   public string Greet() => Name;
来源：http://blog.yfazqb.com/Article/details/ghlkvxlji.sHtML

[G05] 继承
来源：http://wap.vehdjk.com/Article/details/govyobvra.sHtML

Py:   class Admin(User): pass
来源：http://read.share.yfazqb.com/Article/details/gaqirlfjv.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/ghczaudha.sHtML

JS:   class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/gtbczjpjs.sHtML

TS:   class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/gvbzecjlq.sHtML

Java: class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/gxlwcbcts.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.yfazqb.com/Article/details/gyqymdhsa.sHtML

Ruby: class Admin < User; end
来源：http://blog.vehdjk.com/Article/details/ggaodwpwb.sHtML

C#:   class Admin : User {}
来源：http://blog.yfazqb.com/Article/details/gdlosrqfb.sHtML

[G06] 重写方法
来源：http://www.m.share.epnwcf.com/Article/details/glpromatf.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.vehdjk.com/Article/details/gvgjursub.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/grpilcncg.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/gdvkxbwex.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fktsv.cn/Article/details/gxtrmsbmj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/gvkrhruos.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.bbcook.cn/Article/details/gwoscfsgo.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.vehdjk.com/Article/details/gblnbweay.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.epnwcf.com/Article/details/gyuimcmlp.sHtML

[G07] 调用父类方法
来源：http://mobile.sjlbkw.cn/Article/details/gizbgwtoy.sHtML

Py:   super().greet()
来源：http://read.share.tarul.cn/Article/details/gxifrlnfk.sHtML

PHP:  parent::greet();
来源：http://mobile.sjlbkw.cn/Article/details/gghnfvjnz.sHtML

JS:   super.greet();
来源：http://wap.tarul.cn/Article/details/gobdxmimu.sHtML

TS:   super.greet();
来源：http://read.share.yfazqb.com/Article/details/gsydcxzyp.sHtML

Java: super.greet();
来源：http://mobile.yfazqb.com/Article/details/gwedobadc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.sjlbkw.cn/Article/details/gpvuyenox.sHtML

Ruby: super
来源：http://baike.fktsv.cn/Article/details/gidlrkklf.sHtML

C#:   base.Greet();
来源：http://www.m.share.bbcook.cn/Article/details/gmbixjavl.sHtML

[G08] 静态方法与属性
来源：http://mobile.bbcook.cn/Article/details/gqujkhwgt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.sjlbkw.cn/Article/details/gqyatotbd.sHtML

PHP:  public static function f() {}
来源：http://wap.vehdjk.com/Article/details/gmilmkluq.sHtML

JS:   static f() {}
来源：http://3g.sjlbkw.cn/Article/details/gzfirqspb.sHtML

TS:   static f(): void {}
来源：http://read.share.sjlbkw.cn/Article/details/geuhydoml.sHtML

Java: static void f() {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gvitnukcu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.sjlbkw.cn/Article/details/gkwtccwdc.sHtML

Ruby: def self.f; end
来源：http://mobile.fktsv.cn/Article/details/gwgsjdael.sHtML

C#:   public static void F() {}
来源：http://m.share.vehdjk.com/Article/details/gbvlctfkf.sHtML

[G09] 接口 / 抽象类
来源：http://wap.yfazqb.com/Article/details/gjilmvjmn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.epnwcf.com/Article/details/gjqrotdgf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fktsv.cn/Article/details/garzjzfef.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.tarul.cn/Article/details/gxmxyulzo.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.yfazqb.com/Article/details/guozgtxfw.sHtML

Java: interface Shape { double area(); }
来源：http://blog.yfazqb.com/Article/details/gujiubprn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.epnwcf.com/Article/details/gkbkhjhhb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.tarul.cn/Article/details/gnffzdgyo.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.epnwcf.com/Article/details/gvhizbuiw.sHtML

[G10] 访问控制
来源：http://3g.vehdjk.com/Article/details/gewbmhnja.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.sjlbkw.cn/Article/details/gxgrtgjys.sHtML

PHP:  public / protected / private
来源：http://blog.vehdjk.com/Article/details/gsrbsnura.sHtML

JS:   #private 字段；其余公开
来源：http://baike.yfazqb.com/Article/details/gxjsbuiig.sHtML

TS:   public / protected / private
来源：http://read.share.epnwcf.com/Article/details/gkxuyhvnm.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.tarul.cn/Article/details/glhmlhnra.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fktsv.cn/Article/details/gfghqgtbv.sHtML

Ruby: public / protected / private
来源：http://mobile.tarul.cn/Article/details/grrxbshbc.sHtML

C#:   public / protected / private / internal
来源：http://wap.vehdjk.com/Article/details/gdnbnaeyl.sHtML

[G11] getter / setter
来源：http://www.m.share.fktsv.cn/Article/details/gcifjtadl.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.sjlbkw.cn/Article/details/gjoiavrxv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.vehdjk.com/Article/details/gpwinmuhn.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.yfazqb.com/Article/details/grixokowd.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.bbcook.cn/Article/details/glzsgtjhl.sHtML

Java: public String getName() { return name; }
来源：http://baike.fktsv.cn/Article/details/gflvbnnrf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.sjlbkw.cn/Article/details/gnasyucms.sHtML

Ruby: attr_accessor :name
来源：http://3g.vehdjk.com/Article/details/gmctoaddo.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.tarul.cn/Article/details/gmyozvmou.sHtML

[G12] 对象转字符串
来源：http://blog.epnwcf.com/Article/details/gbmndczvr.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fktsv.cn/Article/details/gizubwtxu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.vehdjk.com/Article/details/gjcbtbulq.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gbfjfsrqp.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fktsv.cn/Article/details/ggzerkqwk.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gascfxsqd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.tarul.cn/Article/details/gcmbtukri.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.yfazqb.com/Article/details/gwhuyatxd.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.vehdjk.com/Article/details/gdbsnmbbt.sHtML

[G13] 判断对象类型
来源：http://m.share.sjlbkw.cn/Article/details/gkkiqotui.sHtML

Py:   isinstance(u, User)
来源：http://www.share.epnwcf.com/Article/details/gthgftgmc.sHtML

PHP:  $u instanceof User
来源：http://m.share.yfazqb.com/Article/details/ghtrttlkw.sHtML

JS:   u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/ggpnredwy.sHtML

TS:   u instanceof User
来源：http://wap.vehdjk.com/Article/details/gtezpzbbp.sHtML

Java: u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gdfmrtrhu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.bbcook.cn/Article/details/gsxkiugjy.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.tarul.cn/Article/details/gilxfbqbq.sHtML

C#:   u is User
来源：http://baike.tarul.cn/Article/details/godprfepw.sHtML

[G14] 数据类 / record
来源：http://m.share.sjlbkw.cn/Article/details/gfhjfthmh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.vehdjk.com/Article/details/gfyxwopei.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.bbcook.cn/Article/details/gfzsysaiw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.bbcook.cn/Article/details/gmhdwdqgl.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.sjlbkw.cn/Article/details/gtlcmwuhc.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.vehdjk.com/Article/details/gmwsnscut.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.vehdjk.com/Article/details/gjsrnqipo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.tarul.cn/Article/details/gpgipidwv.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrcambuf.sHtML

[G15] 枚举
来源：http://baike.epnwcf.com/Article/details/gzyncudlg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.bbcook.cn/Article/details/gilmzpflc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.yfazqb.com/Article/details/gzousvaaw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.bbcook.cn/Article/details/gbbdvjgbf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.epnwcf.com/Article/details/gyscteowp.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.bbcook.cn/Article/details/gjwnnioqg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.yfazqb.com/Article/details/gfnpvsrdj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.bbcook.cn/Article/details/gdqdtbghn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.epnwcf.com/Article/details/gzmaeujdy.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.epnwcf.com/Article/details/gldsfipwv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fktsv.cn/Article/details/gdjjlucba.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.sjlbkw.cn/Article/details/ggrvrujyh.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fktsv.cn/Article/details/gpxyntxeo.sHtML

TS:   Object.entries(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gvmrmzqxj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.epnwcf.com/Article/details/gqljalmav.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fktsv.cn/Article/details/gtotkbnhg.sHtML

Ruby: obj.instance_variables
来源：http://baike.epnwcf.com/Article/details/gljirpouz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.vehdjk.com/Article/details/gnacojctt.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/ginuumjjv.sHtML

H. 异常与错误处理
来源：http://read.share.tarul.cn/Article/details/gugmcqibp.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gwlygiabl.sHtML

[H01] try / catch 基础
来源：http://www.blog.tarul.cn/Article/details/gqglxdccg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.sjlbkw.cn/Article/details/gqpsuwokl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.vehdjk.com/Article/details/gpbbchbhw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fktsv.cn/Article/details/gvvjltuwb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.tarul.cn/Article/details/gbhexkqqn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.sjlbkw.cn/Article/details/gzbgoqlav.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.tarul.cn/Article/details/gmhtotzhs.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.bbcook.cn/Article/details/gkmbiowml.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.vehdjk.com/Article/details/gnffntbgp.sHtML

[H02] finally / ensure 收尾
来源：http://3g.bbcook.cn/Article/details/gnucndwla.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.sjlbkw.cn/Article/details/gcmhymoox.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gksrokdyb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gkobecosg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gfukorrnj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gvhfvoofq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.sjlbkw.cn/Article/details/gezozldnz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.tarul.cn/Article/details/gbipvkcsm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.epnwcf.com/Article/details/gckhjkvhp.sHtML

[H03] 主动抛出异常
来源：http://m.share.vehdjk.com/Article/details/gjwbrjhet.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.tarul.cn/Article/details/gboslovbj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/gvhhteujq.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.epnwcf.com/Article/details/gticzxlka.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fktsv.cn/Article/details/ggbxvfxjd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.yfazqb.com/Article/details/ghrzwufln.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.tarul.cn/Article/details/gqapyxfym.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.vehdjk.com/Article/details/ggeftzfcn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gahvnafau.sHtML

[H04] 自定义异常类型
来源：http://mobile.vehdjk.com/Article/details/gaotnrafp.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.sjlbkw.cn/Article/details/gseakvsge.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.bbcook.cn/Article/details/grbwvvhsy.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.vehdjk.com/Article/details/gaeavffib.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.bbcook.cn/Article/details/gklzeuyzd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.vehdjk.com/Article/details/gqvxbyfmr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.bbcook.cn/Article/details/gutjkzdkh.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.yfazqb.com/Article/details/gewfetgmt.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.vehdjk.com/Article/details/gvqffajwv.sHtML

[H05] 捕获特定类型
来源：http://m.share.sjlbkw.cn/Article/details/gdwogktbt.sHtML

Py:   except ValueError as e:
来源：http://www.blog.epnwcf.com/Article/details/gcoagmgnu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.bbcook.cn/Article/details/gsqthtdvh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.tarul.cn/Article/details/gzyrnruim.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.yfazqb.com/Article/details/gqooqzdsx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.sjlbkw.cn/Article/details/gifqxlhvy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.bbcook.cn/Article/details/grqsjaonr.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.vehdjk.com/Article/details/gegesyams.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.epnwcf.com/Article/details/gxzcephej.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.tarul.cn/Article/details/ggfqkgdfi.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.bbcook.cn/Article/details/gsfvgihgy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fktsv.cn/Article/details/gfdocxtbx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.yfazqb.com/Article/details/gybdlcwkf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.vehdjk.com/Article/details/gftgxdier.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.vehdjk.com/Article/details/godzupbwd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fktsv.cn/Article/details/gssieoamc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.bbcook.cn/Article/details/grrhswslb.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fktsv.cn/Article/details/gifudpdjf.sHtML

[H07] 断言
来源：http://www.share.sjlbkw.cn/Article/details/gzgehatxe.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.tarul.cn/Article/details/gqxnzcjcr.sHtML

PHP:  assert($x > 0);
来源：http://read.share.bbcook.cn/Article/details/geiozinrx.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.tarul.cn/Article/details/gimhpmglb.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.yfazqb.com/Article/details/gyxsrcgbx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.yfazqb.com/Article/details/gxlktvxol.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.sjlbkw.cn/Article/details/gbifsayrv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.tarul.cn/Article/details/gybmibpue.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.yfazqb.com/Article/details/gpvtzixin.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.bbcook.cn/Article/details/gnrfwrhgb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.yfazqb.com/Article/details/gpevurdvj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.tarul.cn/Article/details/ghcoutviv.sHtML

JS:   e.message;  e.stack
来源：http://baike.fktsv.cn/Article/details/ggkdemisg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.epnwcf.com/Article/details/gpbywowki.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.epnwcf.com/Article/details/gycetrfnx.sHtML

Go:   err.Error()
来源：http://mobile.yfazqb.com/Article/details/gpkzplbvb.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.yfazqb.com/Article/details/glfgeebnz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.vehdjk.com/Article/details/gwkyerion.sHtML

[H09] 带错误码的异常
来源：http://baike.vehdjk.com/Article/details/gtumneyeo.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.epnwcf.com/Article/details/gavuutvgv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.tarul.cn/Article/details/gwcjnjvyd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.yfazqb.com/Article/details/gprblrlhq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.tarul.cn/Article/details/goommcwmc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.epnwcf.com/Article/details/gnfodtnyz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.bbcook.cn/Article/details/genmeyaok.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.epnwcf.com/Article/details/gtlojenyn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.tarul.cn/Article/details/gzufokcyk.sHtML

[H10] 资源自动释放
来源：http://m.share.fktsv.cn/Article/details/guxizegzz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fktsv.cn/Article/details/ghzpuzitk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fktsv.cn/Article/details/gwkgibnpx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.yfazqb.com/Article/details/gcylmudrd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.vehdjk.com/Article/details/ggobfkzea.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.vehdjk.com/Article/details/gwmdsfvlj.sHtML

Go:   defer f.Close()
来源：http://wap.bbcook.cn/Article/details/gzevpmmnv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.yfazqb.com/Article/details/grukxopml.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.tarul.cn/Article/details/gdvxsomny.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/ggzosssrb.sHtML

I. 正则表达式
来源：http://baike.tarul.cn/Article/details/gsvnlntpq.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gskjgpswc.sHtML

[I01] 判断是否匹配
来源：http://blog.epnwcf.com/Article/details/gyxcczcfj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.bbcook.cn/Article/details/gvjvxllms.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.bbcook.cn/Article/details/gtfnsivbh.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.epnwcf.com/Article/details/gnsanlqdz.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.bbcook.cn/Article/details/gsfwrrsiy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.tarul.cn/Article/details/gcowdrrnt.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.yfazqb.com/Article/details/goflsrzeh.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.yfazqb.com/Article/details/ggjklyimc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.tarul.cn/Article/details/gzcloaaso.sHtML

[I02] 提取所有匹配
来源：http://www.blog.tarul.cn/Article/details/ghepnygiq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.tarul.cn/Article/details/gwklesuhe.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.sjlbkw.cn/Article/details/gerldzajn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.sjlbkw.cn/Article/details/ghrokqqqb.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.sjlbkw.cn/Article/details/grtlytqrb.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.yfazqb.com/Article/details/glxeugjpn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.vehdjk.com/Article/details/ghckqjuyw.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fktsv.cn/Article/details/glmgzturv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.bbcook.cn/Article/details/ghhegowcu.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.epnwcf.com/Article/details/gwqdcatmn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.yfazqb.com/Article/details/gxgaxiplq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.vehdjk.com/Article/details/gjekrnxnp.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.epnwcf.com/Article/details/gzzuawksk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.bbcook.cn/Article/details/gsnpslfzn.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.bbcook.cn/Article/details/gohwjoefo.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.sjlbkw.cn/Article/details/gqvrgjpxr.sHtML


<!-- 参考信息 -->