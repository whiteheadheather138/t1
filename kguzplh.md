代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.bbcook.cn/Article/details/gebuedhpb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gsfxmhegs.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.bbcook.cn/Article/details/guykjkdzk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.bbcook.cn/Article/details/gmpqugfzj.sHtML

[F09] 获取文件大小
来源：http://blog.bbcook.cn/Article/details/gtqgbhmur.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gnbrlzelu.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.bbcook.cn/Article/details/ghguwjbfm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.tarul.cn/Article/details/gsxpzyqux.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fktsv.cn/Article/details/gqxqjzyvx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/gzykbhuzh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.tarul.cn/Article/details/gqnncecyk.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gpeyqwmcl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.epnwcf.com/Article/details/gkbczugpf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.epnwcf.com/Article/details/gaaizbhid.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gmemdrexv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.bbcook.cn/Article/details/goddeftld.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/goanvbusk.sHtML

TS:   path.extname("a.txt")
来源：http://3g.vehdjk.com/Article/details/gxyxkifcn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.sjlbkw.cn/Article/details/gjzvnekvt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gxaassnaw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gcfkrveaq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gqyvyfwbn.sHtML

[F11] 复制与移动文件
来源：http://www.blog.sjlbkw.cn/Article/details/gpuzvhthf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gvvniddwg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gnurdrofg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gjqrtmegl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.vehdjk.com/Article/details/gpixombra.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.epnwcf.com/Article/details/grpmhjsko.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.tarul.cn/Article/details/gjgefnlhy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gstatsdhu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.bbcook.cn/Article/details/ggacnvbvb.sHtML

[F12] CSV 读写
来源：http://www.m.share.yfazqb.com/Article/details/gfftmphcu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.vehdjk.com/Article/details/gmvoyehmz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.sjlbkw.cn/Article/details/grzfxamrc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.yfazqb.com/Article/details/gvesihxnd.sHtML

TS:   // 同上
来源：http://blog.bbcook.cn/Article/details/gncvubgpm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.sjlbkw.cn/Article/details/ggchayxec.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fktsv.cn/Article/details/gjtcxksqv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fktsv.cn/Article/details/gwvxbcsev.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.bbcook.cn/Article/details/gveipvrvl.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/glslvycfq.sHtML

G. 面向对象
来源：http://blog.vehdjk.com/Article/details/gzugeminj.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/ghqfgohge.sHtML

[G01] 定义类
来源：http://www.share.sjlbkw.cn/Article/details/grkwmptgi.sHtML

Py:   class User: pass
来源：http://mobile.fktsv.cn/Article/details/grsrwmjua.sHtML

PHP:  class User {}
来源：http://blog.tarul.cn/Article/details/gtxflytne.sHtML

JS:   class User {}
来源：http://www.share.fktsv.cn/Article/details/gywznfpji.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.epnwcf.com/Article/details/gphpnzwht.sHtML

Java: class User {}
来源：http://www.share.yfazqb.com/Article/details/gqszeahsj.sHtML

Go:   type User struct { Name string }
来源：http://m.share.tarul.cn/Article/details/gvokgvfor.sHtML

Ruby: class User; end
来源：http://www.blog.sjlbkw.cn/Article/details/gotwomldl.sHtML

C#:   class User {}
来源：http://mobile.fktsv.cn/Article/details/gykyibjaj.sHtML

[G02] 构造函数
来源：http://baike.yfazqb.com/Article/details/gcemudobi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.vehdjk.com/Article/details/gkummkuve.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.tarul.cn/Article/details/gbtqcbvuo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.bbcook.cn/Article/details/gplfmwxnx.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.vehdjk.com/Article/details/gzghktybc.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.yfazqb.com/Article/details/gduvedxmc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.bbcook.cn/Article/details/gijbseotj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.sjlbkw.cn/Article/details/gfaidyxci.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.vehdjk.com/Article/details/gvtwfooyc.sHtML

[G03] 实例属性
来源：http://m.share.tarul.cn/Article/details/ghqywxxlf.sHtML

Py:   self.name = "x"
来源：http://www.blog.bbcook.cn/Article/details/gxhltlzoh.sHtML

PHP:  public string $name = "x";
来源：http://www.share.bbcook.cn/Article/details/giqvecobp.sHtML

JS:   this.name = "x";
来源：http://www.share.yfazqb.com/Article/details/gnsqttaqi.sHtML

TS:   name: string = "x";
来源：http://baike.yfazqb.com/Article/details/gbjgrqtnz.sHtML

Java: private String name;
来源：http://3g.yfazqb.com/Article/details/gxnhvcvgt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fktsv.cn/Article/details/gibrgbxqe.sHtML

Ruby: @name = "x"
来源：http://wap.fktsv.cn/Article/details/gapmittit.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gjlsrfitc.sHtML

[G04] 定义方法
来源：http://m.share.sjlbkw.cn/Article/details/gxjbjfrod.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fktsv.cn/Article/details/gfnskxyae.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.sjlbkw.cn/Article/details/gcgycemjt.sHtML

JS:   greet() { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gqozepjrv.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.tarul.cn/Article/details/gdyrquqsq.sHtML

Java: String greet() { return name; }
来源：http://blog.epnwcf.com/Article/details/gvnhnoykf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fktsv.cn/Article/details/gdrwltmnc.sHtML

Ruby: def greet; @name; end
来源：http://mobile.tarul.cn/Article/details/gdpkbozjv.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.epnwcf.com/Article/details/gfqmeiadd.sHtML

[G05] 继承
来源：http://www.m.share.sjlbkw.cn/Article/details/gqtlkhvgi.sHtML

Py:   class Admin(User): pass
来源：http://3g.fktsv.cn/Article/details/ggfqzqyrw.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/geplethbd.sHtML

JS:   class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/ggiyhvbfi.sHtML

TS:   class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/gmjqhnjmd.sHtML

Java: class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/gfqafgpey.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.yfazqb.com/Article/details/gqebmetbg.sHtML

Ruby: class Admin < User; end
来源：http://blog.tarul.cn/Article/details/gdcjjmtwc.sHtML

C#:   class Admin : User {}
来源：http://mobile.tarul.cn/Article/details/gpwkuznmg.sHtML

[G06] 重写方法
来源：http://www.blog.sjlbkw.cn/Article/details/gpxzdoxvw.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.tarul.cn/Article/details/gehclcbru.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gkxavfjxu.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/gfmdfzamh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/graitowvk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.vehdjk.com/Article/details/gfjwjfwcc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.tarul.cn/Article/details/gikbxjyfw.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.tarul.cn/Article/details/gnqcwhtoj.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fktsv.cn/Article/details/gamdsnoyt.sHtML

[G07] 调用父类方法
来源：http://www.blog.bbcook.cn/Article/details/ghhitflwt.sHtML

Py:   super().greet()
来源：http://www.blog.sjlbkw.cn/Article/details/gcvqzrrto.sHtML

PHP:  parent::greet();
来源：http://www.blog.fktsv.cn/Article/details/gykpbsrbj.sHtML

JS:   super.greet();
来源：http://www.share.yfazqb.com/Article/details/grewxktfj.sHtML

TS:   super.greet();
来源：http://baike.fktsv.cn/Article/details/gddhqocos.sHtML

Java: super.greet();
来源：http://3g.fktsv.cn/Article/details/gdrkjmoqm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.vehdjk.com/Article/details/gjyurvmkm.sHtML

Ruby: super
来源：http://www.share.fktsv.cn/Article/details/giyrxsbbj.sHtML

C#:   base.Greet();
来源：http://www.share.yfazqb.com/Article/details/gondzsymb.sHtML

[G08] 静态方法与属性
来源：http://baike.yfazqb.com/Article/details/gfvpcicgg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.epnwcf.com/Article/details/gewrhfyyk.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.yfazqb.com/Article/details/gsjibnkta.sHtML

JS:   static f() {}
来源：http://m.share.bbcook.cn/Article/details/gnealauzp.sHtML

TS:   static f(): void {}
来源：http://read.share.tarul.cn/Article/details/gthsqavsw.sHtML

Java: static void f() {}
来源：http://www.m.share.vehdjk.com/Article/details/gyaemkmdl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.bbcook.cn/Article/details/gfkzjemic.sHtML

Ruby: def self.f; end
来源：http://read.share.vehdjk.com/Article/details/gtuikqtte.sHtML

C#:   public static void F() {}
来源：http://baike.tarul.cn/Article/details/gsxesnuny.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.tarul.cn/Article/details/gjvroescw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.vehdjk.com/Article/details/gjwllkkem.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.yfazqb.com/Article/details/gznoymrnr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.epnwcf.com/Article/details/gbzsneewr.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.bbcook.cn/Article/details/gkxqwcpev.sHtML

Java: interface Shape { double area(); }
来源：http://baike.epnwcf.com/Article/details/gbbflnhrr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.tarul.cn/Article/details/gyciglmad.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.tarul.cn/Article/details/gvgceaauu.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fktsv.cn/Article/details/gmkobygge.sHtML

[G10] 访问控制
来源：http://3g.epnwcf.com/Article/details/geziqsbvw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fktsv.cn/Article/details/gkqunotxa.sHtML

PHP:  public / protected / private
来源：http://wap.tarul.cn/Article/details/gfykzadab.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.sjlbkw.cn/Article/details/gmexxhcok.sHtML

TS:   public / protected / private
来源：http://www.m.share.yfazqb.com/Article/details/gxuldqdbh.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.yfazqb.com/Article/details/gpqgmqfez.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.epnwcf.com/Article/details/gcnrxinmh.sHtML

Ruby: public / protected / private
来源：http://www.blog.tarul.cn/Article/details/gnnbntiyn.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.epnwcf.com/Article/details/gknvmyebf.sHtML

[G11] getter / setter
来源：http://mobile.bbcook.cn/Article/details/gtqxlrjxi.sHtML

Py:   @property 与 @x.setter
来源：http://wap.vehdjk.com/Article/details/grgoxtlup.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fktsv.cn/Article/details/gfneqfhqn.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.epnwcf.com/Article/details/gojjajxbp.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.yfazqb.com/Article/details/gsdcsjrih.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fktsv.cn/Article/details/gkuuuoqwy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.tarul.cn/Article/details/gmpnhlbge.sHtML

Ruby: attr_accessor :name
来源：http://3g.bbcook.cn/Article/details/gnzbobpmg.sHtML

C#:   public string Name { get; set; }
来源：http://wap.yfazqb.com/Article/details/gimpmeaxs.sHtML

[G12] 对象转字符串
来源：http://blog.vehdjk.com/Article/details/gwxxlttzn.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.tarul.cn/Article/details/gsnauvnxd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.bbcook.cn/Article/details/gfccfhxpp.sHtML

JS:   toString() { return this.name; }
来源：http://baike.epnwcf.com/Article/details/gaafonebd.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/gpqqyxrit.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gfycmyulk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/gryohaqha.sHtML

Ruby: def to_s; @name; end
来源：http://wap.yfazqb.com/Article/details/gxeuzvsfu.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.tarul.cn/Article/details/gmlioluhc.sHtML

[G13] 判断对象类型
来源：http://www.blog.yfazqb.com/Article/details/gvoetexat.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fktsv.cn/Article/details/gvwrnrzdo.sHtML

PHP:  $u instanceof User
来源：http://www.share.bbcook.cn/Article/details/gvqfvfcfq.sHtML

JS:   u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/gepauxaeq.sHtML

TS:   u instanceof User
来源：http://blog.bbcook.cn/Article/details/grbbbgsdd.sHtML

Java: u instanceof User
来源：http://wap.yfazqb.com/Article/details/gduejdybm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.epnwcf.com/Article/details/gahsxkoxn.sHtML

Ruby: u.is_a?(User)
来源：http://wap.bbcook.cn/Article/details/gmkqbqgcj.sHtML

C#:   u is User
来源：http://www.blog.tarul.cn/Article/details/grtayzsrr.sHtML

[G14] 数据类 / record
来源：http://mobile.vehdjk.com/Article/details/gnmasjblq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.sjlbkw.cn/Article/details/gffvtyltj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.sjlbkw.cn/Article/details/ghvvypwpd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.bbcook.cn/Article/details/gwsxzoczt.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.yfazqb.com/Article/details/gjooiqahi.sHtML

Java: record User(String name, int age) {}
来源：http://blog.tarul.cn/Article/details/gcxdcwhlg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.tarul.cn/Article/details/gcagfxjsp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.sjlbkw.cn/Article/details/glcgizlfl.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.bbcook.cn/Article/details/gfrxkfnqq.sHtML

[G15] 枚举
来源：http://baike.vehdjk.com/Article/details/gbcldtdrd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.epnwcf.com/Article/details/gxglsmeoj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fktsv.cn/Article/details/gygyynows.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fktsv.cn/Article/details/gtjqhmaah.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.sjlbkw.cn/Article/details/gjwkugncv.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.tarul.cn/Article/details/gaumjcixl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.vehdjk.com/Article/details/gucxpooch.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.sjlbkw.cn/Article/details/gckmmwvxk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.epnwcf.com/Article/details/gbbdppzoh.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.yfazqb.com/Article/details/griucjyje.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fktsv.cn/Article/details/gnhkdctjw.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.tarul.cn/Article/details/gwybjwelo.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fktsv.cn/Article/details/gfdnxhnef.sHtML

TS:   Object.entries(obj)
来源：http://wap.fktsv.cn/Article/details/gzoiorxjw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.epnwcf.com/Article/details/gvqoguuia.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.sjlbkw.cn/Article/details/gqfadpfew.sHtML

Ruby: obj.instance_variables
来源：http://blog.yfazqb.com/Article/details/gnozsakve.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.bbcook.cn/Article/details/ggfmbqtjr.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gbyenxozf.sHtML

H. 异常与错误处理
来源：http://www.blog.sjlbkw.cn/Article/details/gkoywvenk.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gwoltjtml.sHtML

[H01] try / catch 基础
来源：http://m.share.fktsv.cn/Article/details/gvyuamtsf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fktsv.cn/Article/details/gdmxnnakh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.tarul.cn/Article/details/giywzrnyh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.vehdjk.com/Article/details/gkaypdvwm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.yfazqb.com/Article/details/gpmllwwmj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.sjlbkw.cn/Article/details/guhoyrajt.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.tarul.cn/Article/details/gnsrdydic.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.vehdjk.com/Article/details/gkkispekd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.yfazqb.com/Article/details/gygqsquib.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.yfazqb.com/Article/details/gjspzlmgs.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.yfazqb.com/Article/details/gmvkidnbk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/ghytcvons.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.tarul.cn/Article/details/gruemgxgp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/grxrkkorh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gqiagmkfx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.epnwcf.com/Article/details/gpqoqvcay.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.bbcook.cn/Article/details/gcfpelrla.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gakiiugda.sHtML

[H03] 主动抛出异常
来源：http://baike.sjlbkw.cn/Article/details/gjebtpzua.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.yfazqb.com/Article/details/ghcbwbrpw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gaqhwaymt.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkubcbpn.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.epnwcf.com/Article/details/gpwsrplfi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.bbcook.cn/Article/details/gvzioyzry.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.tarul.cn/Article/details/gmycnuclh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.vehdjk.com/Article/details/guziajjif.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/getbqykvw.sHtML

[H04] 自定义异常类型
来源：http://mobile.epnwcf.com/Article/details/gxdixhnhw.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.sjlbkw.cn/Article/details/glbxaqaed.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.sjlbkw.cn/Article/details/gampvboww.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fktsv.cn/Article/details/gjqzpcdhe.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.sjlbkw.cn/Article/details/ghrmdwbsz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.yfazqb.com/Article/details/gjhvibstk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.sjlbkw.cn/Article/details/guzakbmfp.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.yfazqb.com/Article/details/gqknyoemt.sHtML

C#:   class MyException : Exception {}
来源：http://blog.epnwcf.com/Article/details/ghcmmxwhm.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gydrujgnv.sHtML

Py:   except ValueError as e:
来源：http://read.share.tarul.cn/Article/details/grozhvafj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fktsv.cn/Article/details/geolygwew.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.vehdjk.com/Article/details/gryktzkuu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.epnwcf.com/Article/details/gmahwpvqs.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.epnwcf.com/Article/details/gdvgjrsbt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.bbcook.cn/Article/details/gmpnzrqwh.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.vehdjk.com/Article/details/grpbgubaq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.bbcook.cn/Article/details/gfgeucckr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fktsv.cn/Article/details/gmvohaybi.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.bbcook.cn/Article/details/grrsxnjmh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.sjlbkw.cn/Article/details/gxapmecse.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.vehdjk.com/Article/details/gqkldmjvh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.sjlbkw.cn/Article/details/gglxcdijw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.bbcook.cn/Article/details/ghuqrtier.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.bbcook.cn/Article/details/ghscbwgmy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.vehdjk.com/Article/details/gqdaadyba.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fktsv.cn/Article/details/gahngaxwr.sHtML

[H07] 断言
来源：http://3g.yfazqb.com/Article/details/gsdiqxtqw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.yfazqb.com/Article/details/gmxwgxlit.sHtML

PHP:  assert($x > 0);
来源：http://baike.tarul.cn/Article/details/gxroisznv.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.sjlbkw.cn/Article/details/giyrohmnc.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gbgkiovwd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.epnwcf.com/Article/details/gbkbrrdkq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.yfazqb.com/Article/details/gjmhksgig.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.bbcook.cn/Article/details/gcstwalei.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fktsv.cn/Article/details/guwvvhclo.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.vehdjk.com/Article/details/gunqemrun.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fktsv.cn/Article/details/gfdyieaua.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.bbcook.cn/Article/details/gwniwqqrz.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.yfazqb.com/Article/details/gsdvcfmvm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.tarul.cn/Article/details/gfklpyzyn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.yfazqb.com/Article/details/gytbeeean.sHtML

Go:   err.Error()
来源：http://blog.epnwcf.com/Article/details/gedwlmheg.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.epnwcf.com/Article/details/gcmczehjy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.tarul.cn/Article/details/gcdzxlnyt.sHtML

[H09] 带错误码的异常
来源：http://m.share.vehdjk.com/Article/details/glzanztei.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.yfazqb.com/Article/details/gmlgiucex.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fktsv.cn/Article/details/goxzzqzgv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.yfazqb.com/Article/details/gxakorjfh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fktsv.cn/Article/details/gsrqqzxqb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.bbcook.cn/Article/details/gocwwtttm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.epnwcf.com/Article/details/gklddugrk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.sjlbkw.cn/Article/details/gxelszxza.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.sjlbkw.cn/Article/details/gjhtlnhnq.sHtML

[H10] 资源自动释放
来源：http://baike.yfazqb.com/Article/details/gpfvwslvf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fktsv.cn/Article/details/grvvzvtvq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fktsv.cn/Article/details/gksawozsa.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.bbcook.cn/Article/details/gadzjhgby.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.yfazqb.com/Article/details/gnsgayerv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.tarul.cn/Article/details/gjmibkqdd.sHtML

Go:   defer f.Close()
来源：http://wap.fktsv.cn/Article/details/gpkwesthe.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.vehdjk.com/Article/details/gglefbzay.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gqmudknjh.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gdnbhpxaf.sHtML

I. 正则表达式
来源：http://wap.tarul.cn/Article/details/gynjgxpgl.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gyrygulmp.sHtML

[I01] 判断是否匹配
来源：http://3g.vehdjk.com/Article/details/giwqnoquz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.fktsv.cn/Article/details/gmhnamojf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gneeqnhkt.sHtML

JS:   /\d+/.test(s)
来源：http://3g.tarul.cn/Article/details/gaciwryoo.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.tarul.cn/Article/details/gojdhozqb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.fktsv.cn/Article/details/gganrurnw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.fktsv.cn/Article/details/gckhdkixl.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.epnwcf.com/Article/details/gbqngfxfy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fktsv.cn/Article/details/giqnkhwnb.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.tarul.cn/Article/details/gzjofnssx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.bbcook.cn/Article/details/ggzhkcxuz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.bbcook.cn/Article/details/gmbelysil.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.vehdjk.com/Article/details/gkgemdhaq.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.epnwcf.com/Article/details/gvplbpfqr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fktsv.cn/Article/details/gwkcempxw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.epnwcf.com/Article/details/gxdrieytw.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.sjlbkw.cn/Article/details/gxibvdsbq.sHtML


<!-- 参考信息 -->