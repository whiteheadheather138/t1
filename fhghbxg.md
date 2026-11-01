代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://wap.sjlbkw.cn/Article/details/gzkazktoo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.bbcook.cn/Article/details/gpyrfnzft.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/garobperh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gqqaadmje.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/gowavxgrl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/grtgvhiah.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.yfazqb.com/Article/details/gscbylvij.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gzmyuyvyo.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.epnwcf.com/Article/details/geipnixxj.sHtML

[F06] 删除文件
来源：http://www.share.sjlbkw.cn/Article/details/gjjlujdpm.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fktsv.cn/Article/details/gmuzxzmca.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/ggjnppgkh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gqtrylchv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gmbwjcblc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gdpteffny.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fktsv.cn/Article/details/gitugbsoe.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gfsqorvky.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/goelhpwdf.sHtML

[F07] 创建目录（含多级）
来源：http://baike.bbcook.cn/Article/details/grphnrupm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.tarul.cn/Article/details/gbqcoevkl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.vehdjk.com/Article/details/gcpnpxdyy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.bbcook.cn/Article/details/gsgjmhsmt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fktsv.cn/Article/details/gdxbqsudr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.bbcook.cn/Article/details/gnfidnmsd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.vehdjk.com/Article/details/gehxhqmls.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.tarul.cn/Article/details/glfwroaeb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.bbcook.cn/Article/details/gzritbcbq.sHtML

[F08] 遍历目录
来源：http://mobile.yfazqb.com/Article/details/gcecpqwva.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.bbcook.cn/Article/details/goduyzvfa.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.sjlbkw.cn/Article/details/gckxoukie.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fktsv.cn/Article/details/gxnsisadp.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.epnwcf.com/Article/details/gwfebsbhv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.epnwcf.com/Article/details/gvzyjkjmy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fktsv.cn/Article/details/gljfnvtqm.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fktsv.cn/Article/details/ggvmzxtvz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.vehdjk.com/Article/details/gbascxcpe.sHtML

[F09] 获取文件大小
来源：http://blog.bbcook.cn/Article/details/ghsowghkn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gugnnnbvj.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gwndopcyu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.yfazqb.com/Article/details/gjllfbnnb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.tarul.cn/Article/details/gczzweiyx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/gmumfslei.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.bbcook.cn/Article/details/gehkvpint.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gloucznbi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.epnwcf.com/Article/details/gftxdjwpa.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.bbcook.cn/Article/details/gpsvezvtq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gmknerszt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gbxfbaued.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gxkuvqxza.sHtML

TS:   path.extname("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gifjdkbhi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.sjlbkw.cn/Article/details/gyzfckyqv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gihcvoizc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gwwrsrgml.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/gvqpvfoog.sHtML

[F11] 复制与移动文件
来源：http://www.blog.vehdjk.com/Article/details/gklunhmpz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/geghjwzpf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.epnwcf.com/Article/details/gzlykbekl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.vehdjk.com/Article/details/gkhwnrfdy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gfvbeqhix.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/gluxtazpp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.tarul.cn/Article/details/grskfcmjo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.vehdjk.com/Article/details/gettfquib.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.tarul.cn/Article/details/gpjkdhpcd.sHtML

[F12] CSV 读写
来源：http://www.m.share.yfazqb.com/Article/details/gqithzkgp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.epnwcf.com/Article/details/gylibrkhu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.tarul.cn/Article/details/gxvxwolqc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.yfazqb.com/Article/details/gcggdnvsi.sHtML

TS:   // 同上
来源：http://baike.vehdjk.com/Article/details/gffupeiey.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.sjlbkw.cn/Article/details/gplabiotj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.bbcook.cn/Article/details/gkhvmdykc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.tarul.cn/Article/details/gmnbbzdpf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.bbcook.cn/Article/details/gqrtdzfcl.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gbmzsvbia.sHtML

G. 面向对象
来源：http://blog.fktsv.cn/Article/details/gjofvdhcn.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gcuhwobeb.sHtML

[G01] 定义类
来源：http://www.blog.fktsv.cn/Article/details/ggpsujufj.sHtML

Py:   class User: pass
来源：http://www.share.yfazqb.com/Article/details/ghfwiyiko.sHtML

PHP:  class User {}
来源：http://mobile.vehdjk.com/Article/details/gwpwcredd.sHtML

JS:   class User {}
来源：http://www.m.share.vehdjk.com/Article/details/gepljlbeq.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.vehdjk.com/Article/details/glwztukuz.sHtML

Java: class User {}
来源：http://www.share.yfazqb.com/Article/details/gxaorjrzs.sHtML

Go:   type User struct { Name string }
来源：http://blog.tarul.cn/Article/details/gycouvdxy.sHtML

Ruby: class User; end
来源：http://www.blog.vehdjk.com/Article/details/gjushzflh.sHtML

C#:   class User {}
来源：http://baike.yfazqb.com/Article/details/gkxjvdbfz.sHtML

[G02] 构造函数
来源：http://www.share.epnwcf.com/Article/details/gcgszzudg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fktsv.cn/Article/details/gziiboijr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.yfazqb.com/Article/details/ggxnvwryz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fktsv.cn/Article/details/gjpcrgpuk.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.tarul.cn/Article/details/glpemvxlk.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.sjlbkw.cn/Article/details/gocsdxhlx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.yfazqb.com/Article/details/gohxriybd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.yfazqb.com/Article/details/grrnnbshb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.yfazqb.com/Article/details/ghgqmjcbw.sHtML

[G03] 实例属性
来源：http://mobile.bbcook.cn/Article/details/ghdisijbj.sHtML

Py:   self.name = "x"
来源：http://www.blog.sjlbkw.cn/Article/details/gxdwiaizk.sHtML

PHP:  public string $name = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gconhkyyx.sHtML

JS:   this.name = "x";
来源：http://www.blog.yfazqb.com/Article/details/gyqinqhqv.sHtML

TS:   name: string = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gmrxnlcla.sHtML

Java: private String name;
来源：http://www.blog.tarul.cn/Article/details/gncjgywaj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.yfazqb.com/Article/details/gsxmgyohk.sHtML

Ruby: @name = "x"
来源：http://wap.sjlbkw.cn/Article/details/gukghxmjd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.epnwcf.com/Article/details/gsbxsjmnm.sHtML

[G04] 定义方法
来源：http://www.blog.yfazqb.com/Article/details/ggqakyrqh.sHtML

Py:   def greet(self): return self.name
来源：http://baike.bbcook.cn/Article/details/gqsejlakn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.tarul.cn/Article/details/gkefrtimo.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.tarul.cn/Article/details/gjccyxaso.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/godceopnp.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gwgsbgvph.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.bbcook.cn/Article/details/gxuagxgqh.sHtML

Ruby: def greet; @name; end
来源：http://blog.yfazqb.com/Article/details/gdrwimobi.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.yfazqb.com/Article/details/gastcimbd.sHtML

[G05] 继承
来源：http://blog.bbcook.cn/Article/details/gznkcdsop.sHtML

Py:   class Admin(User): pass
来源：http://wap.vehdjk.com/Article/details/gkbaxiafu.sHtML

PHP:  class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gqgyxykkh.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fktsv.cn/Article/details/gutvahfnb.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fktsv.cn/Article/details/gejrraimy.sHtML

Java: class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gncccvwhm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.vehdjk.com/Article/details/grqddmixp.sHtML

Ruby: class Admin < User; end
来源：http://wap.epnwcf.com/Article/details/gerbjlabo.sHtML

C#:   class Admin : User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gpvfckpym.sHtML

[G06] 重写方法
来源：http://m.share.fktsv.cn/Article/details/gngxgedif.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.tarul.cn/Article/details/gtaenqrjy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gthvugzwm.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.tarul.cn/Article/details/gcaljeeln.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/gxuyojtzv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/gsmtrxtss.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.sjlbkw.cn/Article/details/glxtgzvak.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.yfazqb.com/Article/details/gpphfaqsl.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.yfazqb.com/Article/details/gwxkrbycb.sHtML

[G07] 调用父类方法
来源：http://3g.bbcook.cn/Article/details/ggozjardo.sHtML

Py:   super().greet()
来源：http://blog.tarul.cn/Article/details/gheazzfjb.sHtML

PHP:  parent::greet();
来源：http://blog.sjlbkw.cn/Article/details/giwlohdbz.sHtML

JS:   super.greet();
来源：http://mobile.yfazqb.com/Article/details/gzbrvajtl.sHtML

TS:   super.greet();
来源：http://3g.tarul.cn/Article/details/gcshvxguk.sHtML

Java: super.greet();
来源：http://wap.yfazqb.com/Article/details/ggjkgnqga.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fktsv.cn/Article/details/gbppiedth.sHtML

Ruby: super
来源：http://read.share.epnwcf.com/Article/details/gmcygoggt.sHtML

C#:   base.Greet();
来源：http://mobile.epnwcf.com/Article/details/gyvpkrard.sHtML

[G08] 静态方法与属性
来源：http://3g.vehdjk.com/Article/details/gfjgitfps.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fktsv.cn/Article/details/gsqizdaez.sHtML

PHP:  public static function f() {}
来源：http://m.share.vehdjk.com/Article/details/glwsebjzc.sHtML

JS:   static f() {}
来源：http://read.share.bbcook.cn/Article/details/geasrogoo.sHtML

TS:   static f(): void {}
来源：http://www.share.vehdjk.com/Article/details/gbzswatls.sHtML

Java: static void f() {}
来源：http://3g.sjlbkw.cn/Article/details/gvypnugoj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.vehdjk.com/Article/details/gacbkzxhe.sHtML

Ruby: def self.f; end
来源：http://m.share.bbcook.cn/Article/details/gzomycgjb.sHtML

C#:   public static void F() {}
来源：http://www.m.share.vehdjk.com/Article/details/ghwcwygmo.sHtML

[G09] 接口 / 抽象类
来源：http://blog.tarul.cn/Article/details/gpnuqampv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.epnwcf.com/Article/details/gilrzhzfp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.bbcook.cn/Article/details/gqquvvavt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.yfazqb.com/Article/details/gvyoygmdi.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.vehdjk.com/Article/details/gcikjhglp.sHtML

Java: interface Shape { double area(); }
来源：http://baike.epnwcf.com/Article/details/gpzbgjekp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.epnwcf.com/Article/details/gvvtkmphp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.yfazqb.com/Article/details/gualgwdhn.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.vehdjk.com/Article/details/gyszwfkyv.sHtML

[G10] 访问控制
来源：http://www.blog.bbcook.cn/Article/details/ggzifevvv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fktsv.cn/Article/details/grebborfc.sHtML

PHP:  public / protected / private
来源：http://baike.vehdjk.com/Article/details/gxnsgnqlr.sHtML

JS:   #private 字段；其余公开
来源：http://wap.bbcook.cn/Article/details/gegwiwbgt.sHtML

TS:   public / protected / private
来源：http://read.share.epnwcf.com/Article/details/gcjxmyymq.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.bbcook.cn/Article/details/gjfeduxqm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.bbcook.cn/Article/details/geslkgtkb.sHtML

Ruby: public / protected / private
来源：http://blog.vehdjk.com/Article/details/gxiegbqgv.sHtML

C#:   public / protected / private / internal
来源：http://baike.epnwcf.com/Article/details/gtfybbygc.sHtML

[G11] getter / setter
来源：http://mobile.vehdjk.com/Article/details/ggcrjpwyj.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.epnwcf.com/Article/details/gyzfokfny.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.epnwcf.com/Article/details/gnvivkdki.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.yfazqb.com/Article/details/gugiilcjb.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.tarul.cn/Article/details/gexlzweuw.sHtML

Java: public String getName() { return name; }
来源：http://www.share.bbcook.cn/Article/details/gcdiqzhwb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.bbcook.cn/Article/details/gvnqiwgqk.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.yfazqb.com/Article/details/gpwxckxek.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fktsv.cn/Article/details/gmxsuptxv.sHtML

[G12] 对象转字符串
来源：http://www.blog.yfazqb.com/Article/details/gfhhnewnj.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fktsv.cn/Article/details/gwcdbpaqn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.bbcook.cn/Article/details/ggorviurm.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gqrverteh.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.vehdjk.com/Article/details/ggbatrlfn.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fktsv.cn/Article/details/gfcchtotp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.tarul.cn/Article/details/gsdyfgvvq.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.yfazqb.com/Article/details/ggxdxqfhb.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.vehdjk.com/Article/details/gorrfupgj.sHtML

[G13] 判断对象类型
来源：http://baike.fktsv.cn/Article/details/gwsvmspgg.sHtML

Py:   isinstance(u, User)
来源：http://mobile.tarul.cn/Article/details/gfyxgfxze.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/gnnoowptq.sHtML

JS:   u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/gvqobznbg.sHtML

TS:   u instanceof User
来源：http://mobile.epnwcf.com/Article/details/gvuwvgwbj.sHtML

Java: u instanceof User
来源：http://3g.vehdjk.com/Article/details/gfmckehbw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.epnwcf.com/Article/details/gtyxsgrka.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fktsv.cn/Article/details/gkzncvazr.sHtML

C#:   u is User
来源：http://3g.vehdjk.com/Article/details/gymevlmbn.sHtML

[G14] 数据类 / record
来源：http://www.m.share.tarul.cn/Article/details/gqqjinvjp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.yfazqb.com/Article/details/gtedrbaik.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.vehdjk.com/Article/details/gcbornwsv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.epnwcf.com/Article/details/gtnwhwnet.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.yfazqb.com/Article/details/gjnelunux.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.bbcook.cn/Article/details/grkiftpaj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.yfazqb.com/Article/details/gekqdueai.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.tarul.cn/Article/details/gospfxikq.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.vehdjk.com/Article/details/geuvdlous.sHtML

[G15] 枚举
来源：http://read.share.sjlbkw.cn/Article/details/gietcscxs.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.yfazqb.com/Article/details/gpuichspy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fktsv.cn/Article/details/gjvhvcyyu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.tarul.cn/Article/details/gebxtvwho.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fktsv.cn/Article/details/gsvasklic.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.vehdjk.com/Article/details/geguvythi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.sjlbkw.cn/Article/details/gvedglzwr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.yfazqb.com/Article/details/gymwtbrxu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.sjlbkw.cn/Article/details/gzqiwbnsq.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.yfazqb.com/Article/details/gitrinqoe.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.bbcook.cn/Article/details/gedcmhifh.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.yfazqb.com/Article/details/gnzsgkbhy.sHtML

JS:   Object.entries(obj)
来源：http://blog.bbcook.cn/Article/details/gwmxapyys.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.bbcook.cn/Article/details/gbxtqtcjz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fktsv.cn/Article/details/gcjvubphj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.vehdjk.com/Article/details/gmemtzxtx.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fktsv.cn/Article/details/gheynjfru.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.vehdjk.com/Article/details/gxtxtdyjz.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gokrqozfl.sHtML

H. 异常与错误处理
来源：http://read.share.fktsv.cn/Article/details/gfikyhxpg.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/grzwejgqt.sHtML

[H01] try / catch 基础
来源：http://m.share.tarul.cn/Article/details/gatqisaoq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fktsv.cn/Article/details/ggyfhinmh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.vehdjk.com/Article/details/gbegzoqoi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.epnwcf.com/Article/details/gbaxsqzvb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.sjlbkw.cn/Article/details/goptyoutf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.sjlbkw.cn/Article/details/glbnykcvl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.sjlbkw.cn/Article/details/ghcxdamok.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.epnwcf.com/Article/details/goljdfhim.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.epnwcf.com/Article/details/gviyiickq.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.epnwcf.com/Article/details/gbdavtegi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.bbcook.cn/Article/details/gmcoibhwm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.bbcook.cn/Article/details/gxpfzrndl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.tarul.cn/Article/details/ghhubyyii.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gvlnmptgc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fktsv.cn/Article/details/ggzpdxgiu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fktsv.cn/Article/details/gniutqnnf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.tarul.cn/Article/details/guzgzxfkm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gypcpvtyd.sHtML

[H03] 主动抛出异常
来源：http://mobile.yfazqb.com/Article/details/gbpxurakn.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.tarul.cn/Article/details/gfmeqiamr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.yfazqb.com/Article/details/ginbgvrjy.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gahxaksrg.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gpqdeixxx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.vehdjk.com/Article/details/gpqvsiwev.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.epnwcf.com/Article/details/gbluvzvss.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.sjlbkw.cn/Article/details/gepchrodf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gfwobyopo.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gbuqrucnq.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.epnwcf.com/Article/details/gkijwkdzq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.sjlbkw.cn/Article/details/goqafmtkx.sHtML

JS:   class MyError extends Error {}
来源：http://3g.sjlbkw.cn/Article/details/gmwqukiaa.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.bbcook.cn/Article/details/gvguvuqzs.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.sjlbkw.cn/Article/details/gsbwaaois.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.yfazqb.com/Article/details/gnjpleuht.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fktsv.cn/Article/details/gcurreiag.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.yfazqb.com/Article/details/ghjwwdqye.sHtML

[H05] 捕获特定类型
来源：http://www.share.fktsv.cn/Article/details/gimwztxuh.sHtML

Py:   except ValueError as e:
来源：http://wap.sjlbkw.cn/Article/details/gzmslwkbt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.tarul.cn/Article/details/gharlspuc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.bbcook.cn/Article/details/gouhifisb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.bbcook.cn/Article/details/gdzvlivfe.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.yfazqb.com/Article/details/gyyymnoso.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.epnwcf.com/Article/details/glrgafvbf.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fktsv.cn/Article/details/ghncqtiov.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.vehdjk.com/Article/details/gjalfpmey.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.yfazqb.com/Article/details/gjluqpdfp.sHtML

Py:   value = d.get("k") or default
来源：http://3g.yfazqb.com/Article/details/geymkxnng.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.epnwcf.com/Article/details/gpmavyvhb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.epnwcf.com/Article/details/gscesyqut.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.tarul.cn/Article/details/gaxfbcaju.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.vehdjk.com/Article/details/gyosiyjyj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.yfazqb.com/Article/details/gtiurvdog.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.sjlbkw.cn/Article/details/gjybaqedy.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.vehdjk.com/Article/details/ghqmjkaom.sHtML

[H07] 断言
来源：http://blog.epnwcf.com/Article/details/gtzuiscos.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fktsv.cn/Article/details/gsswtxupj.sHtML

PHP:  assert($x > 0);
来源：http://baike.sjlbkw.cn/Article/details/grslnfnxq.sHtML

JS:   console.assert(x > 0);
来源：http://3g.epnwcf.com/Article/details/ghzwmilph.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.epnwcf.com/Article/details/gvpebwklg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.sjlbkw.cn/Article/details/geptbwbvb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fktsv.cn/Article/details/gbeiatkfd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.vehdjk.com/Article/details/gbbswkach.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.vehdjk.com/Article/details/gvohzsroh.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fktsv.cn/Article/details/gdawxhegj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.sjlbkw.cn/Article/details/gvbhjnvqc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.bbcook.cn/Article/details/gujpmasxy.sHtML

JS:   e.message;  e.stack
来源：http://baike.sjlbkw.cn/Article/details/gkgjctfxe.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.yfazqb.com/Article/details/grndoqumj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fktsv.cn/Article/details/grzevanec.sHtML

Go:   err.Error()
来源：http://www.m.share.fktsv.cn/Article/details/gwyhqcude.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fktsv.cn/Article/details/gaegeiagg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.epnwcf.com/Article/details/gxdofppfl.sHtML

[H09] 带错误码的异常
来源：http://m.share.vehdjk.com/Article/details/gbbhvksoo.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.sjlbkw.cn/Article/details/goanzmclm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.vehdjk.com/Article/details/gymkgklrh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.tarul.cn/Article/details/gcpmyyoqj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.epnwcf.com/Article/details/gavvdkwwe.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.vehdjk.com/Article/details/gdzohrdrb.sHtML


<!-- 参考信息 -->