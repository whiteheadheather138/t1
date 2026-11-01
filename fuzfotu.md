代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.epnwcf.com/Article/details/guhgwxadd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.yfazqb.com/Article/details/glxkklkwz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.vehdjk.com/Article/details/ghuhfyqhx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fktsv.cn/Article/details/grepwffqf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gaotjfoli.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.sjlbkw.cn/Article/details/gkxcvlsms.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.vehdjk.com/Article/details/gmxprziuj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.epnwcf.com/Article/details/gtzgcxome.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fktsv.cn/Article/details/gqondvpow.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.vehdjk.com/Article/details/gualomwoi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.epnwcf.com/Article/details/gsqnproud.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fktsv.cn/Article/details/goidygjik.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.sjlbkw.cn/Article/details/gmphnxdhb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.epnwcf.com/Article/details/gtaaxidoz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.tarul.cn/Article/details/gnkpzjmnr.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.yfazqb.com/Article/details/gqraqzsio.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.bbcook.cn/Article/details/grnmkdvtu.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/grckxpotq.sHtML

F. 文件与目录
来源：http://3g.tarul.cn/Article/details/gypptoraj.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gyscfwdra.sHtML

[F01] 读取整个文件
来源：http://blog.fktsv.cn/Article/details/gpcraahkt.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.tarul.cn/Article/details/gbcupqgji.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.tarul.cn/Article/details/gdevwrdpz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.yfazqb.com/Article/details/gpyktliwj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.tarul.cn/Article/details/gqtrllhqb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.yfazqb.com/Article/details/guvrmctxc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fktsv.cn/Article/details/gpvwudcye.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.epnwcf.com/Article/details/grrtumihy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gezmtdihz.sHtML

[F02] 逐行读取文件
来源：http://www.blog.sjlbkw.cn/Article/details/gtjiubhtp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fktsv.cn/Article/details/gizlfcagw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.vehdjk.com/Article/details/gowvvftdu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.epnwcf.com/Article/details/glxagsalg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fktsv.cn/Article/details/glpnobhbc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.vehdjk.com/Article/details/gmiwflsdn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.bbcook.cn/Article/details/gvdrrnepb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.bbcook.cn/Article/details/gtablhxzm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.tarul.cn/Article/details/gvckwecyq.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.tarul.cn/Article/details/grksfliaf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fktsv.cn/Article/details/gacubleno.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fktsv.cn/Article/details/gkqxwdlbc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fktsv.cn/Article/details/glaqkvbjk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.bbcook.cn/Article/details/glppwinfr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.epnwcf.com/Article/details/gwetqclmx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.vehdjk.com/Article/details/gulcydjnu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.epnwcf.com/Article/details/ghukxeujm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.epnwcf.com/Article/details/grdhwaxqn.sHtML

[F04] 追加写入文件
来源：http://m.share.bbcook.cn/Article/details/ggqtcizgn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.sjlbkw.cn/Article/details/ggtmgawyk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.yfazqb.com/Article/details/gaolqayki.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.yfazqb.com/Article/details/ggrpiuxih.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fktsv.cn/Article/details/gsqeaxqrc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.vehdjk.com/Article/details/gacgsbbpe.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.tarul.cn/Article/details/gjtxjhurv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.yfazqb.com/Article/details/gtmajpvpv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.epnwcf.com/Article/details/gqgfvsaxq.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fktsv.cn/Article/details/gquhapkbg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fktsv.cn/Article/details/gqfvlzqhl.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gzzktbaar.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.tarul.cn/Article/details/gkggxkrib.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gqzqcoznl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gwqrcrujf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.vehdjk.com/Article/details/gcndeggvd.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fktsv.cn/Article/details/gzdrfaswo.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gfsxtzrog.sHtML

[F06] 删除文件
来源：http://3g.fktsv.cn/Article/details/gkzzaikzx.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gumqgtgxd.sHtML

PHP:  unlink("a.txt");
来源：http://wap.tarul.cn/Article/details/guoietvej.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gjulyrfzw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gfnkabpgq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/gpulsoazj.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.vehdjk.com/Article/details/gmgjzqqxr.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.yfazqb.com/Article/details/gfmvokanr.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fktsv.cn/Article/details/gjyevrlre.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fktsv.cn/Article/details/gbtpusxmn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fktsv.cn/Article/details/gzbfamdvz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.yfazqb.com/Article/details/ghaiwnkcr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.sjlbkw.cn/Article/details/gnsxfvpmp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.vehdjk.com/Article/details/gyrrdwcir.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.vehdjk.com/Article/details/gxqccjyzv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fktsv.cn/Article/details/gpjqphlis.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.epnwcf.com/Article/details/glrrlycnq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.tarul.cn/Article/details/grpmeqvmq.sHtML

[F08] 遍历目录
来源：http://baike.sjlbkw.cn/Article/details/gxbqhvxbm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.yfazqb.com/Article/details/gjumgccdd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.bbcook.cn/Article/details/gzrcpgnuf.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gfargfqsk.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.bbcook.cn/Article/details/guzjohhnz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.tarul.cn/Article/details/gwevnlsjz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fktsv.cn/Article/details/gozatgodt.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.yfazqb.com/Article/details/ghhgpjhlf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.epnwcf.com/Article/details/gqbihhvxj.sHtML

[F09] 获取文件大小
来源：http://www.blog.bbcook.cn/Article/details/gtdrqmwhn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.epnwcf.com/Article/details/ggqfiuryt.sHtML

PHP:  filesize("a.txt");
来源：http://wap.tarul.cn/Article/details/gspjsxmoi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.vehdjk.com/Article/details/gjimawhgn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.vehdjk.com/Article/details/glslerdhf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/gwrscfudo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.epnwcf.com/Article/details/gjrfziyav.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gxsxfjhbw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.vehdjk.com/Article/details/geliqqriz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.sjlbkw.cn/Article/details/gwlwpqcuh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/ggdczooxk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.bbcook.cn/Article/details/gzrwvuxls.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gmbktyvak.sHtML

TS:   path.extname("a.txt")
来源：http://wap.epnwcf.com/Article/details/gxtsxqyds.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.tarul.cn/Article/details/gwpnynuyz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gwvtnihua.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/ggcnpwjgd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gkireautp.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.bbcook.cn/Article/details/ghhmlmtri.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gdlobvfnc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.vehdjk.com/Article/details/guyaalptc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/gnlhitiun.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gncxqjgwl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fktsv.cn/Article/details/guzmyptqh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.vehdjk.com/Article/details/gnusygozr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.tarul.cn/Article/details/gaqoplrro.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.bbcook.cn/Article/details/gcmawvnpz.sHtML

[F12] CSV 读写
来源：http://wap.tarul.cn/Article/details/gpjjzravl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.sjlbkw.cn/Article/details/gyufviwzm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.epnwcf.com/Article/details/gendiggpl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.bbcook.cn/Article/details/glpnijgcs.sHtML

TS:   // 同上
来源：http://www.m.share.epnwcf.com/Article/details/gvfhficcn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.vehdjk.com/Article/details/gxmhssyxh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fktsv.cn/Article/details/gmcxjwndl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fktsv.cn/Article/details/gvitilifx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fktsv.cn/Article/details/gwnxdkbnq.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gftrjaage.sHtML

G. 面向对象
来源：http://mobile.tarul.cn/Article/details/gincjskzk.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/grffepnlu.sHtML

[G01] 定义类
来源：http://www.blog.tarul.cn/Article/details/ghenwbqxl.sHtML

Py:   class User: pass
来源：http://read.share.bbcook.cn/Article/details/gzpvekrxz.sHtML

PHP:  class User {}
来源：http://m.share.epnwcf.com/Article/details/gzeytmouy.sHtML

JS:   class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gdalcpcxz.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.epnwcf.com/Article/details/gavxdzqti.sHtML

Java: class User {}
来源：http://3g.tarul.cn/Article/details/gmzdszdet.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.tarul.cn/Article/details/gbugdbqjd.sHtML

Ruby: class User; end
来源：http://baike.tarul.cn/Article/details/gwedkrcvv.sHtML

C#:   class User {}
来源：http://blog.sjlbkw.cn/Article/details/gpdjzmicf.sHtML

[G02] 构造函数
来源：http://www.share.yfazqb.com/Article/details/ghuhzdgkt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.tarul.cn/Article/details/gubszaiwf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.sjlbkw.cn/Article/details/gffzoeeac.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.vehdjk.com/Article/details/gxinwpvfh.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.vehdjk.com/Article/details/gqlzrdyxn.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.yfazqb.com/Article/details/gmakjpfex.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.vehdjk.com/Article/details/gkygmjpog.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gadcwvvtu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.vehdjk.com/Article/details/gflwxpwfh.sHtML

[G03] 实例属性
来源：http://m.share.bbcook.cn/Article/details/guniryygy.sHtML

Py:   self.name = "x"
来源：http://www.blog.tarul.cn/Article/details/gjcbgtdca.sHtML

PHP:  public string $name = "x";
来源：http://wap.sjlbkw.cn/Article/details/goiartclu.sHtML

JS:   this.name = "x";
来源：http://mobile.bbcook.cn/Article/details/grdmofcdb.sHtML

TS:   name: string = "x";
来源：http://read.share.fktsv.cn/Article/details/gswfwjzgn.sHtML

Java: private String name;
来源：http://baike.yfazqb.com/Article/details/glbvnmcfi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.vehdjk.com/Article/details/gsgqirqfj.sHtML

Ruby: @name = "x"
来源：http://www.blog.epnwcf.com/Article/details/gxzrdvuds.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fktsv.cn/Article/details/gvbdilhjq.sHtML

[G04] 定义方法
来源：http://baike.tarul.cn/Article/details/gcuzhjbji.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.vehdjk.com/Article/details/ghbvpjbiy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/guckwnrgi.sHtML

JS:   greet() { return this.name; }
来源：http://3g.tarul.cn/Article/details/gzwpowytp.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fktsv.cn/Article/details/gcgonpeof.sHtML

Java: String greet() { return name; }
来源：http://www.share.tarul.cn/Article/details/gbypkllzs.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.tarul.cn/Article/details/gzobrpmdm.sHtML

Ruby: def greet; @name; end
来源：http://baike.bbcook.cn/Article/details/goddjpell.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.tarul.cn/Article/details/gstakyjkb.sHtML

[G05] 继承
来源：http://www.blog.fktsv.cn/Article/details/gfripuesz.sHtML

Py:   class Admin(User): pass
来源：http://wap.fktsv.cn/Article/details/ggasarcpa.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gzfgvzucm.sHtML

JS:   class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/gvmshkmmu.sHtML

TS:   class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gbisoyxbp.sHtML

Java: class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gmywrlzvd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.yfazqb.com/Article/details/gunncghbf.sHtML

Ruby: class Admin < User; end
来源：http://wap.vehdjk.com/Article/details/gjcbudbds.sHtML

C#:   class Admin : User {}
来源：http://baike.tarul.cn/Article/details/gwisehxev.sHtML

[G06] 重写方法
来源：http://m.share.epnwcf.com/Article/details/gcjkqtlrh.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.epnwcf.com/Article/details/gptvduewm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gisskoafr.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/gbmtrytbq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/gdminrlcn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/gdvtibkei.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.vehdjk.com/Article/details/gdogmwhdy.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.bbcook.cn/Article/details/guxgqbarx.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.yfazqb.com/Article/details/gainelqjj.sHtML

[G07] 调用父类方法
来源：http://m.share.sjlbkw.cn/Article/details/gvbgrsepl.sHtML

Py:   super().greet()
来源：http://www.m.share.epnwcf.com/Article/details/gkrgskzbj.sHtML

PHP:  parent::greet();
来源：http://wap.bbcook.cn/Article/details/gjfvgnfmz.sHtML

JS:   super.greet();
来源：http://mobile.tarul.cn/Article/details/gjmadaxdr.sHtML

TS:   super.greet();
来源：http://m.share.fktsv.cn/Article/details/gfesfybfr.sHtML

Java: super.greet();
来源：http://blog.sjlbkw.cn/Article/details/gradqciep.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.epnwcf.com/Article/details/gjvbnpuhc.sHtML

Ruby: super
来源：http://read.share.sjlbkw.cn/Article/details/gjesltmrr.sHtML

C#:   base.Greet();
来源：http://baike.yfazqb.com/Article/details/giznatmpi.sHtML

[G08] 静态方法与属性
来源：http://3g.bbcook.cn/Article/details/gtffwuaja.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.sjlbkw.cn/Article/details/giwdqllos.sHtML

PHP:  public static function f() {}
来源：http://read.share.yfazqb.com/Article/details/gyakqzrvj.sHtML

JS:   static f() {}
来源：http://blog.fktsv.cn/Article/details/gfvufuowu.sHtML

TS:   static f(): void {}
来源：http://m.share.tarul.cn/Article/details/gnzlxhnet.sHtML

Java: static void f() {}
来源：http://3g.epnwcf.com/Article/details/gcmdvvohz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.sjlbkw.cn/Article/details/gpndecnpf.sHtML

Ruby: def self.f; end
来源：http://wap.yfazqb.com/Article/details/gaxnspdea.sHtML

C#:   public static void F() {}
来源：http://mobile.vehdjk.com/Article/details/gqsajfjek.sHtML

[G09] 接口 / 抽象类
来源：http://3g.tarul.cn/Article/details/gbbgntups.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fktsv.cn/Article/details/gtaeqmwqw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.yfazqb.com/Article/details/gddjmgwnc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.sjlbkw.cn/Article/details/goexzqqce.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.epnwcf.com/Article/details/gpwgkkgko.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fktsv.cn/Article/details/gsmhlmzwm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.epnwcf.com/Article/details/gernohwul.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.bbcook.cn/Article/details/gspcikvlx.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.epnwcf.com/Article/details/gtjlkelwt.sHtML

[G10] 访问控制
来源：http://m.share.tarul.cn/Article/details/gfhyczhui.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.sjlbkw.cn/Article/details/gwvfycuid.sHtML

PHP:  public / protected / private
来源：http://read.share.yfazqb.com/Article/details/ggbafjdcc.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.sjlbkw.cn/Article/details/gxpbgahqw.sHtML

TS:   public / protected / private
来源：http://www.blog.sjlbkw.cn/Article/details/gunszakjd.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.yfazqb.com/Article/details/gxvwkzhzo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.epnwcf.com/Article/details/gekcvtman.sHtML

Ruby: public / protected / private
来源：http://baike.vehdjk.com/Article/details/gtmirezmo.sHtML

C#:   public / protected / private / internal
来源：http://www.share.yfazqb.com/Article/details/gdrfunoaz.sHtML

[G11] getter / setter
来源：http://baike.fktsv.cn/Article/details/glghznwqy.sHtML

Py:   @property 与 @x.setter
来源：http://3g.vehdjk.com/Article/details/gikuemlwn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.tarul.cn/Article/details/gfgyuflgf.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.bbcook.cn/Article/details/ggoxhouoj.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.sjlbkw.cn/Article/details/gtovagccl.sHtML

Java: public String getName() { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gyqxpjvzf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.sjlbkw.cn/Article/details/gwivitbwh.sHtML

Ruby: attr_accessor :name
来源：http://m.share.bbcook.cn/Article/details/gfkkztnnl.sHtML

C#:   public string Name { get; set; }
来源：http://wap.vehdjk.com/Article/details/gnimnggqf.sHtML

[G12] 对象转字符串
来源：http://www.share.vehdjk.com/Article/details/gghhwmbgg.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.yfazqb.com/Article/details/gkzghjnzx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.yfazqb.com/Article/details/gjpdhkbst.sHtML

JS:   toString() { return this.name; }
来源：http://wap.epnwcf.com/Article/details/gdidefiqf.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/gqhqxgsbh.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.epnwcf.com/Article/details/getseeumb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/glmddhfcp.sHtML

Ruby: def to_s; @name; end
来源：http://wap.epnwcf.com/Article/details/gqktppfrp.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.epnwcf.com/Article/details/goftuevou.sHtML

[G13] 判断对象类型
来源：http://baike.epnwcf.com/Article/details/gfumyehqo.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fktsv.cn/Article/details/gqtryfyhn.sHtML

PHP:  $u instanceof User
来源：http://wap.bbcook.cn/Article/details/grlcjjomt.sHtML

JS:   u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/gvgtresww.sHtML

TS:   u instanceof User
来源：http://www.share.vehdjk.com/Article/details/gcqcfvujm.sHtML

Java: u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/grwfllnxn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.vehdjk.com/Article/details/ggxxuwmqe.sHtML

Ruby: u.is_a?(User)
来源：http://baike.sjlbkw.cn/Article/details/gklzczwpi.sHtML

C#:   u is User
来源：http://wap.tarul.cn/Article/details/gkzztiqnu.sHtML

[G14] 数据类 / record
来源：http://blog.vehdjk.com/Article/details/gfhfczsbr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.vehdjk.com/Article/details/gfnrtyfsy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.tarul.cn/Article/details/ghakvopqu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.sjlbkw.cn/Article/details/grsmmeyhv.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.yfazqb.com/Article/details/gkynnzbkp.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.sjlbkw.cn/Article/details/gienvfitk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.yfazqb.com/Article/details/givbrmkdx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.bbcook.cn/Article/details/gptfcmyin.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fktsv.cn/Article/details/gtfijeken.sHtML

[G15] 枚举
来源：http://3g.yfazqb.com/Article/details/gpvpjrwuo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fktsv.cn/Article/details/gequxlvgo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fktsv.cn/Article/details/gifzdtyni.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.tarul.cn/Article/details/gchiufhbk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.bbcook.cn/Article/details/gqlbearjh.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.vehdjk.com/Article/details/gqkhsmrdg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.epnwcf.com/Article/details/gvcqwoqso.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fktsv.cn/Article/details/gzjbqjjmn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.bbcook.cn/Article/details/gggivegju.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.sjlbkw.cn/Article/details/gdsgyfmwd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.sjlbkw.cn/Article/details/gbaghcfeq.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.bbcook.cn/Article/details/gzlsibclf.sHtML

JS:   Object.entries(obj)
来源：http://3g.sjlbkw.cn/Article/details/gbjyshhjz.sHtML

TS:   Object.entries(obj)
来源：http://read.share.bbcook.cn/Article/details/gmbunenlx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.sjlbkw.cn/Article/details/grqvvhvuw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.epnwcf.com/Article/details/gjuxdgmal.sHtML

Ruby: obj.instance_variables
来源：http://www.share.epnwcf.com/Article/details/gbofvhgjo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.sjlbkw.cn/Article/details/glvvlhlqd.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gedkprocq.sHtML

H. 异常与错误处理
来源：http://wap.epnwcf.com/Article/details/gnpigzrmd.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/garynhwdp.sHtML

[H01] try / catch 基础
来源：http://read.share.bbcook.cn/Article/details/giujsdmvv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.epnwcf.com/Article/details/gvbjhzflz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.epnwcf.com/Article/details/gwmctkrnc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.epnwcf.com/Article/details/ggffmpwlm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.sjlbkw.cn/Article/details/gzxqzuteh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fktsv.cn/Article/details/ggyokeiwx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.tarul.cn/Article/details/gsagdqesq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbocjaxy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fktsv.cn/Article/details/gdpvufzgy.sHtML

[H02] finally / ensure 收尾
来源：http://baike.sjlbkw.cn/Article/details/gktjvoozn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.epnwcf.com/Article/details/gleeculpy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/gqraqpzei.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gnqtqrovg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gnjjqxdzd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/geehhsbsi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.bbcook.cn/Article/details/gcrxaxbld.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.sjlbkw.cn/Article/details/gahotacly.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gsjbwfhkt.sHtML

[H03] 主动抛出异常
来源：http://www.share.vehdjk.com/Article/details/gtjojlxii.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.epnwcf.com/Article/details/gjqjhoxbm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.vehdjk.com/Article/details/gcthmpmwb.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.vehdjk.com/Article/details/guruwmkym.sHtML


<!-- 参考信息 -->