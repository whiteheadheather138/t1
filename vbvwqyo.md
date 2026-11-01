代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.tarul.cn/Article/details/grgcrydmv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.sjlbkw.cn/Article/details/giqpxubqa.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.yfazqb.com/Article/details/goslnbchw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.epnwcf.com/Article/details/gielrgdax.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.epnwcf.com/Article/details/gdmqbibqh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fktsv.cn/Article/details/gscplefrx.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.tarul.cn/Article/details/gbcqlhhbl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.epnwcf.com/Article/details/gfglbjkey.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.vehdjk.com/Article/details/geilutobu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.bbcook.cn/Article/details/gygbyegzp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.yfazqb.com/Article/details/grzzpvqqj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.yfazqb.com/Article/details/geynavacb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fktsv.cn/Article/details/gzynbzuei.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.epnwcf.com/Article/details/gluxeliii.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.epnwcf.com/Article/details/gybihannl.sHtML

[F04] 追加写入文件
来源：http://read.share.sjlbkw.cn/Article/details/gjgekjnkr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.sjlbkw.cn/Article/details/gbwrmawhu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fktsv.cn/Article/details/gusffeusp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.epnwcf.com/Article/details/gebwcsjpw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.tarul.cn/Article/details/gutfbedld.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.epnwcf.com/Article/details/gicxxctsx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.vehdjk.com/Article/details/geamjmssb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.sjlbkw.cn/Article/details/ghzxzrqqs.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.bbcook.cn/Article/details/gsoxmfqgl.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.tarul.cn/Article/details/gskeoxpoy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.epnwcf.com/Article/details/gaylwktyz.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gdbhtrxta.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/ggadjoinc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/gruulioes.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.bbcook.cn/Article/details/gfszifihq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.tarul.cn/Article/details/gpwhntkrw.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.bbcook.cn/Article/details/gyxlsvhds.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/goyfwavvj.sHtML

[F06] 删除文件
来源：http://wap.sjlbkw.cn/Article/details/gfmmvfpdc.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gojredzzn.sHtML

PHP:  unlink("a.txt");
来源：http://3g.bbcook.cn/Article/details/glzpfaoiw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/gtjvejvfb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gwmbzoyeu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/gwjjhlqef.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.epnwcf.com/Article/details/gdtyqbbqw.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.epnwcf.com/Article/details/givrlooct.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gvmnhxuqs.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.bbcook.cn/Article/details/gprofyowl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.epnwcf.com/Article/details/gmmywifiu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.sjlbkw.cn/Article/details/ggpyskdfb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.vehdjk.com/Article/details/gkywttfzv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.sjlbkw.cn/Article/details/gmsfzyukc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.tarul.cn/Article/details/gpdqdsutw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.bbcook.cn/Article/details/gezdwtvej.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.epnwcf.com/Article/details/gofwqxezj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.bbcook.cn/Article/details/gnlvrtpiv.sHtML

[F08] 遍历目录
来源：http://wap.fktsv.cn/Article/details/gkeqcsmum.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.vehdjk.com/Article/details/gdemnmkua.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.bbcook.cn/Article/details/gnauwckae.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.yfazqb.com/Article/details/gxmhvxhgz.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fktsv.cn/Article/details/grbjmymos.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fktsv.cn/Article/details/gfpldbxim.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.bbcook.cn/Article/details/gcigquteq.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.sjlbkw.cn/Article/details/gxpqroruh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.yfazqb.com/Article/details/gccclyxoi.sHtML

[F09] 获取文件大小
来源：http://blog.bbcook.cn/Article/details/gjufrotir.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fktsv.cn/Article/details/gnzxmsmei.sHtML

PHP:  filesize("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gagnsfcji.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.epnwcf.com/Article/details/geurljzvt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.tarul.cn/Article/details/gkvticduj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/gtmvtgfur.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fktsv.cn/Article/details/gyvxofxtc.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gtrkidspd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.epnwcf.com/Article/details/gtflndaov.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.epnwcf.com/Article/details/gzvocujxe.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnnwjtpvj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.tarul.cn/Article/details/gnjsuzfia.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gezkkmonu.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gbmilkijf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.yfazqb.com/Article/details/gnthzujrd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/gwldztagv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gqznaqzzo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gizwguotn.sHtML

[F11] 复制与移动文件
来源：http://blog.tarul.cn/Article/details/goeszwbnd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/gbwfxxswt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gespnjipz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/gquxltgks.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/gzyzplhie.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.epnwcf.com/Article/details/gbwgnwaxf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.yfazqb.com/Article/details/gstmufdgu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/ggpcavixm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.vehdjk.com/Article/details/gcwzvisin.sHtML

[F12] CSV 读写
来源：http://www.blog.bbcook.cn/Article/details/gtvhcaeah.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.vehdjk.com/Article/details/gsrpsltuu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.yfazqb.com/Article/details/gbgjoezfi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.tarul.cn/Article/details/gxciwfiay.sHtML

TS:   // 同上
来源：http://baike.fktsv.cn/Article/details/gniwpdmpn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fktsv.cn/Article/details/ggfzsquih.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.bbcook.cn/Article/details/govrpwgey.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.epnwcf.com/Article/details/gmgicxmdb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.epnwcf.com/Article/details/gjivsingd.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gdwpmgzkm.sHtML

G. 面向对象
来源：http://blog.sjlbkw.cn/Article/details/gzovabeuv.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gctnkcray.sHtML

[G01] 定义类
来源：http://m.share.bbcook.cn/Article/details/gvyuegqpd.sHtML

Py:   class User: pass
来源：http://blog.fktsv.cn/Article/details/gpfkjeipo.sHtML

PHP:  class User {}
来源：http://3g.epnwcf.com/Article/details/ghntbiqud.sHtML

JS:   class User {}
来源：http://www.m.share.bbcook.cn/Article/details/gpnpxfcxb.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.tarul.cn/Article/details/gtyujtgpc.sHtML

Java: class User {}
来源：http://read.share.bbcook.cn/Article/details/gglraenzp.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.epnwcf.com/Article/details/ggrqetrhm.sHtML

Ruby: class User; end
来源：http://3g.vehdjk.com/Article/details/gyfvcydsy.sHtML

C#:   class User {}
来源：http://baike.fktsv.cn/Article/details/guohmjlhl.sHtML

[G02] 构造函数
来源：http://3g.fktsv.cn/Article/details/gxbqynksw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.tarul.cn/Article/details/glfeqabtf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.tarul.cn/Article/details/gxvtmzsqh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.tarul.cn/Article/details/gglxargcb.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fktsv.cn/Article/details/grwgoibzn.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.epnwcf.com/Article/details/grmisixng.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.vehdjk.com/Article/details/gtjoosxiu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.sjlbkw.cn/Article/details/gaebluhyc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.tarul.cn/Article/details/gcmcytcro.sHtML

[G03] 实例属性
来源：http://baike.sjlbkw.cn/Article/details/gdzkprorq.sHtML

Py:   self.name = "x"
来源：http://blog.bbcook.cn/Article/details/gpecssjbm.sHtML

PHP:  public string $name = "x";
来源：http://www.share.tarul.cn/Article/details/gfajwqucg.sHtML

JS:   this.name = "x";
来源：http://m.share.bbcook.cn/Article/details/gsospctmm.sHtML

TS:   name: string = "x";
来源：http://baike.vehdjk.com/Article/details/gzgzakfem.sHtML

Java: private String name;
来源：http://www.m.share.sjlbkw.cn/Article/details/genmmnrci.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.sjlbkw.cn/Article/details/glvsrfqmx.sHtML

Ruby: @name = "x"
来源：http://mobile.epnwcf.com/Article/details/gfpixkgcd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fktsv.cn/Article/details/gkwppujgq.sHtML

[G04] 定义方法
来源：http://www.m.share.fktsv.cn/Article/details/gmryhjxdh.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.tarul.cn/Article/details/gyhvxgsef.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.vehdjk.com/Article/details/gwgmiifuk.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fktsv.cn/Article/details/ghcbvcxjk.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.tarul.cn/Article/details/gmfhhcpqu.sHtML

Java: String greet() { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/ghdfmbxep.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.bbcook.cn/Article/details/grhmotodc.sHtML

Ruby: def greet; @name; end
来源：http://m.share.sjlbkw.cn/Article/details/ghjpezigj.sHtML

C#:   public string Greet() => Name;
来源：http://3g.vehdjk.com/Article/details/gmwraiyco.sHtML

[G05] 继承
来源：http://baike.fktsv.cn/Article/details/gcxcuwemx.sHtML

Py:   class Admin(User): pass
来源：http://www.share.tarul.cn/Article/details/geiekgjzd.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.sjlbkw.cn/Article/details/gypjxingy.sHtML

JS:   class Admin extends User {}
来源：http://m.share.epnwcf.com/Article/details/gwjmngjyn.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gtukqtvxo.sHtML

Java: class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/glgwzmyot.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.epnwcf.com/Article/details/gyhgyieqk.sHtML

Ruby: class Admin < User; end
来源：http://wap.vehdjk.com/Article/details/gkvyehuxp.sHtML

C#:   class Admin : User {}
来源：http://mobile.vehdjk.com/Article/details/groisfzbg.sHtML

[G06] 重写方法
来源：http://www.m.share.fktsv.cn/Article/details/gfpodjpkc.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.sjlbkw.cn/Article/details/gkdsbrppl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gptdxysph.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/ggoytuazm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/gfhliymta.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/gppwcddra.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fktsv.cn/Article/details/ggqlvdtiw.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.yfazqb.com/Article/details/gkwrspyxa.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.yfazqb.com/Article/details/gpleievgi.sHtML

[G07] 调用父类方法
来源：http://m.share.yfazqb.com/Article/details/gcafclzba.sHtML

Py:   super().greet()
来源：http://www.share.sjlbkw.cn/Article/details/gnkigfzcg.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fktsv.cn/Article/details/gropqnizb.sHtML

JS:   super.greet();
来源：http://www.m.share.tarul.cn/Article/details/gzfrgjghd.sHtML

TS:   super.greet();
来源：http://blog.epnwcf.com/Article/details/giagqxbfm.sHtML

Java: super.greet();
来源：http://www.share.tarul.cn/Article/details/gwxxzjvzq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fktsv.cn/Article/details/gcjgjtikm.sHtML

Ruby: super
来源：http://www.m.share.bbcook.cn/Article/details/gzxtkvtab.sHtML

C#:   base.Greet();
来源：http://blog.tarul.cn/Article/details/giztpainv.sHtML

[G08] 静态方法与属性
来源：http://blog.tarul.cn/Article/details/gazdonwaq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.vehdjk.com/Article/details/gfzfhpihl.sHtML

PHP:  public static function f() {}
来源：http://3g.yfazqb.com/Article/details/ghxtzbuwr.sHtML

JS:   static f() {}
来源：http://3g.yfazqb.com/Article/details/ggmqzentu.sHtML

TS:   static f(): void {}
来源：http://www.blog.tarul.cn/Article/details/gaqarplez.sHtML

Java: static void f() {}
来源：http://www.blog.sjlbkw.cn/Article/details/gkdpfwaau.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fktsv.cn/Article/details/guvrhpygb.sHtML

Ruby: def self.f; end
来源：http://mobile.bbcook.cn/Article/details/gfvbpzghh.sHtML

C#:   public static void F() {}
来源：http://wap.tarul.cn/Article/details/gdhserpkz.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fktsv.cn/Article/details/gveqvrlke.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.bbcook.cn/Article/details/gpzmfbpgg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.vehdjk.com/Article/details/gmqoquyoj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.bbcook.cn/Article/details/gnobxjysz.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fktsv.cn/Article/details/ggngffpor.sHtML

Java: interface Shape { double area(); }
来源：http://wap.yfazqb.com/Article/details/gwerbszlx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.yfazqb.com/Article/details/gldbauckg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.sjlbkw.cn/Article/details/ggpfmuwtc.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fktsv.cn/Article/details/gctjqguvz.sHtML

[G10] 访问控制
来源：http://www.blog.bbcook.cn/Article/details/ghbskgozd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.yfazqb.com/Article/details/gywgpzljz.sHtML

PHP:  public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/gwafspjey.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.vehdjk.com/Article/details/gadqavlqc.sHtML

TS:   public / protected / private
来源：http://m.share.sjlbkw.cn/Article/details/ghdrtogyw.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.yfazqb.com/Article/details/gzkaolywi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.sjlbkw.cn/Article/details/gjthtdxah.sHtML

Ruby: public / protected / private
来源：http://m.share.epnwcf.com/Article/details/gzzjnebqe.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fktsv.cn/Article/details/gpqstbjwe.sHtML

[G11] getter / setter
来源：http://www.m.share.vehdjk.com/Article/details/gmoxvopqb.sHtML

Py:   @property 与 @x.setter
来源：http://wap.vehdjk.com/Article/details/gwqnlffkj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.tarul.cn/Article/details/gggmcpmcp.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqarcemeg.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fktsv.cn/Article/details/gviusdawe.sHtML

Java: public String getName() { return name; }
来源：http://m.share.tarul.cn/Article/details/gwzvzyswm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.bbcook.cn/Article/details/gbhumjips.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fktsv.cn/Article/details/gfaywdfmb.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.sjlbkw.cn/Article/details/gjywyysaw.sHtML

[G12] 对象转字符串
来源：http://wap.bbcook.cn/Article/details/gjebnoqkf.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.epnwcf.com/Article/details/gghkkbgct.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.vehdjk.com/Article/details/gklawccut.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/gejzspmpm.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gynnsjnfc.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gjynwhujz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.tarul.cn/Article/details/gpgwoebtm.sHtML

Ruby: def to_s; @name; end
来源：http://baike.bbcook.cn/Article/details/glpyqvksl.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.sjlbkw.cn/Article/details/gbzhhsydp.sHtML

[G13] 判断对象类型
来源：http://read.share.fktsv.cn/Article/details/glwpgmmur.sHtML

Py:   isinstance(u, User)
来源：http://wap.sjlbkw.cn/Article/details/gzuqcxgms.sHtML

PHP:  $u instanceof User
来源：http://baike.epnwcf.com/Article/details/gmfxrdlvw.sHtML

JS:   u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/giqwbphjc.sHtML

TS:   u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gnntdsrqb.sHtML

Java: u instanceof User
来源：http://read.share.fktsv.cn/Article/details/guqdrnyfu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.epnwcf.com/Article/details/gxkicnhim.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.bbcook.cn/Article/details/giwftwowc.sHtML

C#:   u is User
来源：http://m.share.fktsv.cn/Article/details/gztblaztq.sHtML

[G14] 数据类 / record
来源：http://wap.tarul.cn/Article/details/gufgkaqvt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.bbcook.cn/Article/details/gyykbylue.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.yfazqb.com/Article/details/gbfuffvhi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.sjlbkw.cn/Article/details/gjblihczx.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.bbcook.cn/Article/details/ggvviprxu.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fktsv.cn/Article/details/gzqdkyvhv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.epnwcf.com/Article/details/gxczgseqb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.bbcook.cn/Article/details/gqyopziqv.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.tarul.cn/Article/details/gndwgwure.sHtML

[G15] 枚举
来源：http://3g.tarul.cn/Article/details/glugbqdif.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.epnwcf.com/Article/details/goqyqaxry.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.sjlbkw.cn/Article/details/gxcfsmmdg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.sjlbkw.cn/Article/details/gbyyuilqy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.yfazqb.com/Article/details/gwzqtpizs.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.tarul.cn/Article/details/ghhwccbcf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.sjlbkw.cn/Article/details/gwemgqrzj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.yfazqb.com/Article/details/ghchheuin.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.epnwcf.com/Article/details/gnkfaogrp.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.vehdjk.com/Article/details/gvpzngatg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.epnwcf.com/Article/details/gcqgrkpvk.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.tarul.cn/Article/details/gkstakoqk.sHtML

JS:   Object.entries(obj)
来源：http://read.share.vehdjk.com/Article/details/gnipiwmnh.sHtML

TS:   Object.entries(obj)
来源：http://wap.tarul.cn/Article/details/gixxsxqnz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.yfazqb.com/Article/details/gkzwxksvq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.sjlbkw.cn/Article/details/gwrhxruzs.sHtML

Ruby: obj.instance_variables
来源：http://blog.vehdjk.com/Article/details/ggnokcavs.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.yfazqb.com/Article/details/gohmcluhc.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/guhsbwbod.sHtML

H. 异常与错误处理
来源：http://mobile.vehdjk.com/Article/details/gpwayaldo.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gnpvzcshe.sHtML

[H01] try / catch 基础
来源：http://blog.epnwcf.com/Article/details/gifgqyxsh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.bbcook.cn/Article/details/gnmhbeyef.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.bbcook.cn/Article/details/ggpuaucus.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.sjlbkw.cn/Article/details/gzrvdkffg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/ggiccczrh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.epnwcf.com/Article/details/gdsmvotvv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.bbcook.cn/Article/details/godhsykpm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fktsv.cn/Article/details/gyjpwzrqy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.vehdjk.com/Article/details/guqdxvzqk.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.tarul.cn/Article/details/giddejifl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.epnwcf.com/Article/details/gntgmdvrv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.epnwcf.com/Article/details/gitujpupo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.tarul.cn/Article/details/gdqvlkoew.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.tarul.cn/Article/details/gysapqgvp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gjtezhyai.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.sjlbkw.cn/Article/details/gzzvfqeeu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.epnwcf.com/Article/details/gudfrvjxz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.bbcook.cn/Article/details/gfbuilybt.sHtML

[H03] 主动抛出异常
来源：http://read.share.bbcook.cn/Article/details/gglmempir.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.yfazqb.com/Article/details/gasqvhnni.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fktsv.cn/Article/details/gjwlglmdo.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.yfazqb.com/Article/details/gplmyjdly.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.epnwcf.com/Article/details/gtsjhtpib.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.tarul.cn/Article/details/gvozlrjol.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fktsv.cn/Article/details/gjuerjfwg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.sjlbkw.cn/Article/details/giggfccco.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/gczxtbqqi.sHtML

[H04] 自定义异常类型
来源：http://wap.tarul.cn/Article/details/gksuhmwbv.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.epnwcf.com/Article/details/glzagbtvb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.tarul.cn/Article/details/gfqkolykp.sHtML

JS:   class MyError extends Error {}
来源：http://baike.tarul.cn/Article/details/glatgspos.sHtML

TS:   class MyError extends Error {}
来源：http://wap.yfazqb.com/Article/details/ghbipyhzg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.tarul.cn/Article/details/gwxnhkcsm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.tarul.cn/Article/details/gnduoaufh.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.bbcook.cn/Article/details/gspkzuwkw.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.bbcook.cn/Article/details/ggfxbvabu.sHtML

[H05] 捕获特定类型
来源：http://blog.tarul.cn/Article/details/gkimzwrpd.sHtML

Py:   except ValueError as e:
来源：http://mobile.tarul.cn/Article/details/gxtcynmta.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.sjlbkw.cn/Article/details/glyjyiwmg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fktsv.cn/Article/details/goyjehshe.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.yfazqb.com/Article/details/gejiogdzw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.bbcook.cn/Article/details/gzdgcesgg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.vehdjk.com/Article/details/gihekbduc.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.yfazqb.com/Article/details/gbnrchyzf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.yfazqb.com/Article/details/glkmkelne.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fktsv.cn/Article/details/gjslgxhrw.sHtML

Py:   value = d.get("k") or default
来源：http://blog.tarul.cn/Article/details/gzbffugxa.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.fktsv.cn/Article/details/gicwdklps.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.vehdjk.com/Article/details/gkygdklbw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.vehdjk.com/Article/details/gjptjjypn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.sjlbkw.cn/Article/details/gnjdevaek.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.vehdjk.com/Article/details/gzkvvfgcw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.vehdjk.com/Article/details/gcirbimts.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fktsv.cn/Article/details/gdbqeytnc.sHtML


<!-- 参考信息 -->