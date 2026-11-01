代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/gaxybijej.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/gssuhhgfi.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/gnyuenxiy.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gjolptvhi.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.tarul.cn/Article/details/gdkivbzrw.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gadjgydkf.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.sjlbkw.cn/Article/details/geqtwrboa.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.sjlbkw.cn/Article/details/gveukadwp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fktsv.cn/Article/details/gyodalwlu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.sjlbkw.cn/Article/details/goyhiegco.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.epnwcf.com/Article/details/gjzmejagg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.bbcook.cn/Article/details/gwbggqyfd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.epnwcf.com/Article/details/gehckqwvt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.yfazqb.com/Article/details/gncsoabdu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.vehdjk.com/Article/details/gwvqvfhhd.sHtML

[F08] 遍历目录
来源：http://m.share.sjlbkw.cn/Article/details/gcltkzauj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.bbcook.cn/Article/details/gnqxamuuo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.bbcook.cn/Article/details/ghoaliqdv.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fktsv.cn/Article/details/gdaqeztnc.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.sjlbkw.cn/Article/details/gndlxebzk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.vehdjk.com/Article/details/geiebxfdf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.epnwcf.com/Article/details/gdcwuavob.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fktsv.cn/Article/details/gnpodebng.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.yfazqb.com/Article/details/gynuxuslx.sHtML

[F09] 获取文件大小
来源：http://baike.tarul.cn/Article/details/gvnwjjcnu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.bbcook.cn/Article/details/gwnbkesgy.sHtML

PHP:  filesize("a.txt");
来源：http://blog.bbcook.cn/Article/details/gyziprbtn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.epnwcf.com/Article/details/gdwetykpy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.bbcook.cn/Article/details/gbnjpjdzh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/gacsfodru.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.tarul.cn/Article/details/grqzwnohx.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gzfgetzcd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.vehdjk.com/Article/details/guomnluwb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.tarul.cn/Article/details/grzxjmuiz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gosfjksjj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.epnwcf.com/Article/details/gtfzmabja.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gslfwqwet.sHtML

TS:   path.extname("a.txt")
来源：http://baike.vehdjk.com/Article/details/gsecfugne.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.vehdjk.com/Article/details/ggnpmabcu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gzmdujkfm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.tarul.cn/Article/details/gvxidimxf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/gorlguvxp.sHtML

[F11] 复制与移动文件
来源：http://wap.epnwcf.com/Article/details/gkzjifmbb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gafsrtbki.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gdmgzyojv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fktsv.cn/Article/details/geayooczh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/gtqyospik.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.yfazqb.com/Article/details/gibwqnpsq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fktsv.cn/Article/details/gnxzmqcvg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/gdrnaiomz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.tarul.cn/Article/details/gfdqpgiie.sHtML

[F12] CSV 读写
来源：http://wap.fktsv.cn/Article/details/glwradhqw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fktsv.cn/Article/details/gjcgpgepa.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fktsv.cn/Article/details/gbdvotdxb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.bbcook.cn/Article/details/grhuyettc.sHtML

TS:   // 同上
来源：http://wap.vehdjk.com/Article/details/gticunwkk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fktsv.cn/Article/details/grsocsfku.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.yfazqb.com/Article/details/gslcejopa.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fktsv.cn/Article/details/gkyevjipd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.vehdjk.com/Article/details/gnwjyhwmj.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gibrpclyv.sHtML

G. 面向对象
来源：http://baike.epnwcf.com/Article/details/gotvhkrui.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gmngnwwdm.sHtML

[G01] 定义类
来源：http://read.share.sjlbkw.cn/Article/details/gmtclztqz.sHtML

Py:   class User: pass
来源：http://blog.vehdjk.com/Article/details/gaxhfrvhl.sHtML

PHP:  class User {}
来源：http://www.m.share.bbcook.cn/Article/details/gbifzbfxh.sHtML

JS:   class User {}
来源：http://baike.sjlbkw.cn/Article/details/goxpnujkx.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.epnwcf.com/Article/details/goxvdtyua.sHtML

Java: class User {}
来源：http://baike.vehdjk.com/Article/details/gzvgtwgmg.sHtML

Go:   type User struct { Name string }
来源：http://www.share.tarul.cn/Article/details/gcxuqjoqa.sHtML

Ruby: class User; end
来源：http://read.share.sjlbkw.cn/Article/details/gfuhbequa.sHtML

C#:   class User {}
来源：http://www.m.share.yfazqb.com/Article/details/geuiifuod.sHtML

[G02] 构造函数
来源：http://mobile.fktsv.cn/Article/details/gxbfdppxb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.yfazqb.com/Article/details/gejwzbzrd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.tarul.cn/Article/details/gbfynswyt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.tarul.cn/Article/details/gsyipuspr.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.yfazqb.com/Article/details/glajtwjzn.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fktsv.cn/Article/details/gvwgordfw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.sjlbkw.cn/Article/details/gisvvhqlr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.tarul.cn/Article/details/gujdpgqsm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.epnwcf.com/Article/details/gbklycczr.sHtML

[G03] 实例属性
来源：http://m.share.yfazqb.com/Article/details/gmfdcizuo.sHtML

Py:   self.name = "x"
来源：http://3g.epnwcf.com/Article/details/gecaenisk.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.bbcook.cn/Article/details/gooflvqtx.sHtML

JS:   this.name = "x";
来源：http://blog.bbcook.cn/Article/details/gjetqfnvq.sHtML

TS:   name: string = "x";
来源：http://www.share.vehdjk.com/Article/details/gulrexxdp.sHtML

Java: private String name;
来源：http://read.share.vehdjk.com/Article/details/gxxalpaje.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.epnwcf.com/Article/details/ggqznmoxr.sHtML

Ruby: @name = "x"
来源：http://wap.fktsv.cn/Article/details/gimyoeijo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.yfazqb.com/Article/details/gkaojmrbu.sHtML

[G04] 定义方法
来源：http://read.share.sjlbkw.cn/Article/details/glvmybkom.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.sjlbkw.cn/Article/details/gbflxhdam.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.epnwcf.com/Article/details/gdgrinkwd.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gxrhmpopq.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.bbcook.cn/Article/details/gdyefxjwk.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/gmhkrcxwg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.tarul.cn/Article/details/gbyezvgeo.sHtML

Ruby: def greet; @name; end
来源：http://baike.tarul.cn/Article/details/gdcjwazfh.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.yfazqb.com/Article/details/gcznxievs.sHtML

[G05] 继承
来源：http://3g.yfazqb.com/Article/details/gbrnhrigy.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.vehdjk.com/Article/details/gabwakxhs.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gvlzdfjje.sHtML

JS:   class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gocrhymlo.sHtML

TS:   class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/giwktlmnx.sHtML

Java: class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/gmcbkurmt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.epnwcf.com/Article/details/gwptathxb.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.yfazqb.com/Article/details/grmdutbvm.sHtML

C#:   class Admin : User {}
来源：http://wap.vehdjk.com/Article/details/gztlqfnek.sHtML

[G06] 重写方法
来源：http://www.m.share.tarul.cn/Article/details/gclcrcsos.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fktsv.cn/Article/details/gymexncma.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gdypkzidq.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/ggggswxqh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/goaxamqss.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gpxlvfszd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.sjlbkw.cn/Article/details/gljyavifu.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.sjlbkw.cn/Article/details/gcylcfsln.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.bbcook.cn/Article/details/gvuudmhqy.sHtML

[G07] 调用父类方法
来源：http://www.blog.fktsv.cn/Article/details/grfgfbepl.sHtML

Py:   super().greet()
来源：http://blog.epnwcf.com/Article/details/gjmlzbjsw.sHtML

PHP:  parent::greet();
来源：http://read.share.bbcook.cn/Article/details/ggyzfbham.sHtML

JS:   super.greet();
来源：http://read.share.fktsv.cn/Article/details/grfmmeefg.sHtML

TS:   super.greet();
来源：http://www.m.share.fktsv.cn/Article/details/gltvjjhgp.sHtML

Java: super.greet();
来源：http://mobile.tarul.cn/Article/details/gnwykkijf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.sjlbkw.cn/Article/details/gkwypcmmx.sHtML

Ruby: super
来源：http://3g.vehdjk.com/Article/details/gvgkhmbds.sHtML

C#:   base.Greet();
来源：http://read.share.bbcook.cn/Article/details/gjhwcukdc.sHtML

[G08] 静态方法与属性
来源：http://m.share.yfazqb.com/Article/details/gpepllmus.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.sjlbkw.cn/Article/details/gslyfptbp.sHtML

PHP:  public static function f() {}
来源：http://baike.vehdjk.com/Article/details/gktdjbxzk.sHtML

JS:   static f() {}
来源：http://blog.epnwcf.com/Article/details/ghojhbcnv.sHtML

TS:   static f(): void {}
来源：http://www.blog.vehdjk.com/Article/details/ghlzepvqa.sHtML

Java: static void f() {}
来源：http://read.share.bbcook.cn/Article/details/gdiwxzmhf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.yfazqb.com/Article/details/gkmqqblpu.sHtML

Ruby: def self.f; end
来源：http://baike.bbcook.cn/Article/details/glqztgefb.sHtML

C#:   public static void F() {}
来源：http://www.share.vehdjk.com/Article/details/gjqjzlnbl.sHtML

[G09] 接口 / 抽象类
来源：http://wap.sjlbkw.cn/Article/details/gjldeuohy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.epnwcf.com/Article/details/gznvufqwh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.sjlbkw.cn/Article/details/glqlftxmh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.sjlbkw.cn/Article/details/ghstunwre.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.epnwcf.com/Article/details/gwiqgvlnm.sHtML

Java: interface Shape { double area(); }
来源：http://baike.epnwcf.com/Article/details/gxukdxbhd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.tarul.cn/Article/details/gwkkqjkjf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.vehdjk.com/Article/details/gydzyjzzi.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.tarul.cn/Article/details/geqsfjfxh.sHtML

[G10] 访问控制
来源：http://www.share.bbcook.cn/Article/details/goiqxwiqd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.yfazqb.com/Article/details/gnkuwwplr.sHtML

PHP:  public / protected / private
来源：http://read.share.epnwcf.com/Article/details/gcbvoylcl.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.epnwcf.com/Article/details/gnhgrskxs.sHtML

TS:   public / protected / private
来源：http://3g.yfazqb.com/Article/details/gtafupgxk.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.epnwcf.com/Article/details/gasncmfwz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.tarul.cn/Article/details/gftmekmwi.sHtML

Ruby: public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gwrgksnvu.sHtML

C#:   public / protected / private / internal
来源：http://mobile.vehdjk.com/Article/details/gudqmcjgj.sHtML

[G11] getter / setter
来源：http://baike.tarul.cn/Article/details/grxczvjon.sHtML

Py:   @property 与 @x.setter
来源：http://3g.bbcook.cn/Article/details/gtyqhqoqh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/ghvncslcd.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.vehdjk.com/Article/details/gwvxlcozb.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.vehdjk.com/Article/details/gaitujpjq.sHtML

Java: public String getName() { return name; }
来源：http://wap.vehdjk.com/Article/details/gsypbvmrh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.yfazqb.com/Article/details/gsatqksyq.sHtML

Ruby: attr_accessor :name
来源：http://www.share.sjlbkw.cn/Article/details/glvuiwoqm.sHtML

C#:   public string Name { get; set; }
来源：http://wap.yfazqb.com/Article/details/guahtpaan.sHtML

[G12] 对象转字符串
来源：http://m.share.yfazqb.com/Article/details/gvhsgbehz.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fktsv.cn/Article/details/gwnbopfnm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fktsv.cn/Article/details/gxfbnxlkp.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/gvhssxezf.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.vehdjk.com/Article/details/gmehmhana.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.vehdjk.com/Article/details/gewodvrul.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fktsv.cn/Article/details/gcipxcfbb.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.vehdjk.com/Article/details/gpmpkrivz.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.sjlbkw.cn/Article/details/gydggoxlk.sHtML

[G13] 判断对象类型
来源：http://m.share.fktsv.cn/Article/details/gzbjulcod.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.vehdjk.com/Article/details/gewtdiljy.sHtML

PHP:  $u instanceof User
来源：http://mobile.fktsv.cn/Article/details/ggenjwrrt.sHtML

JS:   u instanceof User
来源：http://m.share.sjlbkw.cn/Article/details/gnjbxaxwa.sHtML

TS:   u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/ghkbszbiq.sHtML

Java: u instanceof User
来源：http://3g.epnwcf.com/Article/details/gkvsovhnq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.bbcook.cn/Article/details/gmdkofjoe.sHtML

Ruby: u.is_a?(User)
来源：http://baike.tarul.cn/Article/details/gfxlhctri.sHtML

C#:   u is User
来源：http://www.m.share.sjlbkw.cn/Article/details/ggudicwwx.sHtML

[G14] 数据类 / record
来源：http://mobile.fktsv.cn/Article/details/ghpjmluur.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.bbcook.cn/Article/details/gqwxlbamb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.vehdjk.com/Article/details/gbkibfnlq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.bbcook.cn/Article/details/gqhhmzade.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.yfazqb.com/Article/details/gksichovq.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.vehdjk.com/Article/details/gtfmgkedt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.yfazqb.com/Article/details/gpifwwayj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.sjlbkw.cn/Article/details/grhomtzit.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fktsv.cn/Article/details/gofmehsey.sHtML

[G15] 枚举
来源：http://baike.sjlbkw.cn/Article/details/grvfnlbbb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.yfazqb.com/Article/details/gvxjxqpfk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.epnwcf.com/Article/details/gnnblgxrn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.epnwcf.com/Article/details/glfzwkxqw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.tarul.cn/Article/details/graulxhwo.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.vehdjk.com/Article/details/gfnonajde.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.sjlbkw.cn/Article/details/gmmfeuomu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.sjlbkw.cn/Article/details/gxfkwgdia.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fktsv.cn/Article/details/gdzctxnwx.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.yfazqb.com/Article/details/gauhofrfq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.epnwcf.com/Article/details/gjmbizosk.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.vehdjk.com/Article/details/glxteteyo.sHtML

JS:   Object.entries(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gveqkkqvg.sHtML

TS:   Object.entries(obj)
来源：http://m.share.bbcook.cn/Article/details/gsvvqtztm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.tarul.cn/Article/details/gyafpwtxx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.sjlbkw.cn/Article/details/gfuahyhpm.sHtML

Ruby: obj.instance_variables
来源：http://m.share.yfazqb.com/Article/details/gajohdqzd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.vehdjk.com/Article/details/gncfvxzyn.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/godfwdooz.sHtML

H. 异常与错误处理
来源：http://mobile.yfazqb.com/Article/details/gaumfibfc.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gkzwchwgb.sHtML

[H01] try / catch 基础
来源：http://wap.vehdjk.com/Article/details/gsjuibiwv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fktsv.cn/Article/details/gaemcahti.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gonfzdovu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.yfazqb.com/Article/details/gtjnbgsjw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.bbcook.cn/Article/details/gowayuyal.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.tarul.cn/Article/details/gcwshpvio.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.epnwcf.com/Article/details/gdbfjcxjz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.vehdjk.com/Article/details/gpnhqdtsx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fktsv.cn/Article/details/gwokqvvwq.sHtML

[H02] finally / ensure 收尾
来源：http://wap.sjlbkw.cn/Article/details/gygihujly.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.yfazqb.com/Article/details/gccfvditk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/gsxdxszvy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.yfazqb.com/Article/details/ghqooxker.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/ghiiqdtzg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.epnwcf.com/Article/details/guvmfkwyd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.bbcook.cn/Article/details/glvjjhjgn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.tarul.cn/Article/details/gwzrnpdwn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.tarul.cn/Article/details/ggfhntfjy.sHtML

[H03] 主动抛出异常
来源：http://wap.yfazqb.com/Article/details/gmwrqnrvt.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.tarul.cn/Article/details/gymnrbtzv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.bbcook.cn/Article/details/grjofjayi.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/grzxsjjmo.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/guksfbtgx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.bbcook.cn/Article/details/gvmjbwewr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.yfazqb.com/Article/details/grlwgcpxx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.vehdjk.com/Article/details/gtnosugod.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/gebcwyvlz.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fktsv.cn/Article/details/gevvcqyrt.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fktsv.cn/Article/details/gpjmmqtuh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.bbcook.cn/Article/details/giimbepjv.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.bbcook.cn/Article/details/gplzegzkd.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.epnwcf.com/Article/details/gyjopqawk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.sjlbkw.cn/Article/details/ggqrvtovr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fktsv.cn/Article/details/gvindocoq.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.bbcook.cn/Article/details/gzfguhnzs.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.sjlbkw.cn/Article/details/gieexazoi.sHtML

[H05] 捕获特定类型
来源：http://www.share.fktsv.cn/Article/details/gtcpvtcnn.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdmtjtwt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.sjlbkw.cn/Article/details/gktycvxjw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.yfazqb.com/Article/details/gvsdpiexj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.sjlbkw.cn/Article/details/ggogarxad.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fktsv.cn/Article/details/gvlfdwtgv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.vehdjk.com/Article/details/gunubzfep.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.bbcook.cn/Article/details/gryqeozhf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.tarul.cn/Article/details/grdvdkfhe.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fktsv.cn/Article/details/gnvxkmsuc.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fktsv.cn/Article/details/gbwrownth.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fktsv.cn/Article/details/gdwrnhqxp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fktsv.cn/Article/details/gxmljttjq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.sjlbkw.cn/Article/details/gaebvbrpp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.vehdjk.com/Article/details/gvfzqitwp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.bbcook.cn/Article/details/gevhqbisx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fktsv.cn/Article/details/gbknqtuuq.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.vehdjk.com/Article/details/gpzydtvff.sHtML

[H07] 断言
来源：http://3g.epnwcf.com/Article/details/gtnxgedfh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.tarul.cn/Article/details/gtfzhvaxm.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.bbcook.cn/Article/details/gbxztsckq.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fktsv.cn/Article/details/gbexsedkt.sHtML

TS:   console.assert(x > 0);
来源：http://blog.vehdjk.com/Article/details/gdlieegmk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.yfazqb.com/Article/details/gmbpqtlkj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.sjlbkw.cn/Article/details/gzzbhdgzz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fktsv.cn/Article/details/gneqwolqv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fktsv.cn/Article/details/gigfkslvz.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.epnwcf.com/Article/details/gykptedsc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.tarul.cn/Article/details/gqbnyzods.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fktsv.cn/Article/details/gejzlgsxl.sHtML

JS:   e.message;  e.stack
来源：http://mobile.epnwcf.com/Article/details/gzdzhoqzn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.epnwcf.com/Article/details/ggmwsghwn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.sjlbkw.cn/Article/details/gngrbervq.sHtML

Go:   err.Error()
来源：http://m.share.fktsv.cn/Article/details/gieicqizq.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.bbcook.cn/Article/details/gmfjanaec.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.bbcook.cn/Article/details/gxamyskrd.sHtML

[H09] 带错误码的异常
来源：http://3g.fktsv.cn/Article/details/gcigmcdnt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.sjlbkw.cn/Article/details/gbiaqpxio.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fktsv.cn/Article/details/gjdotupdq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fktsv.cn/Article/details/gjxfmofdn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.vehdjk.com/Article/details/gztbernwd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fktsv.cn/Article/details/gufxumzyg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.tarul.cn/Article/details/gcsuakbzs.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.epnwcf.com/Article/details/gswtvsifc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.sjlbkw.cn/Article/details/gwgnootis.sHtML

[H10] 资源自动释放
来源：http://m.share.vehdjk.com/Article/details/gfpzifcuu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.yfazqb.com/Article/details/gkexqlrgi.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.yfazqb.com/Article/details/gevciaytq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.tarul.cn/Article/details/gonwfdjmb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.yfazqb.com/Article/details/glpcglbzw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.tarul.cn/Article/details/gjeguccye.sHtML

Go:   defer f.Close()
来源：http://mobile.epnwcf.com/Article/details/geacptzzq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.yfazqb.com/Article/details/gkjckkuct.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.yfazqb.com/Article/details/glkqgcpvr.sHtML


<!-- 参考信息 -->