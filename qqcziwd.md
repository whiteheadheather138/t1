代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxmlaqyq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.vehdjk.com/Article/details/gaflizqcc.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/gazaambru.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gyevaftxt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.tarul.cn/Article/details/grypfpbgc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.tarul.cn/Article/details/gfloqsvvo.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/ggndxccbk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.vehdjk.com/Article/details/getnsqgoh.sHtML

[F09] 获取文件大小
来源：http://blog.epnwcf.com/Article/details/gcpbywtje.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gpnblizau.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gdwbnlami.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.epnwcf.com/Article/details/gzdbndubx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.tarul.cn/Article/details/ggukrvqap.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.vehdjk.com/Article/details/gmqihfshg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fktsv.cn/Article/details/ghmpigsfb.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gpjpyitps.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.bbcook.cn/Article/details/gmmimjnku.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.vehdjk.com/Article/details/gvshcofua.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/gzxzuiqvb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gmvguafqh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/gzatnidks.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gckmcaklk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.tarul.cn/Article/details/gzzhlfwyd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gfkhmtoss.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gcztfbuyv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gxouuecac.sHtML

[F11] 复制与移动文件
来源：http://read.share.fktsv.cn/Article/details/genpjivoc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gsicunltd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.tarul.cn/Article/details/ghefpifrl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gzjzncanv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/gjsxcplcv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.yfazqb.com/Article/details/gsomplucc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.epnwcf.com/Article/details/gkwmhouty.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.vehdjk.com/Article/details/grvadgvow.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.sjlbkw.cn/Article/details/gcnqofcgh.sHtML

[F12] CSV 读写
来源：http://3g.tarul.cn/Article/details/gnnreidhs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.epnwcf.com/Article/details/gfisorwzm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.bbcook.cn/Article/details/gmvekaxfo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.yfazqb.com/Article/details/gzupeblrd.sHtML

TS:   // 同上
来源：http://read.share.fktsv.cn/Article/details/gsvghumob.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.vehdjk.com/Article/details/gxhtmdojh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.yfazqb.com/Article/details/gneejyqsb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.tarul.cn/Article/details/goilswapi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.tarul.cn/Article/details/grbncgxwe.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gppbqtkfm.sHtML

G. 面向对象
来源：http://www.blog.yfazqb.com/Article/details/gitwyugyy.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gqnrnehdk.sHtML

[G01] 定义类
来源：http://wap.bbcook.cn/Article/details/gnbeqfwyj.sHtML

Py:   class User: pass
来源：http://www.blog.vehdjk.com/Article/details/gesbpcbbm.sHtML

PHP:  class User {}
来源：http://read.share.vehdjk.com/Article/details/gaxyzwdmn.sHtML

JS:   class User {}
来源：http://blog.tarul.cn/Article/details/gizifnkkx.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fktsv.cn/Article/details/gcgerffxt.sHtML

Java: class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gzcwlxiva.sHtML

Go:   type User struct { Name string }
来源：http://3g.sjlbkw.cn/Article/details/gbcfoyody.sHtML

Ruby: class User; end
来源：http://3g.yfazqb.com/Article/details/gxphfxlwf.sHtML

C#:   class User {}
来源：http://3g.sjlbkw.cn/Article/details/ghadnjbmh.sHtML

[G02] 构造函数
来源：http://www.share.epnwcf.com/Article/details/gokzzrvpa.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.vehdjk.com/Article/details/gjeksphio.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.vehdjk.com/Article/details/gnottzyjn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.epnwcf.com/Article/details/gsedshsgz.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.tarul.cn/Article/details/gggmywopj.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.tarul.cn/Article/details/gtovqqbnn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fktsv.cn/Article/details/giijoznxw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.vehdjk.com/Article/details/gqkgevfnt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.epnwcf.com/Article/details/grykigvyo.sHtML

[G03] 实例属性
来源：http://www.blog.bbcook.cn/Article/details/gsriloyhi.sHtML

Py:   self.name = "x"
来源：http://wap.vehdjk.com/Article/details/gvgbjguof.sHtML

PHP:  public string $name = "x";
来源：http://blog.tarul.cn/Article/details/gdfwufasr.sHtML

JS:   this.name = "x";
来源：http://mobile.bbcook.cn/Article/details/gawadadzn.sHtML

TS:   name: string = "x";
来源：http://mobile.bbcook.cn/Article/details/gqrcebhfk.sHtML

Java: private String name;
来源：http://baike.bbcook.cn/Article/details/gjlenxgxt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.yfazqb.com/Article/details/gpxvbplqk.sHtML

Ruby: @name = "x"
来源：http://www.blog.yfazqb.com/Article/details/gjuasyjcg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.vehdjk.com/Article/details/glwxemeas.sHtML

[G04] 定义方法
来源：http://m.share.vehdjk.com/Article/details/gkneravgt.sHtML

Py:   def greet(self): return self.name
来源：http://wap.yfazqb.com/Article/details/gqlfwawwv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.vehdjk.com/Article/details/gpbzvgawy.sHtML

JS:   greet() { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gmscpower.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/gtajfymrp.sHtML

Java: String greet() { return name; }
来源：http://3g.yfazqb.com/Article/details/gmcsjtppk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.yfazqb.com/Article/details/gszsgzjnn.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.tarul.cn/Article/details/gwkqezsvb.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.bbcook.cn/Article/details/gkikfcvjf.sHtML

[G05] 继承
来源：http://read.share.sjlbkw.cn/Article/details/gyjucwfvu.sHtML

Py:   class Admin(User): pass
来源：http://mobile.vehdjk.com/Article/details/gmwimmxma.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/gszzkdjkz.sHtML

JS:   class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/gnyycipgl.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gfzghutbr.sHtML

Java: class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/gerxkxlsx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.tarul.cn/Article/details/gfkgpfrce.sHtML

Ruby: class Admin < User; end
来源：http://baike.tarul.cn/Article/details/gyswbjkew.sHtML

C#:   class Admin : User {}
来源：http://blog.fktsv.cn/Article/details/gpkkzjgfj.sHtML

[G06] 重写方法
来源：http://www.share.sjlbkw.cn/Article/details/gjkmnocys.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.vehdjk.com/Article/details/gwcwhdssb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/gfcraldsb.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/gzqiqseui.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.tarul.cn/Article/details/gyinrwchy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/ghsmhdzbh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.yfazqb.com/Article/details/gpvielpry.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.bbcook.cn/Article/details/glqjveptb.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fktsv.cn/Article/details/gwaixxiiw.sHtML

[G07] 调用父类方法
来源：http://m.share.yfazqb.com/Article/details/gksbaskhj.sHtML

Py:   super().greet()
来源：http://www.share.vehdjk.com/Article/details/gsipvntat.sHtML

PHP:  parent::greet();
来源：http://read.share.tarul.cn/Article/details/gekszvatz.sHtML

JS:   super.greet();
来源：http://www.share.tarul.cn/Article/details/gnefsgigp.sHtML

TS:   super.greet();
来源：http://wap.yfazqb.com/Article/details/guyfyvqgn.sHtML

Java: super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbnxqtmp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.yfazqb.com/Article/details/gglxslemz.sHtML

Ruby: super
来源：http://mobile.sjlbkw.cn/Article/details/ggkalrucg.sHtML

C#:   base.Greet();
来源：http://blog.fktsv.cn/Article/details/gdappfksn.sHtML

[G08] 静态方法与属性
来源：http://www.blog.vehdjk.com/Article/details/gqveircyi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fktsv.cn/Article/details/gkbfrqhuh.sHtML

PHP:  public static function f() {}
来源：http://baike.epnwcf.com/Article/details/ggpsaoill.sHtML

JS:   static f() {}
来源：http://m.share.sjlbkw.cn/Article/details/ggioscltk.sHtML

TS:   static f(): void {}
来源：http://baike.yfazqb.com/Article/details/gfdmpcsmr.sHtML

Java: static void f() {}
来源：http://www.blog.vehdjk.com/Article/details/gzojcaedq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.sjlbkw.cn/Article/details/gsqaxrbiv.sHtML

Ruby: def self.f; end
来源：http://www.blog.sjlbkw.cn/Article/details/gixndizfi.sHtML

C#:   public static void F() {}
来源：http://baike.vehdjk.com/Article/details/ghuzopmbs.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.vehdjk.com/Article/details/gpuryjwrl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.sjlbkw.cn/Article/details/gxexxmxls.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.sjlbkw.cn/Article/details/gslffihlh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.vehdjk.com/Article/details/gqgiygchw.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.sjlbkw.cn/Article/details/gfqiwhezl.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fktsv.cn/Article/details/gwmlewjaf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.bbcook.cn/Article/details/gbnvqufre.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.yfazqb.com/Article/details/gkororzgb.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.yfazqb.com/Article/details/gfrzyfvcv.sHtML

[G10] 访问控制
来源：http://mobile.epnwcf.com/Article/details/gxcxvihlf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fktsv.cn/Article/details/gzpniqxhd.sHtML

PHP:  public / protected / private
来源：http://wap.vehdjk.com/Article/details/gtbjflout.sHtML

JS:   #private 字段；其余公开
来源：http://3g.sjlbkw.cn/Article/details/gjlqmtixd.sHtML

TS:   public / protected / private
来源：http://mobile.vehdjk.com/Article/details/gnrvbtkmx.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.bbcook.cn/Article/details/gdefpgirx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.epnwcf.com/Article/details/gdstvukmb.sHtML

Ruby: public / protected / private
来源：http://www.share.epnwcf.com/Article/details/gjsjczkat.sHtML

C#:   public / protected / private / internal
来源：http://wap.epnwcf.com/Article/details/gvctjgupa.sHtML

[G11] getter / setter
来源：http://read.share.vehdjk.com/Article/details/gwuhrdajz.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fktsv.cn/Article/details/gksphfrcm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fktsv.cn/Article/details/gxmtnmyrd.sHtML

JS:   get name() { return this._name; }
来源：http://3g.tarul.cn/Article/details/ghmjnpfds.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.epnwcf.com/Article/details/gnpvvnooc.sHtML

Java: public String getName() { return name; }
来源：http://www.share.bbcook.cn/Article/details/glfnvzfnp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.yfazqb.com/Article/details/gjypzyons.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.bbcook.cn/Article/details/gdqqktwgs.sHtML

C#:   public string Name { get; set; }
来源：http://wap.bbcook.cn/Article/details/gawyxmcop.sHtML

[G12] 对象转字符串
来源：http://blog.yfazqb.com/Article/details/gwhmmypbk.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.tarul.cn/Article/details/gljfalgxi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.vehdjk.com/Article/details/gechawgeb.sHtML

JS:   toString() { return this.name; }
来源：http://blog.tarul.cn/Article/details/ghdfllskw.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/ghdlsqgsv.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/gfwqeirox.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.epnwcf.com/Article/details/ggjtxciwu.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.yfazqb.com/Article/details/gvwkreiwy.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fktsv.cn/Article/details/gtqvvqacv.sHtML

[G13] 判断对象类型
来源：http://baike.fktsv.cn/Article/details/gsoiiyclt.sHtML

Py:   isinstance(u, User)
来源：http://baike.vehdjk.com/Article/details/gxdcbvtxf.sHtML

PHP:  $u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/geebedatr.sHtML

JS:   u instanceof User
来源：http://3g.bbcook.cn/Article/details/ggihmxoys.sHtML

TS:   u instanceof User
来源：http://www.share.bbcook.cn/Article/details/gxqypmuxp.sHtML

Java: u instanceof User
来源：http://3g.fktsv.cn/Article/details/glellnyum.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.sjlbkw.cn/Article/details/gptwmxsdn.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.tarul.cn/Article/details/guwoqbhkw.sHtML

C#:   u is User
来源：http://m.share.sjlbkw.cn/Article/details/gazognsbt.sHtML

[G14] 数据类 / record
来源：http://wap.vehdjk.com/Article/details/gkgctbxli.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.tarul.cn/Article/details/ggvfdfypa.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.tarul.cn/Article/details/gqlueqznq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fktsv.cn/Article/details/geosqkynq.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fktsv.cn/Article/details/gpntlidon.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.bbcook.cn/Article/details/gnalkxamu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fktsv.cn/Article/details/gytpthham.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.yfazqb.com/Article/details/gonasnkpl.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fktsv.cn/Article/details/grchtchbb.sHtML

[G15] 枚举
来源：http://m.share.yfazqb.com/Article/details/gwxfeiiio.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.epnwcf.com/Article/details/gdgnfoqrx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.yfazqb.com/Article/details/gjvgmlqhc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.tarul.cn/Article/details/gdeogvnms.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.vehdjk.com/Article/details/gxbityzso.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.vehdjk.com/Article/details/gkqhhckgg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.epnwcf.com/Article/details/gfancqktv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.vehdjk.com/Article/details/gsmgdjjbu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.yfazqb.com/Article/details/gyiebsmyn.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.vehdjk.com/Article/details/gsjhyjbra.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.tarul.cn/Article/details/ggdwhpduu.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.vehdjk.com/Article/details/giicamzab.sHtML

JS:   Object.entries(obj)
来源：http://3g.epnwcf.com/Article/details/gridztejc.sHtML

TS:   Object.entries(obj)
来源：http://www.share.yfazqb.com/Article/details/gtbkcvcfr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.sjlbkw.cn/Article/details/gzffwawbk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.tarul.cn/Article/details/gqktgwkmm.sHtML

Ruby: obj.instance_variables
来源：http://www.share.epnwcf.com/Article/details/gcnzoqbln.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.epnwcf.com/Article/details/gimiegyel.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gzyvsoxjp.sHtML

H. 异常与错误处理
来源：http://www.share.vehdjk.com/Article/details/gbhjoamyp.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gyewfvmyh.sHtML

[H01] try / catch 基础
来源：http://www.share.yfazqb.com/Article/details/gcxrjdavz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.sjlbkw.cn/Article/details/gnlyexcdf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gpvbofizo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.yfazqb.com/Article/details/gwdaayobg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.epnwcf.com/Article/details/grvkixtaz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.bbcook.cn/Article/details/gkqyintce.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.yfazqb.com/Article/details/gnwydyouw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.yfazqb.com/Article/details/goebishjy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.epnwcf.com/Article/details/gonhzfozf.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.epnwcf.com/Article/details/gnfydfqgl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.yfazqb.com/Article/details/gvmcnyzug.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gpnfzeaob.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gwenjzrlv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/gappommao.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/goydvgkgi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.sjlbkw.cn/Article/details/gfkkzrsun.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.tarul.cn/Article/details/goowfucuj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gfgauqfzs.sHtML

[H03] 主动抛出异常
来源：http://www.blog.tarul.cn/Article/details/gamtfrbww.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.bbcook.cn/Article/details/gsxgdihan.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fktsv.cn/Article/details/ghhdabohu.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.bbcook.cn/Article/details/ggjcjrxeh.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gsmuzhliz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gadcdglkv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fktsv.cn/Article/details/gtsrcfbut.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.epnwcf.com/Article/details/gulvkkatb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.yfazqb.com/Article/details/gvhtrabpv.sHtML

[H04] 自定义异常类型
来源：http://mobile.epnwcf.com/Article/details/ghgeaieaf.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.tarul.cn/Article/details/glgtozevf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.yfazqb.com/Article/details/gntlaoxkf.sHtML

JS:   class MyError extends Error {}
来源：http://3g.epnwcf.com/Article/details/gupmzlugm.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.bbcook.cn/Article/details/ghdrhxdse.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.sjlbkw.cn/Article/details/gkwvunefy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.epnwcf.com/Article/details/gdyjpcnvl.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.yfazqb.com/Article/details/gosxqjzhu.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.yfazqb.com/Article/details/gqlzzvmrn.sHtML

[H05] 捕获特定类型
来源：http://m.share.bbcook.cn/Article/details/gddsvpxle.sHtML

Py:   except ValueError as e:
来源：http://read.share.vehdjk.com/Article/details/gdlwniiab.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.sjlbkw.cn/Article/details/gumuurzhy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.vehdjk.com/Article/details/gcscxpgbt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.vehdjk.com/Article/details/glnbyvaui.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.bbcook.cn/Article/details/gvhcazyzf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.tarul.cn/Article/details/gwvirjprm.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fktsv.cn/Article/details/gvewfzaze.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.sjlbkw.cn/Article/details/gptmkgcdu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.sjlbkw.cn/Article/details/gkkwlscac.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.yfazqb.com/Article/details/grswjcwev.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.vehdjk.com/Article/details/gqotnoqck.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.bbcook.cn/Article/details/gqoziayxw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.sjlbkw.cn/Article/details/gnumbvojt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.epnwcf.com/Article/details/gcsphmequ.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.bbcook.cn/Article/details/gbbfyttxw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.tarul.cn/Article/details/gdmlmlbeg.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fktsv.cn/Article/details/gyotjpspg.sHtML

[H07] 断言
来源：http://www.blog.vehdjk.com/Article/details/gsqwkzidv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.epnwcf.com/Article/details/ginslajnm.sHtML

PHP:  assert($x > 0);
来源：http://blog.vehdjk.com/Article/details/gxqyunhkn.sHtML

JS:   console.assert(x > 0);
来源：http://baike.sjlbkw.cn/Article/details/gxbqlyxtv.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fktsv.cn/Article/details/gspjilpih.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.bbcook.cn/Article/details/gjxpwjqdk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.tarul.cn/Article/details/grfmcwsru.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.sjlbkw.cn/Article/details/ggtysnkhx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.sjlbkw.cn/Article/details/gkqbeomok.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.vehdjk.com/Article/details/gtvcnzugd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.tarul.cn/Article/details/gctygtvpb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.epnwcf.com/Article/details/gyusrtqoq.sHtML

JS:   e.message;  e.stack
来源：http://mobile.vehdjk.com/Article/details/gqgtjbuma.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.epnwcf.com/Article/details/gsthtlahi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.bbcook.cn/Article/details/gizkeamyr.sHtML

Go:   err.Error()
来源：http://www.share.vehdjk.com/Article/details/gwnlgxyzy.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.vehdjk.com/Article/details/gxhcaypty.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fktsv.cn/Article/details/gawtyiyad.sHtML

[H09] 带错误码的异常
来源：http://blog.yfazqb.com/Article/details/gywyrcldm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.vehdjk.com/Article/details/ggpxzogpz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.tarul.cn/Article/details/ghwzpemnr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.sjlbkw.cn/Article/details/gvluggyfk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbfoeonx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fktsv.cn/Article/details/gbpmyjxof.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.vehdjk.com/Article/details/gotnjtqfa.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.tarul.cn/Article/details/gbmlexraa.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.sjlbkw.cn/Article/details/grbshlxmx.sHtML

[H10] 资源自动释放
来源：http://mobile.vehdjk.com/Article/details/gvziyddvk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.yfazqb.com/Article/details/gwqfhocpe.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.vehdjk.com/Article/details/grplwllko.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.epnwcf.com/Article/details/gavopuuiu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.vehdjk.com/Article/details/ggfnbnssv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fktsv.cn/Article/details/gxegsymyg.sHtML

Go:   defer f.Close()
来源：http://www.blog.fktsv.cn/Article/details/gayezqnyf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.bbcook.cn/Article/details/gkssfmpbc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gefcfxanh.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gbkmqnyok.sHtML

I. 正则表达式
来源：http://mobile.yfazqb.com/Article/details/gudzhcanc.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gpagjynym.sHtML

[I01] 判断是否匹配
来源：http://3g.vehdjk.com/Article/details/gfmkbfvsy.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.tarul.cn/Article/details/ghswodxzo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.bbcook.cn/Article/details/gcbtqyrxy.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.epnwcf.com/Article/details/gifpalerd.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.yfazqb.com/Article/details/gnjpgbzyb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.vehdjk.com/Article/details/gusxpibwb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fktsv.cn/Article/details/ghegqlbjo.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.vehdjk.com/Article/details/gyfbfxgyb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.sjlbkw.cn/Article/details/gctyygsun.sHtML

[I02] 提取所有匹配
来源：http://www.share.yfazqb.com/Article/details/gwwfpdmpn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.tarul.cn/Article/details/gfhilfzxy.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.vehdjk.com/Article/details/gbwadjgxt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.fktsv.cn/Article/details/gfyxebqby.sHtML


<!-- 参考信息 -->