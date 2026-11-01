代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.sjlbkw.cn/Article/details/gbblggvos.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.tarul.cn/Article/details/gnoppuptl.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.sjlbkw.cn/Article/details/grujzjfxb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.tarul.cn/Article/details/gwmuanwdw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.epnwcf.com/Article/details/gskasbput.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fktsv.cn/Article/details/gubfbcglh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.epnwcf.com/Article/details/gvzijzqym.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.vehdjk.com/Article/details/ggdodyygx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.sjlbkw.cn/Article/details/goldbryif.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.tarul.cn/Article/details/gmtacxjeq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.epnwcf.com/Article/details/gjpxbmged.sHtML

[F04] 追加写入文件
来源：http://3g.sjlbkw.cn/Article/details/ggiozmkfd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.vehdjk.com/Article/details/gihbwlwox.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.tarul.cn/Article/details/ggeaymkpi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.sjlbkw.cn/Article/details/gcuxzczgi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.tarul.cn/Article/details/glusszamh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.yfazqb.com/Article/details/gsmlovynu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.sjlbkw.cn/Article/details/gyjztnxlt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.yfazqb.com/Article/details/gdtqtstze.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.tarul.cn/Article/details/gxdlroqhv.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fktsv.cn/Article/details/gfklfopji.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fktsv.cn/Article/details/gidarprfr.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.tarul.cn/Article/details/gfhwifcer.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gmloccqny.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gmcwrslkf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gadkdfulh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.epnwcf.com/Article/details/gqkcpazfu.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.yfazqb.com/Article/details/gzfbgecjt.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gauycawvm.sHtML

[F06] 删除文件
来源：http://www.blog.fktsv.cn/Article/details/gkpslqgqz.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gojpjaqul.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gmippjqpa.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gbrypiexc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.tarul.cn/Article/details/glfldpgkp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gnaqcynep.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gcepprijm.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.tarul.cn/Article/details/gclxuxnha.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gzlxjjqep.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fktsv.cn/Article/details/gvwkxdyle.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fktsv.cn/Article/details/gnjcmmxxc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.bbcook.cn/Article/details/gqgmejgji.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.sjlbkw.cn/Article/details/gwajjxqvc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.yfazqb.com/Article/details/ggjrssjaw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.tarul.cn/Article/details/gqxotiiru.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.yfazqb.com/Article/details/gubuhurbg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fktsv.cn/Article/details/gpdpfjyiv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.epnwcf.com/Article/details/guhoexifs.sHtML

[F08] 遍历目录
来源：http://www.m.share.vehdjk.com/Article/details/gjlrupdif.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.yfazqb.com/Article/details/gngyhkaif.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fktsv.cn/Article/details/gwawduxmo.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fktsv.cn/Article/details/grzgfdksm.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.tarul.cn/Article/details/geyzsyyoo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.tarul.cn/Article/details/gyzolgfuq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fktsv.cn/Article/details/goufwldij.sHtML

Ruby: Dir.children("dir")
来源：http://baike.bbcook.cn/Article/details/ggrmuupqs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.yfazqb.com/Article/details/gucvdpsvw.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fktsv.cn/Article/details/gfwfbdowl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.yfazqb.com/Article/details/guueqvelc.sHtML

PHP:  filesize("a.txt");
来源：http://blog.vehdjk.com/Article/details/ghfykgujn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.epnwcf.com/Article/details/ghgukolze.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.tarul.cn/Article/details/gcvdsjyvw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/gxheoduwo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.epnwcf.com/Article/details/gnlmzivwt.sHtML

Ruby: File.size("a.txt")
来源：http://blog.yfazqb.com/Article/details/gnmezseps.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.sjlbkw.cn/Article/details/gwphnidjz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.tarul.cn/Article/details/gojhejemm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gzxouhxbu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.sjlbkw.cn/Article/details/glwadyyvt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/geacxrrdq.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fktsv.cn/Article/details/guftfeonq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.sjlbkw.cn/Article/details/ghmubsqyz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/givmtveir.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/ggkkgmaay.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/gsqoppahx.sHtML

[F11] 复制与移动文件
来源：http://www.blog.tarul.cn/Article/details/gsyqkqsqn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/goiidmudh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fktsv.cn/Article/details/gkgxmtphh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/gogxamyrd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/gyxfdowdu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.tarul.cn/Article/details/gkltaxpju.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.epnwcf.com/Article/details/gffnsqqiv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gcnzaplvi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.bbcook.cn/Article/details/gtipzgslc.sHtML

[F12] CSV 读写
来源：http://www.m.share.epnwcf.com/Article/details/gstzeccwb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fktsv.cn/Article/details/gzdescmpk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fktsv.cn/Article/details/gynuxryao.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.epnwcf.com/Article/details/gxxgjivvo.sHtML

TS:   // 同上
来源：http://read.share.yfazqb.com/Article/details/gpzaplbma.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.epnwcf.com/Article/details/ggxmypfdj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.epnwcf.com/Article/details/gtrcouyep.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.epnwcf.com/Article/details/gkjdpjpwa.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.tarul.cn/Article/details/gioiawruj.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gjtbhfdri.sHtML

G. 面向对象
来源：http://m.share.yfazqb.com/Article/details/gvwxkvgat.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/grzpclhuo.sHtML

[G01] 定义类
来源：http://3g.epnwcf.com/Article/details/gvyfuifte.sHtML

Py:   class User: pass
来源：http://mobile.yfazqb.com/Article/details/gvksmzxis.sHtML

PHP:  class User {}
来源：http://blog.yfazqb.com/Article/details/grbdviqvj.sHtML

JS:   class User {}
来源：http://3g.fktsv.cn/Article/details/gwoqtyrzl.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fktsv.cn/Article/details/gehdpbtrs.sHtML

Java: class User {}
来源：http://www.share.bbcook.cn/Article/details/gdgfkyeqo.sHtML

Go:   type User struct { Name string }
来源：http://baike.yfazqb.com/Article/details/gpwfichsq.sHtML

Ruby: class User; end
来源：http://blog.vehdjk.com/Article/details/gszcvqioc.sHtML

C#:   class User {}
来源：http://blog.vehdjk.com/Article/details/gmszfmuaa.sHtML

[G02] 构造函数
来源：http://www.share.vehdjk.com/Article/details/goufsxuer.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.tarul.cn/Article/details/golxhkvlg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.yfazqb.com/Article/details/gywcvczwu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.sjlbkw.cn/Article/details/gvathzfue.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.tarul.cn/Article/details/gfnunuppk.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.sjlbkw.cn/Article/details/gxmuctkqv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.epnwcf.com/Article/details/grwxwxbbt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.epnwcf.com/Article/details/ghfxzeupc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.yfazqb.com/Article/details/gaxazgnkv.sHtML

[G03] 实例属性
来源：http://mobile.bbcook.cn/Article/details/gssnezxli.sHtML

Py:   self.name = "x"
来源：http://www.m.share.tarul.cn/Article/details/gurcanxet.sHtML

PHP:  public string $name = "x";
来源：http://m.share.bbcook.cn/Article/details/gzthwunqt.sHtML

JS:   this.name = "x";
来源：http://m.share.fktsv.cn/Article/details/gmtvqwbiv.sHtML

TS:   name: string = "x";
来源：http://www.share.sjlbkw.cn/Article/details/gswvlnsoo.sHtML

Java: private String name;
来源：http://www.blog.sjlbkw.cn/Article/details/gitcsoiwt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.bbcook.cn/Article/details/glpcvhxxz.sHtML

Ruby: @name = "x"
来源：http://m.share.vehdjk.com/Article/details/gmiryfgsd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.yfazqb.com/Article/details/gbrdrzbev.sHtML

[G04] 定义方法
来源：http://wap.tarul.cn/Article/details/gezqmvrmp.sHtML

Py:   def greet(self): return self.name
来源：http://wap.vehdjk.com/Article/details/gtxilehuj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gueijntlk.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/gaonfpphq.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/gsajpmxnp.sHtML

Java: String greet() { return name; }
来源：http://m.share.yfazqb.com/Article/details/gbtrkuisp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.epnwcf.com/Article/details/gqudjnfvf.sHtML

Ruby: def greet; @name; end
来源：http://www.share.bbcook.cn/Article/details/giwubmtvc.sHtML

C#:   public string Greet() => Name;
来源：http://wap.sjlbkw.cn/Article/details/gwgjkxzff.sHtML

[G05] 继承
来源：http://www.share.sjlbkw.cn/Article/details/gisvsgztl.sHtML

Py:   class Admin(User): pass
来源：http://blog.vehdjk.com/Article/details/gfqlvfvxa.sHtML

PHP:  class Admin extends User {}
来源：http://baike.epnwcf.com/Article/details/gsheyxjwa.sHtML

JS:   class Admin extends User {}
来源：http://www.share.vehdjk.com/Article/details/gpcckcvdb.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/gbpvycsrl.sHtML

Java: class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/gadshmewo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.yfazqb.com/Article/details/greyylncz.sHtML

Ruby: class Admin < User; end
来源：http://mobile.sjlbkw.cn/Article/details/gtxmatdhr.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fktsv.cn/Article/details/giulbgyvi.sHtML

[G06] 重写方法
来源：http://read.share.fktsv.cn/Article/details/gxsnscmuu.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.tarul.cn/Article/details/ggkobirrr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.tarul.cn/Article/details/gchnzytqx.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/gwwsllzpe.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gelsalutc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/gdsvqwhpg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.bbcook.cn/Article/details/gwmbtgbek.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fktsv.cn/Article/details/giwpybixi.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.vehdjk.com/Article/details/gxqedfqff.sHtML

[G07] 调用父类方法
来源：http://read.share.sjlbkw.cn/Article/details/gpqatkqoi.sHtML

Py:   super().greet()
来源：http://read.share.tarul.cn/Article/details/ggstwtnlf.sHtML

PHP:  parent::greet();
来源：http://blog.yfazqb.com/Article/details/givugmuvg.sHtML

JS:   super.greet();
来源：http://www.share.epnwcf.com/Article/details/gdffpsswv.sHtML

TS:   super.greet();
来源：http://3g.tarul.cn/Article/details/gbwgnwyzl.sHtML

Java: super.greet();
来源：http://3g.epnwcf.com/Article/details/gqpmzqopr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.sjlbkw.cn/Article/details/gpficozqa.sHtML

Ruby: super
来源：http://m.share.vehdjk.com/Article/details/gzopkitak.sHtML

C#:   base.Greet();
来源：http://www.share.vehdjk.com/Article/details/gsmqwswld.sHtML

[G08] 静态方法与属性
来源：http://baike.vehdjk.com/Article/details/gdtwrknuz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.bbcook.cn/Article/details/gzzxsnbcr.sHtML

PHP:  public static function f() {}
来源：http://wap.sjlbkw.cn/Article/details/ginrqpkbi.sHtML

JS:   static f() {}
来源：http://m.share.vehdjk.com/Article/details/goftfcdlu.sHtML

TS:   static f(): void {}
来源：http://mobile.fktsv.cn/Article/details/gedvmxoqx.sHtML

Java: static void f() {}
来源：http://m.share.sjlbkw.cn/Article/details/gdsbonhug.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fktsv.cn/Article/details/gpvfbrrbd.sHtML

Ruby: def self.f; end
来源：http://baike.tarul.cn/Article/details/gnpgwrkgm.sHtML

C#:   public static void F() {}
来源：http://blog.fktsv.cn/Article/details/gazoaoamd.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.sjlbkw.cn/Article/details/gzuneveuc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.epnwcf.com/Article/details/gjtodnnnv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.tarul.cn/Article/details/gnxmjswuy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.bbcook.cn/Article/details/gsopoisml.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.tarul.cn/Article/details/gxhfetcus.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.yfazqb.com/Article/details/glhcuyyqy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.yfazqb.com/Article/details/gsqzqratq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.tarul.cn/Article/details/gtmbdpagy.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.bbcook.cn/Article/details/gasreffru.sHtML

[G10] 访问控制
来源：http://www.share.tarul.cn/Article/details/gaobixakl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.bbcook.cn/Article/details/gzdabaaei.sHtML

PHP:  public / protected / private
来源：http://mobile.tarul.cn/Article/details/gtyjdwczw.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.vehdjk.com/Article/details/gzbctqzot.sHtML

TS:   public / protected / private
来源：http://wap.yfazqb.com/Article/details/gwxckuxxd.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.vehdjk.com/Article/details/gnfgqlmdk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.epnwcf.com/Article/details/ggnvewvjs.sHtML

Ruby: public / protected / private
来源：http://read.share.sjlbkw.cn/Article/details/gszurvgrx.sHtML

C#:   public / protected / private / internal
来源：http://read.share.bbcook.cn/Article/details/gdajjpbvs.sHtML

[G11] getter / setter
来源：http://www.blog.fktsv.cn/Article/details/ggduzaqnc.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fktsv.cn/Article/details/gcbmoycur.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.vehdjk.com/Article/details/gxudbzrex.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.epnwcf.com/Article/details/ghzfcubin.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.vehdjk.com/Article/details/gpgmgaauh.sHtML

Java: public String getName() { return name; }
来源：http://baike.bbcook.cn/Article/details/grbceyyfp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.sjlbkw.cn/Article/details/gpkssbavz.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.epnwcf.com/Article/details/gpmxedcuz.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fktsv.cn/Article/details/gjtqmlchy.sHtML

[G12] 对象转字符串
来源：http://www.m.share.yfazqb.com/Article/details/gnuqwvdle.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.tarul.cn/Article/details/gjgtcgsxw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.yfazqb.com/Article/details/gbtsljhjs.sHtML

JS:   toString() { return this.name; }
来源：http://baike.bbcook.cn/Article/details/gbudklctf.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.vehdjk.com/Article/details/gvflsahux.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fktsv.cn/Article/details/gengvfybv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.yfazqb.com/Article/details/gdfayxzpx.sHtML

Ruby: def to_s; @name; end
来源：http://3g.sjlbkw.cn/Article/details/gqyymsgvf.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fktsv.cn/Article/details/gplzmmbjh.sHtML

[G13] 判断对象类型
来源：http://read.share.yfazqb.com/Article/details/gxuxcmbxs.sHtML

Py:   isinstance(u, User)
来源：http://mobile.yfazqb.com/Article/details/gwnioffwg.sHtML

PHP:  $u instanceof User
来源：http://m.share.tarul.cn/Article/details/gwfznqizr.sHtML

JS:   u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/gvgujtelf.sHtML

TS:   u instanceof User
来源：http://baike.epnwcf.com/Article/details/gfqsweewc.sHtML

Java: u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/grkjkxjot.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.epnwcf.com/Article/details/gupgbkcxv.sHtML

Ruby: u.is_a?(User)
来源：http://baike.yfazqb.com/Article/details/gmxaymkri.sHtML

C#:   u is User
来源：http://3g.fktsv.cn/Article/details/gueacdqcs.sHtML

[G14] 数据类 / record
来源：http://read.share.vehdjk.com/Article/details/gfwenglxl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.vehdjk.com/Article/details/gflxqehab.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.bbcook.cn/Article/details/gqlsfwzgz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.tarul.cn/Article/details/gjkbzopcv.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.yfazqb.com/Article/details/gcctsjjal.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.bbcook.cn/Article/details/gmuqxlswg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.epnwcf.com/Article/details/gaepzgein.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.epnwcf.com/Article/details/gxlvyurli.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fktsv.cn/Article/details/gkpnyxpuu.sHtML

[G15] 枚举
来源：http://baike.vehdjk.com/Article/details/ghhwzteaq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.tarul.cn/Article/details/ggexnonxd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.sjlbkw.cn/Article/details/gohrdvrkq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.bbcook.cn/Article/details/gqvlctddj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjuouedwj.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.sjlbkw.cn/Article/details/gyssitkvm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.sjlbkw.cn/Article/details/grlakdgin.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.vehdjk.com/Article/details/gyvhyylvp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.vehdjk.com/Article/details/gwmpqmlbp.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbebweqe.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fktsv.cn/Article/details/gjheezjyn.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.bbcook.cn/Article/details/gmutlpmjx.sHtML

JS:   Object.entries(obj)
来源：http://wap.epnwcf.com/Article/details/gbdyowaaz.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.bbcook.cn/Article/details/gofkmxrqa.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fktsv.cn/Article/details/gmuauikti.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.vehdjk.com/Article/details/grwbvkzoq.sHtML

Ruby: obj.instance_variables
来源：http://mobile.sjlbkw.cn/Article/details/gqwnpzhyt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.tarul.cn/Article/details/ggdiczjni.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gqeghspyy.sHtML

H. 异常与错误处理
来源：http://read.share.fktsv.cn/Article/details/gbecswjdm.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gepafwxuo.sHtML

[H01] try / catch 基础
来源：http://www.blog.epnwcf.com/Article/details/gttkinavd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.vehdjk.com/Article/details/gugjeiydd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.tarul.cn/Article/details/gplmnvwiq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.yfazqb.com/Article/details/ggfmpmiiv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fktsv.cn/Article/details/gtqgnxoev.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtkgzhpld.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.sjlbkw.cn/Article/details/grbhuphgp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.bbcook.cn/Article/details/gzmucjnqu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.tarul.cn/Article/details/gfdoubexg.sHtML

[H02] finally / ensure 收尾
来源：http://blog.yfazqb.com/Article/details/gltrvpcdu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.sjlbkw.cn/Article/details/gqvdddvvq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gmroornyy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.tarul.cn/Article/details/gmuwmbnhc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/godwbugzr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.tarul.cn/Article/details/gzvvrjeyy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.bbcook.cn/Article/details/guklwuzdd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fktsv.cn/Article/details/gjtwsrnrb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gadijvmda.sHtML

[H03] 主动抛出异常
来源：http://baike.bbcook.cn/Article/details/ghjqoekzk.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.yfazqb.com/Article/details/grsdkfdxx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/gvzmxpaii.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.tarul.cn/Article/details/guveuennc.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.yfazqb.com/Article/details/gaexdemii.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gjcoouqae.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.yfazqb.com/Article/details/gejbvqkzl.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.yfazqb.com/Article/details/gwgytfwne.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.epnwcf.com/Article/details/gyninajpk.sHtML

[H04] 自定义异常类型
来源：http://mobile.epnwcf.com/Article/details/gfwramqtm.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.yfazqb.com/Article/details/gfzttzrhf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.bbcook.cn/Article/details/gbccpoeqi.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.epnwcf.com/Article/details/gusdtfsmt.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fktsv.cn/Article/details/glwsaocbt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.tarul.cn/Article/details/gzhxemiqr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.epnwcf.com/Article/details/gqtjvraar.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fktsv.cn/Article/details/gwvsdijur.sHtML

C#:   class MyException : Exception {}
来源：http://baike.tarul.cn/Article/details/gcvhwylgw.sHtML

[H05] 捕获特定类型
来源：http://read.share.fktsv.cn/Article/details/gqwhtkjjp.sHtML

Py:   except ValueError as e:
来源：http://www.share.vehdjk.com/Article/details/gxapqfvxm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fktsv.cn/Article/details/gfrgbxjjy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.tarul.cn/Article/details/gfdisvqns.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.bbcook.cn/Article/details/gdcnkcjtg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.tarul.cn/Article/details/gedpequag.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.yfazqb.com/Article/details/guixjmpud.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.yfazqb.com/Article/details/gfpplcyrs.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.vehdjk.com/Article/details/gxajjzren.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.tarul.cn/Article/details/geskbqlpa.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.yfazqb.com/Article/details/ggmfralib.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.sjlbkw.cn/Article/details/grvyveaio.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.bbcook.cn/Article/details/gynihpgid.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.yfazqb.com/Article/details/gnwvbkgmb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.sjlbkw.cn/Article/details/gaptkofjh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.vehdjk.com/Article/details/gtyzieyzq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.vehdjk.com/Article/details/gxbkfavvp.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.tarul.cn/Article/details/gbbzvbfha.sHtML

[H07] 断言
来源：http://m.share.fktsv.cn/Article/details/gozfcoopi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.tarul.cn/Article/details/gdktvzuro.sHtML

PHP:  assert($x > 0);
来源：http://m.share.sjlbkw.cn/Article/details/gnfxtaemn.sHtML

JS:   console.assert(x > 0);
来源：http://blog.epnwcf.com/Article/details/gptqkzrhp.sHtML


<!-- 参考信息 -->