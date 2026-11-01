代发 wailian999

Ruby: s.lines
来源：http://m.share.yfazqb.com/Article/details/garylbjqb.sHtML

C#:   s.Split('\n')
来源：http://3g.bbcook.cn/Article/details/gnodioapp.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.tarul.cn/Article/details/gghocfgpy.sHtML

Py:   if not s:
来源：http://www.m.share.sjlbkw.cn/Article/details/gcnxzzwrn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.sjlbkw.cn/Article/details/gvixexznb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.epnwcf.com/Article/details/ghwvlpyjb.sHtML

TS:   if (s === "") {}
来源：http://3g.epnwcf.com/Article/details/ggamsifwv.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.tarul.cn/Article/details/guxqnlchv.sHtML

Go:   if s == "" {}
来源：http://baike.tarul.cn/Article/details/gfnhuhjfp.sHtML

Ruby: if s.empty?
来源：http://www.blog.bbcook.cn/Article/details/gxaurchrn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fktsv.cn/Article/details/gxctcjwrr.sHtML

[E21] 超长截断加省略号
来源：http://m.share.sjlbkw.cn/Article/details/gsxgyjsxa.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.yfazqb.com/Article/details/gtwgwafvm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.yfazqb.com/Article/details/ggxqvzuao.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fktsv.cn/Article/details/gaenjmmck.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gmjirufes.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gdevnixhx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.tarul.cn/Article/details/gmptwpxah.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gnhphvvyk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/grekaklup.sHtML

[E22] 字节长度与字符长度
来源：http://baike.bbcook.cn/Article/details/gznyuxwfm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.sjlbkw.cn/Article/details/gptdzdibh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.epnwcf.com/Article/details/gozrkzwsk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.sjlbkw.cn/Article/details/gitsvdxsi.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.tarul.cn/Article/details/gglsckmsj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.yfazqb.com/Article/details/gmtiueoad.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.yfazqb.com/Article/details/gdnaudjxn.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.epnwcf.com/Article/details/gteavfgpm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.epnwcf.com/Article/details/gapaibkig.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/ghwgkmxkb.sHtML

F. 文件与目录
来源：http://baike.bbcook.cn/Article/details/gkdfuxzqp.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gvmefrrlj.sHtML

[F01] 读取整个文件
来源：http://3g.bbcook.cn/Article/details/gzoumcjyd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.bbcook.cn/Article/details/gbevbvdzp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.bbcook.cn/Article/details/gxddbwweu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.yfazqb.com/Article/details/grbknnmcz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.bbcook.cn/Article/details/gptraxdnb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fktsv.cn/Article/details/gdyclcjul.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.tarul.cn/Article/details/gddenhbkz.sHtML

Ruby: File.read("a.txt")
来源：http://wap.yfazqb.com/Article/details/gqajzuatu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.epnwcf.com/Article/details/gzifxgubf.sHtML

[F02] 逐行读取文件
来源：http://blog.fktsv.cn/Article/details/gqvxgdhfx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fktsv.cn/Article/details/gmwmhyztf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.sjlbkw.cn/Article/details/geevamrge.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.vehdjk.com/Article/details/gvkceyoym.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.sjlbkw.cn/Article/details/ghptartdd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.bbcook.cn/Article/details/gtxudrdej.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.sjlbkw.cn/Article/details/gnflcrwjg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fktsv.cn/Article/details/guorsvfpp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.yfazqb.com/Article/details/giambndsv.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.sjlbkw.cn/Article/details/gdmgumloe.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.vehdjk.com/Article/details/gqzkcgtvc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.bbcook.cn/Article/details/gxdhehpwk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.yfazqb.com/Article/details/gkqhnpguw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fktsv.cn/Article/details/gntzkjvmm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.vehdjk.com/Article/details/gufapoysi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.epnwcf.com/Article/details/gzrckjruv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.yfazqb.com/Article/details/gvhjopuaa.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.bbcook.cn/Article/details/gpzkkrblx.sHtML

[F04] 追加写入文件
来源：http://baike.fktsv.cn/Article/details/gjpdjkelv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.yfazqb.com/Article/details/gzcmtwabf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.bbcook.cn/Article/details/gpisnhsjg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpvrnuchp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.yfazqb.com/Article/details/glhztvddq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.epnwcf.com/Article/details/gbtnersou.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gpgspazym.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.tarul.cn/Article/details/gzdvwffoo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fktsv.cn/Article/details/gmkbziflc.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.epnwcf.com/Article/details/gtnuhvjhm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.sjlbkw.cn/Article/details/grtwqyiks.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gayeysfsa.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gifincdcr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/gkcydqhnj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gtiwjppey.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.yfazqb.com/Article/details/gryomkdte.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gdagabclw.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gisikjopg.sHtML

[F06] 删除文件
来源：http://wap.sjlbkw.cn/Article/details/gsrwzysdm.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fktsv.cn/Article/details/ghsesnntw.sHtML

PHP:  unlink("a.txt");
来源：http://blog.yfazqb.com/Article/details/gnwbwweez.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/gcowngmyh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gxllhlptd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gpaepvcqr.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/grfjpofpf.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gmmnebcku.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gsnhualdn.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fktsv.cn/Article/details/gatezszba.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.vehdjk.com/Article/details/gdbjbaxmb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.bbcook.cn/Article/details/giaxpgwfq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.vehdjk.com/Article/details/gkkioukxa.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fktsv.cn/Article/details/gblqsimty.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.vehdjk.com/Article/details/gnazqdgiz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.vehdjk.com/Article/details/giikpddui.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.tarul.cn/Article/details/gitbcyfiv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.tarul.cn/Article/details/gnslutevo.sHtML

[F08] 遍历目录
来源：http://mobile.yfazqb.com/Article/details/gzgerxhof.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.bbcook.cn/Article/details/grmtixjkm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.vehdjk.com/Article/details/ggpdklmmy.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.tarul.cn/Article/details/gfzffjswz.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fktsv.cn/Article/details/gpnlpydfj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.tarul.cn/Article/details/gogxhyorf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.epnwcf.com/Article/details/grjnaxrhp.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.sjlbkw.cn/Article/details/grcpbalfc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.epnwcf.com/Article/details/geepzybfb.sHtML

[F09] 获取文件大小
来源：http://www.blog.bbcook.cn/Article/details/ghfqkjsmf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.tarul.cn/Article/details/gknoxwpio.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/goptoqkoo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.vehdjk.com/Article/details/gjxmprdcv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.sjlbkw.cn/Article/details/gzsnzmwwp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.vehdjk.com/Article/details/gbwcqcyth.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.bbcook.cn/Article/details/gisraanyg.sHtML

Ruby: File.size("a.txt")
来源：http://wap.tarul.cn/Article/details/gensiaivo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.epnwcf.com/Article/details/gccxfgzwn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.tarul.cn/Article/details/gmzegnbmc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/gqnmbpmdt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/ghrnkamsa.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gicetsesv.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gsoqzjega.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.bbcook.cn/Article/details/ghkxyjzup.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gafklbtjt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gsxlmpqij.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gpboxzxsh.sHtML

[F11] 复制与移动文件
来源：http://www.blog.vehdjk.com/Article/details/gnpfbqhdn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gieutsqxm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.tarul.cn/Article/details/gizdmrytg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/ghhabnnfn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/gylxurysj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.tarul.cn/Article/details/gtrjreqwm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.bbcook.cn/Article/details/ggdeslkuf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/gvqpbikjf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fktsv.cn/Article/details/ghduqdpdu.sHtML

[F12] CSV 读写
来源：http://baike.bbcook.cn/Article/details/gcsinzqmz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.sjlbkw.cn/Article/details/gbkweysfr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.bbcook.cn/Article/details/glyzbamft.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.vehdjk.com/Article/details/gdfamzqtz.sHtML

TS:   // 同上
来源：http://mobile.yfazqb.com/Article/details/gwzizlfnh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.vehdjk.com/Article/details/gqfvrvcho.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.sjlbkw.cn/Article/details/gyjklkniy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.bbcook.cn/Article/details/gdtecuoza.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.vehdjk.com/Article/details/gyytcbvjs.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/golukaaga.sHtML

G. 面向对象
来源：http://m.share.bbcook.cn/Article/details/gcrqtnxwk.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gbegdpufi.sHtML

[G01] 定义类
来源：http://www.share.fktsv.cn/Article/details/gensgqefj.sHtML

Py:   class User: pass
来源：http://www.share.sjlbkw.cn/Article/details/gpgbkdliw.sHtML

PHP:  class User {}
来源：http://3g.bbcook.cn/Article/details/geistgaee.sHtML

JS:   class User {}
来源：http://www.blog.bbcook.cn/Article/details/ghcmunrox.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.sjlbkw.cn/Article/details/ghvykrjkj.sHtML

Java: class User {}
来源：http://mobile.vehdjk.com/Article/details/gqrayddxl.sHtML

Go:   type User struct { Name string }
来源：http://read.share.bbcook.cn/Article/details/gstnqvmca.sHtML

Ruby: class User; end
来源：http://mobile.vehdjk.com/Article/details/gcifwzzdk.sHtML

C#:   class User {}
来源：http://mobile.vehdjk.com/Article/details/gqehcwieg.sHtML

[G02] 构造函数
来源：http://blog.sjlbkw.cn/Article/details/gjoigkbdl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.yfazqb.com/Article/details/gkjronhum.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.sjlbkw.cn/Article/details/gbrqqoxnb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.bbcook.cn/Article/details/ggyqomlrz.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.bbcook.cn/Article/details/gvwsflgzw.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fktsv.cn/Article/details/godymoyao.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.epnwcf.com/Article/details/gcfzrlolg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.epnwcf.com/Article/details/gwnpxxnxp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.bbcook.cn/Article/details/gjyytabfk.sHtML

[G03] 实例属性
来源：http://m.share.epnwcf.com/Article/details/gnzbippzk.sHtML

Py:   self.name = "x"
来源：http://mobile.sjlbkw.cn/Article/details/gmynqvvco.sHtML

PHP:  public string $name = "x";
来源：http://mobile.bbcook.cn/Article/details/ghdmnduic.sHtML

JS:   this.name = "x";
来源：http://blog.fktsv.cn/Article/details/gqkndflcv.sHtML

TS:   name: string = "x";
来源：http://www.blog.vehdjk.com/Article/details/gjsqetlde.sHtML

Java: private String name;
来源：http://baike.epnwcf.com/Article/details/gmwyybbtc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.yfazqb.com/Article/details/gzkgzknaw.sHtML

Ruby: @name = "x"
来源：http://www.share.tarul.cn/Article/details/gpstpnlvu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.tarul.cn/Article/details/gewfntfwa.sHtML

[G04] 定义方法
来源：http://wap.fktsv.cn/Article/details/gyvenpbzd.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.tarul.cn/Article/details/gvwnpykdr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gjforhavy.sHtML

JS:   greet() { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gmkcemyds.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.bbcook.cn/Article/details/gytgumlnk.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/grwjwzxlr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.tarul.cn/Article/details/gbxndhawa.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fktsv.cn/Article/details/gmyezxpnm.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.yfazqb.com/Article/details/gzyjqmxcc.sHtML

[G05] 继承
来源：http://m.share.vehdjk.com/Article/details/ghtfunmim.sHtML

Py:   class Admin(User): pass
来源：http://blog.bbcook.cn/Article/details/gjmkunvwe.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/guaxlbrvk.sHtML

JS:   class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/gtqmkwpnr.sHtML

TS:   class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gtxfjuyis.sHtML

Java: class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/glvqcnuwb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.tarul.cn/Article/details/gteayocmz.sHtML

Ruby: class Admin < User; end
来源：http://blog.vehdjk.com/Article/details/gmtpmcoam.sHtML

C#:   class Admin : User {}
来源：http://blog.yfazqb.com/Article/details/gegqzfkjp.sHtML

[G06] 重写方法
来源：http://wap.yfazqb.com/Article/details/gddigrnnm.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.yfazqb.com/Article/details/gmxhjiddn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fktsv.cn/Article/details/gchysramv.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/gbptvhawx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gbpexbbbp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/gjziclovr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.tarul.cn/Article/details/gmidqkbkr.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.bbcook.cn/Article/details/gkitbwmqz.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.bbcook.cn/Article/details/gjugnxjwl.sHtML

[G07] 调用父类方法
来源：http://3g.vehdjk.com/Article/details/gxityrrii.sHtML

Py:   super().greet()
来源：http://read.share.epnwcf.com/Article/details/ggyinplht.sHtML

PHP:  parent::greet();
来源：http://blog.bbcook.cn/Article/details/gkbbqzbja.sHtML

JS:   super.greet();
来源：http://wap.bbcook.cn/Article/details/gyhrlwsjd.sHtML

TS:   super.greet();
来源：http://wap.bbcook.cn/Article/details/gtdmgormp.sHtML

Java: super.greet();
来源：http://www.blog.fktsv.cn/Article/details/gsboqemvp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.yfazqb.com/Article/details/gosyaxibg.sHtML

Ruby: super
来源：http://mobile.vehdjk.com/Article/details/gcnotefmj.sHtML

C#:   base.Greet();
来源：http://www.share.fktsv.cn/Article/details/gwogkkric.sHtML

[G08] 静态方法与属性
来源：http://blog.yfazqb.com/Article/details/gdzkgsxnr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.sjlbkw.cn/Article/details/gdzomjhwa.sHtML

PHP:  public static function f() {}
来源：http://blog.bbcook.cn/Article/details/gposyjzdc.sHtML

JS:   static f() {}
来源：http://baike.tarul.cn/Article/details/gjmnsceba.sHtML

TS:   static f(): void {}
来源：http://www.blog.vehdjk.com/Article/details/gbmjkheeq.sHtML

Java: static void f() {}
来源：http://www.blog.sjlbkw.cn/Article/details/gthqdxpoq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.yfazqb.com/Article/details/gfvzxqudr.sHtML

Ruby: def self.f; end
来源：http://mobile.fktsv.cn/Article/details/gempndjkc.sHtML

C#:   public static void F() {}
来源：http://3g.fktsv.cn/Article/details/gxkmghmrq.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.yfazqb.com/Article/details/gwgaxdooq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.sjlbkw.cn/Article/details/ghmocufxz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.yfazqb.com/Article/details/gctknvgqg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.yfazqb.com/Article/details/gswacmsbg.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.epnwcf.com/Article/details/guwqupilm.sHtML

Java: interface Shape { double area(); }
来源：http://wap.yfazqb.com/Article/details/gcvgovcxd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.epnwcf.com/Article/details/gppiardgd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fktsv.cn/Article/details/griwbprqf.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.tarul.cn/Article/details/godhpksml.sHtML

[G10] 访问控制
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjbzzhtg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fktsv.cn/Article/details/gofkmuhfg.sHtML

PHP:  public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/gldfkodlh.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.epnwcf.com/Article/details/gkaufztjf.sHtML

TS:   public / protected / private
来源：http://wap.tarul.cn/Article/details/gcmakpssg.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.sjlbkw.cn/Article/details/gpdfnquwc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.epnwcf.com/Article/details/grpzhbhfh.sHtML

Ruby: public / protected / private
来源：http://blog.epnwcf.com/Article/details/gxrjribqq.sHtML

C#:   public / protected / private / internal
来源：http://baike.sjlbkw.cn/Article/details/gbzjytyou.sHtML

[G11] getter / setter
来源：http://www.m.share.bbcook.cn/Article/details/ghxqmohog.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.sjlbkw.cn/Article/details/gcnhvoyxw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.sjlbkw.cn/Article/details/gqpdwozvn.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.sjlbkw.cn/Article/details/gfneydlka.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfaaaiqxu.sHtML

Java: public String getName() { return name; }
来源：http://wap.vehdjk.com/Article/details/gglxnczdn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.vehdjk.com/Article/details/gzgazaidx.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.sjlbkw.cn/Article/details/gdwnnajwt.sHtML

C#:   public string Name { get; set; }
来源：http://3g.yfazqb.com/Article/details/gzeaqotdz.sHtML

[G12] 对象转字符串
来源：http://3g.vehdjk.com/Article/details/gvkneqdcz.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.vehdjk.com/Article/details/gcejneozq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.sjlbkw.cn/Article/details/gmezcckmh.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gdyeukzxa.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.tarul.cn/Article/details/gmhlrkyst.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gbjyhcxef.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.vehdjk.com/Article/details/gxxgvtxyi.sHtML

Ruby: def to_s; @name; end
来源：http://baike.tarul.cn/Article/details/gyhcgajiy.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.vehdjk.com/Article/details/giqjroajq.sHtML

[G13] 判断对象类型
来源：http://baike.sjlbkw.cn/Article/details/gbizzxdfy.sHtML

Py:   isinstance(u, User)
来源：http://www.share.epnwcf.com/Article/details/gkrawmpjm.sHtML

PHP:  $u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/gwonqxzhc.sHtML

JS:   u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/giinndwvl.sHtML

TS:   u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/gynbuktdd.sHtML

Java: u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gsdqqymzb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.epnwcf.com/Article/details/gaqekchdy.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.bbcook.cn/Article/details/gpwnagpvs.sHtML

C#:   u is User
来源：http://read.share.sjlbkw.cn/Article/details/gshklpqfg.sHtML

[G14] 数据类 / record
来源：http://www.share.tarul.cn/Article/details/gogvgduhm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.vehdjk.com/Article/details/gkmqsiibv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.yfazqb.com/Article/details/gmokbytdo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.epnwcf.com/Article/details/gwaokwypq.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fktsv.cn/Article/details/gzcjpioso.sHtML

Java: record User(String name, int age) {}
来源：http://blog.bbcook.cn/Article/details/ggbwsvisx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fktsv.cn/Article/details/gwkxthctr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.bbcook.cn/Article/details/gcertfauf.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fktsv.cn/Article/details/gzmqufxvt.sHtML

[G15] 枚举
来源：http://read.share.fktsv.cn/Article/details/gnjpuvigf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.tarul.cn/Article/details/gnkqslays.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.epnwcf.com/Article/details/gmmmufkxx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.vehdjk.com/Article/details/gzzzxyqmk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.tarul.cn/Article/details/gskbbaiji.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.epnwcf.com/Article/details/gbwmtkejv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.epnwcf.com/Article/details/glbqlwfxl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.bbcook.cn/Article/details/gdxkxotuq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.yfazqb.com/Article/details/goajbunte.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.tarul.cn/Article/details/gerchlenw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.bbcook.cn/Article/details/gpyyjnooj.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fktsv.cn/Article/details/godlyqxaj.sHtML

JS:   Object.entries(obj)
来源：http://3g.vehdjk.com/Article/details/gkwusmzpa.sHtML

TS:   Object.entries(obj)
来源：http://m.share.vehdjk.com/Article/details/gfaihbcqp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.tarul.cn/Article/details/gspkfkiiz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.epnwcf.com/Article/details/ghfvzbwho.sHtML

Ruby: obj.instance_variables
来源：http://m.share.epnwcf.com/Article/details/gowavaulu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.sjlbkw.cn/Article/details/gabnmfety.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gxfvtgaep.sHtML

H. 异常与错误处理
来源：http://3g.tarul.cn/Article/details/gjbqeajth.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gwdfroymo.sHtML

[H01] try / catch 基础
来源：http://mobile.tarul.cn/Article/details/ggfqppnqg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.tarul.cn/Article/details/gxgohjnub.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.yfazqb.com/Article/details/gndrslfxt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fktsv.cn/Article/details/gkrmgqgkl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.vehdjk.com/Article/details/gliwalmqa.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.bbcook.cn/Article/details/gxjgpnxrw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fktsv.cn/Article/details/gwzfhbskn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fktsv.cn/Article/details/gtdcaliyo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.yfazqb.com/Article/details/geulbjqyb.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.vehdjk.com/Article/details/gpddnfqbp.sHtML


<!-- 参考信息 -->