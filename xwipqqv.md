代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/grrukjdpn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gxqfyaqyu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.yfazqb.com/Article/details/gtjeklbpq.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.bbcook.cn/Article/details/gzcaiwsxi.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fktsv.cn/Article/details/ghpzenill.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gacoymbfz.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.sjlbkw.cn/Article/details/gpxztsscp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.bbcook.cn/Article/details/gzcomtetc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.bbcook.cn/Article/details/giyzyrdge.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.vehdjk.com/Article/details/ggzqpxsvx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.epnwcf.com/Article/details/gvkafiptu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.bbcook.cn/Article/details/ggnovgtxq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.sjlbkw.cn/Article/details/gwzajmhsy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.yfazqb.com/Article/details/gvgzselzj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fktsv.cn/Article/details/gxtqbjjsp.sHtML

[F08] 遍历目录
来源：http://blog.tarul.cn/Article/details/giqciqoeg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.epnwcf.com/Article/details/gmtqjjmle.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.tarul.cn/Article/details/glfjugtzo.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gwfnwkdqv.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.vehdjk.com/Article/details/gnoavyvlx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.epnwcf.com/Article/details/glwajpdup.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.bbcook.cn/Article/details/gjtjcxnbp.sHtML

Ruby: Dir.children("dir")
来源：http://baike.yfazqb.com/Article/details/glcoisxkk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.tarul.cn/Article/details/gajgwjujn.sHtML

[F09] 获取文件大小
来源：http://www.blog.fktsv.cn/Article/details/gohlyjvkv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gkzjmqizy.sHtML

PHP:  filesize("a.txt");
来源：http://3g.tarul.cn/Article/details/gmcmutefk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.epnwcf.com/Article/details/genunmhik.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.bbcook.cn/Article/details/gzpseqjmo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.yfazqb.com/Article/details/gxhfnsicm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.yfazqb.com/Article/details/gfrrqtatl.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.tarul.cn/Article/details/gbeydlhzt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.vehdjk.com/Article/details/guddhnhbd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.vehdjk.com/Article/details/gttqasnnv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gssayiylt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.epnwcf.com/Article/details/gnijgredb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/gsjteyykx.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.tarul.cn/Article/details/gidlwyaib.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.yfazqb.com/Article/details/gcbpznstj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/goqkbgpph.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gybqexipa.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gfsipfbou.sHtML

[F11] 复制与移动文件
来源：http://www.share.epnwcf.com/Article/details/gijfunxad.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/gyxjhwdrx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.epnwcf.com/Article/details/gctmfxndi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.yfazqb.com/Article/details/gixsgdptp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/gavodyjsi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fktsv.cn/Article/details/gwkocltdk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.vehdjk.com/Article/details/gzoywyszb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/giyvgyakr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.sjlbkw.cn/Article/details/gsrkshxtq.sHtML

[F12] CSV 读写
来源：http://wap.yfazqb.com/Article/details/gsnfoxuwy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fktsv.cn/Article/details/gdgdexeer.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.vehdjk.com/Article/details/gocegtfww.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.yfazqb.com/Article/details/grlmncrxz.sHtML

TS:   // 同上
来源：http://blog.sjlbkw.cn/Article/details/gfcahbzdh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fktsv.cn/Article/details/gbwrquwzr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.epnwcf.com/Article/details/gbojpvypl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.sjlbkw.cn/Article/details/gxmwuvltn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.epnwcf.com/Article/details/gzujfxahv.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gyyihyxmn.sHtML

G. 面向对象
来源：http://www.share.fktsv.cn/Article/details/govqdxmkv.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gktiwsclo.sHtML

[G01] 定义类
来源：http://www.blog.epnwcf.com/Article/details/gfrlxazkq.sHtML

Py:   class User: pass
来源：http://m.share.tarul.cn/Article/details/gppxuejix.sHtML

PHP:  class User {}
来源：http://www.share.tarul.cn/Article/details/ggqiqfdht.sHtML

JS:   class User {}
来源：http://www.m.share.tarul.cn/Article/details/gipvilpol.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fktsv.cn/Article/details/gebjdhbij.sHtML

Java: class User {}
来源：http://baike.tarul.cn/Article/details/grzmqzjbd.sHtML

Go:   type User struct { Name string }
来源：http://mobile.sjlbkw.cn/Article/details/goadmfnqa.sHtML

Ruby: class User; end
来源：http://www.blog.yfazqb.com/Article/details/goxlqmhuh.sHtML

C#:   class User {}
来源：http://www.share.fktsv.cn/Article/details/gpxdyebft.sHtML

[G02] 构造函数
来源：http://www.blog.sjlbkw.cn/Article/details/gyenbmrfj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.tarul.cn/Article/details/gzrltnggk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.vehdjk.com/Article/details/gnjkfsuln.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.yfazqb.com/Article/details/gbqixexue.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.tarul.cn/Article/details/gxxtdgofo.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.sjlbkw.cn/Article/details/gnyqqigko.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.yfazqb.com/Article/details/gaegldvxg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.epnwcf.com/Article/details/ggryiwsww.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.vehdjk.com/Article/details/gvpkyonmq.sHtML

[G03] 实例属性
来源：http://m.share.bbcook.cn/Article/details/gssffjrrw.sHtML

Py:   self.name = "x"
来源：http://m.share.yfazqb.com/Article/details/gbwnueohr.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.tarul.cn/Article/details/gztggqmxb.sHtML

JS:   this.name = "x";
来源：http://baike.vehdjk.com/Article/details/gayipkkyc.sHtML

TS:   name: string = "x";
来源：http://wap.yfazqb.com/Article/details/gettosiug.sHtML

Java: private String name;
来源：http://mobile.fktsv.cn/Article/details/gxupobifc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.yfazqb.com/Article/details/gwiccskrx.sHtML

Ruby: @name = "x"
来源：http://mobile.sjlbkw.cn/Article/details/gzigmpqwq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.tarul.cn/Article/details/gsplxkkqb.sHtML

[G04] 定义方法
来源：http://m.share.epnwcf.com/Article/details/gtdrvizrt.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.vehdjk.com/Article/details/gcwnyoxox.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.yfazqb.com/Article/details/grsktkdji.sHtML

JS:   greet() { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gthyyzkxq.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gblrqmvyw.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fktsv.cn/Article/details/gbujzxggz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.tarul.cn/Article/details/ghbijvxdt.sHtML

Ruby: def greet; @name; end
来源：http://baike.yfazqb.com/Article/details/gpigjdavk.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.yfazqb.com/Article/details/gqgurrsse.sHtML

[G05] 继承
来源：http://wap.yfazqb.com/Article/details/gnccjymue.sHtML

Py:   class Admin(User): pass
来源：http://wap.yfazqb.com/Article/details/gykcxzkpp.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.epnwcf.com/Article/details/gjcqluylx.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/greedzasm.sHtML

TS:   class Admin extends User {}
来源：http://baike.epnwcf.com/Article/details/godhkplqk.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/glamjrody.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.vehdjk.com/Article/details/ggaemssyx.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.yfazqb.com/Article/details/ghyfnfdfb.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.epnwcf.com/Article/details/giqmfncmc.sHtML

[G06] 重写方法
来源：http://m.share.epnwcf.com/Article/details/gtrqgwswh.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.sjlbkw.cn/Article/details/gybzkpxgp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gxerrxusz.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/ggtozuwjm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fktsv.cn/Article/details/giganjuzj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/gewevuatg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.sjlbkw.cn/Article/details/gxgbfpzfr.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.epnwcf.com/Article/details/gsdiyzaea.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.bbcook.cn/Article/details/gylkzctbu.sHtML

[G07] 调用父类方法
来源：http://www.share.tarul.cn/Article/details/gthskupzv.sHtML

Py:   super().greet()
来源：http://3g.yfazqb.com/Article/details/glqcfedqz.sHtML

PHP:  parent::greet();
来源：http://read.share.vehdjk.com/Article/details/gdlnzesqx.sHtML

JS:   super.greet();
来源：http://mobile.bbcook.cn/Article/details/gdxhiqhwu.sHtML

TS:   super.greet();
来源：http://www.blog.tarul.cn/Article/details/ghbwdxdkn.sHtML

Java: super.greet();
来源：http://www.share.epnwcf.com/Article/details/gjsljjnpv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.sjlbkw.cn/Article/details/gbavbspuo.sHtML

Ruby: super
来源：http://mobile.bbcook.cn/Article/details/ggphnfgjq.sHtML

C#:   base.Greet();
来源：http://www.share.bbcook.cn/Article/details/gbrgwwqmc.sHtML

[G08] 静态方法与属性
来源：http://baike.yfazqb.com/Article/details/glmtvbexa.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.tarul.cn/Article/details/gkcongfzr.sHtML

PHP:  public static function f() {}
来源：http://3g.fktsv.cn/Article/details/gpssvosgl.sHtML

JS:   static f() {}
来源：http://www.blog.epnwcf.com/Article/details/grjylrfne.sHtML

TS:   static f(): void {}
来源：http://mobile.yfazqb.com/Article/details/gdjvscbom.sHtML

Java: static void f() {}
来源：http://www.blog.bbcook.cn/Article/details/gmjyemjow.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.bbcook.cn/Article/details/gbnvycxhw.sHtML

Ruby: def self.f; end
来源：http://www.blog.sjlbkw.cn/Article/details/gcqwdqibz.sHtML

C#:   public static void F() {}
来源：http://wap.bbcook.cn/Article/details/guhvqkumi.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.epnwcf.com/Article/details/guxkmzbfe.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.epnwcf.com/Article/details/gnmseshqr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.tarul.cn/Article/details/gvnxvfkyc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fktsv.cn/Article/details/gxpqjevvy.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.vehdjk.com/Article/details/gzeybyyiz.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fktsv.cn/Article/details/gxacynfmb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.bbcook.cn/Article/details/gundbdkii.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fktsv.cn/Article/details/gfnwebcyn.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.epnwcf.com/Article/details/gibndvhgg.sHtML

[G10] 访问控制
来源：http://read.share.bbcook.cn/Article/details/gwcmwvqve.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.yfazqb.com/Article/details/gidbwypyf.sHtML

PHP:  public / protected / private
来源：http://3g.tarul.cn/Article/details/gpcqwnnfl.sHtML

JS:   #private 字段；其余公开
来源：http://blog.sjlbkw.cn/Article/details/gkjczihwr.sHtML

TS:   public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/gmskgwnlh.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.bbcook.cn/Article/details/grniioddp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.bbcook.cn/Article/details/gsrcktwpw.sHtML

Ruby: public / protected / private
来源：http://m.share.tarul.cn/Article/details/gscnnnhha.sHtML

C#:   public / protected / private / internal
来源：http://www.share.bbcook.cn/Article/details/gvebimpcf.sHtML

[G11] getter / setter
来源：http://3g.fktsv.cn/Article/details/gdrbblrvo.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.tarul.cn/Article/details/gwevixojj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fktsv.cn/Article/details/gkpbwjtmo.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.yfazqb.com/Article/details/gjygrjxgv.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.bbcook.cn/Article/details/glsxngevp.sHtML

Java: public String getName() { return name; }
来源：http://baike.epnwcf.com/Article/details/gfusexrov.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fktsv.cn/Article/details/guxpjyint.sHtML

Ruby: attr_accessor :name
来源：http://mobile.yfazqb.com/Article/details/gxcyrchri.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.sjlbkw.cn/Article/details/gikccbzkx.sHtML

[G12] 对象转字符串
来源：http://m.share.yfazqb.com/Article/details/gxetyilit.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.yfazqb.com/Article/details/ghmuatleq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fktsv.cn/Article/details/gflamrgnu.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fktsv.cn/Article/details/gtrbidgrj.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/gcgqelsyz.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gucwpihnm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fktsv.cn/Article/details/gtvqqxkwb.sHtML

Ruby: def to_s; @name; end
来源：http://blog.sjlbkw.cn/Article/details/gkrieurpr.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.vehdjk.com/Article/details/gwaxemrlh.sHtML

[G13] 判断对象类型
来源：http://baike.vehdjk.com/Article/details/gldcscqjo.sHtML

Py:   isinstance(u, User)
来源：http://blog.yfazqb.com/Article/details/gavmrtbyb.sHtML

PHP:  $u instanceof User
来源：http://mobile.bbcook.cn/Article/details/gpawlidfr.sHtML

JS:   u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gjragmzqb.sHtML

TS:   u instanceof User
来源：http://wap.sjlbkw.cn/Article/details/gcdyovtnh.sHtML

Java: u instanceof User
来源：http://3g.tarul.cn/Article/details/ghnwmypep.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.epnwcf.com/Article/details/gsawisiax.sHtML

Ruby: u.is_a?(User)
来源：http://3g.epnwcf.com/Article/details/gxtzanxiv.sHtML

C#:   u is User
来源：http://baike.epnwcf.com/Article/details/gscrjhisg.sHtML

[G14] 数据类 / record
来源：http://wap.bbcook.cn/Article/details/giukaexpp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.sjlbkw.cn/Article/details/geryoiaiw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fktsv.cn/Article/details/gixtsppcg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.vehdjk.com/Article/details/gzoqjvrkj.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fktsv.cn/Article/details/gigrcuoyw.sHtML

Java: record User(String name, int age) {}
来源：http://blog.tarul.cn/Article/details/gtbhlnjlk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.sjlbkw.cn/Article/details/gcixzbyev.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.epnwcf.com/Article/details/gcbrwnkxs.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fktsv.cn/Article/details/gvqisvgbf.sHtML

[G15] 枚举
来源：http://read.share.sjlbkw.cn/Article/details/gwtikobrr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.bbcook.cn/Article/details/gxvrwjtww.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.sjlbkw.cn/Article/details/gpitehepf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.tarul.cn/Article/details/gnamdrkis.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fktsv.cn/Article/details/gyephvxit.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.epnwcf.com/Article/details/glgzhrwdo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzqvopyz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.sjlbkw.cn/Article/details/gonwvhonm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.bbcook.cn/Article/details/gakfwohfp.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.bbcook.cn/Article/details/gxnpdsyuj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fktsv.cn/Article/details/gvpdtpdup.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.vehdjk.com/Article/details/gcnlkvetd.sHtML

JS:   Object.entries(obj)
来源：http://wap.sjlbkw.cn/Article/details/gynrvtzpr.sHtML

TS:   Object.entries(obj)
来源：http://baike.fktsv.cn/Article/details/gbunhudju.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.tarul.cn/Article/details/gyqcvsfto.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.bbcook.cn/Article/details/gmbdzbgye.sHtML

Ruby: obj.instance_variables
来源：http://blog.yfazqb.com/Article/details/gzdsqbsrk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.bbcook.cn/Article/details/gcazqyjgi.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/ghqmbeqqy.sHtML

H. 异常与错误处理
来源：http://mobile.tarul.cn/Article/details/glbyilyle.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gpvaiobob.sHtML

[H01] try / catch 基础
来源：http://read.share.bbcook.cn/Article/details/gcdevjkdl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.vehdjk.com/Article/details/guvxkxiii.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.vehdjk.com/Article/details/gievyzkfn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.epnwcf.com/Article/details/gvrogirga.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.yfazqb.com/Article/details/gaoyddbpk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.vehdjk.com/Article/details/guooazgkg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fktsv.cn/Article/details/gelauxkvl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.sjlbkw.cn/Article/details/gvegowtrx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.epnwcf.com/Article/details/gujwxqowf.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.bbcook.cn/Article/details/gypccalzv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.bbcook.cn/Article/details/gbpptlpor.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/gifdpitvo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gpdkqucai.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/glrerzrhb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/guzhbftvm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.vehdjk.com/Article/details/gssxlntmz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.tarul.cn/Article/details/gyqrumicr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/gclhhntjq.sHtML

[H03] 主动抛出异常
来源：http://read.share.tarul.cn/Article/details/gufrusayc.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.tarul.cn/Article/details/gjoplqtqo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gcsbypyng.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gbxtgchyc.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/gkgtejsda.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.yfazqb.com/Article/details/gcunhqlai.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.epnwcf.com/Article/details/gtmlajozg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.bbcook.cn/Article/details/gkfxaicru.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gfpduihxw.sHtML

[H04] 自定义异常类型
来源：http://3g.sjlbkw.cn/Article/details/gpocbnhds.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.epnwcf.com/Article/details/gkfvksoig.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.bbcook.cn/Article/details/gzhmduifo.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.epnwcf.com/Article/details/gvigzyesq.sHtML

TS:   class MyError extends Error {}
来源：http://wap.sjlbkw.cn/Article/details/gpzrfckkg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.sjlbkw.cn/Article/details/gonqfmyzp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fktsv.cn/Article/details/gmcnbjcdh.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.epnwcf.com/Article/details/gdgkriiww.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.tarul.cn/Article/details/gtnwagtbh.sHtML

[H05] 捕获特定类型
来源：http://www.share.vehdjk.com/Article/details/gttaxvrzj.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.sjlbkw.cn/Article/details/gqrdynpvg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.tarul.cn/Article/details/grkqapvgv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.tarul.cn/Article/details/gjkklunoq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.bbcook.cn/Article/details/gbyamzuxr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.vehdjk.com/Article/details/gyfiorvth.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.sjlbkw.cn/Article/details/gyvwvimnh.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.epnwcf.com/Article/details/gqvoxskhl.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.epnwcf.com/Article/details/gprbxbkfl.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.bbcook.cn/Article/details/gqanylqem.sHtML

Py:   value = d.get("k") or default
来源：http://baike.vehdjk.com/Article/details/grsbiikrd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.sjlbkw.cn/Article/details/guorftpfu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.yfazqb.com/Article/details/gzsdrbrnh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.yfazqb.com/Article/details/gyszszucn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fktsv.cn/Article/details/genjeqmkr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.tarul.cn/Article/details/gfznnbccu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fktsv.cn/Article/details/gztewijgj.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.epnwcf.com/Article/details/gdpszxkfe.sHtML

[H07] 断言
来源：http://mobile.tarul.cn/Article/details/gpsllbzsr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.tarul.cn/Article/details/gjswfizli.sHtML

PHP:  assert($x > 0);
来源：http://3g.fktsv.cn/Article/details/gtmgipqwv.sHtML

JS:   console.assert(x > 0);
来源：http://wap.tarul.cn/Article/details/gvhvhaqlm.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fktsv.cn/Article/details/gymbpxodz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.sjlbkw.cn/Article/details/gwetncvfw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.tarul.cn/Article/details/gjkeksxpr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.bbcook.cn/Article/details/gxfplsogf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.vehdjk.com/Article/details/gubbzglkn.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.yfazqb.com/Article/details/gvvsyddap.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fktsv.cn/Article/details/gjlcdcfzv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.epnwcf.com/Article/details/ghyvymynx.sHtML

JS:   e.message;  e.stack
来源：http://baike.bbcook.cn/Article/details/ggdfeaktx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.bbcook.cn/Article/details/gkozcmwmh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.tarul.cn/Article/details/gohuvzpzy.sHtML

Go:   err.Error()
来源：http://www.share.tarul.cn/Article/details/gpflilxdd.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.sjlbkw.cn/Article/details/gjwrgadnf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.vehdjk.com/Article/details/gyapbhusx.sHtML

[H09] 带错误码的异常
来源：http://www.share.sjlbkw.cn/Article/details/gvchjfkhk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fktsv.cn/Article/details/giikvmkti.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fktsv.cn/Article/details/gjgtfavya.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fktsv.cn/Article/details/gmetadzxx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fktsv.cn/Article/details/gofoyfqac.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.epnwcf.com/Article/details/gdnjzniny.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.yfazqb.com/Article/details/gkiejbvhh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.yfazqb.com/Article/details/gqdtnxmdh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.sjlbkw.cn/Article/details/gbnhhvuqe.sHtML

[H10] 资源自动释放
来源：http://m.share.bbcook.cn/Article/details/gpqoryyra.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.yfazqb.com/Article/details/gujcigvab.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.vehdjk.com/Article/details/ghtjmfrxi.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.epnwcf.com/Article/details/gafkhgret.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.yfazqb.com/Article/details/gvdoobuul.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.vehdjk.com/Article/details/gnopkiscd.sHtML

Go:   defer f.Close()
来源：http://mobile.bbcook.cn/Article/details/ghqyzcvic.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.epnwcf.com/Article/details/gnoorphba.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.tarul.cn/Article/details/gkxqboypf.sHtML


<!-- 参考信息 -->