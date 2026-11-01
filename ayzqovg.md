代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.epnwcf.com/Article/details/glnnmmwzg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.yfazqb.com/Article/details/gguygiwod.sHtML

TS:   if (s === "") {}
来源：http://mobile.bbcook.cn/Article/details/gbpvnweov.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.epnwcf.com/Article/details/gmmnemsra.sHtML

Go:   if s == "" {}
来源：http://3g.bbcook.cn/Article/details/gbupnlenq.sHtML

Ruby: if s.empty?
来源：http://baike.epnwcf.com/Article/details/ggyujkytb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.bbcook.cn/Article/details/gwhnakgst.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fktsv.cn/Article/details/gguirxxdp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fktsv.cn/Article/details/gnmdckwpo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.tarul.cn/Article/details/gsddvaral.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.yfazqb.com/Article/details/gcwxwftbw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fktsv.cn/Article/details/gtwthvxfl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.epnwcf.com/Article/details/glvmpoinr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fktsv.cn/Article/details/gxqvtverk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.tarul.cn/Article/details/gwpmgkjxr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.tarul.cn/Article/details/gwghnzfze.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fktsv.cn/Article/details/grcezmioe.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.vehdjk.com/Article/details/gwlhebnbt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/gqlhlhdka.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.bbcook.cn/Article/details/gfkaijmiy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.bbcook.cn/Article/details/gpdhdynhs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.tarul.cn/Article/details/galhipcmm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fktsv.cn/Article/details/gehgziipn.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.vehdjk.com/Article/details/gktpeutph.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.yfazqb.com/Article/details/gsjjvthin.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/glquqotqe.sHtML

F. 文件与目录
来源：http://www.share.epnwcf.com/Article/details/gftrqchtu.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gmvnzxvnh.sHtML

[F01] 读取整个文件
来源：http://www.m.share.epnwcf.com/Article/details/gijithrwt.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fktsv.cn/Article/details/gysyheqks.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gcpmdixsm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.yfazqb.com/Article/details/geherishh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.yfazqb.com/Article/details/gczjzapuu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.yfazqb.com/Article/details/gqhlkhdsk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fktsv.cn/Article/details/gouhhwpga.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gqegzbqsl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.vehdjk.com/Article/details/grwvihcan.sHtML

[F02] 逐行读取文件
来源：http://baike.sjlbkw.cn/Article/details/gwybpazwv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.tarul.cn/Article/details/geaknepsa.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.tarul.cn/Article/details/gzrfjddps.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.sjlbkw.cn/Article/details/gbccbosit.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.vehdjk.com/Article/details/gkmkiltra.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.bbcook.cn/Article/details/gvnqpajxx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.sjlbkw.cn/Article/details/gghsytgma.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.tarul.cn/Article/details/ggfdijwke.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.bbcook.cn/Article/details/gbtvgyifl.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.vehdjk.com/Article/details/goqmrzdlv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.sjlbkw.cn/Article/details/gyucdsaxp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.sjlbkw.cn/Article/details/gudmluxqg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.yfazqb.com/Article/details/gqharwenm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fktsv.cn/Article/details/gjphzjmaj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.yfazqb.com/Article/details/gnkcwqery.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.yfazqb.com/Article/details/gaqehexqg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.sjlbkw.cn/Article/details/gwqhtorrd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.yfazqb.com/Article/details/ghyrvbnme.sHtML

[F04] 追加写入文件
来源：http://www.blog.tarul.cn/Article/details/gutzyhgdi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.vehdjk.com/Article/details/gvkvycimy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.sjlbkw.cn/Article/details/guyrgurku.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fktsv.cn/Article/details/gqjhxatvs.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.tarul.cn/Article/details/gqgmmtuqf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.vehdjk.com/Article/details/gaixxjgmw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.vehdjk.com/Article/details/gzbmbqpjq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.sjlbkw.cn/Article/details/gczmkvofm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.sjlbkw.cn/Article/details/gtgcirxgj.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.sjlbkw.cn/Article/details/gxgucuzwx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.epnwcf.com/Article/details/gjdkvtcpb.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gnbgpaghp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/gqivphibz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gdyrqbafg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/gnvqammqr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.sjlbkw.cn/Article/details/grchmmyzs.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gwpipeipi.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.bbcook.cn/Article/details/gtwypoblc.sHtML

[F06] 删除文件
来源：http://www.m.share.yfazqb.com/Article/details/gxnjqqohm.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.bbcook.cn/Article/details/geybcolwy.sHtML

PHP:  unlink("a.txt");
来源：http://baike.bbcook.cn/Article/details/gjcvtwele.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/geswitqyf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.vehdjk.com/Article/details/gxdlexdbr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/gecboxzlg.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gjsrenjph.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.bbcook.cn/Article/details/grjcymzkl.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gumycguqc.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.sjlbkw.cn/Article/details/ghootafav.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.sjlbkw.cn/Article/details/ghocbyzjh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.epnwcf.com/Article/details/ggztfaiok.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.bbcook.cn/Article/details/gloinuose.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.epnwcf.com/Article/details/glxvwzbys.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gexjpzjsu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.bbcook.cn/Article/details/gghcutpnt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.vehdjk.com/Article/details/gckpakffa.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.yfazqb.com/Article/details/gaaismgsj.sHtML

[F08] 遍历目录
来源：http://mobile.fktsv.cn/Article/details/gfblyduqp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmcgchyrm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.vehdjk.com/Article/details/gcxkzrnwz.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.bbcook.cn/Article/details/gjjoxnnft.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.sjlbkw.cn/Article/details/gtypzolfi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.sjlbkw.cn/Article/details/gsyksxltx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.yfazqb.com/Article/details/gjzdlllyi.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.epnwcf.com/Article/details/gdyvbrngl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gdpnpvuiw.sHtML

[F09] 获取文件大小
来源：http://3g.tarul.cn/Article/details/giwuufbnk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjqsrfgp.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gmfvqndkj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fktsv.cn/Article/details/gnqmdjikf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fktsv.cn/Article/details/gyzgwcoxv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.vehdjk.com/Article/details/ghcpyzdrg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.yfazqb.com/Article/details/gltosegiu.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fktsv.cn/Article/details/geawvhpwz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.bbcook.cn/Article/details/gcxhefhhs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.bbcook.cn/Article/details/gsmizbshx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gakwsisqu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.bbcook.cn/Article/details/gehhqhwys.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gebqvksnq.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gyizwtpnm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.epnwcf.com/Article/details/gkbauhhps.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gcerbdjxm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/gjeyyupfs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gmbvbymmo.sHtML

[F11] 复制与移动文件
来源：http://m.share.yfazqb.com/Article/details/gawyiqtdc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/gsadidixl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.vehdjk.com/Article/details/gmooombab.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/ggidguwuy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/gibrqtttt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.yfazqb.com/Article/details/gkwoffpik.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fktsv.cn/Article/details/gcwnqltsl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gtlgiixha.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.epnwcf.com/Article/details/gqyfqxvfv.sHtML

[F12] CSV 读写
来源：http://baike.sjlbkw.cn/Article/details/glnfvjpfq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fktsv.cn/Article/details/gjiztiaqp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fktsv.cn/Article/details/gfyrywofp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.epnwcf.com/Article/details/gpdsodpfw.sHtML

TS:   // 同上
来源：http://m.share.tarul.cn/Article/details/gcguvbbnh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.sjlbkw.cn/Article/details/ggwyejktv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.sjlbkw.cn/Article/details/gnvqzqahc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.tarul.cn/Article/details/gvdsvlhho.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.yfazqb.com/Article/details/gdkoajwpf.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gckhsolsr.sHtML

G. 面向对象
来源：http://wap.fktsv.cn/Article/details/giidynebu.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gtktlxiqs.sHtML

[G01] 定义类
来源：http://mobile.fktsv.cn/Article/details/glqjcbflx.sHtML

Py:   class User: pass
来源：http://wap.sjlbkw.cn/Article/details/gabxsvrqj.sHtML

PHP:  class User {}
来源：http://www.blog.epnwcf.com/Article/details/gnjmcqijw.sHtML

JS:   class User {}
来源：http://www.blog.fktsv.cn/Article/details/gdnbsjixi.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fktsv.cn/Article/details/gvosawsht.sHtML

Java: class User {}
来源：http://blog.tarul.cn/Article/details/gdvmcbjez.sHtML

Go:   type User struct { Name string }
来源：http://blog.bbcook.cn/Article/details/gtoyhoddp.sHtML

Ruby: class User; end
来源：http://baike.vehdjk.com/Article/details/gqlppwcyx.sHtML

C#:   class User {}
来源：http://wap.sjlbkw.cn/Article/details/gudfwlxck.sHtML

[G02] 构造函数
来源：http://blog.sjlbkw.cn/Article/details/gzutttysv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.tarul.cn/Article/details/gfejrubjz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.yfazqb.com/Article/details/gzcluaypc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.bbcook.cn/Article/details/gjuugcbre.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.yfazqb.com/Article/details/gqnxgjdoh.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjrpyagsw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.bbcook.cn/Article/details/gjnejcdkh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.yfazqb.com/Article/details/ghjitqpau.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.epnwcf.com/Article/details/gszslbshr.sHtML

[G03] 实例属性
来源：http://3g.yfazqb.com/Article/details/gtgfibchq.sHtML

Py:   self.name = "x"
来源：http://wap.yfazqb.com/Article/details/gihyhlqel.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fktsv.cn/Article/details/gqslnkdmm.sHtML

JS:   this.name = "x";
来源：http://www.blog.yfazqb.com/Article/details/gxkofochq.sHtML

TS:   name: string = "x";
来源：http://m.share.yfazqb.com/Article/details/gyqvdttvp.sHtML

Java: private String name;
来源：http://www.m.share.vehdjk.com/Article/details/ghmwbmybm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.yfazqb.com/Article/details/gftwbqcfh.sHtML

Ruby: @name = "x"
来源：http://www.m.share.vehdjk.com/Article/details/grunvfbcx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.yfazqb.com/Article/details/gbygawvvs.sHtML

[G04] 定义方法
来源：http://wap.vehdjk.com/Article/details/gidvuoaus.sHtML

Py:   def greet(self): return self.name
来源：http://baike.bbcook.cn/Article/details/gofhvzwar.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.vehdjk.com/Article/details/gbxylaetn.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gdsenuayo.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gntfzcfxy.sHtML

Java: String greet() { return name; }
来源：http://baike.yfazqb.com/Article/details/grfwxznjp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.yfazqb.com/Article/details/ghavwyrrg.sHtML

Ruby: def greet; @name; end
来源：http://www.share.epnwcf.com/Article/details/gwzagcink.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.epnwcf.com/Article/details/gumsqjdjf.sHtML

[G05] 继承
来源：http://www.blog.epnwcf.com/Article/details/gzteidbpw.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.epnwcf.com/Article/details/gdtoyjgqt.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/ggsqyejkw.sHtML

JS:   class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/gfxvcoopr.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/gzgmngwte.sHtML

Java: class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gffmmqqzy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.tarul.cn/Article/details/gdrkrquna.sHtML

Ruby: class Admin < User; end
来源：http://baike.sjlbkw.cn/Article/details/gfndplier.sHtML

C#:   class Admin : User {}
来源：http://mobile.vehdjk.com/Article/details/gixmxacsn.sHtML

[G06] 重写方法
来源：http://m.share.sjlbkw.cn/Article/details/gmsxdkcdl.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.epnwcf.com/Article/details/ghqejugjj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.sjlbkw.cn/Article/details/gtbdyqxyt.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/godauoerx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/gpwoxverk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/glqaomott.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.yfazqb.com/Article/details/gorejewvb.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.bbcook.cn/Article/details/gcyzqgtkr.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fktsv.cn/Article/details/gsipuxrax.sHtML

[G07] 调用父类方法
来源：http://3g.tarul.cn/Article/details/gpwisueip.sHtML

Py:   super().greet()
来源：http://3g.sjlbkw.cn/Article/details/gwbsgimzf.sHtML

PHP:  parent::greet();
来源：http://read.share.tarul.cn/Article/details/gehpvziad.sHtML

JS:   super.greet();
来源：http://baike.epnwcf.com/Article/details/gtrskqxvp.sHtML

TS:   super.greet();
来源：http://baike.bbcook.cn/Article/details/gvwyzybpl.sHtML

Java: super.greet();
来源：http://www.blog.epnwcf.com/Article/details/gnegqmiij.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fktsv.cn/Article/details/gqbxfajzy.sHtML

Ruby: super
来源：http://blog.yfazqb.com/Article/details/gkozsnlwz.sHtML

C#:   base.Greet();
来源：http://blog.tarul.cn/Article/details/gqsxswfow.sHtML

[G08] 静态方法与属性
来源：http://read.share.vehdjk.com/Article/details/gsvgdzssh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.vehdjk.com/Article/details/gqiwobhux.sHtML

PHP:  public static function f() {}
来源：http://3g.epnwcf.com/Article/details/gluyoxcgm.sHtML

JS:   static f() {}
来源：http://baike.epnwcf.com/Article/details/gddznnkmq.sHtML

TS:   static f(): void {}
来源：http://mobile.epnwcf.com/Article/details/gntffnuri.sHtML

Java: static void f() {}
来源：http://baike.vehdjk.com/Article/details/grjkgiwvo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.sjlbkw.cn/Article/details/ghcsczegr.sHtML

Ruby: def self.f; end
来源：http://read.share.sjlbkw.cn/Article/details/gspicobiq.sHtML

C#:   public static void F() {}
来源：http://www.share.yfazqb.com/Article/details/gsadcdvhq.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.vehdjk.com/Article/details/gloywcotm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.sjlbkw.cn/Article/details/gibgfikgf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.epnwcf.com/Article/details/ghgstrvga.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.yfazqb.com/Article/details/gnagthbet.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.tarul.cn/Article/details/grflhortz.sHtML

Java: interface Shape { double area(); }
来源：http://baike.epnwcf.com/Article/details/gttrkducs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.yfazqb.com/Article/details/gikulgiva.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.vehdjk.com/Article/details/gfrezgwhz.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fktsv.cn/Article/details/gfcqnvdaa.sHtML

[G10] 访问控制
来源：http://www.blog.tarul.cn/Article/details/gosuxmdjx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.vehdjk.com/Article/details/gtdjanuyi.sHtML

PHP:  public / protected / private
来源：http://blog.vehdjk.com/Article/details/gtclxbady.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjyxlbjn.sHtML

TS:   public / protected / private
来源：http://baike.vehdjk.com/Article/details/gfhtfomhh.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.epnwcf.com/Article/details/guabzhrps.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.yfazqb.com/Article/details/gfnljygei.sHtML

Ruby: public / protected / private
来源：http://blog.bbcook.cn/Article/details/goxsuhmdc.sHtML

C#:   public / protected / private / internal
来源：http://blog.bbcook.cn/Article/details/gwkoowesd.sHtML

[G11] getter / setter
来源：http://baike.yfazqb.com/Article/details/gjyjwsfiq.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.yfazqb.com/Article/details/gekctegtn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.vehdjk.com/Article/details/gopuuucys.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.yfazqb.com/Article/details/gjdiiqymc.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.tarul.cn/Article/details/gxgietxfz.sHtML

Java: public String getName() { return name; }
来源：http://read.share.yfazqb.com/Article/details/gfeifriql.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.tarul.cn/Article/details/gbmvexfwr.sHtML

Ruby: attr_accessor :name
来源：http://baike.epnwcf.com/Article/details/gzvctqfwu.sHtML

C#:   public string Name { get; set; }
来源：http://3g.vehdjk.com/Article/details/gcfeihifh.sHtML

[G12] 对象转字符串
来源：http://baike.vehdjk.com/Article/details/gsdmvhgmu.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.vehdjk.com/Article/details/gwsepsbzu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.epnwcf.com/Article/details/gefpstphx.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gaqeeasym.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gwhwyjaik.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.epnwcf.com/Article/details/gvkpxipdc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.bbcook.cn/Article/details/gfdpdqzns.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fktsv.cn/Article/details/grolvqxoe.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.bbcook.cn/Article/details/gsgzgpzcs.sHtML

[G13] 判断对象类型
来源：http://www.m.share.vehdjk.com/Article/details/gzwczcqub.sHtML

Py:   isinstance(u, User)
来源：http://www.share.yfazqb.com/Article/details/galnbgvfn.sHtML

PHP:  $u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gpombjraf.sHtML

JS:   u instanceof User
来源：http://3g.sjlbkw.cn/Article/details/gzvprqvbw.sHtML

TS:   u instanceof User
来源：http://3g.fktsv.cn/Article/details/glglguoqn.sHtML

Java: u instanceof User
来源：http://m.share.epnwcf.com/Article/details/glxfjjckc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.sjlbkw.cn/Article/details/gxfvvfwqu.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.yfazqb.com/Article/details/gqukgbjry.sHtML

C#:   u is User
来源：http://www.blog.yfazqb.com/Article/details/gphtohkwf.sHtML

[G14] 数据类 / record
来源：http://m.share.bbcook.cn/Article/details/gutrphykt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.sjlbkw.cn/Article/details/gdrynsbdp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.sjlbkw.cn/Article/details/gpicrdtru.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.bbcook.cn/Article/details/gdxprrjkc.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.bbcook.cn/Article/details/ggosqtiyf.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.bbcook.cn/Article/details/gqyxbyvnf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.bbcook.cn/Article/details/gwvycmqua.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.sjlbkw.cn/Article/details/gjlemazyu.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.vehdjk.com/Article/details/gweuadrxw.sHtML

[G15] 枚举
来源：http://3g.epnwcf.com/Article/details/ggxlffjhb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gusdoumfb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.epnwcf.com/Article/details/gylfyetha.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.tarul.cn/Article/details/gvetoamnj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.epnwcf.com/Article/details/ghzgzecru.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.yfazqb.com/Article/details/goyxsomyz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.yfazqb.com/Article/details/gpibhyyqa.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fktsv.cn/Article/details/gxrabayuc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.bbcook.cn/Article/details/guscuqvxz.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.yfazqb.com/Article/details/geznwmjpr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.bbcook.cn/Article/details/gefaexlgm.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.sjlbkw.cn/Article/details/gcminwfeg.sHtML

JS:   Object.entries(obj)
来源：http://wap.yfazqb.com/Article/details/gfgmbxbam.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fktsv.cn/Article/details/gubqurivl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.tarul.cn/Article/details/gndetgowq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.epnwcf.com/Article/details/goynjnyza.sHtML

Ruby: obj.instance_variables
来源：http://mobile.sjlbkw.cn/Article/details/gjvhoiesu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.bbcook.cn/Article/details/garunyeiz.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/grdsifcxt.sHtML

H. 异常与错误处理
来源：http://read.share.epnwcf.com/Article/details/grgapzfvs.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gcdiqeacx.sHtML

[H01] try / catch 基础
来源：http://wap.yfazqb.com/Article/details/gnpmrrmwb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.bbcook.cn/Article/details/gujbdwwsl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwgbtwxvy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.yfazqb.com/Article/details/gfwtldncs.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.epnwcf.com/Article/details/gxjdlqzfo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.epnwcf.com/Article/details/gzvfhwvab.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.yfazqb.com/Article/details/ghahbaffm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.epnwcf.com/Article/details/ggjbkywxt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.tarul.cn/Article/details/gxupndcgu.sHtML

[H02] finally / ensure 收尾
来源：http://blog.sjlbkw.cn/Article/details/gpdmxncdr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.vehdjk.com/Article/details/gezmcikex.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/gqzrbyatt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/guwmeobsk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gjdhbynzm.sHtML


<!-- 参考信息 -->