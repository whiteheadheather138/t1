代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.bbcook.cn/Article/details/gpbqphenz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.yfazqb.com/Article/details/gpmcxjlqd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.tarul.cn/Article/details/gymvzlmmn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fktsv.cn/Article/details/govfgosbo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fktsv.cn/Article/details/gyevpwcpu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.sjlbkw.cn/Article/details/gyejdwydh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/gshahiklz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.epnwcf.com/Article/details/gewkdqhem.sHtML

[E22] 字节长度与字符长度
来源：http://wap.tarul.cn/Article/details/glonkiryj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.yfazqb.com/Article/details/gtlwesxcw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.yfazqb.com/Article/details/ggypqeysm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.epnwcf.com/Article/details/ghyfxyfic.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.bbcook.cn/Article/details/gkiggevgk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.epnwcf.com/Article/details/gdegtjguk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.sjlbkw.cn/Article/details/ghvtazlfo.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fktsv.cn/Article/details/ginunycgo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.vehdjk.com/Article/details/gqztxwxju.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gqkuuxrlu.sHtML

F. 文件与目录
来源：http://mobile.epnwcf.com/Article/details/goioevtxj.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/grktttwtr.sHtML

[F01] 读取整个文件
来源：http://wap.bbcook.cn/Article/details/gbxgsmstx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.yfazqb.com/Article/details/gteurqioh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.vehdjk.com/Article/details/gmikuzfpf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.vehdjk.com/Article/details/grjlmsfqk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fktsv.cn/Article/details/gfwpxxdqa.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gohgdwsmu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.epnwcf.com/Article/details/gsskudhjb.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fktsv.cn/Article/details/gsuuuwlrl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gjjmwaqba.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.tarul.cn/Article/details/gcykfuxnz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.vehdjk.com/Article/details/gqkqybeex.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.yfazqb.com/Article/details/gopsextas.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.bbcook.cn/Article/details/gzgrphewg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.sjlbkw.cn/Article/details/gvyjcvmqa.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.vehdjk.com/Article/details/gfirkebui.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.tarul.cn/Article/details/ggctycaop.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.yfazqb.com/Article/details/gdyynllwi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.tarul.cn/Article/details/gqhaiosuv.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.vehdjk.com/Article/details/gzafhpcmc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.sjlbkw.cn/Article/details/gundudepc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.yfazqb.com/Article/details/gyclisvcr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.epnwcf.com/Article/details/gzklvwozx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fktsv.cn/Article/details/gekuafvee.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fktsv.cn/Article/details/geumwtgzv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.tarul.cn/Article/details/gpazcmtlf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fktsv.cn/Article/details/gitiajqdt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.yfazqb.com/Article/details/gjifjowzx.sHtML

[F04] 追加写入文件
来源：http://m.share.fktsv.cn/Article/details/gvyqbjjdq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.yfazqb.com/Article/details/gtjuqdhxn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.tarul.cn/Article/details/gmrtqwxnx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fktsv.cn/Article/details/gigvglyqz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.yfazqb.com/Article/details/gncdfvgmr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.sjlbkw.cn/Article/details/gtqpttxkk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.vehdjk.com/Article/details/gcfseoril.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.epnwcf.com/Article/details/ghfmqeujl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fktsv.cn/Article/details/gzalqdasx.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.bbcook.cn/Article/details/gmkwbcseo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.vehdjk.com/Article/details/gogaydizj.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.tarul.cn/Article/details/ghpkvnxpt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.tarul.cn/Article/details/ggqaprhxe.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gdmkomejk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/gnekatggf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.yfazqb.com/Article/details/gfdzgskrw.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gzpjsnule.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gihokdjbt.sHtML

[F06] 删除文件
来源：http://wap.tarul.cn/Article/details/gsbbmghqg.sHtML

Py:   os.remove("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gvjtoxvmv.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gnavoqzho.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/glykqfgoi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/guptnkyot.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/gqkugrxlk.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.yfazqb.com/Article/details/gnjvqpcky.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.epnwcf.com/Article/details/gvymljrbe.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gonrxrxhf.sHtML

[F07] 创建目录（含多级）
来源：http://3g.vehdjk.com/Article/details/gwrdbaxzn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fktsv.cn/Article/details/giexixfgx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fktsv.cn/Article/details/gcxhmappu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.yfazqb.com/Article/details/gdtqntycq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.sjlbkw.cn/Article/details/gzipfeeln.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.bbcook.cn/Article/details/gtltblhwr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.bbcook.cn/Article/details/ggzckisei.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.epnwcf.com/Article/details/gurnbgfdb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.tarul.cn/Article/details/gwtdkelcm.sHtML

[F08] 遍历目录
来源：http://www.share.sjlbkw.cn/Article/details/ghwibyxkk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.bbcook.cn/Article/details/gdgwdqsva.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.tarul.cn/Article/details/gfmampwlv.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fktsv.cn/Article/details/gqhnkbmsr.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.sjlbkw.cn/Article/details/gwpnbifkv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fktsv.cn/Article/details/gfvivssha.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.tarul.cn/Article/details/grqsefdov.sHtML

Ruby: Dir.children("dir")
来源：http://wap.sjlbkw.cn/Article/details/gjajtgrxx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.epnwcf.com/Article/details/gzdahzysa.sHtML

[F09] 获取文件大小
来源：http://m.share.yfazqb.com/Article/details/ghpwomgni.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.tarul.cn/Article/details/ggglontle.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gcfzghuaz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.yfazqb.com/Article/details/getrlbyay.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.yfazqb.com/Article/details/grfubpplz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/gcplsdymb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fktsv.cn/Article/details/gjiyyznml.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gkivobfcl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.sjlbkw.cn/Article/details/gbszxjjdt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.vehdjk.com/Article/details/gamvwxrhf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gjvljkdfb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gqklidraw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gssbcfoxz.sHtML

TS:   path.extname("a.txt")
来源：http://wap.epnwcf.com/Article/details/ggkdrxxws.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.vehdjk.com/Article/details/gytbhkjac.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gxpvcuojy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/godazocwv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gkbqbjlbc.sHtML

[F11] 复制与移动文件
来源：http://m.share.yfazqb.com/Article/details/gqezaptni.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gfsjxtavi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.bbcook.cn/Article/details/gsswqdwyl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/gbmxyvvyr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gcfgbyzeg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.tarul.cn/Article/details/gfmovahpz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.tarul.cn/Article/details/gldrzlkoo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/gphhgwkae.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.yfazqb.com/Article/details/ggyjnsukf.sHtML

[F12] CSV 读写
来源：http://m.share.tarul.cn/Article/details/gjcntanek.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.bbcook.cn/Article/details/gmoksaeck.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.vehdjk.com/Article/details/gwjaqxdzl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.yfazqb.com/Article/details/gdaawalor.sHtML

TS:   // 同上
来源：http://mobile.tarul.cn/Article/details/gugijocdj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.bbcook.cn/Article/details/gohvqqnfa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.vehdjk.com/Article/details/gswuboyxg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.bbcook.cn/Article/details/gsqczrxrp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.tarul.cn/Article/details/gljhmwbsy.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/goxquujnj.sHtML

G. 面向对象
来源：http://3g.bbcook.cn/Article/details/gpblhvuzn.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gtairxeby.sHtML

[G01] 定义类
来源：http://m.share.tarul.cn/Article/details/gewpckmib.sHtML

Py:   class User: pass
来源：http://read.share.bbcook.cn/Article/details/gfyrmmkfw.sHtML

PHP:  class User {}
来源：http://mobile.sjlbkw.cn/Article/details/gsahtmxdq.sHtML

JS:   class User {}
来源：http://www.share.tarul.cn/Article/details/gunldtfqv.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.epnwcf.com/Article/details/guzhxavkl.sHtML

Java: class User {}
来源：http://www.share.sjlbkw.cn/Article/details/gqfgeakxf.sHtML

Go:   type User struct { Name string }
来源：http://3g.fktsv.cn/Article/details/gfqklzxxk.sHtML

Ruby: class User; end
来源：http://m.share.tarul.cn/Article/details/gvugmuevx.sHtML

C#:   class User {}
来源：http://read.share.yfazqb.com/Article/details/gkammmzgh.sHtML

[G02] 构造函数
来源：http://m.share.yfazqb.com/Article/details/gpkgwyudf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.vehdjk.com/Article/details/gjdksjhov.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.epnwcf.com/Article/details/gizgifhlm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.epnwcf.com/Article/details/geztybcfc.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.tarul.cn/Article/details/grmehtsgq.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.tarul.cn/Article/details/goyzstmch.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.vehdjk.com/Article/details/gzgrhkdda.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.bbcook.cn/Article/details/glizovnce.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fktsv.cn/Article/details/gralfcdsj.sHtML

[G03] 实例属性
来源：http://mobile.epnwcf.com/Article/details/ghkjqgxwr.sHtML

Py:   self.name = "x"
来源：http://www.share.vehdjk.com/Article/details/grucutfyn.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fktsv.cn/Article/details/guslmoqzh.sHtML

JS:   this.name = "x";
来源：http://www.blog.fktsv.cn/Article/details/gmoggeamd.sHtML

TS:   name: string = "x";
来源：http://blog.vehdjk.com/Article/details/gwczimyxm.sHtML

Java: private String name;
来源：http://www.m.share.vehdjk.com/Article/details/gpvfoyhit.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.bbcook.cn/Article/details/gpuorgcke.sHtML

Ruby: @name = "x"
来源：http://3g.fktsv.cn/Article/details/gwdvchlgx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fktsv.cn/Article/details/gnixrskes.sHtML

[G04] 定义方法
来源：http://blog.epnwcf.com/Article/details/grlteuxko.sHtML

Py:   def greet(self): return self.name
来源：http://baike.bbcook.cn/Article/details/gkbctpikk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.yfazqb.com/Article/details/gdbwekktu.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.bbcook.cn/Article/details/gwesddzke.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.vehdjk.com/Article/details/guqkzcuws.sHtML

Java: String greet() { return name; }
来源：http://mobile.bbcook.cn/Article/details/gitopawhv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fktsv.cn/Article/details/gkvknsdzm.sHtML

Ruby: def greet; @name; end
来源：http://blog.yfazqb.com/Article/details/gdhdkzhpj.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.bbcook.cn/Article/details/gjtkeeayd.sHtML

[G05] 继承
来源：http://www.share.fktsv.cn/Article/details/gscbatjvh.sHtML

Py:   class Admin(User): pass
来源：http://m.share.sjlbkw.cn/Article/details/gclyqkozt.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gnvnhczwt.sHtML

JS:   class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/ghhaiyxif.sHtML

TS:   class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/gcxjrftlt.sHtML

Java: class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/gjxansycj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.vehdjk.com/Article/details/gseylnrhh.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.yfazqb.com/Article/details/gfochpvrx.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fktsv.cn/Article/details/gmvqcdhsv.sHtML

[G06] 重写方法
来源：http://m.share.fktsv.cn/Article/details/gtftdblbc.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fktsv.cn/Article/details/gzunnelzw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gofgnyygm.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.vehdjk.com/Article/details/gogzbkxkh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gsldvihsv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.tarul.cn/Article/details/gxhnqvkdg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.vehdjk.com/Article/details/gtkthtokk.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.bbcook.cn/Article/details/gndkkcfnj.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.epnwcf.com/Article/details/gbniogrnl.sHtML

[G07] 调用父类方法
来源：http://mobile.bbcook.cn/Article/details/giacheoil.sHtML

Py:   super().greet()
来源：http://www.m.share.tarul.cn/Article/details/gjifinpqd.sHtML

PHP:  parent::greet();
来源：http://www.share.tarul.cn/Article/details/gxelftjbn.sHtML

JS:   super.greet();
来源：http://www.share.bbcook.cn/Article/details/gktkwxskv.sHtML

TS:   super.greet();
来源：http://www.m.share.vehdjk.com/Article/details/gavlckeow.sHtML

Java: super.greet();
来源：http://www.blog.fktsv.cn/Article/details/gsecoyshk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.epnwcf.com/Article/details/glaxyprrz.sHtML

Ruby: super
来源：http://www.blog.yfazqb.com/Article/details/gakwoxmlg.sHtML

C#:   base.Greet();
来源：http://read.share.tarul.cn/Article/details/gxberyvgq.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.sjlbkw.cn/Article/details/goeyyydva.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.tarul.cn/Article/details/glqigzyyp.sHtML

PHP:  public static function f() {}
来源：http://baike.epnwcf.com/Article/details/gybxvanwz.sHtML

JS:   static f() {}
来源：http://baike.fktsv.cn/Article/details/gdopsilfy.sHtML

TS:   static f(): void {}
来源：http://m.share.fktsv.cn/Article/details/gbfkfroaz.sHtML

Java: static void f() {}
来源：http://wap.fktsv.cn/Article/details/gyriicslk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.vehdjk.com/Article/details/glzhdkmxg.sHtML

Ruby: def self.f; end
来源：http://blog.tarul.cn/Article/details/gpntsvycj.sHtML

C#:   public static void F() {}
来源：http://3g.tarul.cn/Article/details/gwojzonxn.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.tarul.cn/Article/details/gfrvvfoqg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fktsv.cn/Article/details/gmpejkhxl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.vehdjk.com/Article/details/gmtoptjtk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.epnwcf.com/Article/details/ginkoqhau.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.vehdjk.com/Article/details/gdnuosanv.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.bbcook.cn/Article/details/gdztrfznm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fktsv.cn/Article/details/gpnzkgojf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.tarul.cn/Article/details/gkqixbgto.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.tarul.cn/Article/details/goqzywfkq.sHtML

[G10] 访问控制
来源：http://3g.bbcook.cn/Article/details/gbqlstamd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.tarul.cn/Article/details/gdlnscowm.sHtML

PHP:  public / protected / private
来源：http://3g.tarul.cn/Article/details/gdcwtphcc.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.bbcook.cn/Article/details/gtubfyrwm.sHtML

TS:   public / protected / private
来源：http://www.share.epnwcf.com/Article/details/gralvddya.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.sjlbkw.cn/Article/details/gytgzjahb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.yfazqb.com/Article/details/gpidubzjg.sHtML

Ruby: public / protected / private
来源：http://blog.sjlbkw.cn/Article/details/grgwrnkis.sHtML

C#:   public / protected / private / internal
来源：http://m.share.epnwcf.com/Article/details/ghczayqsi.sHtML

[G11] getter / setter
来源：http://3g.bbcook.cn/Article/details/gqueqoypy.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.bbcook.cn/Article/details/gyzdtykwy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.yfazqb.com/Article/details/gxyycchzf.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.vehdjk.com/Article/details/gtzrczznv.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.epnwcf.com/Article/details/geddfmheu.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gvxzqsoei.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.bbcook.cn/Article/details/gqnipgvck.sHtML

Ruby: attr_accessor :name
来源：http://3g.epnwcf.com/Article/details/ghnacrdzv.sHtML

C#:   public string Name { get; set; }
来源：http://baike.yfazqb.com/Article/details/gzbcmqpad.sHtML

[G12] 对象转字符串
来源：http://www.share.tarul.cn/Article/details/gygbbuivc.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.sjlbkw.cn/Article/details/gumrgiepv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.sjlbkw.cn/Article/details/gffpdsqev.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fktsv.cn/Article/details/ginumiork.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/gjdjvgmby.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.vehdjk.com/Article/details/gpunwsiel.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/gfnxdlggj.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.bbcook.cn/Article/details/ghvzugiuq.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.tarul.cn/Article/details/gbdciyyib.sHtML

[G13] 判断对象类型
来源：http://www.share.bbcook.cn/Article/details/gzuabwdrh.sHtML

Py:   isinstance(u, User)
来源：http://m.share.tarul.cn/Article/details/gxssrwtvf.sHtML

PHP:  $u instanceof User
来源：http://mobile.fktsv.cn/Article/details/ggimvxgfb.sHtML

JS:   u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/gnwzeydod.sHtML

TS:   u instanceof User
来源：http://mobile.bbcook.cn/Article/details/gplyzkfsi.sHtML

Java: u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gnkxkhwev.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.epnwcf.com/Article/details/grgmpmjwz.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.sjlbkw.cn/Article/details/gisvamijh.sHtML

C#:   u is User
来源：http://baike.sjlbkw.cn/Article/details/ghzstbltd.sHtML

[G14] 数据类 / record
来源：http://blog.sjlbkw.cn/Article/details/gmdnfttmx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.sjlbkw.cn/Article/details/gaarblpxo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.vehdjk.com/Article/details/gdhdmfrig.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.vehdjk.com/Article/details/gciriqtty.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.vehdjk.com/Article/details/gsquotdik.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.vehdjk.com/Article/details/geguxgyhp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.sjlbkw.cn/Article/details/gemydwyjr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.yfazqb.com/Article/details/gkufyjjdv.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.yfazqb.com/Article/details/guhfzgmuv.sHtML

[G15] 枚举
来源：http://www.share.yfazqb.com/Article/details/gbatoxrov.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.tarul.cn/Article/details/gxbyasuec.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.bbcook.cn/Article/details/gznqacxch.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.epnwcf.com/Article/details/gchpsapkc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.sjlbkw.cn/Article/details/glbkndqub.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fktsv.cn/Article/details/gwjpqxdic.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fktsv.cn/Article/details/ghhekdhzp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.tarul.cn/Article/details/grjsjwioc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.epnwcf.com/Article/details/govftgvvw.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.epnwcf.com/Article/details/ghxdpamjn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.yfazqb.com/Article/details/gvmvuufsl.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.sjlbkw.cn/Article/details/gercqljbd.sHtML

JS:   Object.entries(obj)
来源：http://wap.epnwcf.com/Article/details/gzfgdahxb.sHtML

TS:   Object.entries(obj)
来源：http://wap.tarul.cn/Article/details/gkkfdfqil.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.bbcook.cn/Article/details/gzzhjnwlx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.sjlbkw.cn/Article/details/gyzuwqtxr.sHtML

Ruby: obj.instance_variables
来源：http://3g.sjlbkw.cn/Article/details/grwlnmfwq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fktsv.cn/Article/details/gvgldtdgh.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/godlewfmi.sHtML

H. 异常与错误处理
来源：http://read.share.epnwcf.com/Article/details/gxeuqkmdj.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gmwntdexx.sHtML

[H01] try / catch 基础
来源：http://baike.epnwcf.com/Article/details/gutwzlyzv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.tarul.cn/Article/details/ghuhqnjmj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.yfazqb.com/Article/details/galurfqgs.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.tarul.cn/Article/details/gdbxqopnu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.bbcook.cn/Article/details/gwybipmkz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.bbcook.cn/Article/details/gbboywini.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.vehdjk.com/Article/details/ghyejktcv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.bbcook.cn/Article/details/gyrgaxcrk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.epnwcf.com/Article/details/ggyikuxsw.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fktsv.cn/Article/details/gioficvip.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.bbcook.cn/Article/details/gcljiffvo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.epnwcf.com/Article/details/gveutygee.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gaaboqslu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gugepegyv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.tarul.cn/Article/details/ghdwivwtg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fktsv.cn/Article/details/gghgnipnb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.tarul.cn/Article/details/gylzwmbfg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gbsncagnl.sHtML

[H03] 主动抛出异常
来源：http://wap.yfazqb.com/Article/details/gqdorfear.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.bbcook.cn/Article/details/gxexqcomv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/gergvwdgb.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.epnwcf.com/Article/details/glagullwy.sHtML


<!-- 参考信息 -->