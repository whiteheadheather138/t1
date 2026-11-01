代发 wailian999

Ruby: s.lines
来源：http://read.share.yfazqb.com/Article/details/glphfvhnu.sHtML

C#:   s.Split('\n')
来源：http://read.share.tarul.cn/Article/details/ghmuokykv.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.epnwcf.com/Article/details/gbhwbavib.sHtML

Py:   if not s:
来源：http://www.share.sjlbkw.cn/Article/details/gysejutpo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.vehdjk.com/Article/details/ghqmpcqjo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.bbcook.cn/Article/details/gxzhkwrhx.sHtML

TS:   if (s === "") {}
来源：http://read.share.epnwcf.com/Article/details/gcristnzz.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.epnwcf.com/Article/details/gmgzwktds.sHtML

Go:   if s == "" {}
来源：http://baike.vehdjk.com/Article/details/gnxqyxwzr.sHtML

Ruby: if s.empty?
来源：http://baike.sjlbkw.cn/Article/details/giathevgx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.vehdjk.com/Article/details/gxvkuqjjm.sHtML

[E21] 超长截断加省略号
来源：http://www.share.tarul.cn/Article/details/gremswyml.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.epnwcf.com/Article/details/gbxicjtet.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fktsv.cn/Article/details/gvjstjmrj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.yfazqb.com/Article/details/gbhiyneyr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gfyvnjstu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/ggduijavf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.tarul.cn/Article/details/gpnsalghq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gkzprnijm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gltowjzhs.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.tarul.cn/Article/details/givhjdqlj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.tarul.cn/Article/details/ghfnelcpf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gwjjjxsyn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fktsv.cn/Article/details/gptvsatxf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.bbcook.cn/Article/details/gxflpljbj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.epnwcf.com/Article/details/gurkkyqdz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fktsv.cn/Article/details/gnyoxqshx.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.yfazqb.com/Article/details/gcfyyewrx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.vehdjk.com/Article/details/geodgenpi.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/grzvyayjc.sHtML

F. 文件与目录
来源：http://www.share.tarul.cn/Article/details/gcsvzmrim.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/ghfcguikv.sHtML

[F01] 读取整个文件
来源：http://www.blog.epnwcf.com/Article/details/gxwkzoorw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.sjlbkw.cn/Article/details/gaebzlxao.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.bbcook.cn/Article/details/guamyxkci.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.tarul.cn/Article/details/gcyshtnbj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.vehdjk.com/Article/details/gzjjegdoi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/gmbspathb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.epnwcf.com/Article/details/gvanhalap.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gfuhyddys.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gwkbdkerg.sHtML

[F02] 逐行读取文件
来源：http://wap.fktsv.cn/Article/details/gegkurold.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fktsv.cn/Article/details/gbpjgbrvh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.yfazqb.com/Article/details/ggjyloypz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.yfazqb.com/Article/details/gbnsxhczc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fktsv.cn/Article/details/gzfkjkcsm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.bbcook.cn/Article/details/gpuyfjsgp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.sjlbkw.cn/Article/details/gpovhtjuq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.tarul.cn/Article/details/gpmkupxxx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.epnwcf.com/Article/details/guokphcma.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fktsv.cn/Article/details/gqeliktwl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.vehdjk.com/Article/details/gnrlkhwyv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fktsv.cn/Article/details/gbfpwayhp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.sjlbkw.cn/Article/details/gpqdppfzq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.bbcook.cn/Article/details/gsgolpmwg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.sjlbkw.cn/Article/details/gagplamhz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.yfazqb.com/Article/details/gccivnqlh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.epnwcf.com/Article/details/ghnfmasnv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.tarul.cn/Article/details/gwtphmone.sHtML

[F04] 追加写入文件
来源：http://www.blog.fktsv.cn/Article/details/gvlrttauj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fktsv.cn/Article/details/grpixatyd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.yfazqb.com/Article/details/gekizhyks.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.tarul.cn/Article/details/gyhakdpfu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.bbcook.cn/Article/details/galsqwrkt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.bbcook.cn/Article/details/grtmbalhb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.vehdjk.com/Article/details/gucntqjtu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.epnwcf.com/Article/details/gmfpokboo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fktsv.cn/Article/details/gbmbxrpwj.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.yfazqb.com/Article/details/gagdznxwz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fktsv.cn/Article/details/gyxapoena.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gnenvjssh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gwxaxotay.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/gzlnvjubb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/gkedozkqg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.bbcook.cn/Article/details/gsaoyoojh.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gynnvxive.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gfiedicwf.sHtML

[F06] 删除文件
来源：http://www.blog.epnwcf.com/Article/details/gbcboieif.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gjxmqleci.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.epnwcf.com/Article/details/grwbzuegm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/gabrpeayh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/goyhurazq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.epnwcf.com/Article/details/gotfebexo.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gytjrlhfv.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fktsv.cn/Article/details/gblxdkuwm.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.tarul.cn/Article/details/ggpssanbf.sHtML

[F07] 创建目录（含多级）
来源：http://baike.sjlbkw.cn/Article/details/givnkqbmb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.bbcook.cn/Article/details/ghzpwfask.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.yfazqb.com/Article/details/gfkmmveuy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.yfazqb.com/Article/details/glvorqwje.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.bbcook.cn/Article/details/gpzrhbskd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fktsv.cn/Article/details/gplkpafvg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.tarul.cn/Article/details/glbjzrqrr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.vehdjk.com/Article/details/gvtorjdwh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fktsv.cn/Article/details/gthyxkvql.sHtML

[F08] 遍历目录
来源：http://baike.tarul.cn/Article/details/gjgrnedne.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.vehdjk.com/Article/details/gqyeqvoup.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.yfazqb.com/Article/details/ggjxbsooj.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gfctwydbl.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.tarul.cn/Article/details/gxjyhkoaj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.tarul.cn/Article/details/gvmtzyfbm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.yfazqb.com/Article/details/gdvvprhmd.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.sjlbkw.cn/Article/details/griaddugm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.epnwcf.com/Article/details/gaynzpbdq.sHtML

[F09] 获取文件大小
来源：http://www.m.share.tarul.cn/Article/details/galyduhvu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.vehdjk.com/Article/details/gnuzoudlf.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.tarul.cn/Article/details/gajseyfia.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.tarul.cn/Article/details/glvfihunx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.vehdjk.com/Article/details/gpyentsky.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.sjlbkw.cn/Article/details/gxumphtgp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fktsv.cn/Article/details/gjqlrsevn.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gjzsjulbl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.epnwcf.com/Article/details/ginhyazls.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.sjlbkw.cn/Article/details/gqcxystke.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/ggkwthgon.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gmsllspsg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gmbumulcd.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.bbcook.cn/Article/details/giszdoeem.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fktsv.cn/Article/details/ggadkgyxi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/ggfhdoppn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gdqposdwv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/goslimkyg.sHtML

[F11] 复制与移动文件
来源：http://www.share.sjlbkw.cn/Article/details/gfhykjamx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.tarul.cn/Article/details/gqpemadfy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gbwvfslpw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/gzdvsazok.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gdmdyydye.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gofizfudb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fktsv.cn/Article/details/godvbyiuy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gyriselep.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.epnwcf.com/Article/details/gbrpvlvjc.sHtML

[F12] CSV 读写
来源：http://m.share.bbcook.cn/Article/details/guyovjhtn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.vehdjk.com/Article/details/gbtvzbdoy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fktsv.cn/Article/details/gbkbqgnzl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.bbcook.cn/Article/details/gabjczvik.sHtML

TS:   // 同上
来源：http://baike.yfazqb.com/Article/details/gpmktorzm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.bbcook.cn/Article/details/gvmnnhrwu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.sjlbkw.cn/Article/details/gbwjremot.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.epnwcf.com/Article/details/gtasqpoyn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.epnwcf.com/Article/details/gmaourrrk.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gbhhjbrsz.sHtML

G. 面向对象
来源：http://wap.fktsv.cn/Article/details/ggqkflfvi.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/grdsspfwq.sHtML

[G01] 定义类
来源：http://www.share.yfazqb.com/Article/details/gzlroyuin.sHtML

Py:   class User: pass
来源：http://3g.epnwcf.com/Article/details/gsrkipugh.sHtML

PHP:  class User {}
来源：http://www.blog.yfazqb.com/Article/details/ghxtjjhiv.sHtML

JS:   class User {}
来源：http://wap.yfazqb.com/Article/details/gdojqjjpa.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.yfazqb.com/Article/details/gaigbfaqk.sHtML

Java: class User {}
来源：http://mobile.yfazqb.com/Article/details/gnxnydmfv.sHtML

Go:   type User struct { Name string }
来源：http://blog.epnwcf.com/Article/details/gpjdtwqma.sHtML

Ruby: class User; end
来源：http://m.share.vehdjk.com/Article/details/gxemkbksd.sHtML

C#:   class User {}
来源：http://3g.vehdjk.com/Article/details/gkvbzhumr.sHtML

[G02] 构造函数
来源：http://www.m.share.vehdjk.com/Article/details/gpzlppawe.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.tarul.cn/Article/details/gtlyqpcvf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.epnwcf.com/Article/details/gpgqynvjr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.epnwcf.com/Article/details/gaoewzlpk.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.vehdjk.com/Article/details/grwdayiif.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.tarul.cn/Article/details/gpibtqynt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fktsv.cn/Article/details/gdrbiwlfi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.tarul.cn/Article/details/gufeqfezg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.sjlbkw.cn/Article/details/gtunaribh.sHtML

[G03] 实例属性
来源：http://www.blog.yfazqb.com/Article/details/gagrdthjc.sHtML

Py:   self.name = "x"
来源：http://www.m.share.bbcook.cn/Article/details/gxmyrxrzz.sHtML

PHP:  public string $name = "x";
来源：http://read.share.tarul.cn/Article/details/gmsfrppqy.sHtML

JS:   this.name = "x";
来源：http://m.share.fktsv.cn/Article/details/gnvaosjij.sHtML

TS:   name: string = "x";
来源：http://www.share.tarul.cn/Article/details/gwadwdkdm.sHtML

Java: private String name;
来源：http://read.share.epnwcf.com/Article/details/gczbysssg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.vehdjk.com/Article/details/gdwrtmlsn.sHtML

Ruby: @name = "x"
来源：http://mobile.epnwcf.com/Article/details/gbzluolwm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gtearcvvm.sHtML

[G04] 定义方法
来源：http://mobile.sjlbkw.cn/Article/details/ghgbbkezz.sHtML

Py:   def greet(self): return self.name
来源：http://blog.sjlbkw.cn/Article/details/gposmrcyo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.yfazqb.com/Article/details/gzkbvjrks.sHtML

JS:   greet() { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gjrvghjds.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gwibkoxqu.sHtML

Java: String greet() { return name; }
来源：http://baike.vehdjk.com/Article/details/gtecdjmam.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/gralswcys.sHtML

Ruby: def greet; @name; end
来源：http://blog.epnwcf.com/Article/details/gaeqzsuba.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.bbcook.cn/Article/details/gpuvxoztu.sHtML

[G05] 继承
来源：http://wap.tarul.cn/Article/details/goqgewcdc.sHtML

Py:   class Admin(User): pass
来源：http://wap.vehdjk.com/Article/details/gbdttdnju.sHtML

PHP:  class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/gtjahyycs.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.vehdjk.com/Article/details/gnvjmxesl.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/ggyrdenie.sHtML

Java: class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/gtjnsieyo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.tarul.cn/Article/details/ghxsymlcn.sHtML

Ruby: class Admin < User; end
来源：http://mobile.yfazqb.com/Article/details/gwvmaqvxq.sHtML

C#:   class Admin : User {}
来源：http://mobile.epnwcf.com/Article/details/gofccohrz.sHtML

[G06] 重写方法
来源：http://blog.bbcook.cn/Article/details/gvpifjiss.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.tarul.cn/Article/details/gursffkkm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/ghjibebzk.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/gjlunclee.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkjucjnxp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.tarul.cn/Article/details/gemkldxlu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.bbcook.cn/Article/details/gedwlkwqn.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fktsv.cn/Article/details/gbzfndgub.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.vehdjk.com/Article/details/goszhdiag.sHtML

[G07] 调用父类方法
来源：http://mobile.yfazqb.com/Article/details/ghxlzxvss.sHtML

Py:   super().greet()
来源：http://3g.tarul.cn/Article/details/gevcbxiob.sHtML

PHP:  parent::greet();
来源：http://wap.sjlbkw.cn/Article/details/gbcdotium.sHtML

JS:   super.greet();
来源：http://read.share.fktsv.cn/Article/details/gjbtmizeu.sHtML

TS:   super.greet();
来源：http://blog.fktsv.cn/Article/details/gzckpolnw.sHtML

Java: super.greet();
来源：http://mobile.yfazqb.com/Article/details/gkcsjscql.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fktsv.cn/Article/details/gzsybblaf.sHtML

Ruby: super
来源：http://3g.bbcook.cn/Article/details/gsvznayln.sHtML

C#:   base.Greet();
来源：http://www.m.share.vehdjk.com/Article/details/gnpnjeuyz.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fktsv.cn/Article/details/gqeicupqp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.epnwcf.com/Article/details/gcgiqxhmo.sHtML

PHP:  public static function f() {}
来源：http://mobile.fktsv.cn/Article/details/gsfbrqkkv.sHtML

JS:   static f() {}
来源：http://baike.bbcook.cn/Article/details/grvehfwpv.sHtML

TS:   static f(): void {}
来源：http://3g.yfazqb.com/Article/details/gckavhikn.sHtML

Java: static void f() {}
来源：http://baike.sjlbkw.cn/Article/details/gverkxexb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.vehdjk.com/Article/details/gdmxonxrk.sHtML

Ruby: def self.f; end
来源：http://blog.tarul.cn/Article/details/gpheuwvvp.sHtML

C#:   public static void F() {}
来源：http://mobile.vehdjk.com/Article/details/gzltxswgp.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.bbcook.cn/Article/details/gjyrmficy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fktsv.cn/Article/details/gxuuavawz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.tarul.cn/Article/details/gtusdwrqd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.epnwcf.com/Article/details/gnvragftn.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.sjlbkw.cn/Article/details/gktyvzdmm.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fktsv.cn/Article/details/gglukzndn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.epnwcf.com/Article/details/glwihwkke.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.tarul.cn/Article/details/gghphptto.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.tarul.cn/Article/details/gnlrvwkqw.sHtML

[G10] 访问控制
来源：http://baike.vehdjk.com/Article/details/gofmwiklf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.tarul.cn/Article/details/gtvontmkk.sHtML

PHP:  public / protected / private
来源：http://read.share.bbcook.cn/Article/details/gqborsimr.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.vehdjk.com/Article/details/gikyjppir.sHtML

TS:   public / protected / private
来源：http://mobile.tarul.cn/Article/details/gyamwxopx.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.sjlbkw.cn/Article/details/glumdvgmy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.sjlbkw.cn/Article/details/gffdgkypc.sHtML

Ruby: public / protected / private
来源：http://mobile.tarul.cn/Article/details/gkpgyogsu.sHtML

C#:   public / protected / private / internal
来源：http://www.share.sjlbkw.cn/Article/details/gcvvldfcz.sHtML

[G11] getter / setter
来源：http://mobile.epnwcf.com/Article/details/glfggcewi.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.yfazqb.com/Article/details/gqdfqgbly.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.tarul.cn/Article/details/giismynfx.sHtML

JS:   get name() { return this._name; }
来源：http://wap.bbcook.cn/Article/details/gsctwaknl.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.vehdjk.com/Article/details/glznpnyxe.sHtML

Java: public String getName() { return name; }
来源：http://wap.vehdjk.com/Article/details/gszanqgff.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.bbcook.cn/Article/details/gpzjnlsvq.sHtML

Ruby: attr_accessor :name
来源：http://baike.epnwcf.com/Article/details/gmbzuiawa.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.vehdjk.com/Article/details/ghthabxtv.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fktsv.cn/Article/details/gbaumpehh.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.vehdjk.com/Article/details/gpcovgzld.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.vehdjk.com/Article/details/gtokqihst.sHtML

JS:   toString() { return this.name; }
来源：http://3g.tarul.cn/Article/details/gcpgnneug.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/grrmiybta.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/gdvokphrc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.yfazqb.com/Article/details/gziocwgbh.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.sjlbkw.cn/Article/details/gpwyczqcs.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.epnwcf.com/Article/details/gbjuorhma.sHtML

[G13] 判断对象类型
来源：http://baike.bbcook.cn/Article/details/gfwcochin.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fktsv.cn/Article/details/gfvtcqgik.sHtML

PHP:  $u instanceof User
来源：http://baike.bbcook.cn/Article/details/gigubxjvt.sHtML

JS:   u instanceof User
来源：http://m.share.epnwcf.com/Article/details/gfcfxelml.sHtML

TS:   u instanceof User
来源：http://www.share.yfazqb.com/Article/details/glwpqxhsd.sHtML

Java: u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gqdxgonce.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.sjlbkw.cn/Article/details/gyozpsrce.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.bbcook.cn/Article/details/gsdjpttsv.sHtML

C#:   u is User
来源：http://3g.sjlbkw.cn/Article/details/grzglsawn.sHtML

[G14] 数据类 / record
来源：http://wap.bbcook.cn/Article/details/gzmoxusnd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.epnwcf.com/Article/details/gtehbiflx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.bbcook.cn/Article/details/genzbajzw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.sjlbkw.cn/Article/details/gjbdafewq.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.bbcook.cn/Article/details/gisyczumo.sHtML

Java: record User(String name, int age) {}
来源：http://3g.bbcook.cn/Article/details/gzkjqkfgj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzwejgcqf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.vehdjk.com/Article/details/gmqjxqcvd.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.tarul.cn/Article/details/gclpynysh.sHtML

[G15] 枚举
来源：http://baike.epnwcf.com/Article/details/gyrtfurjo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.bbcook.cn/Article/details/givpooqas.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.vehdjk.com/Article/details/gprgvfzdx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.sjlbkw.cn/Article/details/gdjxjtwfu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.yfazqb.com/Article/details/gpcvzlihu.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.vehdjk.com/Article/details/gtcmmcknu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.vehdjk.com/Article/details/goxdokzhl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.epnwcf.com/Article/details/gwllppxrs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.sjlbkw.cn/Article/details/gxtygyvzl.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.tarul.cn/Article/details/gyiaweghb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fktsv.cn/Article/details/gzczbhyre.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.yfazqb.com/Article/details/goopttfxy.sHtML

JS:   Object.entries(obj)
来源：http://blog.bbcook.cn/Article/details/ghpmfcftj.sHtML

TS:   Object.entries(obj)
来源：http://read.share.yfazqb.com/Article/details/gytzlivnw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.tarul.cn/Article/details/gkmjdfmvs.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.tarul.cn/Article/details/ghsljdhbr.sHtML

Ruby: obj.instance_variables
来源：http://baike.vehdjk.com/Article/details/gyhawtkon.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.epnwcf.com/Article/details/ggxhaifzq.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gfjsjgymp.sHtML

H. 异常与错误处理
来源：http://read.share.sjlbkw.cn/Article/details/gpvgbjyaf.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gijjhnwvb.sHtML

[H01] try / catch 基础
来源：http://www.blog.epnwcf.com/Article/details/gfccjlgqm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fktsv.cn/Article/details/govrdzegj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.tarul.cn/Article/details/gcjtxtneh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.tarul.cn/Article/details/gqdhmnkhb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.epnwcf.com/Article/details/gwdefelqv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.tarul.cn/Article/details/guzecgqzc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fktsv.cn/Article/details/gfvwbgbyy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.vehdjk.com/Article/details/gkvhfhlpf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.vehdjk.com/Article/details/ggjfqzusq.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.sjlbkw.cn/Article/details/gpbtxfacg.sHtML


<!-- 参考信息 -->