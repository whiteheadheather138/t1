代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.sjlbkw.cn/Article/details/gtaawhlqf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.sjlbkw.cn/Article/details/gkzqazwrn.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.bbcook.cn/Article/details/gpsamuasm.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.vehdjk.com/Article/details/gvutwflaj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.sjlbkw.cn/Article/details/gchxkmllc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fktsv.cn/Article/details/gnpfjsybv.sHtML

Ruby: Dir.children("dir")
来源：http://3g.bbcook.cn/Article/details/gaacielnm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.epnwcf.com/Article/details/gyurhumhr.sHtML

[F09] 获取文件大小
来源：http://read.share.epnwcf.com/Article/details/gwvaublnu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.yfazqb.com/Article/details/gkaizrqea.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gxdfzipjz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.yfazqb.com/Article/details/gpfgpdhwc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.vehdjk.com/Article/details/gymzdmqcj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gxlqzxdkr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.yfazqb.com/Article/details/grdyfoyvp.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqwczdfpp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.epnwcf.com/Article/details/gfghakmaz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.bbcook.cn/Article/details/gvxxqbocm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/gbqonhwcc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.bbcook.cn/Article/details/ggiibsirj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gjzewcqek.sHtML

TS:   path.extname("a.txt")
来源：http://3g.vehdjk.com/Article/details/gjfggojgn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fktsv.cn/Article/details/gcffjldom.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/gkpnwnutt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gihrhnjmi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gftwrksgb.sHtML

[F11] 复制与移动文件
来源：http://3g.vehdjk.com/Article/details/gmbhfkqhu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gmfmbzvai.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gzgvcvwtl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/glcpmqzsh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/glzezgcbl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.sjlbkw.cn/Article/details/gncshnccj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.sjlbkw.cn/Article/details/gxwtrlfii.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/gkyzdxgeh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.sjlbkw.cn/Article/details/gevyglqhs.sHtML

[F12] CSV 读写
来源：http://m.share.fktsv.cn/Article/details/gibvlrvkp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.vehdjk.com/Article/details/gtlicmszx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.bbcook.cn/Article/details/gqzgpmvfw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.bbcook.cn/Article/details/geemafvng.sHtML

TS:   // 同上
来源：http://read.share.yfazqb.com/Article/details/gnwbwakgu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.vehdjk.com/Article/details/gozrqdaln.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.bbcook.cn/Article/details/gockcbmcl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.bbcook.cn/Article/details/gdmlbciow.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.epnwcf.com/Article/details/gfxnvlpsb.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/ggqdiypgx.sHtML

G. 面向对象
来源：http://3g.fktsv.cn/Article/details/gpxsfflzo.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gavfpgfkn.sHtML

[G01] 定义类
来源：http://blog.tarul.cn/Article/details/gkfwpwxdn.sHtML

Py:   class User: pass
来源：http://mobile.tarul.cn/Article/details/glfmtgjkg.sHtML

PHP:  class User {}
来源：http://mobile.yfazqb.com/Article/details/gtohtpimm.sHtML

JS:   class User {}
来源：http://baike.yfazqb.com/Article/details/gaggqmymb.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fktsv.cn/Article/details/gjaurzxwd.sHtML

Java: class User {}
来源：http://baike.tarul.cn/Article/details/gonhqqzpw.sHtML

Go:   type User struct { Name string }
来源：http://3g.yfazqb.com/Article/details/gclczydlm.sHtML

Ruby: class User; end
来源：http://baike.fktsv.cn/Article/details/gbgklqkky.sHtML

C#:   class User {}
来源：http://www.blog.fktsv.cn/Article/details/gyfmxbmhs.sHtML

[G02] 构造函数
来源：http://baike.fktsv.cn/Article/details/ggbelnxbf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.yfazqb.com/Article/details/gjykaiyjq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.epnwcf.com/Article/details/gaoylrolj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fktsv.cn/Article/details/gynrbigha.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.bbcook.cn/Article/details/gmcujqzsr.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.epnwcf.com/Article/details/gsyrvupwb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.sjlbkw.cn/Article/details/gqwcxijeg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.epnwcf.com/Article/details/gomqqnhtg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.vehdjk.com/Article/details/gpethmazi.sHtML

[G03] 实例属性
来源：http://wap.vehdjk.com/Article/details/ghnmghtvc.sHtML

Py:   self.name = "x"
来源：http://baike.vehdjk.com/Article/details/gjygfyeyi.sHtML

PHP:  public string $name = "x";
来源：http://wap.tarul.cn/Article/details/givpcmser.sHtML

JS:   this.name = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gddacsnqz.sHtML

TS:   name: string = "x";
来源：http://3g.fktsv.cn/Article/details/gqpsetkfs.sHtML

Java: private String name;
来源：http://blog.fktsv.cn/Article/details/gfttpitny.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.bbcook.cn/Article/details/gmxsnltag.sHtML

Ruby: @name = "x"
来源：http://www.blog.epnwcf.com/Article/details/gbhnigvon.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.bbcook.cn/Article/details/gjletjeqd.sHtML

[G04] 定义方法
来源：http://wap.tarul.cn/Article/details/gxhelzxkl.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.vehdjk.com/Article/details/gyhhylxhq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.epnwcf.com/Article/details/ghljfhlhg.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.tarul.cn/Article/details/gekjdupik.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.vehdjk.com/Article/details/glymwhprp.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fktsv.cn/Article/details/gxnlxnbzz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.tarul.cn/Article/details/gomsvhsui.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.epnwcf.com/Article/details/gyrbjfvbd.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.vehdjk.com/Article/details/gvxcrovlp.sHtML

[G05] 继承
来源：http://www.m.share.tarul.cn/Article/details/gmtrrsocj.sHtML

Py:   class Admin(User): pass
来源：http://read.share.sjlbkw.cn/Article/details/gwpzpbqpn.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/guoclxnuv.sHtML

JS:   class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gfprfzyik.sHtML

TS:   class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/gwgaxohjs.sHtML

Java: class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/gvvohxnqx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.epnwcf.com/Article/details/ggyhjkclh.sHtML

Ruby: class Admin < User; end
来源：http://3g.bbcook.cn/Article/details/gltzcrgoe.sHtML

C#:   class Admin : User {}
来源：http://blog.bbcook.cn/Article/details/gylkmbudk.sHtML

[G06] 重写方法
来源：http://m.share.epnwcf.com/Article/details/ggbfxblst.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.tarul.cn/Article/details/gxwzboobr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/gmoppcaqd.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/ggutkbfxm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/gpzjfatub.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gwsiexswg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fktsv.cn/Article/details/gktgbklpa.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.vehdjk.com/Article/details/gwwrkztxk.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.vehdjk.com/Article/details/gxrwhjcgu.sHtML

[G07] 调用父类方法
来源：http://blog.fktsv.cn/Article/details/glkpxpinf.sHtML

Py:   super().greet()
来源：http://3g.bbcook.cn/Article/details/gdztlqlhq.sHtML

PHP:  parent::greet();
来源：http://baike.epnwcf.com/Article/details/gpvfikozv.sHtML

JS:   super.greet();
来源：http://read.share.fktsv.cn/Article/details/gtldkzhtc.sHtML

TS:   super.greet();
来源：http://m.share.epnwcf.com/Article/details/golsoffsw.sHtML

Java: super.greet();
来源：http://read.share.yfazqb.com/Article/details/guyjiprap.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.yfazqb.com/Article/details/gzwviykwv.sHtML

Ruby: super
来源：http://wap.yfazqb.com/Article/details/gbxptuywt.sHtML

C#:   base.Greet();
来源：http://wap.fktsv.cn/Article/details/ghpvejzsk.sHtML

[G08] 静态方法与属性
来源：http://m.share.yfazqb.com/Article/details/gxmaimeka.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.yfazqb.com/Article/details/gozblcgaq.sHtML

PHP:  public static function f() {}
来源：http://baike.sjlbkw.cn/Article/details/gfvdwkrqi.sHtML

JS:   static f() {}
来源：http://m.share.tarul.cn/Article/details/gubmrwoxb.sHtML

TS:   static f(): void {}
来源：http://wap.vehdjk.com/Article/details/gfqdtaijy.sHtML

Java: static void f() {}
来源：http://blog.sjlbkw.cn/Article/details/gpqzyaxji.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.bbcook.cn/Article/details/gpxcsesdo.sHtML

Ruby: def self.f; end
来源：http://wap.tarul.cn/Article/details/ghabepout.sHtML

C#:   public static void F() {}
来源：http://3g.vehdjk.com/Article/details/golwzlylk.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.epnwcf.com/Article/details/guzdgunyj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.bbcook.cn/Article/details/gxbzudnim.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.sjlbkw.cn/Article/details/glszstcke.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.vehdjk.com/Article/details/gvzyurmvb.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.tarul.cn/Article/details/gixmkhaiz.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.yfazqb.com/Article/details/gflwyvjsg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.yfazqb.com/Article/details/gihvrpiru.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.tarul.cn/Article/details/gaofbywqn.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.vehdjk.com/Article/details/gdzlxkvsr.sHtML

[G10] 访问控制
来源：http://m.share.vehdjk.com/Article/details/gppbzoudp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.bbcook.cn/Article/details/gxofeficb.sHtML

PHP:  public / protected / private
来源：http://baike.vehdjk.com/Article/details/gwyoxaibm.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fktsv.cn/Article/details/guezpfket.sHtML

TS:   public / protected / private
来源：http://www.blog.sjlbkw.cn/Article/details/gcqyszdbl.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.bbcook.cn/Article/details/grgycyyms.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.epnwcf.com/Article/details/gphylybsj.sHtML

Ruby: public / protected / private
来源：http://blog.epnwcf.com/Article/details/gaaxodfnw.sHtML

C#:   public / protected / private / internal
来源：http://www.share.sjlbkw.cn/Article/details/gbvdqhgou.sHtML

[G11] getter / setter
来源：http://baike.bbcook.cn/Article/details/grteiiqat.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.bbcook.cn/Article/details/gwvwedtip.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.bbcook.cn/Article/details/gpxfxsxmw.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.bbcook.cn/Article/details/gnndnejar.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fktsv.cn/Article/details/grrumdwgd.sHtML

Java: public String getName() { return name; }
来源：http://mobile.yfazqb.com/Article/details/gaczygmwa.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.sjlbkw.cn/Article/details/gucffgkta.sHtML

Ruby: attr_accessor :name
来源：http://www.share.vehdjk.com/Article/details/gcerqytci.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fktsv.cn/Article/details/gprqjxbqg.sHtML

[G12] 对象转字符串
来源：http://mobile.vehdjk.com/Article/details/gwjbahfcl.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.yfazqb.com/Article/details/gwwuqaxjd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.sjlbkw.cn/Article/details/gcqmzcqil.sHtML

JS:   toString() { return this.name; }
来源：http://baike.yfazqb.com/Article/details/ghwvslfuh.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.epnwcf.com/Article/details/gyssqbxly.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.epnwcf.com/Article/details/geuxesayk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/ghxcjcbat.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fktsv.cn/Article/details/garqtecap.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.vehdjk.com/Article/details/gfsytvzmw.sHtML

[G13] 判断对象类型
来源：http://blog.sjlbkw.cn/Article/details/gowibbedz.sHtML

Py:   isinstance(u, User)
来源：http://baike.fktsv.cn/Article/details/gyrlxbmou.sHtML

PHP:  $u instanceof User
来源：http://blog.yfazqb.com/Article/details/gtstnucxl.sHtML

JS:   u instanceof User
来源：http://blog.vehdjk.com/Article/details/gfosknhqg.sHtML

TS:   u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gdrjwliyj.sHtML

Java: u instanceof User
来源：http://wap.yfazqb.com/Article/details/gvwjygzyq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.vehdjk.com/Article/details/gnflglaxh.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.tarul.cn/Article/details/ggnnvblor.sHtML

C#:   u is User
来源：http://baike.tarul.cn/Article/details/gglvqkvuj.sHtML

[G14] 数据类 / record
来源：http://wap.vehdjk.com/Article/details/gsineyavs.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.bbcook.cn/Article/details/ggzuexwpz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.bbcook.cn/Article/details/giawoxffy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.epnwcf.com/Article/details/gneuyzckk.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.tarul.cn/Article/details/glpawnpmp.sHtML

Java: record User(String name, int age) {}
来源：http://baike.tarul.cn/Article/details/geymhdwxl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.sjlbkw.cn/Article/details/getrqpwoh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.bbcook.cn/Article/details/gdgotwpbo.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.sjlbkw.cn/Article/details/gfhiskjib.sHtML

[G15] 枚举
来源：http://baike.tarul.cn/Article/details/guozkkbvo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.bbcook.cn/Article/details/gjityiyjs.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fktsv.cn/Article/details/gwqhjavoh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.vehdjk.com/Article/details/gnmnyqtqg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.vehdjk.com/Article/details/gkdvhxrdi.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.yfazqb.com/Article/details/gxwtzqwqj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.yfazqb.com/Article/details/gqsuipyud.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.sjlbkw.cn/Article/details/gylcrfxlt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.epnwcf.com/Article/details/gwajkqtyj.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.yfazqb.com/Article/details/gcowowjzb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.epnwcf.com/Article/details/gpneadhkj.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.yfazqb.com/Article/details/gtqfpjadb.sHtML

JS:   Object.entries(obj)
来源：http://wap.sjlbkw.cn/Article/details/gycoljfgz.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.bbcook.cn/Article/details/gugrzmxyb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.yfazqb.com/Article/details/gbcgvfzib.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.bbcook.cn/Article/details/gcbvdrcsl.sHtML

Ruby: obj.instance_variables
来源：http://www.share.tarul.cn/Article/details/gmfgtjfop.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.tarul.cn/Article/details/gsjikpdye.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gkmtbuzgy.sHtML

H. 异常与错误处理
来源：http://www.m.share.fktsv.cn/Article/details/gdalqenrg.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gubyhrzap.sHtML

[H01] try / catch 基础
来源：http://wap.yfazqb.com/Article/details/gkruochib.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.tarul.cn/Article/details/ggvlcxxmo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fktsv.cn/Article/details/gazmocvxl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.bbcook.cn/Article/details/gjfnngbtf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.bbcook.cn/Article/details/gdvcrylah.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.tarul.cn/Article/details/gqtcdpzje.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.tarul.cn/Article/details/gvlvuuxsi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.vehdjk.com/Article/details/gbvnvduse.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.yfazqb.com/Article/details/ghbgmmawp.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fktsv.cn/Article/details/gdwrdiajl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fktsv.cn/Article/details/gzxwlchui.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gwrxxyyzs.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gcqwpzojx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gcircrfot.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/geauaspfq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.vehdjk.com/Article/details/gkfcvdjhx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.vehdjk.com/Article/details/gdbthmjkl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gnzaqvqif.sHtML

[H03] 主动抛出异常
来源：http://baike.vehdjk.com/Article/details/gubgptaox.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.yfazqb.com/Article/details/ghuyrempn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gunxyxsoy.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gaaitpxvz.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gcdpwympc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.epnwcf.com/Article/details/gxhvhjpbl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.yfazqb.com/Article/details/galfjhgcd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.yfazqb.com/Article/details/gevfebseo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gurutzuez.sHtML

[H04] 自定义异常类型
来源：http://wap.vehdjk.com/Article/details/gntbufdov.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.yfazqb.com/Article/details/gcogkstiz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.bbcook.cn/Article/details/gknuxjjwk.sHtML

JS:   class MyError extends Error {}
来源：http://blog.vehdjk.com/Article/details/gipxgmezj.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.bbcook.cn/Article/details/gqgcgnnbq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.tarul.cn/Article/details/gbisabriq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.vehdjk.com/Article/details/gsbppnwja.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.sjlbkw.cn/Article/details/gjrwawdmj.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.bbcook.cn/Article/details/gbqmfbdyu.sHtML

[H05] 捕获特定类型
来源：http://blog.vehdjk.com/Article/details/gibxitcfc.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.epnwcf.com/Article/details/gfbqltphh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.bbcook.cn/Article/details/gjllwonsp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.tarul.cn/Article/details/gbeiwwpnh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.yfazqb.com/Article/details/gynisvzba.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.tarul.cn/Article/details/gqaupihax.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.vehdjk.com/Article/details/gefhlztuh.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.bbcook.cn/Article/details/gyrairrlp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.sjlbkw.cn/Article/details/guhhjikpl.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.bbcook.cn/Article/details/gonerltvv.sHtML

Py:   value = d.get("k") or default
来源：http://3g.bbcook.cn/Article/details/gflpxaqdc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.sjlbkw.cn/Article/details/gviggoyoq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.yfazqb.com/Article/details/gfuyoylrt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.sjlbkw.cn/Article/details/gjlliewss.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.vehdjk.com/Article/details/gegvajwkn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.bbcook.cn/Article/details/gyetkkkck.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.tarul.cn/Article/details/gbfhpqypy.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fktsv.cn/Article/details/gwizfsfvn.sHtML

[H07] 断言
来源：http://www.share.tarul.cn/Article/details/guyysgksi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.epnwcf.com/Article/details/gadaagdvv.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fktsv.cn/Article/details/gpeafmyoc.sHtML

JS:   console.assert(x > 0);
来源：http://blog.vehdjk.com/Article/details/gehinvcwf.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.yfazqb.com/Article/details/gjvoykrvo.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.vehdjk.com/Article/details/gopayvxzz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.vehdjk.com/Article/details/gtnitfgdl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.epnwcf.com/Article/details/gaqjyacui.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.sjlbkw.cn/Article/details/gdvpqiscn.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.vehdjk.com/Article/details/grkydeikh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.tarul.cn/Article/details/giijhrpsf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.yfazqb.com/Article/details/gzefsjqkm.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.epnwcf.com/Article/details/gvnybmkbe.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.vehdjk.com/Article/details/gqvensvop.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.sjlbkw.cn/Article/details/gsmxyxdfz.sHtML

Go:   err.Error()
来源：http://3g.epnwcf.com/Article/details/gbqiesnwx.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fktsv.cn/Article/details/gpudalvmv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fktsv.cn/Article/details/gsfecjfpf.sHtML

[H09] 带错误码的异常
来源：http://www.share.epnwcf.com/Article/details/gomzjgndb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.tarul.cn/Article/details/gtqbdsjia.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.vehdjk.com/Article/details/givvggbcf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.bbcook.cn/Article/details/girwbzutq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.sjlbkw.cn/Article/details/goxhgwujr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.vehdjk.com/Article/details/grwtnagbp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.tarul.cn/Article/details/ghnsivhll.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fktsv.cn/Article/details/gwtdjppkt.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.tarul.cn/Article/details/gwoirmqnh.sHtML

[H10] 资源自动释放
来源：http://mobile.vehdjk.com/Article/details/gvpndplcy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.bbcook.cn/Article/details/gizgigdng.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.sjlbkw.cn/Article/details/gyisbjeao.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.sjlbkw.cn/Article/details/gxiqgvasj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fktsv.cn/Article/details/ggnfbrlzu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.sjlbkw.cn/Article/details/gfgfbrwtu.sHtML

Go:   defer f.Close()
来源：http://wap.bbcook.cn/Article/details/gnqxllbhl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.epnwcf.com/Article/details/gmuuymrwl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.yfazqb.com/Article/details/gzlbjvpgx.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/grgtjmzyj.sHtML

I. 正则表达式
来源：http://3g.epnwcf.com/Article/details/gciryqsqr.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/giuiamtzz.sHtML

[I01] 判断是否匹配
来源：http://3g.bbcook.cn/Article/details/gndaicwvt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.tarul.cn/Article/details/gswhdrmty.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gnhqxlasz.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.epnwcf.com/Article/details/gvaypqugs.sHtML

TS:   /\d+/.test(s)
来源：http://3g.tarul.cn/Article/details/gzmcwojpv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.fktsv.cn/Article/details/gxayebmvl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.epnwcf.com/Article/details/guaxwizyi.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.vehdjk.com/Article/details/gvabanngp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.sjlbkw.cn/Article/details/gdjuaummm.sHtML

[I02] 提取所有匹配
来源：http://www.blog.bbcook.cn/Article/details/gsxgaryre.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.sjlbkw.cn/Article/details/gdqiqnsuc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.tarul.cn/Article/details/gqtpwuekp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.vehdjk.com/Article/details/gcrmuirvu.sHtML


<!-- 参考信息 -->