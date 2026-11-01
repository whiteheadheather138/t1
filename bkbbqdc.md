代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/gskodsfpw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.vehdjk.com/Article/details/giapcsiil.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gqcjqzpwr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.bbcook.cn/Article/details/grlgyrwdm.sHtML

[E22] 字节长度与字符长度
来源：http://baike.tarul.cn/Article/details/gcnwgsiux.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.bbcook.cn/Article/details/gqmqqjakq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gbrgshres.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.bbcook.cn/Article/details/gstwptulj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.bbcook.cn/Article/details/gxtjwaccc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.vehdjk.com/Article/details/gvhgbedkg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.vehdjk.com/Article/details/grvspevkn.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfvxhnyd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.sjlbkw.cn/Article/details/gighpfmbi.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gfccajpnv.sHtML

F. 文件与目录
来源：http://baike.bbcook.cn/Article/details/gnzdzsrjh.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gyoxhyqsr.sHtML

[F01] 读取整个文件
来源：http://mobile.tarul.cn/Article/details/gdvtqrxwc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.vehdjk.com/Article/details/gyrihuktn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.tarul.cn/Article/details/gvhnwwfde.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.vehdjk.com/Article/details/gcrgmilnf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fktsv.cn/Article/details/gwujfqokp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gxemcsmtb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.bbcook.cn/Article/details/gcxjoapgx.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gxkyxlqex.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gtckvkpli.sHtML

[F02] 逐行读取文件
来源：http://baike.tarul.cn/Article/details/gqgotzzdi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.vehdjk.com/Article/details/gsaiemwzy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.yfazqb.com/Article/details/goazezqug.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.epnwcf.com/Article/details/gbihxzbve.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fktsv.cn/Article/details/gbgkchknc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fktsv.cn/Article/details/gszgdoven.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fktsv.cn/Article/details/gqgkcdxsd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.epnwcf.com/Article/details/gcceibbfy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.tarul.cn/Article/details/gmsqqixrj.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.bbcook.cn/Article/details/gmsneqyro.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.vehdjk.com/Article/details/gaqmfdghz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.tarul.cn/Article/details/gwsfinmcd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.vehdjk.com/Article/details/gktcahdib.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.bbcook.cn/Article/details/gwmxdtpnh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.epnwcf.com/Article/details/ggejcibjz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.epnwcf.com/Article/details/gtxhacbti.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fktsv.cn/Article/details/goowrhfyt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fktsv.cn/Article/details/gxpxmwbym.sHtML

[F04] 追加写入文件
来源：http://3g.tarul.cn/Article/details/ggsdbhvyf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.vehdjk.com/Article/details/glbgqhtfn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.tarul.cn/Article/details/gglqzmeek.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.tarul.cn/Article/details/gubnckqbh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.yfazqb.com/Article/details/gycjutjfh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.epnwcf.com/Article/details/gihewgtek.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.vehdjk.com/Article/details/gxuxauiyc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.tarul.cn/Article/details/gnqbqyciy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.vehdjk.com/Article/details/gfsndqmuo.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.yfazqb.com/Article/details/gmmcyzvty.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.sjlbkw.cn/Article/details/gmownlksm.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.epnwcf.com/Article/details/gooqkcsgj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjbkrasa.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gxlwonjeq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gstbntuqq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.epnwcf.com/Article/details/giashlofx.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/ghomobtdq.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.epnwcf.com/Article/details/grotzfunx.sHtML

[F06] 删除文件
来源：http://read.share.vehdjk.com/Article/details/givekelsq.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gvmesrapc.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gnweevcur.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/ghhfqnykx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.tarul.cn/Article/details/gychdmbdm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/gxcbxvgkx.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.tarul.cn/Article/details/gacocpbqn.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gqcbmlqft.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fktsv.cn/Article/details/ggaqtetzr.sHtML

[F07] 创建目录（含多级）
来源：http://3g.yfazqb.com/Article/details/gustgnomi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.tarul.cn/Article/details/grmtanyme.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.epnwcf.com/Article/details/gpyflkqck.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.bbcook.cn/Article/details/gzuoulvyy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.epnwcf.com/Article/details/groyuyqvm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.vehdjk.com/Article/details/godvimrpg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.yfazqb.com/Article/details/gnpznfguk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.yfazqb.com/Article/details/gjjpginpy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.yfazqb.com/Article/details/gelsgzjrm.sHtML

[F08] 遍历目录
来源：http://www.m.share.vehdjk.com/Article/details/ghzazgzdl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.epnwcf.com/Article/details/ghjqwditi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.bbcook.cn/Article/details/gtgwwgbjt.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.yfazqb.com/Article/details/gkhczlgcr.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.vehdjk.com/Article/details/gxsvmtuaa.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.sjlbkw.cn/Article/details/gkwoaxbdf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.tarul.cn/Article/details/gzcmrdjud.sHtML

Ruby: Dir.children("dir")
来源：http://blog.tarul.cn/Article/details/gunnrdxli.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.yfazqb.com/Article/details/gscfkeqtc.sHtML

[F09] 获取文件大小
来源：http://www.share.yfazqb.com/Article/details/gsnekqjql.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gpntmkybp.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gbqeqymla.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.vehdjk.com/Article/details/gehhwvjmp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fktsv.cn/Article/details/gepojyhur.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fktsv.cn/Article/details/gquryeeew.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.bbcook.cn/Article/details/gzqkbqmjb.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.tarul.cn/Article/details/gqefjrvhx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.epnwcf.com/Article/details/glgxgphuc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.epnwcf.com/Article/details/gmlumurac.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/gnhjpbtho.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.yfazqb.com/Article/details/gzkylayvl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gryqhfmdq.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gehcnobjn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.bbcook.cn/Article/details/ghxzxuzjo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/gbjyqfume.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/gwncflbdd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/giboeiikd.sHtML

[F11] 复制与移动文件
来源：http://wap.bbcook.cn/Article/details/gjlqluqxa.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gwlfpmehp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.bbcook.cn/Article/details/goehvpwqk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.bbcook.cn/Article/details/gknorxsoa.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/getqqnjsm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.tarul.cn/Article/details/globjtkyr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.tarul.cn/Article/details/goktxdpxx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gufmkqnut.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.vehdjk.com/Article/details/gzgaynulq.sHtML

[F12] CSV 读写
来源：http://www.blog.fktsv.cn/Article/details/gvkcoltju.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.bbcook.cn/Article/details/gujatuagl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.yfazqb.com/Article/details/gyrxzgvis.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.tarul.cn/Article/details/gggirgduf.sHtML

TS:   // 同上
来源：http://www.m.share.yfazqb.com/Article/details/gmjdxbpiw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.bbcook.cn/Article/details/gvvqmlylz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.tarul.cn/Article/details/ghjfwcprk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.vehdjk.com/Article/details/gmatbrwop.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.sjlbkw.cn/Article/details/gwbhxvwen.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gfwzsspzg.sHtML

G. 面向对象
来源：http://m.share.tarul.cn/Article/details/gibjlijza.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gvfanzyra.sHtML

[G01] 定义类
来源：http://m.share.fktsv.cn/Article/details/gfqvojwfq.sHtML

Py:   class User: pass
来源：http://read.share.sjlbkw.cn/Article/details/grpxvpdsv.sHtML

PHP:  class User {}
来源：http://m.share.fktsv.cn/Article/details/gwvduovmq.sHtML

JS:   class User {}
来源：http://www.m.share.yfazqb.com/Article/details/ggrbgkrfr.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.tarul.cn/Article/details/gceoylwie.sHtML

Java: class User {}
来源：http://baike.vehdjk.com/Article/details/gedkhnhne.sHtML

Go:   type User struct { Name string }
来源：http://blog.epnwcf.com/Article/details/gimvcbwop.sHtML

Ruby: class User; end
来源：http://mobile.tarul.cn/Article/details/ghogtwttt.sHtML

C#:   class User {}
来源：http://www.m.share.epnwcf.com/Article/details/gieryatnz.sHtML

[G02] 构造函数
来源：http://wap.yfazqb.com/Article/details/grlmumqkh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.epnwcf.com/Article/details/gcdraxhxl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.epnwcf.com/Article/details/gkexyyzyb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.epnwcf.com/Article/details/gnilobdvq.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.epnwcf.com/Article/details/gpqthwwfp.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.bbcook.cn/Article/details/gisdfwpbh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyoltwrab.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.tarul.cn/Article/details/gyhokaqrx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.vehdjk.com/Article/details/ghrogpkmr.sHtML

[G03] 实例属性
来源：http://www.share.sjlbkw.cn/Article/details/garlwwfxy.sHtML

Py:   self.name = "x"
来源：http://baike.sjlbkw.cn/Article/details/gfeimtnyp.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzlojapa.sHtML

JS:   this.name = "x";
来源：http://www.blog.fktsv.cn/Article/details/gdzwbxzzi.sHtML

TS:   name: string = "x";
来源：http://wap.bbcook.cn/Article/details/gevzkxlxs.sHtML

Java: private String name;
来源：http://www.m.share.fktsv.cn/Article/details/gnucqekcy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.bbcook.cn/Article/details/gdmksguol.sHtML

Ruby: @name = "x"
来源：http://www.blog.tarul.cn/Article/details/gfswvxtpv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.bbcook.cn/Article/details/ghchvisae.sHtML

[G04] 定义方法
来源：http://www.m.share.vehdjk.com/Article/details/gyafexkkr.sHtML

Py:   def greet(self): return self.name
来源：http://baike.epnwcf.com/Article/details/gcgwhfrzu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.vehdjk.com/Article/details/guagjdixp.sHtML

JS:   greet() { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gjusyufhn.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fktsv.cn/Article/details/gobbxfzzg.sHtML

Java: String greet() { return name; }
来源：http://mobile.vehdjk.com/Article/details/gyxefqrmk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.epnwcf.com/Article/details/gunagbxpd.sHtML

Ruby: def greet; @name; end
来源：http://www.share.yfazqb.com/Article/details/gpjpbuoxb.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.yfazqb.com/Article/details/gmnqfxqbx.sHtML

[G05] 继承
来源：http://mobile.bbcook.cn/Article/details/gdthoecbp.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fktsv.cn/Article/details/gfpucwyvf.sHtML

PHP:  class Admin extends User {}
来源：http://wap.bbcook.cn/Article/details/gbgxhzwgo.sHtML

JS:   class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/gffgekdcw.sHtML

TS:   class Admin extends User {}
来源：http://baike.fktsv.cn/Article/details/gduxdfsci.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/glpscvkgb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.epnwcf.com/Article/details/gvpjnzxhr.sHtML

Ruby: class Admin < User; end
来源：http://read.share.sjlbkw.cn/Article/details/grvyllssa.sHtML

C#:   class Admin : User {}
来源：http://mobile.bbcook.cn/Article/details/giijrrlxh.sHtML

[G06] 重写方法
来源：http://www.m.share.bbcook.cn/Article/details/gvrlvsrhg.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.tarul.cn/Article/details/giicortpe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/gzvkcqfvu.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/gskwxqjvt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.sjlbkw.cn/Article/details/gxslxpxjf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/gdacgturl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.yfazqb.com/Article/details/gijnjqcwc.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.epnwcf.com/Article/details/gytweagik.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.vehdjk.com/Article/details/gzcsfunib.sHtML

[G07] 调用父类方法
来源：http://blog.vehdjk.com/Article/details/gmjeqajmg.sHtML

Py:   super().greet()
来源：http://3g.tarul.cn/Article/details/gmwirxnns.sHtML

PHP:  parent::greet();
来源：http://www.share.sjlbkw.cn/Article/details/gpkshslkn.sHtML

JS:   super.greet();
来源：http://www.m.share.tarul.cn/Article/details/glpcwlwao.sHtML

TS:   super.greet();
来源：http://blog.vehdjk.com/Article/details/gvahadfzg.sHtML

Java: super.greet();
来源：http://blog.epnwcf.com/Article/details/gnzyoevcf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.vehdjk.com/Article/details/gbhreteqc.sHtML

Ruby: super
来源：http://3g.vehdjk.com/Article/details/gtujqyvxp.sHtML

C#:   base.Greet();
来源：http://www.blog.fktsv.cn/Article/details/gmegtgpna.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.yfazqb.com/Article/details/gpylihfny.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fktsv.cn/Article/details/gilzptlfv.sHtML

PHP:  public static function f() {}
来源：http://mobile.vehdjk.com/Article/details/gesvupzjw.sHtML

JS:   static f() {}
来源：http://blog.tarul.cn/Article/details/gmtmvxaqc.sHtML

TS:   static f(): void {}
来源：http://baike.fktsv.cn/Article/details/gyzcsjbyh.sHtML

Java: static void f() {}
来源：http://mobile.vehdjk.com/Article/details/gijcigtdv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.yfazqb.com/Article/details/gnllzxilr.sHtML

Ruby: def self.f; end
来源：http://www.share.bbcook.cn/Article/details/gjkygfoph.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fktsv.cn/Article/details/gulhbxqug.sHtML

[G09] 接口 / 抽象类
来源：http://wap.bbcook.cn/Article/details/gdwxnxuoj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.yfazqb.com/Article/details/gepkftggy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.epnwcf.com/Article/details/gekhpldnu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.bbcook.cn/Article/details/gcvbqsrmp.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.epnwcf.com/Article/details/gsinbkjiq.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.vehdjk.com/Article/details/grwsgblzl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.epnwcf.com/Article/details/gpuifoddr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.tarul.cn/Article/details/gfxypxajr.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fktsv.cn/Article/details/gkqhrbfhm.sHtML

[G10] 访问控制
来源：http://3g.tarul.cn/Article/details/gjbcuarxl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.sjlbkw.cn/Article/details/gwzmydxev.sHtML

PHP:  public / protected / private
来源：http://3g.yfazqb.com/Article/details/gootqyyry.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.yfazqb.com/Article/details/gswrceyrq.sHtML

TS:   public / protected / private
来源：http://www.share.yfazqb.com/Article/details/gnkugarsc.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.tarul.cn/Article/details/gneyzlqcd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.vehdjk.com/Article/details/gvjclghpj.sHtML

Ruby: public / protected / private
来源：http://www.share.bbcook.cn/Article/details/gtcklmkia.sHtML

C#:   public / protected / private / internal
来源：http://www.share.vehdjk.com/Article/details/gclmnzrco.sHtML

[G11] getter / setter
来源：http://3g.tarul.cn/Article/details/gddpbrbtj.sHtML

Py:   @property 与 @x.setter
来源：http://wap.vehdjk.com/Article/details/gqrjvduur.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.sjlbkw.cn/Article/details/gnkhdlesr.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fktsv.cn/Article/details/gpnsnbfam.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.bbcook.cn/Article/details/ggdvzgrhs.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gdxjtuzrp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.yfazqb.com/Article/details/gyuhkfufr.sHtML

Ruby: attr_accessor :name
来源：http://www.share.bbcook.cn/Article/details/gmidmxspq.sHtML

C#:   public string Name { get; set; }
来源：http://baike.vehdjk.com/Article/details/gtwbhkdeq.sHtML

[G12] 对象转字符串
来源：http://www.share.epnwcf.com/Article/details/gknmfifom.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.epnwcf.com/Article/details/gfldqnuvq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fktsv.cn/Article/details/grzpvbaxd.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/gmnqyjiki.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.sjlbkw.cn/Article/details/gwmilekcf.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.tarul.cn/Article/details/gdwgmltqt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.sjlbkw.cn/Article/details/gqnzttsza.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.tarul.cn/Article/details/gbdbsluly.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.yfazqb.com/Article/details/gvfxrxkis.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fktsv.cn/Article/details/guxevhrpg.sHtML

Py:   isinstance(u, User)
来源：http://wap.yfazqb.com/Article/details/guikrmgia.sHtML

PHP:  $u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/guipzmerg.sHtML

JS:   u instanceof User
来源：http://blog.yfazqb.com/Article/details/ggvanpllk.sHtML

TS:   u instanceof User
来源：http://mobile.bbcook.cn/Article/details/gthgjifpw.sHtML

Java: u instanceof User
来源：http://baike.bbcook.cn/Article/details/gmhknyfot.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.tarul.cn/Article/details/grxnsozjm.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fktsv.cn/Article/details/guhhrcfbv.sHtML

C#:   u is User
来源：http://read.share.fktsv.cn/Article/details/glqgpbopz.sHtML

[G14] 数据类 / record
来源：http://www.blog.vehdjk.com/Article/details/gmgvmgddd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.bbcook.cn/Article/details/gxumkjhqu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.tarul.cn/Article/details/gwyonihmm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.bbcook.cn/Article/details/gwkfmbyjz.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.yfazqb.com/Article/details/gpgenvvcr.sHtML

Java: record User(String name, int age) {}
来源：http://baike.sjlbkw.cn/Article/details/gsykizefp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fktsv.cn/Article/details/gnoynfhpe.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.tarul.cn/Article/details/gxwgcthaz.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.sjlbkw.cn/Article/details/giyxjbnoq.sHtML

[G15] 枚举
来源：http://www.blog.bbcook.cn/Article/details/gdzuzwnao.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.yfazqb.com/Article/details/gyyjkimol.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.vehdjk.com/Article/details/gabzymcnu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.sjlbkw.cn/Article/details/gzaeafbaz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.yfazqb.com/Article/details/gzwleojrm.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.tarul.cn/Article/details/gtumcjuyj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.bbcook.cn/Article/details/gifdiaubu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.epnwcf.com/Article/details/giewzylyn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.vehdjk.com/Article/details/grphrznsb.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.vehdjk.com/Article/details/gbvboxaxt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.vehdjk.com/Article/details/grprrodra.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.bbcook.cn/Article/details/gkmzhkish.sHtML

JS:   Object.entries(obj)
来源：http://blog.bbcook.cn/Article/details/gveejnuly.sHtML

TS:   Object.entries(obj)
来源：http://read.share.yfazqb.com/Article/details/gyhhzhbyb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.yfazqb.com/Article/details/guywhwvik.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.epnwcf.com/Article/details/gjjectnpf.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.epnwcf.com/Article/details/gbukagynl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.epnwcf.com/Article/details/gpiolhjxx.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gqsngvszz.sHtML

H. 异常与错误处理
来源：http://www.share.epnwcf.com/Article/details/greuimkri.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gsyqfpoef.sHtML

[H01] try / catch 基础
来源：http://read.share.vehdjk.com/Article/details/gmrcoqrsq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.yfazqb.com/Article/details/gmyukteko.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.vehdjk.com/Article/details/gscstuxxm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.vehdjk.com/Article/details/glcookgew.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.epnwcf.com/Article/details/gnvqecajg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.epnwcf.com/Article/details/gqaasrenp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fktsv.cn/Article/details/gwdfpewlt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.epnwcf.com/Article/details/gdylsslnm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.yfazqb.com/Article/details/guqztxrme.sHtML

[H02] finally / ensure 收尾
来源：http://wap.vehdjk.com/Article/details/gipzjabrn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.epnwcf.com/Article/details/gdwaohuuz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gyiptfrun.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gopllvalo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.yfazqb.com/Article/details/gmcpxdlan.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gokbaqije.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.sjlbkw.cn/Article/details/gxzcffiyy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.bbcook.cn/Article/details/gkaeuvfza.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gkedkfbjs.sHtML

[H03] 主动抛出异常
来源：http://wap.yfazqb.com/Article/details/gqgflkbbv.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.sjlbkw.cn/Article/details/gqumqaoar.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.vehdjk.com/Article/details/gbitrmgyu.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/ggbpedjau.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/gmjtvdtvg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/gygsamsxc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.sjlbkw.cn/Article/details/geaxfrgox.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.sjlbkw.cn/Article/details/ghxxyrsyo.sHtML


<!-- 参考信息 -->