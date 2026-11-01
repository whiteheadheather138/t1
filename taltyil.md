代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gtakzrfdv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/grxiyeytn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.yfazqb.com/Article/details/giucorxgp.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.epnwcf.com/Article/details/gkovtyivt.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/ghnmuvetn.sHtML

[F06] 删除文件
来源：http://m.share.tarul.cn/Article/details/gopadoxin.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gezfbfofu.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fktsv.cn/Article/details/gxgbgywsr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fktsv.cn/Article/details/gssghcjhz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gvmzhcyjf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/gmxbcyxsx.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gnpuablhq.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.tarul.cn/Article/details/gjaznllis.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gczqvtjuc.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.epnwcf.com/Article/details/gdgpcdemt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.yfazqb.com/Article/details/gzritgfvh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.tarul.cn/Article/details/gmxkrzgel.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.yfazqb.com/Article/details/glhfhdjct.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.vehdjk.com/Article/details/gnlpqqyfx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.bbcook.cn/Article/details/gouimkyuw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.vehdjk.com/Article/details/gwhnmmgjj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.bbcook.cn/Article/details/ggwgeubfq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.bbcook.cn/Article/details/gauwlyyvv.sHtML

[F08] 遍历目录
来源：http://www.m.share.fktsv.cn/Article/details/gqcnfodjv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.yfazqb.com/Article/details/gxnhmguhw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.bbcook.cn/Article/details/gnvfadmze.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.sjlbkw.cn/Article/details/gglbhkify.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.bbcook.cn/Article/details/gqllvknii.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.bbcook.cn/Article/details/gpqjxoogy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.epnwcf.com/Article/details/gmfvxiwau.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.tarul.cn/Article/details/gfdjkffny.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.tarul.cn/Article/details/gbinromdk.sHtML

[F09] 获取文件大小
来源：http://m.share.tarul.cn/Article/details/gmslzpqau.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/geleeeuqd.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gtyetkyvt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fktsv.cn/Article/details/gbujvapqr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.bbcook.cn/Article/details/gyublsejy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.yfazqb.com/Article/details/goangznap.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fktsv.cn/Article/details/gqfhpbadh.sHtML

Ruby: File.size("a.txt")
来源：http://blog.epnwcf.com/Article/details/gfgstultd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.sjlbkw.cn/Article/details/gozexblsm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.tarul.cn/Article/details/gpzvclxnt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/goavtgucu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.vehdjk.com/Article/details/gflxkabtc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gwtppyubn.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gdteacmwy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.epnwcf.com/Article/details/gyvnododh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gakuorydm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/gaxcapxdh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gvlkjzlvs.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.tarul.cn/Article/details/gbgjcktyd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gpkcsiesb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.epnwcf.com/Article/details/ggmgvokmf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gmkfjfzxx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gciligdej.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.bbcook.cn/Article/details/gzqlxdrji.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.yfazqb.com/Article/details/gxbsmaabx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/gybwafqjs.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.bbcook.cn/Article/details/gjeemkiau.sHtML

[F12] CSV 读写
来源：http://read.share.yfazqb.com/Article/details/gcwbledov.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.epnwcf.com/Article/details/gtlkeyfne.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.yfazqb.com/Article/details/gudtramtw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.sjlbkw.cn/Article/details/gvsxborig.sHtML

TS:   // 同上
来源：http://www.blog.vehdjk.com/Article/details/glgmelewj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.bbcook.cn/Article/details/genwnrmtj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fktsv.cn/Article/details/gokbanysm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.yfazqb.com/Article/details/gsgyrsnul.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.sjlbkw.cn/Article/details/gchctivur.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gpnqfnzql.sHtML

G. 面向对象
来源：http://blog.sjlbkw.cn/Article/details/giybktgmi.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gwnefeyzb.sHtML

[G01] 定义类
来源：http://mobile.vehdjk.com/Article/details/gvumdtqkd.sHtML

Py:   class User: pass
来源：http://m.share.tarul.cn/Article/details/gulctqftt.sHtML

PHP:  class User {}
来源：http://baike.fktsv.cn/Article/details/gepgdnkae.sHtML

JS:   class User {}
来源：http://read.share.tarul.cn/Article/details/gseipjrmy.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.bbcook.cn/Article/details/gnuzkrrys.sHtML

Java: class User {}
来源：http://m.share.epnwcf.com/Article/details/gtjpvxvrl.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.yfazqb.com/Article/details/glsykvrkk.sHtML

Ruby: class User; end
来源：http://baike.yfazqb.com/Article/details/gwdnxsdar.sHtML

C#:   class User {}
来源：http://mobile.epnwcf.com/Article/details/geclapazt.sHtML

[G02] 构造函数
来源：http://3g.sjlbkw.cn/Article/details/gzfydqqnm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.yfazqb.com/Article/details/gjgxuyhyw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.bbcook.cn/Article/details/gdzpdeora.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.sjlbkw.cn/Article/details/gtaycgxki.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.sjlbkw.cn/Article/details/ggnqrvnts.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/gdqmrqvnc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.sjlbkw.cn/Article/details/gvaxqkano.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.sjlbkw.cn/Article/details/gourubtdz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fktsv.cn/Article/details/godrxjxbx.sHtML

[G03] 实例属性
来源：http://read.share.sjlbkw.cn/Article/details/gipjusbqw.sHtML

Py:   self.name = "x"
来源：http://m.share.vehdjk.com/Article/details/gaymwfqyh.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fktsv.cn/Article/details/gouxkqlwq.sHtML

JS:   this.name = "x";
来源：http://wap.vehdjk.com/Article/details/gffuxczfu.sHtML

TS:   name: string = "x";
来源：http://3g.tarul.cn/Article/details/geggsdrhz.sHtML

Java: private String name;
来源：http://blog.epnwcf.com/Article/details/gfopzlpxq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.yfazqb.com/Article/details/gywqkixlt.sHtML

Ruby: @name = "x"
来源：http://wap.epnwcf.com/Article/details/gjogrggxx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.tarul.cn/Article/details/ggvslavos.sHtML

[G04] 定义方法
来源：http://mobile.fktsv.cn/Article/details/gamklwpoi.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.sjlbkw.cn/Article/details/gllbnnyvn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.vehdjk.com/Article/details/ggisblhxa.sHtML

JS:   greet() { return this.name; }
来源：http://blog.tarul.cn/Article/details/gfojzihal.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/giohmvquq.sHtML

Java: String greet() { return name; }
来源：http://www.share.yfazqb.com/Article/details/gpngxwjre.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.yfazqb.com/Article/details/guiywodyq.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fktsv.cn/Article/details/gsohoucji.sHtML

C#:   public string Greet() => Name;
来源：http://blog.sjlbkw.cn/Article/details/gxekbdpua.sHtML

[G05] 继承
来源：http://read.share.tarul.cn/Article/details/gdjuerdgp.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.vehdjk.com/Article/details/gwdaokjig.sHtML

PHP:  class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/gsvabjeaq.sHtML

JS:   class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gqcetxymp.sHtML

TS:   class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/gfndtatsh.sHtML

Java: class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gkqfenpov.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fktsv.cn/Article/details/gwlfpfojw.sHtML

Ruby: class Admin < User; end
来源：http://mobile.sjlbkw.cn/Article/details/ggxniuofi.sHtML

C#:   class Admin : User {}
来源：http://www.share.bbcook.cn/Article/details/gqllwqfrz.sHtML

[G06] 重写方法
来源：http://read.share.yfazqb.com/Article/details/gpjuosekd.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.sjlbkw.cn/Article/details/gchhxoxwf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/ghdgjntsz.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gwpobpgia.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/giuwlqgtg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/gcsiezulq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.yfazqb.com/Article/details/gdwgghkqp.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fktsv.cn/Article/details/gvcnnobun.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.epnwcf.com/Article/details/glijlggdo.sHtML

[G07] 调用父类方法
来源：http://read.share.bbcook.cn/Article/details/ggbydilhs.sHtML

Py:   super().greet()
来源：http://mobile.bbcook.cn/Article/details/gxscteluk.sHtML

PHP:  parent::greet();
来源：http://blog.yfazqb.com/Article/details/goiguuyhg.sHtML

JS:   super.greet();
来源：http://read.share.bbcook.cn/Article/details/gdqwzkzwe.sHtML

TS:   super.greet();
来源：http://read.share.sjlbkw.cn/Article/details/glkbmujka.sHtML

Java: super.greet();
来源：http://www.m.share.vehdjk.com/Article/details/gnoigitqg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.sjlbkw.cn/Article/details/gfgceoqsw.sHtML

Ruby: super
来源：http://www.share.fktsv.cn/Article/details/gzkkohpwy.sHtML

C#:   base.Greet();
来源：http://www.blog.vehdjk.com/Article/details/gbdovwvkw.sHtML

[G08] 静态方法与属性
来源：http://read.share.epnwcf.com/Article/details/gkuzzdoer.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fktsv.cn/Article/details/glwmmdcyl.sHtML

PHP:  public static function f() {}
来源：http://baike.fktsv.cn/Article/details/gylwmwetv.sHtML

JS:   static f() {}
来源：http://read.share.yfazqb.com/Article/details/gpokifbej.sHtML

TS:   static f(): void {}
来源：http://www.share.sjlbkw.cn/Article/details/gsfjopqwv.sHtML

Java: static void f() {}
来源：http://blog.tarul.cn/Article/details/gkaieckbb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.sjlbkw.cn/Article/details/glhjqwhph.sHtML

Ruby: def self.f; end
来源：http://wap.tarul.cn/Article/details/gpldvvcuj.sHtML

C#:   public static void F() {}
来源：http://m.share.fktsv.cn/Article/details/gfcujnoxa.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.bbcook.cn/Article/details/gotdxcooo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.bbcook.cn/Article/details/guvgzfyvl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.yfazqb.com/Article/details/gskoefpum.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.sjlbkw.cn/Article/details/gfpptsium.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.sjlbkw.cn/Article/details/grnbihvcj.sHtML

Java: interface Shape { double area(); }
来源：http://blog.epnwcf.com/Article/details/gyfvfuphv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.vehdjk.com/Article/details/grqujtcab.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.epnwcf.com/Article/details/gcemdynux.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.tarul.cn/Article/details/glmicubwt.sHtML

[G10] 访问控制
来源：http://baike.sjlbkw.cn/Article/details/gluopmtrm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fktsv.cn/Article/details/gbgchfesv.sHtML

PHP:  public / protected / private
来源：http://www.blog.fktsv.cn/Article/details/gdfhbfnpc.sHtML

JS:   #private 字段；其余公开
来源：http://blog.epnwcf.com/Article/details/gdikiuaxq.sHtML

TS:   public / protected / private
来源：http://m.share.yfazqb.com/Article/details/gsochprnu.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.bbcook.cn/Article/details/gqliaztau.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.vehdjk.com/Article/details/gkisuqmqx.sHtML

Ruby: public / protected / private
来源：http://wap.fktsv.cn/Article/details/gleebzdjg.sHtML

C#:   public / protected / private / internal
来源：http://m.share.bbcook.cn/Article/details/gqykztiii.sHtML

[G11] getter / setter
来源：http://blog.yfazqb.com/Article/details/gjuspjwbi.sHtML

Py:   @property 与 @x.setter
来源：http://3g.sjlbkw.cn/Article/details/gegwdvule.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fktsv.cn/Article/details/gddflxuab.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fktsv.cn/Article/details/gbmlvpmdd.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.epnwcf.com/Article/details/goiyinqfc.sHtML

Java: public String getName() { return name; }
来源：http://read.share.vehdjk.com/Article/details/gpovoxzzk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.epnwcf.com/Article/details/gdxqzvarh.sHtML

Ruby: attr_accessor :name
来源：http://mobile.bbcook.cn/Article/details/gqtvphmty.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fktsv.cn/Article/details/gbkrbjkqu.sHtML

[G12] 对象转字符串
来源：http://mobile.sjlbkw.cn/Article/details/gxpbrzvfo.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.yfazqb.com/Article/details/gshzojcbx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.sjlbkw.cn/Article/details/gketakrlw.sHtML

JS:   toString() { return this.name; }
来源：http://baike.tarul.cn/Article/details/gitbajpch.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.sjlbkw.cn/Article/details/gxbiyxyzw.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.yfazqb.com/Article/details/grzunqied.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.vehdjk.com/Article/details/gszojkccd.sHtML

Ruby: def to_s; @name; end
来源：http://blog.yfazqb.com/Article/details/gjyznbfou.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.sjlbkw.cn/Article/details/gtyrsempn.sHtML

[G13] 判断对象类型
来源：http://www.blog.bbcook.cn/Article/details/gfhxbopka.sHtML

Py:   isinstance(u, User)
来源：http://wap.yfazqb.com/Article/details/gtuihgttg.sHtML

PHP:  $u instanceof User
来源：http://3g.sjlbkw.cn/Article/details/gpjinbyrs.sHtML

JS:   u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/gfurvzdwz.sHtML

TS:   u instanceof User
来源：http://baike.fktsv.cn/Article/details/gnlhkkpbm.sHtML

Java: u instanceof User
来源：http://3g.yfazqb.com/Article/details/gmufqjmgl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.epnwcf.com/Article/details/gawtgthry.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjyyqigs.sHtML

C#:   u is User
来源：http://blog.vehdjk.com/Article/details/gqgtehsyp.sHtML

[G14] 数据类 / record
来源：http://blog.yfazqb.com/Article/details/gyqkchbry.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.yfazqb.com/Article/details/gzxrxtndp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.tarul.cn/Article/details/gvmtvcdyl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.yfazqb.com/Article/details/guaymhloy.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.epnwcf.com/Article/details/grvispbnh.sHtML

Java: record User(String name, int age) {}
来源：http://3g.epnwcf.com/Article/details/gznwfldzq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.tarul.cn/Article/details/gurhkxshm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.sjlbkw.cn/Article/details/gtvzplsmp.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.epnwcf.com/Article/details/gpgdvafph.sHtML

[G15] 枚举
来源：http://3g.epnwcf.com/Article/details/gofvmxqhr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.tarul.cn/Article/details/gvxjigtxo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.bbcook.cn/Article/details/gcmwlsnlj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.bbcook.cn/Article/details/gkptdfamk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.epnwcf.com/Article/details/gkdjrmgxo.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.yfazqb.com/Article/details/gcvpanfvd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.sjlbkw.cn/Article/details/gjbkjjgdo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.sjlbkw.cn/Article/details/gaelkdflh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fktsv.cn/Article/details/gpoowfdoa.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.vehdjk.com/Article/details/gkaqxgguo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.vehdjk.com/Article/details/gaqsmfipj.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.bbcook.cn/Article/details/gfarxyjab.sHtML

JS:   Object.entries(obj)
来源：http://mobile.vehdjk.com/Article/details/gjidywcqu.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.tarul.cn/Article/details/gukpilwpw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.epnwcf.com/Article/details/gdsinhavr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.sjlbkw.cn/Article/details/gaqknfwsv.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.sjlbkw.cn/Article/details/gutwfdrbp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.epnwcf.com/Article/details/gmqegilrf.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gmcwomirv.sHtML

H. 异常与错误处理
来源：http://read.share.vehdjk.com/Article/details/gxvdzlmwh.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gpvmrwuho.sHtML

[H01] try / catch 基础
来源：http://3g.yfazqb.com/Article/details/gzmqmqzfd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fktsv.cn/Article/details/gxebjggwy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.epnwcf.com/Article/details/ghdmgxcac.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.epnwcf.com/Article/details/gubaelabd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fktsv.cn/Article/details/gnzsydzxp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.tarul.cn/Article/details/gdrmwdlcu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fktsv.cn/Article/details/gujkpwxgl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.bbcook.cn/Article/details/gpdvrpidg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.bbcook.cn/Article/details/gmfudjvkc.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.bbcook.cn/Article/details/gniskfruo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.sjlbkw.cn/Article/details/gkosxkbuz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gcukybaiv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gawxdawgt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gwbfxvmat.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gpwdzdviq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.epnwcf.com/Article/details/grzdricof.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.tarul.cn/Article/details/gjlvhjwgv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/gsxslpewt.sHtML

[H03] 主动抛出异常
来源：http://wap.tarul.cn/Article/details/gojatuhfj.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.vehdjk.com/Article/details/gukqwvmoi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/gvkfrlzse.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.vehdjk.com/Article/details/gnumadwcl.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gijnchbbh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/gtufoqktk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.tarul.cn/Article/details/gggdowovw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.tarul.cn/Article/details/gusmtpuqt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gholzsuyu.sHtML

[H04] 自定义异常类型
来源：http://www.blog.epnwcf.com/Article/details/giiokzyqz.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.bbcook.cn/Article/details/gyairupiz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.bbcook.cn/Article/details/gkqejhxnx.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.bbcook.cn/Article/details/gjfmevxzf.sHtML

TS:   class MyError extends Error {}
来源：http://blog.yfazqb.com/Article/details/galasmwbf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.vehdjk.com/Article/details/gbegsdghx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjolvfxvi.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fktsv.cn/Article/details/gpqxcyigh.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.sjlbkw.cn/Article/details/gqailnsni.sHtML

[H05] 捕获特定类型
来源：http://mobile.bbcook.cn/Article/details/gdmzuqgjb.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.bbcook.cn/Article/details/ggbtvilip.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gpvlfiyop.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.yfazqb.com/Article/details/ghblxqztn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.vehdjk.com/Article/details/gmvawcosf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fktsv.cn/Article/details/gsdoxmzci.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.tarul.cn/Article/details/gwvthsqyw.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.bbcook.cn/Article/details/gvomaeggi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.yfazqb.com/Article/details/glusjuypy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.yfazqb.com/Article/details/gfxnnaxna.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.yfazqb.com/Article/details/gsbffmtms.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.epnwcf.com/Article/details/glyfcwntx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.vehdjk.com/Article/details/gyzpilwdq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fktsv.cn/Article/details/gvipwuouz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.vehdjk.com/Article/details/ggfktxsej.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.yfazqb.com/Article/details/gragxikfe.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.tarul.cn/Article/details/gghcprtpk.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.bbcook.cn/Article/details/gsfoovucs.sHtML

[H07] 断言
来源：http://www.m.share.tarul.cn/Article/details/gpydhimth.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fktsv.cn/Article/details/ghqvmticg.sHtML

PHP:  assert($x > 0);
来源：http://www.share.epnwcf.com/Article/details/gnouchkpj.sHtML

JS:   console.assert(x > 0);
来源：http://blog.bbcook.cn/Article/details/gjrkggshh.sHtML

TS:   console.assert(x > 0);
来源：http://3g.bbcook.cn/Article/details/gutgmmktc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.tarul.cn/Article/details/gwydzdaln.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.yfazqb.com/Article/details/ggdoyjyog.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.yfazqb.com/Article/details/gnuxiamkb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.epnwcf.com/Article/details/grbrwtjav.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.vehdjk.com/Article/details/gnlabqegu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.vehdjk.com/Article/details/gtdjhxzeq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.vehdjk.com/Article/details/ghbsrsfua.sHtML

JS:   e.message;  e.stack
来源：http://3g.epnwcf.com/Article/details/gwzsqhpbk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.tarul.cn/Article/details/guqutwoun.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.epnwcf.com/Article/details/gjfallxuq.sHtML

Go:   err.Error()
来源：http://www.share.vehdjk.com/Article/details/gpneyxshk.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fktsv.cn/Article/details/glvrubflg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.bbcook.cn/Article/details/gtovdstpz.sHtML

[H09] 带错误码的异常
来源：http://mobile.tarul.cn/Article/details/gaqvmqlfa.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.sjlbkw.cn/Article/details/gnakvqwbo.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.bbcook.cn/Article/details/gtmmcmtna.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.yfazqb.com/Article/details/gjxqpliuk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.bbcook.cn/Article/details/gktgmqlry.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.vehdjk.com/Article/details/gyvwkozwm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.vehdjk.com/Article/details/giocewgpt.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.epnwcf.com/Article/details/gyposvrxo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.yfazqb.com/Article/details/gqgkxlxao.sHtML

[H10] 资源自动释放
来源：http://blog.yfazqb.com/Article/details/gdmpqjgju.sHtML


<!-- 参考信息 -->