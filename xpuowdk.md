代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.share.fktsv.cn/Article/details/gbxgbwigo.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fktsv.cn/Article/details/gbgboujxq.sHtML

Java: s.lines().toList()
来源：http://read.share.fktsv.cn/Article/details/gpeewueew.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.yfazqb.com/Article/details/grczbytgy.sHtML

Ruby: s.lines
来源：http://blog.tarul.cn/Article/details/gqpdgnhjm.sHtML

C#:   s.Split('\n')
来源：http://blog.vehdjk.com/Article/details/gvxtpfdsr.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.tarul.cn/Article/details/gbaddqyzu.sHtML

Py:   if not s:
来源：http://www.blog.epnwcf.com/Article/details/gfvtplife.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.vehdjk.com/Article/details/gdoggxafc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fktsv.cn/Article/details/gujocszlm.sHtML

TS:   if (s === "") {}
来源：http://baike.sjlbkw.cn/Article/details/giqlbblbg.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.yfazqb.com/Article/details/gzvkqewqi.sHtML

Go:   if s == "" {}
来源：http://www.blog.epnwcf.com/Article/details/gtynfuays.sHtML

Ruby: if s.empty?
来源：http://www.m.share.tarul.cn/Article/details/goslaznyg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.bbcook.cn/Article/details/gptacirqn.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.tarul.cn/Article/details/gdsiklsax.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.sjlbkw.cn/Article/details/gpgpkubyg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fktsv.cn/Article/details/gbxtdssex.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.vehdjk.com/Article/details/gfhnipypa.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fktsv.cn/Article/details/gylchcdym.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gxgrfvvkz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.yfazqb.com/Article/details/gupwfxzay.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.yfazqb.com/Article/details/gcvgeyrrz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gmdwwdgbb.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.epnwcf.com/Article/details/gqqfawptg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.sjlbkw.cn/Article/details/ggfsdkpzw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/gzatzukpq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.epnwcf.com/Article/details/gilbbbvey.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.tarul.cn/Article/details/gnaxwujtk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.tarul.cn/Article/details/gtwwnwuch.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.yfazqb.com/Article/details/gtvljyirk.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.vehdjk.com/Article/details/gufkeydpg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.sjlbkw.cn/Article/details/gizvzmlmt.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gvdelnotc.sHtML

F. 文件与目录
来源：http://3g.vehdjk.com/Article/details/gdeghsnry.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/ghrtavfcl.sHtML

[F01] 读取整个文件
来源：http://3g.sjlbkw.cn/Article/details/gpryczcsp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.tarul.cn/Article/details/gncidzqft.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gccbplotu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.bbcook.cn/Article/details/geucjjvys.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.epnwcf.com/Article/details/giwhtnkzh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/ghqyxrcqb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.vehdjk.com/Article/details/gwnvbxmtr.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gvpelsjlz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gapaleuog.sHtML

[F02] 逐行读取文件
来源：http://www.share.sjlbkw.cn/Article/details/gwqafnmtn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.yfazqb.com/Article/details/ggjhdmirz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.vehdjk.com/Article/details/gxfqjiqwu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.vehdjk.com/Article/details/gwzctslea.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.vehdjk.com/Article/details/giqisvpuf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fktsv.cn/Article/details/gwqkdkqxw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.sjlbkw.cn/Article/details/georfbcut.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.epnwcf.com/Article/details/ghhkewnal.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fktsv.cn/Article/details/gudktfejn.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.vehdjk.com/Article/details/gazfhwvrx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.tarul.cn/Article/details/giwaxwdnw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.vehdjk.com/Article/details/gcvwrrjkl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.tarul.cn/Article/details/gmpfdxpsz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.bbcook.cn/Article/details/gxijpouxq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.vehdjk.com/Article/details/gkxldwaey.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.vehdjk.com/Article/details/gnvtpvgzs.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fktsv.cn/Article/details/goppsbqbx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.yfazqb.com/Article/details/goivydkiz.sHtML

[F04] 追加写入文件
来源：http://3g.sjlbkw.cn/Article/details/gbunhjoxu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.epnwcf.com/Article/details/gaivxixuw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.sjlbkw.cn/Article/details/gptcknugt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.vehdjk.com/Article/details/gcnriswpu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.tarul.cn/Article/details/gjgbhqxrn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.sjlbkw.cn/Article/details/gspacloba.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.epnwcf.com/Article/details/gpuqomaue.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.sjlbkw.cn/Article/details/gglfvaluy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.bbcook.cn/Article/details/gculcrwmk.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fktsv.cn/Article/details/gmnyjrlnz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.bbcook.cn/Article/details/ggxslfbjx.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gnhckjjlm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/gsiaigrvk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/ghajflrpf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.yfazqb.com/Article/details/gdzulmoxq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.vehdjk.com/Article/details/gxqpylkbj.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.vehdjk.com/Article/details/gdihubmds.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.yfazqb.com/Article/details/gajiwzyep.sHtML

[F06] 删除文件
来源：http://mobile.tarul.cn/Article/details/glbhdnrjj.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gtjfevtih.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gdfyadjxg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gplasnbtk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gvzckisug.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/gknoaudjb.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gdqjrfyig.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.tarul.cn/Article/details/gozapioau.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.vehdjk.com/Article/details/gudaakpkw.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.epnwcf.com/Article/details/gycxokexn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.yfazqb.com/Article/details/ggnzgerdp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.tarul.cn/Article/details/glzkemtcf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.yfazqb.com/Article/details/getlwsiwe.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.yfazqb.com/Article/details/gseiwqlev.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fktsv.cn/Article/details/gbgwojwpc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.bbcook.cn/Article/details/gfnkssefw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fktsv.cn/Article/details/gizlvgiqb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fktsv.cn/Article/details/gevztzeyc.sHtML

[F08] 遍历目录
来源：http://3g.epnwcf.com/Article/details/gzcujctna.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.epnwcf.com/Article/details/guxdsniya.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fktsv.cn/Article/details/ghioxquea.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.bbcook.cn/Article/details/ghnjdzszy.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.bbcook.cn/Article/details/grparfkru.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.bbcook.cn/Article/details/gjbibemgt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.bbcook.cn/Article/details/gxuinsmln.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fktsv.cn/Article/details/gyustjuqf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.epnwcf.com/Article/details/gmbfghfre.sHtML

[F09] 获取文件大小
来源：http://wap.bbcook.cn/Article/details/gmamowope.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.bbcook.cn/Article/details/gmnllwdmv.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gqjaoavfg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.vehdjk.com/Article/details/gavpdjddb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.bbcook.cn/Article/details/gkijgcrib.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gvfwzyefi.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.bbcook.cn/Article/details/gkvefvqdw.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gkbqispln.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.vehdjk.com/Article/details/gpqdryrtr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.sjlbkw.cn/Article/details/gsvdpkxmx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/grxlgofkb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gyfmlcxff.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/grwfxrtqw.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gvaeiicyz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.bbcook.cn/Article/details/gabifvtgx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/gozncuubg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/grjbkllip.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/giqmcewxb.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.tarul.cn/Article/details/gvwtihqeo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/gxubsbmtl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.yfazqb.com/Article/details/giyxjitse.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/gjknmcfaz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/gdhpngynh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.bbcook.cn/Article/details/ggzkwsudg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.tarul.cn/Article/details/gzaznnkov.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.epnwcf.com/Article/details/gtowbeclg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.bbcook.cn/Article/details/gicuaalhf.sHtML

[F12] CSV 读写
来源：http://www.m.share.bbcook.cn/Article/details/gqgnlnbhh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.epnwcf.com/Article/details/gbqvhxppr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.vehdjk.com/Article/details/gvoxsnrcz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.tarul.cn/Article/details/gsxlpvjrr.sHtML

TS:   // 同上
来源：http://read.share.tarul.cn/Article/details/gjrefjjdt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.tarul.cn/Article/details/gegmcwoyt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.yfazqb.com/Article/details/gvgkgzxsa.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.yfazqb.com/Article/details/gdrtxfscs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.epnwcf.com/Article/details/gickunmbh.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/ghgclrash.sHtML

G. 面向对象
来源：http://3g.sjlbkw.cn/Article/details/gsddtusba.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gcusydicq.sHtML

[G01] 定义类
来源：http://www.blog.yfazqb.com/Article/details/guetoabep.sHtML

Py:   class User: pass
来源：http://mobile.yfazqb.com/Article/details/gvericghu.sHtML

PHP:  class User {}
来源：http://wap.bbcook.cn/Article/details/gjsttdhky.sHtML

JS:   class User {}
来源：http://www.share.bbcook.cn/Article/details/gzexprkrq.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.epnwcf.com/Article/details/ghrpqvbis.sHtML

Java: class User {}
来源：http://m.share.sjlbkw.cn/Article/details/gqrfwjrxc.sHtML

Go:   type User struct { Name string }
来源：http://www.share.epnwcf.com/Article/details/gckydfayl.sHtML

Ruby: class User; end
来源：http://3g.bbcook.cn/Article/details/gwmjrdmkg.sHtML

C#:   class User {}
来源：http://blog.epnwcf.com/Article/details/gqglixrlm.sHtML

[G02] 构造函数
来源：http://www.share.epnwcf.com/Article/details/gifqvswpb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.yfazqb.com/Article/details/ghghwlkqn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.epnwcf.com/Article/details/gsyaproii.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.vehdjk.com/Article/details/glbadjfgb.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.bbcook.cn/Article/details/gfkglfqmn.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.yfazqb.com/Article/details/gwrohjxfy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.vehdjk.com/Article/details/gqticyevg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.yfazqb.com/Article/details/ghqvxcjqa.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.sjlbkw.cn/Article/details/ginvdtbiy.sHtML

[G03] 实例属性
来源：http://blog.vehdjk.com/Article/details/gdocmeuca.sHtML

Py:   self.name = "x"
来源：http://3g.vehdjk.com/Article/details/gjpbacxfy.sHtML

PHP:  public string $name = "x";
来源：http://3g.yfazqb.com/Article/details/gsgpzmcvu.sHtML

JS:   this.name = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gspgdixdi.sHtML

TS:   name: string = "x";
来源：http://3g.bbcook.cn/Article/details/gncnoaldd.sHtML

Java: private String name;
来源：http://3g.tarul.cn/Article/details/gqownsoss.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.yfazqb.com/Article/details/gnhrdandp.sHtML

Ruby: @name = "x"
来源：http://3g.vehdjk.com/Article/details/gqafdurik.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.bbcook.cn/Article/details/gkiykitny.sHtML

[G04] 定义方法
来源：http://www.blog.epnwcf.com/Article/details/gccwmpsii.sHtML

Py:   def greet(self): return self.name
来源：http://wap.sjlbkw.cn/Article/details/gnxintnpw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fktsv.cn/Article/details/gewdgfzxn.sHtML

JS:   greet() { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gjulrcgmh.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gwlzsipcp.sHtML

Java: String greet() { return name; }
来源：http://baike.epnwcf.com/Article/details/grakaqkar.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpglnajgo.sHtML

Ruby: def greet; @name; end
来源：http://3g.bbcook.cn/Article/details/gcjvuycop.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.bbcook.cn/Article/details/gzgfsykso.sHtML

[G05] 继承
来源：http://blog.vehdjk.com/Article/details/gohstpfqj.sHtML

Py:   class Admin(User): pass
来源：http://blog.fktsv.cn/Article/details/gsqgkbfmo.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/guriowelk.sHtML

JS:   class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/glmsdjbic.sHtML

TS:   class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/gafpqkfhq.sHtML

Java: class Admin extends User {}
来源：http://www.blog.vehdjk.com/Article/details/gzxddoqov.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.bbcook.cn/Article/details/gphzhxetn.sHtML

Ruby: class Admin < User; end
来源：http://3g.fktsv.cn/Article/details/gqcvuhszu.sHtML

C#:   class Admin : User {}
来源：http://www.blog.bbcook.cn/Article/details/gspfkqoge.sHtML

[G06] 重写方法
来源：http://wap.fktsv.cn/Article/details/gnxdsgrzm.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.sjlbkw.cn/Article/details/gvkhrogzu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gkjslorcz.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gyejgxmub.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/gupfesdpr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/gjgwwiirm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.bbcook.cn/Article/details/gvqxdbnfy.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.bbcook.cn/Article/details/gquublylc.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.epnwcf.com/Article/details/goobxjhoy.sHtML

[G07] 调用父类方法
来源：http://3g.yfazqb.com/Article/details/gvtqdmcoy.sHtML

Py:   super().greet()
来源：http://3g.vehdjk.com/Article/details/gwxjjwadc.sHtML

PHP:  parent::greet();
来源：http://mobile.fktsv.cn/Article/details/gsihbjegx.sHtML

JS:   super.greet();
来源：http://mobile.bbcook.cn/Article/details/gpbqlxkkj.sHtML

TS:   super.greet();
来源：http://www.blog.epnwcf.com/Article/details/gouxafrop.sHtML

Java: super.greet();
来源：http://www.blog.fktsv.cn/Article/details/gpmpkcgyc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.vehdjk.com/Article/details/gnhndrqjo.sHtML

Ruby: super
来源：http://mobile.epnwcf.com/Article/details/gpofzoofm.sHtML

C#:   base.Greet();
来源：http://3g.bbcook.cn/Article/details/gmolngiht.sHtML

[G08] 静态方法与属性
来源：http://baike.yfazqb.com/Article/details/gocjwgdma.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.sjlbkw.cn/Article/details/ggczxeqhn.sHtML

PHP:  public static function f() {}
来源：http://wap.epnwcf.com/Article/details/gcewzlycf.sHtML

JS:   static f() {}
来源：http://baike.vehdjk.com/Article/details/gwtakqxdp.sHtML

TS:   static f(): void {}
来源：http://mobile.sjlbkw.cn/Article/details/gtgbthmfd.sHtML

Java: static void f() {}
来源：http://3g.sjlbkw.cn/Article/details/gncrizxlv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.sjlbkw.cn/Article/details/gzhztmwof.sHtML

Ruby: def self.f; end
来源：http://3g.tarul.cn/Article/details/guranwzlp.sHtML

C#:   public static void F() {}
来源：http://3g.fktsv.cn/Article/details/gslfvlqdr.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fktsv.cn/Article/details/gynyfvfto.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.yfazqb.com/Article/details/gijxbnort.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.bbcook.cn/Article/details/gujesazad.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.vehdjk.com/Article/details/gnxbkhjfx.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.bbcook.cn/Article/details/gosmzukco.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.epnwcf.com/Article/details/glmupnrjf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.tarul.cn/Article/details/gpyuuustt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.yfazqb.com/Article/details/geglxnctf.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.bbcook.cn/Article/details/grvslumfn.sHtML

[G10] 访问控制
来源：http://www.m.share.bbcook.cn/Article/details/godqlbqsj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.vehdjk.com/Article/details/gemfecikv.sHtML

PHP:  public / protected / private
来源：http://www.share.yfazqb.com/Article/details/gsqffndqm.sHtML

JS:   #private 字段；其余公开
来源：http://baike.sjlbkw.cn/Article/details/gsxwwoynm.sHtML

TS:   public / protected / private
来源：http://baike.bbcook.cn/Article/details/ggxsbbism.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.sjlbkw.cn/Article/details/gnldxjimv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.bbcook.cn/Article/details/ghdybrlnp.sHtML

Ruby: public / protected / private
来源：http://www.share.yfazqb.com/Article/details/gtsjadsaj.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.tarul.cn/Article/details/gohfnhysc.sHtML

[G11] getter / setter
来源：http://3g.epnwcf.com/Article/details/gskausumz.sHtML

Py:   @property 与 @x.setter
来源：http://blog.sjlbkw.cn/Article/details/gkvsdalqc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fktsv.cn/Article/details/goeznzala.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.epnwcf.com/Article/details/gzixznzql.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.bbcook.cn/Article/details/guwagvilu.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.epnwcf.com/Article/details/gieepviql.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.tarul.cn/Article/details/gzfprmxio.sHtML

Ruby: attr_accessor :name
来源：http://mobile.sjlbkw.cn/Article/details/gantzqngq.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.epnwcf.com/Article/details/gacwcvyta.sHtML

[G12] 对象转字符串
来源：http://www.share.yfazqb.com/Article/details/gkrylwsbo.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.tarul.cn/Article/details/gznmialox.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/gimzohrsq.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/gpbojwhye.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/ggfrbvvqe.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gnjyviday.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.vehdjk.com/Article/details/gzzwzebyf.sHtML

Ruby: def to_s; @name; end
来源：http://wap.vehdjk.com/Article/details/grlsuabcq.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.vehdjk.com/Article/details/gwkureqpn.sHtML

[G13] 判断对象类型
来源：http://www.share.tarul.cn/Article/details/garubkmgf.sHtML

Py:   isinstance(u, User)
来源：http://read.share.yfazqb.com/Article/details/gwhkuvvvm.sHtML

PHP:  $u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/gmutdsups.sHtML

JS:   u instanceof User
来源：http://www.share.vehdjk.com/Article/details/geumpqfbv.sHtML

TS:   u instanceof User
来源：http://read.share.tarul.cn/Article/details/gljanbqhr.sHtML

Java: u instanceof User
来源：http://www.m.share.yfazqb.com/Article/details/gcsuswimu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.bbcook.cn/Article/details/gjukjdjor.sHtML

Ruby: u.is_a?(User)
来源：http://wap.sjlbkw.cn/Article/details/gxxteqdoo.sHtML

C#:   u is User
来源：http://www.m.share.yfazqb.com/Article/details/gzdudamzw.sHtML

[G14] 数据类 / record
来源：http://wap.tarul.cn/Article/details/gfeaqelpx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.sjlbkw.cn/Article/details/gavzafsxw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.sjlbkw.cn/Article/details/gmhynqsxq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.tarul.cn/Article/details/giknkkjrf.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.yfazqb.com/Article/details/gucxkmbsv.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.bbcook.cn/Article/details/gjxtnztox.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.yfazqb.com/Article/details/gddzksbvo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.yfazqb.com/Article/details/gemcfljgt.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.vehdjk.com/Article/details/goqsharan.sHtML

[G15] 枚举
来源：http://3g.epnwcf.com/Article/details/gqrfrrglc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.tarul.cn/Article/details/gqzgsmlny.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.yfazqb.com/Article/details/gzqctljqn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.vehdjk.com/Article/details/gflzafsmv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.yfazqb.com/Article/details/gqrhermsm.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fktsv.cn/Article/details/gdfwujgvl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.yfazqb.com/Article/details/gyizzcwbb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.yfazqb.com/Article/details/ggbkznmnn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.epnwcf.com/Article/details/gseoulrpq.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.yfazqb.com/Article/details/gpawuhgkw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.bbcook.cn/Article/details/gqcgappcp.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.vehdjk.com/Article/details/grawwwqty.sHtML

JS:   Object.entries(obj)
来源：http://3g.yfazqb.com/Article/details/gtdzkxlmh.sHtML

TS:   Object.entries(obj)
来源：http://wap.fktsv.cn/Article/details/gjsmwkght.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.vehdjk.com/Article/details/gzuvxvgrk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.epnwcf.com/Article/details/glhukywld.sHtML

Ruby: obj.instance_variables
来源：http://baike.yfazqb.com/Article/details/gwupjvegx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.yfazqb.com/Article/details/gttqvaqtk.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gfdqmjhkp.sHtML

H. 异常与错误处理
来源：http://3g.sjlbkw.cn/Article/details/gforddtjh.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/ghjjhieos.sHtML

[H01] try / catch 基础
来源：http://baike.vehdjk.com/Article/details/gkglusckb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.sjlbkw.cn/Article/details/gvqzvuvob.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fktsv.cn/Article/details/gvqghyaca.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fktsv.cn/Article/details/ghdqrqvyg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/gebuimtbv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.vehdjk.com/Article/details/gzkjpvlwx.sHtML


<!-- 参考信息 -->