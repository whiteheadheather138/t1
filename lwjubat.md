代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://mobile.sjlbkw.cn/Article/details/gfckhxoog.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.tarul.cn/Article/details/gueodnonq.sHtML

Java: s.lines().toList()
来源：http://3g.yfazqb.com/Article/details/gcaxncaob.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.yfazqb.com/Article/details/gbxizujqk.sHtML

Ruby: s.lines
来源：http://baike.vehdjk.com/Article/details/gggtpzkfi.sHtML

C#:   s.Split('\n')
来源：http://3g.tarul.cn/Article/details/gvkizwtsx.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.yfazqb.com/Article/details/gxkhlogsu.sHtML

Py:   if not s:
来源：http://baike.epnwcf.com/Article/details/gaavhklxr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.sjlbkw.cn/Article/details/gujmlozzc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.tarul.cn/Article/details/gzytoouca.sHtML

TS:   if (s === "") {}
来源：http://baike.epnwcf.com/Article/details/gpxsfzrze.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.sjlbkw.cn/Article/details/gzkgwnkqu.sHtML

Go:   if s == "" {}
来源：http://read.share.fktsv.cn/Article/details/gbemacrqs.sHtML

Ruby: if s.empty?
来源：http://m.share.epnwcf.com/Article/details/gdhdiptdk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.vehdjk.com/Article/details/gipvvttnk.sHtML

[E21] 超长截断加省略号
来源：http://www.share.sjlbkw.cn/Article/details/guvvelnjr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fktsv.cn/Article/details/gpilyldep.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/gxlhnztlk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.tarul.cn/Article/details/gfwaywagr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.tarul.cn/Article/details/gevgkgrnd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.tarul.cn/Article/details/gldczwjsb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.tarul.cn/Article/details/gmdtqmgkn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.tarul.cn/Article/details/gvcqshuqa.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fktsv.cn/Article/details/godkfsrag.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.yfazqb.com/Article/details/gjzanyqfx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.yfazqb.com/Article/details/gancbeuip.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/gkfzxcdxe.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.yfazqb.com/Article/details/gcjyyilpk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fktsv.cn/Article/details/grebemibw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.bbcook.cn/Article/details/gildrdgmn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.epnwcf.com/Article/details/gayqvkysi.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.epnwcf.com/Article/details/grgemyhlo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.bbcook.cn/Article/details/ghpcjqfzu.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gaeozdcmq.sHtML

F. 文件与目录
来源：http://blog.tarul.cn/Article/details/gvrhziflt.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/glqmbpiik.sHtML

[F01] 读取整个文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gsdinmiqb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fktsv.cn/Article/details/gurjeksht.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gwfapiahh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.yfazqb.com/Article/details/gppuyenpu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/gdxlnlxqt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/gdobhknfc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fktsv.cn/Article/details/gwphochnc.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gjbjqyime.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gszvjatcc.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fktsv.cn/Article/details/ggdbmdybw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.vehdjk.com/Article/details/gkwsezjlp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.epnwcf.com/Article/details/gcxhgmpju.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.vehdjk.com/Article/details/gdclpubhn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.tarul.cn/Article/details/gfjrhlirq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.tarul.cn/Article/details/gigkzpmyt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.epnwcf.com/Article/details/gwgfgfrgn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.tarul.cn/Article/details/gocjdaiar.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.sjlbkw.cn/Article/details/gwwsddesy.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.bbcook.cn/Article/details/gtexlkmsd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.sjlbkw.cn/Article/details/gbitzdivq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.bbcook.cn/Article/details/gaqfqinzr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fktsv.cn/Article/details/gjedatrmt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.vehdjk.com/Article/details/gdowemjuq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.yfazqb.com/Article/details/gibopphuk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.tarul.cn/Article/details/gvkgsjgud.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.vehdjk.com/Article/details/gxihqmnqb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.bbcook.cn/Article/details/grumtyrin.sHtML

[F04] 追加写入文件
来源：http://mobile.sjlbkw.cn/Article/details/gjcwcikel.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.yfazqb.com/Article/details/gicgapbgh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.bbcook.cn/Article/details/gkndofprl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmsuuyffo.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.yfazqb.com/Article/details/gamxegcwx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.epnwcf.com/Article/details/gqmdzmlbm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.sjlbkw.cn/Article/details/gokmwowhy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.sjlbkw.cn/Article/details/guoqemavw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.bbcook.cn/Article/details/gdxlwzqhd.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.tarul.cn/Article/details/gykcftgtu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.vehdjk.com/Article/details/glcgizedr.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.bbcook.cn/Article/details/giwwrwovq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/ghomnmveb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gzxbbadqe.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/gkmlypfqt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fktsv.cn/Article/details/grciuzrrf.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.yfazqb.com/Article/details/guyfxqgkr.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.yfazqb.com/Article/details/gvziyazqe.sHtML

[F06] 删除文件
来源：http://wap.bbcook.cn/Article/details/gcimrkdcv.sHtML

Py:   os.remove("a.txt")
来源：http://blog.bbcook.cn/Article/details/gtkwuwwau.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gkddhvpqd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gcnwwgnxj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/gshrcfvye.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/gwcczelch.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gvkowtrsv.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwbqgzzkb.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gxtzdlgao.sHtML

[F07] 创建目录（含多级）
来源：http://blog.tarul.cn/Article/details/gokcwenbu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.bbcook.cn/Article/details/gxbxcofgn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fktsv.cn/Article/details/ghbxiubej.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.tarul.cn/Article/details/gtyjgjgej.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.sjlbkw.cn/Article/details/ghfyapfze.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.epnwcf.com/Article/details/gmfeyszzy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.bbcook.cn/Article/details/gbepkqobo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.yfazqb.com/Article/details/gyrgegaxr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.vehdjk.com/Article/details/gbzyyzupm.sHtML

[F08] 遍历目录
来源：http://www.share.fktsv.cn/Article/details/gjnapiqxa.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.yfazqb.com/Article/details/gieqybopf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fktsv.cn/Article/details/gzohrajmi.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gnvhwvujm.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.yfazqb.com/Article/details/ghwrrhplt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.yfazqb.com/Article/details/gfmrmiuwr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.yfazqb.com/Article/details/gnkxumfuw.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.bbcook.cn/Article/details/goznvvesz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gldjvypya.sHtML

[F09] 获取文件大小
来源：http://www.m.share.tarul.cn/Article/details/gskgczwfi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fktsv.cn/Article/details/gdzcnejaz.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gcjsmwmmj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fktsv.cn/Article/details/gwxwpknmo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.bbcook.cn/Article/details/gxghztwbx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.bbcook.cn/Article/details/gsvseyggp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.sjlbkw.cn/Article/details/gsurbdbxj.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.tarul.cn/Article/details/gqukawbcb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fktsv.cn/Article/details/gglnsmtbb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.yfazqb.com/Article/details/gaybnxmwe.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/granjzgio.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.epnwcf.com/Article/details/gcsdufecm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gbwxjgnui.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gfmpewhxw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.sjlbkw.cn/Article/details/gkacvokoe.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/gvxjrawxq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/gydumhftc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gtzwjriyn.sHtML

[F11] 复制与移动文件
来源：http://read.share.sjlbkw.cn/Article/details/gponefdeo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gxbttalqi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.epnwcf.com/Article/details/gvsixiqph.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gtfssawcl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/gwyckcech.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/gzxuknzxn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fktsv.cn/Article/details/gwjtwybjk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/gufzeuvqr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fktsv.cn/Article/details/ghzpyzvsd.sHtML

[F12] CSV 读写
来源：http://m.share.vehdjk.com/Article/details/gnnoculoe.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.bbcook.cn/Article/details/gkhpbiarx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fktsv.cn/Article/details/gqmdxtjty.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.yfazqb.com/Article/details/gbanbjtqc.sHtML

TS:   // 同上
来源：http://m.share.yfazqb.com/Article/details/gvarfazwi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.yfazqb.com/Article/details/gdweyzzck.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.vehdjk.com/Article/details/gyvqwosam.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.yfazqb.com/Article/details/gqfvnbwwf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.yfazqb.com/Article/details/gaepkxohe.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gpbrtnpgo.sHtML

G. 面向对象
来源：http://www.blog.sjlbkw.cn/Article/details/gngfpvehu.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gwmjnqicx.sHtML

[G01] 定义类
来源：http://read.share.epnwcf.com/Article/details/gngpqpbya.sHtML

Py:   class User: pass
来源：http://mobile.tarul.cn/Article/details/geumoaltn.sHtML

PHP:  class User {}
来源：http://mobile.epnwcf.com/Article/details/gnokscrxf.sHtML

JS:   class User {}
来源：http://baike.sjlbkw.cn/Article/details/gtsaolxbn.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.tarul.cn/Article/details/gavycnenk.sHtML

Java: class User {}
来源：http://3g.bbcook.cn/Article/details/gqmrsjgyz.sHtML

Go:   type User struct { Name string }
来源：http://mobile.epnwcf.com/Article/details/gtwsnbqtj.sHtML

Ruby: class User; end
来源：http://baike.tarul.cn/Article/details/gebfvklxs.sHtML

C#:   class User {}
来源：http://read.share.epnwcf.com/Article/details/gfvhmhesi.sHtML

[G02] 构造函数
来源：http://3g.epnwcf.com/Article/details/gpssfnlfc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.yfazqb.com/Article/details/ghvldiyxz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fktsv.cn/Article/details/gvefquxoy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.sjlbkw.cn/Article/details/gachobwqk.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.epnwcf.com/Article/details/gfigoycmq.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.vehdjk.com/Article/details/gtosemzqu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.tarul.cn/Article/details/gxtmwanga.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.tarul.cn/Article/details/gbjsaubpo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/glfxrpoiy.sHtML

[G03] 实例属性
来源：http://read.share.bbcook.cn/Article/details/garzijlid.sHtML

Py:   self.name = "x"
来源：http://wap.fktsv.cn/Article/details/ghwnjwwtm.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.yfazqb.com/Article/details/glcxcodpb.sHtML

JS:   this.name = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gwjzckwis.sHtML

TS:   name: string = "x";
来源：http://3g.tarul.cn/Article/details/gbxkrombw.sHtML

Java: private String name;
来源：http://baike.epnwcf.com/Article/details/gcmrsnygb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.sjlbkw.cn/Article/details/gsokleflj.sHtML

Ruby: @name = "x"
来源：http://www.m.share.bbcook.cn/Article/details/ggfgxatsp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.bbcook.cn/Article/details/grybzrstv.sHtML

[G04] 定义方法
来源：http://www.share.tarul.cn/Article/details/gokqaenmz.sHtML

Py:   def greet(self): return self.name
来源：http://wap.epnwcf.com/Article/details/glkkduvlt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gpzoodaem.sHtML

JS:   greet() { return this.name; }
来源：http://3g.tarul.cn/Article/details/gxxlgifeo.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/gpmxrygdh.sHtML

Java: String greet() { return name; }
来源：http://baike.epnwcf.com/Article/details/glhkuufjx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/gmklrvjoy.sHtML

Ruby: def greet; @name; end
来源：http://wap.yfazqb.com/Article/details/ghrckbwvm.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.tarul.cn/Article/details/gwfjkysrl.sHtML

[G05] 继承
来源：http://mobile.tarul.cn/Article/details/gxenttolv.sHtML

Py:   class Admin(User): pass
来源：http://baike.bbcook.cn/Article/details/guvagbdvr.sHtML

PHP:  class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gdfkggawp.sHtML

JS:   class Admin extends User {}
来源：http://www.share.sjlbkw.cn/Article/details/gzvzljinj.sHtML

TS:   class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gmjreccgs.sHtML

Java: class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/gacojyshz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.sjlbkw.cn/Article/details/gnrpwcgdq.sHtML

Ruby: class Admin < User; end
来源：http://www.share.bbcook.cn/Article/details/gotppynsd.sHtML

C#:   class Admin : User {}
来源：http://wap.epnwcf.com/Article/details/gribvgzuu.sHtML

[G06] 重写方法
来源：http://m.share.yfazqb.com/Article/details/gpusnsolw.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.vehdjk.com/Article/details/gdcqpchmo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.epnwcf.com/Article/details/gmludezew.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fktsv.cn/Article/details/gqwbvdsrh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/gxcihldrj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/gdklzxqmk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.tarul.cn/Article/details/gpyybzpgf.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.tarul.cn/Article/details/gcawhtblj.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.bbcook.cn/Article/details/gssgccman.sHtML

[G07] 调用父类方法
来源：http://www.share.sjlbkw.cn/Article/details/gvsixsbbv.sHtML

Py:   super().greet()
来源：http://mobile.bbcook.cn/Article/details/ghnsxqpii.sHtML

PHP:  parent::greet();
来源：http://www.share.vehdjk.com/Article/details/gqzhgnktt.sHtML

JS:   super.greet();
来源：http://www.m.share.bbcook.cn/Article/details/gkyoiuwfk.sHtML

TS:   super.greet();
来源：http://wap.vehdjk.com/Article/details/gimnzdosw.sHtML

Java: super.greet();
来源：http://read.share.vehdjk.com/Article/details/giueafzsi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.vehdjk.com/Article/details/gayjrylyr.sHtML

Ruby: super
来源：http://www.m.share.bbcook.cn/Article/details/gxdrgdvjq.sHtML

C#:   base.Greet();
来源：http://baike.yfazqb.com/Article/details/gqmnhjimw.sHtML

[G08] 静态方法与属性
来源：http://mobile.epnwcf.com/Article/details/gpdgirady.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.tarul.cn/Article/details/gccqftnms.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.bbcook.cn/Article/details/gngajwmxw.sHtML

JS:   static f() {}
来源：http://read.share.tarul.cn/Article/details/ghdooeonu.sHtML

TS:   static f(): void {}
来源：http://m.share.fktsv.cn/Article/details/gwpdkgohn.sHtML

Java: static void f() {}
来源：http://blog.bbcook.cn/Article/details/gmfttrall.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.tarul.cn/Article/details/gkoweeuvc.sHtML

Ruby: def self.f; end
来源：http://www.share.sjlbkw.cn/Article/details/gvvsvsgfx.sHtML

C#:   public static void F() {}
来源：http://www.m.share.yfazqb.com/Article/details/gmilbxxai.sHtML

[G09] 接口 / 抽象类
来源：http://blog.tarul.cn/Article/details/gonmlfoob.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.yfazqb.com/Article/details/gpiwqqijf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.epnwcf.com/Article/details/gbunpvukn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fktsv.cn/Article/details/ghnmcwirs.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.vehdjk.com/Article/details/gpnkgifri.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fktsv.cn/Article/details/gvzuoutft.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.tarul.cn/Article/details/gkhbsudgy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.yfazqb.com/Article/details/gempdonut.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.vehdjk.com/Article/details/gtvjeyfoh.sHtML

[G10] 访问控制
来源：http://www.m.share.epnwcf.com/Article/details/gimzapwvm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.bbcook.cn/Article/details/gxsiziwkp.sHtML

PHP:  public / protected / private
来源：http://read.share.sjlbkw.cn/Article/details/guiqcusdc.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fktsv.cn/Article/details/gnvqtorqe.sHtML

TS:   public / protected / private
来源：http://m.share.tarul.cn/Article/details/georqtivy.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.vehdjk.com/Article/details/gorlrwvis.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.bbcook.cn/Article/details/gihfqtnco.sHtML

Ruby: public / protected / private
来源：http://www.m.share.epnwcf.com/Article/details/gyjtbrzkv.sHtML

C#:   public / protected / private / internal
来源：http://3g.fktsv.cn/Article/details/gzpjfhsop.sHtML

[G11] getter / setter
来源：http://baike.epnwcf.com/Article/details/geeigpamd.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.sjlbkw.cn/Article/details/gnibpyeow.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.yfazqb.com/Article/details/gilsqcrzg.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fktsv.cn/Article/details/gbkifvbou.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.tarul.cn/Article/details/gnkwypdaj.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fktsv.cn/Article/details/ggjpbyilq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.vehdjk.com/Article/details/gdewsdxny.sHtML

Ruby: attr_accessor :name
来源：http://wap.tarul.cn/Article/details/gyumgfgnu.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.yfazqb.com/Article/details/gpibpulcs.sHtML

[G12] 对象转字符串
来源：http://www.blog.epnwcf.com/Article/details/gjbevmuas.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.epnwcf.com/Article/details/gkqhwmjnd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/gfkrnlxbe.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/gxpndczao.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.epnwcf.com/Article/details/gstqlelpg.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gttzuwnjk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.sjlbkw.cn/Article/details/gndqgmxgt.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.sjlbkw.cn/Article/details/ggjnuvedb.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.epnwcf.com/Article/details/gkzewmkkl.sHtML

[G13] 判断对象类型
来源：http://baike.yfazqb.com/Article/details/gkezuwjmh.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.vehdjk.com/Article/details/gdohcbfwg.sHtML

PHP:  $u instanceof User
来源：http://blog.vehdjk.com/Article/details/gtokpopxz.sHtML

JS:   u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/gysnguaaz.sHtML

TS:   u instanceof User
来源：http://mobile.tarul.cn/Article/details/gczpvofuf.sHtML

Java: u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/gpwjkdysg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.sjlbkw.cn/Article/details/gkhfxisdj.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.epnwcf.com/Article/details/gilslboob.sHtML

C#:   u is User
来源：http://3g.epnwcf.com/Article/details/gsgucgwoy.sHtML

[G14] 数据类 / record
来源：http://mobile.vehdjk.com/Article/details/ghzmiuptu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fktsv.cn/Article/details/gjqspvdam.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.epnwcf.com/Article/details/gbszlzrks.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fktsv.cn/Article/details/gjsbfxcpu.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.vehdjk.com/Article/details/gvwyzaneg.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.sjlbkw.cn/Article/details/gtrkwfwqe.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.yfazqb.com/Article/details/gaebepuyq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.vehdjk.com/Article/details/gcmzoknyc.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.tarul.cn/Article/details/gdumwdqej.sHtML

[G15] 枚举
来源：http://3g.sjlbkw.cn/Article/details/gobwsvspd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.epnwcf.com/Article/details/gukglcysl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.sjlbkw.cn/Article/details/geyafzhdj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.yfazqb.com/Article/details/gdujpbbgf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fktsv.cn/Article/details/geuesuxtb.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.tarul.cn/Article/details/gjzgymlec.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.bbcook.cn/Article/details/gcupdeckx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fktsv.cn/Article/details/giyripnmn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.yfazqb.com/Article/details/gjlnnoapc.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.epnwcf.com/Article/details/guzceeqyy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fktsv.cn/Article/details/gbkckjemt.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.sjlbkw.cn/Article/details/gvhkrzzyy.sHtML

JS:   Object.entries(obj)
来源：http://wap.fktsv.cn/Article/details/geoyxolle.sHtML

TS:   Object.entries(obj)
来源：http://www.share.bbcook.cn/Article/details/ghhjlivcl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.yfazqb.com/Article/details/gtvzxuajv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.yfazqb.com/Article/details/gebtwrrla.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.yfazqb.com/Article/details/goewhlhvl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.yfazqb.com/Article/details/gnbrqslek.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzguafeh.sHtML

H. 异常与错误处理
来源：http://baike.yfazqb.com/Article/details/gwjatqlxf.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gfexnvzus.sHtML

[H01] try / catch 基础
来源：http://www.m.share.sjlbkw.cn/Article/details/grisvsuxu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.vehdjk.com/Article/details/gdifjoibe.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.sjlbkw.cn/Article/details/gbvwnhktp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.tarul.cn/Article/details/gewstfjeu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.bbcook.cn/Article/details/gbyeglogb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.epnwcf.com/Article/details/gcuytupay.sHtML


<!-- 参考信息 -->