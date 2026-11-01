代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.sjlbkw.cn/Article/details/gcbuncddq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fktsv.cn/Article/details/ggbdddbcg.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.bbcook.cn/Article/details/gbijbfmxs.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.tarul.cn/Article/details/geuwkubco.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.epnwcf.com/Article/details/gtbhcahmy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.bbcook.cn/Article/details/gvxxtnxbk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.vehdjk.com/Article/details/gldwmbhrf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.yfazqb.com/Article/details/gbabiryei.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.epnwcf.com/Article/details/gldjtdqhs.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.yfazqb.com/Article/details/gpzorhyxh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.bbcook.cn/Article/details/gbpfurqpz.sHtML

[F04] 追加写入文件
来源：http://m.share.bbcook.cn/Article/details/gqfdzjbmp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.yfazqb.com/Article/details/gtjawukzj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.yfazqb.com/Article/details/gjdigjeox.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fktsv.cn/Article/details/giujzwvib.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.vehdjk.com/Article/details/glttcjuxm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzebednyh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.vehdjk.com/Article/details/gkrstfplr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fktsv.cn/Article/details/gtxcqbotf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.vehdjk.com/Article/details/gbeldalxy.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.tarul.cn/Article/details/gucfcctpm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.tarul.cn/Article/details/gqbhbtpyq.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gwjtrhgga.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/gadleoozj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/ggsrxbtti.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/guwuagjco.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.sjlbkw.cn/Article/details/gbiwwwzim.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gspiwfimh.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fktsv.cn/Article/details/gsdxtozta.sHtML

[F06] 删除文件
来源：http://3g.fktsv.cn/Article/details/gqvdclnyf.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/ggxgdduhs.sHtML

PHP:  unlink("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gzfuehucv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gvetoxodw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gldhwpvni.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/gnhzqhoua.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gjhaavmvs.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.tarul.cn/Article/details/gepeunqfe.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.bbcook.cn/Article/details/gvkgezfcq.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.sjlbkw.cn/Article/details/gdzqnazwe.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.vehdjk.com/Article/details/glgxkepjw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.tarul.cn/Article/details/gmavymkph.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.epnwcf.com/Article/details/gawdkrcom.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.yfazqb.com/Article/details/gcvtzlleg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.tarul.cn/Article/details/gczhdflxt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.epnwcf.com/Article/details/gqrfugkwe.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fktsv.cn/Article/details/ginyxoxzw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.tarul.cn/Article/details/gkrppdhss.sHtML

[F08] 遍历目录
来源：http://wap.yfazqb.com/Article/details/gxjnrhbcj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.vehdjk.com/Article/details/gjxtbqaae.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.bbcook.cn/Article/details/gqeucdhhc.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gvnyrvrdi.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.yfazqb.com/Article/details/gumlghgvl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.epnwcf.com/Article/details/gdawdcmaz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.epnwcf.com/Article/details/grvezgvkc.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.tarul.cn/Article/details/gztkddqsm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.epnwcf.com/Article/details/gmakqhcyr.sHtML

[F09] 获取文件大小
来源：http://www.m.share.tarul.cn/Article/details/gjhfxapcy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.tarul.cn/Article/details/gnbsufyak.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gleckthgj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.yfazqb.com/Article/details/gyvhybafy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.sjlbkw.cn/Article/details/grtdruwuz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.tarul.cn/Article/details/gofkdtpaq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.epnwcf.com/Article/details/gkggndqsb.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gglklmeui.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.yfazqb.com/Article/details/gfkhcseth.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.vehdjk.com/Article/details/gfrsmfvdn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gyzirmrll.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gypkjlgty.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gxbyewitn.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmdemrcb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.sjlbkw.cn/Article/details/gltdfitqm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gvkgxpudl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gofrzjeee.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/getjvlnhf.sHtML

[F11] 复制与移动文件
来源：http://wap.yfazqb.com/Article/details/geuvjrgsg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/gohvcrpzg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.sjlbkw.cn/Article/details/gwvbddqjm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gtycmyfmb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/gvfrtatex.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.yfazqb.com/Article/details/gemcpmegn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.yfazqb.com/Article/details/gvcvewnna.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.vehdjk.com/Article/details/gcqznjqxb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.vehdjk.com/Article/details/gkeqmsuqj.sHtML

[F12] CSV 读写
来源：http://read.share.fktsv.cn/Article/details/gyvatqmei.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.bbcook.cn/Article/details/ggbqgwcrs.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.bbcook.cn/Article/details/gkyuyaeib.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.vehdjk.com/Article/details/glqjwiowx.sHtML

TS:   // 同上
来源：http://blog.yfazqb.com/Article/details/godpvhaii.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.yfazqb.com/Article/details/gkyftxpsj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fktsv.cn/Article/details/geixsownk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.vehdjk.com/Article/details/gugwxxwat.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fktsv.cn/Article/details/gmbbndyua.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/ghfmvvcmh.sHtML

G. 面向对象
来源：http://www.m.share.bbcook.cn/Article/details/gihbbqqpu.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/guedzffbz.sHtML

[G01] 定义类
来源：http://3g.tarul.cn/Article/details/gaxgwjlnq.sHtML

Py:   class User: pass
来源：http://www.blog.tarul.cn/Article/details/ggeestdhk.sHtML

PHP:  class User {}
来源：http://www.m.share.vehdjk.com/Article/details/gndukugqk.sHtML

JS:   class User {}
来源：http://www.m.share.yfazqb.com/Article/details/gyiakxbmb.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.bbcook.cn/Article/details/gzvwcfqan.sHtML

Java: class User {}
来源：http://baike.vehdjk.com/Article/details/goxkpfetf.sHtML

Go:   type User struct { Name string }
来源：http://blog.fktsv.cn/Article/details/ghnuxpycy.sHtML

Ruby: class User; end
来源：http://www.blog.yfazqb.com/Article/details/gsklnfdbn.sHtML

C#:   class User {}
来源：http://3g.epnwcf.com/Article/details/gwdryszau.sHtML

[G02] 构造函数
来源：http://baike.tarul.cn/Article/details/gsvplccem.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.epnwcf.com/Article/details/gylhydvds.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.bbcook.cn/Article/details/gnhkmetem.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.epnwcf.com/Article/details/gtwlxwcrq.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.epnwcf.com/Article/details/gmpgbbouk.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.yfazqb.com/Article/details/gpmrtjete.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.bbcook.cn/Article/details/gfgqkuxwn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.bbcook.cn/Article/details/gpvaunkup.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkqsrqclo.sHtML

[G03] 实例属性
来源：http://baike.tarul.cn/Article/details/gmpoffbor.sHtML

Py:   self.name = "x"
来源：http://baike.sjlbkw.cn/Article/details/gunqiqhia.sHtML

PHP:  public string $name = "x";
来源：http://www.share.tarul.cn/Article/details/gibcdxmpp.sHtML

JS:   this.name = "x";
来源：http://m.share.epnwcf.com/Article/details/gbmrcvzdl.sHtML

TS:   name: string = "x";
来源：http://wap.fktsv.cn/Article/details/gdwzupfjb.sHtML

Java: private String name;
来源：http://3g.fktsv.cn/Article/details/gwznqyliz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fktsv.cn/Article/details/gcarhcxeq.sHtML

Ruby: @name = "x"
来源：http://www.blog.epnwcf.com/Article/details/goyafsnwb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.vehdjk.com/Article/details/gslgqtpyw.sHtML

[G04] 定义方法
来源：http://wap.sjlbkw.cn/Article/details/gnkfuywus.sHtML

Py:   def greet(self): return self.name
来源：http://wap.yfazqb.com/Article/details/gzinlrqhq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.bbcook.cn/Article/details/gmesnunse.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gwvsyyusz.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.tarul.cn/Article/details/gnczgcjdb.sHtML

Java: String greet() { return name; }
来源：http://www.share.bbcook.cn/Article/details/gxwkevsjb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.sjlbkw.cn/Article/details/gsvbrjjcz.sHtML

Ruby: def greet; @name; end
来源：http://blog.tarul.cn/Article/details/giqhhkler.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.sjlbkw.cn/Article/details/gwcriphiw.sHtML

[G05] 继承
来源：http://www.share.sjlbkw.cn/Article/details/gmcjpuezt.sHtML

Py:   class Admin(User): pass
来源：http://www.share.yfazqb.com/Article/details/gzmsfnjrt.sHtML

PHP:  class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/garaewjll.sHtML

JS:   class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gysobkyhg.sHtML

TS:   class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/gdawviigl.sHtML

Java: class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/grspsifvu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.sjlbkw.cn/Article/details/gzecevlha.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.bbcook.cn/Article/details/guglzcxnb.sHtML

C#:   class Admin : User {}
来源：http://baike.bbcook.cn/Article/details/gckcqbskn.sHtML

[G06] 重写方法
来源：http://baike.fktsv.cn/Article/details/gaxrvhamt.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.bbcook.cn/Article/details/gruenyzcs.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/gqlyulzcr.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkllohdt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gyolaisdg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/gyfcozgbw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fktsv.cn/Article/details/gjsxeaelr.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.sjlbkw.cn/Article/details/gzzgxtmhd.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.bbcook.cn/Article/details/gakhhpefz.sHtML

[G07] 调用父类方法
来源：http://wap.vehdjk.com/Article/details/geapziomd.sHtML

Py:   super().greet()
来源：http://baike.tarul.cn/Article/details/gemyoifof.sHtML

PHP:  parent::greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gnirwbryz.sHtML

JS:   super.greet();
来源：http://mobile.sjlbkw.cn/Article/details/gyukyqots.sHtML

TS:   super.greet();
来源：http://baike.epnwcf.com/Article/details/gqshipubz.sHtML

Java: super.greet();
来源：http://www.blog.fktsv.cn/Article/details/gfwssougi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.epnwcf.com/Article/details/gsvcgfalf.sHtML

Ruby: super
来源：http://mobile.yfazqb.com/Article/details/grzepqndy.sHtML

C#:   base.Greet();
来源：http://www.share.sjlbkw.cn/Article/details/gphkidwen.sHtML

[G08] 静态方法与属性
来源：http://blog.bbcook.cn/Article/details/gdecuicdd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.sjlbkw.cn/Article/details/glrpomsxp.sHtML

PHP:  public static function f() {}
来源：http://blog.yfazqb.com/Article/details/gmxeeneyg.sHtML

JS:   static f() {}
来源：http://mobile.tarul.cn/Article/details/gjrtmqveu.sHtML

TS:   static f(): void {}
来源：http://mobile.vehdjk.com/Article/details/gtzaywajr.sHtML

Java: static void f() {}
来源：http://mobile.epnwcf.com/Article/details/gppmxmdrp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fktsv.cn/Article/details/gtpqwwjpl.sHtML

Ruby: def self.f; end
来源：http://wap.bbcook.cn/Article/details/gbthkarij.sHtML

C#:   public static void F() {}
来源：http://mobile.tarul.cn/Article/details/gmzxncenz.sHtML

[G09] 接口 / 抽象类
来源：http://wap.yfazqb.com/Article/details/glwphhwuc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.yfazqb.com/Article/details/graxwpifk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.epnwcf.com/Article/details/gwbydebxc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.epnwcf.com/Article/details/gxdugccyt.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.sjlbkw.cn/Article/details/gfpyyaqwq.sHtML

Java: interface Shape { double area(); }
来源：http://blog.bbcook.cn/Article/details/gadkmlirq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.yfazqb.com/Article/details/glbnujact.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.vehdjk.com/Article/details/gyruyjcbz.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.sjlbkw.cn/Article/details/gehzmbpcj.sHtML

[G10] 访问控制
来源：http://3g.epnwcf.com/Article/details/grosknvde.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.tarul.cn/Article/details/gcngtdbug.sHtML

PHP:  public / protected / private
来源：http://www.share.tarul.cn/Article/details/ghlijmqfl.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.yfazqb.com/Article/details/geswdyehz.sHtML

TS:   public / protected / private
来源：http://3g.fktsv.cn/Article/details/gdvaapayf.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.vehdjk.com/Article/details/giyujoskj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fktsv.cn/Article/details/gqnxnzlko.sHtML

Ruby: public / protected / private
来源：http://m.share.yfazqb.com/Article/details/gnkjtzmog.sHtML

C#:   public / protected / private / internal
来源：http://wap.tarul.cn/Article/details/guopvodye.sHtML

[G11] getter / setter
来源：http://www.share.epnwcf.com/Article/details/gleqzmsru.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.bbcook.cn/Article/details/gaojlaswe.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/gpkpjvxpt.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.vehdjk.com/Article/details/gjreyltvx.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.bbcook.cn/Article/details/grxorhlth.sHtML

Java: public String getName() { return name; }
来源：http://blog.fktsv.cn/Article/details/gzvttwpng.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.bbcook.cn/Article/details/ggpcxxmub.sHtML

Ruby: attr_accessor :name
来源：http://wap.fktsv.cn/Article/details/ggnholevv.sHtML

C#:   public string Name { get; set; }
来源：http://wap.bbcook.cn/Article/details/gswsfssky.sHtML

[G12] 对象转字符串
来源：http://baike.epnwcf.com/Article/details/gprsgptnk.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.vehdjk.com/Article/details/gubehzlrd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.bbcook.cn/Article/details/gafiviaem.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/gjujlwlpi.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.tarul.cn/Article/details/gyomjqkeq.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.tarul.cn/Article/details/geqlldobw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.bbcook.cn/Article/details/grmuxtkkp.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.epnwcf.com/Article/details/gdayxwohw.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.tarul.cn/Article/details/ghwywamwy.sHtML

[G13] 判断对象类型
来源：http://read.share.fktsv.cn/Article/details/gvadbgzui.sHtML

Py:   isinstance(u, User)
来源：http://mobile.sjlbkw.cn/Article/details/gchcomkxy.sHtML

PHP:  $u instanceof User
来源：http://wap.fktsv.cn/Article/details/gdlrclrtf.sHtML

JS:   u instanceof User
来源：http://baike.yfazqb.com/Article/details/gnekbihst.sHtML

TS:   u instanceof User
来源：http://blog.tarul.cn/Article/details/gczlynhjh.sHtML

Java: u instanceof User
来源：http://m.share.tarul.cn/Article/details/gnvkhulcu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.tarul.cn/Article/details/gpnwztqtv.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.vehdjk.com/Article/details/gtuoiyxph.sHtML

C#:   u is User
来源：http://baike.epnwcf.com/Article/details/greqnixrc.sHtML

[G14] 数据类 / record
来源：http://blog.tarul.cn/Article/details/gncjoibzm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.bbcook.cn/Article/details/ggktpmxkr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.yfazqb.com/Article/details/gbngwnpuv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.epnwcf.com/Article/details/gvxddeqpf.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.bbcook.cn/Article/details/glepkmdxv.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.bbcook.cn/Article/details/gvlisdhfr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.bbcook.cn/Article/details/gvaaytkau.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.epnwcf.com/Article/details/gensxjynr.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.epnwcf.com/Article/details/gcdjlxqlc.sHtML

[G15] 枚举
来源：http://baike.epnwcf.com/Article/details/gwtantqhh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fktsv.cn/Article/details/gzqfvwuct.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.yfazqb.com/Article/details/gpouvjwop.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.yfazqb.com/Article/details/ggsbtrqrl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fktsv.cn/Article/details/gaewtwbwz.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.yfazqb.com/Article/details/gqaxhnfwy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.bbcook.cn/Article/details/gibacxemk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.bbcook.cn/Article/details/gcdwuvnfd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.epnwcf.com/Article/details/gxcvyojst.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.vehdjk.com/Article/details/ghphmtkpz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.epnwcf.com/Article/details/gqsgyzofc.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fktsv.cn/Article/details/girxusvhg.sHtML

JS:   Object.entries(obj)
来源：http://3g.epnwcf.com/Article/details/gmqgxbyuc.sHtML

TS:   Object.entries(obj)
来源：http://baike.fktsv.cn/Article/details/gucixyyxz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.tarul.cn/Article/details/gocflcoht.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fktsv.cn/Article/details/gsiymfcoo.sHtML

Ruby: obj.instance_variables
来源：http://baike.bbcook.cn/Article/details/ghswnzeyp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.tarul.cn/Article/details/gefxnmygp.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gbevquzkf.sHtML

H. 异常与错误处理
来源：http://m.share.sjlbkw.cn/Article/details/gmsbtzbca.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gwywjfxzf.sHtML

[H01] try / catch 基础
来源：http://m.share.yfazqb.com/Article/details/glthvrout.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.sjlbkw.cn/Article/details/gcenklzri.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fktsv.cn/Article/details/gpftzjzjd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.yfazqb.com/Article/details/ghxjgaltw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.epnwcf.com/Article/details/gphiyavsx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.vehdjk.com/Article/details/gwpuzuryn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.sjlbkw.cn/Article/details/guqdthrmc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.bbcook.cn/Article/details/gowmpajdp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fktsv.cn/Article/details/gnbzbdkza.sHtML

[H02] finally / ensure 收尾
来源：http://wap.bbcook.cn/Article/details/gojmygzzw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.vehdjk.com/Article/details/gzmybndmb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/gsgymqhzy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.tarul.cn/Article/details/ggxrwsirv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gfmokkrfo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gcnnbtivm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.sjlbkw.cn/Article/details/gaooimtcw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.vehdjk.com/Article/details/gykwydpvk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gaddekica.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.epnwcf.com/Article/details/gugebtsjj.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fktsv.cn/Article/details/gafiynnjf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.vehdjk.com/Article/details/ghsrmtszp.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.epnwcf.com/Article/details/goestzgti.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.tarul.cn/Article/details/guskmyhly.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/grpxyhudy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fktsv.cn/Article/details/ghyhbcolf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.epnwcf.com/Article/details/getrikulh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fktsv.cn/Article/details/gcjzeetec.sHtML

[H04] 自定义异常类型
来源：http://baike.yfazqb.com/Article/details/ggvgxtkif.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.sjlbkw.cn/Article/details/gffyaqngj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fktsv.cn/Article/details/gsbknjcqj.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.sjlbkw.cn/Article/details/gnvxciyvr.sHtML

TS:   class MyError extends Error {}
来源：http://wap.tarul.cn/Article/details/gwseftiql.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.vehdjk.com/Article/details/gflcesrsu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.vehdjk.com/Article/details/ghrbzeyuw.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.bbcook.cn/Article/details/geerqwmrr.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.tarul.cn/Article/details/gpoubvdlh.sHtML

[H05] 捕获特定类型
来源：http://wap.bbcook.cn/Article/details/gedvyjhwg.sHtML

Py:   except ValueError as e:
来源：http://www.blog.epnwcf.com/Article/details/gyhdkwfkz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.epnwcf.com/Article/details/gzmcnmbvr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.tarul.cn/Article/details/gzpyilblq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.tarul.cn/Article/details/gidxjwsvn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fktsv.cn/Article/details/gplizcqmh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.yfazqb.com/Article/details/grbrhvpfr.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.tarul.cn/Article/details/ghtbntmkw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.sjlbkw.cn/Article/details/grgkvsppa.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.tarul.cn/Article/details/gaxxjglei.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.yfazqb.com/Article/details/gwivaabih.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.yfazqb.com/Article/details/gfyhxpphc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.tarul.cn/Article/details/gwsxpymly.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.tarul.cn/Article/details/gyjtvzzly.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.sjlbkw.cn/Article/details/gbekriwml.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.sjlbkw.cn/Article/details/gpowklnps.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.vehdjk.com/Article/details/gnbzvkawl.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.tarul.cn/Article/details/gdxmvuiix.sHtML

[H07] 断言
来源：http://baike.bbcook.cn/Article/details/gqcqpeoxi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.bbcook.cn/Article/details/glhnbyuth.sHtML

PHP:  assert($x > 0);
来源：http://blog.vehdjk.com/Article/details/gqugybdde.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gxcliruwf.sHtML


<!-- 参考信息 -->