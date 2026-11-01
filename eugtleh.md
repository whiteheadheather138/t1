代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.vehdjk.com/Article/details/gldwfzbsg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.yfazqb.com/Article/details/gslkywekp.sHtML

TS:   if (s === "") {}
来源：http://3g.sjlbkw.cn/Article/details/gvbsuorys.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.vehdjk.com/Article/details/gsrzfndlr.sHtML

Go:   if s == "" {}
来源：http://mobile.yfazqb.com/Article/details/gnxpbzjic.sHtML

Ruby: if s.empty?
来源：http://www.share.epnwcf.com/Article/details/gwkwggtxs.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fktsv.cn/Article/details/gyovduxjr.sHtML

[E21] 超长截断加省略号
来源：http://m.share.sjlbkw.cn/Article/details/gjqwifszm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.tarul.cn/Article/details/goofzpkue.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/ggvawdpsi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.tarul.cn/Article/details/gqbnjmsyd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gbhcaymhu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.epnwcf.com/Article/details/gdyniaweh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.tarul.cn/Article/details/gqwclbjgj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gimqiaohq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gzkwyzdzf.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.tarul.cn/Article/details/gkjtrctwq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.sjlbkw.cn/Article/details/gzvbaurnu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gsttdeacb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fktsv.cn/Article/details/gfceaczfa.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.tarul.cn/Article/details/gfbpkvjuh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.bbcook.cn/Article/details/gcthzaqyu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.epnwcf.com/Article/details/gofrpvvel.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.epnwcf.com/Article/details/gcppoussp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.sjlbkw.cn/Article/details/ghyhgvplp.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gqyfiihjv.sHtML

F. 文件与目录
来源：http://read.share.vehdjk.com/Article/details/gwxrspjlm.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/godgzdpuq.sHtML

[F01] 读取整个文件
来源：http://baike.tarul.cn/Article/details/gkkjjjled.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.yfazqb.com/Article/details/grjjpmjhl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.epnwcf.com/Article/details/girmpasbo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.bbcook.cn/Article/details/gceqlqnqf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.yfazqb.com/Article/details/gvetjqjqe.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gporywiiy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fktsv.cn/Article/details/gatfcihlh.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fktsv.cn/Article/details/gmevkotph.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.epnwcf.com/Article/details/gbmbiamfa.sHtML

[F02] 逐行读取文件
来源：http://read.share.tarul.cn/Article/details/gmcvlqmdj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.sjlbkw.cn/Article/details/glzdnvtey.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.bbcook.cn/Article/details/gfwymoyqj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.bbcook.cn/Article/details/golesofke.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.sjlbkw.cn/Article/details/gkgxwbpdl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.tarul.cn/Article/details/gjmdexzdp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.sjlbkw.cn/Article/details/gupeyodgm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.bbcook.cn/Article/details/gnlqomqjv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fktsv.cn/Article/details/glvdzlvkj.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.tarul.cn/Article/details/gsoszmyjl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.bbcook.cn/Article/details/gylxlfiwu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.tarul.cn/Article/details/gaunbftax.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.vehdjk.com/Article/details/gafpizeqa.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.bbcook.cn/Article/details/gaghyvnmm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.vehdjk.com/Article/details/ghtldftus.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.vehdjk.com/Article/details/ghygwoqcr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.bbcook.cn/Article/details/gdqbfcisk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.tarul.cn/Article/details/gqjzpisii.sHtML

[F04] 追加写入文件
来源：http://3g.tarul.cn/Article/details/grwmulebv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.sjlbkw.cn/Article/details/goxflvvvi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.bbcook.cn/Article/details/gbdduabgz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.tarul.cn/Article/details/gqocdopjw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.yfazqb.com/Article/details/gcsdfcbcw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.bbcook.cn/Article/details/gsfukscbx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.bbcook.cn/Article/details/gxzmucvqh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.yfazqb.com/Article/details/grvgovdoz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.yfazqb.com/Article/details/gwkqsdyfd.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.tarul.cn/Article/details/grsafqmwi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.sjlbkw.cn/Article/details/gplnvyvmq.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fktsv.cn/Article/details/glzcwxepc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/gscacgufl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/glfqbpnkx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/gprwumuhz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.tarul.cn/Article/details/gpemgkwky.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gvgqucqmc.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gwlomzvza.sHtML

[F06] 删除文件
来源：http://wap.epnwcf.com/Article/details/gpcyctpdc.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gbhyfdggm.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.yfazqb.com/Article/details/geotjeceh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gsrvxnedl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/gbtnylstu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gipyfiogr.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.epnwcf.com/Article/details/gcrqqdika.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gqrftlxdc.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.yfazqb.com/Article/details/gttftdxzb.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.bbcook.cn/Article/details/glphhwund.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.epnwcf.com/Article/details/gwsjpslde.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.yfazqb.com/Article/details/gaxrfyapo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fktsv.cn/Article/details/gttsayiza.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.tarul.cn/Article/details/godaunypg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fktsv.cn/Article/details/gmfibxqdr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.tarul.cn/Article/details/gtbfmmmsf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fktsv.cn/Article/details/gtflzkdon.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.vehdjk.com/Article/details/glillcxjz.sHtML

[F08] 遍历目录
来源：http://read.share.bbcook.cn/Article/details/givnsiqbr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.vehdjk.com/Article/details/grugqdxnk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.sjlbkw.cn/Article/details/gkzhvghzl.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.epnwcf.com/Article/details/gifozewoe.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.epnwcf.com/Article/details/gtwhkxvod.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.yfazqb.com/Article/details/gohcswvkw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.epnwcf.com/Article/details/gehddvkot.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.bbcook.cn/Article/details/ggapdnfcf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.bbcook.cn/Article/details/goksrlubt.sHtML

[F09] 获取文件大小
来源：http://www.blog.bbcook.cn/Article/details/ggmbqytqu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.bbcook.cn/Article/details/ghecpujhs.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gbjgbchfk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.sjlbkw.cn/Article/details/ggqeplill.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.sjlbkw.cn/Article/details/gujroegmm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gpiclibal.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.vehdjk.com/Article/details/gzbiacdlx.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gbiwyjisi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.vehdjk.com/Article/details/gcasdqsha.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.bbcook.cn/Article/details/gwiooxxlm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/geniccagy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.epnwcf.com/Article/details/ggxadjape.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/gunyfsfpy.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gnqshrdom.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.sjlbkw.cn/Article/details/gkolmsjtw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/gtjvejoox.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gogupejik.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gsgvguckq.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fktsv.cn/Article/details/gkqayuwmq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gotxnvvee.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.bbcook.cn/Article/details/glkoneopi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/gpydmxnwo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/girwlfjuv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.vehdjk.com/Article/details/gccatqefj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.bbcook.cn/Article/details/gxumwfkou.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/gnbnkilgn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.bbcook.cn/Article/details/gjczvsxfm.sHtML

[F12] CSV 读写
来源：http://3g.bbcook.cn/Article/details/gcygzsmzi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.bbcook.cn/Article/details/gwefwxanm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.sjlbkw.cn/Article/details/gnwkqjsyf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjjtnixb.sHtML

TS:   // 同上
来源：http://www.m.share.epnwcf.com/Article/details/ganyolkoy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.vehdjk.com/Article/details/gwmbwcucv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.tarul.cn/Article/details/gyafylfco.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.yfazqb.com/Article/details/gzifpcool.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fktsv.cn/Article/details/gwtpkudmv.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gwkdunncs.sHtML

G. 面向对象
来源：http://3g.fktsv.cn/Article/details/gwduvqwpr.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gfwyzoxja.sHtML

[G01] 定义类
来源：http://wap.vehdjk.com/Article/details/gssfsuejb.sHtML

Py:   class User: pass
来源：http://www.share.vehdjk.com/Article/details/gyzbxgiba.sHtML

PHP:  class User {}
来源：http://blog.epnwcf.com/Article/details/gihhjujit.sHtML

JS:   class User {}
来源：http://mobile.vehdjk.com/Article/details/gwsjqlguv.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.vehdjk.com/Article/details/gfxysvuee.sHtML

Java: class User {}
来源：http://mobile.epnwcf.com/Article/details/gqjkyzrbg.sHtML

Go:   type User struct { Name string }
来源：http://wap.vehdjk.com/Article/details/gzxvtyipq.sHtML

Ruby: class User; end
来源：http://mobile.fktsv.cn/Article/details/goyllhedp.sHtML

C#:   class User {}
来源：http://www.share.sjlbkw.cn/Article/details/gsokqtlkm.sHtML

[G02] 构造函数
来源：http://3g.sjlbkw.cn/Article/details/grjroldxc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.vehdjk.com/Article/details/gypfibzyx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.yfazqb.com/Article/details/gfyhimfut.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.vehdjk.com/Article/details/gxrsgeasg.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.yfazqb.com/Article/details/gjhdggaeu.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.vehdjk.com/Article/details/gxjvxftka.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.vehdjk.com/Article/details/gtrwoizaz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.epnwcf.com/Article/details/gahycwpvw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fktsv.cn/Article/details/giyqdydbs.sHtML

[G03] 实例属性
来源：http://blog.vehdjk.com/Article/details/gpxydljyu.sHtML

Py:   self.name = "x"
来源：http://3g.epnwcf.com/Article/details/govoyckro.sHtML

PHP:  public string $name = "x";
来源：http://m.share.tarul.cn/Article/details/glywnvbju.sHtML

JS:   this.name = "x";
来源：http://blog.sjlbkw.cn/Article/details/gmenlwydc.sHtML

TS:   name: string = "x";
来源：http://wap.fktsv.cn/Article/details/gdfblfggg.sHtML

Java: private String name;
来源：http://3g.fktsv.cn/Article/details/ggiuqqtda.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.epnwcf.com/Article/details/gczzkrtkj.sHtML

Ruby: @name = "x"
来源：http://wap.bbcook.cn/Article/details/ggfdwihas.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.yfazqb.com/Article/details/gfopolfaz.sHtML

[G04] 定义方法
来源：http://www.m.share.tarul.cn/Article/details/ghjbhgsax.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fktsv.cn/Article/details/gdqztmuie.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.bbcook.cn/Article/details/gvlcawwoa.sHtML

JS:   greet() { return this.name; }
来源：http://blog.tarul.cn/Article/details/gbbtbaldm.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.yfazqb.com/Article/details/gxnfwqwxt.sHtML

Java: String greet() { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gzftuysle.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.tarul.cn/Article/details/gffhlpmxq.sHtML

Ruby: def greet; @name; end
来源：http://m.share.tarul.cn/Article/details/gsrzokdrn.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fktsv.cn/Article/details/gxzvnmvko.sHtML

[G05] 继承
来源：http://m.share.fktsv.cn/Article/details/grrbvehwi.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.tarul.cn/Article/details/gedknzugd.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/gavelhbfw.sHtML

JS:   class Admin extends User {}
来源：http://baike.fktsv.cn/Article/details/gcpnutmyt.sHtML

TS:   class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gjkujteyh.sHtML

Java: class Admin extends User {}
来源：http://baike.epnwcf.com/Article/details/gubypjuta.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.sjlbkw.cn/Article/details/ghtebivie.sHtML

Ruby: class Admin < User; end
来源：http://blog.bbcook.cn/Article/details/gogppemgm.sHtML

C#:   class Admin : User {}
来源：http://wap.sjlbkw.cn/Article/details/gmwjvgeyw.sHtML

[G06] 重写方法
来源：http://baike.vehdjk.com/Article/details/gymvmbtzw.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.epnwcf.com/Article/details/gbhdruzsf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gekdfkekh.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/gbkyrdqgy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/gvyuochij.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/glpdmgezh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.tarul.cn/Article/details/gytnimqwf.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fktsv.cn/Article/details/gvbucwluj.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.sjlbkw.cn/Article/details/gewrvssgw.sHtML

[G07] 调用父类方法
来源：http://3g.yfazqb.com/Article/details/gmdcnldhr.sHtML

Py:   super().greet()
来源：http://m.share.tarul.cn/Article/details/gjhewzhdk.sHtML

PHP:  parent::greet();
来源：http://read.share.fktsv.cn/Article/details/gagshscgb.sHtML

JS:   super.greet();
来源：http://www.share.yfazqb.com/Article/details/grcxkazey.sHtML

TS:   super.greet();
来源：http://3g.yfazqb.com/Article/details/guiafpnom.sHtML

Java: super.greet();
来源：http://blog.bbcook.cn/Article/details/gwvsfeywc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.yfazqb.com/Article/details/gcqnxwwls.sHtML

Ruby: super
来源：http://www.blog.yfazqb.com/Article/details/gxhlxuwnm.sHtML

C#:   base.Greet();
来源：http://wap.tarul.cn/Article/details/gnumunmjq.sHtML

[G08] 静态方法与属性
来源：http://baike.bbcook.cn/Article/details/gckcmkpfk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.yfazqb.com/Article/details/gpwunhdgx.sHtML

PHP:  public static function f() {}
来源：http://3g.vehdjk.com/Article/details/gqjgissni.sHtML

JS:   static f() {}
来源：http://blog.fktsv.cn/Article/details/gmlcqqrti.sHtML

TS:   static f(): void {}
来源：http://www.blog.bbcook.cn/Article/details/gdyjiyrcc.sHtML

Java: static void f() {}
来源：http://read.share.vehdjk.com/Article/details/giafipobm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.tarul.cn/Article/details/goxcryvhc.sHtML

Ruby: def self.f; end
来源：http://blog.bbcook.cn/Article/details/gwlsocity.sHtML

C#:   public static void F() {}
来源：http://read.share.sjlbkw.cn/Article/details/guilnmtrc.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fktsv.cn/Article/details/gvrabmycn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.tarul.cn/Article/details/gpxrtfkyr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.yfazqb.com/Article/details/gigryypcb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.tarul.cn/Article/details/gtkhjvdxe.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.tarul.cn/Article/details/gjybpunwg.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fktsv.cn/Article/details/gakokintz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.tarul.cn/Article/details/gibyeyszd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.bbcook.cn/Article/details/gejnyjtgm.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.yfazqb.com/Article/details/gmrghgbau.sHtML

[G10] 访问控制
来源：http://read.share.sjlbkw.cn/Article/details/grxadpumq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.vehdjk.com/Article/details/ghgeplnrg.sHtML

PHP:  public / protected / private
来源：http://baike.bbcook.cn/Article/details/gkrxarbje.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.yfazqb.com/Article/details/gtqilarxn.sHtML

TS:   public / protected / private
来源：http://m.share.epnwcf.com/Article/details/gsapschbz.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.epnwcf.com/Article/details/gsaezcexy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.yfazqb.com/Article/details/gjnefnozc.sHtML

Ruby: public / protected / private
来源：http://3g.bbcook.cn/Article/details/garikvxxp.sHtML

C#:   public / protected / private / internal
来源：http://3g.tarul.cn/Article/details/gczqisjop.sHtML

[G11] getter / setter
来源：http://mobile.bbcook.cn/Article/details/gskvbpvcu.sHtML

Py:   @property 与 @x.setter
来源：http://baike.vehdjk.com/Article/details/gmhvqcewu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.epnwcf.com/Article/details/geewworaj.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.sjlbkw.cn/Article/details/gifxjafll.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fktsv.cn/Article/details/guihvbmnw.sHtML

Java: public String getName() { return name; }
来源：http://blog.vehdjk.com/Article/details/gofdcoqzw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.sjlbkw.cn/Article/details/gizdkinlh.sHtML

Ruby: attr_accessor :name
来源：http://read.share.epnwcf.com/Article/details/gjrxcufqg.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.sjlbkw.cn/Article/details/ghkuznhtx.sHtML

[G12] 对象转字符串
来源：http://read.share.bbcook.cn/Article/details/gyxrvhfgo.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.vehdjk.com/Article/details/ghemcdotd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.vehdjk.com/Article/details/gbzacbjur.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/gxaguwuki.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.tarul.cn/Article/details/gihgskvup.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.epnwcf.com/Article/details/glbzvzhdb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.bbcook.cn/Article/details/gifvgtpds.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fktsv.cn/Article/details/glgaxuygs.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.sjlbkw.cn/Article/details/gtxqcsstc.sHtML

[G13] 判断对象类型
来源：http://3g.fktsv.cn/Article/details/gccspqkvk.sHtML

Py:   isinstance(u, User)
来源：http://3g.tarul.cn/Article/details/gwoagisiu.sHtML

PHP:  $u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/gfrqtlzjo.sHtML

JS:   u instanceof User
来源：http://www.share.bbcook.cn/Article/details/gqmciitlc.sHtML

TS:   u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gqydgdksk.sHtML

Java: u instanceof User
来源：http://read.share.vehdjk.com/Article/details/guvvbzimm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.sjlbkw.cn/Article/details/godwgirqr.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.tarul.cn/Article/details/gpawqvlct.sHtML

C#:   u is User
来源：http://www.share.bbcook.cn/Article/details/gxcqewtsb.sHtML

[G14] 数据类 / record
来源：http://www.share.epnwcf.com/Article/details/gvbilkpbq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.yfazqb.com/Article/details/geixonluz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.bbcook.cn/Article/details/gwbzprlfq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.tarul.cn/Article/details/gvzitkhkc.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.yfazqb.com/Article/details/gtehmrhvu.sHtML

Java: record User(String name, int age) {}
来源：http://wap.bbcook.cn/Article/details/gfaeifahc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.yfazqb.com/Article/details/gmzquiyhb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.sjlbkw.cn/Article/details/gnmuvzarb.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.yfazqb.com/Article/details/gogucsnhz.sHtML

[G15] 枚举
来源：http://www.m.share.sjlbkw.cn/Article/details/gggjofmhq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.yfazqb.com/Article/details/gdlnvxpdw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.vehdjk.com/Article/details/gpwwssdnu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.sjlbkw.cn/Article/details/gzkxxiofm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.vehdjk.com/Article/details/gghqpgrhu.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.vehdjk.com/Article/details/gqwglglyt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.tarul.cn/Article/details/gdgcptkeu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.vehdjk.com/Article/details/gbkpvdpcs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.yfazqb.com/Article/details/guhxunkte.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.vehdjk.com/Article/details/guhbgdhon.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.epnwcf.com/Article/details/gemhgehkd.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.epnwcf.com/Article/details/gdtkysmrl.sHtML

JS:   Object.entries(obj)
来源：http://blog.tarul.cn/Article/details/ghiedipzb.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjxzczce.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fktsv.cn/Article/details/guiqylubr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.yfazqb.com/Article/details/gzzrmhfxx.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.vehdjk.com/Article/details/grqdlzowl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.yfazqb.com/Article/details/glrjireeb.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gjaopvzce.sHtML

H. 异常与错误处理
来源：http://baike.sjlbkw.cn/Article/details/gloaiiqpf.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gyglorzsp.sHtML

[H01] try / catch 基础
来源：http://www.blog.tarul.cn/Article/details/gqmqcuazk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.tarul.cn/Article/details/gykvjmwve.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.sjlbkw.cn/Article/details/geaxhhbcj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.bbcook.cn/Article/details/gkpkbmfnc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.vehdjk.com/Article/details/gvwqexpxo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.vehdjk.com/Article/details/gcicxjviw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.yfazqb.com/Article/details/gwlwzqjnv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.sjlbkw.cn/Article/details/gxzbpgjxk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.yfazqb.com/Article/details/gxbixdomv.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.epnwcf.com/Article/details/gmknngjcn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.epnwcf.com/Article/details/gcmsvzplr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gvwgldhgz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gwfheocgf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.tarul.cn/Article/details/gcialhser.sHtML


<!-- 参考信息 -->