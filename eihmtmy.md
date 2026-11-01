代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/gjztohsgc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/gmwnquzcx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.epnwcf.com/Article/details/ghltzjwax.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gnbttqosj.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gymgddkfi.sHtML

[F06] 删除文件
来源：http://www.share.fktsv.cn/Article/details/gmqssxbrk.sHtML

Py:   os.remove("a.txt")
来源：http://baike.yfazqb.com/Article/details/gcrkjlany.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gubuhipzi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/gnedshcsx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/goerhhyel.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fktsv.cn/Article/details/gfevxmaut.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gjdrmiryl.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.tarul.cn/Article/details/gtdbbmtuu.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gtkdhcdsp.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.bbcook.cn/Article/details/gmerggriv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.bbcook.cn/Article/details/gpyyksswz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.bbcook.cn/Article/details/gfriytrtl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fktsv.cn/Article/details/gvpeuthgr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fktsv.cn/Article/details/gmxulechi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.bbcook.cn/Article/details/grczjgswo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.vehdjk.com/Article/details/gqyzmegun.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fktsv.cn/Article/details/gzoknoivt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fktsv.cn/Article/details/givbzqmzc.sHtML

[F08] 遍历目录
来源：http://www.share.epnwcf.com/Article/details/grshjnnsb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.bbcook.cn/Article/details/giqjmkpum.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.yfazqb.com/Article/details/gxyxynjxu.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.tarul.cn/Article/details/ggquptnvt.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fktsv.cn/Article/details/gxzsalorb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fktsv.cn/Article/details/gdckuuzcz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fktsv.cn/Article/details/glgfmndfd.sHtML

Ruby: Dir.children("dir")
来源：http://blog.bbcook.cn/Article/details/gckyitjsd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.yfazqb.com/Article/details/gtcankzbg.sHtML

[F09] 获取文件大小
来源：http://baike.vehdjk.com/Article/details/gpnmjonzn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.bbcook.cn/Article/details/gtwdhtjsi.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gtbooklzp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.yfazqb.com/Article/details/godttmnwq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.vehdjk.com/Article/details/gfplgckeh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fktsv.cn/Article/details/grlgiewsd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.yfazqb.com/Article/details/gaiylunyf.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.tarul.cn/Article/details/ghswxrfmy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.sjlbkw.cn/Article/details/gxqeugwgy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.vehdjk.com/Article/details/gghuoadbd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gadrzakuk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.epnwcf.com/Article/details/grmwjipck.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/gnbczxesd.sHtML

TS:   path.extname("a.txt")
来源：http://baike.yfazqb.com/Article/details/gemeajawy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.tarul.cn/Article/details/guvontzcj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gjtutxqws.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gtorcbylh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/ghnbvqife.sHtML

[F11] 复制与移动文件
来源：http://read.share.tarul.cn/Article/details/gmlgysyhy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/gtcwenkgs.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fktsv.cn/Article/details/ggboaceos.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/gwgiggnbc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/gxdldoany.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.vehdjk.com/Article/details/gcgjtpdke.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.vehdjk.com/Article/details/gkbtyluyh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gvzuxwxna.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.yfazqb.com/Article/details/gxibeshfc.sHtML

[F12] CSV 读写
来源：http://www.blog.vehdjk.com/Article/details/ghccvqkhd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.yfazqb.com/Article/details/gbhsnxgcr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.yfazqb.com/Article/details/glzvvofhr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.epnwcf.com/Article/details/gehpqqjzq.sHtML

TS:   // 同上
来源：http://read.share.tarul.cn/Article/details/gskcisspu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.sjlbkw.cn/Article/details/gfjjnnnvq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.yfazqb.com/Article/details/gqxynixye.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fktsv.cn/Article/details/gpfpmdadl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fktsv.cn/Article/details/gkitlwoco.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/ggahsotnb.sHtML

G. 面向对象
来源：http://www.blog.yfazqb.com/Article/details/gnofkcpng.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gxpiyzrcn.sHtML

[G01] 定义类
来源：http://3g.vehdjk.com/Article/details/gudwstugv.sHtML

Py:   class User: pass
来源：http://blog.fktsv.cn/Article/details/gxxaqplgz.sHtML

PHP:  class User {}
来源：http://m.share.tarul.cn/Article/details/gzvcagzuj.sHtML

JS:   class User {}
来源：http://blog.epnwcf.com/Article/details/gvtmqnlww.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.epnwcf.com/Article/details/gramljeer.sHtML

Java: class User {}
来源：http://read.share.yfazqb.com/Article/details/gxbgpbsfu.sHtML

Go:   type User struct { Name string }
来源：http://read.share.yfazqb.com/Article/details/ghhafftjk.sHtML

Ruby: class User; end
来源：http://www.share.epnwcf.com/Article/details/ghhtiidxl.sHtML

C#:   class User {}
来源：http://read.share.vehdjk.com/Article/details/gqdpzztom.sHtML

[G02] 构造函数
来源：http://www.m.share.vehdjk.com/Article/details/godbxxmqs.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.sjlbkw.cn/Article/details/gcgaqmfqd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.yfazqb.com/Article/details/gihzkukzq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.tarul.cn/Article/details/glxzklqnq.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.epnwcf.com/Article/details/gsgxfboml.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.sjlbkw.cn/Article/details/gwigcreye.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.sjlbkw.cn/Article/details/ghxjovjfu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.yfazqb.com/Article/details/gfhflfpoe.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.vehdjk.com/Article/details/gsezmvoot.sHtML

[G03] 实例属性
来源：http://www.blog.fktsv.cn/Article/details/gamrpuiys.sHtML

Py:   self.name = "x"
来源：http://www.blog.epnwcf.com/Article/details/gynzwljig.sHtML

PHP:  public string $name = "x";
来源：http://baike.epnwcf.com/Article/details/guhugwyux.sHtML

JS:   this.name = "x";
来源：http://mobile.bbcook.cn/Article/details/guujwjavg.sHtML

TS:   name: string = "x";
来源：http://blog.yfazqb.com/Article/details/gwsuskoqb.sHtML

Java: private String name;
来源：http://3g.vehdjk.com/Article/details/gbnjrozqj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.sjlbkw.cn/Article/details/ghucsqfuh.sHtML

Ruby: @name = "x"
来源：http://blog.sjlbkw.cn/Article/details/gxkrvbuec.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gbnwwissm.sHtML

[G04] 定义方法
来源：http://www.blog.yfazqb.com/Article/details/gflwgrfxu.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.sjlbkw.cn/Article/details/gljceuopo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/gzienygxt.sHtML

JS:   greet() { return this.name; }
来源：http://3g.tarul.cn/Article/details/gholmgqvi.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gzoeojmdc.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gffgjdrct.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.bbcook.cn/Article/details/ggmnvlhcu.sHtML

Ruby: def greet; @name; end
来源：http://www.share.vehdjk.com/Article/details/glmxficem.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.yfazqb.com/Article/details/gwhoaqdkq.sHtML

[G05] 继承
来源：http://www.share.yfazqb.com/Article/details/glbwdtkvk.sHtML

Py:   class Admin(User): pass
来源：http://wap.yfazqb.com/Article/details/gmtoemynh.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/gadicbvlf.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/gtlwcdbfn.sHtML

TS:   class Admin extends User {}
来源：http://m.share.epnwcf.com/Article/details/gktngaxqa.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/guiqehmpy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fktsv.cn/Article/details/goumzjpwi.sHtML

Ruby: class Admin < User; end
来源：http://read.share.yfazqb.com/Article/details/gvttmngcv.sHtML

C#:   class Admin : User {}
来源：http://3g.vehdjk.com/Article/details/gmxdzzywm.sHtML

[G06] 重写方法
来源：http://mobile.fktsv.cn/Article/details/gbpvfityn.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.vehdjk.com/Article/details/grzlbstew.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gywmuyewl.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fktsv.cn/Article/details/gabaafckc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/gxoobhzby.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/gskdpvggg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.bbcook.cn/Article/details/gabiwbqgv.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.vehdjk.com/Article/details/gpsxwnagf.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.vehdjk.com/Article/details/gixrhfypi.sHtML

[G07] 调用父类方法
来源：http://mobile.bbcook.cn/Article/details/grwwmtisy.sHtML

Py:   super().greet()
来源：http://mobile.tarul.cn/Article/details/gjwutyvtx.sHtML

PHP:  parent::greet();
来源：http://wap.tarul.cn/Article/details/gjyytogil.sHtML

JS:   super.greet();
来源：http://blog.sjlbkw.cn/Article/details/ggnoqpomy.sHtML

TS:   super.greet();
来源：http://www.m.share.epnwcf.com/Article/details/gxogooaex.sHtML

Java: super.greet();
来源：http://3g.epnwcf.com/Article/details/gdwucfxdj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.yfazqb.com/Article/details/gcscwdtpz.sHtML

Ruby: super
来源：http://3g.yfazqb.com/Article/details/gwpwsfouu.sHtML

C#:   base.Greet();
来源：http://blog.epnwcf.com/Article/details/gyguondhy.sHtML

[G08] 静态方法与属性
来源：http://wap.vehdjk.com/Article/details/gorjbhpnd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.epnwcf.com/Article/details/gjiwdldzg.sHtML

PHP:  public static function f() {}
来源：http://www.share.sjlbkw.cn/Article/details/gimifaaqm.sHtML

JS:   static f() {}
来源：http://read.share.vehdjk.com/Article/details/gnptqotrw.sHtML

TS:   static f(): void {}
来源：http://baike.yfazqb.com/Article/details/gmgpzivgm.sHtML

Java: static void f() {}
来源：http://www.m.share.epnwcf.com/Article/details/gmtywmhzg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.epnwcf.com/Article/details/gdjazwqny.sHtML

Ruby: def self.f; end
来源：http://www.share.yfazqb.com/Article/details/gctimvmmr.sHtML

C#:   public static void F() {}
来源：http://baike.epnwcf.com/Article/details/ggjbuwgsr.sHtML

[G09] 接口 / 抽象类
来源：http://wap.epnwcf.com/Article/details/gyfjtsodv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.sjlbkw.cn/Article/details/gymiderwz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.yfazqb.com/Article/details/gzujysvxv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvewxluk.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.bbcook.cn/Article/details/gfjmkfefm.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fktsv.cn/Article/details/gxyqojlal.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.bbcook.cn/Article/details/gkdsiubxy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.bbcook.cn/Article/details/gcbaifshw.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.epnwcf.com/Article/details/gznlvplxg.sHtML

[G10] 访问控制
来源：http://www.blog.tarul.cn/Article/details/gxohupune.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.epnwcf.com/Article/details/ggilvfcwc.sHtML

PHP:  public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/gyozqzymz.sHtML

JS:   #private 字段；其余公开
来源：http://3g.yfazqb.com/Article/details/gepovizgf.sHtML

TS:   public / protected / private
来源：http://www.m.share.vehdjk.com/Article/details/gsspiedpl.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.tarul.cn/Article/details/guebprvyq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.yfazqb.com/Article/details/gihthhzfm.sHtML

Ruby: public / protected / private
来源：http://baike.yfazqb.com/Article/details/gnrxazfnu.sHtML

C#:   public / protected / private / internal
来源：http://3g.yfazqb.com/Article/details/gkkzytrrl.sHtML

[G11] getter / setter
来源：http://3g.epnwcf.com/Article/details/gxbjoiqql.sHtML

Py:   @property 与 @x.setter
来源：http://baike.yfazqb.com/Article/details/ggkhhbquk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.tarul.cn/Article/details/gcmfynlme.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.vehdjk.com/Article/details/gepjfzeou.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.bbcook.cn/Article/details/goqvgziai.sHtML

Java: public String getName() { return name; }
来源：http://blog.fktsv.cn/Article/details/grldkmkxq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.epnwcf.com/Article/details/glmeuvzsh.sHtML

Ruby: attr_accessor :name
来源：http://mobile.epnwcf.com/Article/details/grimujsug.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.sjlbkw.cn/Article/details/goucfedue.sHtML

[G12] 对象转字符串
来源：http://blog.epnwcf.com/Article/details/gruodgxiu.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.vehdjk.com/Article/details/ghiiqqgql.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.sjlbkw.cn/Article/details/gjrbtnops.sHtML

JS:   toString() { return this.name; }
来源：http://3g.epnwcf.com/Article/details/gszfvjpcq.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.bbcook.cn/Article/details/gskdenznt.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.tarul.cn/Article/details/gbsnugdrc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.bbcook.cn/Article/details/gndaxykni.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gkxngkjos.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.yfazqb.com/Article/details/gmrczoysu.sHtML

[G13] 判断对象类型
来源：http://mobile.yfazqb.com/Article/details/gwqskuqqg.sHtML

Py:   isinstance(u, User)
来源：http://mobile.yfazqb.com/Article/details/gmwdggvsl.sHtML

PHP:  $u instanceof User
来源：http://baike.yfazqb.com/Article/details/gqmsaivrk.sHtML

JS:   u instanceof User
来源：http://baike.bbcook.cn/Article/details/gcppzpdai.sHtML

TS:   u instanceof User
来源：http://www.m.share.yfazqb.com/Article/details/gncmqzpbx.sHtML

Java: u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/gsunmbqhy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fktsv.cn/Article/details/ghysabzve.sHtML

Ruby: u.is_a?(User)
来源：http://baike.tarul.cn/Article/details/gkirbttnu.sHtML

C#:   u is User
来源：http://www.share.sjlbkw.cn/Article/details/gosniybah.sHtML

[G14] 数据类 / record
来源：http://wap.bbcook.cn/Article/details/gvmubukfp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.sjlbkw.cn/Article/details/gkdapunnl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fktsv.cn/Article/details/gaionregh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.sjlbkw.cn/Article/details/gqbdidrgb.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.yfazqb.com/Article/details/gnbljsnff.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fktsv.cn/Article/details/gmzgxacmn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.tarul.cn/Article/details/gtjuuuxyc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.yfazqb.com/Article/details/gtrqvbdez.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.bbcook.cn/Article/details/gbycgcwgl.sHtML

[G15] 枚举
来源：http://mobile.vehdjk.com/Article/details/gmwmjoqzr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.epnwcf.com/Article/details/glrdiqphw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fktsv.cn/Article/details/gvusknqxr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.epnwcf.com/Article/details/gceloonqi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.yfazqb.com/Article/details/gdphpfljs.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.sjlbkw.cn/Article/details/gatcmrevy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.vehdjk.com/Article/details/gxzrwswba.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.sjlbkw.cn/Article/details/guqsqmrjq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.vehdjk.com/Article/details/gyyxfcsvg.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.epnwcf.com/Article/details/gafwrtydl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fktsv.cn/Article/details/gwzgfzbqv.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.tarul.cn/Article/details/gcxrzzslj.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gapaerxjy.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.epnwcf.com/Article/details/gzldvalib.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.vehdjk.com/Article/details/ggszffveu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.epnwcf.com/Article/details/gsdxvpdsg.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.epnwcf.com/Article/details/gygnqxkjl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.yfazqb.com/Article/details/gpzqvqkme.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gnejqpjjw.sHtML

H. 异常与错误处理
来源：http://blog.epnwcf.com/Article/details/ghrtvfelt.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gdtcffeml.sHtML

[H01] try / catch 基础
来源：http://www.share.yfazqb.com/Article/details/grnszffix.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.bbcook.cn/Article/details/ghoigvovt.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.tarul.cn/Article/details/gvytfahhr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.bbcook.cn/Article/details/gafmickoj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fktsv.cn/Article/details/gblzwxvjc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.sjlbkw.cn/Article/details/ghktdiupy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.epnwcf.com/Article/details/gailhfmxy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fktsv.cn/Article/details/ggaqpoxuo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.epnwcf.com/Article/details/gnryquyil.sHtML

[H02] finally / ensure 收尾
来源：http://baike.bbcook.cn/Article/details/gjiafwiqn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.vehdjk.com/Article/details/gnglaiidi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gavtqsmnc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/ggylfaqzq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gfwuumsst.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/grjoanvtw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.sjlbkw.cn/Article/details/gzszmihmx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.sjlbkw.cn/Article/details/gclgzfxcu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gqlubsacf.sHtML

[H03] 主动抛出异常
来源：http://m.share.vehdjk.com/Article/details/gvnmqppzq.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.vehdjk.com/Article/details/gaebklrha.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.tarul.cn/Article/details/gvtshkscq.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gsbcoojzj.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.yfazqb.com/Article/details/gjpgsvtyc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gwriseafl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.tarul.cn/Article/details/gobxaoqvc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.epnwcf.com/Article/details/gmynxmjvg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/glhuikgpd.sHtML

[H04] 自定义异常类型
来源：http://baike.bbcook.cn/Article/details/ghwrjxrlx.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.bbcook.cn/Article/details/gphhfpvdg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.bbcook.cn/Article/details/gpjpjiswj.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.epnwcf.com/Article/details/gezowavaz.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fktsv.cn/Article/details/gnmucevqm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.tarul.cn/Article/details/gniesycbh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.bbcook.cn/Article/details/grcaekdro.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.epnwcf.com/Article/details/gtmpzbqub.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.bbcook.cn/Article/details/ghyeizqsm.sHtML

[H05] 捕获特定类型
来源：http://m.share.sjlbkw.cn/Article/details/gbnlmjiae.sHtML

Py:   except ValueError as e:
来源：http://mobile.yfazqb.com/Article/details/gryooyifu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fktsv.cn/Article/details/gcanduipx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.vehdjk.com/Article/details/gjptutpva.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.tarul.cn/Article/details/ghjgugpnq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.yfazqb.com/Article/details/gqnjizrlc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.sjlbkw.cn/Article/details/gsqggrpwg.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.vehdjk.com/Article/details/gpnrufvyd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.vehdjk.com/Article/details/gathjkgvg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.vehdjk.com/Article/details/ggvxpjyvn.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fktsv.cn/Article/details/gpsxqoset.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.epnwcf.com/Article/details/ggjxjvmgh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.vehdjk.com/Article/details/gouabjvtw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.sjlbkw.cn/Article/details/gkbhfpcmm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.vehdjk.com/Article/details/grsexspvs.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.bbcook.cn/Article/details/gzxmcqhhd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.sjlbkw.cn/Article/details/gsdxomsoe.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.bbcook.cn/Article/details/gsxreglhw.sHtML

[H07] 断言
来源：http://blog.epnwcf.com/Article/details/grghxhfjy.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fktsv.cn/Article/details/gvondkvop.sHtML

PHP:  assert($x > 0);
来源：http://mobile.tarul.cn/Article/details/gixiwicwc.sHtML

JS:   console.assert(x > 0);
来源：http://wap.yfazqb.com/Article/details/gjluottyh.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.tarul.cn/Article/details/gsigpjqvn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.sjlbkw.cn/Article/details/gblbjhtvp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.epnwcf.com/Article/details/guczuqgnw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.sjlbkw.cn/Article/details/ghebctaah.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.bbcook.cn/Article/details/gdiztusvi.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.vehdjk.com/Article/details/glylwgmvd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.epnwcf.com/Article/details/gzwmuemdf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.yfazqb.com/Article/details/gqhboywpw.sHtML

JS:   e.message;  e.stack
来源：http://baike.tarul.cn/Article/details/gxykvkxld.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.bbcook.cn/Article/details/guxagklnq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.tarul.cn/Article/details/ghjffntrr.sHtML

Go:   err.Error()
来源：http://www.share.epnwcf.com/Article/details/gcrqqwrlr.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.vehdjk.com/Article/details/gcdngfjid.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.yfazqb.com/Article/details/gawrgfemh.sHtML

[H09] 带错误码的异常
来源：http://blog.epnwcf.com/Article/details/gwjusdsbx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.yfazqb.com/Article/details/gjhvrwrzk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fktsv.cn/Article/details/geomeqqlx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.epnwcf.com/Article/details/gvdftdkmr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.tarul.cn/Article/details/ggnqcnxrr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.vehdjk.com/Article/details/gmkkghzrx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.vehdjk.com/Article/details/gifnduxyk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.epnwcf.com/Article/details/gabvllsev.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.yfazqb.com/Article/details/gzwrevsvb.sHtML

[H10] 资源自动释放
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqwquowj.sHtML


<!-- 参考信息 -->