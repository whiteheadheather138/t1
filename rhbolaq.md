代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.blog.vehdjk.com/Article/details/gjznharso.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.yfazqb.com/Article/details/gayreprhl.sHtML

Java: s.lines().toList()
来源：http://blog.bbcook.cn/Article/details/gkwtrqiav.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.epnwcf.com/Article/details/gypdapscp.sHtML

Ruby: s.lines
来源：http://baike.bbcook.cn/Article/details/gtljbztbe.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.tarul.cn/Article/details/gtwjosybw.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.sjlbkw.cn/Article/details/gktpppqef.sHtML

Py:   if not s:
来源：http://blog.tarul.cn/Article/details/ggjsfkwsm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fktsv.cn/Article/details/gmhlckmea.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fktsv.cn/Article/details/gcpejvjye.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.epnwcf.com/Article/details/glkrfscqg.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.sjlbkw.cn/Article/details/gozpvvlmz.sHtML

Go:   if s == "" {}
来源：http://www.blog.tarul.cn/Article/details/ggdiofwvv.sHtML

Ruby: if s.empty?
来源：http://www.share.yfazqb.com/Article/details/gksyrumcm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.epnwcf.com/Article/details/gekurkllh.sHtML

[E21] 超长截断加省略号
来源：http://m.share.sjlbkw.cn/Article/details/gdagvdcdo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.bbcook.cn/Article/details/gtzlcdygt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gmwhspkjs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fktsv.cn/Article/details/gqvxsyghm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/gjnowohbs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gwfvdsblf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.yfazqb.com/Article/details/gzcmdfywf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.bbcook.cn/Article/details/ggzzyjarv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/ggjuqzquh.sHtML

[E22] 字节长度与字符长度
来源：http://wap.tarul.cn/Article/details/gqihltfox.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.yfazqb.com/Article/details/gibtsuqtf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gzcalbqom.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.bbcook.cn/Article/details/gwnntukks.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.tarul.cn/Article/details/gcdqgcafe.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.bbcook.cn/Article/details/guwujsads.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.epnwcf.com/Article/details/gcvtrwtyx.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.tarul.cn/Article/details/ggxhdsjfc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.epnwcf.com/Article/details/geugdookl.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gfbjnaztq.sHtML

F. 文件与目录
来源：http://www.m.share.vehdjk.com/Article/details/gyjnrqnpe.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/guafbysgr.sHtML

[F01] 读取整个文件
来源：http://www.share.bbcook.cn/Article/details/gevuzhxlj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.tarul.cn/Article/details/ggndyzbku.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gfmgsvfsz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.sjlbkw.cn/Article/details/grwmtbhbk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.epnwcf.com/Article/details/ghfbwrgwf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/gjweeskjo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.sjlbkw.cn/Article/details/gusjflxjt.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gvqnrfore.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.yfazqb.com/Article/details/gxkfhujnx.sHtML

[F02] 逐行读取文件
来源：http://wap.epnwcf.com/Article/details/gmvxqqfqs.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.tarul.cn/Article/details/gjhhycagl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.vehdjk.com/Article/details/gzimahnkb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.epnwcf.com/Article/details/gwiwqqomx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.sjlbkw.cn/Article/details/gxpuhegro.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.epnwcf.com/Article/details/ghmlqlngk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.bbcook.cn/Article/details/gjnbbxjje.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.epnwcf.com/Article/details/gwnfrzmhg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.sjlbkw.cn/Article/details/gkwpuecjq.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.bbcook.cn/Article/details/gztisczzv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.epnwcf.com/Article/details/grknlvnrk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fktsv.cn/Article/details/glojvzrlz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fktsv.cn/Article/details/gnrtceuwz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.vehdjk.com/Article/details/gimrpsaiu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.yfazqb.com/Article/details/ghephdoxz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.bbcook.cn/Article/details/gpioryuoz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.bbcook.cn/Article/details/ggbhzpfdt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.sjlbkw.cn/Article/details/gmkxrdaun.sHtML

[F04] 追加写入文件
来源：http://www.blog.yfazqb.com/Article/details/ggojtvvqv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.bbcook.cn/Article/details/gvmpfzapc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.epnwcf.com/Article/details/gyoinhrbi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.sjlbkw.cn/Article/details/gxgyqkymw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.bbcook.cn/Article/details/grdchqdye.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.bbcook.cn/Article/details/gizumedux.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.tarul.cn/Article/details/gjypwkrvd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.yfazqb.com/Article/details/gybeeynbl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.epnwcf.com/Article/details/gwmkqlnwi.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gyyrhkujt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.vehdjk.com/Article/details/geaswgftc.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gxbfliepl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/guhiaauem.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gsvquzamw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gfqvcyrkd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.vehdjk.com/Article/details/gtaovfvaq.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gauawzxgf.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.tarul.cn/Article/details/gsaekmome.sHtML

[F06] 删除文件
来源：http://3g.tarul.cn/Article/details/gohiafjyg.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gvewzdyji.sHtML

PHP:  unlink("a.txt");
来源：http://3g.tarul.cn/Article/details/ghllhqlow.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gydtkjzrt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gfhsjctlb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/gpwnmvzjs.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.tarul.cn/Article/details/gukcsuryq.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gkbrbvyxl.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.bbcook.cn/Article/details/goibedcvp.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.sjlbkw.cn/Article/details/gyxckedna.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.yfazqb.com/Article/details/gxmtcjmfz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.tarul.cn/Article/details/ggwgndzse.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fktsv.cn/Article/details/gbvmzbkux.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.sjlbkw.cn/Article/details/gtwiistup.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.epnwcf.com/Article/details/gvlqmqxra.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fktsv.cn/Article/details/gfyohnnhi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.vehdjk.com/Article/details/gbcklwkhx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fktsv.cn/Article/details/gfhgiadvm.sHtML

[F08] 遍历目录
来源：http://read.share.vehdjk.com/Article/details/gktlzzmsd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.bbcook.cn/Article/details/gcvhfyvvb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.tarul.cn/Article/details/gbqdhctvm.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fktsv.cn/Article/details/gdbbxizjl.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.epnwcf.com/Article/details/gaxjxamsa.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.epnwcf.com/Article/details/ghntftqup.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gxdffwreu.sHtML

Ruby: Dir.children("dir")
来源：http://blog.bbcook.cn/Article/details/gjpvkomiu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.tarul.cn/Article/details/gyhtblppp.sHtML

[F09] 获取文件大小
来源：http://www.share.tarul.cn/Article/details/gfpunmnyr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.tarul.cn/Article/details/gmneerkmm.sHtML

PHP:  filesize("a.txt");
来源：http://blog.tarul.cn/Article/details/goqxswpnq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.bbcook.cn/Article/details/gizvjrzwc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fktsv.cn/Article/details/gkwptounb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/gmzoesfxi.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.vehdjk.com/Article/details/gindblndc.sHtML

Ruby: File.size("a.txt")
来源：http://blog.yfazqb.com/Article/details/gzwpwkmwm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fktsv.cn/Article/details/gwhbuzhkk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.sjlbkw.cn/Article/details/gbkkbimtp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/grytwlvhw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gycpxmzpn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/goaaswnva.sHtML

TS:   path.extname("a.txt")
来源：http://blog.tarul.cn/Article/details/gvecnedrv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.yfazqb.com/Article/details/gwnslzbpi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/goiiiudai.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gyqlpdjdb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gifhllpux.sHtML

[F11] 复制与移动文件
来源：http://baike.bbcook.cn/Article/details/gywwxalfr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/gylkxjbqv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.vehdjk.com/Article/details/gwsnysubq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gstsuqsnl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/gosuksmbd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.epnwcf.com/Article/details/gunsdeeyv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.vehdjk.com/Article/details/gmpdjqgpt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/gmmnologm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.epnwcf.com/Article/details/gmdckvajn.sHtML

[F12] CSV 读写
来源：http://m.share.epnwcf.com/Article/details/gdokazloh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.vehdjk.com/Article/details/gejtujzoh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.epnwcf.com/Article/details/gbealcjqo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.tarul.cn/Article/details/gqqryhfvi.sHtML

TS:   // 同上
来源：http://www.share.tarul.cn/Article/details/gizwzahho.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.vehdjk.com/Article/details/ggwbgkryi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.vehdjk.com/Article/details/gyswdchoo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fktsv.cn/Article/details/ggotjcqhd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.vehdjk.com/Article/details/gtxrtrvjf.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gwvsqlfvd.sHtML

G. 面向对象
来源：http://www.m.share.yfazqb.com/Article/details/glkhzlztw.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/glnsrqqtz.sHtML

[G01] 定义类
来源：http://read.share.fktsv.cn/Article/details/gwflhgruw.sHtML

Py:   class User: pass
来源：http://read.share.bbcook.cn/Article/details/gqemypnrv.sHtML

PHP:  class User {}
来源：http://read.share.epnwcf.com/Article/details/gcyhoikdp.sHtML

JS:   class User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqzidpjx.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.sjlbkw.cn/Article/details/gwkvnumeu.sHtML

Java: class User {}
来源：http://m.share.vehdjk.com/Article/details/gdrupieiq.sHtML

Go:   type User struct { Name string }
来源：http://baike.yfazqb.com/Article/details/glxmrfqav.sHtML

Ruby: class User; end
来源：http://mobile.fktsv.cn/Article/details/guilrmxoh.sHtML

C#:   class User {}
来源：http://m.share.vehdjk.com/Article/details/gwvxrfmnv.sHtML

[G02] 构造函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gcwgvqekn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.sjlbkw.cn/Article/details/gkuhxqvxx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.vehdjk.com/Article/details/gpsloihoc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fktsv.cn/Article/details/govludshe.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.tarul.cn/Article/details/govwdoyyz.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.bbcook.cn/Article/details/gqgglmmgv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.epnwcf.com/Article/details/gpoohlgwx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwbuwgcc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.yfazqb.com/Article/details/gszttvjhr.sHtML

[G03] 实例属性
来源：http://mobile.bbcook.cn/Article/details/gimbjegkm.sHtML

Py:   self.name = "x"
来源：http://www.blog.bbcook.cn/Article/details/gnkhdsobc.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.vehdjk.com/Article/details/gvfyquzay.sHtML

JS:   this.name = "x";
来源：http://baike.fktsv.cn/Article/details/gyumtdbgi.sHtML

TS:   name: string = "x";
来源：http://baike.fktsv.cn/Article/details/gfntyxgii.sHtML

Java: private String name;
来源：http://read.share.epnwcf.com/Article/details/gqrnoxnqk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.vehdjk.com/Article/details/gskoxipdq.sHtML

Ruby: @name = "x"
来源：http://www.blog.bbcook.cn/Article/details/gvvkrmzut.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gpcfbvfox.sHtML

[G04] 定义方法
来源：http://m.share.vehdjk.com/Article/details/guhpfajkv.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.yfazqb.com/Article/details/gvthbnnvx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.tarul.cn/Article/details/gwefnbvoq.sHtML

JS:   greet() { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gakfsgbhb.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/giufgtyuu.sHtML

Java: String greet() { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/gqxxbxuxa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/glaxrmcnb.sHtML

Ruby: def greet; @name; end
来源：http://blog.sjlbkw.cn/Article/details/gcmsdhffh.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.tarul.cn/Article/details/gramvokpb.sHtML

[G05] 继承
来源：http://www.share.bbcook.cn/Article/details/gpigchknc.sHtML

Py:   class Admin(User): pass
来源：http://3g.fktsv.cn/Article/details/gyuojgknf.sHtML

PHP:  class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gibcadzai.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/gbblmnjeg.sHtML

TS:   class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gpljulyvb.sHtML

Java: class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/gfgrafukr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.vehdjk.com/Article/details/gzfqhwizm.sHtML

Ruby: class Admin < User; end
来源：http://3g.vehdjk.com/Article/details/gpbndxqmg.sHtML

C#:   class Admin : User {}
来源：http://3g.fktsv.cn/Article/details/gzyrgwbbo.sHtML

[G06] 重写方法
来源：http://wap.sjlbkw.cn/Article/details/glxdudmdc.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.vehdjk.com/Article/details/ginbklihb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.vehdjk.com/Article/details/gfyeggpkz.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.yfazqb.com/Article/details/gebwgkzwq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.tarul.cn/Article/details/gbbmepukp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/gxggffufn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.tarul.cn/Article/details/gzaftumwr.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.sjlbkw.cn/Article/details/ggxxexswo.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.tarul.cn/Article/details/ggzigbqhc.sHtML

[G07] 调用父类方法
来源：http://www.m.share.yfazqb.com/Article/details/gmgapjcnx.sHtML

Py:   super().greet()
来源：http://www.share.fktsv.cn/Article/details/gcxaiscrl.sHtML

PHP:  parent::greet();
来源：http://m.share.fktsv.cn/Article/details/gzjwwuite.sHtML

JS:   super.greet();
来源：http://m.share.epnwcf.com/Article/details/gywhgomjj.sHtML

TS:   super.greet();
来源：http://3g.epnwcf.com/Article/details/gqgtbjrek.sHtML

Java: super.greet();
来源：http://mobile.bbcook.cn/Article/details/glwvoqobz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.sjlbkw.cn/Article/details/gfvzowdlt.sHtML

Ruby: super
来源：http://www.blog.fktsv.cn/Article/details/gavjmkjuk.sHtML

C#:   base.Greet();
来源：http://3g.vehdjk.com/Article/details/gmzucwjys.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.vehdjk.com/Article/details/givijnkyu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.yfazqb.com/Article/details/gnpvdtemb.sHtML

PHP:  public static function f() {}
来源：http://mobile.vehdjk.com/Article/details/grwiynudv.sHtML

JS:   static f() {}
来源：http://wap.fktsv.cn/Article/details/gbpmilyvd.sHtML

TS:   static f(): void {}
来源：http://wap.tarul.cn/Article/details/geulkfzxf.sHtML

Java: static void f() {}
来源：http://www.blog.fktsv.cn/Article/details/grlmivjxj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.epnwcf.com/Article/details/gjosmttla.sHtML

Ruby: def self.f; end
来源：http://wap.sjlbkw.cn/Article/details/gqzgykzax.sHtML

C#:   public static void F() {}
来源：http://wap.fktsv.cn/Article/details/gvhsphqri.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fktsv.cn/Article/details/gfeblsdrk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.sjlbkw.cn/Article/details/gelrjzvui.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.epnwcf.com/Article/details/gjdmshfdd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.bbcook.cn/Article/details/gzzyqzypt.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.tarul.cn/Article/details/gafunpknr.sHtML

Java: interface Shape { double area(); }
来源：http://blog.tarul.cn/Article/details/gvneukylz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fktsv.cn/Article/details/gtentamip.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.epnwcf.com/Article/details/gufehddnv.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.epnwcf.com/Article/details/grwqqdshj.sHtML

[G10] 访问控制
来源：http://read.share.fktsv.cn/Article/details/gwtbihjwm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.sjlbkw.cn/Article/details/gnjxickmx.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fktsv.cn/Article/details/gnrgvbbck.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.bbcook.cn/Article/details/gisxzpvig.sHtML

TS:   public / protected / private
来源：http://read.share.vehdjk.com/Article/details/gnybzjffk.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.bbcook.cn/Article/details/gzefchmsc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.vehdjk.com/Article/details/grksgxdae.sHtML

Ruby: public / protected / private
来源：http://read.share.vehdjk.com/Article/details/gqtgxzeoc.sHtML

C#:   public / protected / private / internal
来源：http://3g.fktsv.cn/Article/details/goyhtwpxs.sHtML

[G11] getter / setter
来源：http://mobile.vehdjk.com/Article/details/ghktnpwrn.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.epnwcf.com/Article/details/gaekheraf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/gojatehxr.sHtML

JS:   get name() { return this._name; }
来源：http://baike.epnwcf.com/Article/details/golehbiiq.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fktsv.cn/Article/details/gzmaybcri.sHtML

Java: public String getName() { return name; }
来源：http://wap.epnwcf.com/Article/details/gaehebdzx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.vehdjk.com/Article/details/gjgnbqytv.sHtML

Ruby: attr_accessor :name
来源：http://www.share.bbcook.cn/Article/details/gsysssruh.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fktsv.cn/Article/details/glgmtnjsx.sHtML

[G12] 对象转字符串
来源：http://www.share.bbcook.cn/Article/details/gddslmimn.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.yfazqb.com/Article/details/grdyeqdfy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fktsv.cn/Article/details/gbcjchpck.sHtML

JS:   toString() { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gkzssgkau.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.tarul.cn/Article/details/gerjxociq.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.epnwcf.com/Article/details/givjcqmmv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.yfazqb.com/Article/details/goqswqgqv.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fktsv.cn/Article/details/gprtaknlz.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.bbcook.cn/Article/details/gqxauvmxq.sHtML

[G13] 判断对象类型
来源：http://baike.vehdjk.com/Article/details/gzvwkvfcc.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.sjlbkw.cn/Article/details/gwdconmjv.sHtML

PHP:  $u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gnuuuxsnl.sHtML

JS:   u instanceof User
来源：http://blog.fktsv.cn/Article/details/gtataatjg.sHtML

TS:   u instanceof User
来源：http://m.share.yfazqb.com/Article/details/gdbgpafnf.sHtML

Java: u instanceof User
来源：http://www.share.fktsv.cn/Article/details/gffjnonkd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.sjlbkw.cn/Article/details/ggefiprqz.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.tarul.cn/Article/details/gcoktekjm.sHtML

C#:   u is User
来源：http://3g.tarul.cn/Article/details/gopaucfip.sHtML

[G14] 数据类 / record
来源：http://www.m.share.vehdjk.com/Article/details/gmpuagbyk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fktsv.cn/Article/details/gltyzfrkq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.epnwcf.com/Article/details/gbsxszlli.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.epnwcf.com/Article/details/gaiqlqxvo.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.sjlbkw.cn/Article/details/gzuvvxerf.sHtML

Java: record User(String name, int age) {}
来源：http://blog.yfazqb.com/Article/details/gmrummhec.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.tarul.cn/Article/details/gyferzcyh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.sjlbkw.cn/Article/details/geohofpjr.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.vehdjk.com/Article/details/gjqauruyg.sHtML

[G15] 枚举
来源：http://read.share.tarul.cn/Article/details/gyhuwzwzi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.vehdjk.com/Article/details/grhhykeiq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.yfazqb.com/Article/details/gdictuorx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.yfazqb.com/Article/details/gibwqdagz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.bbcook.cn/Article/details/gwszqmjpq.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.epnwcf.com/Article/details/gfsbdtdvp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.epnwcf.com/Article/details/ghhlawbmd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.tarul.cn/Article/details/geellesul.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.epnwcf.com/Article/details/gxsezmpux.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.vehdjk.com/Article/details/gswpttidz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.epnwcf.com/Article/details/gcpawbnhd.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.epnwcf.com/Article/details/gkczwscut.sHtML

JS:   Object.entries(obj)
来源：http://wap.yfazqb.com/Article/details/gaejwdiaw.sHtML

TS:   Object.entries(obj)
来源：http://read.share.epnwcf.com/Article/details/gshacdhns.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.bbcook.cn/Article/details/gparrzque.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.epnwcf.com/Article/details/gdzbvibrg.sHtML

Ruby: obj.instance_variables
来源：http://read.share.sjlbkw.cn/Article/details/gwewfdjif.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.sjlbkw.cn/Article/details/gmejczxhx.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/ggqgeaxng.sHtML

H. 异常与错误处理
来源：http://www.m.share.fktsv.cn/Article/details/gpyeefiac.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gqgxdpinj.sHtML

[H01] try / catch 基础
来源：http://mobile.fktsv.cn/Article/details/gtvyzoups.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fktsv.cn/Article/details/govokdzko.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.bbcook.cn/Article/details/gxkrkfita.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.yfazqb.com/Article/details/gismydipn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.bbcook.cn/Article/details/gzihqxpeu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.sjlbkw.cn/Article/details/gcetzyhos.sHtML


<!-- 参考信息 -->