代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.epnwcf.com/Article/details/gdpawaima.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.sjlbkw.cn/Article/details/gfhsvxtiz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/ggibjhmpj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/gybckhkcq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.bbcook.cn/Article/details/ghkupfoop.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.vehdjk.com/Article/details/gprvegkdk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.epnwcf.com/Article/details/gacnrmcrc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.vehdjk.com/Article/details/gomqfiqga.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.yfazqb.com/Article/details/gqyfspogz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.bbcook.cn/Article/details/gwboslnmz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.yfazqb.com/Article/details/gbgylvead.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.sjlbkw.cn/Article/details/gbauqmdrm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.yfazqb.com/Article/details/ggnmqnnjr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.vehdjk.com/Article/details/gqnuvqpsc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.epnwcf.com/Article/details/ghdiswibx.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.bbcook.cn/Article/details/gbexjvwip.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.epnwcf.com/Article/details/gbfleegzj.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gxxikhlcb.sHtML

F. 文件与目录
来源：http://mobile.fktsv.cn/Article/details/gzwycjxtk.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gcjxccqbu.sHtML

[F01] 读取整个文件
来源：http://mobile.vehdjk.com/Article/details/gydeqjqgd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.epnwcf.com/Article/details/gykxocpal.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gawstijur.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.vehdjk.com/Article/details/ggjilzcnx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.bbcook.cn/Article/details/gxhfbvizq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gmyuatohb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fktsv.cn/Article/details/gqlhwwrya.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gyfnbxakl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.bbcook.cn/Article/details/gscsknles.sHtML

[F02] 逐行读取文件
来源：http://www.share.sjlbkw.cn/Article/details/gpqnzudup.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.tarul.cn/Article/details/ghsryjvbt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fktsv.cn/Article/details/gfkylqelh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.sjlbkw.cn/Article/details/gcnessoec.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.epnwcf.com/Article/details/gkrigriyq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.vehdjk.com/Article/details/gjycexpus.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.vehdjk.com/Article/details/ggypklrim.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.tarul.cn/Article/details/gmtpnisxj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.yfazqb.com/Article/details/gmdbhrfck.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.vehdjk.com/Article/details/gnlvhytjx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.sjlbkw.cn/Article/details/gaqnpoprt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.bbcook.cn/Article/details/gdhtyauxn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.sjlbkw.cn/Article/details/gjbeyddpo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.tarul.cn/Article/details/gshqubtrp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.epnwcf.com/Article/details/geuemjlso.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fktsv.cn/Article/details/gtopjhmfh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fktsv.cn/Article/details/ghblgdcjs.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.bbcook.cn/Article/details/gglsvcnuv.sHtML

[F04] 追加写入文件
来源：http://baike.bbcook.cn/Article/details/ghiainmwx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.yfazqb.com/Article/details/gbvctxqwt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.tarul.cn/Article/details/gnxncpdqx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.epnwcf.com/Article/details/gpnhxulwx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.epnwcf.com/Article/details/gfazickip.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.yfazqb.com/Article/details/gjisennig.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.vehdjk.com/Article/details/gizbdhhaz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fktsv.cn/Article/details/gtsturbpm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.tarul.cn/Article/details/giztqqeag.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.yfazqb.com/Article/details/gkmyoduua.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.vehdjk.com/Article/details/gwpyplvlc.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.yfazqb.com/Article/details/grgtnrrej.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/gkrjcalla.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.epnwcf.com/Article/details/gfkeabzpc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/gmhgnlrmn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.vehdjk.com/Article/details/gsiziercd.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.bbcook.cn/Article/details/gkgkpazcm.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fktsv.cn/Article/details/gitbyousj.sHtML

[F06] 删除文件
来源：http://www.share.tarul.cn/Article/details/glnqdepfy.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gzuodmcsf.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gczfjxirx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/goccdhlql.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/gnpaqsxzc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.tarul.cn/Article/details/gzqwdxuby.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gvhfgnmfy.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gqwnsafpp.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gzfopgdwt.sHtML

[F07] 创建目录（含多级）
来源：http://wap.yfazqb.com/Article/details/gaotbqqff.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fktsv.cn/Article/details/gcabnceqb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fktsv.cn/Article/details/gtjjkphhr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.sjlbkw.cn/Article/details/geflgdmmz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.sjlbkw.cn/Article/details/gaolgylzm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.sjlbkw.cn/Article/details/gpnytuphy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.tarul.cn/Article/details/gjwcanziw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.sjlbkw.cn/Article/details/gzvexpsld.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.yfazqb.com/Article/details/gkgqjjbxl.sHtML

[F08] 遍历目录
来源：http://www.m.share.epnwcf.com/Article/details/gtsbtxguy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.yfazqb.com/Article/details/gigidlqtx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.vehdjk.com/Article/details/gquimftyl.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.yfazqb.com/Article/details/gtrxcrqzd.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.sjlbkw.cn/Article/details/gxcdbohzb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.tarul.cn/Article/details/gwgdduewz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.yfazqb.com/Article/details/ggogljgxk.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fktsv.cn/Article/details/gegqnjbeo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.tarul.cn/Article/details/glzputayj.sHtML

[F09] 获取文件大小
来源：http://baike.sjlbkw.cn/Article/details/gzjkjindv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gkvuxfbvz.sHtML

PHP:  filesize("a.txt");
来源：http://3g.yfazqb.com/Article/details/gcnbuxczm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.yfazqb.com/Article/details/gfrtlxjpd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.bbcook.cn/Article/details/gvheuwkub.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.vehdjk.com/Article/details/gfjvxtmxu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.yfazqb.com/Article/details/gznucyipa.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gyvglucbs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fktsv.cn/Article/details/gfnwxzlrq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.epnwcf.com/Article/details/gxfzcjyti.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjuuujxjb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.yfazqb.com/Article/details/gsyvuxefx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gmoabxeep.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/ggmiuoqns.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fktsv.cn/Article/details/gtbhydivs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gvbhhxrga.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gqpsxnlvt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/gegtkobyp.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fktsv.cn/Article/details/gcoikprls.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/gllerkjod.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fktsv.cn/Article/details/gxmxtdnbq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/gbubojpsd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gbsmbglbw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.vehdjk.com/Article/details/glfsbgfdo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.yfazqb.com/Article/details/gcomkykqg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/gbkziugza.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.vehdjk.com/Article/details/gzgourqrh.sHtML

[F12] CSV 读写
来源：http://mobile.vehdjk.com/Article/details/ggfuzegbd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.bbcook.cn/Article/details/grkjygkfy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.tarul.cn/Article/details/gnglklfqm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.bbcook.cn/Article/details/gefeoment.sHtML

TS:   // 同上
来源：http://blog.sjlbkw.cn/Article/details/gfphqkwph.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fktsv.cn/Article/details/ggevjgdwf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.vehdjk.com/Article/details/glceliyzz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.yfazqb.com/Article/details/grklzwfhn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.yfazqb.com/Article/details/ggfaqrmza.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gajkapfvv.sHtML

G. 面向对象
来源：http://mobile.yfazqb.com/Article/details/gzvpuifex.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gvoqomsdx.sHtML

[G01] 定义类
来源：http://blog.fktsv.cn/Article/details/gxyilzvuv.sHtML

Py:   class User: pass
来源：http://www.blog.sjlbkw.cn/Article/details/gqfjbcryj.sHtML

PHP:  class User {}
来源：http://www.m.share.yfazqb.com/Article/details/gtetlwkzk.sHtML

JS:   class User {}
来源：http://3g.yfazqb.com/Article/details/gdxbwcyaj.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.yfazqb.com/Article/details/grgwztgiy.sHtML

Java: class User {}
来源：http://www.share.fktsv.cn/Article/details/gwfbrvlda.sHtML

Go:   type User struct { Name string }
来源：http://www.share.bbcook.cn/Article/details/gdorebqod.sHtML

Ruby: class User; end
来源：http://wap.bbcook.cn/Article/details/gkwomzafj.sHtML

C#:   class User {}
来源：http://mobile.yfazqb.com/Article/details/glpbkyibz.sHtML

[G02] 构造函数
来源：http://wap.yfazqb.com/Article/details/gidnpshpy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fktsv.cn/Article/details/gdrmijmog.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.sjlbkw.cn/Article/details/gsjvvqjnk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fktsv.cn/Article/details/gtcumurof.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.tarul.cn/Article/details/godjcrrfm.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fktsv.cn/Article/details/gdkbyhees.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.tarul.cn/Article/details/gtrjerefg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.tarul.cn/Article/details/gmwipbpnq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.bbcook.cn/Article/details/gsndelpdq.sHtML

[G03] 实例属性
来源：http://m.share.vehdjk.com/Article/details/gntnumvkl.sHtML

Py:   self.name = "x"
来源：http://wap.sjlbkw.cn/Article/details/gmxefgzvr.sHtML

PHP:  public string $name = "x";
来源：http://baike.bbcook.cn/Article/details/gwwfyedtp.sHtML

JS:   this.name = "x";
来源：http://baike.vehdjk.com/Article/details/gkoywbwga.sHtML

TS:   name: string = "x";
来源：http://3g.yfazqb.com/Article/details/gdcjajori.sHtML

Java: private String name;
来源：http://blog.vehdjk.com/Article/details/gsasjlvmv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.vehdjk.com/Article/details/ggfbgzcep.sHtML

Ruby: @name = "x"
来源：http://m.share.fktsv.cn/Article/details/gfltsafob.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.tarul.cn/Article/details/gcylruzwd.sHtML

[G04] 定义方法
来源：http://wap.yfazqb.com/Article/details/gojxufjyd.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.tarul.cn/Article/details/gqqmpwxsr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.tarul.cn/Article/details/gnulvoadu.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fktsv.cn/Article/details/gefisthlz.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gzaoxfwvg.sHtML

Java: String greet() { return name; }
来源：http://wap.fktsv.cn/Article/details/gmkxzwgcw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.vehdjk.com/Article/details/gscqlfhhc.sHtML

Ruby: def greet; @name; end
来源：http://read.share.tarul.cn/Article/details/gldgmoyjm.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.sjlbkw.cn/Article/details/gnitploby.sHtML

[G05] 继承
来源：http://blog.tarul.cn/Article/details/gajwdidtw.sHtML

Py:   class Admin(User): pass
来源：http://3g.tarul.cn/Article/details/gnoeeaxno.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/gfokvslds.sHtML

JS:   class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/ghcesjudj.sHtML

TS:   class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/grildbuhl.sHtML

Java: class Admin extends User {}
来源：http://mobile.fktsv.cn/Article/details/gnsajqnbo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.vehdjk.com/Article/details/geskmlzhm.sHtML

Ruby: class Admin < User; end
来源：http://mobile.epnwcf.com/Article/details/gpxdmqdrh.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.vehdjk.com/Article/details/gldqhlpvi.sHtML

[G06] 重写方法
来源：http://www.share.yfazqb.com/Article/details/gdodjpshj.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.vehdjk.com/Article/details/gljxhlfst.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/gwzxyilta.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fktsv.cn/Article/details/glyzupqny.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/gxwtdatdm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/gxuwpsdgd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.vehdjk.com/Article/details/gvyyxngsj.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.tarul.cn/Article/details/gluknzvdp.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fktsv.cn/Article/details/gyeazfpiu.sHtML

[G07] 调用父类方法
来源：http://www.share.vehdjk.com/Article/details/gxriwokdn.sHtML

Py:   super().greet()
来源：http://wap.fktsv.cn/Article/details/gctxdjygj.sHtML

PHP:  parent::greet();
来源：http://wap.yfazqb.com/Article/details/gtjethldr.sHtML

JS:   super.greet();
来源：http://baike.sjlbkw.cn/Article/details/gymdlpnsc.sHtML

TS:   super.greet();
来源：http://3g.yfazqb.com/Article/details/gkwoqrivh.sHtML

Java: super.greet();
来源：http://read.share.yfazqb.com/Article/details/gjutexrza.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.epnwcf.com/Article/details/ghuwsatmp.sHtML

Ruby: super
来源：http://mobile.sjlbkw.cn/Article/details/gpnmdomjh.sHtML

C#:   base.Greet();
来源：http://baike.tarul.cn/Article/details/gzfwimhia.sHtML

[G08] 静态方法与属性
来源：http://read.share.bbcook.cn/Article/details/ggrcaxxpc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.yfazqb.com/Article/details/gosjmctlq.sHtML

PHP:  public static function f() {}
来源：http://www.blog.yfazqb.com/Article/details/gytnmmxrh.sHtML

JS:   static f() {}
来源：http://baike.epnwcf.com/Article/details/gadnzbygl.sHtML

TS:   static f(): void {}
来源：http://www.share.epnwcf.com/Article/details/gmurzjsrt.sHtML

Java: static void f() {}
来源：http://baike.sjlbkw.cn/Article/details/gxzrhkmhc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.yfazqb.com/Article/details/gfllwkyes.sHtML

Ruby: def self.f; end
来源：http://www.share.bbcook.cn/Article/details/gvjvwfcbx.sHtML

C#:   public static void F() {}
来源：http://www.m.share.yfazqb.com/Article/details/grdrlhsub.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fktsv.cn/Article/details/gffuzfmkl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.yfazqb.com/Article/details/gjfaeozto.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.epnwcf.com/Article/details/gqodogjpq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.epnwcf.com/Article/details/gijbjkqdd.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gawtwsueo.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.yfazqb.com/Article/details/gwwsypsau.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.sjlbkw.cn/Article/details/gfwilkmya.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.yfazqb.com/Article/details/gyzvtvqkn.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.sjlbkw.cn/Article/details/gavsdarmr.sHtML

[G10] 访问控制
来源：http://www.m.share.epnwcf.com/Article/details/ghmogaxwp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.bbcook.cn/Article/details/gstzjvunh.sHtML

PHP:  public / protected / private
来源：http://www.m.share.vehdjk.com/Article/details/gujxlgzmq.sHtML

JS:   #private 字段；其余公开
来源：http://blog.yfazqb.com/Article/details/gmfzlzozc.sHtML

TS:   public / protected / private
来源：http://m.share.bbcook.cn/Article/details/gtbvricgm.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.yfazqb.com/Article/details/gggmbutws.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.yfazqb.com/Article/details/gfoliiyuf.sHtML

Ruby: public / protected / private
来源：http://m.share.epnwcf.com/Article/details/gdngezzty.sHtML

C#:   public / protected / private / internal
来源：http://mobile.tarul.cn/Article/details/ggmlusvxj.sHtML

[G11] getter / setter
来源：http://read.share.yfazqb.com/Article/details/gvxhqwbko.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fktsv.cn/Article/details/gvcnxqnfo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.yfazqb.com/Article/details/gknfwuhzb.sHtML

JS:   get name() { return this._name; }
来源：http://3g.sjlbkw.cn/Article/details/gkqzysotz.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.yfazqb.com/Article/details/gyyohcmwg.sHtML

Java: public String getName() { return name; }
来源：http://3g.bbcook.cn/Article/details/grlfyvkps.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fktsv.cn/Article/details/gscblcfoi.sHtML

Ruby: attr_accessor :name
来源：http://3g.sjlbkw.cn/Article/details/geedtcghk.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.bbcook.cn/Article/details/goqzlltgv.sHtML

[G12] 对象转字符串
来源：http://wap.tarul.cn/Article/details/gjepnllqk.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.epnwcf.com/Article/details/gzgaspuhu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.bbcook.cn/Article/details/guugkfqyv.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.bbcook.cn/Article/details/gkfnoaidd.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.tarul.cn/Article/details/gcdnrjvwb.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.tarul.cn/Article/details/gvquhydxy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/gdyxdfqyp.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fktsv.cn/Article/details/galugykcs.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.yfazqb.com/Article/details/gihdzecll.sHtML

[G13] 判断对象类型
来源：http://www.blog.bbcook.cn/Article/details/goproeunq.sHtML

Py:   isinstance(u, User)
来源：http://blog.vehdjk.com/Article/details/gohusczgn.sHtML

PHP:  $u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/gyuarhdrb.sHtML

JS:   u instanceof User
来源：http://www.share.epnwcf.com/Article/details/gvyuomxpb.sHtML

TS:   u instanceof User
来源：http://www.share.bbcook.cn/Article/details/gzsthmdpl.sHtML

Java: u instanceof User
来源：http://m.share.bbcook.cn/Article/details/gxdxalfvy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.sjlbkw.cn/Article/details/grdqwehxx.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fktsv.cn/Article/details/ggwbozyue.sHtML

C#:   u is User
来源：http://www.blog.sjlbkw.cn/Article/details/gfdkrwqxm.sHtML

[G14] 数据类 / record
来源：http://m.share.sjlbkw.cn/Article/details/gikrzkenc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.sjlbkw.cn/Article/details/guyuegvee.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.sjlbkw.cn/Article/details/gkxuekxrl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.sjlbkw.cn/Article/details/gxzamlawh.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.epnwcf.com/Article/details/gixfejgrp.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.sjlbkw.cn/Article/details/gvrpulkoo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.yfazqb.com/Article/details/gdmmnxttu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.bbcook.cn/Article/details/gxzcihkoz.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fktsv.cn/Article/details/gaizaxyir.sHtML

[G15] 枚举
来源：http://3g.tarul.cn/Article/details/gysclovyc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.epnwcf.com/Article/details/goszrwvid.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fktsv.cn/Article/details/gbqkuzalb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.yfazqb.com/Article/details/gdvjnzmem.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.yfazqb.com/Article/details/glqlycbmi.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.bbcook.cn/Article/details/gautumsbr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.vehdjk.com/Article/details/grgrqlmec.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.vehdjk.com/Article/details/gfzlrifgp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.tarul.cn/Article/details/gkihuqdtz.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.sjlbkw.cn/Article/details/ggcrgqwfh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.epnwcf.com/Article/details/gxcgrkzjz.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.sjlbkw.cn/Article/details/gtskxqpso.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fktsv.cn/Article/details/geaxdcjxq.sHtML

TS:   Object.entries(obj)
来源：http://3g.vehdjk.com/Article/details/giritcrxz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.epnwcf.com/Article/details/gjyvpegin.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.tarul.cn/Article/details/ggddhqimx.sHtML

Ruby: obj.instance_variables
来源：http://blog.sjlbkw.cn/Article/details/gbxmrxppy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.vehdjk.com/Article/details/gxofmzjuf.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gyijgohje.sHtML

H. 异常与错误处理
来源：http://www.m.share.vehdjk.com/Article/details/gffdeashx.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gnkkewtzd.sHtML

[H01] try / catch 基础
来源：http://www.m.share.tarul.cn/Article/details/gcemrmnad.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fktsv.cn/Article/details/gxhfihuxw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.vehdjk.com/Article/details/ggiznnubd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.tarul.cn/Article/details/gmoomolmo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.epnwcf.com/Article/details/guaufzvif.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.yfazqb.com/Article/details/gboexeros.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.yfazqb.com/Article/details/gyosfkupc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fktsv.cn/Article/details/gmwizejyx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.tarul.cn/Article/details/gmrlvnbrb.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.bbcook.cn/Article/details/gnshfwnux.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.yfazqb.com/Article/details/gpkouhabg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fktsv.cn/Article/details/gpvxwrtjx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gsjgmqwrx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.tarul.cn/Article/details/geysocwfc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gssrwsupi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.vehdjk.com/Article/details/grejxdsdv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.tarul.cn/Article/details/grxzjjksn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.epnwcf.com/Article/details/gqsdisgnf.sHtML

[H03] 主动抛出异常
来源：http://wap.vehdjk.com/Article/details/grjbdzvgx.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.tarul.cn/Article/details/ghhnlfjjy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/ghoehucxi.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/gqdygczgf.sHtML


<!-- 参考信息 -->