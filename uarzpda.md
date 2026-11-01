代发 wailian999

Go:   if s == "" {}
来源：http://blog.sjlbkw.cn/Article/details/gygnrohiw.sHtML

Ruby: if s.empty?
来源：http://baike.epnwcf.com/Article/details/gkbfvrhip.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.epnwcf.com/Article/details/gizklukcr.sHtML

[E21] 超长截断加省略号
来源：http://3g.yfazqb.com/Article/details/gcszedylm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.tarul.cn/Article/details/gricphsbx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.yfazqb.com/Article/details/gspiievsb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.yfazqb.com/Article/details/gdaizjxnp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/gvgvxxbdr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/gvxdzcwkf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.tarul.cn/Article/details/glthmhzoe.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.bbcook.cn/Article/details/gobiklxvd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.epnwcf.com/Article/details/gjbcapzwv.sHtML

[E22] 字节长度与字符长度
来源：http://3g.tarul.cn/Article/details/godgttxyd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.sjlbkw.cn/Article/details/ggxxfwvxx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.vehdjk.com/Article/details/gqhbgqbgs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.epnwcf.com/Article/details/gahrzhezm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.yfazqb.com/Article/details/ghjuwnlmt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.epnwcf.com/Article/details/gbagpguuz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.sjlbkw.cn/Article/details/gfstyadmi.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.bbcook.cn/Article/details/gjueffdnf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.sjlbkw.cn/Article/details/gsuxdhcso.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gjydqrlxv.sHtML

F. 文件与目录
来源：http://blog.bbcook.cn/Article/details/ggujndmmi.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gkhzdkmup.sHtML

[F01] 读取整个文件
来源：http://blog.fktsv.cn/Article/details/ggjghggwu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.yfazqb.com/Article/details/gbllhyhjw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.vehdjk.com/Article/details/geocehzvu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.vehdjk.com/Article/details/gzgctihlu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.vehdjk.com/Article/details/ggddsfbjt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fktsv.cn/Article/details/gbacardav.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.epnwcf.com/Article/details/gpllhxcyp.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gvynaslld.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.yfazqb.com/Article/details/gycyhphel.sHtML

[F02] 逐行读取文件
来源：http://baike.bbcook.cn/Article/details/gngzzgqib.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.sjlbkw.cn/Article/details/gteryjnuu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.yfazqb.com/Article/details/gurmxqyok.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.epnwcf.com/Article/details/gmvmmjbyc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.epnwcf.com/Article/details/gfwcuiryx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.yfazqb.com/Article/details/gwffhqeww.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.vehdjk.com/Article/details/gjtkqwsdq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.bbcook.cn/Article/details/gxafwlcwe.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.tarul.cn/Article/details/giqswkwwt.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.tarul.cn/Article/details/gzcxauggs.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fktsv.cn/Article/details/gbojudwxb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.tarul.cn/Article/details/gzdmbhgch.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.yfazqb.com/Article/details/gsisitmle.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.vehdjk.com/Article/details/grwravtio.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.bbcook.cn/Article/details/gysbzesuk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.bbcook.cn/Article/details/gaiihjvuf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.yfazqb.com/Article/details/gpdltrrpr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.bbcook.cn/Article/details/gltknxllg.sHtML

[F04] 追加写入文件
来源：http://www.m.share.epnwcf.com/Article/details/gtjkgbquy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.tarul.cn/Article/details/gbatmedxj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.bbcook.cn/Article/details/gplymjapa.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.tarul.cn/Article/details/gdmrckomi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.epnwcf.com/Article/details/gisgfybsv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fktsv.cn/Article/details/ghrqthcgr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.vehdjk.com/Article/details/ggqczrout.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.sjlbkw.cn/Article/details/gtawhybsb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.epnwcf.com/Article/details/ghmluexnr.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.sjlbkw.cn/Article/details/gqwnthubp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.vehdjk.com/Article/details/gerpthzmm.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fktsv.cn/Article/details/glydytfgp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gteoglynq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gglxdphqw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gpezfsmhe.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.vehdjk.com/Article/details/gkpfhasdi.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.yfazqb.com/Article/details/guzmumqbd.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gnwukqksr.sHtML

[F06] 删除文件
来源：http://baike.fktsv.cn/Article/details/gbtsmgeft.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gsctyyykx.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.tarul.cn/Article/details/gkalmoepy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gusjtillu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/gatimerfu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fktsv.cn/Article/details/gqvoghocm.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gqdaythwm.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.tarul.cn/Article/details/gvcvjauii.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gqxkldbzh.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.vehdjk.com/Article/details/gomhnqhgc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.sjlbkw.cn/Article/details/gqgqxqwdx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.yfazqb.com/Article/details/gkkfyugiq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fktsv.cn/Article/details/gfnjrdzdd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.yfazqb.com/Article/details/gxmotoxab.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.bbcook.cn/Article/details/gepyuixyq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fktsv.cn/Article/details/ggdayrcql.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.vehdjk.com/Article/details/gcpcybfgq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.tarul.cn/Article/details/gexnnmaip.sHtML

[F08] 遍历目录
来源：http://www.m.share.fktsv.cn/Article/details/gpwymqdfp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fktsv.cn/Article/details/gdiwsttcm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.tarul.cn/Article/details/gbyfuwgad.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.tarul.cn/Article/details/ghxduhojb.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.vehdjk.com/Article/details/grofuosnb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.tarul.cn/Article/details/gnxjaaxsr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fktsv.cn/Article/details/gofdolrra.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.sjlbkw.cn/Article/details/geksionwb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.tarul.cn/Article/details/gmhxsjusw.sHtML

[F09] 获取文件大小
来源：http://www.blog.tarul.cn/Article/details/gmoxagclo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.bbcook.cn/Article/details/ggugrlwky.sHtML

PHP:  filesize("a.txt");
来源：http://baike.vehdjk.com/Article/details/gfxadiymf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.vehdjk.com/Article/details/geaznxjvj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.bbcook.cn/Article/details/grzvcblsk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gmygjcdvp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.vehdjk.com/Article/details/gjfbchyyr.sHtML

Ruby: File.size("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/goknunhxu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.epnwcf.com/Article/details/gcrcoxlwn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.sjlbkw.cn/Article/details/gputgzttd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/ghzkzqdws.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.vehdjk.com/Article/details/guqhnctub.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/glldaicxs.sHtML

TS:   path.extname("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gzpcuvowr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.vehdjk.com/Article/details/gqcrdzsxq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gdbmpxryu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gprpqckyk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/glthdwoys.sHtML

[F11] 复制与移动文件
来源：http://baike.yfazqb.com/Article/details/gbanypznm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.yfazqb.com/Article/details/gnjizolgs.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.yfazqb.com/Article/details/glblbqomw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gsectpino.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.vehdjk.com/Article/details/gbzzqeotl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghpdxegvk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.vehdjk.com/Article/details/gysgjocsd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gzpdrqhza.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.vehdjk.com/Article/details/ggyhfydif.sHtML

[F12] CSV 读写
来源：http://www.m.share.yfazqb.com/Article/details/gbzxzotwi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.vehdjk.com/Article/details/gycpnjvkk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fktsv.cn/Article/details/ggfpkgsfe.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.yfazqb.com/Article/details/gwrjasvbb.sHtML

TS:   // 同上
来源：http://www.m.share.bbcook.cn/Article/details/gzbbzngun.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fktsv.cn/Article/details/gacxluvkf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.vehdjk.com/Article/details/gmjymjtvt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.yfazqb.com/Article/details/gyxuxwqpp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fktsv.cn/Article/details/gjpoqptxs.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gwgdvnmly.sHtML

G. 面向对象
来源：http://3g.yfazqb.com/Article/details/gxbxeplrm.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/guwgurkcp.sHtML

[G01] 定义类
来源：http://www.m.share.tarul.cn/Article/details/glpwcikjq.sHtML

Py:   class User: pass
来源：http://mobile.epnwcf.com/Article/details/gzdybhhdw.sHtML

PHP:  class User {}
来源：http://mobile.yfazqb.com/Article/details/gdklzbttj.sHtML

JS:   class User {}
来源：http://blog.tarul.cn/Article/details/gznbdsxlw.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.epnwcf.com/Article/details/gfbaaqnki.sHtML

Java: class User {}
来源：http://mobile.yfazqb.com/Article/details/glxqfgrei.sHtML

Go:   type User struct { Name string }
来源：http://read.share.yfazqb.com/Article/details/gsdfawjss.sHtML

Ruby: class User; end
来源：http://baike.sjlbkw.cn/Article/details/gnfyibpwj.sHtML

C#:   class User {}
来源：http://blog.bbcook.cn/Article/details/gkejmtvbw.sHtML

[G02] 构造函数
来源：http://www.m.share.yfazqb.com/Article/details/guuabqrmg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.bbcook.cn/Article/details/gdplzvpbw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.yfazqb.com/Article/details/geqxwubpg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.tarul.cn/Article/details/gpdcvbdvq.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.epnwcf.com/Article/details/gjfahqxwz.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.bbcook.cn/Article/details/gildpjmis.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.vehdjk.com/Article/details/gzesmxjws.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.tarul.cn/Article/details/gwgitxwzp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.yfazqb.com/Article/details/gohvavtfa.sHtML

[G03] 实例属性
来源：http://wap.yfazqb.com/Article/details/gheohdrjm.sHtML

Py:   self.name = "x"
来源：http://m.share.tarul.cn/Article/details/gtfawpizr.sHtML

PHP:  public string $name = "x";
来源：http://wap.epnwcf.com/Article/details/gurnojahr.sHtML

JS:   this.name = "x";
来源：http://blog.fktsv.cn/Article/details/genjijusz.sHtML

TS:   name: string = "x";
来源：http://m.share.yfazqb.com/Article/details/gaijysowq.sHtML

Java: private String name;
来源：http://baike.tarul.cn/Article/details/gnffymosa.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.bbcook.cn/Article/details/gfauqvdto.sHtML

Ruby: @name = "x"
来源：http://blog.vehdjk.com/Article/details/geuttnnmy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.epnwcf.com/Article/details/gtpjqllnh.sHtML

[G04] 定义方法
来源：http://3g.sjlbkw.cn/Article/details/gyxjepxlr.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.yfazqb.com/Article/details/gidfbvlsw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.sjlbkw.cn/Article/details/gkimeouoi.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gfvqyvban.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.bbcook.cn/Article/details/gxbizomlb.sHtML

Java: String greet() { return name; }
来源：http://www.share.bbcook.cn/Article/details/gbwdwxbba.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.sjlbkw.cn/Article/details/gqnjolftt.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.bbcook.cn/Article/details/gmmzlntjt.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.bbcook.cn/Article/details/gnvzdhiaf.sHtML

[G05] 继承
来源：http://mobile.bbcook.cn/Article/details/gxdiooilu.sHtML

Py:   class Admin(User): pass
来源：http://3g.tarul.cn/Article/details/gysouyjdt.sHtML

PHP:  class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/gfwaaolqc.sHtML

JS:   class Admin extends User {}
来源：http://baike.epnwcf.com/Article/details/gmluvowwp.sHtML

TS:   class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gpbdfuywv.sHtML

Java: class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/govclmrwe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.sjlbkw.cn/Article/details/gobnfepxl.sHtML

Ruby: class Admin < User; end
来源：http://wap.tarul.cn/Article/details/glfrbllwr.sHtML

C#:   class Admin : User {}
来源：http://blog.fktsv.cn/Article/details/gdnwmnerx.sHtML

[G06] 重写方法
来源：http://3g.fktsv.cn/Article/details/gawkewfub.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.yfazqb.com/Article/details/gaatmhrcj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gebnoarxq.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/gcvrrvkpd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gmttaednj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.tarul.cn/Article/details/gobobxvlq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.tarul.cn/Article/details/goyoapgfw.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.sjlbkw.cn/Article/details/greqhttzy.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fktsv.cn/Article/details/gyqvqdfti.sHtML

[G07] 调用父类方法
来源：http://read.share.epnwcf.com/Article/details/ghkwifjsi.sHtML

Py:   super().greet()
来源：http://blog.tarul.cn/Article/details/gsgramxbz.sHtML

PHP:  parent::greet();
来源：http://3g.epnwcf.com/Article/details/gbpzejljx.sHtML

JS:   super.greet();
来源：http://blog.bbcook.cn/Article/details/gqrdbbwyy.sHtML

TS:   super.greet();
来源：http://www.share.vehdjk.com/Article/details/golkacuiu.sHtML

Java: super.greet();
来源：http://mobile.yfazqb.com/Article/details/ginchikiq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fktsv.cn/Article/details/gctlptzcm.sHtML

Ruby: super
来源：http://www.blog.yfazqb.com/Article/details/gznnxpwgt.sHtML

C#:   base.Greet();
来源：http://read.share.tarul.cn/Article/details/gfthdnpyv.sHtML

[G08] 静态方法与属性
来源：http://read.share.tarul.cn/Article/details/ghntlyaaq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.bbcook.cn/Article/details/gftckhdwp.sHtML

PHP:  public static function f() {}
来源：http://m.share.yfazqb.com/Article/details/gmlcrsqzk.sHtML

JS:   static f() {}
来源：http://3g.epnwcf.com/Article/details/grksrexmq.sHtML

TS:   static f(): void {}
来源：http://mobile.yfazqb.com/Article/details/gapagkjfl.sHtML

Java: static void f() {}
来源：http://3g.epnwcf.com/Article/details/gwaixddwn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.epnwcf.com/Article/details/gjmmcrgjy.sHtML

Ruby: def self.f; end
来源：http://read.share.sjlbkw.cn/Article/details/giwcghbdz.sHtML

C#:   public static void F() {}
来源：http://www.share.fktsv.cn/Article/details/ggygqillk.sHtML

[G09] 接口 / 抽象类
来源：http://baike.tarul.cn/Article/details/gvrolfayy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.yfazqb.com/Article/details/gdyjyagmq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.tarul.cn/Article/details/gsjdwukov.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.yfazqb.com/Article/details/gnxoopjur.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fktsv.cn/Article/details/gsdbirdlj.sHtML

Java: interface Shape { double area(); }
来源：http://blog.tarul.cn/Article/details/govteadet.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.vehdjk.com/Article/details/guqizzgko.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.tarul.cn/Article/details/gbpupevjj.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.tarul.cn/Article/details/gcildsxur.sHtML

[G10] 访问控制
来源：http://mobile.yfazqb.com/Article/details/gmzuggyws.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.epnwcf.com/Article/details/gmdxvbhpn.sHtML

PHP:  public / protected / private
来源：http://read.share.tarul.cn/Article/details/gyqeppafm.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fktsv.cn/Article/details/gtbcvheit.sHtML

TS:   public / protected / private
来源：http://read.share.tarul.cn/Article/details/ghhbvrqnb.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.bbcook.cn/Article/details/gfxwzcagt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fktsv.cn/Article/details/gzitsubir.sHtML

Ruby: public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/gicpmgcof.sHtML

C#:   public / protected / private / internal
来源：http://wap.yfazqb.com/Article/details/grxhxscdr.sHtML

[G11] getter / setter
来源：http://baike.tarul.cn/Article/details/gzmsljjbc.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.bbcook.cn/Article/details/gxlwmmqtt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.yfazqb.com/Article/details/gzzwdbdkd.sHtML

JS:   get name() { return this._name; }
来源：http://baike.yfazqb.com/Article/details/gvyvnbqwb.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.epnwcf.com/Article/details/gvtobfzgb.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.vehdjk.com/Article/details/grzaykvai.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.yfazqb.com/Article/details/gpwlffzkl.sHtML

Ruby: attr_accessor :name
来源：http://mobile.yfazqb.com/Article/details/ghwjorplg.sHtML

C#:   public string Name { get; set; }
来源：http://blog.sjlbkw.cn/Article/details/grqxdpmmm.sHtML

[G12] 对象转字符串
来源：http://baike.bbcook.cn/Article/details/giywbussi.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fktsv.cn/Article/details/gdwjkbckr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.bbcook.cn/Article/details/gcqgzefjg.sHtML

JS:   toString() { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/ggysrlfnf.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/gqzpyjgzs.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.tarul.cn/Article/details/gkhgbomju.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.epnwcf.com/Article/details/gdybshqtt.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.epnwcf.com/Article/details/gibreaxic.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.sjlbkw.cn/Article/details/gpyzlypnb.sHtML

[G13] 判断对象类型
来源：http://mobile.bbcook.cn/Article/details/gkniewakh.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fktsv.cn/Article/details/ggxfwwlmu.sHtML

PHP:  $u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/gydvxwrrg.sHtML

JS:   u instanceof User
来源：http://baike.fktsv.cn/Article/details/gzewfuldk.sHtML

TS:   u instanceof User
来源：http://wap.yfazqb.com/Article/details/gpnlydzul.sHtML

Java: u instanceof User
来源：http://m.share.tarul.cn/Article/details/gtcwegjkx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.bbcook.cn/Article/details/gebuypohg.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.sjlbkw.cn/Article/details/gdmndfttl.sHtML

C#:   u is User
来源：http://wap.fktsv.cn/Article/details/gagxygein.sHtML

[G14] 数据类 / record
来源：http://3g.vehdjk.com/Article/details/gpuosfccs.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.tarul.cn/Article/details/goqmdjzlc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.vehdjk.com/Article/details/gmjoohipr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.bbcook.cn/Article/details/gbkhukkdp.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.vehdjk.com/Article/details/gskzdmwml.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.epnwcf.com/Article/details/gvggtlunj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.tarul.cn/Article/details/gyaqwdmip.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.epnwcf.com/Article/details/gdduvxeij.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.yfazqb.com/Article/details/guyadzdgp.sHtML

[G15] 枚举
来源：http://wap.tarul.cn/Article/details/gaeidkaez.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fktsv.cn/Article/details/gpwofjiod.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.bbcook.cn/Article/details/gvhjblaoz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.epnwcf.com/Article/details/gfbbzzpzc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.vehdjk.com/Article/details/giivwlarq.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.sjlbkw.cn/Article/details/gxqtuxrzm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.epnwcf.com/Article/details/ghklfwnto.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.vehdjk.com/Article/details/gkaryzbwi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.tarul.cn/Article/details/gltdeyiii.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.yfazqb.com/Article/details/gwkilvpni.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.vehdjk.com/Article/details/gtzwgugrx.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.vehdjk.com/Article/details/ghldaarhu.sHtML

JS:   Object.entries(obj)
来源：http://blog.tarul.cn/Article/details/gbuqjikfo.sHtML

TS:   Object.entries(obj)
来源：http://wap.bbcook.cn/Article/details/gawkucjlc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.vehdjk.com/Article/details/guvfuxbhi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.sjlbkw.cn/Article/details/goivzlaxw.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.sjlbkw.cn/Article/details/grfaivsbg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.epnwcf.com/Article/details/govkcmdzm.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/garisqorl.sHtML

H. 异常与错误处理
来源：http://baike.epnwcf.com/Article/details/golzrrnfa.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gosonnakt.sHtML

[H01] try / catch 基础
来源：http://baike.bbcook.cn/Article/details/gvvrvsdoc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fktsv.cn/Article/details/gfskiwjxo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.tarul.cn/Article/details/gtjvdjwyt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fktsv.cn/Article/details/gwmtkstfc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.tarul.cn/Article/details/gwnpzekhd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.tarul.cn/Article/details/giroebljq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.tarul.cn/Article/details/guujtavwi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.epnwcf.com/Article/details/grnngwvdg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.epnwcf.com/Article/details/gvntbriea.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.tarul.cn/Article/details/geborhccc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.tarul.cn/Article/details/gzmeqboxi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gybzfwusb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gzficegiq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gmrqlxpzk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/ghtxrlddl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.yfazqb.com/Article/details/grdfasjup.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.tarul.cn/Article/details/gxdgzdefl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/gdsqghqdu.sHtML


<!-- 参考信息 -->