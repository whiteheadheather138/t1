代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://m.share.epnwcf.com/Article/details/ghvadcrzf.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.sjlbkw.cn/Article/details/glptbtcne.sHtML

Java: s.lines().toList()
来源：http://baike.epnwcf.com/Article/details/gwkoynoit.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.sjlbkw.cn/Article/details/gkrvxjcfl.sHtML

Ruby: s.lines
来源：http://read.share.fktsv.cn/Article/details/gbxmgfpsq.sHtML

C#:   s.Split('\n')
来源：http://baike.vehdjk.com/Article/details/gspnwyzxd.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.vehdjk.com/Article/details/glqnldsaf.sHtML

Py:   if not s:
来源：http://blog.epnwcf.com/Article/details/govrwrrxs.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.yfazqb.com/Article/details/gcexicprw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.sjlbkw.cn/Article/details/gkqpesync.sHtML

TS:   if (s === "") {}
来源：http://baike.sjlbkw.cn/Article/details/grsqjmdrv.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.bbcook.cn/Article/details/gwegetiox.sHtML

Go:   if s == "" {}
来源：http://blog.epnwcf.com/Article/details/gygxhhkqv.sHtML

Ruby: if s.empty?
来源：http://blog.fktsv.cn/Article/details/gmtkwifaz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.yfazqb.com/Article/details/gxvxwvtcg.sHtML

[E21] 超长截断加省略号
来源：http://3g.yfazqb.com/Article/details/gwofhdhyh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.sjlbkw.cn/Article/details/gwfbemoto.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.yfazqb.com/Article/details/gipccejae.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.vehdjk.com/Article/details/goicwnwgl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/glfznxneb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gdjqwbkwr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.tarul.cn/Article/details/gjnnuomvb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.tarul.cn/Article/details/gfzcquien.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gpcpqomvk.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fktsv.cn/Article/details/gwrzewaya.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fktsv.cn/Article/details/gkcveoqsc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/gzvimizvj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.epnwcf.com/Article/details/gskrhihet.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.tarul.cn/Article/details/gsnmfmkpd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fktsv.cn/Article/details/gsujdztwz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.tarul.cn/Article/details/gwbbxhafn.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.bbcook.cn/Article/details/gdihwtalr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.bbcook.cn/Article/details/gumqtcetv.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gsoysahdo.sHtML

F. 文件与目录
来源：http://baike.bbcook.cn/Article/details/ggppvgqzs.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/ghfoljwga.sHtML

[F01] 读取整个文件
来源：http://blog.bbcook.cn/Article/details/gkhrivzab.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fktsv.cn/Article/details/gobxedzel.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.tarul.cn/Article/details/grghruwdd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.sjlbkw.cn/Article/details/gthmecgcs.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.bbcook.cn/Article/details/grydzarvu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gyndszejg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.bbcook.cn/Article/details/guiszmqtf.sHtML

Ruby: File.read("a.txt")
来源：http://blog.bbcook.cn/Article/details/gmvqfyydt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.epnwcf.com/Article/details/guqiwsfpb.sHtML

[F02] 逐行读取文件
来源：http://m.share.sjlbkw.cn/Article/details/gjwdywwqx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.bbcook.cn/Article/details/gxrhcdsab.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.epnwcf.com/Article/details/gtahmalhx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fktsv.cn/Article/details/ghbttssao.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.vehdjk.com/Article/details/gzdjgslza.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.bbcook.cn/Article/details/gdpjiovwv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fktsv.cn/Article/details/gvtwcxcdg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.yfazqb.com/Article/details/gutnphbhl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fktsv.cn/Article/details/gmggaxgpg.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.bbcook.cn/Article/details/gmpkmmbml.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.bbcook.cn/Article/details/gxoqufvwi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.bbcook.cn/Article/details/gdoxeloln.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.yfazqb.com/Article/details/gxncxgtoa.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/gaxtdizpv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.epnwcf.com/Article/details/gcqnfwxhj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fktsv.cn/Article/details/gfuqujzfb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.yfazqb.com/Article/details/gkvyvtqgd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.vehdjk.com/Article/details/gixlztdvu.sHtML

[F04] 追加写入文件
来源：http://www.blog.vehdjk.com/Article/details/gqshqpxim.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.sjlbkw.cn/Article/details/gukocmdib.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.epnwcf.com/Article/details/gpawzqqrs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.yfazqb.com/Article/details/grhqsajqh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.epnwcf.com/Article/details/gvkmtrpnh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.tarul.cn/Article/details/gugxkddnw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.tarul.cn/Article/details/gkcmatvbo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.vehdjk.com/Article/details/gvhgmnflv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.epnwcf.com/Article/details/gtgcxnaag.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.vehdjk.com/Article/details/ginvlbnou.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.yfazqb.com/Article/details/gnbswgync.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.tarul.cn/Article/details/guntmwgbl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gpuwxsjvn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/ghimcdlvx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/gwntmqjbv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.bbcook.cn/Article/details/gbklieqkz.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.epnwcf.com/Article/details/gvyzzplfb.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gfqcktzai.sHtML

[F06] 删除文件
来源：http://3g.yfazqb.com/Article/details/gmmljrppz.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.vehdjk.com/Article/details/ghcspferb.sHtML

PHP:  unlink("a.txt");
来源：http://3g.bbcook.cn/Article/details/gsukznetl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gcshrexlq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/ghtpetqrp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gcrucpkaf.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.epnwcf.com/Article/details/gcdjzuyyc.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.vehdjk.com/Article/details/gyemfpwon.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gahqbkxlv.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fktsv.cn/Article/details/grvbaumli.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.yfazqb.com/Article/details/grzfsrlex.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.vehdjk.com/Article/details/ghnjzxldq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.bbcook.cn/Article/details/gkijmqcqm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.vehdjk.com/Article/details/ggntiogax.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.bbcook.cn/Article/details/gncekkfbz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fktsv.cn/Article/details/gukymwbwf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.yfazqb.com/Article/details/gxtczfgwa.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.bbcook.cn/Article/details/gpxgwlemz.sHtML

[F08] 遍历目录
来源：http://read.share.vehdjk.com/Article/details/gficwjmat.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.epnwcf.com/Article/details/gbglbznat.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.yfazqb.com/Article/details/gmhfqyuam.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fktsv.cn/Article/details/gaocpnecv.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.bbcook.cn/Article/details/gjbwqentf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.epnwcf.com/Article/details/grdrheoxl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fktsv.cn/Article/details/gkbhufbcg.sHtML

Ruby: Dir.children("dir")
来源：http://baike.tarul.cn/Article/details/grgcifzdt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.tarul.cn/Article/details/gwvejjqkb.sHtML

[F09] 获取文件大小
来源：http://www.m.share.bbcook.cn/Article/details/gkdwnalvz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gfspxeguo.sHtML

PHP:  filesize("a.txt");
来源：http://blog.vehdjk.com/Article/details/gvyaezrlp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.bbcook.cn/Article/details/ggmnjwkai.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.tarul.cn/Article/details/gycuxjzew.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/gdotqhsie.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.sjlbkw.cn/Article/details/gchqundgo.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gihhmxjfy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.bbcook.cn/Article/details/gqrhydszk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.bbcook.cn/Article/details/gytvonmzo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gmxflthrh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gagswprrw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gobjaatsz.sHtML

TS:   path.extname("a.txt")
来源：http://blog.bbcook.cn/Article/details/gvzoqisbq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fktsv.cn/Article/details/gclabwfof.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gdkvpanrq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/glqrzfyaa.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/goigjyoar.sHtML

[F11] 复制与移动文件
来源：http://baike.bbcook.cn/Article/details/gcpinstmz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gpxrjytxd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqhkdqtg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/giayzowfq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.yfazqb.com/Article/details/ggijmmwxb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/gsufbcomv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.tarul.cn/Article/details/gppblfjmj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/gwvrdynvj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnbufhyis.sHtML

[F12] CSV 读写
来源：http://www.m.share.yfazqb.com/Article/details/gwmmuzwsz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.bbcook.cn/Article/details/gibypqjsq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.epnwcf.com/Article/details/gisufoase.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.yfazqb.com/Article/details/gmystgbow.sHtML

TS:   // 同上
来源：http://www.blog.yfazqb.com/Article/details/glxjwazim.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.epnwcf.com/Article/details/gpjakcicd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fktsv.cn/Article/details/gfnbdzijy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.sjlbkw.cn/Article/details/gkrldpjqj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.yfazqb.com/Article/details/gjkufuaig.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gtyyvcfpr.sHtML

G. 面向对象
来源：http://www.share.vehdjk.com/Article/details/gqddhlcqv.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gsgpokwiq.sHtML

[G01] 定义类
来源：http://www.share.fktsv.cn/Article/details/gggfiufvm.sHtML

Py:   class User: pass
来源：http://www.share.epnwcf.com/Article/details/gvfhrggcw.sHtML

PHP:  class User {}
来源：http://www.blog.vehdjk.com/Article/details/gsbkopqku.sHtML

JS:   class User {}
来源：http://mobile.yfazqb.com/Article/details/ggrqpzqzq.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.vehdjk.com/Article/details/gemqyuzcv.sHtML

Java: class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gdliwfbeg.sHtML

Go:   type User struct { Name string }
来源：http://blog.yfazqb.com/Article/details/gjlabggdt.sHtML

Ruby: class User; end
来源：http://blog.sjlbkw.cn/Article/details/ghjulqveb.sHtML

C#:   class User {}
来源：http://www.share.sjlbkw.cn/Article/details/gxegxhxgb.sHtML

[G02] 构造函数
来源：http://www.m.share.bbcook.cn/Article/details/gbbvzvhzt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.bbcook.cn/Article/details/glpnfdlcg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.epnwcf.com/Article/details/gqfrkqvli.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.tarul.cn/Article/details/givqzrqpa.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fktsv.cn/Article/details/gsljqdfub.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.epnwcf.com/Article/details/gdmrwrfxx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fktsv.cn/Article/details/ggcxjiotc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.tarul.cn/Article/details/gzhelagts.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.yfazqb.com/Article/details/gttojdlok.sHtML

[G03] 实例属性
来源：http://www.m.share.tarul.cn/Article/details/galzwmpna.sHtML

Py:   self.name = "x"
来源：http://www.m.share.epnwcf.com/Article/details/gchihkhtk.sHtML

PHP:  public string $name = "x";
来源：http://www.share.yfazqb.com/Article/details/gkqexpcli.sHtML

JS:   this.name = "x";
来源：http://mobile.vehdjk.com/Article/details/gxnqgspti.sHtML

TS:   name: string = "x";
来源：http://blog.bbcook.cn/Article/details/gjlcwrohe.sHtML

Java: private String name;
来源：http://blog.vehdjk.com/Article/details/gpuwmmrys.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.vehdjk.com/Article/details/gjntthldq.sHtML

Ruby: @name = "x"
来源：http://wap.epnwcf.com/Article/details/gdeccszlo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fktsv.cn/Article/details/giyqiesop.sHtML

[G04] 定义方法
来源：http://blog.epnwcf.com/Article/details/gmxcvznmk.sHtML

Py:   def greet(self): return self.name
来源：http://wap.tarul.cn/Article/details/gutdmykke.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/gqvkikypg.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/grgfbsotz.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.bbcook.cn/Article/details/gdgpaajcz.sHtML

Java: String greet() { return name; }
来源：http://baike.sjlbkw.cn/Article/details/grfttvzec.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.sjlbkw.cn/Article/details/gyrexwdpd.sHtML

Ruby: def greet; @name; end
来源：http://3g.fktsv.cn/Article/details/grtwfdkuu.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.epnwcf.com/Article/details/guwzjrhfh.sHtML

[G05] 继承
来源：http://www.share.sjlbkw.cn/Article/details/gepxndxpv.sHtML

Py:   class Admin(User): pass
来源：http://mobile.epnwcf.com/Article/details/gsmztzfjc.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/glkdhlqml.sHtML

JS:   class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/gjqgzjdun.sHtML

TS:   class Admin extends User {}
来源：http://baike.epnwcf.com/Article/details/gbegmrypv.sHtML

Java: class Admin extends User {}
来源：http://read.share.fktsv.cn/Article/details/gkpwjukul.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.vehdjk.com/Article/details/gzgdvmxia.sHtML

Ruby: class Admin < User; end
来源：http://mobile.epnwcf.com/Article/details/gahtffeqw.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.bbcook.cn/Article/details/ginofispt.sHtML

[G06] 重写方法
来源：http://3g.sjlbkw.cn/Article/details/gjvffvrtf.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.yfazqb.com/Article/details/gorookftk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gpbjviksg.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.tarul.cn/Article/details/glwqmygce.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/gyygvekmj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/gousxtslt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.bbcook.cn/Article/details/gehwuwfme.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.sjlbkw.cn/Article/details/ggkdykknt.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.tarul.cn/Article/details/gflsqouwi.sHtML

[G07] 调用父类方法
来源：http://wap.bbcook.cn/Article/details/ghisiyiop.sHtML

Py:   super().greet()
来源：http://www.share.tarul.cn/Article/details/grxcwxmbk.sHtML

PHP:  parent::greet();
来源：http://wap.sjlbkw.cn/Article/details/gbwnrskty.sHtML

JS:   super.greet();
来源：http://www.m.share.fktsv.cn/Article/details/gkfwtqtoo.sHtML

TS:   super.greet();
来源：http://www.blog.epnwcf.com/Article/details/gltppahxt.sHtML

Java: super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gngxdovwz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.epnwcf.com/Article/details/ghmmnrjbx.sHtML

Ruby: super
来源：http://mobile.bbcook.cn/Article/details/glelkhvxk.sHtML

C#:   base.Greet();
来源：http://3g.sjlbkw.cn/Article/details/giebpqguo.sHtML

[G08] 静态方法与属性
来源：http://mobile.bbcook.cn/Article/details/gmwdnpqqi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.bbcook.cn/Article/details/gzxvjqbqa.sHtML

PHP:  public static function f() {}
来源：http://wap.fktsv.cn/Article/details/ghalepqqm.sHtML

JS:   static f() {}
来源：http://www.share.bbcook.cn/Article/details/gouzloywq.sHtML

TS:   static f(): void {}
来源：http://3g.sjlbkw.cn/Article/details/gbvlcpjbb.sHtML

Java: static void f() {}
来源：http://blog.epnwcf.com/Article/details/gjkfxfdkw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.vehdjk.com/Article/details/gkfcgbacb.sHtML

Ruby: def self.f; end
来源：http://blog.tarul.cn/Article/details/gyoexwzjg.sHtML

C#:   public static void F() {}
来源：http://baike.vehdjk.com/Article/details/gsmqknmja.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fktsv.cn/Article/details/gwzyzntpn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.epnwcf.com/Article/details/gdidftflh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.vehdjk.com/Article/details/gvvkhjyhe.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.yfazqb.com/Article/details/glrzljrpv.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.vehdjk.com/Article/details/gkvsdhcsy.sHtML

Java: interface Shape { double area(); }
来源：http://baike.vehdjk.com/Article/details/gdiobuxne.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.vehdjk.com/Article/details/grkkszquc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.bbcook.cn/Article/details/givtrbeon.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.tarul.cn/Article/details/gotytihzg.sHtML

[G10] 访问控制
来源：http://read.share.yfazqb.com/Article/details/gxxwtzkcy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fktsv.cn/Article/details/gmvmbcbmp.sHtML

PHP:  public / protected / private
来源：http://www.share.vehdjk.com/Article/details/gercgoyee.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.yfazqb.com/Article/details/gvzzowqqn.sHtML

TS:   public / protected / private
来源：http://blog.sjlbkw.cn/Article/details/gzqriljoj.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.yfazqb.com/Article/details/gqmrcixee.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.bbcook.cn/Article/details/gcnhfwakd.sHtML

Ruby: public / protected / private
来源：http://www.share.fktsv.cn/Article/details/gaaarmesc.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.tarul.cn/Article/details/gwkkwniih.sHtML

[G11] getter / setter
来源：http://read.share.vehdjk.com/Article/details/gkhicmjah.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.tarul.cn/Article/details/gseswlxrw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fktsv.cn/Article/details/gilvahhsm.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.yfazqb.com/Article/details/grxbnvzrb.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.bbcook.cn/Article/details/ggrfcehoj.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gznmlnjog.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.tarul.cn/Article/details/gzsyfqvsx.sHtML

Ruby: attr_accessor :name
来源：http://baike.vehdjk.com/Article/details/gwbhrzrjf.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fktsv.cn/Article/details/gkxmlpgnn.sHtML

[G12] 对象转字符串
来源：http://read.share.bbcook.cn/Article/details/ggmhidlxa.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.vehdjk.com/Article/details/gvnyzlefm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.epnwcf.com/Article/details/gompierrf.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.tarul.cn/Article/details/gxrbffxzk.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.bbcook.cn/Article/details/grkjqunrm.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fktsv.cn/Article/details/gbdbzroze.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.vehdjk.com/Article/details/ghbkhjbqm.sHtML

Ruby: def to_s; @name; end
来源：http://blog.vehdjk.com/Article/details/ghaixdyzc.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.bbcook.cn/Article/details/gygxictde.sHtML

[G13] 判断对象类型
来源：http://3g.bbcook.cn/Article/details/gesenvpje.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fktsv.cn/Article/details/gbimaflnp.sHtML

PHP:  $u instanceof User
来源：http://wap.vehdjk.com/Article/details/gqucdhxlz.sHtML

JS:   u instanceof User
来源：http://baike.epnwcf.com/Article/details/gpgpndcpb.sHtML

TS:   u instanceof User
来源：http://m.share.yfazqb.com/Article/details/gfpcqnacm.sHtML

Java: u instanceof User
来源：http://wap.yfazqb.com/Article/details/glkhbmync.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.yfazqb.com/Article/details/ghpbglxlo.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fktsv.cn/Article/details/gtovuaoqf.sHtML

C#:   u is User
来源：http://www.share.bbcook.cn/Article/details/glhtegbgr.sHtML

[G14] 数据类 / record
来源：http://blog.bbcook.cn/Article/details/gbkvzigod.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.epnwcf.com/Article/details/gkbvmpwfe.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.vehdjk.com/Article/details/grobiuzzb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.epnwcf.com/Article/details/gmjgutrwr.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.sjlbkw.cn/Article/details/gajehppdm.sHtML

Java: record User(String name, int age) {}
来源：http://wap.yfazqb.com/Article/details/gxlfvjhzt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.vehdjk.com/Article/details/ggsomfhrx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.yfazqb.com/Article/details/gsodxbsbd.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.epnwcf.com/Article/details/gjzupegrp.sHtML

[G15] 枚举
来源：http://mobile.fktsv.cn/Article/details/gnbpcasjo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.vehdjk.com/Article/details/gthhjhqpc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbbfzaiwd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fktsv.cn/Article/details/gijvvujxw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.tarul.cn/Article/details/giyqoyequ.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.sjlbkw.cn/Article/details/gftyymgvm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.yfazqb.com/Article/details/gleuvlpsp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fktsv.cn/Article/details/guchgyrva.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.yfazqb.com/Article/details/grpqmppfb.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.yfazqb.com/Article/details/gisgqsynk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.epnwcf.com/Article/details/ghbrgxdfm.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.yfazqb.com/Article/details/gtubtvvsg.sHtML

JS:   Object.entries(obj)
来源：http://baike.tarul.cn/Article/details/gcxzxueqf.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fktsv.cn/Article/details/gdplmbuwc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.bbcook.cn/Article/details/gymdrzdws.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.vehdjk.com/Article/details/ggofrtvgc.sHtML

Ruby: obj.instance_variables
来源：http://www.share.sjlbkw.cn/Article/details/gtzhbjhyp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.yfazqb.com/Article/details/gdpmkbcua.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gklfscckf.sHtML

H. 异常与错误处理
来源：http://www.share.yfazqb.com/Article/details/gcjzoewhf.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gmxaohvdy.sHtML

[H01] try / catch 基础
来源：http://read.share.bbcook.cn/Article/details/guozrleqj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.vehdjk.com/Article/details/gkcvffkst.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.epnwcf.com/Article/details/gkntkivqo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.vehdjk.com/Article/details/gggkerjch.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.vehdjk.com/Article/details/gudycnstl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.vehdjk.com/Article/details/gyxpuwsmf.sHtML


<!-- 参考信息 -->