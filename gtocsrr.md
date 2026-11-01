代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.sjlbkw.cn/Article/details/grsrwzosp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.tarul.cn/Article/details/gkgxtcbka.sHtML

TS:   if (s === "") {}
来源：http://3g.fktsv.cn/Article/details/ggxmlhixj.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.tarul.cn/Article/details/gsyuhbvln.sHtML

Go:   if s == "" {}
来源：http://wap.yfazqb.com/Article/details/gafwskkcj.sHtML

Ruby: if s.empty?
来源：http://m.share.sjlbkw.cn/Article/details/glfcicdrt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.sjlbkw.cn/Article/details/gafjrozrf.sHtML

[E21] 超长截断加省略号
来源：http://baike.sjlbkw.cn/Article/details/gtuddbccg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.yfazqb.com/Article/details/gjclwuiwk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/gizkwfftf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.epnwcf.com/Article/details/glkdrwkfb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.yfazqb.com/Article/details/gacdroujz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gxurunbxx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.sjlbkw.cn/Article/details/gtizxaqbl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.epnwcf.com/Article/details/ghmjlucre.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fktsv.cn/Article/details/gezxveito.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.bbcook.cn/Article/details/gtsrdbnau.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.yfazqb.com/Article/details/gsoahbglp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fktsv.cn/Article/details/ghzyfvzze.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.epnwcf.com/Article/details/gtsbvepuq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.epnwcf.com/Article/details/gsgcbhnvn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fktsv.cn/Article/details/gzivjiiax.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.bbcook.cn/Article/details/geewshkhq.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fktsv.cn/Article/details/gnnavgrct.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.sjlbkw.cn/Article/details/gkpazscgx.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gdqwpwscb.sHtML

F. 文件与目录
来源：http://mobile.sjlbkw.cn/Article/details/gzypsfxwb.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gqmtfodbu.sHtML

[F01] 读取整个文件
来源：http://blog.epnwcf.com/Article/details/gdfuvnsne.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.vehdjk.com/Article/details/gjozytdmv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.epnwcf.com/Article/details/gbjgsnhfy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.bbcook.cn/Article/details/ghxwmshbd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fktsv.cn/Article/details/gssierpqt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.yfazqb.com/Article/details/ggegjovdz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fktsv.cn/Article/details/gylnwpgxb.sHtML

Ruby: File.read("a.txt")
来源：http://3g.bbcook.cn/Article/details/gypdpopsr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gmvwttlgs.sHtML

[F02] 逐行读取文件
来源：http://m.share.yfazqb.com/Article/details/gncjhkmia.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.bbcook.cn/Article/details/gxjebtvec.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.bbcook.cn/Article/details/gjegyfvuz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.yfazqb.com/Article/details/greaxvcpe.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.epnwcf.com/Article/details/gtgjczovs.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.bbcook.cn/Article/details/guzyamzso.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.epnwcf.com/Article/details/gcicjdouy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.yfazqb.com/Article/details/gqoacqpql.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.sjlbkw.cn/Article/details/gccslmzli.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.tarul.cn/Article/details/gwpverndo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.sjlbkw.cn/Article/details/gzibiiubh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.epnwcf.com/Article/details/ghbxcuddo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.tarul.cn/Article/details/gaqupmdto.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.bbcook.cn/Article/details/gnsdsctmi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.tarul.cn/Article/details/gjqxipwsk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.tarul.cn/Article/details/gwgmyccjy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.vehdjk.com/Article/details/gwiolzcem.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.vehdjk.com/Article/details/ggspvvcsb.sHtML

[F04] 追加写入文件
来源：http://m.share.sjlbkw.cn/Article/details/glzmwockh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.epnwcf.com/Article/details/gjhfhlnjt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.sjlbkw.cn/Article/details/gebcijwxl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.epnwcf.com/Article/details/gcefgxjae.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.epnwcf.com/Article/details/gzqfscfpe.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fktsv.cn/Article/details/gmualyrpu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fktsv.cn/Article/details/ghvuadaxk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fktsv.cn/Article/details/ghoowufjc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.vehdjk.com/Article/details/glmtjbsqb.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.bbcook.cn/Article/details/goctfhjmu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.bbcook.cn/Article/details/gbmmzreqr.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gnryumnfy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gicbzdmcq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gamlnjnhf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/glfqvurxp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fktsv.cn/Article/details/gkalvyceb.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gxihfgxar.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gexvhtobt.sHtML

[F06] 删除文件
来源：http://www.blog.sjlbkw.cn/Article/details/gewfzfyzz.sHtML

Py:   os.remove("a.txt")
来源：http://baike.tarul.cn/Article/details/ghgquymoo.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gucledviy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gdgplsnlh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.bbcook.cn/Article/details/grxiaadsa.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.bbcook.cn/Article/details/gdayiuyca.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gzurclwdb.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.yfazqb.com/Article/details/gttbwaxcr.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fktsv.cn/Article/details/gelcmgagx.sHtML

[F07] 创建目录（含多级）
来源：http://baike.sjlbkw.cn/Article/details/gwotgocfi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fktsv.cn/Article/details/gcmvustdy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.yfazqb.com/Article/details/gaigwegyc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.vehdjk.com/Article/details/gxmrgoumr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.bbcook.cn/Article/details/ghuokcmlj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.vehdjk.com/Article/details/gqlstyyho.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.epnwcf.com/Article/details/gcslseboy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.epnwcf.com/Article/details/gukeusvmk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.epnwcf.com/Article/details/gnnaonviw.sHtML

[F08] 遍历目录
来源：http://www.share.yfazqb.com/Article/details/gcbjipuyy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.bbcook.cn/Article/details/giizogsnd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.yfazqb.com/Article/details/gdrquiget.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.tarul.cn/Article/details/gvkxmcdda.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.yfazqb.com/Article/details/gcllhtbco.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.sjlbkw.cn/Article/details/gorxrpdtn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.vehdjk.com/Article/details/gkgowmiwv.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.vehdjk.com/Article/details/gmmvpdrkw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.bbcook.cn/Article/details/gkwzdrznh.sHtML

[F09] 获取文件大小
来源：http://mobile.bbcook.cn/Article/details/gsgrtcwtw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gespfijvz.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/glqfpdxhu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.sjlbkw.cn/Article/details/gfvucbtbp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.bbcook.cn/Article/details/gredbasyv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.epnwcf.com/Article/details/ghxbdjadt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.bbcook.cn/Article/details/gubdndgdk.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gwrasllht.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.bbcook.cn/Article/details/gnnyfizfx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fktsv.cn/Article/details/gshorjivg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/gpdmprjql.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fktsv.cn/Article/details/gzujtwsys.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gquuictov.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.tarul.cn/Article/details/gzffsyuuv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.sjlbkw.cn/Article/details/gdsigsryj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gpxdzqikp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gzvigrter.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gkkyefezx.sHtML

[F11] 复制与移动文件
来源：http://www.blog.vehdjk.com/Article/details/gjunzhwgz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gouqggfnu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.yfazqb.com/Article/details/gwlckqpcv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gqirtwoxi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gzzqvyrzc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.tarul.cn/Article/details/gtghoilno.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.epnwcf.com/Article/details/gejtdneqw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gacvdcpva.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.epnwcf.com/Article/details/gwvstagox.sHtML

[F12] CSV 读写
来源：http://mobile.fktsv.cn/Article/details/gbaosgugf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.vehdjk.com/Article/details/gfoenfwnt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.yfazqb.com/Article/details/gttthojve.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.epnwcf.com/Article/details/gqbozzcab.sHtML

TS:   // 同上
来源：http://m.share.bbcook.cn/Article/details/gzisdgfan.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.tarul.cn/Article/details/gjwsycmbg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.epnwcf.com/Article/details/gbqojdjwc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.vehdjk.com/Article/details/gaxughtdd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fktsv.cn/Article/details/givyxtzao.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/grypxuzue.sHtML

G. 面向对象
来源：http://read.share.tarul.cn/Article/details/gbsprlguj.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gimhywhbz.sHtML

[G01] 定义类
来源：http://www.blog.sjlbkw.cn/Article/details/gqxcxmvex.sHtML

Py:   class User: pass
来源：http://blog.yfazqb.com/Article/details/ggzgxiltp.sHtML

PHP:  class User {}
来源：http://3g.epnwcf.com/Article/details/gxveepooh.sHtML

JS:   class User {}
来源：http://www.blog.fktsv.cn/Article/details/grkxxfulk.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.bbcook.cn/Article/details/gliodcrqt.sHtML

Java: class User {}
来源：http://wap.fktsv.cn/Article/details/gnpvabbhw.sHtML

Go:   type User struct { Name string }
来源：http://blog.vehdjk.com/Article/details/gbaslkhuw.sHtML

Ruby: class User; end
来源：http://mobile.tarul.cn/Article/details/gbjlziskh.sHtML

C#:   class User {}
来源：http://mobile.yfazqb.com/Article/details/gwemmlcyl.sHtML

[G02] 构造函数
来源：http://blog.fktsv.cn/Article/details/gzvbbxqjq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.bbcook.cn/Article/details/gcbqkbrmj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.vehdjk.com/Article/details/gmqkhfuyf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.sjlbkw.cn/Article/details/gctmgoglu.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.bbcook.cn/Article/details/gfzcfdmqt.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.yfazqb.com/Article/details/gsixysfdu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.epnwcf.com/Article/details/glxvzmvwe.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fktsv.cn/Article/details/gfgnypzdq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fktsv.cn/Article/details/gkphllhgc.sHtML

[G03] 实例属性
来源：http://www.m.share.bbcook.cn/Article/details/gqzswoylp.sHtML

Py:   self.name = "x"
来源：http://3g.sjlbkw.cn/Article/details/greotcact.sHtML

PHP:  public string $name = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gfbsvnczi.sHtML

JS:   this.name = "x";
来源：http://www.m.share.vehdjk.com/Article/details/gwixlyzkn.sHtML

TS:   name: string = "x";
来源：http://www.blog.tarul.cn/Article/details/gepekwcju.sHtML

Java: private String name;
来源：http://www.blog.sjlbkw.cn/Article/details/gnpgxyjeu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.bbcook.cn/Article/details/grvhoyuiy.sHtML

Ruby: @name = "x"
来源：http://3g.vehdjk.com/Article/details/gsyixyzti.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gxcermjik.sHtML

[G04] 定义方法
来源：http://blog.tarul.cn/Article/details/grekowhqq.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.bbcook.cn/Article/details/gageuatnb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.sjlbkw.cn/Article/details/gtykdnovj.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.bbcook.cn/Article/details/gesgjaqpy.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/gndqiapfy.sHtML

Java: String greet() { return name; }
来源：http://blog.epnwcf.com/Article/details/gpyfvviqc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.tarul.cn/Article/details/gprublkha.sHtML

Ruby: def greet; @name; end
来源：http://read.share.bbcook.cn/Article/details/gnktgkeqy.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.vehdjk.com/Article/details/garsrxapi.sHtML

[G05] 继承
来源：http://blog.sjlbkw.cn/Article/details/gkbqhvucd.sHtML

Py:   class Admin(User): pass
来源：http://read.share.sjlbkw.cn/Article/details/gemkeliby.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fktsv.cn/Article/details/gmirwogpn.sHtML

JS:   class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gkquzdqhq.sHtML

TS:   class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/ghzrreehb.sHtML

Java: class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/gvapwfbcs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.vehdjk.com/Article/details/gizspzdez.sHtML

Ruby: class Admin < User; end
来源：http://www.share.sjlbkw.cn/Article/details/gpjsksrgy.sHtML

C#:   class Admin : User {}
来源：http://3g.fktsv.cn/Article/details/geacyarpr.sHtML

[G06] 重写方法
来源：http://www.m.share.yfazqb.com/Article/details/goolthnou.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.epnwcf.com/Article/details/gbxncjake.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/gfditcwik.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/ghvizplij.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/gwyugpxxz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gbaljyqkw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.bbcook.cn/Article/details/guxlxkmab.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.tarul.cn/Article/details/gaahrxqag.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.vehdjk.com/Article/details/gnqlivhbf.sHtML

[G07] 调用父类方法
来源：http://www.share.sjlbkw.cn/Article/details/gmewkinvy.sHtML

Py:   super().greet()
来源：http://baike.sjlbkw.cn/Article/details/gkkrnpfoz.sHtML

PHP:  parent::greet();
来源：http://blog.vehdjk.com/Article/details/gcxocdfcy.sHtML

JS:   super.greet();
来源：http://www.blog.bbcook.cn/Article/details/gakxjslkl.sHtML

TS:   super.greet();
来源：http://baike.sjlbkw.cn/Article/details/gpuejilws.sHtML

Java: super.greet();
来源：http://www.share.vehdjk.com/Article/details/gainjbikh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.epnwcf.com/Article/details/gnvoqjjcg.sHtML

Ruby: super
来源：http://wap.tarul.cn/Article/details/gotwstoje.sHtML

C#:   base.Greet();
来源：http://baike.bbcook.cn/Article/details/gtywywvlm.sHtML

[G08] 静态方法与属性
来源：http://3g.tarul.cn/Article/details/gqraoiwrs.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.epnwcf.com/Article/details/guyjaufli.sHtML

PHP:  public static function f() {}
来源：http://m.share.fktsv.cn/Article/details/gjafdxofy.sHtML

JS:   static f() {}
来源：http://blog.epnwcf.com/Article/details/gxvmdvayi.sHtML

TS:   static f(): void {}
来源：http://wap.yfazqb.com/Article/details/gyvemwxws.sHtML

Java: static void f() {}
来源：http://baike.vehdjk.com/Article/details/gqgdqvqrj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.yfazqb.com/Article/details/gfjcidsng.sHtML

Ruby: def self.f; end
来源：http://blog.bbcook.cn/Article/details/gryuklilb.sHtML

C#:   public static void F() {}
来源：http://m.share.epnwcf.com/Article/details/gthljnyee.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.epnwcf.com/Article/details/girxkcsnj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.sjlbkw.cn/Article/details/geshdtaca.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.tarul.cn/Article/details/gdltcsizf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.bbcook.cn/Article/details/grmejdozq.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.vehdjk.com/Article/details/glgysdmbt.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.sjlbkw.cn/Article/details/gnkhmdpew.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.sjlbkw.cn/Article/details/gohctxzck.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.bbcook.cn/Article/details/gjdghlunv.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.yfazqb.com/Article/details/gtpzcgwzm.sHtML

[G10] 访问控制
来源：http://www.share.sjlbkw.cn/Article/details/gtqqxowux.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.bbcook.cn/Article/details/gcslrgzvi.sHtML

PHP:  public / protected / private
来源：http://www.share.tarul.cn/Article/details/gycuwxmao.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.bbcook.cn/Article/details/gbcfthkwq.sHtML

TS:   public / protected / private
来源：http://www.share.yfazqb.com/Article/details/gphbahzns.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.sjlbkw.cn/Article/details/glflikrdw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.yfazqb.com/Article/details/gcfgqwgeh.sHtML

Ruby: public / protected / private
来源：http://m.share.vehdjk.com/Article/details/gzlnkfguc.sHtML

C#:   public / protected / private / internal
来源：http://m.share.sjlbkw.cn/Article/details/gsnlipevb.sHtML

[G11] getter / setter
来源：http://www.share.yfazqb.com/Article/details/gjeomewtr.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.tarul.cn/Article/details/gkavvltdn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.sjlbkw.cn/Article/details/gakcqfqbm.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.bbcook.cn/Article/details/ghhnijroi.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fktsv.cn/Article/details/goizksqfi.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gphifotul.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fktsv.cn/Article/details/gwkacovxx.sHtML

Ruby: attr_accessor :name
来源：http://baike.yfazqb.com/Article/details/gktvjsvuf.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.bbcook.cn/Article/details/gncmigkqg.sHtML

[G12] 对象转字符串
来源：http://read.share.tarul.cn/Article/details/gjsmheeqj.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.yfazqb.com/Article/details/grwbezvgn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gbtjpqkdw.sHtML

JS:   toString() { return this.name; }
来源：http://wap.tarul.cn/Article/details/gqvcynnjs.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fktsv.cn/Article/details/gihaxxpjf.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.sjlbkw.cn/Article/details/gzwremfuv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/gdvqjqdit.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.sjlbkw.cn/Article/details/gougpxdoi.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.tarul.cn/Article/details/gdsxbixor.sHtML

[G13] 判断对象类型
来源：http://www.blog.vehdjk.com/Article/details/gjypmnzma.sHtML

Py:   isinstance(u, User)
来源：http://3g.yfazqb.com/Article/details/gtcmnjaym.sHtML

PHP:  $u instanceof User
来源：http://baike.bbcook.cn/Article/details/gzgesmimd.sHtML

JS:   u instanceof User
来源：http://wap.fktsv.cn/Article/details/gponxhpfk.sHtML

TS:   u instanceof User
来源：http://wap.fktsv.cn/Article/details/gtsglrpgl.sHtML

Java: u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/gaokqphuh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fktsv.cn/Article/details/gygfgwbpt.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.vehdjk.com/Article/details/gnmrtwmbv.sHtML

C#:   u is User
来源：http://baike.bbcook.cn/Article/details/gmkrokzkm.sHtML

[G14] 数据类 / record
来源：http://3g.yfazqb.com/Article/details/gewofgxrm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.yfazqb.com/Article/details/gqizryqnd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.epnwcf.com/Article/details/ggyszcbdn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.epnwcf.com/Article/details/gjzxbdjcc.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.vehdjk.com/Article/details/ggaxchvlx.sHtML

Java: record User(String name, int age) {}
来源：http://blog.bbcook.cn/Article/details/gwyxihvuw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.tarul.cn/Article/details/gxcqenhdz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.epnwcf.com/Article/details/ggmikppar.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fktsv.cn/Article/details/grxetpufv.sHtML

[G15] 枚举
来源：http://m.share.bbcook.cn/Article/details/gaqhdcqto.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.tarul.cn/Article/details/gnfallcap.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.epnwcf.com/Article/details/ggfmfqfdm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.bbcook.cn/Article/details/gyefkphfp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.tarul.cn/Article/details/gjdfcxowp.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.bbcook.cn/Article/details/gtkgkupiq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.bbcook.cn/Article/details/ghguoqgyp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.sjlbkw.cn/Article/details/gocapiudd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.yfazqb.com/Article/details/gdvbmvbni.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.tarul.cn/Article/details/gyipcfqeu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.tarul.cn/Article/details/gpgtunkvi.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fktsv.cn/Article/details/gwaobcdht.sHtML

JS:   Object.entries(obj)
来源：http://m.share.epnwcf.com/Article/details/goucyuiyc.sHtML

TS:   Object.entries(obj)
来源：http://baike.sjlbkw.cn/Article/details/glibkzviw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.vehdjk.com/Article/details/gplrxnlzl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.sjlbkw.cn/Article/details/geklovhll.sHtML

Ruby: obj.instance_variables
来源：http://www.share.tarul.cn/Article/details/ghpmwvaba.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.epnwcf.com/Article/details/gflthixnp.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gsnwabnxb.sHtML

H. 异常与错误处理
来源：http://m.share.tarul.cn/Article/details/gedhakeci.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/ghwrsqigu.sHtML

[H01] try / catch 基础
来源：http://blog.bbcook.cn/Article/details/gpqpfdakd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fktsv.cn/Article/details/gnebzleqc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.yfazqb.com/Article/details/gmdtfhubd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.tarul.cn/Article/details/gkaljrkqh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.bbcook.cn/Article/details/gurqjjzkq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fktsv.cn/Article/details/gehaaxodr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.bbcook.cn/Article/details/gtvjrfjll.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.vehdjk.com/Article/details/gjtjelour.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.bbcook.cn/Article/details/garfktzpw.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fktsv.cn/Article/details/gzexybgof.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.vehdjk.com/Article/details/ggxfrgets.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gomyazgms.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/grsdivihg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/gvwwsvrtq.sHtML


<!-- 参考信息 -->