代发 wailian999

Go:   if s == "" {}
来源：http://read.share.fktsv.cn/Article/details/gwbtllxxz.sHtML

Ruby: if s.empty?
来源：http://3g.yfazqb.com/Article/details/gwpfumxdj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.sjlbkw.cn/Article/details/gkytvbjtq.sHtML

[E21] 超长截断加省略号
来源：http://mobile.bbcook.cn/Article/details/goqnjnlzx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fktsv.cn/Article/details/gpbhcrixe.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/gnntaqxjk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.bbcook.cn/Article/details/gmslpkqkw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gxjtptzny.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/gdldtyxhl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.bbcook.cn/Article/details/gnajqqkbt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/gqffeynbd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fktsv.cn/Article/details/gspxbmrhc.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gqhferzmj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.yfazqb.com/Article/details/gonnuctzl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/grczgboqe.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.bbcook.cn/Article/details/gedxjrhfd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.tarul.cn/Article/details/giyqaklut.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.tarul.cn/Article/details/ggyotswia.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.yfazqb.com/Article/details/gejjmpbkb.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fktsv.cn/Article/details/gpdfaepvr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.tarul.cn/Article/details/gounigpie.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gbumrocpp.sHtML

F. 文件与目录
来源：http://baike.fktsv.cn/Article/details/gjvnulkva.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gerftvnip.sHtML

[F01] 读取整个文件
来源：http://mobile.epnwcf.com/Article/details/gxmcgkien.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.tarul.cn/Article/details/gkvtpdnud.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gxbztjkqh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.tarul.cn/Article/details/gaqwazkog.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.yfazqb.com/Article/details/glbjdwbno.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gabnwtuug.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.vehdjk.com/Article/details/gbdymncek.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.tarul.cn/Article/details/gvhbzwvfi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gazlewxtj.sHtML

[F02] 逐行读取文件
来源：http://wap.bbcook.cn/Article/details/gevjbyvhj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.yfazqb.com/Article/details/gulzuoibq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.yfazqb.com/Article/details/grquxmqdl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.sjlbkw.cn/Article/details/gnldxbiyw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.epnwcf.com/Article/details/guwntewzo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.vehdjk.com/Article/details/gjvpsjcfv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.bbcook.cn/Article/details/gdcmyurpa.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.yfazqb.com/Article/details/guypzfgfh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.vehdjk.com/Article/details/gasckmxkf.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fktsv.cn/Article/details/gbshaxvfm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.vehdjk.com/Article/details/gpcqiyynw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.vehdjk.com/Article/details/gylgcznof.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.epnwcf.com/Article/details/gvqbaqjsw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.epnwcf.com/Article/details/gulcenhsx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.vehdjk.com/Article/details/gzeawjuns.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.sjlbkw.cn/Article/details/gsqwwlygd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.sjlbkw.cn/Article/details/gzgvgdrjl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqhnkppn.sHtML

[F04] 追加写入文件
来源：http://3g.tarul.cn/Article/details/gnxinmqor.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.vehdjk.com/Article/details/ggrqdpkvh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fktsv.cn/Article/details/gdmwbdvtx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.epnwcf.com/Article/details/gudycauzp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.tarul.cn/Article/details/gvbpzssbb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.tarul.cn/Article/details/gfniwrllw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fktsv.cn/Article/details/gxoporpdc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fktsv.cn/Article/details/gmwvvnqxh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.epnwcf.com/Article/details/gmwevbyze.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.vehdjk.com/Article/details/garokvaly.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.bbcook.cn/Article/details/gzryhyshl.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.yfazqb.com/Article/details/gftwinhbs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fktsv.cn/Article/details/gcwfceqht.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gwnajrebn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.vehdjk.com/Article/details/ghehyqyyz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.bbcook.cn/Article/details/gjfdqqffl.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.yfazqb.com/Article/details/goppjlfvn.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fktsv.cn/Article/details/ghzxkiqqc.sHtML

[F06] 删除文件
来源：http://www.m.share.fktsv.cn/Article/details/gxakchdgu.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gpscxvcdu.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gllldexno.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/guaydiigt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/goidzahak.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gtntdyadz.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.bbcook.cn/Article/details/gmhgfsapa.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.yfazqb.com/Article/details/gvzclekix.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gngphlmoo.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.yfazqb.com/Article/details/gbomfuzae.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fktsv.cn/Article/details/giulwchbz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.sjlbkw.cn/Article/details/gnbryvidv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.sjlbkw.cn/Article/details/gmycpkrnk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.vehdjk.com/Article/details/gfuqrbtmd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.vehdjk.com/Article/details/gdgzagmdp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.yfazqb.com/Article/details/gitsjtupd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fktsv.cn/Article/details/gzjviwqxe.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.epnwcf.com/Article/details/gegpydmjh.sHtML

[F08] 遍历目录
来源：http://read.share.epnwcf.com/Article/details/gtvgxduwe.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.vehdjk.com/Article/details/gsulxjngz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.sjlbkw.cn/Article/details/gwsuulgbq.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.epnwcf.com/Article/details/gcwdpxkpk.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.epnwcf.com/Article/details/ggvkmlnbs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.sjlbkw.cn/Article/details/guuezlxtu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gybuwxmpi.sHtML

Ruby: Dir.children("dir")
来源：http://baike.yfazqb.com/Article/details/gzrgpwqqx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.bbcook.cn/Article/details/gnenmikqk.sHtML

[F09] 获取文件大小
来源：http://read.share.vehdjk.com/Article/details/gvhuzygej.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/ggsdhozwm.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fktsv.cn/Article/details/gfjksachi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.yfazqb.com/Article/details/glbfbsbri.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.tarul.cn/Article/details/gxdpsxthb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.vehdjk.com/Article/details/gdcowwrzn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.vehdjk.com/Article/details/gaqfutoaj.sHtML

Ruby: File.size("a.txt")
来源：http://wap.tarul.cn/Article/details/gyftmgoax.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.epnwcf.com/Article/details/giphegajk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.yfazqb.com/Article/details/gxnzylbxe.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gasdhvhyo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gahdiahir.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gqlvtenup.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gemxucixz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.tarul.cn/Article/details/gmhtkjklk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gnoewhbsp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/grousujsr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/ggzlpcchf.sHtML

[F11] 复制与移动文件
来源：http://blog.fktsv.cn/Article/details/grvcgpebo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gssvfzdin.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.yfazqb.com/Article/details/gprvqlcfb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.tarul.cn/Article/details/gfklmgwgt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/glumeajyn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.vehdjk.com/Article/details/gdfprhjib.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.tarul.cn/Article/details/ghhsowysz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/gxfqqqqky.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.vehdjk.com/Article/details/gkqivxbhs.sHtML

[F12] CSV 读写
来源：http://blog.vehdjk.com/Article/details/gclkjqhxy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.yfazqb.com/Article/details/gucnqtnjq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.sjlbkw.cn/Article/details/gxrsqulji.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.epnwcf.com/Article/details/ghjpoonoo.sHtML

TS:   // 同上
来源：http://wap.vehdjk.com/Article/details/gwwahqyea.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.vehdjk.com/Article/details/gbrczfdwa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.yfazqb.com/Article/details/gjblfhvpt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.yfazqb.com/Article/details/gvdogzfvh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.sjlbkw.cn/Article/details/gamrvqdwm.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/ghucnwhxp.sHtML

G. 面向对象
来源：http://wap.epnwcf.com/Article/details/gfqgyojxq.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gakvduosl.sHtML

[G01] 定义类
来源：http://www.share.tarul.cn/Article/details/ghwnyxxzp.sHtML

Py:   class User: pass
来源：http://m.share.fktsv.cn/Article/details/gnwukecwb.sHtML

PHP:  class User {}
来源：http://baike.bbcook.cn/Article/details/grbeamcfm.sHtML

JS:   class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gvrsqxnll.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.yfazqb.com/Article/details/grutufusp.sHtML

Java: class User {}
来源：http://baike.epnwcf.com/Article/details/gbwonoviw.sHtML

Go:   type User struct { Name string }
来源：http://read.share.tarul.cn/Article/details/gmfszhbof.sHtML

Ruby: class User; end
来源：http://m.share.fktsv.cn/Article/details/gwujmpewj.sHtML

C#:   class User {}
来源：http://read.share.vehdjk.com/Article/details/ghfjjrtrt.sHtML

[G02] 构造函数
来源：http://wap.sjlbkw.cn/Article/details/gcgztwknf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.tarul.cn/Article/details/garecowdj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.bbcook.cn/Article/details/gecikpnvn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fktsv.cn/Article/details/gwskbwflh.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.sjlbkw.cn/Article/details/gnyvtglbk.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.tarul.cn/Article/details/gmamgcvds.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.bbcook.cn/Article/details/glgtxywxq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.yfazqb.com/Article/details/gbdjlqkxq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fktsv.cn/Article/details/gflanruia.sHtML

[G03] 实例属性
来源：http://baike.epnwcf.com/Article/details/gqwllthtl.sHtML

Py:   self.name = "x"
来源：http://www.m.share.vehdjk.com/Article/details/gfqdvicjp.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fktsv.cn/Article/details/gkqlfkcsy.sHtML

JS:   this.name = "x";
来源：http://3g.bbcook.cn/Article/details/gjzglrpam.sHtML

TS:   name: string = "x";
来源：http://www.share.bbcook.cn/Article/details/gmhhxkvdo.sHtML

Java: private String name;
来源：http://m.share.fktsv.cn/Article/details/gekqphbfy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.tarul.cn/Article/details/gymbnigua.sHtML

Ruby: @name = "x"
来源：http://read.share.bbcook.cn/Article/details/ghfkdkzcu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.vehdjk.com/Article/details/gqtnbfiud.sHtML

[G04] 定义方法
来源：http://www.blog.tarul.cn/Article/details/gbkarusyc.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.bbcook.cn/Article/details/gxkndhxfi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.vehdjk.com/Article/details/grxhjgelg.sHtML

JS:   greet() { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gqvpcmgck.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.bbcook.cn/Article/details/gmidbgoxf.sHtML

Java: String greet() { return name; }
来源：http://wap.epnwcf.com/Article/details/gsmqcuntj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.yfazqb.com/Article/details/gmfgwgwmc.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gypswoenh.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.vehdjk.com/Article/details/gixzjcamo.sHtML

[G05] 继承
来源：http://read.share.fktsv.cn/Article/details/gozgffoke.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.tarul.cn/Article/details/gezhywabj.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/gnsrqclzz.sHtML

JS:   class Admin extends User {}
来源：http://baike.fktsv.cn/Article/details/gforufeld.sHtML

TS:   class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gvhdiygjw.sHtML

Java: class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gamjvhoki.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.epnwcf.com/Article/details/grknkzmuv.sHtML

Ruby: class Admin < User; end
来源：http://3g.fktsv.cn/Article/details/gipmtozze.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.epnwcf.com/Article/details/gjnxklmxa.sHtML

[G06] 重写方法
来源：http://m.share.bbcook.cn/Article/details/gjveqxvko.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.vehdjk.com/Article/details/gxiqvcirv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/gcymgoixl.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/gdiamazct.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.tarul.cn/Article/details/givpwtytu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/gcwzwgblt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fktsv.cn/Article/details/gpgrikpki.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fktsv.cn/Article/details/goirkmccw.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.sjlbkw.cn/Article/details/gmndillqt.sHtML

[G07] 调用父类方法
来源：http://www.m.share.yfazqb.com/Article/details/gkhfjsedi.sHtML

Py:   super().greet()
来源：http://www.m.share.bbcook.cn/Article/details/ghhgfnqkc.sHtML

PHP:  parent::greet();
来源：http://www.m.share.bbcook.cn/Article/details/gtxtryfih.sHtML

JS:   super.greet();
来源：http://3g.yfazqb.com/Article/details/gmllpsexc.sHtML

TS:   super.greet();
来源：http://www.blog.tarul.cn/Article/details/gpmitutou.sHtML

Java: super.greet();
来源：http://www.share.vehdjk.com/Article/details/gccfzlwos.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.bbcook.cn/Article/details/gfxkulwys.sHtML

Ruby: super
来源：http://blog.tarul.cn/Article/details/gdtwrhqto.sHtML

C#:   base.Greet();
来源：http://www.m.share.bbcook.cn/Article/details/gzznfkzis.sHtML

[G08] 静态方法与属性
来源：http://baike.bbcook.cn/Article/details/gwyrmpdrr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.bbcook.cn/Article/details/gtbrtpklq.sHtML

PHP:  public static function f() {}
来源：http://baike.tarul.cn/Article/details/ghejvhldl.sHtML

JS:   static f() {}
来源：http://3g.vehdjk.com/Article/details/gzoiceeoh.sHtML

TS:   static f(): void {}
来源：http://baike.bbcook.cn/Article/details/ghhooqbsb.sHtML

Java: static void f() {}
来源：http://m.share.vehdjk.com/Article/details/gzrasihry.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.tarul.cn/Article/details/gqenxmjze.sHtML

Ruby: def self.f; end
来源：http://m.share.bbcook.cn/Article/details/ghfjukigg.sHtML

C#:   public static void F() {}
来源：http://wap.yfazqb.com/Article/details/geiescsnb.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.epnwcf.com/Article/details/gwozzgweu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.tarul.cn/Article/details/gfyukgooe.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fktsv.cn/Article/details/gycqebdpe.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.sjlbkw.cn/Article/details/gjowzpnla.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.epnwcf.com/Article/details/ggozcfadx.sHtML

Java: interface Shape { double area(); }
来源：http://baike.yfazqb.com/Article/details/glwlpmgut.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.vehdjk.com/Article/details/gmsczxcdf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.epnwcf.com/Article/details/gdqpobovu.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.sjlbkw.cn/Article/details/gajolqyql.sHtML

[G10] 访问控制
来源：http://baike.sjlbkw.cn/Article/details/gyzjifqoa.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.tarul.cn/Article/details/gqtktyuvr.sHtML

PHP:  public / protected / private
来源：http://3g.fktsv.cn/Article/details/gaimsllux.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.yfazqb.com/Article/details/ggoizcyab.sHtML

TS:   public / protected / private
来源：http://www.blog.sjlbkw.cn/Article/details/gpbnlvnbu.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.vehdjk.com/Article/details/gfcifkhqw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.sjlbkw.cn/Article/details/gjfondamq.sHtML

Ruby: public / protected / private
来源：http://www.share.epnwcf.com/Article/details/grtogfufn.sHtML

C#:   public / protected / private / internal
来源：http://baike.epnwcf.com/Article/details/gqfzucmqc.sHtML

[G11] getter / setter
来源：http://baike.bbcook.cn/Article/details/gltmemhzt.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.vehdjk.com/Article/details/geiabelgc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fktsv.cn/Article/details/gxjkbqquo.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.tarul.cn/Article/details/gesstibeq.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.tarul.cn/Article/details/gnohjcpcf.sHtML

Java: public String getName() { return name; }
来源：http://wap.tarul.cn/Article/details/gxfalhzvr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/gounotjvb.sHtML

Ruby: attr_accessor :name
来源：http://www.share.epnwcf.com/Article/details/gixmrwrqa.sHtML

C#:   public string Name { get; set; }
来源：http://wap.yfazqb.com/Article/details/gxpwnorxs.sHtML

[G12] 对象转字符串
来源：http://www.m.share.tarul.cn/Article/details/gatywuunm.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.epnwcf.com/Article/details/gwzztpfue.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/gqshbohpu.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.bbcook.cn/Article/details/gzsellnwt.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.bbcook.cn/Article/details/gbcckhzdp.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.bbcook.cn/Article/details/ggsoieavg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.bbcook.cn/Article/details/grqyrbjqw.sHtML

Ruby: def to_s; @name; end
来源：http://3g.epnwcf.com/Article/details/ggerjmdam.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fktsv.cn/Article/details/gdbdyoaav.sHtML

[G13] 判断对象类型
来源：http://www.m.share.tarul.cn/Article/details/gaxglfkqr.sHtML

Py:   isinstance(u, User)
来源：http://blog.sjlbkw.cn/Article/details/gqrpleblu.sHtML

PHP:  $u instanceof User
来源：http://wap.bbcook.cn/Article/details/gngtnnwky.sHtML

JS:   u instanceof User
来源：http://baike.bbcook.cn/Article/details/gnzdfyrrf.sHtML

TS:   u instanceof User
来源：http://mobile.tarul.cn/Article/details/giosykaap.sHtML

Java: u instanceof User
来源：http://mobile.tarul.cn/Article/details/gagfpcczb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.vehdjk.com/Article/details/gjfmfxjos.sHtML

Ruby: u.is_a?(User)
来源：http://wap.tarul.cn/Article/details/grqrrgahz.sHtML

C#:   u is User
来源：http://www.blog.fktsv.cn/Article/details/ggsvptwll.sHtML

[G14] 数据类 / record
来源：http://blog.yfazqb.com/Article/details/gdftegyyn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.epnwcf.com/Article/details/gdqxxhovn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.vehdjk.com/Article/details/gtmghzeuv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.bbcook.cn/Article/details/gtnjeyjmr.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.yfazqb.com/Article/details/gnpwalosi.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fktsv.cn/Article/details/guqyhxtco.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fktsv.cn/Article/details/gvnpiuiwz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.bbcook.cn/Article/details/grhdclksf.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.tarul.cn/Article/details/gmzmbbqva.sHtML

[G15] 枚举
来源：http://3g.bbcook.cn/Article/details/gajcwrpiw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.yfazqb.com/Article/details/gwrwkazjr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fktsv.cn/Article/details/gihbghvaf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.vehdjk.com/Article/details/gqzwcnpba.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fktsv.cn/Article/details/gpbgusups.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fktsv.cn/Article/details/giwbtndbj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.yfazqb.com/Article/details/gxgianjwk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.sjlbkw.cn/Article/details/ghcgxeynj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.tarul.cn/Article/details/gijvdeleu.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.bbcook.cn/Article/details/gvubnxfwa.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fktsv.cn/Article/details/gbztyxbld.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.epnwcf.com/Article/details/gmbjnjbbk.sHtML

JS:   Object.entries(obj)
来源：http://baike.vehdjk.com/Article/details/gmqqrjfea.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.vehdjk.com/Article/details/gwathfflt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fktsv.cn/Article/details/gkcsutskh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.yfazqb.com/Article/details/gxixvgddp.sHtML

Ruby: obj.instance_variables
来源：http://m.share.bbcook.cn/Article/details/gorddmmnx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.tarul.cn/Article/details/gbniltyce.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gzlnxwkfo.sHtML

H. 异常与错误处理
来源：http://m.share.yfazqb.com/Article/details/gpaaxnoqu.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gzmfitqor.sHtML

[H01] try / catch 基础
来源：http://mobile.sjlbkw.cn/Article/details/gmbkngecg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.tarul.cn/Article/details/gmyaiatbv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.yfazqb.com/Article/details/gfprjwzgw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.sjlbkw.cn/Article/details/gnpoujvgm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.epnwcf.com/Article/details/gmfcpxknk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.tarul.cn/Article/details/gufmkrigl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.tarul.cn/Article/details/grvapgzpd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.bbcook.cn/Article/details/gzwtpihbd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.tarul.cn/Article/details/gfplckntd.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fktsv.cn/Article/details/gbqeeudoq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.bbcook.cn/Article/details/gahlgpodt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gaomkqzqg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gwwdujptn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.bbcook.cn/Article/details/gaikyjdfq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.tarul.cn/Article/details/gwmwgxrnj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fktsv.cn/Article/details/guilzbwtm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.yfazqb.com/Article/details/grurcdwbh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fktsv.cn/Article/details/gnijiflob.sHtML


<!-- 参考信息 -->