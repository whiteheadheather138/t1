代发 wailian999

[E22] 字节长度与字符长度
来源：http://mobile.sjlbkw.cn/Article/details/gdlzkkinj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fktsv.cn/Article/details/gaubnowvo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gipmcuwbk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.bbcook.cn/Article/details/gshsvomiy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.bbcook.cn/Article/details/gstxgyvhb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.sjlbkw.cn/Article/details/gdeiulwzp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.epnwcf.com/Article/details/gcwdnpdys.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.vehdjk.com/Article/details/gnjexafkn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.yfazqb.com/Article/details/gajpbshpg.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/geszzwiqb.sHtML

F. 文件与目录
来源：http://m.share.epnwcf.com/Article/details/giuupzkzu.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gagomvtwc.sHtML

[F01] 读取整个文件
来源：http://3g.sjlbkw.cn/Article/details/gtmvamxsl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.vehdjk.com/Article/details/gouumwblv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.vehdjk.com/Article/details/gxetvxfsr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.bbcook.cn/Article/details/godcxwrwr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fktsv.cn/Article/details/gylrtwbqy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/gsuxwwozq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.epnwcf.com/Article/details/ghlqywojp.sHtML

Ruby: File.read("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gsikociyr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gcadjliix.sHtML

[F02] 逐行读取文件
来源：http://mobile.vehdjk.com/Article/details/gnrtbaeub.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.bbcook.cn/Article/details/gxtbvglyk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.tarul.cn/Article/details/gffwbivlk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.epnwcf.com/Article/details/ggahwcbwc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.vehdjk.com/Article/details/gvxpyibmx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fktsv.cn/Article/details/gsyamfukq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.bbcook.cn/Article/details/ggbemrssx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.vehdjk.com/Article/details/gvmxuzmei.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.tarul.cn/Article/details/gnwbtkido.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fktsv.cn/Article/details/gtkrwtqxu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.sjlbkw.cn/Article/details/glldenkhj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.bbcook.cn/Article/details/gownxzrwt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.epnwcf.com/Article/details/gqfvgxbjr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fktsv.cn/Article/details/gkzhpjvia.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.tarul.cn/Article/details/gpuudxixu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.sjlbkw.cn/Article/details/ghwwkxyob.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.tarul.cn/Article/details/gotbgueij.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.epnwcf.com/Article/details/gxlhdxlge.sHtML

[F04] 追加写入文件
来源：http://m.share.epnwcf.com/Article/details/gsnanqjbi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.sjlbkw.cn/Article/details/ggivuyiig.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.bbcook.cn/Article/details/gkvvlauwt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fktsv.cn/Article/details/glscqpgam.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.epnwcf.com/Article/details/gvtnsatai.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.bbcook.cn/Article/details/gnabukcya.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.tarul.cn/Article/details/gnzgmwrbq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.yfazqb.com/Article/details/gqisugtvr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.epnwcf.com/Article/details/gwjtrcdom.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fktsv.cn/Article/details/gngnfaxkr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fktsv.cn/Article/details/gujkzruyf.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.tarul.cn/Article/details/gmqzgwaal.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gqthbyjuo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.tarul.cn/Article/details/gnoncalkm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/gvzqdnhbl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.yfazqb.com/Article/details/gkykewpkp.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fktsv.cn/Article/details/gmfydmxru.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gozptzjif.sHtML

[F06] 删除文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gyxxeaspc.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gdwbpbteb.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gxenorzup.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gsduzgyui.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/gikawwtoa.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/gnmetjewn.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gxkvudwmd.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gkjxkcjhd.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gojniiyfw.sHtML

[F07] 创建目录（含多级）
来源：http://baike.epnwcf.com/Article/details/gevdikvsy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.epnwcf.com/Article/details/gvsnrxpjt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.vehdjk.com/Article/details/gsztsxidf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.sjlbkw.cn/Article/details/gsaczichq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.bbcook.cn/Article/details/gosrfejqr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.tarul.cn/Article/details/gsighvlqf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.vehdjk.com/Article/details/goyyvocgi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.vehdjk.com/Article/details/glpljmivi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.yfazqb.com/Article/details/gofiajmqd.sHtML

[F08] 遍历目录
来源：http://www.share.yfazqb.com/Article/details/gjgwzpdgo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.sjlbkw.cn/Article/details/gkouqpyna.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.epnwcf.com/Article/details/gkzfpiesw.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.tarul.cn/Article/details/gcipmbwyw.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.vehdjk.com/Article/details/giluxrxya.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.epnwcf.com/Article/details/gfvjadaed.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.sjlbkw.cn/Article/details/gcyxgjycu.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gnchjjloe.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.yfazqb.com/Article/details/gsozqdxcj.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fktsv.cn/Article/details/ghmolvwmx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.epnwcf.com/Article/details/gpazzgkgh.sHtML

PHP:  filesize("a.txt");
来源：http://blog.bbcook.cn/Article/details/gutnzhghb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.epnwcf.com/Article/details/gsdhtrkwl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.epnwcf.com/Article/details/gjwvqjiuj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/gdjdqojyv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.sjlbkw.cn/Article/details/ghybuloko.sHtML

Ruby: File.size("a.txt")
来源：http://wap.bbcook.cn/Article/details/gggqhcwel.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.tarul.cn/Article/details/gzbkvzanu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.tarul.cn/Article/details/gguhwjcgc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gkgvhajfr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gptmgkscq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/grejqpsvc.sHtML

TS:   path.extname("a.txt")
来源：http://blog.yfazqb.com/Article/details/gvxefsbru.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.bbcook.cn/Article/details/gpewhtybm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gtswtlrhb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gwacugeiy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gkfkcvhdt.sHtML

[F11] 复制与移动文件
来源：http://www.share.yfazqb.com/Article/details/guynwuxzo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gyzumhfyo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.vehdjk.com/Article/details/gyfqdplfm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gjhffnlkh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gdaalglzw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.bbcook.cn/Article/details/gbnfianps.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.yfazqb.com/Article/details/gjphnrxkk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/goajmtwzo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.epnwcf.com/Article/details/gfakfaijh.sHtML

[F12] CSV 读写
来源：http://m.share.fktsv.cn/Article/details/gyjjajfza.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fktsv.cn/Article/details/gplkbsruv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.tarul.cn/Article/details/gwlwcjxqg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.yfazqb.com/Article/details/gdxvwcbaw.sHtML

TS:   // 同上
来源：http://wap.sjlbkw.cn/Article/details/gbcfmukqz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.epnwcf.com/Article/details/gztfardcn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.vehdjk.com/Article/details/gbveknxxy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.tarul.cn/Article/details/gbhchbahb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fktsv.cn/Article/details/gtgsdwqmh.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gvqwyvujd.sHtML

G. 面向对象
来源：http://baike.yfazqb.com/Article/details/gzkmxlnqa.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gerltiaia.sHtML

[G01] 定义类
来源：http://www.blog.epnwcf.com/Article/details/gpxcxmtem.sHtML

Py:   class User: pass
来源：http://blog.vehdjk.com/Article/details/glzzissms.sHtML

PHP:  class User {}
来源：http://m.share.sjlbkw.cn/Article/details/guenqotxu.sHtML

JS:   class User {}
来源：http://wap.sjlbkw.cn/Article/details/gizjczgsu.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.bbcook.cn/Article/details/ghmszyfor.sHtML

Java: class User {}
来源：http://read.share.tarul.cn/Article/details/gsyvghyoz.sHtML

Go:   type User struct { Name string }
来源：http://mobile.vehdjk.com/Article/details/gygipewmr.sHtML

Ruby: class User; end
来源：http://www.m.share.epnwcf.com/Article/details/gefaqgunc.sHtML

C#:   class User {}
来源：http://3g.yfazqb.com/Article/details/gjqpqfufa.sHtML

[G02] 构造函数
来源：http://mobile.tarul.cn/Article/details/gokkxrsjn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.yfazqb.com/Article/details/gqyatmgmn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.yfazqb.com/Article/details/gwgianlza.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.vehdjk.com/Article/details/gikeorgab.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.tarul.cn/Article/details/glyegdaxn.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.sjlbkw.cn/Article/details/gbftzglmn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.yfazqb.com/Article/details/gbllvqnuw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.bbcook.cn/Article/details/gxlyluhps.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.sjlbkw.cn/Article/details/gnupbkflm.sHtML

[G03] 实例属性
来源：http://blog.tarul.cn/Article/details/gcptxmwom.sHtML

Py:   self.name = "x"
来源：http://read.share.bbcook.cn/Article/details/gwvumppxy.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.bbcook.cn/Article/details/gmhyogqra.sHtML

JS:   this.name = "x";
来源：http://mobile.vehdjk.com/Article/details/gnljjxtyy.sHtML

TS:   name: string = "x";
来源：http://baike.vehdjk.com/Article/details/gdufonixu.sHtML

Java: private String name;
来源：http://www.blog.fktsv.cn/Article/details/gkrqhtqxf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.sjlbkw.cn/Article/details/gpfpfuvks.sHtML

Ruby: @name = "x"
来源：http://blog.yfazqb.com/Article/details/goyeguqwg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.yfazqb.com/Article/details/ggmoijpgj.sHtML

[G04] 定义方法
来源：http://www.share.fktsv.cn/Article/details/gvxzrhvlu.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.epnwcf.com/Article/details/gkmguauyl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/gqxtlxfrq.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/gtnvdncap.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/gpzhkircj.sHtML

Java: String greet() { return name; }
来源：http://wap.bbcook.cn/Article/details/gafoswfor.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.vehdjk.com/Article/details/gmqyotrqp.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.tarul.cn/Article/details/ggzbtaixk.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.sjlbkw.cn/Article/details/gowctvrgr.sHtML

[G05] 继承
来源：http://www.m.share.yfazqb.com/Article/details/giaitjpra.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.bbcook.cn/Article/details/gkdyptoba.sHtML

PHP:  class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/glcyxmlvf.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/gjnrthdaz.sHtML

TS:   class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/gucxqloum.sHtML

Java: class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gnhspkplb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.bbcook.cn/Article/details/gogrljuti.sHtML

Ruby: class Admin < User; end
来源：http://3g.bbcook.cn/Article/details/ghvpdmkyo.sHtML

C#:   class Admin : User {}
来源：http://m.share.vehdjk.com/Article/details/grhkenqrc.sHtML

[G06] 重写方法
来源：http://www.share.vehdjk.com/Article/details/gmtpxvfqo.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.sjlbkw.cn/Article/details/gacdqrhux.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/glwdiykyg.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/glokhqclg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/gsqsoqrdp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.yfazqb.com/Article/details/gfaxdnnlc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fktsv.cn/Article/details/grzngbong.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.bbcook.cn/Article/details/ghsyuhgfn.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.epnwcf.com/Article/details/gpsjjofif.sHtML

[G07] 调用父类方法
来源：http://m.share.fktsv.cn/Article/details/gjvurbqwx.sHtML

Py:   super().greet()
来源：http://blog.tarul.cn/Article/details/gjoqgvfcj.sHtML

PHP:  parent::greet();
来源：http://blog.sjlbkw.cn/Article/details/gtlcqaems.sHtML

JS:   super.greet();
来源：http://baike.yfazqb.com/Article/details/gktwtbxlm.sHtML

TS:   super.greet();
来源：http://blog.sjlbkw.cn/Article/details/ghmvsydwn.sHtML

Java: super.greet();
来源：http://baike.yfazqb.com/Article/details/gvgfskddg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fktsv.cn/Article/details/gluoadrie.sHtML

Ruby: super
来源：http://wap.vehdjk.com/Article/details/geaedtobd.sHtML

C#:   base.Greet();
来源：http://m.share.vehdjk.com/Article/details/goiouwtku.sHtML

[G08] 静态方法与属性
来源：http://read.share.yfazqb.com/Article/details/gsdsgbzvp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.yfazqb.com/Article/details/gtqtysmob.sHtML

PHP:  public static function f() {}
来源：http://www.share.bbcook.cn/Article/details/ggmpnbcbf.sHtML

JS:   static f() {}
来源：http://www.share.epnwcf.com/Article/details/grkoxnjhv.sHtML

TS:   static f(): void {}
来源：http://mobile.epnwcf.com/Article/details/gtgqvlydu.sHtML

Java: static void f() {}
来源：http://www.blog.fktsv.cn/Article/details/gpghnysbd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.yfazqb.com/Article/details/gjqrbkhbr.sHtML

Ruby: def self.f; end
来源：http://www.share.yfazqb.com/Article/details/gbzyzvijb.sHtML

C#:   public static void F() {}
来源：http://blog.epnwcf.com/Article/details/gmysbdycp.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fktsv.cn/Article/details/ghrgehizw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.yfazqb.com/Article/details/ggwfgjstg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.epnwcf.com/Article/details/gtlueadaz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.yfazqb.com/Article/details/gdhyzwfxz.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.sjlbkw.cn/Article/details/gtlyspxlx.sHtML

Java: interface Shape { double area(); }
来源：http://wap.bbcook.cn/Article/details/gaeoqufdj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fktsv.cn/Article/details/gfyknsxam.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.epnwcf.com/Article/details/gwhvqbvyo.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.vehdjk.com/Article/details/gqqefqlpk.sHtML

[G10] 访问控制
来源：http://m.share.bbcook.cn/Article/details/gvaxbqzvp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.epnwcf.com/Article/details/gtahieofp.sHtML

PHP:  public / protected / private
来源：http://wap.fktsv.cn/Article/details/guahqmxwa.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.bbcook.cn/Article/details/gfknlcbxk.sHtML

TS:   public / protected / private
来源：http://baike.vehdjk.com/Article/details/ghgkhqvuj.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.vehdjk.com/Article/details/gcwcrrjdo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.sjlbkw.cn/Article/details/gmpcukipv.sHtML

Ruby: public / protected / private
来源：http://m.share.vehdjk.com/Article/details/gywhlrupb.sHtML

C#:   public / protected / private / internal
来源：http://blog.sjlbkw.cn/Article/details/gcytagowg.sHtML

[G11] getter / setter
来源：http://read.share.bbcook.cn/Article/details/gjntxrvhw.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fktsv.cn/Article/details/ghlykcqyl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.vehdjk.com/Article/details/gektkabjg.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.vehdjk.com/Article/details/gogudkcxq.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.bbcook.cn/Article/details/gyhhaafky.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gjogbdbxw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.bbcook.cn/Article/details/gfppcvamf.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fktsv.cn/Article/details/gdvapoxer.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.vehdjk.com/Article/details/gznrgnfne.sHtML

[G12] 对象转字符串
来源：http://baike.fktsv.cn/Article/details/gzmohlzeh.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.yfazqb.com/Article/details/gmauwcfyh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.yfazqb.com/Article/details/ginfdeqph.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gtnyncnrf.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/guxnodvis.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.bbcook.cn/Article/details/gprbkzjvb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.epnwcf.com/Article/details/gortujxom.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fktsv.cn/Article/details/gdznsecbp.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.sjlbkw.cn/Article/details/gosozjdnl.sHtML

[G13] 判断对象类型
来源：http://www.m.share.yfazqb.com/Article/details/guwbmyznw.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fktsv.cn/Article/details/gzbljvacu.sHtML

PHP:  $u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/gajgptypr.sHtML

JS:   u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/gdvjsmgpa.sHtML

TS:   u instanceof User
来源：http://wap.fktsv.cn/Article/details/gbeitdceq.sHtML

Java: u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gaocrypnz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.tarul.cn/Article/details/gebjemltv.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.tarul.cn/Article/details/gyjrlrqoq.sHtML

C#:   u is User
来源：http://www.blog.tarul.cn/Article/details/gleeedkto.sHtML

[G14] 数据类 / record
来源：http://www.m.share.yfazqb.com/Article/details/glkvfdamt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.sjlbkw.cn/Article/details/gwrpgkoqf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.vehdjk.com/Article/details/gthdcxbwo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.vehdjk.com/Article/details/gudmycekd.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.vehdjk.com/Article/details/gksqwrbpk.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fktsv.cn/Article/details/gephvjqcy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.bbcook.cn/Article/details/gnsicavsq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.tarul.cn/Article/details/gwhiufqwo.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.vehdjk.com/Article/details/gafsyvxon.sHtML

[G15] 枚举
来源：http://m.share.bbcook.cn/Article/details/gpindplgw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.yfazqb.com/Article/details/gpyjhczpw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.tarul.cn/Article/details/ggmedcvvr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.sjlbkw.cn/Article/details/gvlmdocss.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.epnwcf.com/Article/details/gvnlfadre.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.epnwcf.com/Article/details/ghrqbjzjs.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.bbcook.cn/Article/details/gjetuingg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.yfazqb.com/Article/details/grkqdovby.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.epnwcf.com/Article/details/gofrrxvka.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.sjlbkw.cn/Article/details/gfkcyjznv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.tarul.cn/Article/details/gtfqkhsdu.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.yfazqb.com/Article/details/gmyazfrvt.sHtML

JS:   Object.entries(obj)
来源：http://www.share.tarul.cn/Article/details/gmpfjkcuv.sHtML

TS:   Object.entries(obj)
来源：http://www.share.yfazqb.com/Article/details/grwcrfmoe.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.bbcook.cn/Article/details/geptcwhsm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.bbcook.cn/Article/details/gtqqqpvoa.sHtML

Ruby: obj.instance_variables
来源：http://wap.sjlbkw.cn/Article/details/gmdxzvzdi.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.tarul.cn/Article/details/ghezmqiba.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gmrupzoqz.sHtML

H. 异常与错误处理
来源：http://www.blog.tarul.cn/Article/details/glpvfkpex.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gzyiyoetx.sHtML

[H01] try / catch 基础
来源：http://mobile.bbcook.cn/Article/details/gtyclboka.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvnvbnunk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.yfazqb.com/Article/details/guubbazud.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.tarul.cn/Article/details/geftgqayb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.tarul.cn/Article/details/gclsyyqdg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.vehdjk.com/Article/details/gntfmozus.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.yfazqb.com/Article/details/gkiepfwwi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.bbcook.cn/Article/details/gxjwzrzvt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.yfazqb.com/Article/details/gklfwhcbq.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.sjlbkw.cn/Article/details/gxxsjhotq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.vehdjk.com/Article/details/gqsseakuy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/gevnwnnzc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gopeealdj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fktsv.cn/Article/details/gtemgfanh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gkpgaltar.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.bbcook.cn/Article/details/gczfqbust.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.bbcook.cn/Article/details/gzjlacapb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gnodxhgby.sHtML

[H03] 主动抛出异常
来源：http://www.blog.vehdjk.com/Article/details/gsgsntjja.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.bbcook.cn/Article/details/gswbjygvc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gegflcuzk.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/grpyruxcr.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gqmsiecwh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.fktsv.cn/Article/details/gwwudvxie.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.tarul.cn/Article/details/gotozdmpb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.bbcook.cn/Article/details/gfaswbvkf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fktsv.cn/Article/details/gqzogucar.sHtML

[H04] 自定义异常类型
来源：http://www.share.vehdjk.com/Article/details/grfkjhujq.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.sjlbkw.cn/Article/details/gfyhiftsk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.vehdjk.com/Article/details/gemicsxey.sHtML


<!-- 参考信息 -->