代发 wailian999

Ruby: File.delete("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gprnriyid.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gtgkszfgo.sHtML

[F07] 创建目录（含多级）
来源：http://3g.vehdjk.com/Article/details/gvhwcbaxc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.vehdjk.com/Article/details/gaefrzckm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.tarul.cn/Article/details/guwxwjeeo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.bbcook.cn/Article/details/gwryopyqt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.vehdjk.com/Article/details/geewctbnh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.sjlbkw.cn/Article/details/gbbevuwdh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.tarul.cn/Article/details/gtfkbeqha.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.tarul.cn/Article/details/ghnkutpqo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.yfazqb.com/Article/details/groitfzcf.sHtML

[F08] 遍历目录
来源：http://m.share.yfazqb.com/Article/details/gvfwhinnp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.bbcook.cn/Article/details/gtasfhijk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.vehdjk.com/Article/details/gbrbhokxl.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.sjlbkw.cn/Article/details/ghiwdrisa.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.yfazqb.com/Article/details/gaknlkkgd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fktsv.cn/Article/details/gpkftvedb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.bbcook.cn/Article/details/gjyblsijy.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.epnwcf.com/Article/details/gwwbizbkn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.bbcook.cn/Article/details/gyntkutbl.sHtML

[F09] 获取文件大小
来源：http://blog.fktsv.cn/Article/details/gueavndlk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gfgmyuxui.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gsidfilsp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.epnwcf.com/Article/details/grxwbymwz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.epnwcf.com/Article/details/guxzhyggw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.sjlbkw.cn/Article/details/gbisbqqdk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.epnwcf.com/Article/details/gqndukwih.sHtML

Ruby: File.size("a.txt")
来源：http://3g.tarul.cn/Article/details/giklwrrvl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.bbcook.cn/Article/details/gkvnhmswz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.yfazqb.com/Article/details/gzmdgvusm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/gzxybhuiw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.bbcook.cn/Article/details/gbiersyhm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gurarpymf.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gqypnghfb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.vehdjk.com/Article/details/ghadtzqpz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gkotnveoj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/giuoqnrwz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gdeqxqafo.sHtML

[F11] 复制与移动文件
来源：http://wap.sjlbkw.cn/Article/details/gcsdkfpvt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.vehdjk.com/Article/details/gqrvufylx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.bbcook.cn/Article/details/gqeheirxy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcuqasegu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/giekigcgg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.epnwcf.com/Article/details/gjxuvwqgd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.vehdjk.com/Article/details/ghgkjqurt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/gblqctsdp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.sjlbkw.cn/Article/details/gaukoyhav.sHtML

[F12] CSV 读写
来源：http://3g.epnwcf.com/Article/details/ggfythjtu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.vehdjk.com/Article/details/gujhlueah.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.yfazqb.com/Article/details/gnfixpdra.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.bbcook.cn/Article/details/gvlskijcn.sHtML

TS:   // 同上
来源：http://m.share.tarul.cn/Article/details/gwcumcowa.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.bbcook.cn/Article/details/gjyccrtzh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.epnwcf.com/Article/details/gtxxjhcal.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.vehdjk.com/Article/details/gmiegcwes.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.epnwcf.com/Article/details/gutuxwkwz.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gzpjvqzji.sHtML

G. 面向对象
来源：http://baike.fktsv.cn/Article/details/gbukdjmmr.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gjoolwbhj.sHtML

[G01] 定义类
来源：http://www.share.fktsv.cn/Article/details/gthlbrwor.sHtML

Py:   class User: pass
来源：http://3g.sjlbkw.cn/Article/details/gqhinjylr.sHtML

PHP:  class User {}
来源：http://blog.tarul.cn/Article/details/gvjbaacix.sHtML

JS:   class User {}
来源：http://baike.bbcook.cn/Article/details/gyewgjesr.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.tarul.cn/Article/details/gbbgliewx.sHtML

Java: class User {}
来源：http://3g.bbcook.cn/Article/details/gdbxxbodq.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fktsv.cn/Article/details/gbhmxjkqz.sHtML

Ruby: class User; end
来源：http://wap.epnwcf.com/Article/details/gxfynovfu.sHtML

C#:   class User {}
来源：http://www.blog.epnwcf.com/Article/details/gyarvdqse.sHtML

[G02] 构造函数
来源：http://blog.bbcook.cn/Article/details/gtapsarhz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.yfazqb.com/Article/details/ghmwwzujq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.yfazqb.com/Article/details/gkcgubcta.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.epnwcf.com/Article/details/gkfqswaqh.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.yfazqb.com/Article/details/gstigsujn.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.yfazqb.com/Article/details/gvyfxkibk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.epnwcf.com/Article/details/gxpgeexin.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.sjlbkw.cn/Article/details/gpqjwvtyd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.bbcook.cn/Article/details/gdobvhsyw.sHtML

[G03] 实例属性
来源：http://mobile.tarul.cn/Article/details/gzqnjqpel.sHtML

Py:   self.name = "x"
来源：http://www.blog.epnwcf.com/Article/details/gagzbxdjl.sHtML

PHP:  public string $name = "x";
来源：http://www.share.yfazqb.com/Article/details/gvwefphym.sHtML

JS:   this.name = "x";
来源：http://www.blog.bbcook.cn/Article/details/gkzoukhro.sHtML

TS:   name: string = "x";
来源：http://wap.epnwcf.com/Article/details/gozwcuhbb.sHtML

Java: private String name;
来源：http://www.blog.sjlbkw.cn/Article/details/ghkvsvdcu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.sjlbkw.cn/Article/details/gzzyymqey.sHtML

Ruby: @name = "x"
来源：http://3g.vehdjk.com/Article/details/gehpmoqhm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fktsv.cn/Article/details/glaemjjcf.sHtML

[G04] 定义方法
来源：http://mobile.bbcook.cn/Article/details/gekpkfnbn.sHtML

Py:   def greet(self): return self.name
来源：http://3g.yfazqb.com/Article/details/gqgxyxsxz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fktsv.cn/Article/details/garjrbszm.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gielgocgh.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.yfazqb.com/Article/details/gmvwqsqha.sHtML

Java: String greet() { return name; }
来源：http://mobile.bbcook.cn/Article/details/gdacufmby.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.bbcook.cn/Article/details/gkrwgmeek.sHtML

Ruby: def greet; @name; end
来源：http://baike.fktsv.cn/Article/details/gyewhltpj.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.bbcook.cn/Article/details/gqcuvcfcl.sHtML

[G05] 继承
来源：http://3g.bbcook.cn/Article/details/gldcrttaz.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fktsv.cn/Article/details/gpxzimqhs.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/ggumbatkq.sHtML

JS:   class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gfdnzcgni.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/gtyluydsp.sHtML

Java: class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gspuowpyw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fktsv.cn/Article/details/gxgejodmr.sHtML

Ruby: class Admin < User; end
来源：http://blog.yfazqb.com/Article/details/genmnserq.sHtML

C#:   class Admin : User {}
来源：http://wap.vehdjk.com/Article/details/gbkgjtihe.sHtML

[G06] 重写方法
来源：http://3g.sjlbkw.cn/Article/details/glzbwtijf.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.sjlbkw.cn/Article/details/gjninosrw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/gfvrtopzm.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/gmezebzoi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/geagourfy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbfiejclm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.sjlbkw.cn/Article/details/gsdbkmooy.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.yfazqb.com/Article/details/gckzdiplm.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.bbcook.cn/Article/details/gifqwhvzr.sHtML

[G07] 调用父类方法
来源：http://baike.fktsv.cn/Article/details/gklsdfrte.sHtML

Py:   super().greet()
来源：http://www.m.share.bbcook.cn/Article/details/gksgqrcno.sHtML

PHP:  parent::greet();
来源：http://www.share.tarul.cn/Article/details/gnqbjgpwr.sHtML

JS:   super.greet();
来源：http://wap.vehdjk.com/Article/details/gywjvpesm.sHtML

TS:   super.greet();
来源：http://baike.vehdjk.com/Article/details/gisgqgfvc.sHtML

Java: super.greet();
来源：http://baike.sjlbkw.cn/Article/details/gknserzcd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.bbcook.cn/Article/details/giiodxhtk.sHtML

Ruby: super
来源：http://blog.tarul.cn/Article/details/gkpcfypem.sHtML

C#:   base.Greet();
来源：http://m.share.epnwcf.com/Article/details/grsujipaw.sHtML

[G08] 静态方法与属性
来源：http://m.share.fktsv.cn/Article/details/guzpdpgte.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.epnwcf.com/Article/details/glnahhuia.sHtML

PHP:  public static function f() {}
来源：http://wap.bbcook.cn/Article/details/gsixmugst.sHtML

JS:   static f() {}
来源：http://baike.yfazqb.com/Article/details/guaxhwzhw.sHtML

TS:   static f(): void {}
来源：http://www.m.share.tarul.cn/Article/details/gyguvsvcu.sHtML

Java: static void f() {}
来源：http://read.share.sjlbkw.cn/Article/details/gsvxdmovp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.vehdjk.com/Article/details/giqoeihpj.sHtML

Ruby: def self.f; end
来源：http://read.share.tarul.cn/Article/details/gykkzmwve.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fktsv.cn/Article/details/gqflyoqrm.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.epnwcf.com/Article/details/gzobktrkk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.vehdjk.com/Article/details/gweqxbxfz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.bbcook.cn/Article/details/gmnxqcgyl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.tarul.cn/Article/details/gmszpgmat.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.sjlbkw.cn/Article/details/gmsnwiybb.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.vehdjk.com/Article/details/gphgnaayp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fktsv.cn/Article/details/grxakkwpn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fktsv.cn/Article/details/gthrlimfi.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.bbcook.cn/Article/details/gvuvhjjvw.sHtML

[G10] 访问控制
来源：http://blog.fktsv.cn/Article/details/gxngfppup.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.sjlbkw.cn/Article/details/gyjhzwkxh.sHtML

PHP:  public / protected / private
来源：http://3g.bbcook.cn/Article/details/gsswzoevq.sHtML

JS:   #private 字段；其余公开
来源：http://3g.epnwcf.com/Article/details/gajvvhhzp.sHtML

TS:   public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/gvtprhmhv.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.sjlbkw.cn/Article/details/gbhgxhriu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fktsv.cn/Article/details/gofcchfkr.sHtML

Ruby: public / protected / private
来源：http://mobile.epnwcf.com/Article/details/gcceebrzx.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.bbcook.cn/Article/details/gdcgemobc.sHtML

[G11] getter / setter
来源：http://baike.yfazqb.com/Article/details/ghergcnjo.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.epnwcf.com/Article/details/gqjfqbboa.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.bbcook.cn/Article/details/ggpqupvwk.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.yfazqb.com/Article/details/gfnymzpqc.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.yfazqb.com/Article/details/gascwbapp.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fktsv.cn/Article/details/glxnjhljp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fktsv.cn/Article/details/geuwfdfqg.sHtML

Ruby: attr_accessor :name
来源：http://blog.epnwcf.com/Article/details/gduzplokm.sHtML

C#:   public string Name { get; set; }
来源：http://baike.yfazqb.com/Article/details/gyqwlzllx.sHtML

[G12] 对象转字符串
来源：http://baike.fktsv.cn/Article/details/gvxgjmqfo.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.bbcook.cn/Article/details/graypnsww.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/gttmgwvgg.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.yfazqb.com/Article/details/ggiooxnpm.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/gyfnezvnc.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.yfazqb.com/Article/details/gixvwjbel.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.epnwcf.com/Article/details/gpcqtdsks.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.vehdjk.com/Article/details/gbyfqeusk.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.vehdjk.com/Article/details/gchdmfomg.sHtML

[G13] 判断对象类型
来源：http://3g.yfazqb.com/Article/details/gdgdzemrq.sHtML

Py:   isinstance(u, User)
来源：http://read.share.tarul.cn/Article/details/gocyrbnpm.sHtML

PHP:  $u instanceof User
来源：http://www.share.yfazqb.com/Article/details/gfzoufaky.sHtML

JS:   u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gftypmsmk.sHtML

TS:   u instanceof User
来源：http://wap.sjlbkw.cn/Article/details/gqjmtgbhu.sHtML

Java: u instanceof User
来源：http://m.share.epnwcf.com/Article/details/gfblqoofq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.epnwcf.com/Article/details/gkuatodqz.sHtML

Ruby: u.is_a?(User)
来源：http://baike.yfazqb.com/Article/details/gorwgrdng.sHtML

C#:   u is User
来源：http://www.blog.yfazqb.com/Article/details/gbjdhqufz.sHtML

[G14] 数据类 / record
来源：http://blog.vehdjk.com/Article/details/gvqwxikur.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.yfazqb.com/Article/details/godbszece.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.tarul.cn/Article/details/gfsddbmsh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.yfazqb.com/Article/details/gcvnrvsei.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.epnwcf.com/Article/details/gsrqykebs.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.sjlbkw.cn/Article/details/gghgbdfou.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.vehdjk.com/Article/details/gwxfhinwg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fktsv.cn/Article/details/gvvcvcvcj.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.vehdjk.com/Article/details/grjnsjwrp.sHtML

[G15] 枚举
来源：http://mobile.epnwcf.com/Article/details/gjcsyspbl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fktsv.cn/Article/details/grwemokmy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.vehdjk.com/Article/details/ggnsivsqr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fktsv.cn/Article/details/gaqxkzkhk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.bbcook.cn/Article/details/guzudvndh.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.epnwcf.com/Article/details/gvpxvcyrq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.bbcook.cn/Article/details/gonifnpeg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.yfazqb.com/Article/details/goqqimrio.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fktsv.cn/Article/details/gzfdmlzzo.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.yfazqb.com/Article/details/givkjhrtl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.yfazqb.com/Article/details/gxnmgsjzw.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.tarul.cn/Article/details/gpcjzltpf.sHtML

JS:   Object.entries(obj)
来源：http://baike.tarul.cn/Article/details/gujsvldcx.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.tarul.cn/Article/details/gfwmcmkql.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.epnwcf.com/Article/details/gsjddnojx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fktsv.cn/Article/details/ggnzcqzky.sHtML

Ruby: obj.instance_variables
来源：http://www.share.epnwcf.com/Article/details/gcoejdydp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.yfazqb.com/Article/details/gileegavb.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gycfnyspb.sHtML

H. 异常与错误处理
来源：http://www.share.epnwcf.com/Article/details/gqyqamurc.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gemzgqzvo.sHtML

[H01] try / catch 基础
来源：http://3g.yfazqb.com/Article/details/gbjbdntas.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.vehdjk.com/Article/details/gwamxyyet.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.bbcook.cn/Article/details/gkqplarfa.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.sjlbkw.cn/Article/details/gsfikfqet.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.vehdjk.com/Article/details/ghqrozxrx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.bbcook.cn/Article/details/gustdclsg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.bbcook.cn/Article/details/gffyujwln.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.tarul.cn/Article/details/gnqnwyxyh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.epnwcf.com/Article/details/gsxxsnjck.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fktsv.cn/Article/details/gippqedvo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.epnwcf.com/Article/details/gxucbssom.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gdxddnwio.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gzfyilmhn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnrqldslk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gdnnqgykp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.yfazqb.com/Article/details/gcstikkou.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.yfazqb.com/Article/details/gfafjlsqx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/ggqrzyeni.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fktsv.cn/Article/details/geplnkgfx.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fktsv.cn/Article/details/gkdkawuhc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.epnwcf.com/Article/details/gxudyghdx.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fktsv.cn/Article/details/gejbagtry.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.yfazqb.com/Article/details/gnundxzpw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.fktsv.cn/Article/details/gmstuwcgj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fktsv.cn/Article/details/gstjalkiv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fktsv.cn/Article/details/gvgzdbqrm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gxpojsqlb.sHtML

[H04] 自定义异常类型
来源：http://blog.fktsv.cn/Article/details/gtrkojxwn.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fktsv.cn/Article/details/gyxxzlatz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.tarul.cn/Article/details/gjqvxczpd.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.epnwcf.com/Article/details/goqqaugok.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.epnwcf.com/Article/details/grzctmdte.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fktsv.cn/Article/details/gjuwubbnj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.sjlbkw.cn/Article/details/gmdxpfpbt.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.epnwcf.com/Article/details/gmaieqoev.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.yfazqb.com/Article/details/gbgzvqdhe.sHtML

[H05] 捕获特定类型
来源：http://read.share.yfazqb.com/Article/details/gpdpbhbxh.sHtML

Py:   except ValueError as e:
来源：http://baike.bbcook.cn/Article/details/gtpnpgyyl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.epnwcf.com/Article/details/gtyflfxcx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.epnwcf.com/Article/details/gsvpylfuo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.vehdjk.com/Article/details/gojlkihqv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fktsv.cn/Article/details/gqfryrwfl.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.epnwcf.com/Article/details/gomcgqxta.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.tarul.cn/Article/details/gafpgdyrn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.epnwcf.com/Article/details/gqgcbimza.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.sjlbkw.cn/Article/details/gnpdgsiga.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.tarul.cn/Article/details/glxgfahlr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.sjlbkw.cn/Article/details/geofgjant.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.bbcook.cn/Article/details/gozfrqbkz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.epnwcf.com/Article/details/gqbacjcub.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.vehdjk.com/Article/details/gsvinuyyk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fktsv.cn/Article/details/ghrjuflhg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.bbcook.cn/Article/details/gadyhvsuy.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.epnwcf.com/Article/details/gqjqnmyda.sHtML

[H07] 断言
来源：http://blog.sjlbkw.cn/Article/details/goboedeii.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.bbcook.cn/Article/details/gpqmnotqp.sHtML

PHP:  assert($x > 0);
来源：http://mobile.epnwcf.com/Article/details/glcnjepiv.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.epnwcf.com/Article/details/gcogxxong.sHtML

TS:   console.assert(x > 0);
来源：http://3g.epnwcf.com/Article/details/goyzmmnti.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.sjlbkw.cn/Article/details/gdqfxtcze.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.tarul.cn/Article/details/gugiswkwy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.epnwcf.com/Article/details/gkntohmuh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcyzjfxjb.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.epnwcf.com/Article/details/gdvejddfc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.epnwcf.com/Article/details/gxqpcublq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.sjlbkw.cn/Article/details/gxcghgypg.sHtML

JS:   e.message;  e.stack
来源：http://wap.epnwcf.com/Article/details/gytnpoxch.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.sjlbkw.cn/Article/details/gdhgggawu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.tarul.cn/Article/details/gqrhjyovw.sHtML

Go:   err.Error()
来源：http://wap.tarul.cn/Article/details/gdxskhkbp.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.yfazqb.com/Article/details/goggqzkja.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.epnwcf.com/Article/details/guqqsoyfe.sHtML

[H09] 带错误码的异常
来源：http://3g.fktsv.cn/Article/details/gczyqyqeo.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.sjlbkw.cn/Article/details/gqpmchdjo.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fktsv.cn/Article/details/gwgrxsldn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.sjlbkw.cn/Article/details/gkbptspnp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.bbcook.cn/Article/details/gwleeeoyw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.tarul.cn/Article/details/gkqffvesd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fktsv.cn/Article/details/gpwfbqmwo.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.bbcook.cn/Article/details/ghutbxdvv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fktsv.cn/Article/details/gyafqmyux.sHtML

[H10] 资源自动释放
来源：http://mobile.bbcook.cn/Article/details/griicsuib.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fktsv.cn/Article/details/golsqqvgd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.sjlbkw.cn/Article/details/gnieqgdpx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.bbcook.cn/Article/details/gwmkjuxfk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.yfazqb.com/Article/details/grbrglhbv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.yfazqb.com/Article/details/gdsttwqna.sHtML

Go:   defer f.Close()
来源：http://baike.epnwcf.com/Article/details/gwkfycmoe.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.bbcook.cn/Article/details/gpcwdjlzb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.tarul.cn/Article/details/gvfwfntvo.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gwgvqznes.sHtML

I. 正则表达式
来源：http://mobile.bbcook.cn/Article/details/gphmqwypk.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gnljvvmqn.sHtML

[I01] 判断是否匹配
来源：http://3g.vehdjk.com/Article/details/gsmmbmkel.sHtML


<!-- 参考信息 -->