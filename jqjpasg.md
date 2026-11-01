代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gycyrytnb.sHtML

[F02] 逐行读取文件
来源：http://baike.yfazqb.com/Article/details/gpmmljeth.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.yfazqb.com/Article/details/geiafjcih.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.vehdjk.com/Article/details/gxxffjqwl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fktsv.cn/Article/details/gflmyaqjo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.sjlbkw.cn/Article/details/grjlkoqxt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.vehdjk.com/Article/details/ghahxuakr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.yfazqb.com/Article/details/gjugaunjf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.yfazqb.com/Article/details/gakdcuqnm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.tarul.cn/Article/details/gjcnzoegf.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.tarul.cn/Article/details/gtfaxahcz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fktsv.cn/Article/details/gssgjdakg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fktsv.cn/Article/details/gibvznhee.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.yfazqb.com/Article/details/ghpkasoap.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.vehdjk.com/Article/details/gzyjirski.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.epnwcf.com/Article/details/gyuamyqoi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.vehdjk.com/Article/details/gpahzymwm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.bbcook.cn/Article/details/gnejufweq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.bbcook.cn/Article/details/geyfbywbo.sHtML

[F04] 追加写入文件
来源：http://wap.tarul.cn/Article/details/gsuamrwrm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.bbcook.cn/Article/details/gowxnerqk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.tarul.cn/Article/details/gssenfzkh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.tarul.cn/Article/details/gafkuxzkg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.epnwcf.com/Article/details/gysxzeuko.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.bbcook.cn/Article/details/gwgqcnxxt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.bbcook.cn/Article/details/gccslelpq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.sjlbkw.cn/Article/details/gkewxhqxa.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.bbcook.cn/Article/details/gygchxnqs.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.tarul.cn/Article/details/grqchmsjh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fktsv.cn/Article/details/ghxwcjnrs.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gzbqjvwcj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/ggxhrgmtw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/gxbapekai.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.vehdjk.com/Article/details/gjmkuruwv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.yfazqb.com/Article/details/gwokaskcu.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/giahigbva.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.bbcook.cn/Article/details/ggrbgezuu.sHtML

[F06] 删除文件
来源：http://www.share.bbcook.cn/Article/details/gdkezdxyo.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.tarul.cn/Article/details/ggmxrxrsc.sHtML

PHP:  unlink("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gnrstguts.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.tarul.cn/Article/details/gvwhqmgsj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/gkwasrmfp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.vehdjk.com/Article/details/gztmzsyjo.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.tarul.cn/Article/details/gbjqqtkfm.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.tarul.cn/Article/details/gtifhpgpm.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.bbcook.cn/Article/details/gpcrbbflk.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.epnwcf.com/Article/details/gpohsyxmt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjudvedj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fktsv.cn/Article/details/gsomrdhww.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.tarul.cn/Article/details/gzggrtiwo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.vehdjk.com/Article/details/gqdbchhsn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.sjlbkw.cn/Article/details/grxhbmulv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.epnwcf.com/Article/details/glknchwem.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.sjlbkw.cn/Article/details/gsvnogakz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.vehdjk.com/Article/details/gpmpuohof.sHtML

[F08] 遍历目录
来源：http://3g.vehdjk.com/Article/details/gcauloxuq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.epnwcf.com/Article/details/gyzgcpnca.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fktsv.cn/Article/details/glumfepwo.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnwrwfmsg.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gjanqxpwx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.bbcook.cn/Article/details/gtqdaprpp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.vehdjk.com/Article/details/gbkvofwyf.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fktsv.cn/Article/details/gyzsllvlv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.epnwcf.com/Article/details/grzmjlqhg.sHtML

[F09] 获取文件大小
来源：http://blog.sjlbkw.cn/Article/details/gkwrccnwa.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gomwhtbiv.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gehhaczsq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fktsv.cn/Article/details/giezeeidc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.vehdjk.com/Article/details/gexeoonnq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fktsv.cn/Article/details/gzooybqby.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.sjlbkw.cn/Article/details/gjcrcjwpf.sHtML

Ruby: File.size("a.txt")
来源：http://baike.vehdjk.com/Article/details/gchubhwcc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.sjlbkw.cn/Article/details/gudckuzjk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.sjlbkw.cn/Article/details/gcgvqgtdw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gjmijmklk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.bbcook.cn/Article/details/gcbxizhko.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gatnbhxow.sHtML

TS:   path.extname("a.txt")
来源：http://wap.bbcook.cn/Article/details/gijkzynle.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fktsv.cn/Article/details/giaegybuk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/goausejij.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gepncuqoj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/gtrrkoqnp.sHtML

[F11] 复制与移动文件
来源：http://m.share.bbcook.cn/Article/details/gckybexju.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/garnqmifg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.bbcook.cn/Article/details/gebzklynf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/gceqhizmk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gciwazxsh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.tarul.cn/Article/details/gsqpdyixz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.bbcook.cn/Article/details/guxntopnw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gjbigztpr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fktsv.cn/Article/details/ggxcqieep.sHtML

[F12] CSV 读写
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmpgpfbo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.sjlbkw.cn/Article/details/gskuanjsn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.tarul.cn/Article/details/gdbkoigfz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.vehdjk.com/Article/details/gmemnykgp.sHtML

TS:   // 同上
来源：http://3g.sjlbkw.cn/Article/details/gzzacvbds.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.epnwcf.com/Article/details/gyshierqp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.bbcook.cn/Article/details/gaxqchrpb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.epnwcf.com/Article/details/gfaspyubf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fktsv.cn/Article/details/gqhujnarj.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gqjfvrajy.sHtML

G. 面向对象
来源：http://www.share.yfazqb.com/Article/details/gcngfncxk.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gotuntnqk.sHtML

[G01] 定义类
来源：http://blog.yfazqb.com/Article/details/giqkruvpb.sHtML

Py:   class User: pass
来源：http://www.m.share.yfazqb.com/Article/details/gxzwsqgta.sHtML

PHP:  class User {}
来源：http://www.share.epnwcf.com/Article/details/gblcjzqzz.sHtML

JS:   class User {}
来源：http://read.share.tarul.cn/Article/details/gfsqvvvwc.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.bbcook.cn/Article/details/gumqowoyl.sHtML

Java: class User {}
来源：http://read.share.vehdjk.com/Article/details/gpyvvwjad.sHtML

Go:   type User struct { Name string }
来源：http://blog.vehdjk.com/Article/details/ghiszlgkr.sHtML

Ruby: class User; end
来源：http://m.share.bbcook.cn/Article/details/gpqccpbym.sHtML

C#:   class User {}
来源：http://mobile.yfazqb.com/Article/details/gffizkisg.sHtML

[G02] 构造函数
来源：http://wap.yfazqb.com/Article/details/goxzkmdwn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.tarul.cn/Article/details/gnongmyvj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.tarul.cn/Article/details/ggzchbzth.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.epnwcf.com/Article/details/gwjbfetyk.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.yfazqb.com/Article/details/gfffbfoam.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.epnwcf.com/Article/details/geccqzceh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.bbcook.cn/Article/details/gpuvoewev.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.bbcook.cn/Article/details/gbydxvasv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjignlwjr.sHtML

[G03] 实例属性
来源：http://m.share.bbcook.cn/Article/details/gnwlhhssc.sHtML

Py:   self.name = "x"
来源：http://mobile.fktsv.cn/Article/details/gcjbjimbp.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.tarul.cn/Article/details/gmyeqixfh.sHtML

JS:   this.name = "x";
来源：http://blog.bbcook.cn/Article/details/gwpjjbjjx.sHtML

TS:   name: string = "x";
来源：http://wap.bbcook.cn/Article/details/gzvgpyrlr.sHtML

Java: private String name;
来源：http://www.blog.vehdjk.com/Article/details/gyqqhuwvl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fktsv.cn/Article/details/gnuavzild.sHtML

Ruby: @name = "x"
来源：http://wap.bbcook.cn/Article/details/gujtvdshk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.tarul.cn/Article/details/gmwvjsvtb.sHtML

[G04] 定义方法
来源：http://www.share.epnwcf.com/Article/details/gbavogzeq.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.yfazqb.com/Article/details/gxhlwlccf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/gnzfdaiyd.sHtML

JS:   greet() { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gjfbvlnta.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.epnwcf.com/Article/details/gvzcurhpg.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gqcqnjvsh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fktsv.cn/Article/details/gwggtknja.sHtML

Ruby: def greet; @name; end
来源：http://baike.epnwcf.com/Article/details/gejswhral.sHtML

C#:   public string Greet() => Name;
来源：http://blog.epnwcf.com/Article/details/gnfwlunnq.sHtML

[G05] 继承
来源：http://www.share.yfazqb.com/Article/details/gtqnyfujt.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.vehdjk.com/Article/details/gkjyziamn.sHtML

PHP:  class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/gpphjlssa.sHtML

JS:   class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/grandekmt.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.tarul.cn/Article/details/gslwimeef.sHtML

Java: class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gajfqqbnu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.epnwcf.com/Article/details/gbmzlypyl.sHtML

Ruby: class Admin < User; end
来源：http://www.share.yfazqb.com/Article/details/gzpjnryjf.sHtML

C#:   class Admin : User {}
来源：http://read.share.epnwcf.com/Article/details/gxclxgoez.sHtML

[G06] 重写方法
来源：http://mobile.vehdjk.com/Article/details/gofckulve.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.epnwcf.com/Article/details/gfuigotqz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.vehdjk.com/Article/details/grwiarjxg.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/gbmdxyphc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gynrnnrov.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gjrwhjcge.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.epnwcf.com/Article/details/gamcyxyek.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.yfazqb.com/Article/details/gntpmhidv.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.epnwcf.com/Article/details/gnupirwej.sHtML

[G07] 调用父类方法
来源：http://read.share.epnwcf.com/Article/details/gjzroykme.sHtML

Py:   super().greet()
来源：http://www.m.share.epnwcf.com/Article/details/gmfsuxyuo.sHtML

PHP:  parent::greet();
来源：http://www.m.share.vehdjk.com/Article/details/ginzlzpfa.sHtML

JS:   super.greet();
来源：http://www.share.fktsv.cn/Article/details/gxwgkddtn.sHtML

TS:   super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/grqkmbojl.sHtML

Java: super.greet();
来源：http://baike.epnwcf.com/Article/details/gqgoxakvk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.epnwcf.com/Article/details/gavrhhkcg.sHtML

Ruby: super
来源：http://blog.tarul.cn/Article/details/ggtxwqbkf.sHtML

C#:   base.Greet();
来源：http://3g.epnwcf.com/Article/details/gysznhevt.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.yfazqb.com/Article/details/gpvvdfhoa.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.vehdjk.com/Article/details/gcxehatvm.sHtML

PHP:  public static function f() {}
来源：http://mobile.bbcook.cn/Article/details/gwmztwiiq.sHtML

JS:   static f() {}
来源：http://read.share.bbcook.cn/Article/details/gyxanndwp.sHtML

TS:   static f(): void {}
来源：http://wap.tarul.cn/Article/details/gxzbsjsbe.sHtML

Java: static void f() {}
来源：http://baike.yfazqb.com/Article/details/ggcqjmeun.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.vehdjk.com/Article/details/gcgpzsgzk.sHtML

Ruby: def self.f; end
来源：http://www.share.bbcook.cn/Article/details/gpkjevyhy.sHtML

C#:   public static void F() {}
来源：http://www.share.vehdjk.com/Article/details/gbmpymocy.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.bbcook.cn/Article/details/glcjsneuh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.vehdjk.com/Article/details/gczlxpwax.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.sjlbkw.cn/Article/details/gtcruwmnb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.sjlbkw.cn/Article/details/gjaexyijw.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.vehdjk.com/Article/details/gvtokukgf.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.epnwcf.com/Article/details/gvidmxlsl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.sjlbkw.cn/Article/details/ghjbdjamk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.sjlbkw.cn/Article/details/gfkouzoyd.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.bbcook.cn/Article/details/gqaxtaddy.sHtML

[G10] 访问控制
来源：http://mobile.bbcook.cn/Article/details/gjtxnobov.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.vehdjk.com/Article/details/gpqhmtlxm.sHtML

PHP:  public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/gaojddgeq.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.yfazqb.com/Article/details/galshzboe.sHtML

TS:   public / protected / private
来源：http://blog.epnwcf.com/Article/details/ghswdsars.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fktsv.cn/Article/details/gtecakfbr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.epnwcf.com/Article/details/ghvshsdzs.sHtML

Ruby: public / protected / private
来源：http://www.share.vehdjk.com/Article/details/gnbirkdfa.sHtML

C#:   public / protected / private / internal
来源：http://blog.tarul.cn/Article/details/gtogtypem.sHtML

[G11] getter / setter
来源：http://www.share.bbcook.cn/Article/details/gzcyiouys.sHtML

Py:   @property 与 @x.setter
来源：http://wap.yfazqb.com/Article/details/glayaenxu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fktsv.cn/Article/details/galmusizt.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fktsv.cn/Article/details/gqjckzzfi.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fktsv.cn/Article/details/guwcbscou.sHtML

Java: public String getName() { return name; }
来源：http://baike.epnwcf.com/Article/details/ggcfkihbv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.yfazqb.com/Article/details/gbuglegia.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.yfazqb.com/Article/details/gzlpcfwwl.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.vehdjk.com/Article/details/ghoeufnjf.sHtML

[G12] 对象转字符串
来源：http://wap.bbcook.cn/Article/details/gwhjfmhyk.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.epnwcf.com/Article/details/gmxxviwjj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.tarul.cn/Article/details/gcfmhnxdw.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.bbcook.cn/Article/details/guffsxbqh.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.epnwcf.com/Article/details/gjbzexrou.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fktsv.cn/Article/details/gtagabpva.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.vehdjk.com/Article/details/gvknaznui.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fktsv.cn/Article/details/gnjzyjpzl.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.sjlbkw.cn/Article/details/gydwteysv.sHtML

[G13] 判断对象类型
来源：http://m.share.tarul.cn/Article/details/gguutgkic.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.bbcook.cn/Article/details/gddgfcngc.sHtML

PHP:  $u instanceof User
来源：http://read.share.epnwcf.com/Article/details/gfszhedfe.sHtML

JS:   u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/gkabtnncs.sHtML

TS:   u instanceof User
来源：http://baike.tarul.cn/Article/details/gxldxhxws.sHtML

Java: u instanceof User
来源：http://mobile.tarul.cn/Article/details/grkmhsaij.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.tarul.cn/Article/details/gawhrxilt.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fktsv.cn/Article/details/gcjydhtcu.sHtML

C#:   u is User
来源：http://wap.bbcook.cn/Article/details/gumnrgrjd.sHtML

[G14] 数据类 / record
来源：http://mobile.bbcook.cn/Article/details/gkivtkbvd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.sjlbkw.cn/Article/details/gzobcmopy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.epnwcf.com/Article/details/gvvjyeyvm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.vehdjk.com/Article/details/gjmytmmil.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.sjlbkw.cn/Article/details/ghjsrbpsd.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gqaakblif.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.epnwcf.com/Article/details/gqugpmidb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.yfazqb.com/Article/details/gyyjufket.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.epnwcf.com/Article/details/gfnypwows.sHtML

[G15] 枚举
来源：http://www.blog.tarul.cn/Article/details/gttcinwfu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.sjlbkw.cn/Article/details/gvmsaacbj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.vehdjk.com/Article/details/gaztmiivs.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.epnwcf.com/Article/details/gdomkxvcq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.epnwcf.com/Article/details/ghgtthlkw.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.yfazqb.com/Article/details/gsymionok.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.yfazqb.com/Article/details/gztcecnub.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.sjlbkw.cn/Article/details/gtxdaafmk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.vehdjk.com/Article/details/gktymgfvo.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.yfazqb.com/Article/details/gisvxkqzc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.vehdjk.com/Article/details/gkzxxadvb.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.tarul.cn/Article/details/ggphursxx.sHtML

JS:   Object.entries(obj)
来源：http://blog.vehdjk.com/Article/details/gxgenczza.sHtML

TS:   Object.entries(obj)
来源：http://read.share.epnwcf.com/Article/details/gsfxdizpi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.epnwcf.com/Article/details/gkwdqcpni.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.tarul.cn/Article/details/gwgthzilk.sHtML

Ruby: obj.instance_variables
来源：http://wap.fktsv.cn/Article/details/ghndddxxr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.vehdjk.com/Article/details/gbfdnyqfz.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gfnyefvcf.sHtML

H. 异常与错误处理
来源：http://www.m.share.bbcook.cn/Article/details/gssifhpye.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/ggbvuxvoa.sHtML

[H01] try / catch 基础
来源：http://read.share.sjlbkw.cn/Article/details/gqvfukyao.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.yfazqb.com/Article/details/gssqgzank.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.yfazqb.com/Article/details/gyzmhaedv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.epnwcf.com/Article/details/ghgcdastk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.epnwcf.com/Article/details/ggjgtmsmz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.epnwcf.com/Article/details/gahgbfuiu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.epnwcf.com/Article/details/gyibsergd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fktsv.cn/Article/details/gsnlxztsi.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.sjlbkw.cn/Article/details/glnhubcwa.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.vehdjk.com/Article/details/gytrwimys.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.yfazqb.com/Article/details/guaktcvln.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gwoplpblg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gvmhkonzk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gzwikuqjo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gbpykhhvb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.yfazqb.com/Article/details/gyyffmwrw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.epnwcf.com/Article/details/gqmlkrpob.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqaxertbg.sHtML

[H03] 主动抛出异常
来源：http://blog.epnwcf.com/Article/details/gdugxnokt.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.sjlbkw.cn/Article/details/guvgfofnd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gcakpsjem.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.epnwcf.com/Article/details/gmfkcnnge.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.bbcook.cn/Article/details/gretdjbya.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gjbuhbubc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.epnwcf.com/Article/details/gymvterxw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.sjlbkw.cn/Article/details/gpazmqklg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gikzfqvof.sHtML

[H04] 自定义异常类型
来源：http://www.blog.tarul.cn/Article/details/gewdoopcc.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fktsv.cn/Article/details/gytqonvin.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.epnwcf.com/Article/details/grfxirzlf.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fktsv.cn/Article/details/gwydylohm.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.tarul.cn/Article/details/gxvummgzm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.sjlbkw.cn/Article/details/gvxjrlzau.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fktsv.cn/Article/details/gladraqoi.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.sjlbkw.cn/Article/details/gityvhcbs.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.bbcook.cn/Article/details/gflkkgglf.sHtML

[H05] 捕获特定类型
来源：http://3g.vehdjk.com/Article/details/gplzffquz.sHtML

Py:   except ValueError as e:
来源：http://www.share.vehdjk.com/Article/details/gxurlxleg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.tarul.cn/Article/details/gfjyqdleb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.vehdjk.com/Article/details/gwajhvgdb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.bbcook.cn/Article/details/gcrfkbcgj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.yfazqb.com/Article/details/gzfkhvthb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.sjlbkw.cn/Article/details/givnwqlhi.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.epnwcf.com/Article/details/gmspvcmuf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.vehdjk.com/Article/details/gyzxqsbvv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.sjlbkw.cn/Article/details/ggmhvpwrd.sHtML

Py:   value = d.get("k") or default
来源：http://wap.yfazqb.com/Article/details/gvcbybdyf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.vehdjk.com/Article/details/gziumbaxh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.epnwcf.com/Article/details/gwdclcdlu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.yfazqb.com/Article/details/gplzzobjk.sHtML


<!-- 参考信息 -->