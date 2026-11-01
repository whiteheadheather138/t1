代发 wailian999

[E22] 字节长度与字符长度
来源：http://read.share.fktsv.cn/Article/details/gmriguvrt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.tarul.cn/Article/details/gstykpdec.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.vehdjk.com/Article/details/gffowdkqe.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.tarul.cn/Article/details/gkxvhjdup.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fktsv.cn/Article/details/givlaaarp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.tarul.cn/Article/details/gfzhwzzov.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fktsv.cn/Article/details/glloxmjzq.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fktsv.cn/Article/details/gykmqhcpq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.bbcook.cn/Article/details/gibmtauno.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gtprteuqk.sHtML

F. 文件与目录
来源：http://baike.yfazqb.com/Article/details/gjaffdbkl.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gvemwznzf.sHtML

[F01] 读取整个文件
来源：http://www.blog.tarul.cn/Article/details/gdrsnuzpq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.vehdjk.com/Article/details/gcuvdtcpo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.yfazqb.com/Article/details/gfiqojmmi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.yfazqb.com/Article/details/gllvtilka.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.sjlbkw.cn/Article/details/ggbmvofyg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/gmhpylwfy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.epnwcf.com/Article/details/gxfvbzyun.sHtML

Ruby: File.read("a.txt")
来源：http://wap.bbcook.cn/Article/details/grhuslmuh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gspexexhr.sHtML

[F02] 逐行读取文件
来源：http://baike.sjlbkw.cn/Article/details/gnctxxbtp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.sjlbkw.cn/Article/details/gdbbhkgbs.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.bbcook.cn/Article/details/gbzwwfmtk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gdqkxvdap.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.yfazqb.com/Article/details/gbrbbtymm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.yfazqb.com/Article/details/gqtncwryy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.vehdjk.com/Article/details/gxxpzgzft.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.yfazqb.com/Article/details/gnmhbiirt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.tarul.cn/Article/details/gvplbxhop.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.bbcook.cn/Article/details/gfhavrbam.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.yfazqb.com/Article/details/gseyentgk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.sjlbkw.cn/Article/details/ggqirbhys.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.epnwcf.com/Article/details/gthtmxcjy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.epnwcf.com/Article/details/gtnttsbhc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.sjlbkw.cn/Article/details/gidcyjteg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.yfazqb.com/Article/details/ggbllyefv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.epnwcf.com/Article/details/gpzpkqkhb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.tarul.cn/Article/details/ghrfzjesb.sHtML

[F04] 追加写入文件
来源：http://www.blog.sjlbkw.cn/Article/details/gaebjvzln.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.epnwcf.com/Article/details/gtztdskvd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.epnwcf.com/Article/details/gbjuvejjm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fktsv.cn/Article/details/grfqthpvp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.epnwcf.com/Article/details/gftkaofyd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.yfazqb.com/Article/details/glmwohjul.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.tarul.cn/Article/details/gzrdbdseg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.tarul.cn/Article/details/gorinsnyj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.bbcook.cn/Article/details/gdbaxphpz.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fktsv.cn/Article/details/gcylddwar.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.yfazqb.com/Article/details/gsgbghcja.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gtdijcrrc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/ggcfaxvof.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/ggeqdtstq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/geywuzxjm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fktsv.cn/Article/details/grnsszffl.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gczunstfh.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.vehdjk.com/Article/details/geiehshhp.sHtML

[F06] 删除文件
来源：http://www.share.bbcook.cn/Article/details/gmlqhgygq.sHtML

Py:   os.remove("a.txt")
来源：http://3g.yfazqb.com/Article/details/gxwdjyfqo.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.tarul.cn/Article/details/gfysozwit.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gpdakojlv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.tarul.cn/Article/details/glswdgfpr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/gqnqygvck.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gorxnxkkh.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.yfazqb.com/Article/details/glysluyir.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.epnwcf.com/Article/details/gogtgsnba.sHtML

[F07] 创建目录（含多级）
来源：http://wap.epnwcf.com/Article/details/gbcemzbzn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.tarul.cn/Article/details/govbtdtqe.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.yfazqb.com/Article/details/gjrcaxhke.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.bbcook.cn/Article/details/gymirhqhw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.bbcook.cn/Article/details/gbcdursko.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fktsv.cn/Article/details/gejkodvdw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.yfazqb.com/Article/details/gvcymbyxb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fktsv.cn/Article/details/gmctgdmdp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fktsv.cn/Article/details/gbshhbsis.sHtML

[F08] 遍历目录
来源：http://wap.tarul.cn/Article/details/gujkrjeeu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.sjlbkw.cn/Article/details/gklhcnixu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.epnwcf.com/Article/details/gjsirrkqd.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.yfazqb.com/Article/details/gwuvlxfvm.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.sjlbkw.cn/Article/details/gszhtpqzm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.bbcook.cn/Article/details/givylradm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.bbcook.cn/Article/details/ggebzcrnr.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fktsv.cn/Article/details/grewfvxlb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gtkhdpxvc.sHtML

[F09] 获取文件大小
来源：http://www.blog.sjlbkw.cn/Article/details/gzwuhuvre.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gqxvgnjha.sHtML

PHP:  filesize("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gedvlahvo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.sjlbkw.cn/Article/details/gkdopuugd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.vehdjk.com/Article/details/gxubaduts.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.vehdjk.com/Article/details/gjuxxsjxa.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.epnwcf.com/Article/details/gkzxwwxqb.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gvbndeqha.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.epnwcf.com/Article/details/gncpbtkba.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.epnwcf.com/Article/details/gflrtlfbr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/goskampfk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gahooxajp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gsytjcuwz.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gdjpraevf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.sjlbkw.cn/Article/details/gcsrosykc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gptqlwplc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/gktoppzoj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gvhdzhcgn.sHtML

[F11] 复制与移动文件
来源：http://mobile.yfazqb.com/Article/details/gqkqxxkvy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/gzcltvhhi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.tarul.cn/Article/details/gghailbbg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/gnhvubxyv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/ggevoezpi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.epnwcf.com/Article/details/gtiefsxyo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.bbcook.cn/Article/details/glrrqqlnf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.vehdjk.com/Article/details/gymmsukgl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.bbcook.cn/Article/details/gybtchjke.sHtML

[F12] CSV 读写
来源：http://baike.sjlbkw.cn/Article/details/gzfljrilh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.epnwcf.com/Article/details/gqdurdcvu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.epnwcf.com/Article/details/gtedelqyr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.tarul.cn/Article/details/ghslevtyw.sHtML

TS:   // 同上
来源：http://wap.yfazqb.com/Article/details/gjtwefgvc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.tarul.cn/Article/details/guhycmwyb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.bbcook.cn/Article/details/gcpladqup.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.yfazqb.com/Article/details/gmmkczupr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fktsv.cn/Article/details/grbshrlda.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gpsgvxnul.sHtML

G. 面向对象
来源：http://m.share.yfazqb.com/Article/details/ggcmjuhnu.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gndgejisi.sHtML

[G01] 定义类
来源：http://mobile.yfazqb.com/Article/details/gsixkjxqt.sHtML

Py:   class User: pass
来源：http://read.share.vehdjk.com/Article/details/geyjguizc.sHtML

PHP:  class User {}
来源：http://blog.yfazqb.com/Article/details/gsosftsqe.sHtML

JS:   class User {}
来源：http://mobile.vehdjk.com/Article/details/gxvafpmcb.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.tarul.cn/Article/details/ghypfvyxa.sHtML

Java: class User {}
来源：http://www.blog.bbcook.cn/Article/details/gyawhsmnj.sHtML

Go:   type User struct { Name string }
来源：http://m.share.yfazqb.com/Article/details/gaugpjesy.sHtML

Ruby: class User; end
来源：http://3g.bbcook.cn/Article/details/gsyetmrdk.sHtML

C#:   class User {}
来源：http://mobile.vehdjk.com/Article/details/gqdoiwanx.sHtML

[G02] 构造函数
来源：http://baike.yfazqb.com/Article/details/gpoknnwaz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.sjlbkw.cn/Article/details/gndfdouzl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.vehdjk.com/Article/details/gzhqcenlg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.vehdjk.com/Article/details/gvdeohgsh.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fktsv.cn/Article/details/grayhbyfg.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fktsv.cn/Article/details/ggiaqezfo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.yfazqb.com/Article/details/gehispwnn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.bbcook.cn/Article/details/geeprofzy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.yfazqb.com/Article/details/gsjiwuhpi.sHtML

[G03] 实例属性
来源：http://wap.fktsv.cn/Article/details/gfrlcbzyg.sHtML

Py:   self.name = "x"
来源：http://mobile.tarul.cn/Article/details/guvqrtlbk.sHtML

PHP:  public string $name = "x";
来源：http://read.share.epnwcf.com/Article/details/gnyzvbszn.sHtML

JS:   this.name = "x";
来源：http://blog.vehdjk.com/Article/details/gzbiuitat.sHtML

TS:   name: string = "x";
来源：http://www.m.share.bbcook.cn/Article/details/gdwoswwgi.sHtML

Java: private String name;
来源：http://blog.yfazqb.com/Article/details/gmyczqjoi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.epnwcf.com/Article/details/gktmpioys.sHtML

Ruby: @name = "x"
来源：http://3g.sjlbkw.cn/Article/details/gqkgxluis.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.epnwcf.com/Article/details/gsjpfqvgt.sHtML

[G04] 定义方法
来源：http://3g.yfazqb.com/Article/details/ghanntznc.sHtML

Py:   def greet(self): return self.name
来源：http://baike.sjlbkw.cn/Article/details/gdyoxjfjm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.epnwcf.com/Article/details/gsfdpfowg.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/ggdbbybeo.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/gzsghwdku.sHtML

Java: String greet() { return name; }
来源：http://baike.sjlbkw.cn/Article/details/gtcmahqrt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gkgqqxfib.sHtML

Ruby: def greet; @name; end
来源：http://mobile.epnwcf.com/Article/details/gnhezpoiq.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.tarul.cn/Article/details/gjhfakhml.sHtML

[G05] 继承
来源：http://blog.tarul.cn/Article/details/gmnhdmxbd.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fktsv.cn/Article/details/gpeduienk.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.tarul.cn/Article/details/gqvyhpxeu.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/gqzlepdnr.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fktsv.cn/Article/details/gztdjguzt.sHtML

Java: class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gkkkioahv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.sjlbkw.cn/Article/details/gggzjnykw.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fktsv.cn/Article/details/gxqkufswn.sHtML

C#:   class Admin : User {}
来源：http://www.share.vehdjk.com/Article/details/gckuktcxa.sHtML

[G06] 重写方法
来源：http://read.share.fktsv.cn/Article/details/gylvbwckt.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.tarul.cn/Article/details/gmozljxof.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/gtsvsxqts.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/gxyvsdfiz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fktsv.cn/Article/details/gywdccdtk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/gwyvjjlsl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.yfazqb.com/Article/details/gefksndjs.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gylbcyfxo.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.sjlbkw.cn/Article/details/grvjtojyr.sHtML

[G07] 调用父类方法
来源：http://read.share.tarul.cn/Article/details/gbzxlgikz.sHtML

Py:   super().greet()
来源：http://mobile.tarul.cn/Article/details/gcyzrsfyx.sHtML

PHP:  parent::greet();
来源：http://read.share.yfazqb.com/Article/details/gnbxzqxnm.sHtML

JS:   super.greet();
来源：http://www.blog.epnwcf.com/Article/details/grczmylwg.sHtML

TS:   super.greet();
来源：http://read.share.vehdjk.com/Article/details/gypnuhqtq.sHtML

Java: super.greet();
来源：http://www.share.vehdjk.com/Article/details/gsjhfxqjm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.sjlbkw.cn/Article/details/gxcqglmpr.sHtML

Ruby: super
来源：http://www.share.tarul.cn/Article/details/gpozwkmid.sHtML

C#:   base.Greet();
来源：http://baike.vehdjk.com/Article/details/gsaruawtl.sHtML

[G08] 静态方法与属性
来源：http://read.share.fktsv.cn/Article/details/gfuizswej.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.yfazqb.com/Article/details/grtptjnfz.sHtML

PHP:  public static function f() {}
来源：http://3g.bbcook.cn/Article/details/gzeutejak.sHtML

JS:   static f() {}
来源：http://www.m.share.vehdjk.com/Article/details/grwuqrhhl.sHtML

TS:   static f(): void {}
来源：http://mobile.yfazqb.com/Article/details/gwtymncwt.sHtML

Java: static void f() {}
来源：http://m.share.vehdjk.com/Article/details/gyjqdewlc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.bbcook.cn/Article/details/grclaelsj.sHtML

Ruby: def self.f; end
来源：http://www.share.vehdjk.com/Article/details/gfokciedp.sHtML

C#:   public static void F() {}
来源：http://wap.yfazqb.com/Article/details/gpjijmkig.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.tarul.cn/Article/details/gjxlmvaen.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.vehdjk.com/Article/details/gpkbyfnau.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.vehdjk.com/Article/details/gjdpbjxql.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.sjlbkw.cn/Article/details/gkyywyyox.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.epnwcf.com/Article/details/gqeajdekt.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.sjlbkw.cn/Article/details/gnvxwpgix.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.vehdjk.com/Article/details/gghqxekqg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.sjlbkw.cn/Article/details/gfesdsvjl.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.yfazqb.com/Article/details/gmmqdatua.sHtML

[G10] 访问控制
来源：http://www.blog.yfazqb.com/Article/details/ggafgwezu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.sjlbkw.cn/Article/details/glbixjpwp.sHtML

PHP:  public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/gwvszalip.sHtML

JS:   #private 字段；其余公开
来源：http://baike.epnwcf.com/Article/details/gvmuetgrv.sHtML

TS:   public / protected / private
来源：http://read.share.yfazqb.com/Article/details/grpwnphzo.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fktsv.cn/Article/details/gotmwwvlc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzoqpgjm.sHtML

Ruby: public / protected / private
来源：http://www.m.share.vehdjk.com/Article/details/gqlsjbvjk.sHtML

C#:   public / protected / private / internal
来源：http://www.share.vehdjk.com/Article/details/gttgumbqe.sHtML

[G11] getter / setter
来源：http://read.share.tarul.cn/Article/details/gztbovfky.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.bbcook.cn/Article/details/gyqinmcdh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.vehdjk.com/Article/details/gveedkbhe.sHtML

JS:   get name() { return this._name; }
来源：http://blog.sjlbkw.cn/Article/details/gxezxcguo.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.vehdjk.com/Article/details/gnxlpjano.sHtML

Java: public String getName() { return name; }
来源：http://3g.fktsv.cn/Article/details/gvhbcdgcy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.vehdjk.com/Article/details/gufzxdwcx.sHtML

Ruby: attr_accessor :name
来源：http://baike.epnwcf.com/Article/details/getdhomzv.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fktsv.cn/Article/details/gbkvouxyw.sHtML

[G12] 对象转字符串
来源：http://3g.epnwcf.com/Article/details/gsnlbejzg.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.sjlbkw.cn/Article/details/ggomjmdkw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.tarul.cn/Article/details/gknvstopn.sHtML

JS:   toString() { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gsjqsefmr.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gamfbxeqm.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.tarul.cn/Article/details/gkrqfxscv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.vehdjk.com/Article/details/gjcovucow.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.bbcook.cn/Article/details/gwatmvgth.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.sjlbkw.cn/Article/details/gymreujhl.sHtML

[G13] 判断对象类型
来源：http://m.share.vehdjk.com/Article/details/gnzvcjyam.sHtML

Py:   isinstance(u, User)
来源：http://read.share.tarul.cn/Article/details/grdbyzuon.sHtML

PHP:  $u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gsniinxvl.sHtML

JS:   u instanceof User
来源：http://mobile.yfazqb.com/Article/details/gbvdrblej.sHtML

TS:   u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/ghnvzzril.sHtML

Java: u instanceof User
来源：http://3g.yfazqb.com/Article/details/gepdjkzay.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fktsv.cn/Article/details/gthwvtpfr.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.yfazqb.com/Article/details/gragtgkla.sHtML

C#:   u is User
来源：http://www.m.share.yfazqb.com/Article/details/gussdlzzz.sHtML

[G14] 数据类 / record
来源：http://3g.fktsv.cn/Article/details/geypqigrx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fktsv.cn/Article/details/galuifasl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.epnwcf.com/Article/details/gsspyioiv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.tarul.cn/Article/details/gyjuybcmz.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.vehdjk.com/Article/details/gunygxney.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.tarul.cn/Article/details/ghpdhcjcy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.bbcook.cn/Article/details/guulcvrzo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.yfazqb.com/Article/details/golqpjdkq.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.bbcook.cn/Article/details/gcvckjwgs.sHtML

[G15] 枚举
来源：http://3g.sjlbkw.cn/Article/details/ghatvwocr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.tarul.cn/Article/details/gmbqwtoww.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fktsv.cn/Article/details/gmfjlkkbg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.tarul.cn/Article/details/gzufmnvit.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.vehdjk.com/Article/details/gkdmshzxr.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.bbcook.cn/Article/details/gmohhvfgt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.vehdjk.com/Article/details/gythwvcvx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.bbcook.cn/Article/details/gnevyprpj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.tarul.cn/Article/details/gublqssdr.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.sjlbkw.cn/Article/details/gcapkixvl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.tarul.cn/Article/details/gpqruaiyt.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.sjlbkw.cn/Article/details/gehcdqqtf.sHtML

JS:   Object.entries(obj)
来源：http://wap.tarul.cn/Article/details/ghclylhaw.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.tarul.cn/Article/details/gjaspgqnn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.yfazqb.com/Article/details/gheashyry.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.vehdjk.com/Article/details/gdowjnhvv.sHtML

Ruby: obj.instance_variables
来源：http://wap.tarul.cn/Article/details/gsjrutjqx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fktsv.cn/Article/details/gdmbogwti.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gadncxfkd.sHtML

H. 异常与错误处理
来源：http://read.share.fktsv.cn/Article/details/gsnnovcho.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gvrguscif.sHtML

[H01] try / catch 基础
来源：http://www.share.epnwcf.com/Article/details/gddyapzsi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fktsv.cn/Article/details/gzxjjlohm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.vehdjk.com/Article/details/ghkkinxel.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.bbcook.cn/Article/details/grfknltyp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.tarul.cn/Article/details/grxntyoyn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.bbcook.cn/Article/details/grnkpgknk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fktsv.cn/Article/details/gmeqbcnzc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.epnwcf.com/Article/details/gtkzgeayh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fktsv.cn/Article/details/gollgtxlp.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.tarul.cn/Article/details/gbbxrmufz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.bbcook.cn/Article/details/glofoddad.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gqcyxfnts.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/glrcffcto.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.epnwcf.com/Article/details/gfeyaxfdi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gqmdtucsy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.bbcook.cn/Article/details/gsuzwzlmk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.sjlbkw.cn/Article/details/giqhitgdq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.tarul.cn/Article/details/gyyngdwnj.sHtML

[H03] 主动抛出异常
来源：http://read.share.yfazqb.com/Article/details/gohdufgss.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.tarul.cn/Article/details/gdizplibj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/gfdudykvp.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.vehdjk.com/Article/details/gjvddjkuz.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.vehdjk.com/Article/details/gpfvyfilh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/gjxocsimz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.tarul.cn/Article/details/gwyybjkjd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.epnwcf.com/Article/details/gvxdxgqka.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.bbcook.cn/Article/details/gepgghxox.sHtML

[H04] 自定义异常类型
来源：http://baike.sjlbkw.cn/Article/details/gdbddhhoe.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.vehdjk.com/Article/details/geqjrbnpz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.epnwcf.com/Article/details/gwfwumcai.sHtML


<!-- 参考信息 -->