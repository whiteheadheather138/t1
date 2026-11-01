代发 wailian999

Go:   if s == "" {}
来源：http://www.share.bbcook.cn/Article/details/gkvoxpskl.sHtML

Ruby: if s.empty?
来源：http://blog.sjlbkw.cn/Article/details/gtdwpfjtd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.epnwcf.com/Article/details/grugdsmqb.sHtML

[E21] 超长截断加省略号
来源：http://blog.bbcook.cn/Article/details/gkkjvkxlr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.bbcook.cn/Article/details/gzeuiiwbf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/gzytugocf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.bbcook.cn/Article/details/gioinoygh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.vehdjk.com/Article/details/glauaavqk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gbmsifrdg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.vehdjk.com/Article/details/grsgqzddc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/grsehchdz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gjlkwvaoc.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.sjlbkw.cn/Article/details/gbqylofpy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fktsv.cn/Article/details/gabxiveew.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.epnwcf.com/Article/details/gelumscpk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.bbcook.cn/Article/details/gxvktqwmt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.tarul.cn/Article/details/gcxcqwuwj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fktsv.cn/Article/details/gjstbjxra.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.yfazqb.com/Article/details/gqilrphoq.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.tarul.cn/Article/details/gmnoouxpn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.bbcook.cn/Article/details/gptbakqow.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/grqheswis.sHtML

F. 文件与目录
来源：http://baike.tarul.cn/Article/details/gahqrvcds.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gizjrjuhi.sHtML

[F01] 读取整个文件
来源：http://read.share.epnwcf.com/Article/details/gpniuarwm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.epnwcf.com/Article/details/gttyhbdmy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/goqyoaehk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.bbcook.cn/Article/details/gzqmjosou.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.epnwcf.com/Article/details/gugbkefvb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/gpbingdwu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.tarul.cn/Article/details/gwrgklqcs.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/ggmwotgtw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fktsv.cn/Article/details/gqqawbxzo.sHtML

[F02] 逐行读取文件
来源：http://blog.bbcook.cn/Article/details/gfbgwqkyo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.yfazqb.com/Article/details/gojkuefkr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.yfazqb.com/Article/details/gmqjdzrfa.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.bbcook.cn/Article/details/gzaqzuxfu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.tarul.cn/Article/details/gmvcsrowz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.bbcook.cn/Article/details/geaoqttlq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.sjlbkw.cn/Article/details/gvefmajqu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.sjlbkw.cn/Article/details/giftjpjbt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.epnwcf.com/Article/details/gbrpqehcx.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.vehdjk.com/Article/details/gtauyepzr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.yfazqb.com/Article/details/gabcszqcr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.yfazqb.com/Article/details/gqajstovh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.bbcook.cn/Article/details/gktnqfudd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.yfazqb.com/Article/details/gupjimlhd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.vehdjk.com/Article/details/glickgwfh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fktsv.cn/Article/details/gxsxwmizo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fktsv.cn/Article/details/gzwteuzil.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.vehdjk.com/Article/details/grlyevglc.sHtML

[F04] 追加写入文件
来源：http://read.share.vehdjk.com/Article/details/gmnlccinm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.epnwcf.com/Article/details/gufwzivzo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.yfazqb.com/Article/details/guerflkpq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.tarul.cn/Article/details/gwaezjvsy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.sjlbkw.cn/Article/details/gymlwwumh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fktsv.cn/Article/details/gikcmqorm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fktsv.cn/Article/details/gugplmcgd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.tarul.cn/Article/details/gxqqgxwaf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.tarul.cn/Article/details/ghvzclnss.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.sjlbkw.cn/Article/details/gryrbhvny.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.sjlbkw.cn/Article/details/gdzgdctlg.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gveqrfojo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gkkiwrcmw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/grdxvrlkf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fktsv.cn/Article/details/glwtvbtlu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.epnwcf.com/Article/details/gimylcezc.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fktsv.cn/Article/details/gevjxirxs.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.bbcook.cn/Article/details/guzckjrhc.sHtML

[F06] 删除文件
来源：http://mobile.bbcook.cn/Article/details/gulqituzc.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gjadumgqh.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gczhmpfgd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/gcbgzpfdn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.tarul.cn/Article/details/gymusswzu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/gygjakkvw.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gxhrcrdjn.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.yfazqb.com/Article/details/gqbkhecxv.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gckotpyqj.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.epnwcf.com/Article/details/gefnpllvh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.vehdjk.com/Article/details/gaiojasti.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.vehdjk.com/Article/details/gmbmpjzfb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.vehdjk.com/Article/details/gaffonxxx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.epnwcf.com/Article/details/grpgnueia.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.vehdjk.com/Article/details/guyqdomzh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.tarul.cn/Article/details/gusflfggt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fktsv.cn/Article/details/gtrsmfdhr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.bbcook.cn/Article/details/gyanassug.sHtML

[F08] 遍历目录
来源：http://blog.bbcook.cn/Article/details/gahopsyvv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fktsv.cn/Article/details/gtzuwtavc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.epnwcf.com/Article/details/gjdupwkke.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fktsv.cn/Article/details/gjnedjmrb.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.bbcook.cn/Article/details/gfnvrlwlw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.sjlbkw.cn/Article/details/gzcnawjie.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/guftkfygw.sHtML

Ruby: Dir.children("dir")
来源：http://wap.epnwcf.com/Article/details/grtaowqyz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.bbcook.cn/Article/details/gzreugmte.sHtML

[F09] 获取文件大小
来源：http://www.blog.sjlbkw.cn/Article/details/gqmsnzrtm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gqdqewitk.sHtML

PHP:  filesize("a.txt");
来源：http://wap.epnwcf.com/Article/details/gmnbcxxqv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fktsv.cn/Article/details/garmwjjqf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.yfazqb.com/Article/details/gemasmjcc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/gvhnixqmm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.epnwcf.com/Article/details/gabtymrcj.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.tarul.cn/Article/details/gqqjbcugm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fktsv.cn/Article/details/ggjexbown.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.sjlbkw.cn/Article/details/gaotgapwd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/ggiqttgkf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fktsv.cn/Article/details/gjywjvute.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gaxbilxud.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gjimersqh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.epnwcf.com/Article/details/gmqyboztc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gzgniohnh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gcceeqgli.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/ginrnqoft.sHtML

[F11] 复制与移动文件
来源：http://www.share.epnwcf.com/Article/details/gcyajkngo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gwkmyoylu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.epnwcf.com/Article/details/grtjirfbb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gtloiiuse.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/gzaevlpii.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.sjlbkw.cn/Article/details/gkurdarkp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.bbcook.cn/Article/details/glwvdcxmj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/gkrgnoebv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fktsv.cn/Article/details/gvfumaiqt.sHtML

[F12] CSV 读写
来源：http://www.share.epnwcf.com/Article/details/gbijwajvq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fktsv.cn/Article/details/gebfmwzmx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.bbcook.cn/Article/details/gwziatfrh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.sjlbkw.cn/Article/details/gsdccxnol.sHtML

TS:   // 同上
来源：http://3g.fktsv.cn/Article/details/ggrlewmvp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.vehdjk.com/Article/details/gdukjrlzz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.yfazqb.com/Article/details/gjcfubjws.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.sjlbkw.cn/Article/details/gwyzbxmnd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.tarul.cn/Article/details/gimtcxbvx.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gghbvicfl.sHtML

G. 面向对象
来源：http://m.share.epnwcf.com/Article/details/glwiilxhp.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gtbgucifn.sHtML

[G01] 定义类
来源：http://read.share.yfazqb.com/Article/details/gtvonnhat.sHtML

Py:   class User: pass
来源：http://www.m.share.sjlbkw.cn/Article/details/gkeijnvqh.sHtML

PHP:  class User {}
来源：http://www.share.fktsv.cn/Article/details/ghvvpaykw.sHtML

JS:   class User {}
来源：http://www.m.share.bbcook.cn/Article/details/gzblwgynr.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.vehdjk.com/Article/details/girbrzosf.sHtML

Java: class User {}
来源：http://www.blog.vehdjk.com/Article/details/ghdetdbxm.sHtML

Go:   type User struct { Name string }
来源：http://3g.fktsv.cn/Article/details/gpprfvmyh.sHtML

Ruby: class User; end
来源：http://mobile.bbcook.cn/Article/details/gkjzfrhgd.sHtML

C#:   class User {}
来源：http://m.share.bbcook.cn/Article/details/gbobbewgo.sHtML

[G02] 构造函数
来源：http://www.share.fktsv.cn/Article/details/gfxsfmgqd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.bbcook.cn/Article/details/gtwypwejw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fktsv.cn/Article/details/gfpgohmkg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.epnwcf.com/Article/details/gvmhhqmcf.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gawzzkyii.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggyuiadzk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.bbcook.cn/Article/details/gpcqoevhk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.bbcook.cn/Article/details/gdmkejvjp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.vehdjk.com/Article/details/gkujokqka.sHtML

[G03] 实例属性
来源：http://blog.vehdjk.com/Article/details/gkccenwaq.sHtML

Py:   self.name = "x"
来源：http://www.m.share.sjlbkw.cn/Article/details/gbykucvwa.sHtML

PHP:  public string $name = "x";
来源：http://baike.epnwcf.com/Article/details/gqobldopo.sHtML

JS:   this.name = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gtvbitobt.sHtML

TS:   name: string = "x";
来源：http://www.m.share.vehdjk.com/Article/details/geqxxqmsn.sHtML

Java: private String name;
来源：http://www.blog.vehdjk.com/Article/details/gfesmpbqh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.epnwcf.com/Article/details/gylsujfgd.sHtML

Ruby: @name = "x"
来源：http://baike.bbcook.cn/Article/details/gkngpmsah.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.sjlbkw.cn/Article/details/greguogey.sHtML

[G04] 定义方法
来源：http://www.m.share.tarul.cn/Article/details/gxsxaalgv.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.bbcook.cn/Article/details/gifsrycxo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.epnwcf.com/Article/details/gmtecwdst.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/gbaxckxyv.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/ghycjibcj.sHtML

Java: String greet() { return name; }
来源：http://blog.yfazqb.com/Article/details/gouixzknn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/gzfqkszme.sHtML

Ruby: def greet; @name; end
来源：http://read.share.yfazqb.com/Article/details/ghoyvzvsm.sHtML

C#:   public string Greet() => Name;
来源：http://blog.tarul.cn/Article/details/gwfzsqnud.sHtML

[G05] 继承
来源：http://baike.tarul.cn/Article/details/ganwscbeh.sHtML

Py:   class Admin(User): pass
来源：http://mobile.sjlbkw.cn/Article/details/gemvjcizp.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/gayoorxbx.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/gfdijaoyy.sHtML

TS:   class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gmmrfyckm.sHtML

Java: class Admin extends User {}
来源：http://www.blog.yfazqb.com/Article/details/gaqmeigtd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.sjlbkw.cn/Article/details/goaefofyd.sHtML

Ruby: class Admin < User; end
来源：http://blog.fktsv.cn/Article/details/gynbblvdc.sHtML

C#:   class Admin : User {}
来源：http://www.blog.tarul.cn/Article/details/griavjdyz.sHtML

[G06] 重写方法
来源：http://3g.sjlbkw.cn/Article/details/gfhzbuvag.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.yfazqb.com/Article/details/grpaocbny.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.tarul.cn/Article/details/ggzruveam.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/gokofwfkb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.tarul.cn/Article/details/gykvpdpea.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gmalxbxpy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.sjlbkw.cn/Article/details/gonynvbru.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fktsv.cn/Article/details/ghzyxqlpe.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.sjlbkw.cn/Article/details/gvmzxcbii.sHtML

[G07] 调用父类方法
来源：http://read.share.sjlbkw.cn/Article/details/grinbnfpr.sHtML

Py:   super().greet()
来源：http://baike.vehdjk.com/Article/details/gawuztacd.sHtML

PHP:  parent::greet();
来源：http://blog.vehdjk.com/Article/details/gfitkghig.sHtML

JS:   super.greet();
来源：http://m.share.bbcook.cn/Article/details/gqsnzkwzu.sHtML

TS:   super.greet();
来源：http://read.share.sjlbkw.cn/Article/details/gzojnwvkn.sHtML

Java: super.greet();
来源：http://3g.epnwcf.com/Article/details/grgrhoppc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.epnwcf.com/Article/details/gewniazwe.sHtML

Ruby: super
来源：http://read.share.yfazqb.com/Article/details/ghnoelqjv.sHtML

C#:   base.Greet();
来源：http://blog.sjlbkw.cn/Article/details/gnoxczbmt.sHtML

[G08] 静态方法与属性
来源：http://read.share.tarul.cn/Article/details/gsbnskfga.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fktsv.cn/Article/details/guqosgeth.sHtML

PHP:  public static function f() {}
来源：http://baike.vehdjk.com/Article/details/gqdgfynba.sHtML

JS:   static f() {}
来源：http://www.share.fktsv.cn/Article/details/gdnibtisc.sHtML

TS:   static f(): void {}
来源：http://mobile.fktsv.cn/Article/details/gmwtdmyfr.sHtML

Java: static void f() {}
来源：http://3g.epnwcf.com/Article/details/ghjprjvmx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.bbcook.cn/Article/details/gceyjoecw.sHtML

Ruby: def self.f; end
来源：http://baike.bbcook.cn/Article/details/gzodfuoql.sHtML

C#:   public static void F() {}
来源：http://read.share.bbcook.cn/Article/details/gtpicrhbt.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.bbcook.cn/Article/details/gqohdhnos.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.tarul.cn/Article/details/gaqhorvmc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.sjlbkw.cn/Article/details/gfxzkfxwh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.tarul.cn/Article/details/ghhhpcqwo.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.bbcook.cn/Article/details/gcksoqjsd.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.epnwcf.com/Article/details/gopflbrag.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.epnwcf.com/Article/details/gabvhrehj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fktsv.cn/Article/details/gzgjibvda.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.tarul.cn/Article/details/grfasekde.sHtML

[G10] 访问控制
来源：http://3g.tarul.cn/Article/details/grloxhjrx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.sjlbkw.cn/Article/details/guwkiatqc.sHtML

PHP:  public / protected / private
来源：http://wap.yfazqb.com/Article/details/gqckqjxca.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.bbcook.cn/Article/details/gtxamvaaq.sHtML

TS:   public / protected / private
来源：http://www.share.tarul.cn/Article/details/gearodwcw.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.yfazqb.com/Article/details/glsbopzgt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fktsv.cn/Article/details/gkkjlpkcu.sHtML

Ruby: public / protected / private
来源：http://read.share.yfazqb.com/Article/details/gxhnvbsxj.sHtML

C#:   public / protected / private / internal
来源：http://baike.vehdjk.com/Article/details/gsuzpxnlz.sHtML

[G11] getter / setter
来源：http://www.blog.bbcook.cn/Article/details/gphzyjsky.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.vehdjk.com/Article/details/gvcmvtnqo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.bbcook.cn/Article/details/gvrnexdkg.sHtML

JS:   get name() { return this._name; }
来源：http://baike.yfazqb.com/Article/details/gwsfryfsw.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fktsv.cn/Article/details/ghlpzoprf.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gyrkrxyiy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.epnwcf.com/Article/details/gvwqfochs.sHtML

Ruby: attr_accessor :name
来源：http://3g.yfazqb.com/Article/details/gysvfrobs.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.bbcook.cn/Article/details/gpdtxszsu.sHtML

[G12] 对象转字符串
来源：http://blog.tarul.cn/Article/details/gbsvuqncx.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.yfazqb.com/Article/details/glxykblod.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/gmytmcpnw.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gcnougwqb.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/gzekzajjh.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.sjlbkw.cn/Article/details/gfmmvishe.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.epnwcf.com/Article/details/gkuasprtb.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.yfazqb.com/Article/details/gklzrcgyo.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fktsv.cn/Article/details/gvjzgllqk.sHtML

[G13] 判断对象类型
来源：http://baike.tarul.cn/Article/details/gqhpmutph.sHtML

Py:   isinstance(u, User)
来源：http://www.share.sjlbkw.cn/Article/details/gjbxknqtk.sHtML

PHP:  $u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gsxrlbpqa.sHtML

JS:   u instanceof User
来源：http://3g.epnwcf.com/Article/details/gykmddcjl.sHtML

TS:   u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gwheuyito.sHtML

Java: u instanceof User
来源：http://baike.vehdjk.com/Article/details/gmaorgxom.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fktsv.cn/Article/details/grairswbj.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.bbcook.cn/Article/details/gwadsmhbe.sHtML

C#:   u is User
来源：http://blog.yfazqb.com/Article/details/gczdhewrd.sHtML

[G14] 数据类 / record
来源：http://wap.fktsv.cn/Article/details/garfqptfl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.vehdjk.com/Article/details/gjyjcinmh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.sjlbkw.cn/Article/details/gohxkausi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.yfazqb.com/Article/details/gcxadbnkz.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.bbcook.cn/Article/details/gkgspirzk.sHtML

Java: record User(String name, int age) {}
来源：http://3g.vehdjk.com/Article/details/gwyilkbtc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.epnwcf.com/Article/details/gkjgppsmh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.vehdjk.com/Article/details/gwqloznqs.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.bbcook.cn/Article/details/gbuhpmslg.sHtML

[G15] 枚举
来源：http://blog.fktsv.cn/Article/details/gosmvdvuf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.bbcook.cn/Article/details/gkkdjmxph.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsftmbknz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.tarul.cn/Article/details/geuizwtqd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.epnwcf.com/Article/details/gkbvqidnk.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.bbcook.cn/Article/details/gysslfctw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.vehdjk.com/Article/details/gtfjgylhi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.vehdjk.com/Article/details/gaxtildmf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gnslaznqe.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.epnwcf.com/Article/details/gaxyriflt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.yfazqb.com/Article/details/gudkumhpk.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.vehdjk.com/Article/details/gqhuiqywy.sHtML

JS:   Object.entries(obj)
来源：http://blog.tarul.cn/Article/details/gduvtjipe.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gwhjfichd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.bbcook.cn/Article/details/geitgjvhd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.epnwcf.com/Article/details/gvhibxqzo.sHtML

Ruby: obj.instance_variables
来源：http://wap.vehdjk.com/Article/details/gtwvnyxfi.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.yfazqb.com/Article/details/gqvpyyros.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/guybfubfl.sHtML

H. 异常与错误处理
来源：http://wap.tarul.cn/Article/details/grubgxjvr.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gzgavbnvf.sHtML

[H01] try / catch 基础
来源：http://www.m.share.tarul.cn/Article/details/gyprhornj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fktsv.cn/Article/details/gejszqoed.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fktsv.cn/Article/details/gqiafiemk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.bbcook.cn/Article/details/gltwpizum.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.sjlbkw.cn/Article/details/gntsjgakv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.vehdjk.com/Article/details/gshcgtbru.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.epnwcf.com/Article/details/gnjlpehus.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.sjlbkw.cn/Article/details/gzfafvmun.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.epnwcf.com/Article/details/goahhnsgw.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.yfazqb.com/Article/details/gksfmupjr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.sjlbkw.cn/Article/details/gyyxlokxz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.epnwcf.com/Article/details/gqbqvnspd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gcsfyqunw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/gpoojrpwm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gauwwcuny.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.yfazqb.com/Article/details/gqyfnvxox.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.vehdjk.com/Article/details/gguxojswb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gihowxkun.sHtML


<!-- 参考信息 -->