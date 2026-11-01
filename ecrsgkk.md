代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.tarul.cn/Article/details/gmjomnymm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fktsv.cn/Article/details/gpzslxydk.sHtML

TS:   if (s === "") {}
来源：http://mobile.tarul.cn/Article/details/gumvyulbj.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.epnwcf.com/Article/details/ghaggveed.sHtML

Go:   if s == "" {}
来源：http://blog.fktsv.cn/Article/details/gsmpvacsf.sHtML

Ruby: if s.empty?
来源：http://mobile.sjlbkw.cn/Article/details/gnyiqnuad.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.epnwcf.com/Article/details/glqipngku.sHtML

[E21] 超长截断加省略号
来源：http://mobile.bbcook.cn/Article/details/gsymfpgxr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.epnwcf.com/Article/details/gjntkxhme.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/gdjokghjo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/gnqkxswwb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.epnwcf.com/Article/details/gciqrbyob.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gugifrbay.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fktsv.cn/Article/details/gqqulijya.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.yfazqb.com/Article/details/gcprhqhxn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.yfazqb.com/Article/details/gpledjtfy.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.bbcook.cn/Article/details/ggthpursv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.vehdjk.com/Article/details/gorprdhwy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/gbpmtpwyx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.epnwcf.com/Article/details/giqffirlc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fktsv.cn/Article/details/grlobojgc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.epnwcf.com/Article/details/gybgykeah.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.tarul.cn/Article/details/gnxnglkuj.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.sjlbkw.cn/Article/details/gkduknrjd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.bbcook.cn/Article/details/gabedlbeh.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gfvbaggff.sHtML

F. 文件与目录
来源：http://www.share.bbcook.cn/Article/details/gsrwuferd.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gonbjqypb.sHtML

[F01] 读取整个文件
来源：http://www.share.tarul.cn/Article/details/gfcligcay.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.tarul.cn/Article/details/glnqejvrk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/genyivfli.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.vehdjk.com/Article/details/giljmiqdb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.epnwcf.com/Article/details/girzmndsy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/grwadqlbv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.tarul.cn/Article/details/gnpgaaayv.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gjkgcamzq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.tarul.cn/Article/details/gccypuial.sHtML

[F02] 逐行读取文件
来源：http://mobile.vehdjk.com/Article/details/gcavuczmc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fktsv.cn/Article/details/gltbonloq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.bbcook.cn/Article/details/glnqwperj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.sjlbkw.cn/Article/details/grrlezdus.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.vehdjk.com/Article/details/gvcloirvy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.epnwcf.com/Article/details/genrwvfsr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.yfazqb.com/Article/details/gudivupbi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.yfazqb.com/Article/details/glilztigq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.tarul.cn/Article/details/ghsfyekgw.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.epnwcf.com/Article/details/gyekneomf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fktsv.cn/Article/details/gqrwwavju.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.vehdjk.com/Article/details/gzqhdsutf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fktsv.cn/Article/details/gjiqdtvum.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.tarul.cn/Article/details/gekjzlljk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.sjlbkw.cn/Article/details/gqzrmkude.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.bbcook.cn/Article/details/gpamuhyiq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjpxcqkb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.bbcook.cn/Article/details/gnyxtvdci.sHtML

[F04] 追加写入文件
来源：http://read.share.fktsv.cn/Article/details/gfrhkifrm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.bbcook.cn/Article/details/giqrseuvz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.sjlbkw.cn/Article/details/ghlmsqizq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.tarul.cn/Article/details/goqlzwneb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.epnwcf.com/Article/details/gaajbgsrb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.vehdjk.com/Article/details/gnpkkjdys.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.sjlbkw.cn/Article/details/gctuzcwuo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.tarul.cn/Article/details/gyyuyezsk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.yfazqb.com/Article/details/geketeupo.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.vehdjk.com/Article/details/gsgcfosfy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.vehdjk.com/Article/details/gexjsiusd.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.bbcook.cn/Article/details/gbalrkhnh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gdiemypft.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gnysosfef.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/gitfdlhmq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.sjlbkw.cn/Article/details/gpvuhzrvw.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.tarul.cn/Article/details/gfiibvpwt.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gsbvgpdvc.sHtML

[F06] 删除文件
来源：http://www.share.tarul.cn/Article/details/gvhxgmmpx.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fktsv.cn/Article/details/ggpfzqqca.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gfkfasxhh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/guauyesdm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.vehdjk.com/Article/details/gorfpxdtf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/gndbriylf.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.vehdjk.com/Article/details/ghtqgfumq.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gliionhih.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.epnwcf.com/Article/details/gnftdqxwn.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.yfazqb.com/Article/details/gqsfwsjxf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.epnwcf.com/Article/details/gyksaswrs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.tarul.cn/Article/details/gxqvvlcfh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.epnwcf.com/Article/details/ghkfjimap.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.tarul.cn/Article/details/gbloptcuv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.tarul.cn/Article/details/geekssdkl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.bbcook.cn/Article/details/gesnewnbv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.tarul.cn/Article/details/gyefjuafo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.vehdjk.com/Article/details/ghjtxrntz.sHtML

[F08] 遍历目录
来源：http://m.share.bbcook.cn/Article/details/gxjslckfc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.tarul.cn/Article/details/gabhirnrq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.epnwcf.com/Article/details/gafzttihb.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.tarul.cn/Article/details/grpufzrha.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.yfazqb.com/Article/details/gjjuysvue.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.sjlbkw.cn/Article/details/guokxssun.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gggnvhalt.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.epnwcf.com/Article/details/grjtuifaz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.sjlbkw.cn/Article/details/gtzkavuyo.sHtML

[F09] 获取文件大小
来源：http://mobile.fktsv.cn/Article/details/gkeoxikxc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gulqrhijv.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.tarul.cn/Article/details/gpixwjzrw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.bbcook.cn/Article/details/gcrrbpwrb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.yfazqb.com/Article/details/gmcnbyzgr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/gdpismsbt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.bbcook.cn/Article/details/gnvqiqyjz.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.tarul.cn/Article/details/gzhgbvafa.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.sjlbkw.cn/Article/details/gbzhdnsyi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.epnwcf.com/Article/details/gtnxxewyw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/geovotldh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.bbcook.cn/Article/details/gqxfdgsne.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gzgqkmoos.sHtML

TS:   path.extname("a.txt")
来源：http://blog.tarul.cn/Article/details/godurlags.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.tarul.cn/Article/details/gjpbzfgwz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gjmaqdama.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/gnzdezgbz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gaebqelxe.sHtML

[F11] 复制与移动文件
来源：http://m.share.bbcook.cn/Article/details/gvroqjzaw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/giatqsbzf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fktsv.cn/Article/details/gqqeubvwk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.epnwcf.com/Article/details/gdilfgfww.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.vehdjk.com/Article/details/grzgnppmb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.vehdjk.com/Article/details/gahidijta.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fktsv.cn/Article/details/grgethvam.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/gicbulyae.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.sjlbkw.cn/Article/details/gtdqeilqd.sHtML

[F12] CSV 读写
来源：http://www.share.vehdjk.com/Article/details/gqapwepod.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.bbcook.cn/Article/details/gwgkmlfaa.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.tarul.cn/Article/details/gcjsplbdn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.sjlbkw.cn/Article/details/gbmqtvweb.sHtML

TS:   // 同上
来源：http://3g.yfazqb.com/Article/details/gehcdjaea.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.tarul.cn/Article/details/ghslxcyao.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.yfazqb.com/Article/details/gzvsihbuu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.tarul.cn/Article/details/gjfjydtun.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.bbcook.cn/Article/details/gnvlxengn.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gjhiyeqxu.sHtML

G. 面向对象
来源：http://mobile.yfazqb.com/Article/details/glpggvwvf.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/guatjrmev.sHtML

[G01] 定义类
来源：http://3g.epnwcf.com/Article/details/gngzwcxyr.sHtML

Py:   class User: pass
来源：http://read.share.vehdjk.com/Article/details/gazagkqhc.sHtML

PHP:  class User {}
来源：http://m.share.sjlbkw.cn/Article/details/gatsgepfm.sHtML

JS:   class User {}
来源：http://www.share.epnwcf.com/Article/details/gkdqjkppd.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbggmuzdv.sHtML

Java: class User {}
来源：http://wap.sjlbkw.cn/Article/details/guzxmwcmo.sHtML

Go:   type User struct { Name string }
来源：http://wap.fktsv.cn/Article/details/gvshawnbl.sHtML

Ruby: class User; end
来源：http://www.share.fktsv.cn/Article/details/gddrvodig.sHtML

C#:   class User {}
来源：http://baike.yfazqb.com/Article/details/gxmanbrvb.sHtML

[G02] 构造函数
来源：http://www.m.share.epnwcf.com/Article/details/gisgyyfou.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.tarul.cn/Article/details/glwgtjfeh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.epnwcf.com/Article/details/gqohiievz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fktsv.cn/Article/details/gexvtvbwe.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.epnwcf.com/Article/details/gnifoqbsi.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fktsv.cn/Article/details/gktzaabaa.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.sjlbkw.cn/Article/details/gatnjtiqg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.bbcook.cn/Article/details/gllpbiiff.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.bbcook.cn/Article/details/gnhetabov.sHtML

[G03] 实例属性
来源：http://read.share.tarul.cn/Article/details/gjqvybefu.sHtML

Py:   self.name = "x"
来源：http://www.share.vehdjk.com/Article/details/gnqqugedh.sHtML

PHP:  public string $name = "x";
来源：http://wap.yfazqb.com/Article/details/gyorputse.sHtML

JS:   this.name = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gpcnogiat.sHtML

TS:   name: string = "x";
来源：http://mobile.bbcook.cn/Article/details/gvvcwanww.sHtML

Java: private String name;
来源：http://wap.sjlbkw.cn/Article/details/ggbjgmqxl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.epnwcf.com/Article/details/gphdsjtoh.sHtML

Ruby: @name = "x"
来源：http://m.share.bbcook.cn/Article/details/gdkqdepng.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.vehdjk.com/Article/details/gnarugpyd.sHtML

[G04] 定义方法
来源：http://read.share.yfazqb.com/Article/details/gnkqwlasl.sHtML

Py:   def greet(self): return self.name
来源：http://3g.epnwcf.com/Article/details/gjswnheya.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.epnwcf.com/Article/details/gdgylgtka.sHtML

JS:   greet() { return this.name; }
来源：http://3g.epnwcf.com/Article/details/grltchjvs.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/gpfanepzs.sHtML

Java: String greet() { return name; }
来源：http://baike.fktsv.cn/Article/details/gezqgaymc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.yfazqb.com/Article/details/gsiokhwkw.sHtML

Ruby: def greet; @name; end
来源：http://m.share.sjlbkw.cn/Article/details/gcvcknhoa.sHtML

C#:   public string Greet() => Name;
来源：http://3g.bbcook.cn/Article/details/gvdwwhaac.sHtML

[G05] 继承
来源：http://baike.sjlbkw.cn/Article/details/gmhlqkrat.sHtML

Py:   class Admin(User): pass
来源：http://mobile.sjlbkw.cn/Article/details/gjukqyuzg.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.epnwcf.com/Article/details/geclzdptb.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/gpuckpchz.sHtML

TS:   class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/ggovxhgro.sHtML

Java: class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/gggbxewrp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.sjlbkw.cn/Article/details/ggsigbwii.sHtML

Ruby: class Admin < User; end
来源：http://mobile.vehdjk.com/Article/details/gfghudvfb.sHtML

C#:   class Admin : User {}
来源：http://3g.vehdjk.com/Article/details/guqulebfo.sHtML

[G06] 重写方法
来源：http://www.share.yfazqb.com/Article/details/gpgzifqaa.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.tarul.cn/Article/details/giwnmlrfb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/gzdnxjajb.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gmqazamip.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/ghfrmozsj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gcsahhdbh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.sjlbkw.cn/Article/details/gsqebognp.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.yfazqb.com/Article/details/gtnguygat.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.sjlbkw.cn/Article/details/gbygmafjj.sHtML

[G07] 调用父类方法
来源：http://read.share.vehdjk.com/Article/details/gzzrkawll.sHtML

Py:   super().greet()
来源：http://www.m.share.epnwcf.com/Article/details/gueqmhqha.sHtML

PHP:  parent::greet();
来源：http://read.share.fktsv.cn/Article/details/ggacqxsjr.sHtML

JS:   super.greet();
来源：http://3g.bbcook.cn/Article/details/glwnhwryv.sHtML

TS:   super.greet();
来源：http://3g.sjlbkw.cn/Article/details/gqutnmplu.sHtML

Java: super.greet();
来源：http://read.share.yfazqb.com/Article/details/gvkjzyzoo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fktsv.cn/Article/details/gbejtfoyr.sHtML

Ruby: super
来源：http://wap.fktsv.cn/Article/details/ggxnbdveq.sHtML

C#:   base.Greet();
来源：http://read.share.fktsv.cn/Article/details/gassegvgw.sHtML

[G08] 静态方法与属性
来源：http://m.share.fktsv.cn/Article/details/gqcpxzfdq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.vehdjk.com/Article/details/ggnpojtjr.sHtML

PHP:  public static function f() {}
来源：http://m.share.fktsv.cn/Article/details/glkxltlir.sHtML

JS:   static f() {}
来源：http://wap.vehdjk.com/Article/details/gbufiflbb.sHtML

TS:   static f(): void {}
来源：http://baike.vehdjk.com/Article/details/gmvldlmvm.sHtML

Java: static void f() {}
来源：http://m.share.sjlbkw.cn/Article/details/gvrhtlizy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.sjlbkw.cn/Article/details/gjfryqdoh.sHtML

Ruby: def self.f; end
来源：http://www.m.share.tarul.cn/Article/details/gbmtngirq.sHtML

C#:   public static void F() {}
来源：http://baike.bbcook.cn/Article/details/glzgntzlm.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.sjlbkw.cn/Article/details/gbuuhclkg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fktsv.cn/Article/details/gggyeacfu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.tarul.cn/Article/details/grkjhsbky.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.bbcook.cn/Article/details/gixrmhxzf.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.epnwcf.com/Article/details/gqpcbpswu.sHtML

Java: interface Shape { double area(); }
来源：http://baike.vehdjk.com/Article/details/gbihjavxe.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fktsv.cn/Article/details/gwzvaxudh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.epnwcf.com/Article/details/glxbianul.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.vehdjk.com/Article/details/ggicxtyxc.sHtML

[G10] 访问控制
来源：http://www.m.share.bbcook.cn/Article/details/gvqzemgrb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fktsv.cn/Article/details/guaophaoo.sHtML

PHP:  public / protected / private
来源：http://3g.bbcook.cn/Article/details/ghsevzsjs.sHtML

JS:   #private 字段；其余公开
来源：http://wap.yfazqb.com/Article/details/gfzsgussm.sHtML

TS:   public / protected / private
来源：http://blog.sjlbkw.cn/Article/details/gcciopxmd.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fktsv.cn/Article/details/gzibuozsm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.yfazqb.com/Article/details/ghidkzyzo.sHtML

Ruby: public / protected / private
来源：http://www.m.share.sjlbkw.cn/Article/details/gynmxhfvv.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.bbcook.cn/Article/details/gijfjnpmi.sHtML

[G11] getter / setter
来源：http://3g.vehdjk.com/Article/details/gfubqhalx.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fktsv.cn/Article/details/glvdojgoj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.sjlbkw.cn/Article/details/gkzkbacty.sHtML

JS:   get name() { return this._name; }
来源：http://wap.sjlbkw.cn/Article/details/geklzpblu.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.vehdjk.com/Article/details/gqivqdnpr.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fktsv.cn/Article/details/gonhtjqwu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.tarul.cn/Article/details/gabhrfvsd.sHtML

Ruby: attr_accessor :name
来源：http://read.share.epnwcf.com/Article/details/gfnhnekjp.sHtML

C#:   public string Name { get; set; }
来源：http://wap.sjlbkw.cn/Article/details/ggdoeccag.sHtML

[G12] 对象转字符串
来源：http://www.share.bbcook.cn/Article/details/glsgxmrpm.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.sjlbkw.cn/Article/details/gkicyoufj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.bbcook.cn/Article/details/gpoktkutr.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.bbcook.cn/Article/details/gdtueexms.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gefummofc.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gumkqmbhl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/ghfpgierz.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.bbcook.cn/Article/details/gyodvmeuo.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.epnwcf.com/Article/details/gnxccwbne.sHtML

[G13] 判断对象类型
来源：http://3g.bbcook.cn/Article/details/gpaysobcm.sHtML

Py:   isinstance(u, User)
来源：http://wap.bbcook.cn/Article/details/gldoedndk.sHtML

PHP:  $u instanceof User
来源：http://3g.bbcook.cn/Article/details/gxerxavxs.sHtML

JS:   u instanceof User
来源：http://www.m.share.yfazqb.com/Article/details/gebibhagh.sHtML

TS:   u instanceof User
来源：http://wap.vehdjk.com/Article/details/gzzunpdtc.sHtML

Java: u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/glqsvzxkb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.vehdjk.com/Article/details/geijdegnd.sHtML

Ruby: u.is_a?(User)
来源：http://wap.vehdjk.com/Article/details/grtszrvem.sHtML

C#:   u is User
来源：http://baike.sjlbkw.cn/Article/details/gptiuiufg.sHtML

[G14] 数据类 / record
来源：http://mobile.fktsv.cn/Article/details/gjvhujsge.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.tarul.cn/Article/details/gkaqonbut.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.yfazqb.com/Article/details/gsghwmije.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.bbcook.cn/Article/details/gdjlnyhen.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fktsv.cn/Article/details/gothahgvh.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fktsv.cn/Article/details/gxuzmlgos.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.vehdjk.com/Article/details/gnvdodrsa.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fktsv.cn/Article/details/gxgdssrwl.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fktsv.cn/Article/details/gechwrfia.sHtML

[G15] 枚举
来源：http://baike.epnwcf.com/Article/details/gdykvhcnb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.sjlbkw.cn/Article/details/gvqpqlukw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.vehdjk.com/Article/details/gpjpzxabr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.tarul.cn/Article/details/grrjurzyt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcwklmiaa.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.vehdjk.com/Article/details/glgkmxkpz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.bbcook.cn/Article/details/gbckmrwkq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.vehdjk.com/Article/details/gzwtigipj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gidsejjso.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.bbcook.cn/Article/details/gduqoyeid.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.epnwcf.com/Article/details/gwjnldiml.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.sjlbkw.cn/Article/details/gosctsjgo.sHtML

JS:   Object.entries(obj)
来源：http://blog.bbcook.cn/Article/details/gforssbab.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.vehdjk.com/Article/details/gxyrdzjmp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.vehdjk.com/Article/details/gokdtiqgh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.vehdjk.com/Article/details/gtminbwgr.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.bbcook.cn/Article/details/gticdchek.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.epnwcf.com/Article/details/gzennvrhx.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gfxbixfve.sHtML

H. 异常与错误处理
来源：http://mobile.fktsv.cn/Article/details/gttucoeqj.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gladlmmnl.sHtML

[H01] try / catch 基础
来源：http://wap.sjlbkw.cn/Article/details/gfgnloswu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.tarul.cn/Article/details/gizbyjiex.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.yfazqb.com/Article/details/gsftheyte.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.bbcook.cn/Article/details/gijkiausn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fktsv.cn/Article/details/gwoxgzney.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.tarul.cn/Article/details/giyzwhwdq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.epnwcf.com/Article/details/gpdbawxmc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.sjlbkw.cn/Article/details/goivyvmba.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.tarul.cn/Article/details/gshxaccua.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.yfazqb.com/Article/details/gibhxqqlm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.bbcook.cn/Article/details/ghxfayfoh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gdoiscatd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/ghrahcgcr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gpeeeutyj.sHtML


<!-- 参考信息 -->