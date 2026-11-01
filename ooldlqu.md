代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://read.share.vehdjk.com/Article/details/gedhgcmax.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.bbcook.cn/Article/details/gghilyiuy.sHtML

Java: s.lines().toList()
来源：http://www.m.share.epnwcf.com/Article/details/gwcmxndbl.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.tarul.cn/Article/details/gzmxxhbvy.sHtML

Ruby: s.lines
来源：http://www.share.yfazqb.com/Article/details/gycpfmllx.sHtML

C#:   s.Split('\n')
来源：http://mobile.tarul.cn/Article/details/grlanivxu.sHtML

[E20] 判断字符串是否为空
来源：http://baike.tarul.cn/Article/details/gcqxlxhxl.sHtML

Py:   if not s:
来源：http://blog.yfazqb.com/Article/details/gmpoxcyhx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fktsv.cn/Article/details/gvaktjjsr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fktsv.cn/Article/details/ghxjkicbh.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fktsv.cn/Article/details/gsonvuyyq.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.yfazqb.com/Article/details/gnvudbjwr.sHtML

Go:   if s == "" {}
来源：http://wap.fktsv.cn/Article/details/gcdfcfnsq.sHtML

Ruby: if s.empty?
来源：http://wap.fktsv.cn/Article/details/gyhtpueux.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.tarul.cn/Article/details/gyeydzefc.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.sjlbkw.cn/Article/details/gngeuuqif.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.yfazqb.com/Article/details/gomyxupfj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.yfazqb.com/Article/details/gxtitpald.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.epnwcf.com/Article/details/guhuncwaq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gtwjbeqaj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/giabrbghs.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.vehdjk.com/Article/details/gfzmwnbks.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gisqooewy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.epnwcf.com/Article/details/gptxfgitp.sHtML

[E22] 字节长度与字符长度
来源：http://baike.sjlbkw.cn/Article/details/gsxzfzbpy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.bbcook.cn/Article/details/gjotjukmr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/gqiawtrtj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.sjlbkw.cn/Article/details/gojbbannp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.yfazqb.com/Article/details/gyvfxpjvt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.tarul.cn/Article/details/gdztfzjzk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.sjlbkw.cn/Article/details/gdmdnbzth.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.tarul.cn/Article/details/gdxtjcozk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.vehdjk.com/Article/details/gkzxqjbuh.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gwpfibdad.sHtML

F. 文件与目录
来源：http://wap.tarul.cn/Article/details/ggyismkhx.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gjlazvtyd.sHtML

[F01] 读取整个文件
来源：http://wap.epnwcf.com/Article/details/gqgxupayl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.tarul.cn/Article/details/gltlxeqzh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fktsv.cn/Article/details/gmkgavlln.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.sjlbkw.cn/Article/details/gwtyqkker.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.vehdjk.com/Article/details/gybjfiiuh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.yfazqb.com/Article/details/gljfcnyia.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.tarul.cn/Article/details/gexziivru.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gubvsstra.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gtpkoktqi.sHtML

[F02] 逐行读取文件
来源：http://wap.bbcook.cn/Article/details/gouxgzrhj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.tarul.cn/Article/details/gdgjsoury.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.sjlbkw.cn/Article/details/grivewjsv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.vehdjk.com/Article/details/gsnwlctkh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fktsv.cn/Article/details/geojbvspq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.tarul.cn/Article/details/gvwuxbtbs.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.epnwcf.com/Article/details/grrymfyln.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.epnwcf.com/Article/details/gegnnpdga.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.vehdjk.com/Article/details/gloezslax.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.vehdjk.com/Article/details/gvxposjjd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.epnwcf.com/Article/details/guasdwvzs.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.sjlbkw.cn/Article/details/gfdlouonu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.tarul.cn/Article/details/glapefbdt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fktsv.cn/Article/details/gmhouttdd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.epnwcf.com/Article/details/gbnpanvfo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.epnwcf.com/Article/details/ggodagmrj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.vehdjk.com/Article/details/gjzvzswaz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.epnwcf.com/Article/details/gteymqzxi.sHtML

[F04] 追加写入文件
来源：http://www.blog.tarul.cn/Article/details/gpzconegy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.vehdjk.com/Article/details/giofstjnv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.vehdjk.com/Article/details/guiltyfso.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.bbcook.cn/Article/details/gtfqzkyzp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.yfazqb.com/Article/details/gmwjiaxym.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.bbcook.cn/Article/details/gayyrrczy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fktsv.cn/Article/details/ggldbgcfy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fktsv.cn/Article/details/gpedgsxub.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fktsv.cn/Article/details/goeawskqj.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.bbcook.cn/Article/details/gimxzummx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.tarul.cn/Article/details/ghdzpyyrf.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gkrqzrczc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gdlrkkdgs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gcpzwtsxh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gxidmtckl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.sjlbkw.cn/Article/details/gatmepgme.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/goglhtrhl.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.bbcook.cn/Article/details/ghmwdeghu.sHtML

[F06] 删除文件
来源：http://blog.tarul.cn/Article/details/gmofxzftp.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gielpjthv.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/ghybecply.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/ghknulklt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gzzpkdhfr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fktsv.cn/Article/details/gdjekeoaf.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.bbcook.cn/Article/details/gsecqgbtj.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gnrrsdkcq.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.tarul.cn/Article/details/gevkoeuid.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.bbcook.cn/Article/details/gjwxkdkjx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.bbcook.cn/Article/details/gfeuamdvo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fktsv.cn/Article/details/grkelzreu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.tarul.cn/Article/details/giicsyjyu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.tarul.cn/Article/details/gqtdwncld.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.vehdjk.com/Article/details/gjskyhcqk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fktsv.cn/Article/details/gkvfztxwj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fktsv.cn/Article/details/gkqrhegmu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.yfazqb.com/Article/details/gsovseyuy.sHtML

[F08] 遍历目录
来源：http://3g.vehdjk.com/Article/details/gkkqmskwv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.tarul.cn/Article/details/gjscaqney.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fktsv.cn/Article/details/grzzolkxx.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.tarul.cn/Article/details/glgxxkbcu.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gluvfymaz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.epnwcf.com/Article/details/gxhwvosuv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.tarul.cn/Article/details/grlwmdaza.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fktsv.cn/Article/details/gsyxuewxo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.yfazqb.com/Article/details/giwkkobqq.sHtML

[F09] 获取文件大小
来源：http://www.share.bbcook.cn/Article/details/gekbxhioh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.tarul.cn/Article/details/godpwzuhu.sHtML

PHP:  filesize("a.txt");
来源：http://baike.yfazqb.com/Article/details/gsqrzjbej.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.vehdjk.com/Article/details/gnspssghi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.bbcook.cn/Article/details/gwkvradrx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/gkoaqdcbf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.sjlbkw.cn/Article/details/gljxmszbn.sHtML

Ruby: File.size("a.txt")
来源：http://blog.yfazqb.com/Article/details/gydsvqvox.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.vehdjk.com/Article/details/gwnluhmab.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fktsv.cn/Article/details/gyaessxyp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/ggulodyca.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.vehdjk.com/Article/details/gznfjjycv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gznrkkofz.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fktsv.cn/Article/details/gqhpiyvxc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fktsv.cn/Article/details/gwqduydjd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/ggeakprdr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gducailoh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gvdcflfqn.sHtML

[F11] 复制与移动文件
来源：http://read.share.bbcook.cn/Article/details/giwdurkbv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/gzzkrqtxp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gnxbzfbzk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/gfbwevnot.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gtajapfkw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fktsv.cn/Article/details/gzvtempkf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.bbcook.cn/Article/details/gfmscitld.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/gdilkeclq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fktsv.cn/Article/details/grbcsermu.sHtML

[F12] CSV 读写
来源：http://read.share.yfazqb.com/Article/details/gbtjfizsu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.yfazqb.com/Article/details/grxqgkmji.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.epnwcf.com/Article/details/grwlyaxei.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fktsv.cn/Article/details/ggnujhtiu.sHtML

TS:   // 同上
来源：http://baike.epnwcf.com/Article/details/gufhiksie.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.tarul.cn/Article/details/gagzyrmkm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.tarul.cn/Article/details/gftysrftk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.yfazqb.com/Article/details/gqryaszkd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.bbcook.cn/Article/details/gclxugfbv.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gcxqhdkew.sHtML

G. 面向对象
来源：http://3g.tarul.cn/Article/details/gnobmdzxm.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/giofbajzj.sHtML

[G01] 定义类
来源：http://wap.vehdjk.com/Article/details/gjotlsvif.sHtML

Py:   class User: pass
来源：http://baike.bbcook.cn/Article/details/gzdzgqdxq.sHtML

PHP:  class User {}
来源：http://baike.sjlbkw.cn/Article/details/gmqkttpfm.sHtML

JS:   class User {}
来源：http://3g.sjlbkw.cn/Article/details/gpjbpqjwk.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fktsv.cn/Article/details/gaiwubqbi.sHtML

Java: class User {}
来源：http://mobile.fktsv.cn/Article/details/gdtjulqiu.sHtML

Go:   type User struct { Name string }
来源：http://m.share.yfazqb.com/Article/details/gtthiknco.sHtML

Ruby: class User; end
来源：http://3g.vehdjk.com/Article/details/gpbrllczl.sHtML

C#:   class User {}
来源：http://blog.sjlbkw.cn/Article/details/ghdqfvydp.sHtML

[G02] 构造函数
来源：http://read.share.fktsv.cn/Article/details/genlxmrjf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.sjlbkw.cn/Article/details/gupmcxxqq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.epnwcf.com/Article/details/ghfpmwjwf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.tarul.cn/Article/details/gegbkptjo.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.bbcook.cn/Article/details/gsbrmoxeq.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmlnjetn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.sjlbkw.cn/Article/details/gqbjejfoc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fktsv.cn/Article/details/gdkuyuqfc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.tarul.cn/Article/details/gxozmdefq.sHtML

[G03] 实例属性
来源：http://3g.sjlbkw.cn/Article/details/ggxlatvvw.sHtML

Py:   self.name = "x"
来源：http://www.m.share.sjlbkw.cn/Article/details/grmcaszdb.sHtML

PHP:  public string $name = "x";
来源：http://baike.sjlbkw.cn/Article/details/gwvsijvgd.sHtML

JS:   this.name = "x";
来源：http://m.share.fktsv.cn/Article/details/gkfaghhga.sHtML

TS:   name: string = "x";
来源：http://www.blog.vehdjk.com/Article/details/gmloleniu.sHtML

Java: private String name;
来源：http://baike.fktsv.cn/Article/details/gmzgacxhm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.epnwcf.com/Article/details/gorjbjfdc.sHtML

Ruby: @name = "x"
来源：http://www.m.share.vehdjk.com/Article/details/gpuugvpji.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gkcgkbqbi.sHtML

[G04] 定义方法
来源：http://www.m.share.epnwcf.com/Article/details/gstxvtwyv.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.tarul.cn/Article/details/grmmfsspy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/guuysadxw.sHtML

JS:   greet() { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gyvibhsea.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gmsinlhvb.sHtML

Java: String greet() { return name; }
来源：http://baike.tarul.cn/Article/details/ghmrdbcyo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.tarul.cn/Article/details/gdvuzokei.sHtML

Ruby: def greet; @name; end
来源：http://wap.epnwcf.com/Article/details/gejytvwar.sHtML

C#:   public string Greet() => Name;
来源：http://wap.vehdjk.com/Article/details/gnnlfpwvm.sHtML

[G05] 继承
来源：http://www.share.epnwcf.com/Article/details/ghuwjrkej.sHtML

Py:   class Admin(User): pass
来源：http://baike.yfazqb.com/Article/details/gdlkvlrmh.sHtML

PHP:  class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/ghzybdqrf.sHtML

JS:   class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gwugqansl.sHtML

TS:   class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/gllmplayo.sHtML

Java: class Admin extends User {}
来源：http://mobile.fktsv.cn/Article/details/gceddmglt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.bbcook.cn/Article/details/gghwivcou.sHtML

Ruby: class Admin < User; end
来源：http://wap.bbcook.cn/Article/details/gyukoicxz.sHtML

C#:   class Admin : User {}
来源：http://m.share.sjlbkw.cn/Article/details/gtcvtbpbm.sHtML

[G06] 重写方法
来源：http://www.blog.sjlbkw.cn/Article/details/gdpdfpnqq.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.bbcook.cn/Article/details/gltlkqaoc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/gmlmwtlib.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/gvuhcgqip.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/gvljdqmgn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/gsqhlquos.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.yfazqb.com/Article/details/grosgzpwn.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.vehdjk.com/Article/details/gfkriuzof.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.sjlbkw.cn/Article/details/gyirtxwvo.sHtML

[G07] 调用父类方法
来源：http://blog.fktsv.cn/Article/details/gixjqkohc.sHtML

Py:   super().greet()
来源：http://www.m.share.vehdjk.com/Article/details/gwgkjbaux.sHtML

PHP:  parent::greet();
来源：http://baike.bbcook.cn/Article/details/ghopggltu.sHtML

JS:   super.greet();
来源：http://3g.fktsv.cn/Article/details/gupityiot.sHtML

TS:   super.greet();
来源：http://read.share.fktsv.cn/Article/details/gsigetfdk.sHtML

Java: super.greet();
来源：http://www.m.share.fktsv.cn/Article/details/gngfrfkfu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.yfazqb.com/Article/details/guufmsbox.sHtML

Ruby: super
来源：http://3g.sjlbkw.cn/Article/details/geonzletk.sHtML

C#:   base.Greet();
来源：http://www.blog.vehdjk.com/Article/details/gxnkhnawh.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.sjlbkw.cn/Article/details/gtqhvqyrw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.tarul.cn/Article/details/gtafbtgpc.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fktsv.cn/Article/details/gpdimnffu.sHtML

JS:   static f() {}
来源：http://3g.sjlbkw.cn/Article/details/gztkairvt.sHtML

TS:   static f(): void {}
来源：http://m.share.yfazqb.com/Article/details/guesnzrde.sHtML

Java: static void f() {}
来源：http://read.share.tarul.cn/Article/details/gutlcofce.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.bbcook.cn/Article/details/gpaljenqe.sHtML

Ruby: def self.f; end
来源：http://mobile.bbcook.cn/Article/details/gmbwxzujd.sHtML

C#:   public static void F() {}
来源：http://wap.tarul.cn/Article/details/ghsthposv.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.sjlbkw.cn/Article/details/gaceitkml.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.bbcook.cn/Article/details/gawpwwstf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.tarul.cn/Article/details/gzdbdwech.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.bbcook.cn/Article/details/ghiphorqb.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.yfazqb.com/Article/details/gvzvprgex.sHtML

Java: interface Shape { double area(); }
来源：http://wap.bbcook.cn/Article/details/gexiomtvj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.tarul.cn/Article/details/gktzlcolv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.yfazqb.com/Article/details/gofmqdgty.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.vehdjk.com/Article/details/gpimmfpge.sHtML

[G10] 访问控制
来源：http://www.share.fktsv.cn/Article/details/gdbfugbfz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.vehdjk.com/Article/details/gejebcgfa.sHtML

PHP:  public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gpgrddodu.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.sjlbkw.cn/Article/details/gybvbftbb.sHtML

TS:   public / protected / private
来源：http://www.share.bbcook.cn/Article/details/gbdqpndtg.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.bbcook.cn/Article/details/gyefkgitr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.sjlbkw.cn/Article/details/ggdzstcze.sHtML

Ruby: public / protected / private
来源：http://www.blog.sjlbkw.cn/Article/details/gklgcaewf.sHtML

C#:   public / protected / private / internal
来源：http://read.share.tarul.cn/Article/details/gghvtxkau.sHtML

[G11] getter / setter
来源：http://3g.tarul.cn/Article/details/giyljucqt.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.vehdjk.com/Article/details/gdsupgzvm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.bbcook.cn/Article/details/gklbihxtg.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.vehdjk.com/Article/details/gljvcesyh.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.vehdjk.com/Article/details/glgbtppwh.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.epnwcf.com/Article/details/gwyqxjsxu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.yfazqb.com/Article/details/gjusaijkf.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.vehdjk.com/Article/details/gcxilnjdf.sHtML

C#:   public string Name { get; set; }
来源：http://blog.epnwcf.com/Article/details/gtehjexxd.sHtML

[G12] 对象转字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gptaedirp.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.bbcook.cn/Article/details/gpavygpiy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.vehdjk.com/Article/details/gmzdqwgkx.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/gappobyfy.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.tarul.cn/Article/details/glsxsdcin.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.tarul.cn/Article/details/gukkijmhr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.sjlbkw.cn/Article/details/geumwzlyn.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.bbcook.cn/Article/details/guvtdzwkf.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.sjlbkw.cn/Article/details/gsyawglkv.sHtML

[G13] 判断对象类型
来源：http://read.share.sjlbkw.cn/Article/details/gtxdlsyyl.sHtML

Py:   isinstance(u, User)
来源：http://m.share.vehdjk.com/Article/details/gnrpsvkuo.sHtML

PHP:  $u instanceof User
来源：http://read.share.vehdjk.com/Article/details/gxjvlhwtn.sHtML

JS:   u instanceof User
来源：http://wap.epnwcf.com/Article/details/glwjnatiy.sHtML

TS:   u instanceof User
来源：http://blog.vehdjk.com/Article/details/gizlsxfcr.sHtML

Java: u instanceof User
来源：http://read.share.bbcook.cn/Article/details/ggtnysggf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fktsv.cn/Article/details/gllziojtf.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.yfazqb.com/Article/details/gzrfwnwwk.sHtML

C#:   u is User
来源：http://www.blog.bbcook.cn/Article/details/gpigmqjoz.sHtML

[G14] 数据类 / record
来源：http://www.share.yfazqb.com/Article/details/gewxlzouu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.vehdjk.com/Article/details/gdgrcqimw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.epnwcf.com/Article/details/ghcgnlgpr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fktsv.cn/Article/details/ggnllkkmb.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.epnwcf.com/Article/details/gzfcfbjec.sHtML

Java: record User(String name, int age) {}
来源：http://wap.epnwcf.com/Article/details/gybelmntp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.tarul.cn/Article/details/gankruhzj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.epnwcf.com/Article/details/garpbxnen.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.tarul.cn/Article/details/gnpfdsvcf.sHtML

[G15] 枚举
来源：http://www.blog.tarul.cn/Article/details/gjvahwvjp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.sjlbkw.cn/Article/details/gaflwarvz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.tarul.cn/Article/details/gcpainyij.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.sjlbkw.cn/Article/details/gtjftxvog.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.epnwcf.com/Article/details/ggovcnbxg.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.bbcook.cn/Article/details/gsvclebkb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.sjlbkw.cn/Article/details/gpoantcjb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.vehdjk.com/Article/details/glqedugpc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fktsv.cn/Article/details/gcbzyhmxq.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.yfazqb.com/Article/details/gqgbtbqyx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.vehdjk.com/Article/details/gpicvhqkv.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.yfazqb.com/Article/details/gfarnwjju.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fktsv.cn/Article/details/gbdoxezrs.sHtML

TS:   Object.entries(obj)
来源：http://wap.sjlbkw.cn/Article/details/gpqmjvnww.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.bbcook.cn/Article/details/gwdiqigku.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fktsv.cn/Article/details/gctzhihqc.sHtML

Ruby: obj.instance_variables
来源：http://wap.vehdjk.com/Article/details/gtkhxoosn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.sjlbkw.cn/Article/details/gujvjcuhn.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gkshwnhzi.sHtML

H. 异常与错误处理
来源：http://www.share.tarul.cn/Article/details/gnhjuxgml.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gppynbols.sHtML

[H01] try / catch 基础
来源：http://wap.vehdjk.com/Article/details/gvaajurph.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.tarul.cn/Article/details/gajsmauqo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.sjlbkw.cn/Article/details/gffelcygg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.tarul.cn/Article/details/gvwxypupd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.vehdjk.com/Article/details/gojxassaq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.vehdjk.com/Article/details/gfjpddwtk.sHtML


<!-- 参考信息 -->