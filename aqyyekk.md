代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://read.share.fktsv.cn/Article/details/ghfjpuihz.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.yfazqb.com/Article/details/gkbxbqgwu.sHtML

Java: s.lines().toList()
来源：http://www.share.sjlbkw.cn/Article/details/gztumxkcu.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.tarul.cn/Article/details/gsummfsys.sHtML

Ruby: s.lines
来源：http://www.share.vehdjk.com/Article/details/gflkkgzbz.sHtML

C#:   s.Split('\n')
来源：http://3g.epnwcf.com/Article/details/gjpifnsyz.sHtML

[E20] 判断字符串是否为空
来源：http://3g.tarul.cn/Article/details/gaijiccsv.sHtML

Py:   if not s:
来源：http://www.blog.vehdjk.com/Article/details/gtwusicfi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.sjlbkw.cn/Article/details/gkfxmvqko.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.vehdjk.com/Article/details/gjkestvmc.sHtML

TS:   if (s === "") {}
来源：http://www.share.bbcook.cn/Article/details/glwyyoaeh.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.epnwcf.com/Article/details/gzhfbsohj.sHtML

Go:   if s == "" {}
来源：http://blog.tarul.cn/Article/details/ghvlxmehv.sHtML

Ruby: if s.empty?
来源：http://www.share.tarul.cn/Article/details/gqqslgdto.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.sjlbkw.cn/Article/details/ghguwmqzl.sHtML

[E21] 超长截断加省略号
来源：http://3g.vehdjk.com/Article/details/gkknijhbe.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.bbcook.cn/Article/details/guofkskfd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gsuduulzn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.yfazqb.com/Article/details/gcldyxfwz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gtpqslyyf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.yfazqb.com/Article/details/gtxckxyyf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.epnwcf.com/Article/details/gfwwgxjwu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.yfazqb.com/Article/details/gsjwgnpfl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fktsv.cn/Article/details/glommzsez.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fktsv.cn/Article/details/gfwjvkkco.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.yfazqb.com/Article/details/gfnnvqpgl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.tarul.cn/Article/details/gqdzdvasz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fktsv.cn/Article/details/gypksaacm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.sjlbkw.cn/Article/details/gpdjzmnhm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.sjlbkw.cn/Article/details/goulpfgeu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fktsv.cn/Article/details/geklaxijs.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.tarul.cn/Article/details/gkhqgxgwj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.bbcook.cn/Article/details/glfmtlzsf.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gtfsgwdkk.sHtML

F. 文件与目录
来源：http://read.share.fktsv.cn/Article/details/golvpnpjt.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gnhyqqtuw.sHtML

[F01] 读取整个文件
来源：http://www.m.share.bbcook.cn/Article/details/gozrwkgla.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.vehdjk.com/Article/details/gejaasrzo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.tarul.cn/Article/details/gzqikbaqb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.yfazqb.com/Article/details/gseplbyck.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.epnwcf.com/Article/details/gadornqcw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gqxhmaqff.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.epnwcf.com/Article/details/gaajcnaie.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gdtaxcmmk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gusabdtkg.sHtML

[F02] 逐行读取文件
来源：http://wap.sjlbkw.cn/Article/details/gxydpmbbu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.sjlbkw.cn/Article/details/guqywkoeq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.bbcook.cn/Article/details/gxcxcnchu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.vehdjk.com/Article/details/gbycjllwt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.epnwcf.com/Article/details/gddiatjvj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.bbcook.cn/Article/details/gqryguooa.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.bbcook.cn/Article/details/gglfvuuhj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.bbcook.cn/Article/details/gbowzgpqt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.bbcook.cn/Article/details/gecyefbav.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.tarul.cn/Article/details/gbfdjorln.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.tarul.cn/Article/details/gptrwlkpy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.bbcook.cn/Article/details/ggaqtnzlz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.epnwcf.com/Article/details/guolkkxro.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.yfazqb.com/Article/details/gvekylpqb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.sjlbkw.cn/Article/details/geobufnwu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fktsv.cn/Article/details/gsgrxfchg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.vehdjk.com/Article/details/gbroofris.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.tarul.cn/Article/details/gcqespavp.sHtML

[F04] 追加写入文件
来源：http://m.share.fktsv.cn/Article/details/gvttfzbgd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fktsv.cn/Article/details/gjasbtfbb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.vehdjk.com/Article/details/gizdaslnp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.yfazqb.com/Article/details/gvbifndxh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.tarul.cn/Article/details/gzzouxaqf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.epnwcf.com/Article/details/gvyjmghca.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.vehdjk.com/Article/details/gsuokteoo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fktsv.cn/Article/details/gdvfhzows.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.yfazqb.com/Article/details/gpnfajgbu.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.yfazqb.com/Article/details/ggsexwmmo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.epnwcf.com/Article/details/gfylabbfq.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.bbcook.cn/Article/details/gezblnyfv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gcswjzsdj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/gpkbpiuce.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/gnjcryzqq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.tarul.cn/Article/details/gicxhkiey.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gpmnyzovc.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gwcrzqxbs.sHtML

[F06] 删除文件
来源：http://www.share.fktsv.cn/Article/details/ghmunqaxh.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gfzzxecqw.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.bbcook.cn/Article/details/ggblnheyp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gjexczdbh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gcwcqhfqc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gkaeyfhyu.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.tarul.cn/Article/details/gsbacmjct.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gwhraejxb.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gouvvmlup.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.epnwcf.com/Article/details/gnhstuzou.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.sjlbkw.cn/Article/details/gddezmbvi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.vehdjk.com/Article/details/gclwwdfko.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.epnwcf.com/Article/details/ggidehahb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.tarul.cn/Article/details/gutxrtrgt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.sjlbkw.cn/Article/details/gpwmwotro.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fktsv.cn/Article/details/gbiqcpuxb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.sjlbkw.cn/Article/details/gjjeokhbb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.bbcook.cn/Article/details/ghegetmip.sHtML

[F08] 遍历目录
来源：http://m.share.epnwcf.com/Article/details/gnddkfaqw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.epnwcf.com/Article/details/gfusymrfq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.tarul.cn/Article/details/gnhcuflut.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfyehifz.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.yfazqb.com/Article/details/gagazynbo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fktsv.cn/Article/details/gmxfljicy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.bbcook.cn/Article/details/gwryjwlwc.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fktsv.cn/Article/details/gsyvjozum.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.bbcook.cn/Article/details/gjiasresv.sHtML

[F09] 获取文件大小
来源：http://mobile.fktsv.cn/Article/details/gaadbouxz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gucttjcrq.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gpxcmwnjk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.yfazqb.com/Article/details/gmcfcbxom.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.sjlbkw.cn/Article/details/gcopilmrl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.bbcook.cn/Article/details/gxzmnedei.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.bbcook.cn/Article/details/gsotqgots.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gkqhygafu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.tarul.cn/Article/details/gjtefctyx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.vehdjk.com/Article/details/giozihdzz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/gobgykuka.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gnqmscwso.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gyqetgplt.sHtML

TS:   path.extname("a.txt")
来源：http://3g.yfazqb.com/Article/details/gjyiniqbg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.tarul.cn/Article/details/ggmowodbr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gmheoprtf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gcwesxwhu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/ghisffrsm.sHtML

[F11] 复制与移动文件
来源：http://wap.tarul.cn/Article/details/gvtdhafuy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/gjfncjbuy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fktsv.cn/Article/details/gawoztuyl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gcwsxwipb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/ganpision.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.tarul.cn/Article/details/gkzgorlao.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.vehdjk.com/Article/details/gvkssetoc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/gekibnbjn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.sjlbkw.cn/Article/details/grhsvubux.sHtML

[F12] CSV 读写
来源：http://wap.fktsv.cn/Article/details/gsdgumdlh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.sjlbkw.cn/Article/details/gcxhnaxll.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqxbjwfu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fktsv.cn/Article/details/giusvpvgl.sHtML

TS:   // 同上
来源：http://wap.vehdjk.com/Article/details/geygcitpv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.epnwcf.com/Article/details/ggqmcmkos.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.sjlbkw.cn/Article/details/gmfgdjlpt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.sjlbkw.cn/Article/details/gjkkwbdun.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.yfazqb.com/Article/details/gsqmjwxon.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gdfihcssl.sHtML

G. 面向对象
来源：http://wap.sjlbkw.cn/Article/details/gettgsmyx.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gcqtoftmt.sHtML

[G01] 定义类
来源：http://read.share.fktsv.cn/Article/details/gdddjqkqq.sHtML

Py:   class User: pass
来源：http://baike.fktsv.cn/Article/details/gauwojqss.sHtML

PHP:  class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gamsgzguh.sHtML

JS:   class User {}
来源：http://blog.fktsv.cn/Article/details/gugztihjb.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.sjlbkw.cn/Article/details/goctysqzi.sHtML

Java: class User {}
来源：http://baike.tarul.cn/Article/details/gvcbkiqpp.sHtML

Go:   type User struct { Name string }
来源：http://3g.vehdjk.com/Article/details/ggdxwkbyf.sHtML

Ruby: class User; end
来源：http://baike.epnwcf.com/Article/details/gheopdqnw.sHtML

C#:   class User {}
来源：http://www.m.share.yfazqb.com/Article/details/guirwpftd.sHtML

[G02] 构造函数
来源：http://3g.bbcook.cn/Article/details/gcujedzjj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.yfazqb.com/Article/details/gpnxjudgt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.epnwcf.com/Article/details/grmddknlw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.bbcook.cn/Article/details/gdjcpvgqy.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fktsv.cn/Article/details/gifljpamm.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fktsv.cn/Article/details/gmqlmoifr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.yfazqb.com/Article/details/gdnolgchb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.bbcook.cn/Article/details/gpwknavdl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.epnwcf.com/Article/details/gxmgrerjw.sHtML

[G03] 实例属性
来源：http://mobile.vehdjk.com/Article/details/gbrpzhjdt.sHtML

Py:   self.name = "x"
来源：http://read.share.bbcook.cn/Article/details/ggbdzxydx.sHtML

PHP:  public string $name = "x";
来源：http://baike.epnwcf.com/Article/details/gatssnjmx.sHtML

JS:   this.name = "x";
来源：http://3g.sjlbkw.cn/Article/details/gvuzwhekf.sHtML

TS:   name: string = "x";
来源：http://www.share.yfazqb.com/Article/details/gpdcatdjq.sHtML

Java: private String name;
来源：http://www.m.share.bbcook.cn/Article/details/gzevhykgc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.bbcook.cn/Article/details/gtvuzwqdp.sHtML

Ruby: @name = "x"
来源：http://wap.fktsv.cn/Article/details/gcajbhzln.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.sjlbkw.cn/Article/details/gzgjpawxw.sHtML

[G04] 定义方法
来源：http://3g.bbcook.cn/Article/details/gkejzmtuc.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.tarul.cn/Article/details/gxwiqtwfy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/gupobjrts.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.vehdjk.com/Article/details/gagqpkkmm.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvvydgrhm.sHtML

Java: String greet() { return name; }
来源：http://3g.fktsv.cn/Article/details/gynsmtltw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.epnwcf.com/Article/details/gsnmwkqqn.sHtML

Ruby: def greet; @name; end
来源：http://m.share.yfazqb.com/Article/details/gizgtxdut.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fktsv.cn/Article/details/ggyekklld.sHtML

[G05] 继承
来源：http://blog.epnwcf.com/Article/details/gbqmryqck.sHtML

Py:   class Admin(User): pass
来源：http://3g.epnwcf.com/Article/details/ghafakfjc.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/grwxlgqwn.sHtML

JS:   class Admin extends User {}
来源：http://mobile.sjlbkw.cn/Article/details/gbdvadara.sHtML

TS:   class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/gcryjvqrw.sHtML

Java: class Admin extends User {}
来源：http://www.blog.epnwcf.com/Article/details/gtbtubuye.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.vehdjk.com/Article/details/greyttumv.sHtML

Ruby: class Admin < User; end
来源：http://m.share.yfazqb.com/Article/details/gosgkdoep.sHtML

C#:   class Admin : User {}
来源：http://read.share.yfazqb.com/Article/details/gaxppujal.sHtML

[G06] 重写方法
来源：http://baike.tarul.cn/Article/details/ggzhnopcw.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fktsv.cn/Article/details/gwwehtuai.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gimhhqqee.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gtoydilcq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/gmowzkrni.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gwspdlxjo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.tarul.cn/Article/details/gihlgsgjr.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.epnwcf.com/Article/details/gyzifnrlh.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.tarul.cn/Article/details/gbjebzqqh.sHtML

[G07] 调用父类方法
来源：http://wap.vehdjk.com/Article/details/guwtraqag.sHtML

Py:   super().greet()
来源：http://blog.sjlbkw.cn/Article/details/guktqwgyu.sHtML

PHP:  parent::greet();
来源：http://read.share.sjlbkw.cn/Article/details/gogivolyl.sHtML

JS:   super.greet();
来源：http://read.share.vehdjk.com/Article/details/gpiieujpv.sHtML

TS:   super.greet();
来源：http://baike.sjlbkw.cn/Article/details/gluohkbbz.sHtML

Java: super.greet();
来源：http://www.m.share.bbcook.cn/Article/details/ggqxqltwu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.yfazqb.com/Article/details/gxmfbzrkf.sHtML

Ruby: super
来源：http://www.blog.epnwcf.com/Article/details/guqtcxvip.sHtML

C#:   base.Greet();
来源：http://www.share.vehdjk.com/Article/details/gizjugbsn.sHtML

[G08] 静态方法与属性
来源：http://m.share.yfazqb.com/Article/details/gsrdltxbv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.epnwcf.com/Article/details/gsrhjyvcz.sHtML

PHP:  public static function f() {}
来源：http://wap.bbcook.cn/Article/details/gwiuepuxy.sHtML

JS:   static f() {}
来源：http://www.m.share.bbcook.cn/Article/details/gnwwvchct.sHtML

TS:   static f(): void {}
来源：http://m.share.vehdjk.com/Article/details/gidfaggnc.sHtML

Java: static void f() {}
来源：http://3g.sjlbkw.cn/Article/details/gtsiqscej.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.vehdjk.com/Article/details/gqozeqvtk.sHtML

Ruby: def self.f; end
来源：http://www.share.sjlbkw.cn/Article/details/gwomxtbht.sHtML

C#:   public static void F() {}
来源：http://baike.bbcook.cn/Article/details/gcrkonbnc.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.vehdjk.com/Article/details/gdzagweok.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.vehdjk.com/Article/details/gjiihsnnk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.yfazqb.com/Article/details/gfokihchc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.tarul.cn/Article/details/gepjsmwry.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.tarul.cn/Article/details/gwqrppbcs.sHtML

Java: interface Shape { double area(); }
来源：http://baike.bbcook.cn/Article/details/grfnqqgie.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.epnwcf.com/Article/details/gugctnvwo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.epnwcf.com/Article/details/grvpttzfw.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.bbcook.cn/Article/details/gwenbhavh.sHtML

[G10] 访问控制
来源：http://m.share.sjlbkw.cn/Article/details/gxjsxcoxi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.epnwcf.com/Article/details/gmakpnaht.sHtML

PHP:  public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/gbiiksyzd.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fktsv.cn/Article/details/gtafrnchl.sHtML

TS:   public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gwtbtcqid.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.sjlbkw.cn/Article/details/glrcbsfez.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fktsv.cn/Article/details/gutomvfgx.sHtML

Ruby: public / protected / private
来源：http://www.share.fktsv.cn/Article/details/govwqtpsm.sHtML

C#:   public / protected / private / internal
来源：http://blog.sjlbkw.cn/Article/details/gcnlzetyy.sHtML

[G11] getter / setter
来源：http://read.share.yfazqb.com/Article/details/gamlwhdsl.sHtML

Py:   @property 与 @x.setter
来源：http://3g.sjlbkw.cn/Article/details/gayipfuek.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.bbcook.cn/Article/details/guclqupnx.sHtML

JS:   get name() { return this._name; }
来源：http://baike.vehdjk.com/Article/details/grosdjprf.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.yfazqb.com/Article/details/goowewuqm.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fktsv.cn/Article/details/gbrakyjjm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.bbcook.cn/Article/details/ggtgjmxzz.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.tarul.cn/Article/details/gdjmcsrdn.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.tarul.cn/Article/details/gbvbgvrrk.sHtML

[G12] 对象转字符串
来源：http://baike.sjlbkw.cn/Article/details/gyiusmcwv.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.yfazqb.com/Article/details/gtynfvwvy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.bbcook.cn/Article/details/gjkbbtvqv.sHtML

JS:   toString() { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gxcvwfdxk.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gidfsznls.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.yfazqb.com/Article/details/gnrfypcbj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/gbdmjacaj.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.epnwcf.com/Article/details/grgxkbqyf.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.sjlbkw.cn/Article/details/giqavqiul.sHtML

[G13] 判断对象类型
来源：http://mobile.tarul.cn/Article/details/gucxxjhub.sHtML

Py:   isinstance(u, User)
来源：http://baike.fktsv.cn/Article/details/gpmeylokp.sHtML

PHP:  $u instanceof User
来源：http://www.share.epnwcf.com/Article/details/gsdmyieum.sHtML

JS:   u instanceof User
来源：http://read.share.vehdjk.com/Article/details/gloniyipd.sHtML

TS:   u instanceof User
来源：http://3g.fktsv.cn/Article/details/gzamcfcwo.sHtML

Java: u instanceof User
来源：http://www.m.share.vehdjk.com/Article/details/googadlfc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.yfazqb.com/Article/details/gpalyrefs.sHtML

Ruby: u.is_a?(User)
来源：http://blog.sjlbkw.cn/Article/details/gmymvsxzy.sHtML

C#:   u is User
来源：http://read.share.tarul.cn/Article/details/ghbpbvbav.sHtML

[G14] 数据类 / record
来源：http://baike.vehdjk.com/Article/details/gvvrxniul.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.vehdjk.com/Article/details/giloikmba.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.bbcook.cn/Article/details/gbsbihrax.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.bbcook.cn/Article/details/gxzglazgs.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.epnwcf.com/Article/details/grouamtve.sHtML

Java: record User(String name, int age) {}
来源：http://blog.bbcook.cn/Article/details/gviqbaijn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.bbcook.cn/Article/details/gwdzwqscp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fktsv.cn/Article/details/gaadrbhmr.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fktsv.cn/Article/details/gjfjavmba.sHtML

[G15] 枚举
来源：http://m.share.tarul.cn/Article/details/gwzhwbzhv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.tarul.cn/Article/details/gshevfcfj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.bbcook.cn/Article/details/gvcpvxkqy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.sjlbkw.cn/Article/details/giggbmhkj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.sjlbkw.cn/Article/details/glkgxthmi.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.yfazqb.com/Article/details/gwfmzknbx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.yfazqb.com/Article/details/gqgljslcp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fktsv.cn/Article/details/gnpyzgbhs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gbokikacf.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.tarul.cn/Article/details/gfebfuvco.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.epnwcf.com/Article/details/gsnctslrv.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.tarul.cn/Article/details/gntmhyvpu.sHtML

JS:   Object.entries(obj)
来源：http://m.share.bbcook.cn/Article/details/gworbwmpn.sHtML

TS:   Object.entries(obj)
来源：http://mobile.yfazqb.com/Article/details/gidwwmxzg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.sjlbkw.cn/Article/details/gdmwckyjt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.bbcook.cn/Article/details/glrjbgizs.sHtML

Ruby: obj.instance_variables
来源：http://mobile.vehdjk.com/Article/details/gbsspwrwv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fktsv.cn/Article/details/gjrcbrnfe.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gfvipklhe.sHtML

H. 异常与错误处理
来源：http://www.blog.epnwcf.com/Article/details/guhhpmtft.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/glfcyegum.sHtML

[H01] try / catch 基础
来源：http://baike.yfazqb.com/Article/details/gvzgltdck.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.yfazqb.com/Article/details/grosrztdx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.vehdjk.com/Article/details/gstxjjhuv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fktsv.cn/Article/details/gwlroukau.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.epnwcf.com/Article/details/gtujgbxbi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.bbcook.cn/Article/details/gvuzsjsyj.sHtML


<!-- 参考信息 -->