代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.vehdjk.com/Article/details/gkftnxola.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.yfazqb.com/Article/details/goumgaubj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fktsv.cn/Article/details/gcblhjprd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.sjlbkw.cn/Article/details/gxrtcqdkf.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fktsv.cn/Article/details/gcigixhmf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fktsv.cn/Article/details/gcqbiiepq.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.tarul.cn/Article/details/gveumwcvs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gqfcuudol.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gtqzsmdwu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.vehdjk.com/Article/details/gvtxbnwjb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fktsv.cn/Article/details/gwwebnujs.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gmpgtvrae.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.tarul.cn/Article/details/grrewidwv.sHtML

[F06] 删除文件
来源：http://read.share.vehdjk.com/Article/details/gixllixow.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gsxivmcah.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.vehdjk.com/Article/details/guwjqffzk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.tarul.cn/Article/details/gnkbwzegc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/gshdmmdbu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/givetfxxx.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.tarul.cn/Article/details/gkakgrlpw.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.tarul.cn/Article/details/grhglqlta.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gtgwfwsed.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.yfazqb.com/Article/details/gapwqeete.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.yfazqb.com/Article/details/gjsttqwlk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.epnwcf.com/Article/details/gfegxzgsa.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.epnwcf.com/Article/details/gseyyhnml.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.yfazqb.com/Article/details/ggqbxsbsn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.vehdjk.com/Article/details/gqysgmfgw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fktsv.cn/Article/details/geoupukcb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.sjlbkw.cn/Article/details/guyrusvgp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.vehdjk.com/Article/details/gjicrrdni.sHtML

[F08] 遍历目录
来源：http://read.share.tarul.cn/Article/details/grqsntcie.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.epnwcf.com/Article/details/gfyzfmshr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.tarul.cn/Article/details/ggxeguvhh.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fktsv.cn/Article/details/gukwpnsgw.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.bbcook.cn/Article/details/gdascwmtq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fktsv.cn/Article/details/glsuzpcle.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.yfazqb.com/Article/details/gyetfeuem.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fktsv.cn/Article/details/ghluiegav.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.vehdjk.com/Article/details/gefwnrhjz.sHtML

[F09] 获取文件大小
来源：http://read.share.epnwcf.com/Article/details/gvixygvvj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.bbcook.cn/Article/details/gwanrbaqg.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gqucvfbce.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.sjlbkw.cn/Article/details/glxmdrnoh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.sjlbkw.cn/Article/details/ggwkxktno.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/gqijtrdtr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.epnwcf.com/Article/details/gusagbaje.sHtML

Ruby: File.size("a.txt")
来源：http://baike.yfazqb.com/Article/details/gccegeljh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.epnwcf.com/Article/details/gzoechltr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fktsv.cn/Article/details/gpzfwyoqi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gvhbjevmu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.yfazqb.com/Article/details/gkeopbqnk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gwcojqpyp.sHtML

TS:   path.extname("a.txt")
来源：http://wap.bbcook.cn/Article/details/gtvmzqyii.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fktsv.cn/Article/details/gauuzkikk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gcusedlrp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/glyybkrdr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/ghjbybvhl.sHtML

[F11] 复制与移动文件
来源：http://3g.yfazqb.com/Article/details/gzvydjcod.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/gyhreqdel.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.sjlbkw.cn/Article/details/goddejaiu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/grljmnuhu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gsjfwijku.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.tarul.cn/Article/details/guhpovwym.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.bbcook.cn/Article/details/gsadbytry.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/gwxvlzfdh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.epnwcf.com/Article/details/gyljrtmtd.sHtML

[F12] CSV 读写
来源：http://www.blog.vehdjk.com/Article/details/ggjlcrtje.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.bbcook.cn/Article/details/gusdrxgpi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.vehdjk.com/Article/details/glotubsej.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.sjlbkw.cn/Article/details/gddpdwmqu.sHtML

TS:   // 同上
来源：http://www.blog.bbcook.cn/Article/details/gbmrpcofj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.tarul.cn/Article/details/griievnwu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.vehdjk.com/Article/details/gccxphfqf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fktsv.cn/Article/details/gnotqhllu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.tarul.cn/Article/details/gzntancao.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gbndcxeps.sHtML

G. 面向对象
来源：http://baike.tarul.cn/Article/details/ggprapvbr.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gjbrzngei.sHtML

[G01] 定义类
来源：http://www.m.share.yfazqb.com/Article/details/guiyxrhgh.sHtML

Py:   class User: pass
来源：http://read.share.fktsv.cn/Article/details/gszrpngst.sHtML

PHP:  class User {}
来源：http://wap.bbcook.cn/Article/details/gkedamgyf.sHtML

JS:   class User {}
来源：http://3g.bbcook.cn/Article/details/ggeuuubev.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.tarul.cn/Article/details/gpwoksgtm.sHtML

Java: class User {}
来源：http://baike.bbcook.cn/Article/details/gmmlelagi.sHtML

Go:   type User struct { Name string }
来源：http://blog.bbcook.cn/Article/details/gzpkxdfvb.sHtML

Ruby: class User; end
来源：http://3g.sjlbkw.cn/Article/details/giwvnxebi.sHtML

C#:   class User {}
来源：http://www.blog.fktsv.cn/Article/details/gqljhmapi.sHtML

[G02] 构造函数
来源：http://blog.tarul.cn/Article/details/gecjsefmx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.bbcook.cn/Article/details/gbnprtmpd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.tarul.cn/Article/details/gxkynipwx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.bbcook.cn/Article/details/gootaatkp.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.vehdjk.com/Article/details/gkgdkzicb.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/gqjfmwsaq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.tarul.cn/Article/details/gxpmtppfh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fktsv.cn/Article/details/gcpfqlknn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.tarul.cn/Article/details/gpocpuhcd.sHtML

[G03] 实例属性
来源：http://3g.sjlbkw.cn/Article/details/guiurhxta.sHtML

Py:   self.name = "x"
来源：http://3g.vehdjk.com/Article/details/gucdwqqzg.sHtML

PHP:  public string $name = "x";
来源：http://m.share.bbcook.cn/Article/details/gvotrtenc.sHtML

JS:   this.name = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gbaglovbl.sHtML

TS:   name: string = "x";
来源：http://wap.vehdjk.com/Article/details/gjrsiilsh.sHtML

Java: private String name;
来源：http://www.blog.fktsv.cn/Article/details/gvksdvcwj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.tarul.cn/Article/details/gmfabquog.sHtML

Ruby: @name = "x"
来源：http://www.m.share.yfazqb.com/Article/details/gkslwfuxk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.sjlbkw.cn/Article/details/gzkwrnanj.sHtML

[G04] 定义方法
来源：http://www.m.share.epnwcf.com/Article/details/gwgvjrstm.sHtML

Py:   def greet(self): return self.name
来源：http://3g.yfazqb.com/Article/details/gsrirmzsx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.vehdjk.com/Article/details/gbtkxkrtb.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/ggkobevgj.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.tarul.cn/Article/details/gcanydnee.sHtML

Java: String greet() { return name; }
来源：http://www.share.yfazqb.com/Article/details/gljpigaei.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fktsv.cn/Article/details/gaccnodzo.sHtML

Ruby: def greet; @name; end
来源：http://mobile.sjlbkw.cn/Article/details/gxndfuxnk.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fktsv.cn/Article/details/gxzmwkzhg.sHtML

[G05] 继承
来源：http://www.blog.tarul.cn/Article/details/ghcnotzrr.sHtML

Py:   class Admin(User): pass
来源：http://blog.fktsv.cn/Article/details/gxvtdkowd.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/gkjubosmf.sHtML

JS:   class Admin extends User {}
来源：http://m.share.epnwcf.com/Article/details/ghymxudpe.sHtML

TS:   class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/ggeldffxs.sHtML

Java: class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/gihrjqzhe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fktsv.cn/Article/details/gmeywiysg.sHtML

Ruby: class Admin < User; end
来源：http://read.share.epnwcf.com/Article/details/gdsninbxi.sHtML

C#:   class Admin : User {}
来源：http://read.share.fktsv.cn/Article/details/gqwokxqvm.sHtML

[G06] 重写方法
来源：http://3g.yfazqb.com/Article/details/gkvvkcrju.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.vehdjk.com/Article/details/gyhvpjljd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gymplxwbl.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.tarul.cn/Article/details/gpfcwkweg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/gmkxkamyr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gsehtxlxm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.vehdjk.com/Article/details/gozzedria.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.vehdjk.com/Article/details/gjihxkqaz.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.yfazqb.com/Article/details/guszrgyue.sHtML

[G07] 调用父类方法
来源：http://3g.sjlbkw.cn/Article/details/gqprdurox.sHtML

Py:   super().greet()
来源：http://www.blog.fktsv.cn/Article/details/gbfpvwtan.sHtML

PHP:  parent::greet();
来源：http://baike.tarul.cn/Article/details/gtbbaaqur.sHtML

JS:   super.greet();
来源：http://3g.fktsv.cn/Article/details/gdecnwbqg.sHtML

TS:   super.greet();
来源：http://blog.tarul.cn/Article/details/glkujccpd.sHtML

Java: super.greet();
来源：http://www.m.share.fktsv.cn/Article/details/glwcfmaps.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.yfazqb.com/Article/details/gpfzbgouz.sHtML

Ruby: super
来源：http://mobile.vehdjk.com/Article/details/gojcgklzi.sHtML

C#:   base.Greet();
来源：http://3g.vehdjk.com/Article/details/gpsvqaqnp.sHtML

[G08] 静态方法与属性
来源：http://blog.sjlbkw.cn/Article/details/gkidpfpze.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.yfazqb.com/Article/details/gzxmcltth.sHtML

PHP:  public static function f() {}
来源：http://www.share.fktsv.cn/Article/details/gpgnwdkgg.sHtML

JS:   static f() {}
来源：http://wap.tarul.cn/Article/details/gaaxurvjl.sHtML

TS:   static f(): void {}
来源：http://read.share.vehdjk.com/Article/details/ghpvimwyx.sHtML

Java: static void f() {}
来源：http://3g.fktsv.cn/Article/details/gvwkabufp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fktsv.cn/Article/details/gepghspst.sHtML

Ruby: def self.f; end
来源：http://www.blog.tarul.cn/Article/details/gnmifitlm.sHtML

C#:   public static void F() {}
来源：http://www.share.fktsv.cn/Article/details/gcdleapuh.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fktsv.cn/Article/details/gcaylkgzk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.yfazqb.com/Article/details/gbqipzaie.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fktsv.cn/Article/details/gbbavlnqn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.vehdjk.com/Article/details/gtffhpeko.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fktsv.cn/Article/details/gyeicntia.sHtML

Java: interface Shape { double area(); }
来源：http://wap.sjlbkw.cn/Article/details/gjaiqsfmg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fktsv.cn/Article/details/gysjofsrv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.sjlbkw.cn/Article/details/gnqdmkekn.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.vehdjk.com/Article/details/giisknisk.sHtML

[G10] 访问控制
来源：http://www.m.share.epnwcf.com/Article/details/gxnaqrtur.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fktsv.cn/Article/details/ghraxnbqr.sHtML

PHP:  public / protected / private
来源：http://m.share.bbcook.cn/Article/details/gzovcbejk.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.yfazqb.com/Article/details/gwyxinrwr.sHtML

TS:   public / protected / private
来源：http://wap.sjlbkw.cn/Article/details/ghhtjhcao.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fktsv.cn/Article/details/gdfrmtxha.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.bbcook.cn/Article/details/gfsvktnam.sHtML

Ruby: public / protected / private
来源：http://3g.vehdjk.com/Article/details/gyytsiztc.sHtML

C#:   public / protected / private / internal
来源：http://read.share.vehdjk.com/Article/details/glvfzmazg.sHtML

[G11] getter / setter
来源：http://baike.sjlbkw.cn/Article/details/glazrajfa.sHtML

Py:   @property 与 @x.setter
来源：http://baike.sjlbkw.cn/Article/details/grchcszqu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.yfazqb.com/Article/details/gtmwdzfnn.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.vehdjk.com/Article/details/gqrrszbky.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.bbcook.cn/Article/details/gkaixiklh.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/grcqqwnzu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.yfazqb.com/Article/details/gxppvnieu.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.bbcook.cn/Article/details/gypmtxwfe.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fktsv.cn/Article/details/gykobwsgz.sHtML

[G12] 对象转字符串
来源：http://read.share.sjlbkw.cn/Article/details/gmqksfawn.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.epnwcf.com/Article/details/ggsuuvagh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/gvvjkpira.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.bbcook.cn/Article/details/ghfcbidvz.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fktsv.cn/Article/details/ghnkcijrc.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.vehdjk.com/Article/details/gynixmdyx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.vehdjk.com/Article/details/gnlqkztiz.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.vehdjk.com/Article/details/gtdjfvjab.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.vehdjk.com/Article/details/gsnaqpfus.sHtML

[G13] 判断对象类型
来源：http://www.m.share.vehdjk.com/Article/details/ggruufmxj.sHtML

Py:   isinstance(u, User)
来源：http://m.share.epnwcf.com/Article/details/gdnkzjgrm.sHtML

PHP:  $u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/gpqnmarix.sHtML

JS:   u instanceof User
来源：http://blog.yfazqb.com/Article/details/gsrlzwaeq.sHtML

TS:   u instanceof User
来源：http://mobile.epnwcf.com/Article/details/ghkhtzxnc.sHtML

Java: u instanceof User
来源：http://blog.fktsv.cn/Article/details/gflciodlm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.sjlbkw.cn/Article/details/gezwkqwvl.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.vehdjk.com/Article/details/gqtzgzaro.sHtML

C#:   u is User
来源：http://mobile.tarul.cn/Article/details/gypehdkbn.sHtML

[G14] 数据类 / record
来源：http://m.share.vehdjk.com/Article/details/gziokudgo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.bbcook.cn/Article/details/ggrgcardn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.sjlbkw.cn/Article/details/gygsvygpj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.bbcook.cn/Article/details/glqawxccd.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.tarul.cn/Article/details/gkwavoaov.sHtML

Java: record User(String name, int age) {}
来源：http://baike.sjlbkw.cn/Article/details/gjyngvcpn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fktsv.cn/Article/details/giuqeviyc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fktsv.cn/Article/details/gcgfedhnk.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.epnwcf.com/Article/details/guxouizim.sHtML

[G15] 枚举
来源：http://wap.epnwcf.com/Article/details/gmfzibkot.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.epnwcf.com/Article/details/glzbybuos.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.yfazqb.com/Article/details/ghmcuboes.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.epnwcf.com/Article/details/gqxifghai.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fktsv.cn/Article/details/goxqounuk.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.sjlbkw.cn/Article/details/gglklsdej.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.epnwcf.com/Article/details/ggfbvqyin.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.epnwcf.com/Article/details/gksemylrv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.bbcook.cn/Article/details/gnbylkpry.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.yfazqb.com/Article/details/gtbfjaooo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.epnwcf.com/Article/details/ghxxmyjlv.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.bbcook.cn/Article/details/gurljnohk.sHtML

JS:   Object.entries(obj)
来源：http://mobile.tarul.cn/Article/details/gumxdascs.sHtML

TS:   Object.entries(obj)
来源：http://mobile.bbcook.cn/Article/details/gwryevmyp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.vehdjk.com/Article/details/gvpizswbp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fktsv.cn/Article/details/gidmnxdmo.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.vehdjk.com/Article/details/gndmttioe.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.vehdjk.com/Article/details/giszomief.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gfrzuwhhl.sHtML

H. 异常与错误处理
来源：http://www.blog.fktsv.cn/Article/details/gisrmmgok.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gvhftwxzm.sHtML

[H01] try / catch 基础
来源：http://m.share.epnwcf.com/Article/details/ghbtwcgpf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.bbcook.cn/Article/details/gerbxvxvk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.tarul.cn/Article/details/goaahowss.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.yfazqb.com/Article/details/gpvwlqqoi.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gclyvbmww.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.bbcook.cn/Article/details/gjegnuxsb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.bbcook.cn/Article/details/gotnuhepd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.vehdjk.com/Article/details/gcpmfitjy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.yfazqb.com/Article/details/gprwgyoss.sHtML

[H02] finally / ensure 收尾
来源：http://blog.bbcook.cn/Article/details/gphorspjs.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.bbcook.cn/Article/details/gvtpusuuq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gfnxobzxy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gvwgrdvtx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gjuxemjsw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gmlheimms.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.bbcook.cn/Article/details/gqtcaawiv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.sjlbkw.cn/Article/details/grfwdllwv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gycotvdsg.sHtML

[H03] 主动抛出异常
来源：http://baike.vehdjk.com/Article/details/gpkwvcsqi.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.yfazqb.com/Article/details/gysehhfxk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.tarul.cn/Article/details/giwriznvv.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.yfazqb.com/Article/details/gqfmarnzg.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/gsdfthfqv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.vehdjk.com/Article/details/gnonpkivt.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.sjlbkw.cn/Article/details/gbdzwxhci.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.tarul.cn/Article/details/gwybhngys.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.yfazqb.com/Article/details/gdippkyjr.sHtML

[H04] 自定义异常类型
来源：http://www.share.tarul.cn/Article/details/gjtunutjv.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fktsv.cn/Article/details/gmugspgjw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.yfazqb.com/Article/details/gqtgypjgh.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.vehdjk.com/Article/details/gbwkhwjmk.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.vehdjk.com/Article/details/gequgmszg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.epnwcf.com/Article/details/gcsbxdgbh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.yfazqb.com/Article/details/gucrunhyb.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.bbcook.cn/Article/details/glntekbaf.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.epnwcf.com/Article/details/gqgwxadjh.sHtML

[H05] 捕获特定类型
来源：http://3g.vehdjk.com/Article/details/gxogkpgik.sHtML

Py:   except ValueError as e:
来源：http://m.share.vehdjk.com/Article/details/gbzmyloin.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fktsv.cn/Article/details/ggagqawkk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.sjlbkw.cn/Article/details/gzriulikd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.epnwcf.com/Article/details/gzblznjcx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.vehdjk.com/Article/details/gfuvfaktt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.yfazqb.com/Article/details/gdkuzjcmt.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.epnwcf.com/Article/details/glpvrlycq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.bbcook.cn/Article/details/geiisinao.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.yfazqb.com/Article/details/grwjgubtr.sHtML

Py:   value = d.get("k") or default
来源：http://blog.bbcook.cn/Article/details/glxzljnpp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.bbcook.cn/Article/details/gjaduvnbg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.yfazqb.com/Article/details/gizhjsvfc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.tarul.cn/Article/details/gpugcbiqp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.vehdjk.com/Article/details/gdvmyrqek.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.epnwcf.com/Article/details/gyojujrkt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.epnwcf.com/Article/details/ggucvkvpn.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.vehdjk.com/Article/details/gadjoazel.sHtML

[H07] 断言
来源：http://www.blog.yfazqb.com/Article/details/ghcctjysj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.tarul.cn/Article/details/goolelwlj.sHtML

PHP:  assert($x > 0);
来源：http://wap.vehdjk.com/Article/details/gqmairlug.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.vehdjk.com/Article/details/gswhagwom.sHtML

TS:   console.assert(x > 0);
来源：http://baike.sjlbkw.cn/Article/details/gemztnqhb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fktsv.cn/Article/details/gzabdjhmt.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.bbcook.cn/Article/details/gczzqoebh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fktsv.cn/Article/details/gwvhnfaqq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gjhbwylrb.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.bbcook.cn/Article/details/gshdxaepj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.tarul.cn/Article/details/gexkefhog.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fktsv.cn/Article/details/gnbkxnhcn.sHtML

JS:   e.message;  e.stack
来源：http://www.share.sjlbkw.cn/Article/details/gdezwghmq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.tarul.cn/Article/details/givpunlcd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.epnwcf.com/Article/details/gakjuwnut.sHtML

Go:   err.Error()
来源：http://www.share.bbcook.cn/Article/details/guyaebrkk.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.bbcook.cn/Article/details/gizrixpdr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.tarul.cn/Article/details/gnphqbhoq.sHtML

[H09] 带错误码的异常
来源：http://www.share.yfazqb.com/Article/details/gcyjadxrg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.bbcook.cn/Article/details/gdhtitiet.sHtML


<!-- 参考信息 -->