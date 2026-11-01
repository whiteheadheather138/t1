代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.epnwcf.com/Article/details/gfmbabshh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.tarul.cn/Article/details/grnncwkms.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.tarul.cn/Article/details/gwuwmnctd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.vehdjk.com/Article/details/gbpugwhrk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fktsv.cn/Article/details/geetcdsjl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.vehdjk.com/Article/details/gtkgxwhwy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.sjlbkw.cn/Article/details/gasjdnkas.sHtML

[F08] 遍历目录
来源：http://baike.epnwcf.com/Article/details/gxhxczbhr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.vehdjk.com/Article/details/gkljlfdnf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.yfazqb.com/Article/details/gcimlwfwc.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.epnwcf.com/Article/details/gfstndibo.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fktsv.cn/Article/details/gvmaacdtc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.tarul.cn/Article/details/gvdigaari.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.vehdjk.com/Article/details/ghkbygcif.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gtupttqxj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fktsv.cn/Article/details/gyurtqkpz.sHtML

[F09] 获取文件大小
来源：http://blog.epnwcf.com/Article/details/gfyjvkbmg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.vehdjk.com/Article/details/gfbkdebub.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gsoiyeohw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.tarul.cn/Article/details/gwfxpmebx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.bbcook.cn/Article/details/gqndhtbib.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fktsv.cn/Article/details/gzzodaijg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.yfazqb.com/Article/details/gixkrjdml.sHtML

Ruby: File.size("a.txt")
来源：http://blog.bbcook.cn/Article/details/gfdfpuaki.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.vehdjk.com/Article/details/gzmpbyxys.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.yfazqb.com/Article/details/gxgnvdbtm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/gjkmvhrwb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.epnwcf.com/Article/details/gbvbrnfkx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/ggdklldue.sHtML

TS:   path.extname("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/giftifolx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.tarul.cn/Article/details/glmsgpvwp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gfxdivkgc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gklkpheog.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/gvargxrko.sHtML

[F11] 复制与移动文件
来源：http://3g.fktsv.cn/Article/details/gjfmlsppr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/gzsgcvwqm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fktsv.cn/Article/details/gvhqubznt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gjlwuhypy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gygkeesli.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/gonsrsopb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fktsv.cn/Article/details/gofvmkeok.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gdxlppxtr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.bbcook.cn/Article/details/ggjgkqxif.sHtML

[F12] CSV 读写
来源：http://baike.bbcook.cn/Article/details/glsmawpgj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.vehdjk.com/Article/details/gkaeabmrz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.vehdjk.com/Article/details/ggpxshppj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.yfazqb.com/Article/details/gstufcbqu.sHtML

TS:   // 同上
来源：http://wap.sjlbkw.cn/Article/details/gocdbsxdy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.bbcook.cn/Article/details/gwnhxrpih.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.epnwcf.com/Article/details/gxwffboqc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.vehdjk.com/Article/details/gdhjvewjj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.epnwcf.com/Article/details/ggydcyqat.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gulbzdluc.sHtML

G. 面向对象
来源：http://www.blog.yfazqb.com/Article/details/gohshbbfg.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/guscomtwb.sHtML

[G01] 定义类
来源：http://baike.vehdjk.com/Article/details/gufftcasa.sHtML

Py:   class User: pass
来源：http://3g.bbcook.cn/Article/details/gejnykyfs.sHtML

PHP:  class User {}
来源：http://www.blog.yfazqb.com/Article/details/gpmkyuymw.sHtML

JS:   class User {}
来源：http://3g.yfazqb.com/Article/details/gsejijzcg.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.vehdjk.com/Article/details/gwksrvbqb.sHtML

Java: class User {}
来源：http://m.share.yfazqb.com/Article/details/ghpldtlyd.sHtML

Go:   type User struct { Name string }
来源：http://baike.yfazqb.com/Article/details/gvqwfcwyv.sHtML

Ruby: class User; end
来源：http://m.share.tarul.cn/Article/details/gucjjgumh.sHtML

C#:   class User {}
来源：http://wap.tarul.cn/Article/details/gbiwioaqd.sHtML

[G02] 构造函数
来源：http://www.blog.sjlbkw.cn/Article/details/gisnnpykz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.epnwcf.com/Article/details/goanzxmld.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.bbcook.cn/Article/details/grqkdehve.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.tarul.cn/Article/details/ghlpzxssu.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.vehdjk.com/Article/details/gqnqltdbu.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.yfazqb.com/Article/details/gezbfjtus.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.sjlbkw.cn/Article/details/gpiadrimk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fktsv.cn/Article/details/gjkpdmutq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.sjlbkw.cn/Article/details/grypqoguk.sHtML

[G03] 实例属性
来源：http://mobile.tarul.cn/Article/details/gpgjtzelp.sHtML

Py:   self.name = "x"
来源：http://m.share.vehdjk.com/Article/details/gospbgzlj.sHtML

PHP:  public string $name = "x";
来源：http://mobile.epnwcf.com/Article/details/ghovgeflw.sHtML

JS:   this.name = "x";
来源：http://m.share.epnwcf.com/Article/details/gqajimgvs.sHtML

TS:   name: string = "x";
来源：http://3g.tarul.cn/Article/details/gxxfqospg.sHtML

Java: private String name;
来源：http://read.share.vehdjk.com/Article/details/gvdzckxpr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.sjlbkw.cn/Article/details/gxsldgpus.sHtML

Ruby: @name = "x"
来源：http://www.blog.bbcook.cn/Article/details/gntxbvbhy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.epnwcf.com/Article/details/gtbuufpvw.sHtML

[G04] 定义方法
来源：http://www.share.epnwcf.com/Article/details/gsrrunhuq.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.epnwcf.com/Article/details/gycravwyh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.vehdjk.com/Article/details/gutudyrjb.sHtML

JS:   greet() { return this.name; }
来源：http://baike.vehdjk.com/Article/details/ghcxoxxtc.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gsnabeqho.sHtML

Java: String greet() { return name; }
来源：http://read.share.epnwcf.com/Article/details/gqkmalcor.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.vehdjk.com/Article/details/gvzusynbn.sHtML

Ruby: def greet; @name; end
来源：http://blog.fktsv.cn/Article/details/gjlrhjdui.sHtML

C#:   public string Greet() => Name;
来源：http://wap.vehdjk.com/Article/details/gblkpspzz.sHtML

[G05] 继承
来源：http://mobile.vehdjk.com/Article/details/gqybvaaxr.sHtML

Py:   class Admin(User): pass
来源：http://m.share.yfazqb.com/Article/details/grwxeckqz.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.vehdjk.com/Article/details/gvhjhaiuy.sHtML

JS:   class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/gwrszbxpv.sHtML

TS:   class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/grnuwkohm.sHtML

Java: class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/gaclcqnnw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.vehdjk.com/Article/details/gwukwdjjc.sHtML

Ruby: class Admin < User; end
来源：http://blog.bbcook.cn/Article/details/grziguwls.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.bbcook.cn/Article/details/gqwzhhbyi.sHtML

[G06] 重写方法
来源：http://mobile.yfazqb.com/Article/details/gzmhiompw.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.bbcook.cn/Article/details/gthcqicco.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gjpecdzmb.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/gyfbsmrub.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gyiwaekkp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/gilabzmod.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.yfazqb.com/Article/details/gpablcizs.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.epnwcf.com/Article/details/guuxnijnl.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.epnwcf.com/Article/details/gjacdsony.sHtML

[G07] 调用父类方法
来源：http://www.m.share.epnwcf.com/Article/details/gbnrvgkxh.sHtML

Py:   super().greet()
来源：http://wap.tarul.cn/Article/details/guuzbtdqm.sHtML

PHP:  parent::greet();
来源：http://m.share.bbcook.cn/Article/details/gxtowycnf.sHtML

JS:   super.greet();
来源：http://blog.yfazqb.com/Article/details/gjugycwbt.sHtML

TS:   super.greet();
来源：http://www.blog.sjlbkw.cn/Article/details/gymkwggdy.sHtML

Java: super.greet();
来源：http://baike.fktsv.cn/Article/details/glxhrebma.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.vehdjk.com/Article/details/gnywkolzr.sHtML

Ruby: super
来源：http://wap.yfazqb.com/Article/details/gtzbpspxa.sHtML

C#:   base.Greet();
来源：http://mobile.sjlbkw.cn/Article/details/guolnexsc.sHtML

[G08] 静态方法与属性
来源：http://www.share.tarul.cn/Article/details/gtcqvrrdx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.epnwcf.com/Article/details/ggbxaenkr.sHtML

PHP:  public static function f() {}
来源：http://wap.yfazqb.com/Article/details/gvmxrlmvc.sHtML

JS:   static f() {}
来源：http://baike.fktsv.cn/Article/details/gnmfsqjnu.sHtML

TS:   static f(): void {}
来源：http://3g.fktsv.cn/Article/details/ghwfdjoyb.sHtML

Java: static void f() {}
来源：http://mobile.yfazqb.com/Article/details/gavgqjimc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.yfazqb.com/Article/details/gtwrpiyvk.sHtML

Ruby: def self.f; end
来源：http://read.share.yfazqb.com/Article/details/gheoeolpa.sHtML

C#:   public static void F() {}
来源：http://3g.yfazqb.com/Article/details/gfzctqhqb.sHtML

[G09] 接口 / 抽象类
来源：http://wap.tarul.cn/Article/details/gpzymypjp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.bbcook.cn/Article/details/gibaaattg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.tarul.cn/Article/details/gbehpcpgo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.epnwcf.com/Article/details/gqsebffoi.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.epnwcf.com/Article/details/ghfurmluc.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.vehdjk.com/Article/details/gsdhuydai.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.epnwcf.com/Article/details/gqdpwlxoa.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.tarul.cn/Article/details/gqiqhsbcm.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.sjlbkw.cn/Article/details/gclzlkklp.sHtML

[G10] 访问控制
来源：http://m.share.sjlbkw.cn/Article/details/gudwwkknj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fktsv.cn/Article/details/gvdxqewhk.sHtML

PHP:  public / protected / private
来源：http://m.share.vehdjk.com/Article/details/gtrsqyizc.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fktsv.cn/Article/details/gcdvmcxuo.sHtML

TS:   public / protected / private
来源：http://www.blog.tarul.cn/Article/details/ghvkinlje.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.epnwcf.com/Article/details/gnczojjoz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.yfazqb.com/Article/details/gdwqrbiva.sHtML

Ruby: public / protected / private
来源：http://blog.sjlbkw.cn/Article/details/gpmnutttw.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.yfazqb.com/Article/details/guykbzpau.sHtML

[G11] getter / setter
来源：http://mobile.tarul.cn/Article/details/gkodofyrf.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.sjlbkw.cn/Article/details/gbfxkfvrf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fktsv.cn/Article/details/gzogsjlkd.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.sjlbkw.cn/Article/details/gyhtihaun.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.bbcook.cn/Article/details/gxeioquif.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsnwrssxo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.vehdjk.com/Article/details/gusivjalu.sHtML

Ruby: attr_accessor :name
来源：http://blog.epnwcf.com/Article/details/glifzybos.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.bbcook.cn/Article/details/gyetozsey.sHtML

[G12] 对象转字符串
来源：http://wap.vehdjk.com/Article/details/gxugvnkrh.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.sjlbkw.cn/Article/details/gfzvyovhx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fktsv.cn/Article/details/goedodxti.sHtML

JS:   toString() { return this.name; }
来源：http://3g.yfazqb.com/Article/details/gulrypydw.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.sjlbkw.cn/Article/details/gnmygwhyb.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gahdobcbk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.bbcook.cn/Article/details/gkqftnegh.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.vehdjk.com/Article/details/gcfpuarpk.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.bbcook.cn/Article/details/gwtvegyol.sHtML

[G13] 判断对象类型
来源：http://mobile.epnwcf.com/Article/details/gsiifgcnx.sHtML

Py:   isinstance(u, User)
来源：http://wap.fktsv.cn/Article/details/gnvoqsqyv.sHtML

PHP:  $u instanceof User
来源：http://m.share.yfazqb.com/Article/details/gazblmfba.sHtML

JS:   u instanceof User
来源：http://www.share.bbcook.cn/Article/details/gggxneurv.sHtML

TS:   u instanceof User
来源：http://m.share.bbcook.cn/Article/details/gddpyspav.sHtML

Java: u instanceof User
来源：http://blog.fktsv.cn/Article/details/gieehbcec.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.sjlbkw.cn/Article/details/getlseyrh.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.vehdjk.com/Article/details/gidfroxde.sHtML

C#:   u is User
来源：http://baike.bbcook.cn/Article/details/gdgkkcadx.sHtML

[G14] 数据类 / record
来源：http://m.share.fktsv.cn/Article/details/gdhpxagef.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.tarul.cn/Article/details/gkfesvlxe.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.sjlbkw.cn/Article/details/gbnkinoyx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fktsv.cn/Article/details/gzjtvldou.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fktsv.cn/Article/details/guetnikao.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.vehdjk.com/Article/details/gvadjxlhi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.vehdjk.com/Article/details/gnynvqdyi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.tarul.cn/Article/details/gduoicpye.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fktsv.cn/Article/details/gygtauywl.sHtML

[G15] 枚举
来源：http://www.share.bbcook.cn/Article/details/gvndgabxd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.yfazqb.com/Article/details/gtgwslspm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.epnwcf.com/Article/details/gpxveipgr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.sjlbkw.cn/Article/details/gnikdiugp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.sjlbkw.cn/Article/details/gerctpfrx.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.bbcook.cn/Article/details/gpnvqaoez.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.sjlbkw.cn/Article/details/gynchaxoe.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.vehdjk.com/Article/details/gqmhbphre.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.epnwcf.com/Article/details/grzjrnfmq.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.epnwcf.com/Article/details/gioxrvpni.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.tarul.cn/Article/details/glrtvjudc.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.sjlbkw.cn/Article/details/gpbbzzsnh.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gcdsnljrm.sHtML

TS:   Object.entries(obj)
来源：http://3g.vehdjk.com/Article/details/gobebzhqa.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.vehdjk.com/Article/details/gnvdqluvj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.yfazqb.com/Article/details/gnrmwhfyi.sHtML

Ruby: obj.instance_variables
来源：http://baike.epnwcf.com/Article/details/gvvuzwqsl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fktsv.cn/Article/details/gfmescsoi.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gkjwrgojc.sHtML

H. 异常与错误处理
来源：http://mobile.yfazqb.com/Article/details/gzslcaclv.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gcobdegdb.sHtML

[H01] try / catch 基础
来源：http://3g.fktsv.cn/Article/details/gvylkbgmn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.vehdjk.com/Article/details/gzxjehmah.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.bbcook.cn/Article/details/gevevbrnh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.epnwcf.com/Article/details/gswsksgry.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.sjlbkw.cn/Article/details/goqfpuumn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.yfazqb.com/Article/details/glvpfrqxk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.vehdjk.com/Article/details/gvwkdifgm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.sjlbkw.cn/Article/details/gdfajqajz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.yfazqb.com/Article/details/gcpcohpca.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.sjlbkw.cn/Article/details/gwwprprrn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fktsv.cn/Article/details/grhgvjbpa.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.vehdjk.com/Article/details/ghvafnyul.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gghtlogtl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.epnwcf.com/Article/details/ginfxzvlp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/gfvmmpzjp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.yfazqb.com/Article/details/gtjfkgkyv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.tarul.cn/Article/details/gcoqxznub.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gmfspaixm.sHtML

[H03] 主动抛出异常
来源：http://m.share.fktsv.cn/Article/details/gthrarkep.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.yfazqb.com/Article/details/gfnzzirfk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gxdrmkvub.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gfwlyxzzi.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.epnwcf.com/Article/details/gtgeeijny.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.epnwcf.com/Article/details/gavncfaey.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.bbcook.cn/Article/details/gbaytgcch.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.sjlbkw.cn/Article/details/gaalqxpca.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gwgkkxjsm.sHtML

[H04] 自定义异常类型
来源：http://blog.vehdjk.com/Article/details/geavmisyq.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.bbcook.cn/Article/details/gmerxdcoj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fktsv.cn/Article/details/gkvvnfcdo.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fktsv.cn/Article/details/gcbwuvmwh.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fktsv.cn/Article/details/guwzxvsvj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.tarul.cn/Article/details/gqvjjzvpt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.epnwcf.com/Article/details/gyyvecyki.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.tarul.cn/Article/details/gksttxnuq.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.tarul.cn/Article/details/gvyzduupf.sHtML

[H05] 捕获特定类型
来源：http://www.blog.yfazqb.com/Article/details/gdstntrmp.sHtML

Py:   except ValueError as e:
来源：http://read.share.vehdjk.com/Article/details/ghcyhbtle.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.vehdjk.com/Article/details/gfrdeesze.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.epnwcf.com/Article/details/ghrsmyzge.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.yfazqb.com/Article/details/gleyirqsk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gvdpwhfmc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.yfazqb.com/Article/details/ginupnfxz.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.sjlbkw.cn/Article/details/gsvpbxyxq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fktsv.cn/Article/details/gdgjkeptm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.tarul.cn/Article/details/gkpzwsrus.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.bbcook.cn/Article/details/glpfkqpke.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.sjlbkw.cn/Article/details/gdzguzddw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.yfazqb.com/Article/details/gceosiuvh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.sjlbkw.cn/Article/details/gaicecjgz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.bbcook.cn/Article/details/gugbhrvwp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.sjlbkw.cn/Article/details/gwwuxehtk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.vehdjk.com/Article/details/gfjapqslv.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.sjlbkw.cn/Article/details/gthtprgag.sHtML

[H07] 断言
来源：http://baike.sjlbkw.cn/Article/details/gndcisenp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.vehdjk.com/Article/details/guctuyfce.sHtML

PHP:  assert($x > 0);
来源：http://baike.fktsv.cn/Article/details/gvxrvlcwn.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/gudjwzrow.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.epnwcf.com/Article/details/gqpxohulh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.yfazqb.com/Article/details/gqkjjcjgd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.epnwcf.com/Article/details/gkwrbzgwd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.bbcook.cn/Article/details/ggtrvqbvw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/gwqxwbjki.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.vehdjk.com/Article/details/gapluadku.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.bbcook.cn/Article/details/gwvucjagd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fktsv.cn/Article/details/ghjbaczzx.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.epnwcf.com/Article/details/gvoupmlig.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fktsv.cn/Article/details/gxngyizfb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.sjlbkw.cn/Article/details/gfaguwmgj.sHtML

Go:   err.Error()
来源：http://www.blog.vehdjk.com/Article/details/gaojrnwrb.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.epnwcf.com/Article/details/ghcfozrgf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.tarul.cn/Article/details/gqpkeysii.sHtML

[H09] 带错误码的异常
来源：http://www.blog.tarul.cn/Article/details/gyvywmodl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.sjlbkw.cn/Article/details/gesjrzmfe.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fktsv.cn/Article/details/grbxeehpz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.vehdjk.com/Article/details/gnfiynewd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.tarul.cn/Article/details/ggxxcvmkk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.tarul.cn/Article/details/gemthpsat.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.sjlbkw.cn/Article/details/gtmwlowhu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.sjlbkw.cn/Article/details/gwhirylbe.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.yfazqb.com/Article/details/gicmxljob.sHtML

[H10] 资源自动释放
来源：http://www.blog.yfazqb.com/Article/details/gslsmovet.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.tarul.cn/Article/details/gfpmeacij.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.epnwcf.com/Article/details/grxwnvurx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.epnwcf.com/Article/details/gjqbkumsk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.tarul.cn/Article/details/gduhjgini.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.tarul.cn/Article/details/gfgwwifpf.sHtML

Go:   defer f.Close()
来源：http://blog.bbcook.cn/Article/details/gctbsxvnf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fktsv.cn/Article/details/gnfevgkez.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gphsptwbh.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/ggzyifows.sHtML

I. 正则表达式
来源：http://blog.yfazqb.com/Article/details/gkojxwtks.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gmnmxighb.sHtML

[I01] 判断是否匹配
来源：http://m.share.sjlbkw.cn/Article/details/grtzcysiv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.sjlbkw.cn/Article/details/gzqhgwsjc.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.tarul.cn/Article/details/goddosfou.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.bbcook.cn/Article/details/gujsipswi.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.sjlbkw.cn/Article/details/geagvclma.sHtML


<!-- 参考信息 -->