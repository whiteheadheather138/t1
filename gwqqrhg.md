代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.tarul.cn/Article/details/ggivxgivc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gofrhpjoo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.bbcook.cn/Article/details/gyyalwkvy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.yfazqb.com/Article/details/gmbvpgrzx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fktsv.cn/Article/details/goabwyxfp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.epnwcf.com/Article/details/gackhheca.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gevqlowfb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gvpfrozar.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.bbcook.cn/Article/details/gfuzlsiyg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.bbcook.cn/Article/details/gzaofzjrr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/gcciqnede.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.vehdjk.com/Article/details/glknkgsol.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.sjlbkw.cn/Article/details/gnhtbjpkt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.sjlbkw.cn/Article/details/gvjaxwuxv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.bbcook.cn/Article/details/gcwrumadk.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.bbcook.cn/Article/details/gtkflzhiu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fktsv.cn/Article/details/gobyyffaz.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/grbhsodpx.sHtML

F. 文件与目录
来源：http://baike.yfazqb.com/Article/details/gztwoxuiy.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gswktiopo.sHtML

[F01] 读取整个文件
来源：http://m.share.vehdjk.com/Article/details/gdvztamms.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.vehdjk.com/Article/details/ghuihvoyg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gslikstqt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fktsv.cn/Article/details/glnickiqr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.sjlbkw.cn/Article/details/gioumbjfo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.bbcook.cn/Article/details/gzoicsums.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fktsv.cn/Article/details/grdtzlned.sHtML

Ruby: File.read("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gevqxgxsc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gqxuditus.sHtML

[F02] 逐行读取文件
来源：http://mobile.yfazqb.com/Article/details/gojjzcnfd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.yfazqb.com/Article/details/gvbmgaaor.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.yfazqb.com/Article/details/gbsfhjmxr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.tarul.cn/Article/details/gjeyppmeo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.yfazqb.com/Article/details/gpsyqnxkc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fktsv.cn/Article/details/gvjlofjwm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.vehdjk.com/Article/details/giklshitu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.epnwcf.com/Article/details/gqwalmjoa.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.epnwcf.com/Article/details/gdgrkkdif.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.yfazqb.com/Article/details/ghykodvjc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.epnwcf.com/Article/details/gwhjllikl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fktsv.cn/Article/details/gfignauup.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.yfazqb.com/Article/details/gryxnkqgf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.epnwcf.com/Article/details/gurcjgyaj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.epnwcf.com/Article/details/gvfbpuphy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.epnwcf.com/Article/details/ghpvnierj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fktsv.cn/Article/details/grbsbxbha.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.epnwcf.com/Article/details/gkgzzzage.sHtML

[F04] 追加写入文件
来源：http://www.m.share.vehdjk.com/Article/details/gpoiqksbx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.yfazqb.com/Article/details/gnymssxab.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.tarul.cn/Article/details/gixeekhdg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.tarul.cn/Article/details/gopcdrtri.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.vehdjk.com/Article/details/gjnslefkq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.bbcook.cn/Article/details/gnnnykaol.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.yfazqb.com/Article/details/gfniqqfxw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.epnwcf.com/Article/details/gedxnkhoa.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.sjlbkw.cn/Article/details/gwjozkcnh.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.epnwcf.com/Article/details/gobvgdnsj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fktsv.cn/Article/details/gaibbnqqu.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.tarul.cn/Article/details/gjkadxhea.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.bbcook.cn/Article/details/ggwnrkame.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gbjqpsinr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/gsrihyxvh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.epnwcf.com/Article/details/gtbmkqwty.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gysalphqi.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.bbcook.cn/Article/details/ggnbuhheu.sHtML

[F06] 删除文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gvkmdmxjf.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gjbkqwbad.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gxmogswlc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/guxtpsomk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.yfazqb.com/Article/details/gqwvwdiph.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.vehdjk.com/Article/details/gkenbedxt.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gkcuikdjj.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fktsv.cn/Article/details/ggurhymkd.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gcfibtgeb.sHtML

[F07] 创建目录（含多级）
来源：http://blog.sjlbkw.cn/Article/details/gajqwulow.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.yfazqb.com/Article/details/gitbmcvcw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fktsv.cn/Article/details/ggpbbymxs.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.vehdjk.com/Article/details/ghexngond.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.sjlbkw.cn/Article/details/gzqxfrcgw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.bbcook.cn/Article/details/guglrlkna.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fktsv.cn/Article/details/gvizjrqwy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.yfazqb.com/Article/details/gyfhlkanv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.vehdjk.com/Article/details/gckreccpt.sHtML

[F08] 遍历目录
来源：http://m.share.fktsv.cn/Article/details/gziobtgji.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fktsv.cn/Article/details/gwartviik.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.yfazqb.com/Article/details/giojjmtbl.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fktsv.cn/Article/details/gpcpyxsea.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.bbcook.cn/Article/details/gnjxikmsh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.bbcook.cn/Article/details/ggonkcjja.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.vehdjk.com/Article/details/grtaucwnv.sHtML

Ruby: Dir.children("dir")
来源：http://wap.bbcook.cn/Article/details/ghlabwiqy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.epnwcf.com/Article/details/gksoimhgw.sHtML

[F09] 获取文件大小
来源：http://www.blog.sjlbkw.cn/Article/details/gijsqhmne.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gsalvvoyz.sHtML

PHP:  filesize("a.txt");
来源：http://3g.tarul.cn/Article/details/gbildopai.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.vehdjk.com/Article/details/gzemohgrf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.vehdjk.com/Article/details/gbyfqxafe.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gaelgxbwe.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.bbcook.cn/Article/details/glxdvbgzu.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gulmjyxhu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.tarul.cn/Article/details/giidbowfz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.tarul.cn/Article/details/goimqxhkz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gqdeertcw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.yfazqb.com/Article/details/guivpdvvs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gqqbhxfsc.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fktsv.cn/Article/details/gitylupba.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.epnwcf.com/Article/details/gysddgzmc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gduedqhuj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gfapuntth.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gjtakeyqy.sHtML

[F11] 复制与移动文件
来源：http://www.share.epnwcf.com/Article/details/gqtycfdph.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/gotzksaye.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.bbcook.cn/Article/details/gulossrqw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.vehdjk.com/Article/details/gmgpzxfgr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/gtwucnpph.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtfqpoutr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.tarul.cn/Article/details/gmdpdwbje.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.vehdjk.com/Article/details/gjremjctg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.tarul.cn/Article/details/gdzoixsxc.sHtML

[F12] CSV 读写
来源：http://3g.sjlbkw.cn/Article/details/gckyqnvvh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.epnwcf.com/Article/details/geskkulji.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.yfazqb.com/Article/details/gormqdqww.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.vehdjk.com/Article/details/grdpryxol.sHtML

TS:   // 同上
来源：http://3g.sjlbkw.cn/Article/details/gvhctaewb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.bbcook.cn/Article/details/gylwkgpzs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.bbcook.cn/Article/details/gyvartgyw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.vehdjk.com/Article/details/gknccbfbp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.epnwcf.com/Article/details/ghzekbfyo.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gyhdddyap.sHtML

G. 面向对象
来源：http://3g.bbcook.cn/Article/details/gqhyozmrs.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/ghlttsezd.sHtML

[G01] 定义类
来源：http://baike.sjlbkw.cn/Article/details/gckldmmbc.sHtML

Py:   class User: pass
来源：http://blog.yfazqb.com/Article/details/ggtdtokwx.sHtML

PHP:  class User {}
来源：http://mobile.fktsv.cn/Article/details/gahfglept.sHtML

JS:   class User {}
来源：http://wap.yfazqb.com/Article/details/gvmcfkqgd.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.yfazqb.com/Article/details/gnubeeqco.sHtML

Java: class User {}
来源：http://read.share.tarul.cn/Article/details/guadthbwm.sHtML

Go:   type User struct { Name string }
来源：http://mobile.tarul.cn/Article/details/giaiyoiak.sHtML

Ruby: class User; end
来源：http://mobile.fktsv.cn/Article/details/giwrmelsu.sHtML

C#:   class User {}
来源：http://3g.tarul.cn/Article/details/gvflajfbn.sHtML

[G02] 构造函数
来源：http://blog.bbcook.cn/Article/details/givmhzgfp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.epnwcf.com/Article/details/gomtxtffd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.yfazqb.com/Article/details/gvwzbaioi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.epnwcf.com/Article/details/gwakldavf.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.yfazqb.com/Article/details/geouegaeh.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.sjlbkw.cn/Article/details/gajiiosku.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.sjlbkw.cn/Article/details/ggnczuwms.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fktsv.cn/Article/details/gvlpzerac.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gnyajmfvv.sHtML

[G03] 实例属性
来源：http://3g.epnwcf.com/Article/details/guhurddko.sHtML

Py:   self.name = "x"
来源：http://baike.vehdjk.com/Article/details/goaibmwpv.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.bbcook.cn/Article/details/gqnxcqjpo.sHtML

JS:   this.name = "x";
来源：http://www.share.yfazqb.com/Article/details/gokjmxtds.sHtML

TS:   name: string = "x";
来源：http://baike.epnwcf.com/Article/details/gdabkvmwn.sHtML

Java: private String name;
来源：http://read.share.bbcook.cn/Article/details/gdbxjtohy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.sjlbkw.cn/Article/details/gcsikrehn.sHtML

Ruby: @name = "x"
来源：http://3g.yfazqb.com/Article/details/ggdhtrlmm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.epnwcf.com/Article/details/glrzyyqaa.sHtML

[G04] 定义方法
来源：http://www.blog.sjlbkw.cn/Article/details/grvlhyxwb.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.epnwcf.com/Article/details/glupekoad.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.tarul.cn/Article/details/gekprbsxn.sHtML

JS:   greet() { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gngvbmzle.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/ggjuxzuuj.sHtML

Java: String greet() { return name; }
来源：http://m.share.tarul.cn/Article/details/gtwndbbfu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.bbcook.cn/Article/details/gxfjfmhyr.sHtML

Ruby: def greet; @name; end
来源：http://mobile.vehdjk.com/Article/details/gwyscpsxq.sHtML

C#:   public string Greet() => Name;
来源：http://3g.epnwcf.com/Article/details/gyzqsusgc.sHtML

[G05] 继承
来源：http://www.m.share.tarul.cn/Article/details/gyeawrilf.sHtML

Py:   class Admin(User): pass
来源：http://baike.epnwcf.com/Article/details/gnhbsukdm.sHtML

PHP:  class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gpwoefaiv.sHtML

JS:   class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/gdhfebmop.sHtML

TS:   class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gusvkaoor.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/gmjqwtibe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.sjlbkw.cn/Article/details/gnlmjtnhy.sHtML

Ruby: class Admin < User; end
来源：http://mobile.vehdjk.com/Article/details/giyfljlms.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fktsv.cn/Article/details/guhuklvgm.sHtML

[G06] 重写方法
来源：http://read.share.sjlbkw.cn/Article/details/gnyhmhbpt.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.sjlbkw.cn/Article/details/gekvmekph.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gpthevccb.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/gdoztgcia.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/guhaackbn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/gvqpucacy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.epnwcf.com/Article/details/gcqqefopy.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.tarul.cn/Article/details/gyzdobqvx.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.tarul.cn/Article/details/gikflpdzh.sHtML

[G07] 调用父类方法
来源：http://mobile.fktsv.cn/Article/details/gzyvnlghf.sHtML

Py:   super().greet()
来源：http://wap.sjlbkw.cn/Article/details/gklrouyww.sHtML

PHP:  parent::greet();
来源：http://www.m.share.epnwcf.com/Article/details/gpeozqznl.sHtML

JS:   super.greet();
来源：http://blog.vehdjk.com/Article/details/gakgddzke.sHtML

TS:   super.greet();
来源：http://m.share.yfazqb.com/Article/details/gyjqtgrum.sHtML

Java: super.greet();
来源：http://www.blog.sjlbkw.cn/Article/details/gwoaibaxx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fktsv.cn/Article/details/gkiddhmnz.sHtML

Ruby: super
来源：http://www.blog.tarul.cn/Article/details/gidxbenes.sHtML

C#:   base.Greet();
来源：http://baike.fktsv.cn/Article/details/gpyftbqce.sHtML

[G08] 静态方法与属性
来源：http://www.blog.sjlbkw.cn/Article/details/gcydnavaf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.tarul.cn/Article/details/gwppapxxm.sHtML

PHP:  public static function f() {}
来源：http://www.blog.vehdjk.com/Article/details/gwbqfpfts.sHtML

JS:   static f() {}
来源：http://www.m.share.yfazqb.com/Article/details/gtvhiyild.sHtML

TS:   static f(): void {}
来源：http://baike.epnwcf.com/Article/details/ghwotmvng.sHtML

Java: static void f() {}
来源：http://read.share.yfazqb.com/Article/details/gxaqlebwe.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.sjlbkw.cn/Article/details/ghkebslug.sHtML

Ruby: def self.f; end
来源：http://www.blog.bbcook.cn/Article/details/glorytpoa.sHtML

C#:   public static void F() {}
来源：http://baike.fktsv.cn/Article/details/gkpgjknde.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.bbcook.cn/Article/details/gojjxsfow.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.tarul.cn/Article/details/gklgghbvq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.bbcook.cn/Article/details/gdxrtjdby.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fktsv.cn/Article/details/gqohguueq.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fktsv.cn/Article/details/gdmblqpnf.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.vehdjk.com/Article/details/gcmhvkkdp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.tarul.cn/Article/details/ghjcwozoq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.vehdjk.com/Article/details/gtgyijoem.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fktsv.cn/Article/details/gxutiojot.sHtML

[G10] 访问控制
来源：http://www.m.share.epnwcf.com/Article/details/gwhevoyav.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.epnwcf.com/Article/details/gonohvteh.sHtML

PHP:  public / protected / private
来源：http://blog.bbcook.cn/Article/details/ggfwyuhyo.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.tarul.cn/Article/details/gijuoczxy.sHtML

TS:   public / protected / private
来源：http://read.share.fktsv.cn/Article/details/gouoyeezf.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.epnwcf.com/Article/details/grgaskogl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.bbcook.cn/Article/details/ghzjgfuwa.sHtML

Ruby: public / protected / private
来源：http://3g.fktsv.cn/Article/details/gilgzhlue.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.yfazqb.com/Article/details/gxfcboofl.sHtML

[G11] getter / setter
来源：http://read.share.bbcook.cn/Article/details/ghrdjzczy.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.tarul.cn/Article/details/gkhpxttpj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.bbcook.cn/Article/details/grajqarpx.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fktsv.cn/Article/details/gmpwdbzza.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.bbcook.cn/Article/details/gdiqsbxqo.sHtML

Java: public String getName() { return name; }
来源：http://www.share.epnwcf.com/Article/details/gwiiusdxd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.yfazqb.com/Article/details/ggimccllc.sHtML

Ruby: attr_accessor :name
来源：http://3g.yfazqb.com/Article/details/gbmkiorxh.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.epnwcf.com/Article/details/gyumwpepz.sHtML

[G12] 对象转字符串
来源：http://read.share.sjlbkw.cn/Article/details/gcfpxxaji.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.vehdjk.com/Article/details/glbsbzhgj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.tarul.cn/Article/details/gvrdzzivv.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/gidoqseho.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.yfazqb.com/Article/details/gkngpizeu.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gsofidmuo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.sjlbkw.cn/Article/details/gfwtgjlqn.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fktsv.cn/Article/details/gushhtlkz.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.sjlbkw.cn/Article/details/gddilygbn.sHtML

[G13] 判断对象类型
来源：http://www.share.vehdjk.com/Article/details/gujrrweym.sHtML

Py:   isinstance(u, User)
来源：http://read.share.sjlbkw.cn/Article/details/gtrxqvqkw.sHtML

PHP:  $u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gwzjuggus.sHtML

JS:   u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gxiwuaifi.sHtML

TS:   u instanceof User
来源：http://baike.epnwcf.com/Article/details/gzomfessu.sHtML

Java: u instanceof User
来源：http://mobile.bbcook.cn/Article/details/grweuvnpe.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fktsv.cn/Article/details/gpwypaycj.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.sjlbkw.cn/Article/details/gbezrmvky.sHtML

C#:   u is User
来源：http://www.share.vehdjk.com/Article/details/gfdgglqsd.sHtML

[G14] 数据类 / record
来源：http://mobile.bbcook.cn/Article/details/gdjvpvqal.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.sjlbkw.cn/Article/details/gcabwualw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.vehdjk.com/Article/details/gjroicdiv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.epnwcf.com/Article/details/gvsdgqkwj.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.sjlbkw.cn/Article/details/gshpwloht.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.vehdjk.com/Article/details/gwgjkaihr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.epnwcf.com/Article/details/gutcstptr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.epnwcf.com/Article/details/gyujutpsy.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fktsv.cn/Article/details/gxzgfqkwz.sHtML

[G15] 枚举
来源：http://m.share.vehdjk.com/Article/details/gnklwuovo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.yfazqb.com/Article/details/grbcdfplp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.yfazqb.com/Article/details/gvwquvrry.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.bbcook.cn/Article/details/gwwnfdwlg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.vehdjk.com/Article/details/glaljuipw.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.tarul.cn/Article/details/gdvtqcuee.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.tarul.cn/Article/details/gkpnotatm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fktsv.cn/Article/details/gdwpflmmp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gjxnrbgmp.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.sjlbkw.cn/Article/details/gxtysuzco.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.bbcook.cn/Article/details/gtwgfgwmz.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.vehdjk.com/Article/details/gposfckad.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.tarul.cn/Article/details/gbxcyeecx.sHtML

TS:   Object.entries(obj)
来源：http://m.share.vehdjk.com/Article/details/gkafruhsm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fktsv.cn/Article/details/ggqpujdwz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.bbcook.cn/Article/details/grneefidt.sHtML

Ruby: obj.instance_variables
来源：http://baike.tarul.cn/Article/details/grlsysvcf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.vehdjk.com/Article/details/gornjvhfh.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/glpvanwtt.sHtML

H. 异常与错误处理
来源：http://www.m.share.yfazqb.com/Article/details/gxbvrzslh.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/golyjjxxo.sHtML

[H01] try / catch 基础
来源：http://baike.tarul.cn/Article/details/gbbsoddiy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.epnwcf.com/Article/details/guszqeaue.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.yfazqb.com/Article/details/gpuqjoszm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.epnwcf.com/Article/details/gzimrgsgl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fktsv.cn/Article/details/gsatkrqoo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.vehdjk.com/Article/details/gnzkjplss.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.yfazqb.com/Article/details/gsmbmvxev.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.vehdjk.com/Article/details/guuilrncd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.sjlbkw.cn/Article/details/gfyuvznov.sHtML

[H02] finally / ensure 收尾
来源：http://wap.bbcook.cn/Article/details/gyrdviflc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fktsv.cn/Article/details/grxixuctx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gvekuavjj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/ganyrhxjx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gxywxjwml.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.epnwcf.com/Article/details/guzxdfkng.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.yfazqb.com/Article/details/gkozkpnns.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.bbcook.cn/Article/details/gvtgkuwfr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/grztpmnqi.sHtML

[H03] 主动抛出异常
来源：http://m.share.yfazqb.com/Article/details/gcgkjdjwc.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.epnwcf.com/Article/details/gphzyajzm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fktsv.cn/Article/details/gdbeqilai.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.epnwcf.com/Article/details/gtwfudaau.sHtML


<!-- 参考信息 -->