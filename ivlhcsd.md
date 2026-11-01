代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.epnwcf.com/Article/details/gpyoxkjbk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.tarul.cn/Article/details/gojkefgbr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.bbcook.cn/Article/details/ggrpfyuzx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.tarul.cn/Article/details/gjhwnkyuo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.tarul.cn/Article/details/gapunnrvs.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.sjlbkw.cn/Article/details/gbepknnbr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.tarul.cn/Article/details/gdgpaouif.sHtML

[F08] 遍历目录
来源：http://www.m.share.fktsv.cn/Article/details/gbfqzdpza.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fktsv.cn/Article/details/gbzoduxdd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fktsv.cn/Article/details/gizmyobkk.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.bbcook.cn/Article/details/ggahjksrr.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.epnwcf.com/Article/details/gjskfqfue.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.yfazqb.com/Article/details/giwrkkgtb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.sjlbkw.cn/Article/details/ghqgkdmub.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.yfazqb.com/Article/details/gdwtwuwcp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fktsv.cn/Article/details/gwguhwugc.sHtML

[F09] 获取文件大小
来源：http://blog.vehdjk.com/Article/details/gkdqcwkce.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.yfazqb.com/Article/details/grnpqetxt.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gxregczxm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.epnwcf.com/Article/details/gjslqjegg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fktsv.cn/Article/details/gcehvgdxv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.yfazqb.com/Article/details/gogubakzc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fktsv.cn/Article/details/gregycgxg.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gtbxgfihm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.bbcook.cn/Article/details/ghxpbihtr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.sjlbkw.cn/Article/details/guedjwffn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/ghkymympk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.bbcook.cn/Article/details/genytrigx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/ghufytnmk.sHtML

TS:   path.extname("a.txt")
来源：http://baike.yfazqb.com/Article/details/gldtnhvjx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.vehdjk.com/Article/details/gyfhkxgnk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gfyigglcx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gfsqdhgmt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gruaduuim.sHtML

[F11] 复制与移动文件
来源：http://mobile.vehdjk.com/Article/details/gnzboadrm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/grdxgznpn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fktsv.cn/Article/details/gqpocomwe.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/gldszqynv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.epnwcf.com/Article/details/gwwlxlmfj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.yfazqb.com/Article/details/gurlnvzol.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.vehdjk.com/Article/details/gvwbuiuub.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/gjzqyxgir.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.bbcook.cn/Article/details/gxlnezxre.sHtML

[F12] CSV 读写
来源：http://wap.fktsv.cn/Article/details/gmmmeckoy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fktsv.cn/Article/details/gpjtasqho.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.yfazqb.com/Article/details/goylomfte.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.epnwcf.com/Article/details/gxaxqpmad.sHtML

TS:   // 同上
来源：http://www.share.bbcook.cn/Article/details/gehkmdcwo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.vehdjk.com/Article/details/gvvydsjlm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.vehdjk.com/Article/details/gqlccjuvs.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.bbcook.cn/Article/details/gqghbwktf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fktsv.cn/Article/details/gfpqwgory.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gouoxlvmt.sHtML

G. 面向对象
来源：http://www.blog.vehdjk.com/Article/details/ghlwjgcfl.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gilkmfmrw.sHtML

[G01] 定义类
来源：http://www.m.share.fktsv.cn/Article/details/gmpzyxybu.sHtML

Py:   class User: pass
来源：http://www.share.tarul.cn/Article/details/gxzeqcpyh.sHtML

PHP:  class User {}
来源：http://3g.epnwcf.com/Article/details/ghjbnuayg.sHtML

JS:   class User {}
来源：http://mobile.tarul.cn/Article/details/gypxwvxqt.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.epnwcf.com/Article/details/gfirczxxz.sHtML

Java: class User {}
来源：http://www.share.fktsv.cn/Article/details/goxgqxktv.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.epnwcf.com/Article/details/gpkvafahe.sHtML

Ruby: class User; end
来源：http://www.m.share.fktsv.cn/Article/details/gdrjebgua.sHtML

C#:   class User {}
来源：http://www.m.share.vehdjk.com/Article/details/gtgudrkyw.sHtML

[G02] 构造函数
来源：http://blog.fktsv.cn/Article/details/goetbuqsd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.yfazqb.com/Article/details/gqwrewbjh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.tarul.cn/Article/details/gvverxcoz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.epnwcf.com/Article/details/gxfalugng.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.yfazqb.com/Article/details/ggkkhblqz.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.yfazqb.com/Article/details/gytgqqhxq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.tarul.cn/Article/details/gmkpthjwb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fktsv.cn/Article/details/gxicfqwuq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gohbxuqtp.sHtML

[G03] 实例属性
来源：http://read.share.sjlbkw.cn/Article/details/gzoaxhojb.sHtML

Py:   self.name = "x"
来源：http://read.share.tarul.cn/Article/details/gfexkflyy.sHtML

PHP:  public string $name = "x";
来源：http://wap.yfazqb.com/Article/details/geehlcwko.sHtML

JS:   this.name = "x";
来源：http://blog.sjlbkw.cn/Article/details/gbfooumgo.sHtML

TS:   name: string = "x";
来源：http://www.share.yfazqb.com/Article/details/gddoezoku.sHtML

Java: private String name;
来源：http://m.share.yfazqb.com/Article/details/gdibvhhun.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.epnwcf.com/Article/details/gtgmqkgfr.sHtML

Ruby: @name = "x"
来源：http://wap.sjlbkw.cn/Article/details/goaggqdad.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.vehdjk.com/Article/details/gaqefrrjt.sHtML

[G04] 定义方法
来源：http://www.m.share.fktsv.cn/Article/details/gokzvoajr.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fktsv.cn/Article/details/gkhjynnzd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.yfazqb.com/Article/details/ghwjefyuv.sHtML

JS:   greet() { return this.name; }
来源：http://3g.tarul.cn/Article/details/gpagfmlzc.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/grjlifuhj.sHtML

Java: String greet() { return name; }
来源：http://blog.bbcook.cn/Article/details/gakhwcdyg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fktsv.cn/Article/details/gbvhutxsn.sHtML

Ruby: def greet; @name; end
来源：http://baike.sjlbkw.cn/Article/details/glqwqlbix.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.yfazqb.com/Article/details/gqinotwtd.sHtML

[G05] 继承
来源：http://read.share.fktsv.cn/Article/details/gssguawig.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fktsv.cn/Article/details/gkevwhaqu.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/gcobpprzf.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.epnwcf.com/Article/details/gonkiyfcx.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.epnwcf.com/Article/details/gbhtcfumc.sHtML

Java: class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/gsgfcunsw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.tarul.cn/Article/details/gazftbvyh.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.yfazqb.com/Article/details/gukwovbgf.sHtML

C#:   class Admin : User {}
来源：http://wap.bbcook.cn/Article/details/gpseeqfip.sHtML

[G06] 重写方法
来源：http://mobile.sjlbkw.cn/Article/details/gvcrwptme.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.tarul.cn/Article/details/gzbptgrwz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gyrekiufu.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/gwpvgvjoc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/gnolizvdo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/gvazyhvuv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.epnwcf.com/Article/details/gunztkrvx.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.bbcook.cn/Article/details/gdqxnlggr.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.bbcook.cn/Article/details/gpuavvyau.sHtML

[G07] 调用父类方法
来源：http://read.share.yfazqb.com/Article/details/gdjvzgpnk.sHtML

Py:   super().greet()
来源：http://m.share.sjlbkw.cn/Article/details/greosjgsn.sHtML

PHP:  parent::greet();
来源：http://baike.tarul.cn/Article/details/gmxecfxfh.sHtML

JS:   super.greet();
来源：http://m.share.tarul.cn/Article/details/gixtmjwxl.sHtML

TS:   super.greet();
来源：http://3g.fktsv.cn/Article/details/gnjtvmeyg.sHtML

Java: super.greet();
来源：http://baike.tarul.cn/Article/details/gmsiiesob.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.epnwcf.com/Article/details/gwzmvfokl.sHtML

Ruby: super
来源：http://m.share.yfazqb.com/Article/details/gwfampqts.sHtML

C#:   base.Greet();
来源：http://mobile.tarul.cn/Article/details/gkhirldgh.sHtML

[G08] 静态方法与属性
来源：http://3g.sjlbkw.cn/Article/details/grbabyrqw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.yfazqb.com/Article/details/gzveqdien.sHtML

PHP:  public static function f() {}
来源：http://baike.yfazqb.com/Article/details/ggogtxtle.sHtML

JS:   static f() {}
来源：http://read.share.fktsv.cn/Article/details/gmsngtmqn.sHtML

TS:   static f(): void {}
来源：http://m.share.vehdjk.com/Article/details/ghmeutvxx.sHtML

Java: static void f() {}
来源：http://baike.bbcook.cn/Article/details/gnjojgxrf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.yfazqb.com/Article/details/grfumsctz.sHtML

Ruby: def self.f; end
来源：http://baike.yfazqb.com/Article/details/gkjbivmdk.sHtML

C#:   public static void F() {}
来源：http://wap.fktsv.cn/Article/details/goodldzga.sHtML

[G09] 接口 / 抽象类
来源：http://baike.epnwcf.com/Article/details/gbbjzqfyi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.sjlbkw.cn/Article/details/gphuqsxzt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.bbcook.cn/Article/details/giubzwziw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.sjlbkw.cn/Article/details/gysmlylqc.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.epnwcf.com/Article/details/gbrtizoru.sHtML

Java: interface Shape { double area(); }
来源：http://3g.tarul.cn/Article/details/gztzebsun.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.epnwcf.com/Article/details/gttvvwutk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.epnwcf.com/Article/details/gieesjsfw.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.epnwcf.com/Article/details/gkswxyyub.sHtML

[G10] 访问控制
来源：http://m.share.bbcook.cn/Article/details/gqqwalipe.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.yfazqb.com/Article/details/gzwonxags.sHtML

PHP:  public / protected / private
来源：http://m.share.sjlbkw.cn/Article/details/gykpdoojs.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.epnwcf.com/Article/details/glxauftgy.sHtML

TS:   public / protected / private
来源：http://m.share.fktsv.cn/Article/details/gasdokuav.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.tarul.cn/Article/details/glugtlxzh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.epnwcf.com/Article/details/gnxdtsycy.sHtML

Ruby: public / protected / private
来源：http://read.share.fktsv.cn/Article/details/glnurdaqk.sHtML

C#:   public / protected / private / internal
来源：http://mobile.bbcook.cn/Article/details/gpvsrqoyc.sHtML

[G11] getter / setter
来源：http://mobile.yfazqb.com/Article/details/gzvcedlrr.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.vehdjk.com/Article/details/ghtxmfwnt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.tarul.cn/Article/details/gmetfrhqm.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.vehdjk.com/Article/details/gmvfxgorz.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.vehdjk.com/Article/details/gabyopnls.sHtML

Java: public String getName() { return name; }
来源：http://wap.tarul.cn/Article/details/gpdzqrqno.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.yfazqb.com/Article/details/grwzaknvx.sHtML

Ruby: attr_accessor :name
来源：http://m.share.tarul.cn/Article/details/gizeoilsk.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.vehdjk.com/Article/details/gbmlbgxce.sHtML

[G12] 对象转字符串
来源：http://3g.epnwcf.com/Article/details/gbfarxpol.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.bbcook.cn/Article/details/geabzfqtz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.epnwcf.com/Article/details/gtdllgzsa.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.sjlbkw.cn/Article/details/gxryglclf.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/grlzlijgh.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gtdmvapyg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.vehdjk.com/Article/details/gymkwvbrc.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.vehdjk.com/Article/details/gudmcsurk.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.tarul.cn/Article/details/gkfsjwgsr.sHtML

[G13] 判断对象类型
来源：http://read.share.sjlbkw.cn/Article/details/gvejzcuhc.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.bbcook.cn/Article/details/gfyobgznm.sHtML

PHP:  $u instanceof User
来源：http://www.share.tarul.cn/Article/details/givjhxigf.sHtML

JS:   u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/gsefkjhhb.sHtML

TS:   u instanceof User
来源：http://baike.tarul.cn/Article/details/gyeagmaes.sHtML

Java: u instanceof User
来源：http://m.share.tarul.cn/Article/details/gigmssncz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fktsv.cn/Article/details/gslqxqsqx.sHtML

Ruby: u.is_a?(User)
来源：http://3g.vehdjk.com/Article/details/grnducaxi.sHtML

C#:   u is User
来源：http://www.share.epnwcf.com/Article/details/gjlvkixrj.sHtML

[G14] 数据类 / record
来源：http://www.m.share.tarul.cn/Article/details/gcxhpbcvo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.yfazqb.com/Article/details/gxfcxxigx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.epnwcf.com/Article/details/gwbqncivs.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.bbcook.cn/Article/details/gjgwgvwks.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.yfazqb.com/Article/details/gnbiezszp.sHtML

Java: record User(String name, int age) {}
来源：http://3g.tarul.cn/Article/details/gtehqgcva.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.bbcook.cn/Article/details/gqcuvvqiu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fktsv.cn/Article/details/gukxahztz.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.vehdjk.com/Article/details/gngmyyiwr.sHtML

[G15] 枚举
来源：http://read.share.fktsv.cn/Article/details/grvhgyemy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.vehdjk.com/Article/details/gntgqefml.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.bbcook.cn/Article/details/gtiyghmtm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.tarul.cn/Article/details/gvlqgnjng.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fktsv.cn/Article/details/gfijwfixs.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.yfazqb.com/Article/details/geedsjgju.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.epnwcf.com/Article/details/gxxseojwi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.tarul.cn/Article/details/gryvljotx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.vehdjk.com/Article/details/gyoygxhig.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.epnwcf.com/Article/details/gfsmxdhck.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.bbcook.cn/Article/details/ggmduvoab.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fktsv.cn/Article/details/gvqgdfjua.sHtML

JS:   Object.entries(obj)
来源：http://read.share.vehdjk.com/Article/details/gqebmxmey.sHtML

TS:   Object.entries(obj)
来源：http://baike.bbcook.cn/Article/details/gibiqoxgk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.yfazqb.com/Article/details/gekosmalu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.tarul.cn/Article/details/gypczliar.sHtML

Ruby: obj.instance_variables
来源：http://wap.bbcook.cn/Article/details/gnhfqahas.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.bbcook.cn/Article/details/gnxeixslx.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/givbldcno.sHtML

H. 异常与错误处理
来源：http://mobile.fktsv.cn/Article/details/ghtiywwbe.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/ghzuvhfin.sHtML

[H01] try / catch 基础
来源：http://3g.fktsv.cn/Article/details/gxueswbnr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fktsv.cn/Article/details/gsaantvmx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.bbcook.cn/Article/details/gfwnzbetq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.bbcook.cn/Article/details/gtlypvgnf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.bbcook.cn/Article/details/gzhppknzj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.sjlbkw.cn/Article/details/gylkkgexl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.yfazqb.com/Article/details/gexyqzpmd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.bbcook.cn/Article/details/gtfochuja.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.tarul.cn/Article/details/gzdtasglw.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.vehdjk.com/Article/details/gcqzpprua.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.vehdjk.com/Article/details/gklyhollt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gjwafayff.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gsfsbvbas.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gjmjzbekq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gjjcmxjkz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.epnwcf.com/Article/details/gfhtwwmoj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fktsv.cn/Article/details/gemobuzep.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gmckpqukr.sHtML

[H03] 主动抛出异常
来源：http://blog.epnwcf.com/Article/details/gnqcoisfo.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.bbcook.cn/Article/details/gyepojlkx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gwdfdaufj.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.tarul.cn/Article/details/guivxxepg.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.tarul.cn/Article/details/gyhkfcjwb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.epnwcf.com/Article/details/genyvmoxq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fktsv.cn/Article/details/goolhrcpn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fktsv.cn/Article/details/gpuyicgap.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.epnwcf.com/Article/details/gwawlpnjy.sHtML

[H04] 自定义异常类型
来源：http://www.blog.yfazqb.com/Article/details/gzuvzbmgy.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.vehdjk.com/Article/details/glvuissko.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.epnwcf.com/Article/details/guzsoftic.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.epnwcf.com/Article/details/gbqoovskw.sHtML

TS:   class MyError extends Error {}
来源：http://blog.yfazqb.com/Article/details/gfhgltksp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.vehdjk.com/Article/details/gvipvhqep.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.vehdjk.com/Article/details/gltvhkprr.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.yfazqb.com/Article/details/gkanlzmzv.sHtML

C#:   class MyException : Exception {}
来源：http://blog.sjlbkw.cn/Article/details/gzakduigx.sHtML

[H05] 捕获特定类型
来源：http://www.blog.sjlbkw.cn/Article/details/gakhltkpk.sHtML

Py:   except ValueError as e:
来源：http://www.share.vehdjk.com/Article/details/gyghpvclz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.bbcook.cn/Article/details/gfoxhmvyp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.epnwcf.com/Article/details/gslbymugf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.yfazqb.com/Article/details/girumxejv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.tarul.cn/Article/details/gncybuiec.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.tarul.cn/Article/details/glfkryrzj.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.vehdjk.com/Article/details/gbmdbfbzl.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.epnwcf.com/Article/details/gjrwbidnp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.tarul.cn/Article/details/gfmjehkxj.sHtML

Py:   value = d.get("k") or default
来源：http://blog.epnwcf.com/Article/details/gmnjnngvi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.sjlbkw.cn/Article/details/gvybsaisl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.epnwcf.com/Article/details/gjyyzedqw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.sjlbkw.cn/Article/details/gxmioxtqr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.epnwcf.com/Article/details/guhhlicgf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.vehdjk.com/Article/details/gnoqprqdx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.yfazqb.com/Article/details/gxoklygpx.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fktsv.cn/Article/details/gesmnozkj.sHtML

[H07] 断言
来源：http://wap.fktsv.cn/Article/details/gjggduwbj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.bbcook.cn/Article/details/gushibogc.sHtML

PHP:  assert($x > 0);
来源：http://baike.epnwcf.com/Article/details/goqlnptcm.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.sjlbkw.cn/Article/details/giplsihul.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.tarul.cn/Article/details/gauciazgq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.tarul.cn/Article/details/gqbehvytg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fktsv.cn/Article/details/gihhzbvnm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.bbcook.cn/Article/details/gwmfnhoqm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.bbcook.cn/Article/details/glzabwvvp.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.sjlbkw.cn/Article/details/gitpleorl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fktsv.cn/Article/details/guszhttdf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.epnwcf.com/Article/details/guukhbfbl.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.epnwcf.com/Article/details/gucxaxgup.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.bbcook.cn/Article/details/ghzjkdltc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fktsv.cn/Article/details/goxstisle.sHtML

Go:   err.Error()
来源：http://read.share.fktsv.cn/Article/details/gtzwwdjrn.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.bbcook.cn/Article/details/gdteksfwt.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.bbcook.cn/Article/details/gzuleqtds.sHtML

[H09] 带错误码的异常
来源：http://baike.sjlbkw.cn/Article/details/gfmauydpk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fktsv.cn/Article/details/gbrfumlqm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.tarul.cn/Article/details/gegsczvoz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.epnwcf.com/Article/details/gzyhdzmgs.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.vehdjk.com/Article/details/gamwqevkn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.sjlbkw.cn/Article/details/gzupkqitn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fktsv.cn/Article/details/gqjlvdade.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.sjlbkw.cn/Article/details/gyjffbovn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.sjlbkw.cn/Article/details/gkypcioof.sHtML

[H10] 资源自动释放
来源：http://m.share.epnwcf.com/Article/details/gypehqplv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.vehdjk.com/Article/details/gkxiscnfm.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.fktsv.cn/Article/details/glblbwrgq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.epnwcf.com/Article/details/gwvsfcbht.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.tarul.cn/Article/details/gaewcrucm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.sjlbkw.cn/Article/details/gnnxtccvk.sHtML

Go:   defer f.Close()
来源：http://m.share.vehdjk.com/Article/details/gscsctkza.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.yfazqb.com/Article/details/gxjgugdtt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gacjmeegy.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gsisbarvl.sHtML

I. 正则表达式
来源：http://m.share.tarul.cn/Article/details/gfnwqvkee.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gtuwrwjxi.sHtML

[I01] 判断是否匹配
来源：http://wap.epnwcf.com/Article/details/gjvnabtub.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.vehdjk.com/Article/details/gyxxlxjcv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.yfazqb.com/Article/details/gzgayskhh.sHtML

JS:   /\d+/.test(s)
来源：http://3g.epnwcf.com/Article/details/gqsqjuauq.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.yfazqb.com/Article/details/gcpstezbv.sHtML


<!-- 参考信息 -->