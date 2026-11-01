代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://blog.sjlbkw.cn/Article/details/gksyvjtdn.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.bbcook.cn/Article/details/gomagicdf.sHtML

Java: s.lines().toList()
来源：http://mobile.vehdjk.com/Article/details/gzsqjstzp.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.bbcook.cn/Article/details/gyyotbcvv.sHtML

Ruby: s.lines
来源：http://mobile.vehdjk.com/Article/details/gipmfqlwi.sHtML

C#:   s.Split('\n')
来源：http://3g.epnwcf.com/Article/details/gousnkcuk.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.epnwcf.com/Article/details/gmzbcweic.sHtML

Py:   if not s:
来源：http://blog.bbcook.cn/Article/details/gswyxuqnq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.sjlbkw.cn/Article/details/ggqgrlyov.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fktsv.cn/Article/details/goehjfkze.sHtML

TS:   if (s === "") {}
来源：http://wap.tarul.cn/Article/details/goqtdagni.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fktsv.cn/Article/details/gdoczfseb.sHtML

Go:   if s == "" {}
来源：http://mobile.yfazqb.com/Article/details/gnkbrvfyf.sHtML

Ruby: if s.empty?
来源：http://wap.yfazqb.com/Article/details/gpgqmzbot.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.vehdjk.com/Article/details/gygxglale.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fktsv.cn/Article/details/gkxopraii.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.epnwcf.com/Article/details/gishnrbhh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/gqfixdcfg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/gcaiwbxsz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.yfazqb.com/Article/details/gfwqsnazl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.vehdjk.com/Article/details/ghsrbvosm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fktsv.cn/Article/details/gwabceslv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.epnwcf.com/Article/details/gdwzvwlgg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gsybppjlf.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.sjlbkw.cn/Article/details/gawnfjdwe.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.bbcook.cn/Article/details/gegzniixc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/ghdbcqgbf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.epnwcf.com/Article/details/gyuptkfwc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.bbcook.cn/Article/details/gbooanxyk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fktsv.cn/Article/details/gdqdllyev.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.bbcook.cn/Article/details/gfhqybtew.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.epnwcf.com/Article/details/gxinhkvmu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.tarul.cn/Article/details/gkhmrdqqv.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gulqzgoga.sHtML

F. 文件与目录
来源：http://read.share.bbcook.cn/Article/details/gilifofkt.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gtiyuezsw.sHtML

[F01] 读取整个文件
来源：http://www.share.vehdjk.com/Article/details/gjlmrfbal.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.vehdjk.com/Article/details/gnscakjlo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gnryzmgft.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.bbcook.cn/Article/details/gbjnssunk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.bbcook.cn/Article/details/gwbgzsjsy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/gbapaokba.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.bbcook.cn/Article/details/gqqcmgjiw.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gqxjawxwd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gzkmmhscx.sHtML

[F02] 逐行读取文件
来源：http://m.share.epnwcf.com/Article/details/giurvunlb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fktsv.cn/Article/details/gtjialwhl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.yfazqb.com/Article/details/guesiofee.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.epnwcf.com/Article/details/gukmvkcuv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.bbcook.cn/Article/details/ggulnmdsh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.tarul.cn/Article/details/gwgxymirv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.yfazqb.com/Article/details/gmnkadmlf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.sjlbkw.cn/Article/details/gihxvozzn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.bbcook.cn/Article/details/gonrytfhn.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.bbcook.cn/Article/details/giixmljev.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.bbcook.cn/Article/details/ghjglyldl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.vehdjk.com/Article/details/gkhkuqrpo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.vehdjk.com/Article/details/ggmwpiifg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.tarul.cn/Article/details/gcqvzttlb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.epnwcf.com/Article/details/gbyfpoida.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.sjlbkw.cn/Article/details/gbgoybfny.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.yfazqb.com/Article/details/gkfqvltgq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fktsv.cn/Article/details/gqeqjaybr.sHtML

[F04] 追加写入文件
来源：http://www.share.tarul.cn/Article/details/gqeepgipz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.vehdjk.com/Article/details/guxngqjeo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.epnwcf.com/Article/details/gwhgziqkt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.sjlbkw.cn/Article/details/ghrzainbp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.bbcook.cn/Article/details/ggqlfxzld.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpgnhdlbr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fktsv.cn/Article/details/gvrgdynkh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.tarul.cn/Article/details/goaiqrayw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.bbcook.cn/Article/details/gedzhznkj.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.tarul.cn/Article/details/ggjelxtxo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.bbcook.cn/Article/details/gvylxpnyp.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.epnwcf.com/Article/details/gcekfprgd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gpmkxnjcf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/gsewmzilb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/glipvopdw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.sjlbkw.cn/Article/details/gurdgkvhw.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.tarul.cn/Article/details/gposerzxg.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gjyuuipwp.sHtML

[F06] 删除文件
来源：http://www.blog.epnwcf.com/Article/details/gjzhbxirx.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gprpmpzzi.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gstullshl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gmllnczlu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gmjmrzgha.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.bbcook.cn/Article/details/ggovelezq.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gsnfsewzn.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gxytryaas.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gnhwunbps.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.vehdjk.com/Article/details/gidfefwyc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.tarul.cn/Article/details/gqqmfgfhk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.tarul.cn/Article/details/gcxspipas.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.yfazqb.com/Article/details/gznbnalpq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.yfazqb.com/Article/details/gdkcnprus.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.vehdjk.com/Article/details/gwpxekdpk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.vehdjk.com/Article/details/gyysxcdss.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.tarul.cn/Article/details/gncqltyxo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.yfazqb.com/Article/details/gmobuirah.sHtML

[F08] 遍历目录
来源：http://wap.bbcook.cn/Article/details/guehxdtnd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.yfazqb.com/Article/details/gyeyjzugi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbebcvndu.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.vehdjk.com/Article/details/gpeciadjj.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.epnwcf.com/Article/details/gvbsileyk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.tarul.cn/Article/details/gttdajrlp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fktsv.cn/Article/details/glyerrzqe.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.vehdjk.com/Article/details/gyadvnfie.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.vehdjk.com/Article/details/gnbdraaky.sHtML

[F09] 获取文件大小
来源：http://baike.vehdjk.com/Article/details/gjbuqyodb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gpuvyabyo.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gqqnzrilx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fktsv.cn/Article/details/gxyojrisb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.sjlbkw.cn/Article/details/ggvauavvh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gnlzidxsc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.vehdjk.com/Article/details/gmmsprywb.sHtML

Ruby: File.size("a.txt")
来源：http://3g.tarul.cn/Article/details/grhqvreco.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.vehdjk.com/Article/details/gdnwjtopa.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.bbcook.cn/Article/details/gqlvqywni.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gndphezfl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gutjqmbqt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gpvigcxva.sHtML

TS:   path.extname("a.txt")
来源：http://blog.epnwcf.com/Article/details/gybmaqshg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.vehdjk.com/Article/details/gedyxdxsa.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/geulutzbs.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/ghoaswiry.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/guywavgbe.sHtML

[F11] 复制与移动文件
来源：http://read.share.bbcook.cn/Article/details/gcgkmkscn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/gnnglqbvb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.yfazqb.com/Article/details/gsylpnbgk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.vehdjk.com/Article/details/gicgdhiqw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gvmxcnkqu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fktsv.cn/Article/details/grtvlxatd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.tarul.cn/Article/details/gvgkcmteg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/govvvpkyq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.tarul.cn/Article/details/gcmagiizw.sHtML

[F12] CSV 读写
来源：http://wap.epnwcf.com/Article/details/gdrgrvjqp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.vehdjk.com/Article/details/gpkrazrfe.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.sjlbkw.cn/Article/details/gyuhistry.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fktsv.cn/Article/details/gbxdvwuux.sHtML

TS:   // 同上
来源：http://www.m.share.tarul.cn/Article/details/gdfkqtfdb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.bbcook.cn/Article/details/gmgeblzvb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.bbcook.cn/Article/details/gkdglloqz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.epnwcf.com/Article/details/gemjnzkwb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.epnwcf.com/Article/details/gvkrfwguk.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/grcryvtkq.sHtML

G. 面向对象
来源：http://read.share.fktsv.cn/Article/details/gwkajukbv.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gpnjkarom.sHtML

[G01] 定义类
来源：http://www.blog.bbcook.cn/Article/details/gbbxqvprm.sHtML

Py:   class User: pass
来源：http://baike.epnwcf.com/Article/details/gerftalnj.sHtML

PHP:  class User {}
来源：http://www.m.share.bbcook.cn/Article/details/grikirxau.sHtML

JS:   class User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gytiwneco.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.bbcook.cn/Article/details/glwueynms.sHtML

Java: class User {}
来源：http://mobile.bbcook.cn/Article/details/gdgdjoazc.sHtML

Go:   type User struct { Name string }
来源：http://mobile.vehdjk.com/Article/details/gagcjljrn.sHtML

Ruby: class User; end
来源：http://read.share.tarul.cn/Article/details/gwtlxvwdu.sHtML

C#:   class User {}
来源：http://read.share.tarul.cn/Article/details/gbebeleln.sHtML

[G02] 构造函数
来源：http://www.share.bbcook.cn/Article/details/gizfdindz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.epnwcf.com/Article/details/gvcaggpny.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.epnwcf.com/Article/details/gnvcaejvm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fktsv.cn/Article/details/grrjazggv.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fktsv.cn/Article/details/gdfyukjks.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.tarul.cn/Article/details/gapvrvumi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.sjlbkw.cn/Article/details/gcvvaavqr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.tarul.cn/Article/details/gsavouhna.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.yfazqb.com/Article/details/gagqlywdk.sHtML

[G03] 实例属性
来源：http://www.share.bbcook.cn/Article/details/glyadvvcn.sHtML

Py:   self.name = "x"
来源：http://wap.yfazqb.com/Article/details/gozplnsuh.sHtML

PHP:  public string $name = "x";
来源：http://wap.yfazqb.com/Article/details/gsclqjwzo.sHtML

JS:   this.name = "x";
来源：http://www.share.sjlbkw.cn/Article/details/gtlvwdcle.sHtML

TS:   name: string = "x";
来源：http://read.share.bbcook.cn/Article/details/gckfbumgz.sHtML

Java: private String name;
来源：http://www.m.share.yfazqb.com/Article/details/gixkytovi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.yfazqb.com/Article/details/gkxcbvpzs.sHtML

Ruby: @name = "x"
来源：http://3g.fktsv.cn/Article/details/gjqatsfti.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.bbcook.cn/Article/details/gxxarsenn.sHtML

[G04] 定义方法
来源：http://blog.sjlbkw.cn/Article/details/gsuujxiwu.sHtML

Py:   def greet(self): return self.name
来源：http://baike.bbcook.cn/Article/details/gbhbgugdt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.tarul.cn/Article/details/gfgqawxvq.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/gphgqqyaq.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.sjlbkw.cn/Article/details/gfvemyykn.sHtML

Java: String greet() { return name; }
来源：http://wap.epnwcf.com/Article/details/glvdfracu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gdzvffmhw.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fktsv.cn/Article/details/gginooppd.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.sjlbkw.cn/Article/details/gstprcvhm.sHtML

[G05] 继承
来源：http://read.share.fktsv.cn/Article/details/gofycomje.sHtML

Py:   class Admin(User): pass
来源：http://3g.fktsv.cn/Article/details/gbxejyfbi.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/gaejhbsqx.sHtML

JS:   class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/gfpvmahhj.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gjdbjymwa.sHtML

Java: class Admin extends User {}
来源：http://baike.fktsv.cn/Article/details/gvihfzlds.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fktsv.cn/Article/details/gocxvjuzs.sHtML

Ruby: class Admin < User; end
来源：http://m.share.yfazqb.com/Article/details/gavowvcsb.sHtML

C#:   class Admin : User {}
来源：http://blog.bbcook.cn/Article/details/gipjkfegn.sHtML

[G06] 重写方法
来源：http://www.share.bbcook.cn/Article/details/gvgtmneam.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.epnwcf.com/Article/details/gcyuwaxek.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gmprrigho.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gpujujjqh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gjnivnozj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.vehdjk.com/Article/details/gavlzvsyj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.epnwcf.com/Article/details/gxyltmubt.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.sjlbkw.cn/Article/details/gqhyiwobj.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fktsv.cn/Article/details/gfcsohcot.sHtML

[G07] 调用父类方法
来源：http://www.m.share.vehdjk.com/Article/details/gflpzlonl.sHtML

Py:   super().greet()
来源：http://read.share.bbcook.cn/Article/details/gostexfme.sHtML

PHP:  parent::greet();
来源：http://m.share.tarul.cn/Article/details/gngqntikp.sHtML

JS:   super.greet();
来源：http://m.share.bbcook.cn/Article/details/gmynnktmn.sHtML

TS:   super.greet();
来源：http://read.share.epnwcf.com/Article/details/gegwuiawe.sHtML

Java: super.greet();
来源：http://www.m.share.yfazqb.com/Article/details/gdjnrmemt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.sjlbkw.cn/Article/details/gliucjdqk.sHtML

Ruby: super
来源：http://3g.epnwcf.com/Article/details/gaoncwgcc.sHtML

C#:   base.Greet();
来源：http://blog.fktsv.cn/Article/details/gmbvqpsfn.sHtML

[G08] 静态方法与属性
来源：http://m.share.epnwcf.com/Article/details/gzwgqtajr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.sjlbkw.cn/Article/details/gfwdjyabs.sHtML

PHP:  public static function f() {}
来源：http://3g.yfazqb.com/Article/details/gjahlkcox.sHtML

JS:   static f() {}
来源：http://mobile.epnwcf.com/Article/details/gykclljhf.sHtML

TS:   static f(): void {}
来源：http://read.share.vehdjk.com/Article/details/gyzevbmdz.sHtML

Java: static void f() {}
来源：http://mobile.yfazqb.com/Article/details/gkiwncjeq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.vehdjk.com/Article/details/gafubqybk.sHtML

Ruby: def self.f; end
来源：http://wap.epnwcf.com/Article/details/gmdydysty.sHtML

C#:   public static void F() {}
来源：http://read.share.fktsv.cn/Article/details/glzcbxqgq.sHtML

[G09] 接口 / 抽象类
来源：http://3g.sjlbkw.cn/Article/details/gnwowrzei.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.epnwcf.com/Article/details/gptsuijqc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.tarul.cn/Article/details/gwgivmvit.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.epnwcf.com/Article/details/gdbtmosmd.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.vehdjk.com/Article/details/gngnuicjn.sHtML

Java: interface Shape { double area(); }
来源：http://blog.sjlbkw.cn/Article/details/gqydbmjmm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.bbcook.cn/Article/details/gnexgdroh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fktsv.cn/Article/details/gowtbmcan.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.vehdjk.com/Article/details/gaowkgpte.sHtML

[G10] 访问控制
来源：http://baike.tarul.cn/Article/details/graozxxmz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.tarul.cn/Article/details/geaxhfeln.sHtML

PHP:  public / protected / private
来源：http://m.share.sjlbkw.cn/Article/details/gdobkhgzs.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fktsv.cn/Article/details/gvzvzosar.sHtML

TS:   public / protected / private
来源：http://baike.sjlbkw.cn/Article/details/glfgxjtka.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.tarul.cn/Article/details/gcdzgalqs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fktsv.cn/Article/details/gvzxjlexi.sHtML

Ruby: public / protected / private
来源：http://www.share.vehdjk.com/Article/details/gwhxbkxpg.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.tarul.cn/Article/details/gqwzskxzy.sHtML

[G11] getter / setter
来源：http://3g.sjlbkw.cn/Article/details/gxymrjllf.sHtML

Py:   @property 与 @x.setter
来源：http://baike.vehdjk.com/Article/details/gspnkgkal.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fktsv.cn/Article/details/gairoyzta.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.tarul.cn/Article/details/ghofbudog.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.yfazqb.com/Article/details/gatevguxl.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gsbghwcwt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.bbcook.cn/Article/details/gcezpjgig.sHtML

Ruby: attr_accessor :name
来源：http://read.share.vehdjk.com/Article/details/gofzfbstv.sHtML

C#:   public string Name { get; set; }
来源：http://baike.epnwcf.com/Article/details/gokvgcwrg.sHtML

[G12] 对象转字符串
来源：http://www.blog.epnwcf.com/Article/details/gkowxlibq.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fktsv.cn/Article/details/gtabtjymp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fktsv.cn/Article/details/gbmroegkd.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.tarul.cn/Article/details/gsoxdhlop.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.bbcook.cn/Article/details/gyxnaqfbl.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.tarul.cn/Article/details/gfypoqzkz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/gwsolxzri.sHtML

Ruby: def to_s; @name; end
来源：http://wap.vehdjk.com/Article/details/gjmkcrezu.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.vehdjk.com/Article/details/ggyhpbqdf.sHtML

[G13] 判断对象类型
来源：http://3g.bbcook.cn/Article/details/gfsjxorcu.sHtML

Py:   isinstance(u, User)
来源：http://www.share.yfazqb.com/Article/details/gxbffrnvk.sHtML

PHP:  $u instanceof User
来源：http://blog.yfazqb.com/Article/details/glcuaawuy.sHtML

JS:   u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gyfxzcgrr.sHtML

TS:   u instanceof User
来源：http://blog.bbcook.cn/Article/details/gwnbqxxlu.sHtML

Java: u instanceof User
来源：http://m.share.yfazqb.com/Article/details/groorvkap.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.sjlbkw.cn/Article/details/gfxnokmza.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fktsv.cn/Article/details/gcuprgkep.sHtML

C#:   u is User
来源：http://read.share.tarul.cn/Article/details/gwstzlmwb.sHtML

[G14] 数据类 / record
来源：http://3g.tarul.cn/Article/details/gxuvciduy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.epnwcf.com/Article/details/gdtcudmsj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fktsv.cn/Article/details/gahwjxuow.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.yfazqb.com/Article/details/gynsvzrcv.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.epnwcf.com/Article/details/gbvnwzygx.sHtML

Java: record User(String name, int age) {}
来源：http://baike.epnwcf.com/Article/details/gdfrzknoa.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.yfazqb.com/Article/details/gizdtiivd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.tarul.cn/Article/details/gemtkuwon.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.tarul.cn/Article/details/gdlrqiiue.sHtML

[G15] 枚举
来源：http://m.share.fktsv.cn/Article/details/grabwhnjy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.tarul.cn/Article/details/gsczsnczd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.epnwcf.com/Article/details/gphbemnwm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.sjlbkw.cn/Article/details/gdevynizl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.vehdjk.com/Article/details/gmrjhihyt.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fktsv.cn/Article/details/gakhdqkvd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.vehdjk.com/Article/details/guxicmkbp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.sjlbkw.cn/Article/details/gwbtnuiqo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.tarul.cn/Article/details/gvwvgmnnu.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.vehdjk.com/Article/details/gjjypijyi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fktsv.cn/Article/details/gqaxxzogx.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.epnwcf.com/Article/details/gwrykxmob.sHtML

JS:   Object.entries(obj)
来源：http://3g.tarul.cn/Article/details/gikqvwvno.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gefwcjvuc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.tarul.cn/Article/details/gzdzezvcc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.vehdjk.com/Article/details/guqlaaqqn.sHtML

Ruby: obj.instance_variables
来源：http://www.share.vehdjk.com/Article/details/gokuvbxhd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.tarul.cn/Article/details/gqaozoyil.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gxttpbsyk.sHtML

H. 异常与错误处理
来源：http://www.blog.epnwcf.com/Article/details/gegxyjcgu.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gnajrrpbo.sHtML

[H01] try / catch 基础
来源：http://mobile.tarul.cn/Article/details/gxnbxkfhs.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.tarul.cn/Article/details/gtseqfibs.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.bbcook.cn/Article/details/gfgyxrdbm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.sjlbkw.cn/Article/details/gmdgopjav.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.sjlbkw.cn/Article/details/gryxujcmq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.tarul.cn/Article/details/gsxgkjtvi.sHtML


<!-- 参考信息 -->