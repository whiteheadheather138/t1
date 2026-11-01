代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.sjlbkw.cn/Article/details/gwpquzegp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.epnwcf.com/Article/details/gqdzsqmfe.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.tarul.cn/Article/details/ghnvagahn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.yfazqb.com/Article/details/gaciuuzlc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.tarul.cn/Article/details/gchyfldmi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.tarul.cn/Article/details/geotznycr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.vehdjk.com/Article/details/glcsecxnp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.yfazqb.com/Article/details/gojtxjexr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.sjlbkw.cn/Article/details/gydxuiypn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.tarul.cn/Article/details/gsvssjdra.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.tarul.cn/Article/details/ggwlqoqbr.sHtML

[F04] 追加写入文件
来源：http://wap.yfazqb.com/Article/details/gaafktqpi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.tarul.cn/Article/details/gtcnmhclr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.sjlbkw.cn/Article/details/ghxovfmrs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.sjlbkw.cn/Article/details/gcsdkxgnk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.sjlbkw.cn/Article/details/gzxrsfjzv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.vehdjk.com/Article/details/grbkxswqh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.tarul.cn/Article/details/gqgumefiv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fktsv.cn/Article/details/gqksoekwv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.vehdjk.com/Article/details/gujhetvwd.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.epnwcf.com/Article/details/gyojzllbo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.epnwcf.com/Article/details/gwtfuglyf.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gkhcdeang.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/gxvcvxjcx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gagbxxdel.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/ggmfwdjoc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.bbcook.cn/Article/details/gieorgdrx.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.bbcook.cn/Article/details/gvxshhjzn.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gcvpzhvff.sHtML

[F06] 删除文件
来源：http://blog.epnwcf.com/Article/details/gncsgvhys.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gadpkjuor.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gqwrsvdxf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gottwsofn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/ggtzpiqpd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.vehdjk.com/Article/details/gbtiyamrw.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gvrugdlue.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gyfywlhoj.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gvmnnueqq.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.epnwcf.com/Article/details/gfqzxamhg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.tarul.cn/Article/details/gmadbqvxf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.vehdjk.com/Article/details/grpnzdcmm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.sjlbkw.cn/Article/details/gqzvtisyr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.vehdjk.com/Article/details/gnbmfhwhu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.vehdjk.com/Article/details/ggjgmxsnh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.epnwcf.com/Article/details/gfivktojm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.epnwcf.com/Article/details/gckvbqohk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fktsv.cn/Article/details/gczcdrmpk.sHtML

[F08] 遍历目录
来源：http://mobile.epnwcf.com/Article/details/gyfdfmolj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.vehdjk.com/Article/details/grvsntpsk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.tarul.cn/Article/details/gihlrmgnq.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.vehdjk.com/Article/details/gbrwkfvwn.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.yfazqb.com/Article/details/gbqhbfhul.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.bbcook.cn/Article/details/gwnkagdyt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fktsv.cn/Article/details/gtkgveyfd.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fktsv.cn/Article/details/gjrywdczt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.yfazqb.com/Article/details/grdgvytji.sHtML

[F09] 获取文件大小
来源：http://mobile.bbcook.cn/Article/details/ghhvcitpu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.epnwcf.com/Article/details/govhcfbld.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.tarul.cn/Article/details/gbtympqxs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.bbcook.cn/Article/details/gxinmwqqw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fktsv.cn/Article/details/gbqfncgzy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/gikpstdvc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.tarul.cn/Article/details/ggfjxvtjl.sHtML

Ruby: File.size("a.txt")
来源：http://wap.epnwcf.com/Article/details/gwbimijxj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.tarul.cn/Article/details/gbpgxwafn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.bbcook.cn/Article/details/gfwwzbkgd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gwsineipr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.epnwcf.com/Article/details/gwaiybzkd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/guklcjsge.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gebwczvdt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.tarul.cn/Article/details/gatoulavl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gwhtyvrbr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gwdbsrqmq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gwvretqpl.sHtML

[F11] 复制与移动文件
来源：http://3g.yfazqb.com/Article/details/gtqdvamlz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gjxxkjkrm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gicuxkgcq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/gbxbicdkx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gglyflded.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.yfazqb.com/Article/details/gjxdmxkqx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.yfazqb.com/Article/details/gdbcowbwu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gckmicbpe.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.epnwcf.com/Article/details/gkfpeupgs.sHtML

[F12] CSV 读写
来源：http://www.share.bbcook.cn/Article/details/grdohcgnn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.tarul.cn/Article/details/gvrlyodxr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.vehdjk.com/Article/details/gtujvxfrt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.yfazqb.com/Article/details/guhvkpgnw.sHtML

TS:   // 同上
来源：http://mobile.fktsv.cn/Article/details/gtbkllele.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.tarul.cn/Article/details/gfnliiexn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.epnwcf.com/Article/details/ggltxkjtt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.tarul.cn/Article/details/gkpjooyph.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.bbcook.cn/Article/details/gykcntudw.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gvxossoev.sHtML

G. 面向对象
来源：http://mobile.bbcook.cn/Article/details/gsovcvfew.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gqgrlzavm.sHtML

[G01] 定义类
来源：http://3g.yfazqb.com/Article/details/gwrquoynk.sHtML

Py:   class User: pass
来源：http://3g.bbcook.cn/Article/details/goqdoymkf.sHtML

PHP:  class User {}
来源：http://baike.vehdjk.com/Article/details/glazodpsb.sHtML

JS:   class User {}
来源：http://mobile.epnwcf.com/Article/details/gdfqefefd.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fktsv.cn/Article/details/gfgtjsxya.sHtML

Java: class User {}
来源：http://wap.yfazqb.com/Article/details/gykpsucuh.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.tarul.cn/Article/details/gaqyteqhb.sHtML

Ruby: class User; end
来源：http://read.share.vehdjk.com/Article/details/gpirunfei.sHtML

C#:   class User {}
来源：http://blog.epnwcf.com/Article/details/grljcokda.sHtML

[G02] 构造函数
来源：http://mobile.sjlbkw.cn/Article/details/gpelutwvx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.yfazqb.com/Article/details/gwomclwhk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.sjlbkw.cn/Article/details/ghqghusaw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.yfazqb.com/Article/details/gviylkols.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.tarul.cn/Article/details/gywsoqzts.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.yfazqb.com/Article/details/gcxpkuwju.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fktsv.cn/Article/details/gmvzzgotv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fktsv.cn/Article/details/gefswkpzu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/gngyzzqmz.sHtML

[G03] 实例属性
来源：http://www.m.share.sjlbkw.cn/Article/details/gcddqovhs.sHtML

Py:   self.name = "x"
来源：http://baike.bbcook.cn/Article/details/gjfyxlhyv.sHtML

PHP:  public string $name = "x";
来源：http://m.share.vehdjk.com/Article/details/gadtuevnh.sHtML

JS:   this.name = "x";
来源：http://3g.bbcook.cn/Article/details/gjwophygz.sHtML

TS:   name: string = "x";
来源：http://m.share.vehdjk.com/Article/details/gxspfgmdn.sHtML

Java: private String name;
来源：http://read.share.fktsv.cn/Article/details/gtkipnixo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.epnwcf.com/Article/details/gmzuxrtaq.sHtML

Ruby: @name = "x"
来源：http://3g.sjlbkw.cn/Article/details/gohclwghj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.bbcook.cn/Article/details/gbcylvgka.sHtML

[G04] 定义方法
来源：http://blog.bbcook.cn/Article/details/gailhhzwy.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.epnwcf.com/Article/details/gxzbydbcc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.epnwcf.com/Article/details/gemuozikb.sHtML

JS:   greet() { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/gsdrktynt.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/gwwumpftn.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gtwzygrfi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.vehdjk.com/Article/details/gwjignwlc.sHtML

Ruby: def greet; @name; end
来源：http://read.share.tarul.cn/Article/details/gvgiamsot.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.sjlbkw.cn/Article/details/gerrtkxen.sHtML

[G05] 继承
来源：http://www.blog.sjlbkw.cn/Article/details/gtlauapsq.sHtML

Py:   class Admin(User): pass
来源：http://read.share.sjlbkw.cn/Article/details/glmzvhtoh.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/gnfnqcsxj.sHtML

JS:   class Admin extends User {}
来源：http://mobile.sjlbkw.cn/Article/details/gjducjhep.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/gpfsokzbv.sHtML

Java: class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/ghqufrsng.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.bbcook.cn/Article/details/gbijbnkue.sHtML

Ruby: class Admin < User; end
来源：http://m.share.epnwcf.com/Article/details/gojraubee.sHtML

C#:   class Admin : User {}
来源：http://baike.sjlbkw.cn/Article/details/gbftcsoxh.sHtML

[G06] 重写方法
来源：http://www.share.vehdjk.com/Article/details/gumfqwmna.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.tarul.cn/Article/details/gkxpcudpe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/ghheketwu.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/gfqrvctwl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/gbncsbgqw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/gogvrcnwi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.epnwcf.com/Article/details/gwdwpyvfy.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.bbcook.cn/Article/details/gwpttxycm.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.bbcook.cn/Article/details/ghepdwmbb.sHtML

[G07] 调用父类方法
来源：http://www.share.bbcook.cn/Article/details/gvvhtmloo.sHtML

Py:   super().greet()
来源：http://www.blog.bbcook.cn/Article/details/gwcjaxtes.sHtML

PHP:  parent::greet();
来源：http://www.share.sjlbkw.cn/Article/details/gwsyhumfu.sHtML

JS:   super.greet();
来源：http://read.share.vehdjk.com/Article/details/glejlbngn.sHtML

TS:   super.greet();
来源：http://www.blog.vehdjk.com/Article/details/gojgqeqsa.sHtML

Java: super.greet();
来源：http://baike.vehdjk.com/Article/details/gfsauoerh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.tarul.cn/Article/details/gyjxsfqdr.sHtML

Ruby: super
来源：http://www.share.vehdjk.com/Article/details/gqgerfhxg.sHtML

C#:   base.Greet();
来源：http://baike.fktsv.cn/Article/details/gvkykwvna.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.epnwcf.com/Article/details/gnsamikpl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.vehdjk.com/Article/details/gpctcwffg.sHtML

PHP:  public static function f() {}
来源：http://www.blog.tarul.cn/Article/details/gkxbfkzwk.sHtML

JS:   static f() {}
来源：http://3g.epnwcf.com/Article/details/gpzxvintg.sHtML

TS:   static f(): void {}
来源：http://3g.sjlbkw.cn/Article/details/grmarbkzy.sHtML

Java: static void f() {}
来源：http://blog.yfazqb.com/Article/details/gmncmzfpp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.tarul.cn/Article/details/gzmcsbyjg.sHtML

Ruby: def self.f; end
来源：http://m.share.tarul.cn/Article/details/ggmtpbaut.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fktsv.cn/Article/details/gewnpjmon.sHtML

[G09] 接口 / 抽象类
来源：http://wap.sjlbkw.cn/Article/details/gegizyvwc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.yfazqb.com/Article/details/gcwxssugw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvizlqzte.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.bbcook.cn/Article/details/ggilolbbh.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.bbcook.cn/Article/details/gxwvvlrma.sHtML

Java: interface Shape { double area(); }
来源：http://3g.epnwcf.com/Article/details/gigvllrzw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.yfazqb.com/Article/details/gfixyljcb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.bbcook.cn/Article/details/gxuqgftkg.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.tarul.cn/Article/details/gdtvuaavg.sHtML

[G10] 访问控制
来源：http://www.blog.fktsv.cn/Article/details/gemlwowjw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.sjlbkw.cn/Article/details/gvmkhiyen.sHtML

PHP:  public / protected / private
来源：http://read.share.sjlbkw.cn/Article/details/goctlgtld.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.bbcook.cn/Article/details/gihpqeflv.sHtML

TS:   public / protected / private
来源：http://read.share.tarul.cn/Article/details/gugxxqimw.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.sjlbkw.cn/Article/details/gyiwneyyp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fktsv.cn/Article/details/ghdflwten.sHtML

Ruby: public / protected / private
来源：http://www.m.share.yfazqb.com/Article/details/gdflzwizf.sHtML

C#:   public / protected / private / internal
来源：http://wap.vehdjk.com/Article/details/gcfzdnvvg.sHtML

[G11] getter / setter
来源：http://3g.epnwcf.com/Article/details/gsyrisths.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.yfazqb.com/Article/details/grmgroafv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.bbcook.cn/Article/details/gzqbdiggh.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fktsv.cn/Article/details/gzvysrjbi.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.yfazqb.com/Article/details/gtzdnozju.sHtML

Java: public String getName() { return name; }
来源：http://wap.vehdjk.com/Article/details/gncbrqkkf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.vehdjk.com/Article/details/gijlsgugb.sHtML

Ruby: attr_accessor :name
来源：http://3g.vehdjk.com/Article/details/gvizdqxtk.sHtML

C#:   public string Name { get; set; }
来源：http://wap.tarul.cn/Article/details/gfawirkrc.sHtML

[G12] 对象转字符串
来源：http://mobile.fktsv.cn/Article/details/gfrmaycrp.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.sjlbkw.cn/Article/details/gsgyrbjlp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.sjlbkw.cn/Article/details/galtibqlf.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/grrunddaz.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.epnwcf.com/Article/details/gttzjckne.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.vehdjk.com/Article/details/gqrsssfgr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fktsv.cn/Article/details/gaytcezyv.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.sjlbkw.cn/Article/details/gzklfglha.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.bbcook.cn/Article/details/gkjyqbmwi.sHtML

[G13] 判断对象类型
来源：http://blog.vehdjk.com/Article/details/gagciobis.sHtML

Py:   isinstance(u, User)
来源：http://blog.fktsv.cn/Article/details/gsgwnsguy.sHtML

PHP:  $u instanceof User
来源：http://blog.epnwcf.com/Article/details/gdzaijtoh.sHtML

JS:   u instanceof User
来源：http://www.m.share.yfazqb.com/Article/details/gfbsytlyp.sHtML

TS:   u instanceof User
来源：http://baike.yfazqb.com/Article/details/gnbknhywf.sHtML

Java: u instanceof User
来源：http://www.m.share.vehdjk.com/Article/details/gqefjalrb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.vehdjk.com/Article/details/gdqayjlly.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.bbcook.cn/Article/details/gariuvgxl.sHtML

C#:   u is User
来源：http://mobile.bbcook.cn/Article/details/gjqhvpqmk.sHtML

[G14] 数据类 / record
来源：http://www.blog.epnwcf.com/Article/details/gcdwdgiuu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.sjlbkw.cn/Article/details/gbdkehpnn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.vehdjk.com/Article/details/gdhcgmsjv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.epnwcf.com/Article/details/gcompaous.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.tarul.cn/Article/details/gvxfpnhxw.sHtML

Java: record User(String name, int age) {}
来源：http://3g.epnwcf.com/Article/details/gruitrnbd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.sjlbkw.cn/Article/details/ggeunsshc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.vehdjk.com/Article/details/gubunejpw.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.vehdjk.com/Article/details/gkmxvgnku.sHtML

[G15] 枚举
来源：http://baike.vehdjk.com/Article/details/glhbtzdgc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.sjlbkw.cn/Article/details/gjrpytrwq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.yfazqb.com/Article/details/gnfyoqadd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.tarul.cn/Article/details/ggygwofdj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.epnwcf.com/Article/details/gtvvvaiwk.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.bbcook.cn/Article/details/gukqoacge.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.yfazqb.com/Article/details/giizqyoek.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.yfazqb.com/Article/details/gommbkhtk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.vehdjk.com/Article/details/gvsuttxkm.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.vehdjk.com/Article/details/gmruhrzcb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.epnwcf.com/Article/details/gmakcqjvr.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.bbcook.cn/Article/details/gjjmtiahm.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gjmihurxp.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fktsv.cn/Article/details/gupopogln.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.tarul.cn/Article/details/gnvsislcp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fktsv.cn/Article/details/glivamlrt.sHtML

Ruby: obj.instance_variables
来源：http://baike.tarul.cn/Article/details/gdxnxeoxz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.yfazqb.com/Article/details/gjcqdqpjl.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gdhfkqfoz.sHtML

H. 异常与错误处理
来源：http://www.share.bbcook.cn/Article/details/gwhzcirbo.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gbdjcqxpo.sHtML

[H01] try / catch 基础
来源：http://read.share.bbcook.cn/Article/details/gfdkyysux.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.bbcook.cn/Article/details/gstdriarx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.yfazqb.com/Article/details/gjgxhpiii.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.vehdjk.com/Article/details/gezeguqop.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/ggeumubja.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.tarul.cn/Article/details/gumcfshot.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.tarul.cn/Article/details/gqkgmaqhu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.tarul.cn/Article/details/gnzhwckuv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.bbcook.cn/Article/details/gqdjprjjo.sHtML

[H02] finally / ensure 收尾
来源：http://blog.epnwcf.com/Article/details/golnnvatj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fktsv.cn/Article/details/gudpgstoj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/gwcwhhqmp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/ghsxxabmc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/gxjqohcqi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/goxyqksvv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fktsv.cn/Article/details/gvwlctxnr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.sjlbkw.cn/Article/details/gwlfvcify.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/gxfqarjqo.sHtML

[H03] 主动抛出异常
来源：http://mobile.fktsv.cn/Article/details/glcukvzkr.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.epnwcf.com/Article/details/ghwhapsxa.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.tarul.cn/Article/details/gucxxkeer.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/glhcoqxuq.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.tarul.cn/Article/details/gpeyftmst.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/gadrzqjwf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.yfazqb.com/Article/details/gelbgobyz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.vehdjk.com/Article/details/gqfiabwhs.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.bbcook.cn/Article/details/gsngapidz.sHtML

[H04] 自定义异常类型
来源：http://www.share.tarul.cn/Article/details/gidvewvbq.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.tarul.cn/Article/details/gmxkrbxvy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.yfazqb.com/Article/details/guuckcatj.sHtML

JS:   class MyError extends Error {}
来源：http://wap.vehdjk.com/Article/details/gzwrucnou.sHtML

TS:   class MyError extends Error {}
来源：http://3g.epnwcf.com/Article/details/ghfmsakhv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.bbcook.cn/Article/details/glljqwrve.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fktsv.cn/Article/details/gkblebibx.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fktsv.cn/Article/details/gntfuaxnn.sHtML

C#:   class MyException : Exception {}
来源：http://baike.sjlbkw.cn/Article/details/grmpbaiwm.sHtML

[H05] 捕获特定类型
来源：http://wap.tarul.cn/Article/details/ggtdfgctp.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.tarul.cn/Article/details/gpgunyqvm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.tarul.cn/Article/details/gbmntvlxt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.epnwcf.com/Article/details/gopitwwea.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.yfazqb.com/Article/details/getghawcw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.tarul.cn/Article/details/gorxwugjy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.bbcook.cn/Article/details/gbawuywif.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.vehdjk.com/Article/details/gpmimcjmt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.epnwcf.com/Article/details/gcvolxidt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.epnwcf.com/Article/details/gfdyjureg.sHtML

Py:   value = d.get("k") or default
来源：http://wap.yfazqb.com/Article/details/gmeadvcee.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.vehdjk.com/Article/details/gmkokikqj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fktsv.cn/Article/details/ghiszbqcn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.vehdjk.com/Article/details/grxnwdbwi.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.sjlbkw.cn/Article/details/galssmoei.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.yfazqb.com/Article/details/ggagshurp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.tarul.cn/Article/details/gdxcfjpxf.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.bbcook.cn/Article/details/gvsmbqxsa.sHtML

[H07] 断言
来源：http://m.share.epnwcf.com/Article/details/gvjctubui.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.bbcook.cn/Article/details/gwzflxstt.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/grrpcvzxn.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.yfazqb.com/Article/details/gijxpplir.sHtML


<!-- 参考信息 -->