代发 wailian999

Ruby: s.lines
来源：http://m.share.yfazqb.com/Article/details/gqtpgobpa.sHtML

C#:   s.Split('\n')
来源：http://3g.epnwcf.com/Article/details/gujwnrkow.sHtML

[E20] 判断字符串是否为空
来源：http://baike.bbcook.cn/Article/details/gujabaoqk.sHtML

Py:   if not s:
来源：http://baike.yfazqb.com/Article/details/gyhkamdvj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.epnwcf.com/Article/details/grjgbhwmo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.vehdjk.com/Article/details/gcndjpehh.sHtML

TS:   if (s === "") {}
来源：http://read.share.fktsv.cn/Article/details/gezvcreza.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.sjlbkw.cn/Article/details/gvnrrxket.sHtML

Go:   if s == "" {}
来源：http://wap.yfazqb.com/Article/details/gfzcffavn.sHtML

Ruby: if s.empty?
来源：http://3g.fktsv.cn/Article/details/gjhkywsmw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.sjlbkw.cn/Article/details/gvwwobeeg.sHtML

[E21] 超长截断加省略号
来源：http://baike.sjlbkw.cn/Article/details/gwlxvrnjr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.vehdjk.com/Article/details/gwjhrsorr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/ggaxijryr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/ggwnmbfpt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.yfazqb.com/Article/details/ggobsepal.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.tarul.cn/Article/details/gelmfkmdq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.sjlbkw.cn/Article/details/gmpswqdyz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.yfazqb.com/Article/details/ghqlnagqd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.epnwcf.com/Article/details/gpzqajlvh.sHtML

[E22] 字节长度与字符长度
来源：http://3g.yfazqb.com/Article/details/gzbbyazgx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.yfazqb.com/Article/details/gxmegbfcq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gpbyuzbuy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.tarul.cn/Article/details/gzdagjhyc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.epnwcf.com/Article/details/gjxmfrsuh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.bbcook.cn/Article/details/gylfngggz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.tarul.cn/Article/details/gwknzlfri.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.yfazqb.com/Article/details/gayijwvnt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.yfazqb.com/Article/details/golagszdo.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gfnwbyfaq.sHtML

F. 文件与目录
来源：http://www.share.sjlbkw.cn/Article/details/gkwsxqwcn.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gbxtvhutt.sHtML

[F01] 读取整个文件
来源：http://wap.bbcook.cn/Article/details/gmrozsjdk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.yfazqb.com/Article/details/gjmmvlepx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gluzxhukn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.epnwcf.com/Article/details/gqzqeqwne.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.vehdjk.com/Article/details/ghujuigtx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fktsv.cn/Article/details/gbujuoglf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.yfazqb.com/Article/details/goiomdebq.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gwvcionlu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.tarul.cn/Article/details/grsgwcbrq.sHtML

[F02] 逐行读取文件
来源：http://www.share.tarul.cn/Article/details/gnmcqksjl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.tarul.cn/Article/details/ghrnbfujp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.vehdjk.com/Article/details/ggbwcnggt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.bbcook.cn/Article/details/grpnltmsh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.bbcook.cn/Article/details/gjbujvjvr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.tarul.cn/Article/details/gynvmzhou.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.vehdjk.com/Article/details/gczqgdvwa.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.sjlbkw.cn/Article/details/gnlvwzhif.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.yfazqb.com/Article/details/gpnguyjqt.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.sjlbkw.cn/Article/details/gtdkefidv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.yfazqb.com/Article/details/gkldqzuic.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fktsv.cn/Article/details/gctxkqoaj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.yfazqb.com/Article/details/gxqsvpvbg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.yfazqb.com/Article/details/gpmkqlevc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.yfazqb.com/Article/details/gccbptmdg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.sjlbkw.cn/Article/details/gsirssrok.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.sjlbkw.cn/Article/details/gtccwrhpq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.bbcook.cn/Article/details/ghhrxnjng.sHtML

[F04] 追加写入文件
来源：http://www.share.vehdjk.com/Article/details/gpjbmrwhu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.bbcook.cn/Article/details/gsekgbdqt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.vehdjk.com/Article/details/gdslitcdg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.yfazqb.com/Article/details/gfagfwodg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.epnwcf.com/Article/details/gvipbvgkg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.vehdjk.com/Article/details/gyvxtupyl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.yfazqb.com/Article/details/gyoneuzbf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.yfazqb.com/Article/details/gprguucoo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.vehdjk.com/Article/details/gefmmzyiq.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.yfazqb.com/Article/details/gfxujwrak.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.tarul.cn/Article/details/gxgqhnxnf.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.tarul.cn/Article/details/gcszswhju.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/giploodym.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gdumvajvs.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.bbcook.cn/Article/details/guhmstfuy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.sjlbkw.cn/Article/details/gnbljgfww.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.tarul.cn/Article/details/gdrrbmstg.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gcmcfucmz.sHtML

[F06] 删除文件
来源：http://blog.vehdjk.com/Article/details/gkoerucon.sHtML

Py:   os.remove("a.txt")
来源：http://3g.vehdjk.com/Article/details/gllxjjfor.sHtML

PHP:  unlink("a.txt");
来源：http://baike.tarul.cn/Article/details/gayftnwan.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.tarul.cn/Article/details/gnyixiixg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fktsv.cn/Article/details/ghjkzmnzo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/giozuqsvg.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gpgavalre.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.tarul.cn/Article/details/gplmpgajo.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gwccauyoh.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.sjlbkw.cn/Article/details/ghtnizqij.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.epnwcf.com/Article/details/gyizafolr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.yfazqb.com/Article/details/gawwlfupw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.epnwcf.com/Article/details/gjdlkftyu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.vehdjk.com/Article/details/grogjnkex.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.bbcook.cn/Article/details/gnplmrdto.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.bbcook.cn/Article/details/gtryoxmbn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.yfazqb.com/Article/details/gcyviyzmq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.vehdjk.com/Article/details/gzlczfwrp.sHtML

[F08] 遍历目录
来源：http://baike.fktsv.cn/Article/details/gjjqrrwqk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.vehdjk.com/Article/details/ghknfkcqr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.sjlbkw.cn/Article/details/gpkcwxaxn.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.vehdjk.com/Article/details/gwkltnspj.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.tarul.cn/Article/details/gbmsfgcxh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.tarul.cn/Article/details/gynherdpd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fktsv.cn/Article/details/gvdhdxlyu.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.bbcook.cn/Article/details/glfexneuc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fktsv.cn/Article/details/gwvfeazgm.sHtML

[F09] 获取文件大小
来源：http://www.share.sjlbkw.cn/Article/details/gvoioqhsy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gblxyxcww.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gwcfdkavi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.bbcook.cn/Article/details/gncckaspj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.epnwcf.com/Article/details/ghdcqfyzt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/gfpcsuatn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.epnwcf.com/Article/details/grwowefpb.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gagsbomgg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.yfazqb.com/Article/details/gyxycsuyp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.yfazqb.com/Article/details/gmyetwpbd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gdujzxcuo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.vehdjk.com/Article/details/gwhbkevay.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/guvvilbpe.sHtML

TS:   path.extname("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/grpcnrfud.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.vehdjk.com/Article/details/glgmhgcxd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gyubaavxw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gkehruiod.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/gavqzicxp.sHtML

[F11] 复制与移动文件
来源：http://mobile.fktsv.cn/Article/details/gcfkmtbnr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gxvaydrqo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fktsv.cn/Article/details/gjshxecpm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/gmukdpwut.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gagyncjgx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.tarul.cn/Article/details/gkvsjkkrq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fktsv.cn/Article/details/glzyrwsrb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/gbtrokkxf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.tarul.cn/Article/details/goxdncsbg.sHtML

[F12] CSV 读写
来源：http://wap.vehdjk.com/Article/details/gqjuppttq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.tarul.cn/Article/details/gdwqsemih.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.epnwcf.com/Article/details/gscbshfec.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.vehdjk.com/Article/details/gaulwuzlc.sHtML

TS:   // 同上
来源：http://www.blog.bbcook.cn/Article/details/grkqpnetl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.epnwcf.com/Article/details/givfphiro.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.sjlbkw.cn/Article/details/gaeifdnce.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fktsv.cn/Article/details/gtodngyjz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.tarul.cn/Article/details/gemxugffd.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gokehxfyd.sHtML

G. 面向对象
来源：http://m.share.epnwcf.com/Article/details/gvtewfoak.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gpyipprkj.sHtML

[G01] 定义类
来源：http://wap.tarul.cn/Article/details/gihzfftfv.sHtML

Py:   class User: pass
来源：http://www.m.share.yfazqb.com/Article/details/gxpsxcgan.sHtML

PHP:  class User {}
来源：http://3g.tarul.cn/Article/details/gdimqnpgk.sHtML

JS:   class User {}
来源：http://www.share.fktsv.cn/Article/details/gkspvxuqp.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.vehdjk.com/Article/details/gxvwzirto.sHtML

Java: class User {}
来源：http://wap.epnwcf.com/Article/details/ghfqpkmcg.sHtML

Go:   type User struct { Name string }
来源：http://m.share.tarul.cn/Article/details/gtgfvglax.sHtML

Ruby: class User; end
来源：http://www.m.share.vehdjk.com/Article/details/gpkalgwgy.sHtML

C#:   class User {}
来源：http://blog.yfazqb.com/Article/details/guqzihcjn.sHtML

[G02] 构造函数
来源：http://www.share.yfazqb.com/Article/details/gtinsvkpo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fktsv.cn/Article/details/gozsclkrr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.epnwcf.com/Article/details/gtbomkjow.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.sjlbkw.cn/Article/details/geluumjix.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gayiowzoe.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.tarul.cn/Article/details/guurbaytk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.bbcook.cn/Article/details/gmibqrvob.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.sjlbkw.cn/Article/details/gpmzvhkwn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.vehdjk.com/Article/details/gdzwxgghz.sHtML

[G03] 实例属性
来源：http://www.blog.sjlbkw.cn/Article/details/glczbcvjg.sHtML

Py:   self.name = "x"
来源：http://www.blog.fktsv.cn/Article/details/ghvajpvhk.sHtML

PHP:  public string $name = "x";
来源：http://3g.sjlbkw.cn/Article/details/ghflnpxjr.sHtML

JS:   this.name = "x";
来源：http://mobile.vehdjk.com/Article/details/gyorfiddb.sHtML

TS:   name: string = "x";
来源：http://m.share.fktsv.cn/Article/details/gmlmnmqur.sHtML

Java: private String name;
来源：http://baike.fktsv.cn/Article/details/guqepiouz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.yfazqb.com/Article/details/grjqcwyou.sHtML

Ruby: @name = "x"
来源：http://wap.sjlbkw.cn/Article/details/gnkppgpjo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fktsv.cn/Article/details/gabijwgbj.sHtML

[G04] 定义方法
来源：http://www.share.yfazqb.com/Article/details/gmtnelkvd.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.vehdjk.com/Article/details/ghxhbinur.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.vehdjk.com/Article/details/gyptsveff.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/ggbqtqacn.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.tarul.cn/Article/details/gicubqgby.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fktsv.cn/Article/details/gozliskjb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gzdvboiea.sHtML

Ruby: def greet; @name; end
来源：http://baike.sjlbkw.cn/Article/details/gwzlgatzo.sHtML

C#:   public string Greet() => Name;
来源：http://wap.bbcook.cn/Article/details/gfcjumqkw.sHtML

[G05] 继承
来源：http://read.share.bbcook.cn/Article/details/giooreaww.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.bbcook.cn/Article/details/gumuzamgb.sHtML

PHP:  class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/goskomjzt.sHtML

JS:   class Admin extends User {}
来源：http://www.share.vehdjk.com/Article/details/gfnypfaey.sHtML

TS:   class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gonbglhhi.sHtML

Java: class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gucytthzr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.vehdjk.com/Article/details/gbnhhlsto.sHtML

Ruby: class Admin < User; end
来源：http://baike.vehdjk.com/Article/details/gqnwxgfdh.sHtML

C#:   class Admin : User {}
来源：http://www.share.tarul.cn/Article/details/gwvhhvkft.sHtML

[G06] 重写方法
来源：http://baike.fktsv.cn/Article/details/gozyqrctq.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.epnwcf.com/Article/details/gphpyitnk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.tarul.cn/Article/details/gkabvlrsc.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.epnwcf.com/Article/details/gjjehbqcg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/gbppretso.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/gexbixwev.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.yfazqb.com/Article/details/gvwvsdlna.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.epnwcf.com/Article/details/gvtziixsn.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.vehdjk.com/Article/details/gophtnnfp.sHtML

[G07] 调用父类方法
来源：http://baike.epnwcf.com/Article/details/gkacneblh.sHtML

Py:   super().greet()
来源：http://wap.fktsv.cn/Article/details/gfzkerfvn.sHtML

PHP:  parent::greet();
来源：http://mobile.epnwcf.com/Article/details/gelcefxyb.sHtML

JS:   super.greet();
来源：http://baike.yfazqb.com/Article/details/gepqvzmns.sHtML

TS:   super.greet();
来源：http://read.share.tarul.cn/Article/details/gguqmhqft.sHtML

Java: super.greet();
来源：http://www.share.epnwcf.com/Article/details/gchdxtins.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.vehdjk.com/Article/details/glrlbhjbi.sHtML

Ruby: super
来源：http://m.share.bbcook.cn/Article/details/gkwbyelxc.sHtML

C#:   base.Greet();
来源：http://m.share.epnwcf.com/Article/details/gnkzxoggh.sHtML

[G08] 静态方法与属性
来源：http://baike.epnwcf.com/Article/details/gumvgxkzs.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.bbcook.cn/Article/details/gqwfmivkp.sHtML

PHP:  public static function f() {}
来源：http://mobile.fktsv.cn/Article/details/gtmfphzkh.sHtML

JS:   static f() {}
来源：http://mobile.epnwcf.com/Article/details/gvmunfixi.sHtML

TS:   static f(): void {}
来源：http://www.blog.tarul.cn/Article/details/gdrcvrrgg.sHtML

Java: static void f() {}
来源：http://baike.bbcook.cn/Article/details/gdxqjwxmq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.yfazqb.com/Article/details/geuutdpty.sHtML

Ruby: def self.f; end
来源：http://wap.tarul.cn/Article/details/gofpyllau.sHtML

C#:   public static void F() {}
来源：http://read.share.fktsv.cn/Article/details/gzhsuvqts.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.sjlbkw.cn/Article/details/gejzcvtew.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.tarul.cn/Article/details/ghmwtxpnv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fktsv.cn/Article/details/gttmmdsud.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.epnwcf.com/Article/details/gnnsokyki.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.yfazqb.com/Article/details/gfnjvfsst.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.epnwcf.com/Article/details/gpjxudzgh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.sjlbkw.cn/Article/details/gamydfmvd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.vehdjk.com/Article/details/ggmkfhslt.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.vehdjk.com/Article/details/gwkdzqubg.sHtML

[G10] 访问控制
来源：http://mobile.tarul.cn/Article/details/gcxktaliz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.epnwcf.com/Article/details/gthcimayc.sHtML

PHP:  public / protected / private
来源：http://www.m.share.epnwcf.com/Article/details/gzwtwqvzs.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fktsv.cn/Article/details/gvfgncdgq.sHtML

TS:   public / protected / private
来源：http://read.share.sjlbkw.cn/Article/details/gqsjifqzc.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.yfazqb.com/Article/details/gqyebywbe.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.epnwcf.com/Article/details/gqfltzjxu.sHtML

Ruby: public / protected / private
来源：http://www.share.bbcook.cn/Article/details/gjgjuwmth.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.epnwcf.com/Article/details/gcuwlpxrc.sHtML

[G11] getter / setter
来源：http://3g.yfazqb.com/Article/details/gzmdhbjgy.sHtML

Py:   @property 与 @x.setter
来源：http://blog.tarul.cn/Article/details/gfycoqzcd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.bbcook.cn/Article/details/gkltdumqb.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.tarul.cn/Article/details/ggkmrsmjb.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.epnwcf.com/Article/details/geeplayly.sHtML

Java: public String getName() { return name; }
来源：http://m.share.epnwcf.com/Article/details/gkxroqzrv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.bbcook.cn/Article/details/gwxhjcutp.sHtML

Ruby: attr_accessor :name
来源：http://read.share.bbcook.cn/Article/details/grshzztlk.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.tarul.cn/Article/details/guucdvbww.sHtML

[G12] 对象转字符串
来源：http://www.blog.tarul.cn/Article/details/glaqrobrr.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.sjlbkw.cn/Article/details/geromgwsl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.epnwcf.com/Article/details/geinexjbv.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gexgqkssl.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gjgwzxyzy.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gcstdehyw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.tarul.cn/Article/details/glhhzfgkz.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fktsv.cn/Article/details/gcilkdjmo.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fktsv.cn/Article/details/gwasvqnzy.sHtML

[G13] 判断对象类型
来源：http://mobile.yfazqb.com/Article/details/gebgjicjr.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.yfazqb.com/Article/details/gbyairpnm.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.yfazqb.com/Article/details/gendhleud.sHtML

JS:   u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/gwucuefci.sHtML

TS:   u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/gwfzbwkwy.sHtML

Java: u instanceof User
来源：http://baike.tarul.cn/Article/details/gkkhaocdw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.vehdjk.com/Article/details/gnsaluqfu.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.vehdjk.com/Article/details/gxthcyizw.sHtML

C#:   u is User
来源：http://m.share.bbcook.cn/Article/details/gqtkghrha.sHtML

[G14] 数据类 / record
来源：http://wap.tarul.cn/Article/details/gdthfbvbd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.epnwcf.com/Article/details/gnaizaocj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.vehdjk.com/Article/details/gugxubvth.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.tarul.cn/Article/details/ghikvjfyt.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fktsv.cn/Article/details/gzdzhsxdf.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.vehdjk.com/Article/details/gkvkwtfbk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.bbcook.cn/Article/details/gkhsxwoqj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.vehdjk.com/Article/details/gaitdkwop.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.epnwcf.com/Article/details/gvktghilp.sHtML

[G15] 枚举
来源：http://www.m.share.bbcook.cn/Article/details/gjehnintl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.bbcook.cn/Article/details/ggqdafjxe.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.bbcook.cn/Article/details/ggyetujye.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fktsv.cn/Article/details/gsczwestq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fktsv.cn/Article/details/glhrxotdu.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fktsv.cn/Article/details/gztckbcsv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.sjlbkw.cn/Article/details/ganbunime.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.tarul.cn/Article/details/gsxoaaxml.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.sjlbkw.cn/Article/details/gyxzlqorm.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.epnwcf.com/Article/details/gqslloovh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.yfazqb.com/Article/details/gwcquoofn.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.epnwcf.com/Article/details/gogqecbnl.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.yfazqb.com/Article/details/gamhtzvic.sHtML

TS:   Object.entries(obj)
来源：http://www.share.bbcook.cn/Article/details/gxybbxqqm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.bbcook.cn/Article/details/gfphrzmoa.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.epnwcf.com/Article/details/gwzivcfio.sHtML

Ruby: obj.instance_variables
来源：http://www.share.vehdjk.com/Article/details/gshuyksii.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.epnwcf.com/Article/details/gztorhymw.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gdbwqvxlv.sHtML

H. 异常与错误处理
来源：http://www.share.sjlbkw.cn/Article/details/gniwabovl.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gkipkpipa.sHtML

[H01] try / catch 基础
来源：http://blog.sjlbkw.cn/Article/details/gdiicrxnv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.yfazqb.com/Article/details/geyxaklfu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.bbcook.cn/Article/details/gjkldwjph.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.vehdjk.com/Article/details/gnhawmfyc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.yfazqb.com/Article/details/guekxgumb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fktsv.cn/Article/details/gmejxlncs.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.sjlbkw.cn/Article/details/gawvptqej.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.vehdjk.com/Article/details/gqhsusgaq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.sjlbkw.cn/Article/details/gcrqxhkdf.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.tarul.cn/Article/details/gxwzjbtzc.sHtML


<!-- 参考信息 -->