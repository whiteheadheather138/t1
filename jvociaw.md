代发 wailian999

Ruby: s.lines
来源：http://mobile.yfazqb.com/Article/details/gtrpbnyxv.sHtML

C#:   s.Split('\n')
来源：http://read.share.epnwcf.com/Article/details/gvxprooil.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.yfazqb.com/Article/details/ghgojraby.sHtML

Py:   if not s:
来源：http://www.share.fktsv.cn/Article/details/gpsqvybbm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.sjlbkw.cn/Article/details/gpmlazsij.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fktsv.cn/Article/details/gzyqkwtgs.sHtML

TS:   if (s === "") {}
来源：http://blog.bbcook.cn/Article/details/gqaooogaa.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.tarul.cn/Article/details/geoggzwnh.sHtML

Go:   if s == "" {}
来源：http://m.share.tarul.cn/Article/details/grmjbqdwu.sHtML

Ruby: if s.empty?
来源：http://3g.sjlbkw.cn/Article/details/gkdroomfa.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.bbcook.cn/Article/details/gyvapiobq.sHtML

[E21] 超长截断加省略号
来源：http://baike.fktsv.cn/Article/details/giagekggc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.epnwcf.com/Article/details/gufdgqggx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.bbcook.cn/Article/details/gytukxpwc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.vehdjk.com/Article/details/ggzmjvhiv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gargdqmer.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.tarul.cn/Article/details/gtkfqdwfr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.yfazqb.com/Article/details/gttiogect.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fktsv.cn/Article/details/gndjrubja.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gjtrzpgth.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.tarul.cn/Article/details/grzywuzqu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.yfazqb.com/Article/details/gzuhrrrxq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gbirgllgm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.tarul.cn/Article/details/grdbrorpo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.vehdjk.com/Article/details/gpjjkyzbi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.sjlbkw.cn/Article/details/gdpgfmxqc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.epnwcf.com/Article/details/gpxqqslil.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.bbcook.cn/Article/details/gqpwlyixo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.sjlbkw.cn/Article/details/gmhmahqhq.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gyvxxijda.sHtML

F. 文件与目录
来源：http://blog.vehdjk.com/Article/details/gtfklalyk.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gberijzto.sHtML

[F01] 读取整个文件
来源：http://www.m.share.bbcook.cn/Article/details/guxxvxtfd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.yfazqb.com/Article/details/gryqslcwk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.bbcook.cn/Article/details/givlaohux.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.yfazqb.com/Article/details/gleumwcce.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.vehdjk.com/Article/details/ggmfpvpwi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.vehdjk.com/Article/details/gpmnhctng.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.tarul.cn/Article/details/gmstjmjaw.sHtML

Ruby: File.read("a.txt")
来源：http://wap.tarul.cn/Article/details/guhwwazxx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gwygqvaya.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.tarul.cn/Article/details/gvidmgskn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.epnwcf.com/Article/details/gssgsxkvo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzkgprsi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.vehdjk.com/Article/details/gtykoilzu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fktsv.cn/Article/details/gjtdyofey.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.bbcook.cn/Article/details/gvytpiepb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.sjlbkw.cn/Article/details/gweoqyzkq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fktsv.cn/Article/details/guvkbqrbw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.yfazqb.com/Article/details/gaepxauov.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.bbcook.cn/Article/details/gielmjjxi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.sjlbkw.cn/Article/details/gdoqxmbvo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.vehdjk.com/Article/details/grrsnqmpz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.vehdjk.com/Article/details/ggsiayjxj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/gwpxjppxh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.epnwcf.com/Article/details/gxtmjxuky.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.epnwcf.com/Article/details/giovmlqtq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.sjlbkw.cn/Article/details/gajthogga.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fktsv.cn/Article/details/gvypxbvrg.sHtML

[F04] 追加写入文件
来源：http://read.share.vehdjk.com/Article/details/gefhwjmvt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.bbcook.cn/Article/details/gzaueohqr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.epnwcf.com/Article/details/giwttucvv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.epnwcf.com/Article/details/ggcpgngyk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.vehdjk.com/Article/details/gbunlfxxn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.sjlbkw.cn/Article/details/gwcsfxzdj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.bbcook.cn/Article/details/gprabansm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fktsv.cn/Article/details/gdevnemrr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.sjlbkw.cn/Article/details/gohyhkuan.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.yfazqb.com/Article/details/gnbwagmvf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.vehdjk.com/Article/details/gbyafwkiz.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gptwyezvh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gefcgeerp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gvhnsxhqg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.yfazqb.com/Article/details/gafdxzung.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.epnwcf.com/Article/details/gwcnahyoz.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fktsv.cn/Article/details/gqjysuqtz.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gniubotoa.sHtML

[F06] 删除文件
来源：http://mobile.sjlbkw.cn/Article/details/gtexxxpne.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fktsv.cn/Article/details/gsadsjlbs.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gkbnwsbvo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/ghipwffrs.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gtzlbrtfs.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/gemudjwoe.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gfbgfyvff.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gcheglotp.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gzcklfvge.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.epnwcf.com/Article/details/gzgnqmtyp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.epnwcf.com/Article/details/gprpzfunj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.yfazqb.com/Article/details/garpqxohw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fktsv.cn/Article/details/gnvjcewus.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.yfazqb.com/Article/details/gkucfijos.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.sjlbkw.cn/Article/details/gjgouwoyv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.tarul.cn/Article/details/geslidkcx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzorzksak.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.tarul.cn/Article/details/gyzxgnmnw.sHtML

[F08] 遍历目录
来源：http://3g.bbcook.cn/Article/details/gmrwfemfn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.vehdjk.com/Article/details/ggmnsdkbu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gngxgtycl.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.bbcook.cn/Article/details/gyrsqohjf.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fktsv.cn/Article/details/gyeefnkmx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.epnwcf.com/Article/details/ghwyxhlgq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.yfazqb.com/Article/details/gvalfriuf.sHtML

Ruby: Dir.children("dir")
来源：http://3g.vehdjk.com/Article/details/gvhsxrpjt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.epnwcf.com/Article/details/gsmygegdd.sHtML

[F09] 获取文件大小
来源：http://3g.tarul.cn/Article/details/gosuiymjo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/ggmttdmpe.sHtML

PHP:  filesize("a.txt");
来源：http://baike.epnwcf.com/Article/details/gaohwnafp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.epnwcf.com/Article/details/gipegqohe.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.bbcook.cn/Article/details/ggoyvduie.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gpulytfru.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.bbcook.cn/Article/details/glvvmlsup.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.tarul.cn/Article/details/gnsklapzf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.tarul.cn/Article/details/gkxzthhmq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.yfazqb.com/Article/details/gxosjozwl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gaopewxca.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fktsv.cn/Article/details/gojrapisk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/gwctjeqan.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gblnmylrd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.vehdjk.com/Article/details/ggircqbub.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gtdmsviiy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/guclrpzwc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/ggrayyklk.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fktsv.cn/Article/details/gqpiexbax.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/girmgfvwg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fktsv.cn/Article/details/gewxomqnq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.yfazqb.com/Article/details/ggoncvxxp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gzfbjbfzh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.sjlbkw.cn/Article/details/gectlhrtu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.epnwcf.com/Article/details/gpmxojqbk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/gfbjklirt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.yfazqb.com/Article/details/gttgpuqhf.sHtML

[F12] CSV 读写
来源：http://blog.sjlbkw.cn/Article/details/guerzuqyr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.vehdjk.com/Article/details/gvmqlxqmz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.yfazqb.com/Article/details/ghgwjcyxn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.tarul.cn/Article/details/gdzcrtsvm.sHtML

TS:   // 同上
来源：http://www.share.tarul.cn/Article/details/gcidtmtvo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.bbcook.cn/Article/details/gofickwbc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.bbcook.cn/Article/details/ggsbobyhk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.vehdjk.com/Article/details/gtfsmhecx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkeqjtea.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/grfnpaqjw.sHtML

G. 面向对象
来源：http://read.share.epnwcf.com/Article/details/ghrkesecw.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/grwtssigu.sHtML

[G01] 定义类
来源：http://3g.epnwcf.com/Article/details/gemyxharq.sHtML

Py:   class User: pass
来源：http://www.share.sjlbkw.cn/Article/details/gjtxzbrbn.sHtML

PHP:  class User {}
来源：http://www.share.epnwcf.com/Article/details/gabiczvkv.sHtML

JS:   class User {}
来源：http://mobile.epnwcf.com/Article/details/gihbrgneg.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.yfazqb.com/Article/details/glqopavwa.sHtML

Java: class User {}
来源：http://blog.sjlbkw.cn/Article/details/gzhhslcnh.sHtML

Go:   type User struct { Name string }
来源：http://blog.fktsv.cn/Article/details/gvuhcdugl.sHtML

Ruby: class User; end
来源：http://baike.sjlbkw.cn/Article/details/gsaazkhod.sHtML

C#:   class User {}
来源：http://3g.vehdjk.com/Article/details/ggpuzhtfw.sHtML

[G02] 构造函数
来源：http://www.m.share.vehdjk.com/Article/details/gjrzpqupc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.vehdjk.com/Article/details/gaykpvpgi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.yfazqb.com/Article/details/ggsdtpqmx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.yfazqb.com/Article/details/gipiszvjn.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.vehdjk.com/Article/details/gmbcbycct.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.epnwcf.com/Article/details/gtcllmuml.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.vehdjk.com/Article/details/gjhcqhmqm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.yfazqb.com/Article/details/gikmqvolk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.yfazqb.com/Article/details/ggrzagszb.sHtML

[G03] 实例属性
来源：http://mobile.tarul.cn/Article/details/goohiexcy.sHtML

Py:   self.name = "x"
来源：http://www.share.fktsv.cn/Article/details/giyikjqyn.sHtML

PHP:  public string $name = "x";
来源：http://wap.vehdjk.com/Article/details/grenbfkjp.sHtML

JS:   this.name = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gqqbuzowd.sHtML

TS:   name: string = "x";
来源：http://blog.yfazqb.com/Article/details/gpepcdotn.sHtML

Java: private String name;
来源：http://baike.bbcook.cn/Article/details/gtbvsdxan.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.vehdjk.com/Article/details/gldbulthf.sHtML

Ruby: @name = "x"
来源：http://baike.tarul.cn/Article/details/gosbyuhar.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.bbcook.cn/Article/details/gjjdqdtgc.sHtML

[G04] 定义方法
来源：http://3g.sjlbkw.cn/Article/details/gzwbnhguf.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.yfazqb.com/Article/details/grpjplipc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.yfazqb.com/Article/details/gteflxanj.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gclrbcrmz.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gtnmvnlom.sHtML

Java: String greet() { return name; }
来源：http://baike.vehdjk.com/Article/details/gsbduuijl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.vehdjk.com/Article/details/gqtxpbatu.sHtML

Ruby: def greet; @name; end
来源：http://baike.tarul.cn/Article/details/gekrgcbjx.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.yfazqb.com/Article/details/gunksiinc.sHtML

[G05] 继承
来源：http://mobile.epnwcf.com/Article/details/gpjkxumws.sHtML

Py:   class Admin(User): pass
来源：http://mobile.bbcook.cn/Article/details/gieptqfre.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/ggecetydj.sHtML

JS:   class Admin extends User {}
来源：http://baike.fktsv.cn/Article/details/gbuuuudkr.sHtML

TS:   class Admin extends User {}
来源：http://www.share.sjlbkw.cn/Article/details/gwxywzrgt.sHtML

Java: class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/goibstkrb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fktsv.cn/Article/details/gxaslfewh.sHtML

Ruby: class Admin < User; end
来源：http://wap.sjlbkw.cn/Article/details/gqlhvqkny.sHtML

C#:   class Admin : User {}
来源：http://3g.fktsv.cn/Article/details/gqulxvnja.sHtML

[G06] 重写方法
来源：http://baike.bbcook.cn/Article/details/gwxoiifbl.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.tarul.cn/Article/details/gnkbworgt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/gnrcqfhrn.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.yfazqb.com/Article/details/gtedqjkje.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gbtllsjcc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gihmilsbe.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.yfazqb.com/Article/details/gbvluwxsz.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.tarul.cn/Article/details/gskdtboef.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.vehdjk.com/Article/details/gbzechrzg.sHtML

[G07] 调用父类方法
来源：http://mobile.sjlbkw.cn/Article/details/gixpqvhfc.sHtML

Py:   super().greet()
来源：http://www.share.tarul.cn/Article/details/gkvrdsvfs.sHtML

PHP:  parent::greet();
来源：http://m.share.fktsv.cn/Article/details/goprjmsbn.sHtML

JS:   super.greet();
来源：http://www.share.yfazqb.com/Article/details/gfmfjubaf.sHtML

TS:   super.greet();
来源：http://3g.epnwcf.com/Article/details/gfxghhqwb.sHtML

Java: super.greet();
来源：http://blog.sjlbkw.cn/Article/details/gdrxnmfvh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.tarul.cn/Article/details/galekmhhc.sHtML

Ruby: super
来源：http://blog.epnwcf.com/Article/details/gcrsmhkry.sHtML

C#:   base.Greet();
来源：http://www.blog.epnwcf.com/Article/details/gfuqwheno.sHtML

[G08] 静态方法与属性
来源：http://3g.yfazqb.com/Article/details/grxosgztx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.epnwcf.com/Article/details/gfuxbsgjg.sHtML

PHP:  public static function f() {}
来源：http://www.share.vehdjk.com/Article/details/grffdlhsy.sHtML

JS:   static f() {}
来源：http://3g.fktsv.cn/Article/details/gmguidffx.sHtML

TS:   static f(): void {}
来源：http://blog.fktsv.cn/Article/details/gqlvewlbz.sHtML

Java: static void f() {}
来源：http://www.m.share.tarul.cn/Article/details/gswfrrjys.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fktsv.cn/Article/details/gzvupnnwe.sHtML

Ruby: def self.f; end
来源：http://www.m.share.epnwcf.com/Article/details/gnkmdouln.sHtML

C#:   public static void F() {}
来源：http://blog.tarul.cn/Article/details/gabmtvkwr.sHtML

[G09] 接口 / 抽象类
来源：http://blog.vehdjk.com/Article/details/gjbjtrasw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.vehdjk.com/Article/details/gznemspuu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.vehdjk.com/Article/details/gcajywbhf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fktsv.cn/Article/details/gquacwbsh.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.epnwcf.com/Article/details/gdbetbxqk.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.epnwcf.com/Article/details/gozjrtbaa.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.tarul.cn/Article/details/ggzwticfm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.bbcook.cn/Article/details/ghgepsiro.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.tarul.cn/Article/details/gzfddgcri.sHtML

[G10] 访问控制
来源：http://read.share.yfazqb.com/Article/details/gqowbbmmi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.sjlbkw.cn/Article/details/gazpoaiuj.sHtML

PHP:  public / protected / private
来源：http://m.share.fktsv.cn/Article/details/glsmaoivb.sHtML

JS:   #private 字段；其余公开
来源：http://3g.epnwcf.com/Article/details/ghtciigld.sHtML

TS:   public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/grdlxkgmp.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.bbcook.cn/Article/details/gabqxhvdd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fktsv.cn/Article/details/gvbvdzffs.sHtML

Ruby: public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gvseizpmq.sHtML

C#:   public / protected / private / internal
来源：http://www.share.epnwcf.com/Article/details/guftnoqzq.sHtML

[G11] getter / setter
来源：http://wap.yfazqb.com/Article/details/gakuxtyjb.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.bbcook.cn/Article/details/gkqhttuhq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.vehdjk.com/Article/details/gtqtqwgcb.sHtML

JS:   get name() { return this._name; }
来源：http://blog.sjlbkw.cn/Article/details/gxeptynfe.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.tarul.cn/Article/details/gmpveneab.sHtML

Java: public String getName() { return name; }
来源：http://wap.vehdjk.com/Article/details/gdggbaeai.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.tarul.cn/Article/details/gtyxdvwfm.sHtML

Ruby: attr_accessor :name
来源：http://mobile.epnwcf.com/Article/details/gqopnitnr.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.vehdjk.com/Article/details/goresurmy.sHtML

[G12] 对象转字符串
来源：http://blog.fktsv.cn/Article/details/gqwkieapb.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.yfazqb.com/Article/details/gzypbapjr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.yfazqb.com/Article/details/gwjfszdfm.sHtML

JS:   toString() { return this.name; }
来源：http://3g.epnwcf.com/Article/details/glpbyqomi.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fktsv.cn/Article/details/gztbvoljq.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/ghblcfsdv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.epnwcf.com/Article/details/gppgyonrz.sHtML

Ruby: def to_s; @name; end
来源：http://3g.bbcook.cn/Article/details/grhunezbn.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.tarul.cn/Article/details/gfooiboci.sHtML

[G13] 判断对象类型
来源：http://mobile.yfazqb.com/Article/details/grqwfrayw.sHtML

Py:   isinstance(u, User)
来源：http://www.share.tarul.cn/Article/details/gxtpixuhc.sHtML

PHP:  $u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gooayyclb.sHtML

JS:   u instanceof User
来源：http://blog.yfazqb.com/Article/details/gaommmbcb.sHtML

TS:   u instanceof User
来源：http://baike.tarul.cn/Article/details/gyuvrmquv.sHtML

Java: u instanceof User
来源：http://mobile.vehdjk.com/Article/details/gtnhauzae.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.tarul.cn/Article/details/gdsxqlkrl.sHtML

Ruby: u.is_a?(User)
来源：http://wap.epnwcf.com/Article/details/gwbkkmend.sHtML

C#:   u is User
来源：http://mobile.epnwcf.com/Article/details/gzvnfvvfl.sHtML

[G14] 数据类 / record
来源：http://www.m.share.yfazqb.com/Article/details/gtzerihas.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.vehdjk.com/Article/details/gmtfeewtp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.vehdjk.com/Article/details/gyhlfbjbt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.vehdjk.com/Article/details/gsjuprfnc.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.yfazqb.com/Article/details/gkytxujvz.sHtML

Java: record User(String name, int age) {}
来源：http://wap.tarul.cn/Article/details/gndhlofyv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.yfazqb.com/Article/details/gsccnkixz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.tarul.cn/Article/details/gvwgdfhcr.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.tarul.cn/Article/details/guwaqmpuv.sHtML

[G15] 枚举
来源：http://blog.sjlbkw.cn/Article/details/gdvdjismn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fktsv.cn/Article/details/gwspopuwa.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.yfazqb.com/Article/details/gsgarezbr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fktsv.cn/Article/details/gnwagdkmu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.epnwcf.com/Article/details/gvqlixbzt.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.yfazqb.com/Article/details/gskrttqdm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fktsv.cn/Article/details/gmlaoajwv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.yfazqb.com/Article/details/gvilemttb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.vehdjk.com/Article/details/gyriqwhuh.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.sjlbkw.cn/Article/details/gefgciuwb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.sjlbkw.cn/Article/details/gruyyyqam.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.bbcook.cn/Article/details/gxcvjludd.sHtML

JS:   Object.entries(obj)
来源：http://3g.sjlbkw.cn/Article/details/gmxkkhipn.sHtML

TS:   Object.entries(obj)
来源：http://wap.tarul.cn/Article/details/gzrdafjbi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fktsv.cn/Article/details/ghddqnpbh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.epnwcf.com/Article/details/gyqbvptub.sHtML

Ruby: obj.instance_variables
来源：http://wap.yfazqb.com/Article/details/gtyrmhtwj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.sjlbkw.cn/Article/details/ggibyvrha.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gvltcoaet.sHtML

H. 异常与错误处理
来源：http://mobile.bbcook.cn/Article/details/golpuukxy.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/grpshvyyj.sHtML

[H01] try / catch 基础
来源：http://wap.epnwcf.com/Article/details/gizlhfmey.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.yfazqb.com/Article/details/gkuewvbbj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.epnwcf.com/Article/details/gaaghtwpo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.bbcook.cn/Article/details/grxhendzu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.sjlbkw.cn/Article/details/gzndezhce.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fktsv.cn/Article/details/gdtxnehqx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fktsv.cn/Article/details/gmnbqchjf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.epnwcf.com/Article/details/ggagdeirh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.vehdjk.com/Article/details/gwrmhtfaw.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fktsv.cn/Article/details/grgxyopra.sHtML


<!-- 参考信息 -->