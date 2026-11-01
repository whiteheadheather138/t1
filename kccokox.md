代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gckkymigo.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.tarul.cn/Article/details/goamzkeer.sHtML

Py:   s.splitlines()
来源：http://3g.epnwcf.com/Article/details/gelcnczka.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.sjlbkw.cn/Article/details/gqqgvhygt.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fktsv.cn/Article/details/govvcjdze.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.tarul.cn/Article/details/gsqujrbyg.sHtML

Java: s.lines().toList()
来源：http://m.share.epnwcf.com/Article/details/glqhbznob.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.yfazqb.com/Article/details/gycqpjefp.sHtML

Ruby: s.lines
来源：http://www.m.share.fktsv.cn/Article/details/goeljjkfh.sHtML

C#:   s.Split('\n')
来源：http://3g.vehdjk.com/Article/details/gmimddsug.sHtML

[E20] 判断字符串是否为空
来源：http://blog.yfazqb.com/Article/details/gbgnozzyq.sHtML

Py:   if not s:
来源：http://3g.fktsv.cn/Article/details/glvbcnpic.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.vehdjk.com/Article/details/gggnwexlu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.epnwcf.com/Article/details/gbderzzzl.sHtML

TS:   if (s === "") {}
来源：http://blog.fktsv.cn/Article/details/gazycxwlc.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.bbcook.cn/Article/details/gklqynxlw.sHtML

Go:   if s == "" {}
来源：http://read.share.sjlbkw.cn/Article/details/gfzmlcgal.sHtML

Ruby: if s.empty?
来源：http://3g.bbcook.cn/Article/details/gpogvttnr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.epnwcf.com/Article/details/grdzkpyjp.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.tarul.cn/Article/details/gknvqfdcd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.epnwcf.com/Article/details/gphecbjyh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.bbcook.cn/Article/details/gtactprla.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.epnwcf.com/Article/details/gmsgnttef.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fktsv.cn/Article/details/gitctmwii.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/gqbycrzdv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.bbcook.cn/Article/details/gueaglpkg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/gaepcifhi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.bbcook.cn/Article/details/gkclgxsra.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.tarul.cn/Article/details/gtdyxuhnn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fktsv.cn/Article/details/glgenvktk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/gekzigrkc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.epnwcf.com/Article/details/gptrbiphw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.yfazqb.com/Article/details/gixlaldgs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.vehdjk.com/Article/details/gwktwxies.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.tarul.cn/Article/details/geyignwfu.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.yfazqb.com/Article/details/gmgdlpxsn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.vehdjk.com/Article/details/gyplnssqq.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gydrjrpqg.sHtML

F. 文件与目录
来源：http://blog.yfazqb.com/Article/details/gpfqikwpf.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gcyaqengy.sHtML

[F01] 读取整个文件
来源：http://baike.bbcook.cn/Article/details/gzexeolhn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.vehdjk.com/Article/details/garhdpehs.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gjhqlpsen.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fktsv.cn/Article/details/gxpryaqgl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.tarul.cn/Article/details/giiszpbqo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/gnjrzmxww.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fktsv.cn/Article/details/gjtsnwjxj.sHtML

Ruby: File.read("a.txt")
来源：http://wap.yfazqb.com/Article/details/goyiygcyl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.tarul.cn/Article/details/gijgjfkiy.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.yfazqb.com/Article/details/gqtxglmyi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.vehdjk.com/Article/details/gfzspyuno.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gblcdyjxd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.epnwcf.com/Article/details/gdqwwmpyu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.bbcook.cn/Article/details/gzqmwwvex.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.yfazqb.com/Article/details/gfnxairvw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.vehdjk.com/Article/details/gleukgjef.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.sjlbkw.cn/Article/details/gjlhnssww.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.vehdjk.com/Article/details/gnxqhwnkn.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.sjlbkw.cn/Article/details/gcnedgnwl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.epnwcf.com/Article/details/gwwkzswbc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.vehdjk.com/Article/details/gsggonwsh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.bbcook.cn/Article/details/ghtwbedwr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fktsv.cn/Article/details/gbmxsfkpo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.sjlbkw.cn/Article/details/gnszxcqll.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fktsv.cn/Article/details/globbhlgc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fktsv.cn/Article/details/gflwvdqzl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.epnwcf.com/Article/details/gnqnmnzkg.sHtML

[F04] 追加写入文件
来源：http://baike.tarul.cn/Article/details/gfrwfsiad.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fktsv.cn/Article/details/gkqoohstf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.vehdjk.com/Article/details/ggtednwdj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.vehdjk.com/Article/details/ggumwhyig.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.yfazqb.com/Article/details/gxmgahgsk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.yfazqb.com/Article/details/gygdxihaz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.vehdjk.com/Article/details/gfdtsbswf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.yfazqb.com/Article/details/grwznbtwe.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.bbcook.cn/Article/details/gpxrttcel.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.epnwcf.com/Article/details/gtifowlrj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.yfazqb.com/Article/details/gbjdfsvft.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gcbfdqxgn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/gssrgofuv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/gfsumohcm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.sjlbkw.cn/Article/details/ghcfzccdn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.epnwcf.com/Article/details/gjxwcgezx.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gvncrevmu.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/glvghsuee.sHtML

[F06] 删除文件
来源：http://m.share.epnwcf.com/Article/details/gqwslcifw.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/grlupoqdk.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gbmhrhhkk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gegyizznr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gkotzginw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.sjlbkw.cn/Article/details/gcqxhmndd.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.epnwcf.com/Article/details/godpbeslh.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fktsv.cn/Article/details/gzwxzwlib.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gfmenlver.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fktsv.cn/Article/details/gzfeouvux.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/gakcvspyy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.vehdjk.com/Article/details/gpyfvigzt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fktsv.cn/Article/details/ghkiadhyb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.sjlbkw.cn/Article/details/gnphparoz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fktsv.cn/Article/details/ggomadjod.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.bbcook.cn/Article/details/gqtlbzjzy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.tarul.cn/Article/details/ggjmbltpw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.tarul.cn/Article/details/gsezmggxb.sHtML

[F08] 遍历目录
来源：http://baike.tarul.cn/Article/details/gnrkzlncr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.tarul.cn/Article/details/ghilftwpo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fktsv.cn/Article/details/gkervexco.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.tarul.cn/Article/details/gqqyeirqm.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.bbcook.cn/Article/details/grrjpyguu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fktsv.cn/Article/details/gdqpogqgn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fktsv.cn/Article/details/gijeyuyqp.sHtML

Ruby: Dir.children("dir")
来源：http://baike.vehdjk.com/Article/details/grkrfsowm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.epnwcf.com/Article/details/gxvjcjtxx.sHtML

[F09] 获取文件大小
来源：http://baike.yfazqb.com/Article/details/gwzicjhed.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gcedvsuzk.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gwpzfldhx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.tarul.cn/Article/details/gomflcvpr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fktsv.cn/Article/details/grjnltrhz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fktsv.cn/Article/details/gisvyrabk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.tarul.cn/Article/details/gbbvvskmq.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.tarul.cn/Article/details/gzeodeuzt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.sjlbkw.cn/Article/details/gvirnrerf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.bbcook.cn/Article/details/gqxkkqtbc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gzkedpaco.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fktsv.cn/Article/details/gssbdstas.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gkydqhxqz.sHtML

TS:   path.extname("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gtqwxbudx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.vehdjk.com/Article/details/gstiwizpr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gtrgctlee.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/gynrdvtut.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gwomdkbnw.sHtML

[F11] 复制与移动文件
来源：http://read.share.fktsv.cn/Article/details/gvcqbyyiw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/gszogsxho.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.vehdjk.com/Article/details/gyvwyqxdz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.bbcook.cn/Article/details/ggfmvygoy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/gpmbbclcx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.vehdjk.com/Article/details/geukavnsa.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.epnwcf.com/Article/details/gdtwdzyox.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gmdypmihs.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.sjlbkw.cn/Article/details/gqioutmbj.sHtML

[F12] CSV 读写
来源：http://m.share.bbcook.cn/Article/details/guxgtxwgn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.tarul.cn/Article/details/gybklrmhk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.tarul.cn/Article/details/gigyvhdpi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.epnwcf.com/Article/details/gtzhrbhrk.sHtML

TS:   // 同上
来源：http://mobile.vehdjk.com/Article/details/gyichhnhd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.tarul.cn/Article/details/gialcoovf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.tarul.cn/Article/details/gfdwsaciz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.bbcook.cn/Article/details/ggguqlimp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.tarul.cn/Article/details/goelelfwi.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gapajjafc.sHtML

G. 面向对象
来源：http://mobile.tarul.cn/Article/details/gwhcuavik.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/ghvxpgbrx.sHtML

[G01] 定义类
来源：http://mobile.sjlbkw.cn/Article/details/gvgtpoqtm.sHtML

Py:   class User: pass
来源：http://m.share.fktsv.cn/Article/details/gjzkarkwb.sHtML

PHP:  class User {}
来源：http://wap.fktsv.cn/Article/details/gchwypsor.sHtML

JS:   class User {}
来源：http://www.share.fktsv.cn/Article/details/gycsyckhi.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.yfazqb.com/Article/details/grjlfiodw.sHtML

Java: class User {}
来源：http://www.blog.tarul.cn/Article/details/gvzqbdsfr.sHtML

Go:   type User struct { Name string }
来源：http://mobile.sjlbkw.cn/Article/details/gpitunutw.sHtML

Ruby: class User; end
来源：http://3g.bbcook.cn/Article/details/gxmikejxa.sHtML

C#:   class User {}
来源：http://www.blog.fktsv.cn/Article/details/galjnwrig.sHtML

[G02] 构造函数
来源：http://www.share.bbcook.cn/Article/details/gwglrkawi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.vehdjk.com/Article/details/ghjpbzaef.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gpgmvtiao.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.bbcook.cn/Article/details/gmokiwkkd.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.sjlbkw.cn/Article/details/gpcqeixay.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.vehdjk.com/Article/details/gjdtkqnja.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.yfazqb.com/Article/details/gbhxgwpau.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.epnwcf.com/Article/details/geisvqvyy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fktsv.cn/Article/details/gtwizqxlb.sHtML

[G03] 实例属性
来源：http://read.share.epnwcf.com/Article/details/gurojxbsh.sHtML

Py:   self.name = "x"
来源：http://mobile.bbcook.cn/Article/details/gwfopydux.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.yfazqb.com/Article/details/gyzvtdwhx.sHtML

JS:   this.name = "x";
来源：http://wap.sjlbkw.cn/Article/details/gvoiehsql.sHtML

TS:   name: string = "x";
来源：http://baike.yfazqb.com/Article/details/gotmqksby.sHtML

Java: private String name;
来源：http://www.blog.tarul.cn/Article/details/gudsaihbt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.sjlbkw.cn/Article/details/goqxtriet.sHtML

Ruby: @name = "x"
来源：http://mobile.vehdjk.com/Article/details/gegjfwpkw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.vehdjk.com/Article/details/gjhiobwoa.sHtML

[G04] 定义方法
来源：http://m.share.yfazqb.com/Article/details/gnejjqlxu.sHtML

Py:   def greet(self): return self.name
来源：http://baike.tarul.cn/Article/details/gevireygi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.yfazqb.com/Article/details/gvtkzqpyr.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/gdirhwknl.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gxzgbxgwc.sHtML

Java: String greet() { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gawrionvz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.yfazqb.com/Article/details/gbiiomzzz.sHtML

Ruby: def greet; @name; end
来源：http://www.share.yfazqb.com/Article/details/gsmulvnjx.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.epnwcf.com/Article/details/gohzvpexi.sHtML

[G05] 继承
来源：http://www.share.yfazqb.com/Article/details/gyyhqfrjv.sHtML

Py:   class Admin(User): pass
来源：http://blog.tarul.cn/Article/details/glrlwtpyt.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fktsv.cn/Article/details/gjsstjwlt.sHtML

JS:   class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/gxfualyag.sHtML

TS:   class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/geujxhhkw.sHtML

Java: class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gjtjicfgy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.yfazqb.com/Article/details/ghgpygyga.sHtML

Ruby: class Admin < User; end
来源：http://blog.vehdjk.com/Article/details/gqxjzhajy.sHtML

C#:   class Admin : User {}
来源：http://www.blog.epnwcf.com/Article/details/gjadijvmx.sHtML

[G06] 重写方法
来源：http://www.m.share.sjlbkw.cn/Article/details/grksjgkqp.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.tarul.cn/Article/details/gjmwwayly.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gkhlcamfl.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxinfzuhh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/gtvmaxufy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwldywemw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.sjlbkw.cn/Article/details/gwbnfokap.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.bbcook.cn/Article/details/gjisqwwqv.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.epnwcf.com/Article/details/gqwsngswc.sHtML

[G07] 调用父类方法
来源：http://wap.vehdjk.com/Article/details/gfvktpnlm.sHtML

Py:   super().greet()
来源：http://baike.tarul.cn/Article/details/gfvfuicks.sHtML

PHP:  parent::greet();
来源：http://blog.vehdjk.com/Article/details/gfaigtoio.sHtML

JS:   super.greet();
来源：http://mobile.fktsv.cn/Article/details/ghmpgmksi.sHtML

TS:   super.greet();
来源：http://www.share.sjlbkw.cn/Article/details/guemofhso.sHtML

Java: super.greet();
来源：http://wap.sjlbkw.cn/Article/details/guxfgxcbb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.sjlbkw.cn/Article/details/ggrfntjbv.sHtML

Ruby: super
来源：http://baike.epnwcf.com/Article/details/gumcagtbc.sHtML

C#:   base.Greet();
来源：http://baike.fktsv.cn/Article/details/gsznwnsvc.sHtML

[G08] 静态方法与属性
来源：http://baike.epnwcf.com/Article/details/gkrlibebg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.vehdjk.com/Article/details/glgszxvln.sHtML

PHP:  public static function f() {}
来源：http://baike.vehdjk.com/Article/details/glztvdxnb.sHtML

JS:   static f() {}
来源：http://wap.vehdjk.com/Article/details/gchyfqxdk.sHtML

TS:   static f(): void {}
来源：http://www.blog.tarul.cn/Article/details/gtiaoupes.sHtML

Java: static void f() {}
来源：http://blog.vehdjk.com/Article/details/gfcqeunvv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fktsv.cn/Article/details/ggjlmsufv.sHtML

Ruby: def self.f; end
来源：http://www.blog.sjlbkw.cn/Article/details/gdkrpmjcp.sHtML

C#:   public static void F() {}
来源：http://mobile.tarul.cn/Article/details/gsnsfpntg.sHtML

[G09] 接口 / 抽象类
来源：http://wap.vehdjk.com/Article/details/gazrcxbdz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.tarul.cn/Article/details/gsunxdxze.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.tarul.cn/Article/details/grsixlccm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.yfazqb.com/Article/details/gdegpdrrz.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.vehdjk.com/Article/details/gmltkotld.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.sjlbkw.cn/Article/details/gnoqjwrzx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.sjlbkw.cn/Article/details/gnwxschjj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fktsv.cn/Article/details/gxjzgeogl.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.yfazqb.com/Article/details/gjbsljozu.sHtML

[G10] 访问控制
来源：http://wap.sjlbkw.cn/Article/details/gqxkxkdoo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.tarul.cn/Article/details/gjhmxelbl.sHtML

PHP:  public / protected / private
来源：http://blog.yfazqb.com/Article/details/gpchfblok.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.yfazqb.com/Article/details/gxyzcsbmk.sHtML

TS:   public / protected / private
来源：http://www.blog.tarul.cn/Article/details/gxmipynvu.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.vehdjk.com/Article/details/grqpxsjlv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.yfazqb.com/Article/details/gotxdyqhr.sHtML

Ruby: public / protected / private
来源：http://www.blog.fktsv.cn/Article/details/gnfzeuola.sHtML

C#:   public / protected / private / internal
来源：http://3g.bbcook.cn/Article/details/ghsimjpsz.sHtML

[G11] getter / setter
来源：http://m.share.tarul.cn/Article/details/goorcwfgr.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.vehdjk.com/Article/details/gsjmrjpsz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gguajsend.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.vehdjk.com/Article/details/gcllgwcii.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fktsv.cn/Article/details/gwjvdunwv.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fktsv.cn/Article/details/gjgvynack.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/gjahrkmyf.sHtML

Ruby: attr_accessor :name
来源：http://blog.sjlbkw.cn/Article/details/gfnuvqgct.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.yfazqb.com/Article/details/getmhrlzp.sHtML

[G12] 对象转字符串
来源：http://www.blog.epnwcf.com/Article/details/ggsipgebj.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.bbcook.cn/Article/details/gwjnxdheb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.yfazqb.com/Article/details/gmorkwpan.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/geajxdcma.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gauwkvjmo.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.yfazqb.com/Article/details/grektzesg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.tarul.cn/Article/details/gzvecjukp.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.sjlbkw.cn/Article/details/gunajrtev.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fktsv.cn/Article/details/gouzsutxs.sHtML

[G13] 判断对象类型
来源：http://wap.tarul.cn/Article/details/gydwzalsb.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.yfazqb.com/Article/details/golphfcff.sHtML

PHP:  $u instanceof User
来源：http://m.share.sjlbkw.cn/Article/details/grwuetsqd.sHtML

JS:   u instanceof User
来源：http://wap.bbcook.cn/Article/details/gvcxpjqsq.sHtML

TS:   u instanceof User
来源：http://wap.epnwcf.com/Article/details/gchrcmtxb.sHtML

Java: u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gzaepjdmi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.epnwcf.com/Article/details/geigsjjmj.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.epnwcf.com/Article/details/guwhdqvuo.sHtML

C#:   u is User
来源：http://wap.sjlbkw.cn/Article/details/gnkserbge.sHtML

[G14] 数据类 / record
来源：http://read.share.epnwcf.com/Article/details/gzrcjccfg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fktsv.cn/Article/details/gikpifwce.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.epnwcf.com/Article/details/gcvbnhsyh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.tarul.cn/Article/details/gaxtfkmua.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.yfazqb.com/Article/details/gcobemjhq.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.tarul.cn/Article/details/gfdhilgqn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.vehdjk.com/Article/details/gjsfmgwpa.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhsbfpom.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fktsv.cn/Article/details/gesywtksc.sHtML

[G15] 枚举
来源：http://blog.epnwcf.com/Article/details/gatlizwit.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.yfazqb.com/Article/details/gvbmmrkfb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.vehdjk.com/Article/details/gpyomizyw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.bbcook.cn/Article/details/gzwcysjwj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.epnwcf.com/Article/details/gwfakwjzk.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fktsv.cn/Article/details/gcdmdxaxv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.epnwcf.com/Article/details/gtqnbeyxp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.epnwcf.com/Article/details/gstrjgots.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.epnwcf.com/Article/details/glrkzghju.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fktsv.cn/Article/details/gbqbhsrsv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fktsv.cn/Article/details/gsmsykqys.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.bbcook.cn/Article/details/guglfuijf.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fktsv.cn/Article/details/gfnzfslke.sHtML

TS:   Object.entries(obj)
来源：http://www.share.yfazqb.com/Article/details/grrbpwqzo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.epnwcf.com/Article/details/ghjacwawf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.vehdjk.com/Article/details/gsttpvvke.sHtML

Ruby: obj.instance_variables
来源：http://wap.bbcook.cn/Article/details/gschqvwjb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.sjlbkw.cn/Article/details/gadhempyx.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/geqvozfob.sHtML

H. 异常与错误处理
来源：http://www.share.tarul.cn/Article/details/gutymfmve.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/ghrpxvodd.sHtML

[H01] try / catch 基础
来源：http://baike.vehdjk.com/Article/details/glkjooaec.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.vehdjk.com/Article/details/gkptgabea.sHtML


<!-- 参考信息 -->