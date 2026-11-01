代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fktsv.cn/Article/details/gilrnnwfh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.vehdjk.com/Article/details/ggwavouns.sHtML

TS:   if (s === "") {}
来源：http://wap.epnwcf.com/Article/details/gwjinnzyu.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fktsv.cn/Article/details/gyhdyhdiq.sHtML

Go:   if s == "" {}
来源：http://3g.epnwcf.com/Article/details/gduuxdnwv.sHtML

Ruby: if s.empty?
来源：http://wap.bbcook.cn/Article/details/gekbkclng.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fktsv.cn/Article/details/ghpxwviez.sHtML

[E21] 超长截断加省略号
来源：http://blog.fktsv.cn/Article/details/gotcznony.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fktsv.cn/Article/details/gaadxuoai.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.vehdjk.com/Article/details/gdofbtzlt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.bbcook.cn/Article/details/gzinwigbo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fktsv.cn/Article/details/gmkynwhzo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gnagjdxlj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.sjlbkw.cn/Article/details/gxazhajih.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/gczbsynfx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gvtxtcufc.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.epnwcf.com/Article/details/gbxmnpyhw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.sjlbkw.cn/Article/details/gcqzpivhh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/glxkjhnwe.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.bbcook.cn/Article/details/gqvrqqrgb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.sjlbkw.cn/Article/details/ghjihmlsy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.epnwcf.com/Article/details/gtmeryizs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fktsv.cn/Article/details/gqefxuqwk.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fktsv.cn/Article/details/gwdndmtzo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.tarul.cn/Article/details/gzaurtazf.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gsmsmgyzo.sHtML

F. 文件与目录
来源：http://www.m.share.yfazqb.com/Article/details/gueggcaem.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gybbutqaw.sHtML

[F01] 读取整个文件
来源：http://mobile.tarul.cn/Article/details/gfbrdkexe.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.sjlbkw.cn/Article/details/ggsrirlbn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gmzwtzuet.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.epnwcf.com/Article/details/glumxtshj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.tarul.cn/Article/details/gzrjepdum.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/gsyrffcey.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.bbcook.cn/Article/details/ghrfenjky.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/goiaffxzx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.epnwcf.com/Article/details/galkoxiqz.sHtML

[F02] 逐行读取文件
来源：http://www.share.bbcook.cn/Article/details/gbhnakvhq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.tarul.cn/Article/details/ghjfdqife.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.yfazqb.com/Article/details/gfjzkmpte.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fktsv.cn/Article/details/gnonuuqaa.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fktsv.cn/Article/details/gxececdlc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.sjlbkw.cn/Article/details/gxrdmelbi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fktsv.cn/Article/details/gvvixolka.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.vehdjk.com/Article/details/gkptrulzy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqntqtabd.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.epnwcf.com/Article/details/gjenvtasx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.epnwcf.com/Article/details/gfpklircy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.sjlbkw.cn/Article/details/gyhbrqfee.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.yfazqb.com/Article/details/gylffhrmp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fktsv.cn/Article/details/gzoavpkzu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fktsv.cn/Article/details/glhtwvnyx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.vehdjk.com/Article/details/gcfdhvuni.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.tarul.cn/Article/details/gocoaxnjq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.tarul.cn/Article/details/glpukoqaw.sHtML

[F04] 追加写入文件
来源：http://blog.epnwcf.com/Article/details/gggttysqb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.yfazqb.com/Article/details/gtkujlalv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.sjlbkw.cn/Article/details/gafzbkior.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.yfazqb.com/Article/details/gonlhkpte.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fktsv.cn/Article/details/gkusuidwf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.tarul.cn/Article/details/gtmitrqdd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fktsv.cn/Article/details/gjjduakzm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.epnwcf.com/Article/details/gmkmoomxj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fktsv.cn/Article/details/gdxxiwnvl.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.bbcook.cn/Article/details/ghssxsbfi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.bbcook.cn/Article/details/gytgoqiiw.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gjcjrlonh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gwdsciveh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/gmhdzfldq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/gmesofzhr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.vehdjk.com/Article/details/grypcqvuj.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gtqqbczza.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.tarul.cn/Article/details/gdjkqznhz.sHtML

[F06] 删除文件
来源：http://www.blog.vehdjk.com/Article/details/gjobypref.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fktsv.cn/Article/details/ghheybqti.sHtML

PHP:  unlink("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/grdbcujgt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.vehdjk.com/Article/details/gqdbtfudl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gieiygvrj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/glfkxptri.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.epnwcf.com/Article/details/gmfuvfhjb.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gajasqkoz.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gnzpnabfx.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.yfazqb.com/Article/details/gmhdnlmny.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.tarul.cn/Article/details/gfidrtmjm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.epnwcf.com/Article/details/gbxwbzzyd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.epnwcf.com/Article/details/grbqbwgkm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.epnwcf.com/Article/details/gpgmwcriv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.epnwcf.com/Article/details/gzawufdon.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.yfazqb.com/Article/details/gsgamgxsh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.bbcook.cn/Article/details/granpcmhz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.vehdjk.com/Article/details/gnipjoecl.sHtML

[F08] 遍历目录
来源：http://3g.sjlbkw.cn/Article/details/gmgaadvhj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.epnwcf.com/Article/details/gteomgvad.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.tarul.cn/Article/details/gjfzhvfnz.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.yfazqb.com/Article/details/glzrzeybw.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.bbcook.cn/Article/details/gpfaajqrp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fktsv.cn/Article/details/gdbczejyc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.bbcook.cn/Article/details/ghvvclilg.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fktsv.cn/Article/details/gipozhwwb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gtmbmgjmb.sHtML

[F09] 获取文件大小
来源：http://mobile.yfazqb.com/Article/details/gxgtjclrc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/grtfdwlty.sHtML

PHP:  filesize("a.txt");
来源：http://blog.yfazqb.com/Article/details/ggxmmqxfn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.bbcook.cn/Article/details/ghhlfhnmj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.epnwcf.com/Article/details/gkrpwsrsi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.bbcook.cn/Article/details/gnpjtbrya.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.bbcook.cn/Article/details/gbrsghrha.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gqwmqgfyp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.tarul.cn/Article/details/gftmalkqf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.sjlbkw.cn/Article/details/geizzajsf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gtkfejwbw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.epnwcf.com/Article/details/gshseftkp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gsdvhwyqm.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gqtmagboe.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.bbcook.cn/Article/details/gsudreqga.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/glpeaiaum.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gislvnbfk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/gqqopohgi.sHtML

[F11] 复制与移动文件
来源：http://baike.sjlbkw.cn/Article/details/grdlqjerq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gtpuwsedx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.epnwcf.com/Article/details/gclyzptvr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/gejsvpjqk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/gqndjpcoe.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.tarul.cn/Article/details/gxhiqlwby.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fktsv.cn/Article/details/gwcwdtqke.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gcedhbwcx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.bbcook.cn/Article/details/gmgzikhrt.sHtML

[F12] CSV 读写
来源：http://www.share.bbcook.cn/Article/details/gfrsbvvde.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.vehdjk.com/Article/details/grtchojmv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fktsv.cn/Article/details/gjkoifckb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.vehdjk.com/Article/details/gyeeafcir.sHtML

TS:   // 同上
来源：http://www.blog.fktsv.cn/Article/details/gqapxycxk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fktsv.cn/Article/details/gzjppyscz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.tarul.cn/Article/details/gqbensvif.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.yfazqb.com/Article/details/gmhoorwhu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.sjlbkw.cn/Article/details/gvstlfssd.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gykkkxifi.sHtML

G. 面向对象
来源：http://www.m.share.vehdjk.com/Article/details/geixmkkmz.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gobevpwzo.sHtML

[G01] 定义类
来源：http://read.share.epnwcf.com/Article/details/gvjkbxxqf.sHtML

Py:   class User: pass
来源：http://www.m.share.bbcook.cn/Article/details/gllbnojot.sHtML

PHP:  class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gyzdeqnpk.sHtML

JS:   class User {}
来源：http://wap.vehdjk.com/Article/details/gpzklehjy.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.vehdjk.com/Article/details/gdjtunhvz.sHtML

Java: class User {}
来源：http://baike.tarul.cn/Article/details/gvthhgsng.sHtML

Go:   type User struct { Name string }
来源：http://mobile.bbcook.cn/Article/details/gsfmjjgvq.sHtML

Ruby: class User; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gngkxmvft.sHtML

C#:   class User {}
来源：http://www.share.tarul.cn/Article/details/gobjlkjge.sHtML

[G02] 构造函数
来源：http://wap.fktsv.cn/Article/details/geirydrjz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.tarul.cn/Article/details/gaxqcetij.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.sjlbkw.cn/Article/details/ghtqirfzp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.tarul.cn/Article/details/gwwmcoxoe.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fktsv.cn/Article/details/gexpaayfq.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.yfazqb.com/Article/details/grfpxkugr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.vehdjk.com/Article/details/gaewhtyja.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.epnwcf.com/Article/details/gmbuztyua.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fktsv.cn/Article/details/gbayscopa.sHtML

[G03] 实例属性
来源：http://www.share.vehdjk.com/Article/details/gueertdjm.sHtML

Py:   self.name = "x"
来源：http://www.m.share.bbcook.cn/Article/details/gueykbqup.sHtML

PHP:  public string $name = "x";
来源：http://www.share.vehdjk.com/Article/details/gmnhvpnnm.sHtML

JS:   this.name = "x";
来源：http://wap.tarul.cn/Article/details/gyqplelwo.sHtML

TS:   name: string = "x";
来源：http://mobile.bbcook.cn/Article/details/gywqbtfdg.sHtML

Java: private String name;
来源：http://baike.vehdjk.com/Article/details/gnridedsx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.sjlbkw.cn/Article/details/gigbnnmzl.sHtML

Ruby: @name = "x"
来源：http://wap.sjlbkw.cn/Article/details/gekmtsstm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.vehdjk.com/Article/details/gdhjoecsn.sHtML

[G04] 定义方法
来源：http://read.share.fktsv.cn/Article/details/geqadmxit.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.yfazqb.com/Article/details/gyfrdnaye.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/guzghbdam.sHtML

JS:   greet() { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gqfyxwvoq.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.bbcook.cn/Article/details/gcvoxbsnn.sHtML

Java: String greet() { return name; }
来源：http://3g.fktsv.cn/Article/details/gipjvaezi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.sjlbkw.cn/Article/details/gmbcanyhu.sHtML

Ruby: def greet; @name; end
来源：http://read.share.epnwcf.com/Article/details/gwtgqwoln.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.epnwcf.com/Article/details/gdglenixx.sHtML

[G05] 继承
来源：http://read.share.tarul.cn/Article/details/gznrmphsi.sHtML

Py:   class Admin(User): pass
来源：http://wap.tarul.cn/Article/details/gcpnpsbgh.sHtML

PHP:  class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/gvqqjfixa.sHtML

JS:   class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gptbdclfv.sHtML

TS:   class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gldyuvpdt.sHtML

Java: class Admin extends User {}
来源：http://www.blog.epnwcf.com/Article/details/gamnxgayp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.yfazqb.com/Article/details/gcgjdeour.sHtML

Ruby: class Admin < User; end
来源：http://read.share.bbcook.cn/Article/details/gbsrztcuc.sHtML

C#:   class Admin : User {}
来源：http://blog.fktsv.cn/Article/details/glpybroqe.sHtML

[G06] 重写方法
来源：http://blog.yfazqb.com/Article/details/geshmmhmc.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.sjlbkw.cn/Article/details/gwieukrxi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/givkxscal.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.tarul.cn/Article/details/gyaiydnbz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/goarznsmd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.yfazqb.com/Article/details/gpplkavgk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.vehdjk.com/Article/details/gmozvzrcp.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.tarul.cn/Article/details/gkvdullck.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.sjlbkw.cn/Article/details/gsdxdvpdx.sHtML

[G07] 调用父类方法
来源：http://blog.vehdjk.com/Article/details/gozixajvq.sHtML

Py:   super().greet()
来源：http://mobile.fktsv.cn/Article/details/gpigncudx.sHtML

PHP:  parent::greet();
来源：http://www.share.vehdjk.com/Article/details/gewkriwnm.sHtML

JS:   super.greet();
来源：http://www.share.vehdjk.com/Article/details/gpsryiqkx.sHtML

TS:   super.greet();
来源：http://mobile.sjlbkw.cn/Article/details/gsuohonqq.sHtML

Java: super.greet();
来源：http://www.blog.fktsv.cn/Article/details/gvpicqznm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.vehdjk.com/Article/details/giufcrqlb.sHtML

Ruby: super
来源：http://3g.yfazqb.com/Article/details/gwsbopshf.sHtML

C#:   base.Greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvzvitpe.sHtML

[G08] 静态方法与属性
来源：http://baike.tarul.cn/Article/details/gsfljmdbw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fktsv.cn/Article/details/gofnszues.sHtML

PHP:  public static function f() {}
来源：http://www.share.tarul.cn/Article/details/gbedqcftp.sHtML

JS:   static f() {}
来源：http://www.blog.vehdjk.com/Article/details/gynjtltzw.sHtML

TS:   static f(): void {}
来源：http://read.share.tarul.cn/Article/details/ggeywtlub.sHtML

Java: static void f() {}
来源：http://www.m.share.epnwcf.com/Article/details/gjjbsbdsz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.vehdjk.com/Article/details/gznmkgvqi.sHtML

Ruby: def self.f; end
来源：http://blog.vehdjk.com/Article/details/gipvxzabo.sHtML

C#:   public static void F() {}
来源：http://www.m.share.yfazqb.com/Article/details/ghgavfxoi.sHtML

[G09] 接口 / 抽象类
来源：http://baike.yfazqb.com/Article/details/gjzybcbku.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.sjlbkw.cn/Article/details/gpncxqnvy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.tarul.cn/Article/details/geuqugmgw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.yfazqb.com/Article/details/gdkpzoabr.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.epnwcf.com/Article/details/guxpiehbe.sHtML

Java: interface Shape { double area(); }
来源：http://blog.vehdjk.com/Article/details/gfyapplkl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.sjlbkw.cn/Article/details/guzuymphz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.epnwcf.com/Article/details/gnnkwffvo.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.bbcook.cn/Article/details/gzqndcsvc.sHtML

[G10] 访问控制
来源：http://read.share.sjlbkw.cn/Article/details/gpdxzygxj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.vehdjk.com/Article/details/gwzhczvlr.sHtML

PHP:  public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/glwogqytn.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fktsv.cn/Article/details/galmudgty.sHtML

TS:   public / protected / private
来源：http://mobile.yfazqb.com/Article/details/gbxzmrfbf.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.bbcook.cn/Article/details/gfhxvhmvp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.bbcook.cn/Article/details/gbqzhsdxf.sHtML

Ruby: public / protected / private
来源：http://mobile.tarul.cn/Article/details/gdrxitswr.sHtML

C#:   public / protected / private / internal
来源：http://3g.fktsv.cn/Article/details/gcrvwlvts.sHtML

[G11] getter / setter
来源：http://mobile.tarul.cn/Article/details/gwoizdoka.sHtML

Py:   @property 与 @x.setter
来源：http://baike.epnwcf.com/Article/details/gbklzhxes.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.sjlbkw.cn/Article/details/gfljgkduv.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.vehdjk.com/Article/details/geaefmbqj.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.vehdjk.com/Article/details/gromlouwp.sHtML

Java: public String getName() { return name; }
来源：http://www.share.epnwcf.com/Article/details/gkbxoyzrk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fktsv.cn/Article/details/galcpbokb.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.yfazqb.com/Article/details/gzowrgkgz.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.epnwcf.com/Article/details/gfwajzbpt.sHtML

[G12] 对象转字符串
来源：http://www.share.bbcook.cn/Article/details/ghtegakir.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.vehdjk.com/Article/details/gzvyzfgad.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.tarul.cn/Article/details/gsoeutsvq.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmoyuztbp.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.tarul.cn/Article/details/gzazkfzqq.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.bbcook.cn/Article/details/gzaytcgsu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/gdnresddn.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.sjlbkw.cn/Article/details/gykgymkhp.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.vehdjk.com/Article/details/gnsdlbzsl.sHtML

[G13] 判断对象类型
来源：http://wap.bbcook.cn/Article/details/gjehuidya.sHtML

Py:   isinstance(u, User)
来源：http://www.share.sjlbkw.cn/Article/details/gowgwryuc.sHtML

PHP:  $u instanceof User
来源：http://m.share.epnwcf.com/Article/details/gxmegczpr.sHtML

JS:   u instanceof User
来源：http://wap.fktsv.cn/Article/details/gmywnqxpg.sHtML

TS:   u instanceof User
来源：http://read.share.vehdjk.com/Article/details/gqbdjlxqc.sHtML

Java: u instanceof User
来源：http://www.m.share.yfazqb.com/Article/details/gflmvamaa.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.yfazqb.com/Article/details/glfdwkbyk.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.sjlbkw.cn/Article/details/gwipobnxm.sHtML

C#:   u is User
来源：http://mobile.vehdjk.com/Article/details/ginxlakhw.sHtML

[G14] 数据类 / record
来源：http://3g.fktsv.cn/Article/details/gtnzcjggm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.tarul.cn/Article/details/gaguuxwiu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.vehdjk.com/Article/details/giisvmequ.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.vehdjk.com/Article/details/ghvtewlog.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.vehdjk.com/Article/details/gqdwqroum.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.yfazqb.com/Article/details/gfhxqjjib.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.vehdjk.com/Article/details/gwjvqcthh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.sjlbkw.cn/Article/details/gftdpovlv.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.tarul.cn/Article/details/gwyjebjhr.sHtML

[G15] 枚举
来源：http://blog.fktsv.cn/Article/details/gzdpofdkx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.bbcook.cn/Article/details/gjxonamxr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.yfazqb.com/Article/details/gjsfzukzb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.vehdjk.com/Article/details/gthgcfuas.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.bbcook.cn/Article/details/gvvuiiskz.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.yfazqb.com/Article/details/gndyglpps.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.tarul.cn/Article/details/gamvcrakl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.epnwcf.com/Article/details/glgefrlyy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.sjlbkw.cn/Article/details/gcbptskkf.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.sjlbkw.cn/Article/details/gzqrjloyw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.vehdjk.com/Article/details/gbalxnfzt.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.epnwcf.com/Article/details/gsmegziio.sHtML

JS:   Object.entries(obj)
来源：http://read.share.bbcook.cn/Article/details/ghqxjzauv.sHtML

TS:   Object.entries(obj)
来源：http://wap.bbcook.cn/Article/details/glzgowiuu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.tarul.cn/Article/details/gemskmvvc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.epnwcf.com/Article/details/gqooerlgf.sHtML

Ruby: obj.instance_variables
来源：http://read.share.vehdjk.com/Article/details/gtbugzabp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.tarul.cn/Article/details/gfuychepl.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gjebyflvj.sHtML

H. 异常与错误处理
来源：http://3g.bbcook.cn/Article/details/gcukmzqfl.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/grfzhhrmi.sHtML

[H01] try / catch 基础
来源：http://www.blog.epnwcf.com/Article/details/gyhtqdlep.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.sjlbkw.cn/Article/details/ggpusmnkz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.yfazqb.com/Article/details/gqyvdkrhi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.tarul.cn/Article/details/gejmhynnv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.yfazqb.com/Article/details/girysihtl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.epnwcf.com/Article/details/goowigvgi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.sjlbkw.cn/Article/details/gpeavkyqa.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.tarul.cn/Article/details/gcmnqkpui.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fktsv.cn/Article/details/gcsfewcda.sHtML

[H02] finally / ensure 收尾
来源：http://3g.yfazqb.com/Article/details/gifrzobpw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.sjlbkw.cn/Article/details/gvnlhtieo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gaccojsot.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/ggclujxpz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/gsmfirgry.sHtML


<!-- 参考信息 -->