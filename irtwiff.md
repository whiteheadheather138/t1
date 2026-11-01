代发 wailian999

[E22] 字节长度与字符长度
来源：http://www.share.tarul.cn/Article/details/gowvvdfwm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.vehdjk.com/Article/details/gelcnqwzl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.tarul.cn/Article/details/gxqlyzioe.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.sjlbkw.cn/Article/details/garglbwiq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.sjlbkw.cn/Article/details/ghhnjcawc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.epnwcf.com/Article/details/gqvrhbwax.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.bbcook.cn/Article/details/gweuxkkya.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.vehdjk.com/Article/details/gorkruyjx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.sjlbkw.cn/Article/details/gaqnqrsdi.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gvyqpyhxl.sHtML

F. 文件与目录
来源：http://www.m.share.vehdjk.com/Article/details/gbmibftxv.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gelwfzgun.sHtML

[F01] 读取整个文件
来源：http://www.blog.vehdjk.com/Article/details/gqszpzckv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.vehdjk.com/Article/details/gfvflysjj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/ggadbzwax.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.yfazqb.com/Article/details/gtzxrwcxy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.bbcook.cn/Article/details/gtuwxjjda.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gzubpbcim.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.bbcook.cn/Article/details/gcwryaipg.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvunbwpct.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.tarul.cn/Article/details/gcgdbrowo.sHtML

[F02] 逐行读取文件
来源：http://mobile.fktsv.cn/Article/details/gzelbdbli.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fktsv.cn/Article/details/gdmjuhsbo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.epnwcf.com/Article/details/gajcxgpqd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fktsv.cn/Article/details/gheloveha.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fktsv.cn/Article/details/ghhfpaimv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fktsv.cn/Article/details/gwfynzxww.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.sjlbkw.cn/Article/details/gfxmxkelj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsxnnqrgc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.sjlbkw.cn/Article/details/gfbxqqmuj.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fktsv.cn/Article/details/gdfyhlgov.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.yfazqb.com/Article/details/gzpmztqqk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.sjlbkw.cn/Article/details/gdjrdnfnf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.bbcook.cn/Article/details/gbrroxvnr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fktsv.cn/Article/details/gmquajnji.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fktsv.cn/Article/details/gxkmaujeu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.sjlbkw.cn/Article/details/gecubsgst.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fktsv.cn/Article/details/gkbeaduoe.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.vehdjk.com/Article/details/gciszvtgh.sHtML

[F04] 追加写入文件
来源：http://wap.tarul.cn/Article/details/gjaqupgti.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.epnwcf.com/Article/details/gnucawnex.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fktsv.cn/Article/details/ghiakqwan.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.epnwcf.com/Article/details/gnkvtxrpi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.bbcook.cn/Article/details/genjhrrrx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.bbcook.cn/Article/details/glakenmjx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.vehdjk.com/Article/details/gubvzzdkm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.epnwcf.com/Article/details/gidmcxuxm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.sjlbkw.cn/Article/details/gywjtoxwg.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.yfazqb.com/Article/details/gvqtnstio.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.vehdjk.com/Article/details/giuazfeha.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gurtmlhoj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gwrhaydlq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gaxrdbtge.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/ggugaiydh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.vehdjk.com/Article/details/grlfkyszj.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.yfazqb.com/Article/details/gjhysxtsh.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.vehdjk.com/Article/details/gauvetcug.sHtML

[F06] 删除文件
来源：http://www.blog.tarul.cn/Article/details/gksewbyml.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gltrejdsi.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.tarul.cn/Article/details/gjkragnxw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/ghpgxqdvl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/grdjposez.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/griaeebvg.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.yfazqb.com/Article/details/grnfainqi.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gtlualmcj.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gzxrewvrw.sHtML

[F07] 创建目录（含多级）
来源：http://wap.tarul.cn/Article/details/gytdmtwro.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fktsv.cn/Article/details/gnwqfsnxw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.sjlbkw.cn/Article/details/gkqawspaf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.tarul.cn/Article/details/gaafdopvh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.yfazqb.com/Article/details/gddsynryb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.yfazqb.com/Article/details/gmyefamul.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.sjlbkw.cn/Article/details/gwfzatfzr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.sjlbkw.cn/Article/details/gqrvnzhqe.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fktsv.cn/Article/details/gzumtlicq.sHtML

[F08] 遍历目录
来源：http://blog.bbcook.cn/Article/details/gcnpgwlmf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.bbcook.cn/Article/details/gpdehlzmt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.epnwcf.com/Article/details/gxqtspzro.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.epnwcf.com/Article/details/gmhzxbnin.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.sjlbkw.cn/Article/details/gkpcrumnu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.vehdjk.com/Article/details/gvmtzjwtr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.vehdjk.com/Article/details/gdwglhepj.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.bbcook.cn/Article/details/gerbxkxoz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.tarul.cn/Article/details/gljfhfzlu.sHtML

[F09] 获取文件大小
来源：http://3g.fktsv.cn/Article/details/gyhtqztlf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.epnwcf.com/Article/details/gsygdebgp.sHtML

PHP:  filesize("a.txt");
来源：http://baike.yfazqb.com/Article/details/gdipumpxg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.vehdjk.com/Article/details/gpzirncae.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.epnwcf.com/Article/details/gfutjdtat.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/girpnzhoz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.vehdjk.com/Article/details/gthcpjwfg.sHtML

Ruby: File.size("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gnwlnejeu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.epnwcf.com/Article/details/gbjxcqgat.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fktsv.cn/Article/details/gvkniciid.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gzrfqrqvl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gtimioczl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.tarul.cn/Article/details/gcqaqybth.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gqowvsaff.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.vehdjk.com/Article/details/gwjknsamt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gvznxxdbd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/grcrcpicj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/grsirkdqh.sHtML

[F11] 复制与移动文件
来源：http://m.share.tarul.cn/Article/details/gowaaiqjo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gjbwcbtss.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.epnwcf.com/Article/details/gpfhqnenz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gywskwnqj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.vehdjk.com/Article/details/grsvjhggj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.bbcook.cn/Article/details/gyghozrun.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.yfazqb.com/Article/details/gqalqkxru.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.vehdjk.com/Article/details/gshncrrzg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.bbcook.cn/Article/details/gkxhjnbzb.sHtML

[F12] CSV 读写
来源：http://m.share.vehdjk.com/Article/details/gdussdivs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.bbcook.cn/Article/details/gvgvheoas.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.epnwcf.com/Article/details/gdmezaceh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.bbcook.cn/Article/details/gxceliydp.sHtML

TS:   // 同上
来源：http://baike.bbcook.cn/Article/details/gsckicrck.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.tarul.cn/Article/details/gjdrpoatz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.epnwcf.com/Article/details/gnnmfqvpt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.yfazqb.com/Article/details/gigbjycul.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.vehdjk.com/Article/details/gckjgxvvx.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/ghzgdtzlb.sHtML

G. 面向对象
来源：http://www.m.share.vehdjk.com/Article/details/gnvuesgun.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gwrhdjbci.sHtML

[G01] 定义类
来源：http://wap.bbcook.cn/Article/details/goqkejvlq.sHtML

Py:   class User: pass
来源：http://read.share.yfazqb.com/Article/details/gntucqiwq.sHtML

PHP:  class User {}
来源：http://m.share.yfazqb.com/Article/details/gykpozyrm.sHtML

JS:   class User {}
来源：http://3g.vehdjk.com/Article/details/gebvjlaqn.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.vehdjk.com/Article/details/gxxxwrhyi.sHtML

Java: class User {}
来源：http://3g.sjlbkw.cn/Article/details/guydxwgvl.sHtML

Go:   type User struct { Name string }
来源：http://baike.epnwcf.com/Article/details/gzjrprgcp.sHtML

Ruby: class User; end
来源：http://read.share.tarul.cn/Article/details/grrwsuhaj.sHtML

C#:   class User {}
来源：http://mobile.epnwcf.com/Article/details/gsirdahgd.sHtML

[G02] 构造函数
来源：http://wap.sjlbkw.cn/Article/details/gqwjpbnov.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.sjlbkw.cn/Article/details/gezeocexj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.epnwcf.com/Article/details/gsagiylbb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.yfazqb.com/Article/details/gzsfphdpb.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.yfazqb.com/Article/details/gwbublxuy.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.tarul.cn/Article/details/giwenknpg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.vehdjk.com/Article/details/givyoaqzo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.yfazqb.com/Article/details/gkrlzixno.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.vehdjk.com/Article/details/ggyexlchv.sHtML

[G03] 实例属性
来源：http://3g.fktsv.cn/Article/details/gbrpozsso.sHtML

Py:   self.name = "x"
来源：http://mobile.tarul.cn/Article/details/gujqyjooo.sHtML

PHP:  public string $name = "x";
来源：http://read.share.tarul.cn/Article/details/gbsrqavba.sHtML

JS:   this.name = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gfyncuvje.sHtML

TS:   name: string = "x";
来源：http://mobile.epnwcf.com/Article/details/gdyzdnblw.sHtML

Java: private String name;
来源：http://blog.sjlbkw.cn/Article/details/gscmueknm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.yfazqb.com/Article/details/gzmnwprav.sHtML

Ruby: @name = "x"
来源：http://www.m.share.vehdjk.com/Article/details/gbwdpdsib.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.bbcook.cn/Article/details/gkrtvrzia.sHtML

[G04] 定义方法
来源：http://www.blog.sjlbkw.cn/Article/details/godavhsrm.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.sjlbkw.cn/Article/details/gzeuyyslp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.yfazqb.com/Article/details/gsmvvpwfa.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.bbcook.cn/Article/details/ggscbvzuv.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/gbuyhnjkn.sHtML

Java: String greet() { return name; }
来源：http://m.share.fktsv.cn/Article/details/gunwdkazs.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.bbcook.cn/Article/details/gbkrzmkem.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fktsv.cn/Article/details/ghbygwrrh.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.vehdjk.com/Article/details/gukulqrlq.sHtML

[G05] 继承
来源：http://wap.sjlbkw.cn/Article/details/gxisitszy.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.vehdjk.com/Article/details/grnobnspq.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gpeqtaevk.sHtML

JS:   class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/gvtpswxxl.sHtML

TS:   class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/gdooiqnjy.sHtML

Java: class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gtvpevuyr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.sjlbkw.cn/Article/details/gcrqlllty.sHtML

Ruby: class Admin < User; end
来源：http://baike.epnwcf.com/Article/details/gyagrqyzi.sHtML

C#:   class Admin : User {}
来源：http://www.blog.vehdjk.com/Article/details/gwlfuoxpo.sHtML

[G06] 重写方法
来源：http://3g.vehdjk.com/Article/details/gylvmodvh.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.bbcook.cn/Article/details/gwntqqtjo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.tarul.cn/Article/details/golecwxqp.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gcmcrcvwv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/guwxcjiug.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/gvmcyvojj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.vehdjk.com/Article/details/gpcoeshvh.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.sjlbkw.cn/Article/details/guwnjtfcs.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.tarul.cn/Article/details/gilaqokxm.sHtML

[G07] 调用父类方法
来源：http://m.share.vehdjk.com/Article/details/gdvagzijb.sHtML

Py:   super().greet()
来源：http://www.share.tarul.cn/Article/details/githpfrmh.sHtML

PHP:  parent::greet();
来源：http://www.share.fktsv.cn/Article/details/gzsvvcloc.sHtML

JS:   super.greet();
来源：http://blog.epnwcf.com/Article/details/gvjzyidni.sHtML

TS:   super.greet();
来源：http://www.m.share.yfazqb.com/Article/details/gedqzdljg.sHtML

Java: super.greet();
来源：http://www.share.epnwcf.com/Article/details/ggdicdxds.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.bbcook.cn/Article/details/gqekuxmzk.sHtML

Ruby: super
来源：http://www.m.share.sjlbkw.cn/Article/details/goqjymkth.sHtML

C#:   base.Greet();
来源：http://mobile.tarul.cn/Article/details/gjkouwmbx.sHtML

[G08] 静态方法与属性
来源：http://www.blog.tarul.cn/Article/details/gxkutaius.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.yfazqb.com/Article/details/gggqkjqrf.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fktsv.cn/Article/details/gnvcmbbqr.sHtML

JS:   static f() {}
来源：http://baike.epnwcf.com/Article/details/gfmjgywoj.sHtML

TS:   static f(): void {}
来源：http://m.share.tarul.cn/Article/details/gmofyhtiu.sHtML

Java: static void f() {}
来源：http://wap.fktsv.cn/Article/details/gielvzthw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.bbcook.cn/Article/details/glrazrdaz.sHtML

Ruby: def self.f; end
来源：http://read.share.bbcook.cn/Article/details/gzasqrfqv.sHtML

C#:   public static void F() {}
来源：http://read.share.yfazqb.com/Article/details/gsfjzfbcq.sHtML

[G09] 接口 / 抽象类
来源：http://3g.epnwcf.com/Article/details/ggtbnkqkz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fktsv.cn/Article/details/ggfbaqvrf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.bbcook.cn/Article/details/gjkroxedi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.bbcook.cn/Article/details/gvkvbkmmh.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.sjlbkw.cn/Article/details/gcwjrredc.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.epnwcf.com/Article/details/gnsnkwgst.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.epnwcf.com/Article/details/gkboyqszw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.epnwcf.com/Article/details/gashhiios.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.vehdjk.com/Article/details/gmqnvktdj.sHtML

[G10] 访问控制
来源：http://3g.vehdjk.com/Article/details/gclfksqax.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.epnwcf.com/Article/details/gurviprdy.sHtML

PHP:  public / protected / private
来源：http://wap.bbcook.cn/Article/details/gsiybbmny.sHtML

JS:   #private 字段；其余公开
来源：http://3g.epnwcf.com/Article/details/gvyzbmrar.sHtML

TS:   public / protected / private
来源：http://www.m.share.epnwcf.com/Article/details/gclitzyqr.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.tarul.cn/Article/details/giqnfqcmf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.tarul.cn/Article/details/gjqstygmj.sHtML

Ruby: public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/gyttanbjt.sHtML

C#:   public / protected / private / internal
来源：http://www.share.epnwcf.com/Article/details/gijbkkivp.sHtML

[G11] getter / setter
来源：http://read.share.bbcook.cn/Article/details/gibynwgxh.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.sjlbkw.cn/Article/details/giyseymkb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/gebxdctrj.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.sjlbkw.cn/Article/details/geopzehvp.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.tarul.cn/Article/details/gsyamhrdi.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gurbjghlx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.sjlbkw.cn/Article/details/gyflelyul.sHtML

Ruby: attr_accessor :name
来源：http://m.share.tarul.cn/Article/details/gcnbnsjky.sHtML

C#:   public string Name { get; set; }
来源：http://wap.sjlbkw.cn/Article/details/gcqdbxqht.sHtML

[G12] 对象转字符串
来源：http://baike.vehdjk.com/Article/details/gzpcdowhy.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.vehdjk.com/Article/details/gazdvofka.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.vehdjk.com/Article/details/gszegjruz.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/gnxbzwvfq.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/glzjtlzfp.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.vehdjk.com/Article/details/gslglyodn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.sjlbkw.cn/Article/details/gmwrancra.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.vehdjk.com/Article/details/gbrwmjkix.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.epnwcf.com/Article/details/grskpdwqy.sHtML

[G13] 判断对象类型
来源：http://m.share.tarul.cn/Article/details/gcrfoxowr.sHtML

Py:   isinstance(u, User)
来源：http://read.share.bbcook.cn/Article/details/gssszxayg.sHtML

PHP:  $u instanceof User
来源：http://3g.yfazqb.com/Article/details/gzdkcvckk.sHtML

JS:   u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/gnfajobyz.sHtML

TS:   u instanceof User
来源：http://blog.bbcook.cn/Article/details/gttttcabr.sHtML

Java: u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/goisvtzet.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fktsv.cn/Article/details/gfaammeaq.sHtML

Ruby: u.is_a?(User)
来源：http://blog.vehdjk.com/Article/details/ghdmepamt.sHtML

C#:   u is User
来源：http://read.share.sjlbkw.cn/Article/details/gcldfspme.sHtML

[G14] 数据类 / record
来源：http://3g.yfazqb.com/Article/details/gvefvudcq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.sjlbkw.cn/Article/details/gputhcmge.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.bbcook.cn/Article/details/ghnucpgbk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.epnwcf.com/Article/details/giclcccwf.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.tarul.cn/Article/details/gzxpcsdnd.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.vehdjk.com/Article/details/gerncofoc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.sjlbkw.cn/Article/details/gkzjpgahf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.epnwcf.com/Article/details/gguxeovbf.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.epnwcf.com/Article/details/gpmuawijh.sHtML

[G15] 枚举
来源：http://m.share.yfazqb.com/Article/details/gzalnyttf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.bbcook.cn/Article/details/guncriyyf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.sjlbkw.cn/Article/details/gghhcrqik.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.epnwcf.com/Article/details/gzedjqglh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.sjlbkw.cn/Article/details/glkuhecjq.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.bbcook.cn/Article/details/gyqqwirmu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fktsv.cn/Article/details/gzeauhojm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.epnwcf.com/Article/details/grfjznowz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.bbcook.cn/Article/details/gpdvczrud.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.vehdjk.com/Article/details/gaujahhcf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.tarul.cn/Article/details/ggmfokcnu.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.sjlbkw.cn/Article/details/gyvlfrckv.sHtML

JS:   Object.entries(obj)
来源：http://read.share.vehdjk.com/Article/details/gcaiokbwo.sHtML

TS:   Object.entries(obj)
来源：http://3g.vehdjk.com/Article/details/gxwutlomj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.tarul.cn/Article/details/ghbmtpery.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.bbcook.cn/Article/details/gvjwwhohf.sHtML

Ruby: obj.instance_variables
来源：http://blog.fktsv.cn/Article/details/gfbsmdata.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.yfazqb.com/Article/details/ghhrncfij.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/ghyjnpezq.sHtML

H. 异常与错误处理
来源：http://3g.tarul.cn/Article/details/gnicagjxp.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/grbbecmft.sHtML

[H01] try / catch 基础
来源：http://www.m.share.sjlbkw.cn/Article/details/gsoynrxzp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.tarul.cn/Article/details/glrspnzjw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.vehdjk.com/Article/details/gaxiqehnl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.bbcook.cn/Article/details/gychghekw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fktsv.cn/Article/details/gungnubwq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.vehdjk.com/Article/details/ghoekvqph.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.tarul.cn/Article/details/gdvfanvjm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.epnwcf.com/Article/details/gdmuhcuzx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.epnwcf.com/Article/details/gpzizmasj.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.bbcook.cn/Article/details/gmypdpqcn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fktsv.cn/Article/details/gtvdascyo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gnygszykx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/gzzmuejmf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/gczfwnzan.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/gqjuhjduz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.tarul.cn/Article/details/glvtorvnn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.vehdjk.com/Article/details/gduyofgdx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gfnkdejgt.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fktsv.cn/Article/details/ggvlsfcju.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.bbcook.cn/Article/details/gqafupcmh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.tarul.cn/Article/details/glhvbyjyp.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.epnwcf.com/Article/details/gfihdmijx.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.yfazqb.com/Article/details/gqtiwtjrl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.epnwcf.com/Article/details/goxoqfbkc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.bbcook.cn/Article/details/gibyuoofn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fktsv.cn/Article/details/gmesvafzo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.bbcook.cn/Article/details/gvccsgqvh.sHtML

[H04] 自定义异常类型
来源：http://blog.bbcook.cn/Article/details/gaugqdydd.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.epnwcf.com/Article/details/gqitthjoc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.sjlbkw.cn/Article/details/gztfihfcp.sHtML


<!-- 参考信息 -->