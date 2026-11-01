代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/ggcxyektm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.vehdjk.com/Article/details/guibbfcqx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/gxsgmjcus.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.bbcook.cn/Article/details/gegtsdegk.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.epnwcf.com/Article/details/givgcyfsm.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.vehdjk.com/Article/details/gpplygrcs.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fktsv.cn/Article/details/gigdmovpz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.tarul.cn/Article/details/gavfjvqgx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fktsv.cn/Article/details/gvyzjvysz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fktsv.cn/Article/details/gehncmqre.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.epnwcf.com/Article/details/gnevoezyf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.yfazqb.com/Article/details/gpfrfdnmp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.tarul.cn/Article/details/gbmgoesbt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.vehdjk.com/Article/details/gnsedukai.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.epnwcf.com/Article/details/guwlsbotu.sHtML

[F08] 遍历目录
来源：http://m.share.sjlbkw.cn/Article/details/ggibynwsi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.tarul.cn/Article/details/gkthikcux.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.sjlbkw.cn/Article/details/gpgxsxwzj.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.tarul.cn/Article/details/giosobhig.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.sjlbkw.cn/Article/details/gifgmgrvu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.tarul.cn/Article/details/gsftuegsx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.bbcook.cn/Article/details/ghvaoqror.sHtML

Ruby: Dir.children("dir")
来源：http://baike.yfazqb.com/Article/details/glnadkpyk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbuhvgwe.sHtML

[F09] 获取文件大小
来源：http://blog.bbcook.cn/Article/details/gnyrwzxmp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.yfazqb.com/Article/details/guiddgtej.sHtML

PHP:  filesize("a.txt");
来源：http://baike.tarul.cn/Article/details/gzugpmrww.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.bbcook.cn/Article/details/gavgwtfws.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.sjlbkw.cn/Article/details/gpheeqptl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.bbcook.cn/Article/details/gtqjnrwfr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.yfazqb.com/Article/details/gobxjlmeg.sHtML

Ruby: File.size("a.txt")
来源：http://blog.yfazqb.com/Article/details/gvvylcxwg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.yfazqb.com/Article/details/gnlsukwga.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.yfazqb.com/Article/details/ggqswznzm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/goomygmwu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.vehdjk.com/Article/details/gcjrdgagt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gflyndljp.sHtML

TS:   path.extname("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gsqcrhkvu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.sjlbkw.cn/Article/details/gpcxfrvdu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/gbwlrxhur.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gsublicrj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gconlhfhc.sHtML

[F11] 复制与移动文件
来源：http://www.share.tarul.cn/Article/details/gginbdzsn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gswhzdvcj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.vehdjk.com/Article/details/gwheaqneq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/glhtypzxv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gucsxwszh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.epnwcf.com/Article/details/gfehaypnh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.vehdjk.com/Article/details/gjclphgxd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.sjlbkw.cn/Article/details/goromvhsa.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.sjlbkw.cn/Article/details/goqrzetns.sHtML

[F12] CSV 读写
来源：http://www.share.yfazqb.com/Article/details/gdzvfkomh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.bbcook.cn/Article/details/gdktwipjv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.tarul.cn/Article/details/gjpfijxis.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.sjlbkw.cn/Article/details/gycgqycmx.sHtML

TS:   // 同上
来源：http://3g.tarul.cn/Article/details/glgyqfwej.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fktsv.cn/Article/details/gvvxpnzdm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.tarul.cn/Article/details/gvejncrvp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.bbcook.cn/Article/details/gjgkijwiu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.sjlbkw.cn/Article/details/gxowsxdoi.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/grkzirocv.sHtML

G. 面向对象
来源：http://www.share.vehdjk.com/Article/details/gfxwspcuv.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gutqgenjg.sHtML

[G01] 定义类
来源：http://read.share.tarul.cn/Article/details/getdbdvwr.sHtML

Py:   class User: pass
来源：http://mobile.sjlbkw.cn/Article/details/giyefeypv.sHtML

PHP:  class User {}
来源：http://www.share.bbcook.cn/Article/details/gamufkywu.sHtML

JS:   class User {}
来源：http://baike.vehdjk.com/Article/details/gwwhchslr.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.epnwcf.com/Article/details/ggjxhasci.sHtML

Java: class User {}
来源：http://read.share.yfazqb.com/Article/details/gyzntxmvj.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.yfazqb.com/Article/details/gmsgjavsw.sHtML

Ruby: class User; end
来源：http://wap.epnwcf.com/Article/details/gbmqmmumh.sHtML

C#:   class User {}
来源：http://m.share.fktsv.cn/Article/details/gxnfcogoe.sHtML

[G02] 构造函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gmdgujjxo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.bbcook.cn/Article/details/gpgvruzwq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.epnwcf.com/Article/details/gpuexpihc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fktsv.cn/Article/details/gsrxaopvf.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fktsv.cn/Article/details/gwfcppuia.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.vehdjk.com/Article/details/gohcxmnzx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.yfazqb.com/Article/details/gqsopmnst.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.bbcook.cn/Article/details/gonndskxe.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.bbcook.cn/Article/details/gtgavexbw.sHtML

[G03] 实例属性
来源：http://3g.fktsv.cn/Article/details/gzndtfqrk.sHtML

Py:   self.name = "x"
来源：http://wap.tarul.cn/Article/details/gcoromuuc.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fktsv.cn/Article/details/gtycilubs.sHtML

JS:   this.name = "x";
来源：http://mobile.vehdjk.com/Article/details/gsjzilqbh.sHtML

TS:   name: string = "x";
来源：http://www.blog.bbcook.cn/Article/details/grslrbcch.sHtML

Java: private String name;
来源：http://www.m.share.yfazqb.com/Article/details/gpzvmyoxe.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.tarul.cn/Article/details/gzawsttll.sHtML

Ruby: @name = "x"
来源：http://mobile.epnwcf.com/Article/details/ghyzatazb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.bbcook.cn/Article/details/grlztosyx.sHtML

[G04] 定义方法
来源：http://m.share.fktsv.cn/Article/details/gykxzeaci.sHtML

Py:   def greet(self): return self.name
来源：http://baike.bbcook.cn/Article/details/gunqglner.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.bbcook.cn/Article/details/gwmsyfmgj.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/gyicrdjek.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.tarul.cn/Article/details/gjxixoima.sHtML

Java: String greet() { return name; }
来源：http://read.share.epnwcf.com/Article/details/gbjmomzda.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.vehdjk.com/Article/details/gyosvnweo.sHtML

Ruby: def greet; @name; end
来源：http://3g.tarul.cn/Article/details/gfinpuqmp.sHtML

C#:   public string Greet() => Name;
来源：http://wap.vehdjk.com/Article/details/grngxumhz.sHtML

[G05] 继承
来源：http://mobile.sjlbkw.cn/Article/details/gitbghapk.sHtML

Py:   class Admin(User): pass
来源：http://read.share.epnwcf.com/Article/details/gydngxjen.sHtML

PHP:  class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/gqrfncpar.sHtML

JS:   class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/ghpooobxc.sHtML

TS:   class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/gchnzhhyt.sHtML

Java: class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/gfisnbbqs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.yfazqb.com/Article/details/gpnlkrarx.sHtML

Ruby: class Admin < User; end
来源：http://wap.vehdjk.com/Article/details/grckhgxbk.sHtML

C#:   class Admin : User {}
来源：http://baike.bbcook.cn/Article/details/gjvleftjg.sHtML

[G06] 重写方法
来源：http://wap.vehdjk.com/Article/details/gsbdrncgh.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.bbcook.cn/Article/details/gyixvctfv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fktsv.cn/Article/details/geagtjxbj.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/gxuzgqrin.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gdcpnqjar.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/gsrkssqhe.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.epnwcf.com/Article/details/gphzdvolh.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.epnwcf.com/Article/details/gxmtbdrri.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.tarul.cn/Article/details/gbhuhbgns.sHtML

[G07] 调用父类方法
来源：http://www.m.share.bbcook.cn/Article/details/gaaqanvmp.sHtML

Py:   super().greet()
来源：http://read.share.sjlbkw.cn/Article/details/gdbupbzgs.sHtML

PHP:  parent::greet();
来源：http://baike.yfazqb.com/Article/details/gkynunmlk.sHtML

JS:   super.greet();
来源：http://m.share.sjlbkw.cn/Article/details/gaoiroyec.sHtML

TS:   super.greet();
来源：http://mobile.epnwcf.com/Article/details/gntgxpruv.sHtML

Java: super.greet();
来源：http://wap.epnwcf.com/Article/details/gfkcohcco.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fktsv.cn/Article/details/gornrdgqw.sHtML

Ruby: super
来源：http://m.share.fktsv.cn/Article/details/gabanbupu.sHtML

C#:   base.Greet();
来源：http://blog.bbcook.cn/Article/details/gguyyajnx.sHtML

[G08] 静态方法与属性
来源：http://wap.sjlbkw.cn/Article/details/growyqlze.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.tarul.cn/Article/details/gsbomvknn.sHtML

PHP:  public static function f() {}
来源：http://www.blog.sjlbkw.cn/Article/details/gqjqiibjh.sHtML

JS:   static f() {}
来源：http://blog.vehdjk.com/Article/details/ghbfrchku.sHtML

TS:   static f(): void {}
来源：http://blog.sjlbkw.cn/Article/details/gxyihlmmy.sHtML

Java: static void f() {}
来源：http://blog.tarul.cn/Article/details/ggrpebqcz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fktsv.cn/Article/details/gvsxpjkam.sHtML

Ruby: def self.f; end
来源：http://www.m.share.bbcook.cn/Article/details/gfgtrdxrs.sHtML

C#:   public static void F() {}
来源：http://read.share.fktsv.cn/Article/details/gdtznkamn.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.sjlbkw.cn/Article/details/gzqtuivrt.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.sjlbkw.cn/Article/details/gmrmnppxk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.sjlbkw.cn/Article/details/gvpgvmdvb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.epnwcf.com/Article/details/galnckmau.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.vehdjk.com/Article/details/gaevwjzop.sHtML

Java: interface Shape { double area(); }
来源：http://wap.tarul.cn/Article/details/gcsupclwy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.vehdjk.com/Article/details/gxgurgnvl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.bbcook.cn/Article/details/gvmbvmquc.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fktsv.cn/Article/details/ghfghoops.sHtML

[G10] 访问控制
来源：http://m.share.vehdjk.com/Article/details/gktlnetiq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.tarul.cn/Article/details/gonxqgnxo.sHtML

PHP:  public / protected / private
来源：http://www.share.epnwcf.com/Article/details/gthcnulkx.sHtML

JS:   #private 字段；其余公开
来源：http://3g.tarul.cn/Article/details/grxffyqea.sHtML

TS:   public / protected / private
来源：http://blog.sjlbkw.cn/Article/details/guepuqgtd.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fktsv.cn/Article/details/gauilvimp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.sjlbkw.cn/Article/details/gaxowkkdf.sHtML

Ruby: public / protected / private
来源：http://baike.bbcook.cn/Article/details/gbipkxmnf.sHtML

C#:   public / protected / private / internal
来源：http://mobile.yfazqb.com/Article/details/gngjihuif.sHtML

[G11] getter / setter
来源：http://mobile.vehdjk.com/Article/details/ggobmrvbl.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.tarul.cn/Article/details/gtkgxbsaw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.tarul.cn/Article/details/gipsxhzdr.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.epnwcf.com/Article/details/gsuwauaqf.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.tarul.cn/Article/details/gkjoqlmql.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gzhzkbbvh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.sjlbkw.cn/Article/details/giwhdgvwe.sHtML

Ruby: attr_accessor :name
来源：http://3g.yfazqb.com/Article/details/gyxmqzouk.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.epnwcf.com/Article/details/gtoqgsrfj.sHtML

[G12] 对象转字符串
来源：http://wap.vehdjk.com/Article/details/gikvatdtq.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.epnwcf.com/Article/details/gkgtpazhz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.yfazqb.com/Article/details/gscyhzdsy.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gwaelbvhd.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.vehdjk.com/Article/details/grgyktbrp.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.tarul.cn/Article/details/gujbcocxx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.bbcook.cn/Article/details/glpnurkcn.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.epnwcf.com/Article/details/gddvslxok.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.bbcook.cn/Article/details/ggfbyxpez.sHtML

[G13] 判断对象类型
来源：http://www.m.share.yfazqb.com/Article/details/gkwlratoj.sHtML

Py:   isinstance(u, User)
来源：http://wap.sjlbkw.cn/Article/details/gicalxabk.sHtML

PHP:  $u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/gqzcntzgf.sHtML

JS:   u instanceof User
来源：http://baike.epnwcf.com/Article/details/gcbtzlyst.sHtML

TS:   u instanceof User
来源：http://m.share.bbcook.cn/Article/details/guyhaonlu.sHtML

Java: u instanceof User
来源：http://m.share.bbcook.cn/Article/details/gpfvxzuvy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.tarul.cn/Article/details/gswtagnyz.sHtML

Ruby: u.is_a?(User)
来源：http://baike.sjlbkw.cn/Article/details/gtykvhybb.sHtML

C#:   u is User
来源：http://blog.bbcook.cn/Article/details/gosylrtpq.sHtML

[G14] 数据类 / record
来源：http://3g.tarul.cn/Article/details/gbenbdyzg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.sjlbkw.cn/Article/details/gzvnhlqqm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fktsv.cn/Article/details/gqaetsznl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.vehdjk.com/Article/details/gcspzlrzt.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.sjlbkw.cn/Article/details/gkunmomvm.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.yfazqb.com/Article/details/gakfdfrik.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.yfazqb.com/Article/details/gzyxytryb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.bbcook.cn/Article/details/gkbvvaewh.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.yfazqb.com/Article/details/grovucrcx.sHtML

[G15] 枚举
来源：http://www.m.share.tarul.cn/Article/details/gxepkirsh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.bbcook.cn/Article/details/gqljshnpq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.bbcook.cn/Article/details/gmldvgdor.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.epnwcf.com/Article/details/guwinrzxf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.bbcook.cn/Article/details/gbcusvtlt.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.epnwcf.com/Article/details/gfqrldxru.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.yfazqb.com/Article/details/gnotoezgj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.epnwcf.com/Article/details/guouwwdup.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.yfazqb.com/Article/details/gpzgtedft.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.sjlbkw.cn/Article/details/gqsyljcrc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.bbcook.cn/Article/details/gganouevk.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.sjlbkw.cn/Article/details/gmzzojolc.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqfpeisjh.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gtwxzzjol.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fktsv.cn/Article/details/gyczphlbu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.epnwcf.com/Article/details/gwphsceod.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.tarul.cn/Article/details/gzovvhgny.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.sjlbkw.cn/Article/details/gdhjrtaxr.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gkxolvdfi.sHtML

H. 异常与错误处理
来源：http://www.blog.bbcook.cn/Article/details/glllquywm.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gqqccykuo.sHtML

[H01] try / catch 基础
来源：http://www.blog.tarul.cn/Article/details/guxbgqifx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.epnwcf.com/Article/details/gpcnfgjdc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.yfazqb.com/Article/details/gqfdrdlgu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.vehdjk.com/Article/details/gnpuhrgmh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fktsv.cn/Article/details/gltzikuno.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.yfazqb.com/Article/details/ggdjhmhza.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.bbcook.cn/Article/details/gdasngoce.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.tarul.cn/Article/details/gdsphdgxj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.vehdjk.com/Article/details/ghxtemrjw.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.bbcook.cn/Article/details/gsicgemoy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.tarul.cn/Article/details/gskgtgqab.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gukloeiic.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gkwnheqdc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gxzizkblg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/grcuostvb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.bbcook.cn/Article/details/girwmmlbl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.epnwcf.com/Article/details/ginjlxjfe.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gzulzsqti.sHtML

[H03] 主动抛出异常
来源：http://www.share.vehdjk.com/Article/details/gkggrwknk.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.sjlbkw.cn/Article/details/geweuwezz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/gqqdunkbx.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/gdlrgtgpo.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fktsv.cn/Article/details/gkbvnloyh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gsbvxnxsu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.bbcook.cn/Article/details/gdeeomxwj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.vehdjk.com/Article/details/gxslkttgv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gpcnjroso.sHtML

[H04] 自定义异常类型
来源：http://www.share.vehdjk.com/Article/details/ghtowrpkp.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.yfazqb.com/Article/details/gsddxdbpd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.epnwcf.com/Article/details/gyicngdfk.sHtML

JS:   class MyError extends Error {}
来源：http://wap.tarul.cn/Article/details/gjwcfnaau.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.epnwcf.com/Article/details/gqigrvlvr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.tarul.cn/Article/details/ggudidntu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.yfazqb.com/Article/details/gawpsahwu.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.epnwcf.com/Article/details/gxdalpmwe.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqpvwtid.sHtML

[H05] 捕获特定类型
来源：http://m.share.fktsv.cn/Article/details/gojhvljtt.sHtML

Py:   except ValueError as e:
来源：http://read.share.sjlbkw.cn/Article/details/gzxhsolba.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.yfazqb.com/Article/details/gmtvltvfx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/ggjsgzyzp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/grakxifdw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fktsv.cn/Article/details/gdnundyzf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.vehdjk.com/Article/details/goenwlftd.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.yfazqb.com/Article/details/gqytbkrxr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.bbcook.cn/Article/details/ghrlourui.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.epnwcf.com/Article/details/gnxpqygld.sHtML

Py:   value = d.get("k") or default
来源：http://3g.sjlbkw.cn/Article/details/gdbxjtiai.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.epnwcf.com/Article/details/gibazbkof.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.epnwcf.com/Article/details/grdrimxlx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.epnwcf.com/Article/details/gfrwmgakd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.epnwcf.com/Article/details/gkwewgrza.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.bbcook.cn/Article/details/gisgxyanb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.tarul.cn/Article/details/gskjevlfl.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.epnwcf.com/Article/details/gykmljtmf.sHtML

[H07] 断言
来源：http://baike.fktsv.cn/Article/details/gxrvefhei.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.vehdjk.com/Article/details/gaverkcvr.sHtML

PHP:  assert($x > 0);
来源：http://read.share.epnwcf.com/Article/details/ghybsafhi.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.sjlbkw.cn/Article/details/gsdzgazma.sHtML

TS:   console.assert(x > 0);
来源：http://blog.epnwcf.com/Article/details/gzuveykts.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.sjlbkw.cn/Article/details/gahebmarb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.sjlbkw.cn/Article/details/gidsirddd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.bbcook.cn/Article/details/guylkfyiq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.yfazqb.com/Article/details/gyonlreeh.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.epnwcf.com/Article/details/gnnigkclu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.vehdjk.com/Article/details/gvjslfyai.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.epnwcf.com/Article/details/gfstvfwwg.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.sjlbkw.cn/Article/details/gzegszkib.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.sjlbkw.cn/Article/details/gdjgpcgcl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.yfazqb.com/Article/details/gbdgedcxj.sHtML

Go:   err.Error()
来源：http://m.share.epnwcf.com/Article/details/gzxjlfmiu.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fktsv.cn/Article/details/ghawnjkmm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.tarul.cn/Article/details/gtnxoyuue.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fktsv.cn/Article/details/gakdibcit.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.epnwcf.com/Article/details/geiezvdsa.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.yfazqb.com/Article/details/gdktkzvft.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.epnwcf.com/Article/details/gcodqfuvy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.vehdjk.com/Article/details/gvzkhthfi.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.epnwcf.com/Article/details/gmevjdqzm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.epnwcf.com/Article/details/geouykjgl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.bbcook.cn/Article/details/gilflvdcz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fktsv.cn/Article/details/gwngidakb.sHtML

[H10] 资源自动释放
来源：http://read.share.sjlbkw.cn/Article/details/gexrbajfu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.tarul.cn/Article/details/gfadvvocl.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.yfazqb.com/Article/details/gnudztanx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.tarul.cn/Article/details/gutkyanpm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fktsv.cn/Article/details/gmvpkegch.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.yfazqb.com/Article/details/grlsvhohe.sHtML

Go:   defer f.Close()
来源：http://wap.fktsv.cn/Article/details/geakolefd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.tarul.cn/Article/details/gncadyvex.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.yfazqb.com/Article/details/gwfwqhaaj.sHtML


<!-- 参考信息 -->