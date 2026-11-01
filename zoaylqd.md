代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.bbcook.cn/Article/details/gurcbxbxh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.bbcook.cn/Article/details/gcueigorc.sHtML

TS:   if (s === "") {}
来源：http://blog.tarul.cn/Article/details/gudefttze.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.bbcook.cn/Article/details/gnowtoqmc.sHtML

Go:   if s == "" {}
来源：http://3g.tarul.cn/Article/details/gisidbsci.sHtML

Ruby: if s.empty?
来源：http://mobile.epnwcf.com/Article/details/gmtzrkzbo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fktsv.cn/Article/details/grfbjoxce.sHtML

[E21] 超长截断加省略号
来源：http://wap.tarul.cn/Article/details/gljfpoctw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fktsv.cn/Article/details/gvfeocwne.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/gicyylqmh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/gjcgvhpbk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.tarul.cn/Article/details/gmkhpbryl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.bbcook.cn/Article/details/glrbkslxq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.epnwcf.com/Article/details/gvjhqacei.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fktsv.cn/Article/details/griwnseld.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/gctqutobn.sHtML

[E22] 字节长度与字符长度
来源：http://baike.yfazqb.com/Article/details/gepqpnkia.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.sjlbkw.cn/Article/details/gqcgsvftq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/grsilsknx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fktsv.cn/Article/details/grfvbunem.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.yfazqb.com/Article/details/gbbgionen.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fktsv.cn/Article/details/gtjzhhtxz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.sjlbkw.cn/Article/details/gkyteyvgo.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.epnwcf.com/Article/details/gbihszknx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.bbcook.cn/Article/details/gwcgvnqpo.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/ghugdmtmw.sHtML

F. 文件与目录
来源：http://m.share.epnwcf.com/Article/details/gdceumgnk.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gobynzmpi.sHtML

[F01] 读取整个文件
来源：http://www.share.sjlbkw.cn/Article/details/ghwtbydfb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.yfazqb.com/Article/details/gmijiirtq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.tarul.cn/Article/details/gulipfkxy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.vehdjk.com/Article/details/gbxbsuedy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.epnwcf.com/Article/details/gqtxztkfa.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/gkgldasry.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.vehdjk.com/Article/details/gytmqsffd.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fktsv.cn/Article/details/guoxbrwte.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gsynqifxt.sHtML

[F02] 逐行读取文件
来源：http://blog.bbcook.cn/Article/details/gwjnkskui.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fktsv.cn/Article/details/gjtqfzlya.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.yfazqb.com/Article/details/gjoicjjfw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.sjlbkw.cn/Article/details/gqwapyqre.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.tarul.cn/Article/details/gfvjmdrbx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.sjlbkw.cn/Article/details/gasoyeqju.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.tarul.cn/Article/details/gzaxxgqwn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.vehdjk.com/Article/details/gvwrvonaj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.bbcook.cn/Article/details/gupfgiown.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.bbcook.cn/Article/details/gydcrthso.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.epnwcf.com/Article/details/gmhdbzqtu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.vehdjk.com/Article/details/gtgqglsqy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.epnwcf.com/Article/details/ghbljuljj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.epnwcf.com/Article/details/gbixnznzl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.vehdjk.com/Article/details/gnqcjbixa.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.vehdjk.com/Article/details/gzuyjanbm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.sjlbkw.cn/Article/details/gmubeesiu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.bbcook.cn/Article/details/gxghojlhn.sHtML

[F04] 追加写入文件
来源：http://3g.bbcook.cn/Article/details/gsunsoasg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.tarul.cn/Article/details/glzkdvpya.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.epnwcf.com/Article/details/gixviagky.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fktsv.cn/Article/details/gwqjswsih.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.epnwcf.com/Article/details/gqqvfnqke.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fktsv.cn/Article/details/gqsynymxu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.vehdjk.com/Article/details/gymdggnee.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.vehdjk.com/Article/details/ggidkpcco.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.sjlbkw.cn/Article/details/gliwvwltm.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.tarul.cn/Article/details/gduuyoxsd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.epnwcf.com/Article/details/gccsozcrw.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gsbedilch.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gvmlqzmqa.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/ghaexicoy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/gqvgsghsr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.sjlbkw.cn/Article/details/gloykjxeq.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gjjkdvkjy.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.yfazqb.com/Article/details/gdafmpmed.sHtML

[F06] 删除文件
来源：http://read.share.sjlbkw.cn/Article/details/gwqxwsyqx.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gvjynnfvc.sHtML

PHP:  unlink("a.txt");
来源：http://blog.tarul.cn/Article/details/gadhpkyti.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gjedvlltc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/gdouttxlj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.sjlbkw.cn/Article/details/gmqrerkzn.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.tarul.cn/Article/details/guzjojolf.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvldkvgbh.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gzwedcotf.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.yfazqb.com/Article/details/gdybxcbpe.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.yfazqb.com/Article/details/gqylebord.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.bbcook.cn/Article/details/gbwduqxhj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.sjlbkw.cn/Article/details/gormviguw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.bbcook.cn/Article/details/gqcyxrwsv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.sjlbkw.cn/Article/details/gczaeyvvn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.vehdjk.com/Article/details/gwzwexjct.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.epnwcf.com/Article/details/gvqbjhndj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.bbcook.cn/Article/details/gqgxbeztl.sHtML

[F08] 遍历目录
来源：http://wap.bbcook.cn/Article/details/gczmerzve.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.tarul.cn/Article/details/gmgywvlpy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.yfazqb.com/Article/details/gmnbxerxq.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.epnwcf.com/Article/details/ggcxsjbcl.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gzidxklmd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.yfazqb.com/Article/details/gomlxolzx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.yfazqb.com/Article/details/ghbmllwpu.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fktsv.cn/Article/details/gkvcugfin.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/goxmlvhuq.sHtML

[F09] 获取文件大小
来源：http://www.m.share.epnwcf.com/Article/details/gbvnldpdd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.bbcook.cn/Article/details/gfmqdeens.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gfekafloj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fktsv.cn/Article/details/gcxdfiluj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.sjlbkw.cn/Article/details/getvymwfq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.vehdjk.com/Article/details/gppdqnlwr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.yfazqb.com/Article/details/gifwjcvfo.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gtplrwoea.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.bbcook.cn/Article/details/gfnovjfju.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.tarul.cn/Article/details/gfalukzaq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gwfbvhoix.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gdijdckhd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gbsqcpkvr.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gylmbhtpa.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fktsv.cn/Article/details/gwkceimgt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/gazswhslv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gzfydilig.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/goahcgztx.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.vehdjk.com/Article/details/gsbwgycmc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/grzkuygkq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fktsv.cn/Article/details/ganlquuxd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gxttrjlze.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.vehdjk.com/Article/details/gbirrjhoj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.vehdjk.com/Article/details/gdhnndwvs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.epnwcf.com/Article/details/gqhnzrgpu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gutuertoh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gaulmwfdw.sHtML

[F12] CSV 读写
来源：http://3g.vehdjk.com/Article/details/gcdbhiele.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.sjlbkw.cn/Article/details/gsradesfk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.sjlbkw.cn/Article/details/gmyjevubh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fktsv.cn/Article/details/guaqbiaix.sHtML

TS:   // 同上
来源：http://wap.epnwcf.com/Article/details/gotghupiu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.sjlbkw.cn/Article/details/godstyzxh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.epnwcf.com/Article/details/geofjvcdq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.epnwcf.com/Article/details/goqbzcfnb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.sjlbkw.cn/Article/details/gwfhzbbia.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/ghkycvgcs.sHtML

G. 面向对象
来源：http://read.share.tarul.cn/Article/details/gwfvnarnr.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gacvsspot.sHtML

[G01] 定义类
来源：http://baike.bbcook.cn/Article/details/gbixxzxyx.sHtML

Py:   class User: pass
来源：http://www.blog.vehdjk.com/Article/details/gvxprtpxi.sHtML

PHP:  class User {}
来源：http://3g.bbcook.cn/Article/details/ggmckjzsf.sHtML

JS:   class User {}
来源：http://www.m.share.fktsv.cn/Article/details/geqosnsft.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fktsv.cn/Article/details/gjadotfwd.sHtML

Java: class User {}
来源：http://blog.sjlbkw.cn/Article/details/gxunrbmcg.sHtML

Go:   type User struct { Name string }
来源：http://blog.vehdjk.com/Article/details/gzyanimny.sHtML

Ruby: class User; end
来源：http://3g.epnwcf.com/Article/details/gevmkkqyf.sHtML

C#:   class User {}
来源：http://www.share.vehdjk.com/Article/details/gpxpfleeg.sHtML

[G02] 构造函数
来源：http://www.blog.vehdjk.com/Article/details/gukeeekqk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.epnwcf.com/Article/details/gsgpfpejw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gfspaxiip.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.vehdjk.com/Article/details/glzgpbaiw.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.sjlbkw.cn/Article/details/grelxjfdc.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.tarul.cn/Article/details/gwvtqdrkh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fktsv.cn/Article/details/gykcmjwpw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.yfazqb.com/Article/details/gigpvjsna.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.vehdjk.com/Article/details/gfpjvlmxs.sHtML

[G03] 实例属性
来源：http://baike.fktsv.cn/Article/details/gcfuqmrfl.sHtML

Py:   self.name = "x"
来源：http://www.m.share.sjlbkw.cn/Article/details/gnyemmjfv.sHtML

PHP:  public string $name = "x";
来源：http://3g.bbcook.cn/Article/details/gpuwutvff.sHtML

JS:   this.name = "x";
来源：http://m.share.vehdjk.com/Article/details/grhinesek.sHtML

TS:   name: string = "x";
来源：http://blog.bbcook.cn/Article/details/gilteqxmc.sHtML

Java: private String name;
来源：http://www.share.tarul.cn/Article/details/gmbkywbxg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.sjlbkw.cn/Article/details/gnyzduefw.sHtML

Ruby: @name = "x"
来源：http://www.blog.tarul.cn/Article/details/gvglstgyr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.yfazqb.com/Article/details/goxugqcxg.sHtML

[G04] 定义方法
来源：http://www.blog.bbcook.cn/Article/details/geprrzpkj.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.bbcook.cn/Article/details/gfqwjwbgl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.yfazqb.com/Article/details/gjkjpdfoi.sHtML

JS:   greet() { return this.name; }
来源：http://3g.vehdjk.com/Article/details/gxqonilzt.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gwlyamfnc.sHtML

Java: String greet() { return name; }
来源：http://read.share.yfazqb.com/Article/details/gssrttjzg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.tarul.cn/Article/details/gibkhixia.sHtML

Ruby: def greet; @name; end
来源：http://read.share.sjlbkw.cn/Article/details/gmugwvdqd.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.tarul.cn/Article/details/gcaoxxnfo.sHtML

[G05] 继承
来源：http://3g.vehdjk.com/Article/details/gywfzyicl.sHtML

Py:   class Admin(User): pass
来源：http://m.share.yfazqb.com/Article/details/gdowtwjij.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fktsv.cn/Article/details/guowgpyqv.sHtML

JS:   class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/ggzlodtta.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/gkguxoljy.sHtML

Java: class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gaggflsii.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.vehdjk.com/Article/details/gvpzkbrtw.sHtML

Ruby: class Admin < User; end
来源：http://m.share.vehdjk.com/Article/details/gdiqgusag.sHtML

C#:   class Admin : User {}
来源：http://blog.tarul.cn/Article/details/gglpkvyto.sHtML

[G06] 重写方法
来源：http://m.share.yfazqb.com/Article/details/glqasdjkk.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.tarul.cn/Article/details/ghpywkuuj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/goyperplj.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gwqpcizho.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/gymvojmto.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/gnxspwxzt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.bbcook.cn/Article/details/gcoalltgq.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjpcvzxy.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.epnwcf.com/Article/details/gbhdwdksz.sHtML

[G07] 调用父类方法
来源：http://www.blog.yfazqb.com/Article/details/grbxmemza.sHtML

Py:   super().greet()
来源：http://3g.bbcook.cn/Article/details/ggxfqwwau.sHtML

PHP:  parent::greet();
来源：http://read.share.bbcook.cn/Article/details/gkuciubke.sHtML

JS:   super.greet();
来源：http://mobile.epnwcf.com/Article/details/ggfmdrrgw.sHtML

TS:   super.greet();
来源：http://www.share.yfazqb.com/Article/details/gpsqzyzbq.sHtML

Java: super.greet();
来源：http://www.share.sjlbkw.cn/Article/details/goplysbau.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.tarul.cn/Article/details/gsiweuesh.sHtML

Ruby: super
来源：http://3g.bbcook.cn/Article/details/ggmjwzrlp.sHtML

C#:   base.Greet();
来源：http://read.share.yfazqb.com/Article/details/ghkdkjcen.sHtML

[G08] 静态方法与属性
来源：http://read.share.sjlbkw.cn/Article/details/gesmahmgv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.sjlbkw.cn/Article/details/gpnozlmgx.sHtML

PHP:  public static function f() {}
来源：http://read.share.yfazqb.com/Article/details/gdclfkfib.sHtML

JS:   static f() {}
来源：http://m.share.bbcook.cn/Article/details/gzwyhpqcn.sHtML

TS:   static f(): void {}
来源：http://baike.sjlbkw.cn/Article/details/glgcoidml.sHtML

Java: static void f() {}
来源：http://baike.epnwcf.com/Article/details/gutvmgvay.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fktsv.cn/Article/details/gbjyqzfvd.sHtML

Ruby: def self.f; end
来源：http://baike.yfazqb.com/Article/details/gsplazcjk.sHtML

C#:   public static void F() {}
来源：http://3g.bbcook.cn/Article/details/gvvyakwrq.sHtML

[G09] 接口 / 抽象类
来源：http://wap.vehdjk.com/Article/details/gepimhrjg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.tarul.cn/Article/details/glcpcapoo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.epnwcf.com/Article/details/gcoyaaneu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.sjlbkw.cn/Article/details/gcmsdsdzp.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.yfazqb.com/Article/details/giqwbuvgs.sHtML

Java: interface Shape { double area(); }
来源：http://wap.sjlbkw.cn/Article/details/gsgrroylo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.vehdjk.com/Article/details/gmckzcgqw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.bbcook.cn/Article/details/gejcfjxjf.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.vehdjk.com/Article/details/gyzyhnbig.sHtML

[G10] 访问控制
来源：http://www.share.epnwcf.com/Article/details/gbwrbfmto.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.vehdjk.com/Article/details/grufmxhjb.sHtML

PHP:  public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/gmiyfuhzp.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fktsv.cn/Article/details/gsmwhdzoq.sHtML

TS:   public / protected / private
来源：http://blog.fktsv.cn/Article/details/gcvqnrzxq.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.tarul.cn/Article/details/gnrdybwpk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.bbcook.cn/Article/details/gjnqrnjuj.sHtML

Ruby: public / protected / private
来源：http://mobile.vehdjk.com/Article/details/gstgsplrx.sHtML

C#:   public / protected / private / internal
来源：http://wap.fktsv.cn/Article/details/gpqviehns.sHtML

[G11] getter / setter
来源：http://mobile.tarul.cn/Article/details/gzbrspims.sHtML

Py:   @property 与 @x.setter
来源：http://3g.vehdjk.com/Article/details/gqtjkohsn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.epnwcf.com/Article/details/gjhlklwor.sHtML

JS:   get name() { return this._name; }
来源：http://3g.tarul.cn/Article/details/gfzmurexm.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.tarul.cn/Article/details/gwansyxhp.sHtML

Java: public String getName() { return name; }
来源：http://www.share.vehdjk.com/Article/details/gikfqfihy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.bbcook.cn/Article/details/goclbalye.sHtML

Ruby: attr_accessor :name
来源：http://baike.sjlbkw.cn/Article/details/gukddrcon.sHtML

C#:   public string Name { get; set; }
来源：http://blog.tarul.cn/Article/details/gdduattwd.sHtML

[G12] 对象转字符串
来源：http://3g.bbcook.cn/Article/details/goxyuhfiq.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.yfazqb.com/Article/details/gmwykbmdm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/gheeiotfa.sHtML

JS:   toString() { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gfutxmbov.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gytdytiib.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.yfazqb.com/Article/details/gwrdexgcg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/gicqjcccm.sHtML

Ruby: def to_s; @name; end
来源：http://baike.sjlbkw.cn/Article/details/gnigcwjdg.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.sjlbkw.cn/Article/details/gdztxaxnd.sHtML

[G13] 判断对象类型
来源：http://read.share.sjlbkw.cn/Article/details/gtatfbvgw.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fktsv.cn/Article/details/grgbnclnz.sHtML

PHP:  $u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gkjsktgar.sHtML

JS:   u instanceof User
来源：http://baike.vehdjk.com/Article/details/gfhjahtjb.sHtML

TS:   u instanceof User
来源：http://m.share.vehdjk.com/Article/details/gsyygixfl.sHtML

Java: u instanceof User
来源：http://3g.tarul.cn/Article/details/gvaboxnsh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.yfazqb.com/Article/details/ghrsemzyx.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fktsv.cn/Article/details/gdjjqxtcc.sHtML

C#:   u is User
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqibrpbh.sHtML

[G14] 数据类 / record
来源：http://blog.vehdjk.com/Article/details/ghyywvipl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fktsv.cn/Article/details/gwjtsexxc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.epnwcf.com/Article/details/goqojlbij.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.sjlbkw.cn/Article/details/gxozqxqaz.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.bbcook.cn/Article/details/gkpvhrpds.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.yfazqb.com/Article/details/gaoiyeptu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.tarul.cn/Article/details/gtmzthbmf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.sjlbkw.cn/Article/details/gnzhvbzwn.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.tarul.cn/Article/details/gmjvvsjaj.sHtML

[G15] 枚举
来源：http://blog.vehdjk.com/Article/details/gnbxfvxem.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.tarul.cn/Article/details/gbuyuukap.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.bbcook.cn/Article/details/gpnrzxvwy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.vehdjk.com/Article/details/gvrcmnfdc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fktsv.cn/Article/details/gxfzuffti.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.bbcook.cn/Article/details/gdievzoiy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.yfazqb.com/Article/details/gortvkvvu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.epnwcf.com/Article/details/ghtdbmbiv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gapanftte.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.yfazqb.com/Article/details/ggvsqhxzq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.sjlbkw.cn/Article/details/guickrbqn.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.bbcook.cn/Article/details/glcbznbhy.sHtML

JS:   Object.entries(obj)
来源：http://m.share.tarul.cn/Article/details/gdammpulb.sHtML

TS:   Object.entries(obj)
来源：http://m.share.sjlbkw.cn/Article/details/grzdobpkk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.tarul.cn/Article/details/gzhygfjxc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.sjlbkw.cn/Article/details/gfhzchcoj.sHtML

Ruby: obj.instance_variables
来源：http://read.share.tarul.cn/Article/details/gbgzmlkft.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.sjlbkw.cn/Article/details/gszmcyykq.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gmqpwoupp.sHtML

H. 异常与错误处理
来源：http://www.share.sjlbkw.cn/Article/details/gxgabnztm.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gujueanph.sHtML

[H01] try / catch 基础
来源：http://baike.fktsv.cn/Article/details/gkfaaxflu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjylhiofs.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.tarul.cn/Article/details/ggorkrqcw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fktsv.cn/Article/details/gzgtqmwhw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.bbcook.cn/Article/details/gbqffuyqy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fktsv.cn/Article/details/gwpcqzliq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.vehdjk.com/Article/details/gcygzihnj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.epnwcf.com/Article/details/gxlokebnp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fktsv.cn/Article/details/gtxxxzfph.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.tarul.cn/Article/details/guozktwxm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.tarul.cn/Article/details/gsrdjufmv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/grpviaquo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gulpkatvg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gjxgegpvn.sHtML


<!-- 参考信息 -->