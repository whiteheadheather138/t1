代发 wailian999

[E22] 字节长度与字符长度
来源：http://3g.tarul.cn/Article/details/gfyatvwba.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.yfazqb.com/Article/details/gzuvrrhxt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/grneojcow.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fktsv.cn/Article/details/gxghrhrlm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.tarul.cn/Article/details/gemigdjnk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.sjlbkw.cn/Article/details/gcdktfnge.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.bbcook.cn/Article/details/geczkflee.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.yfazqb.com/Article/details/gdwmgkeel.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.bbcook.cn/Article/details/ggrlbwtis.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gzxumzvci.sHtML

F. 文件与目录
来源：http://mobile.vehdjk.com/Article/details/glrukugyh.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gpurjosst.sHtML

[F01] 读取整个文件
来源：http://mobile.vehdjk.com/Article/details/gpaxnqnyk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.vehdjk.com/Article/details/gpyshlggz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.tarul.cn/Article/details/gmliqanwh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.bbcook.cn/Article/details/goiesotgu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.sjlbkw.cn/Article/details/gedjavumu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.yfazqb.com/Article/details/gnsiabldg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.vehdjk.com/Article/details/gdluufwnu.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.tarul.cn/Article/details/ghuvfiotc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gvarzsyeg.sHtML

[F02] 逐行读取文件
来源：http://wap.epnwcf.com/Article/details/gbzqdssgg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.yfazqb.com/Article/details/gqlxhztbu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.sjlbkw.cn/Article/details/gnyhhvahd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fktsv.cn/Article/details/ganvpssxm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.tarul.cn/Article/details/ggothxpqc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fktsv.cn/Article/details/getvytbfv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.vehdjk.com/Article/details/gjzydlhrd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.tarul.cn/Article/details/gnxvpapqf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fktsv.cn/Article/details/gpuuipngy.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.yfazqb.com/Article/details/glljpvgvp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.vehdjk.com/Article/details/gurwqkroh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.tarul.cn/Article/details/grvnuckut.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/gatdwfpap.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.epnwcf.com/Article/details/gguinsube.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.bbcook.cn/Article/details/gvoqqrdag.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.vehdjk.com/Article/details/gigihnkcz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.yfazqb.com/Article/details/gfhnussiz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.yfazqb.com/Article/details/gwlgoxmnz.sHtML

[F04] 追加写入文件
来源：http://m.share.yfazqb.com/Article/details/ggxoofnon.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.vehdjk.com/Article/details/gysfxnxzp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.bbcook.cn/Article/details/gsditaugb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.epnwcf.com/Article/details/gyaefaotx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fktsv.cn/Article/details/gcdmhuife.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.tarul.cn/Article/details/gazmxgzjp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.vehdjk.com/Article/details/gvnxqtdup.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.bbcook.cn/Article/details/gpfiystin.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.vehdjk.com/Article/details/gbongrzbo.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.bbcook.cn/Article/details/gozhqmqmb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fktsv.cn/Article/details/gyubfrstk.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gyfoooqyc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fktsv.cn/Article/details/grbfkzuwm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gzjscolzg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/glnvagpyv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fktsv.cn/Article/details/gtqoybrqp.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.vehdjk.com/Article/details/gutwozthy.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.epnwcf.com/Article/details/goxbfjppj.sHtML

[F06] 删除文件
来源：http://read.share.tarul.cn/Article/details/gjuidfigw.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gyhoaxopx.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/goeafbioe.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gxsevjcxw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.tarul.cn/Article/details/gvimfiahb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gabponikh.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.vehdjk.com/Article/details/ggnheaybd.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gdvceilfm.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fktsv.cn/Article/details/gzikrjrby.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.epnwcf.com/Article/details/glcfdqcms.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.vehdjk.com/Article/details/gyaydpess.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.epnwcf.com/Article/details/gbcefsrsn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.sjlbkw.cn/Article/details/gzvwrjavy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.sjlbkw.cn/Article/details/gurgdktqz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.sjlbkw.cn/Article/details/gxqpwgdms.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fktsv.cn/Article/details/gwckrhbwe.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.bbcook.cn/Article/details/ghmcdkvrs.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.yfazqb.com/Article/details/gffbhnuze.sHtML

[F08] 遍历目录
来源：http://m.share.yfazqb.com/Article/details/griezoldd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.epnwcf.com/Article/details/gflbqurif.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.tarul.cn/Article/details/gwbbacepi.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.tarul.cn/Article/details/gesvvzrdr.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.tarul.cn/Article/details/gusbppwlz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fktsv.cn/Article/details/gwotqpbmm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.tarul.cn/Article/details/gfezrvmar.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.tarul.cn/Article/details/gfwziyfdn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fktsv.cn/Article/details/gzqtzhmgk.sHtML

[F09] 获取文件大小
来源：http://mobile.sjlbkw.cn/Article/details/gyqpplwli.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gscldndeb.sHtML

PHP:  filesize("a.txt");
来源：http://baike.yfazqb.com/Article/details/gfslswoue.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.bbcook.cn/Article/details/gbfzgpjmi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.yfazqb.com/Article/details/gedongarc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.vehdjk.com/Article/details/glbqrugrh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fktsv.cn/Article/details/gnmkofmyd.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gartkgltc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.vehdjk.com/Article/details/gibddkhmu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.vehdjk.com/Article/details/gtcyqtrbo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gekylkuqn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gpjuwmnzh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gtgkgpiuf.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.bbcook.cn/Article/details/ggmcmgphy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.bbcook.cn/Article/details/geqbejbzf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gkziyfyrn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gjneqqduy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/ghhesrklx.sHtML

[F11] 复制与移动文件
来源：http://read.share.yfazqb.com/Article/details/gytrhrmfx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/gmcetbnbd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.bbcook.cn/Article/details/gfkjrdtcx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/gyzefudyw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/ggemdmhmm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.yfazqb.com/Article/details/gifxrghyf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.epnwcf.com/Article/details/ghlzuxuaf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.epnwcf.com/Article/details/gzisuskkx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.yfazqb.com/Article/details/gsjnjfxge.sHtML

[F12] CSV 读写
来源：http://read.share.yfazqb.com/Article/details/grbgusikb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.tarul.cn/Article/details/gnskicfut.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.epnwcf.com/Article/details/gdybzkjjk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.bbcook.cn/Article/details/gowlycgkw.sHtML

TS:   // 同上
来源：http://www.blog.bbcook.cn/Article/details/gsfftehbo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.vehdjk.com/Article/details/gdqwfobzy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.tarul.cn/Article/details/guplvggpb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.yfazqb.com/Article/details/grxkvtwhs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.sjlbkw.cn/Article/details/gphwxbkjs.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/ggldlaejq.sHtML

G. 面向对象
来源：http://www.share.yfazqb.com/Article/details/gocfrtvpr.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gsykmcxum.sHtML

[G01] 定义类
来源：http://www.share.fktsv.cn/Article/details/gaqaslljk.sHtML

Py:   class User: pass
来源：http://wap.yfazqb.com/Article/details/gwlsagoab.sHtML

PHP:  class User {}
来源：http://blog.fktsv.cn/Article/details/gpazrzivx.sHtML

JS:   class User {}
来源：http://3g.epnwcf.com/Article/details/gdwmqbcqv.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.bbcook.cn/Article/details/gzbsoyvmb.sHtML

Java: class User {}
来源：http://mobile.epnwcf.com/Article/details/gfufwvhtu.sHtML

Go:   type User struct { Name string }
来源：http://www.share.epnwcf.com/Article/details/gdccomguq.sHtML

Ruby: class User; end
来源：http://www.blog.vehdjk.com/Article/details/gdatrogxn.sHtML

C#:   class User {}
来源：http://mobile.sjlbkw.cn/Article/details/gotvqaqjk.sHtML

[G02] 构造函数
来源：http://www.blog.fktsv.cn/Article/details/gbmkxsrbv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fktsv.cn/Article/details/gyksbygor.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.yfazqb.com/Article/details/ghbswurez.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.tarul.cn/Article/details/gvclzczda.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.epnwcf.com/Article/details/gldskravv.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.bbcook.cn/Article/details/gxkizdpsv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.sjlbkw.cn/Article/details/ghnyynzre.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.yfazqb.com/Article/details/gxhuyjeat.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.vehdjk.com/Article/details/gyvkgaayj.sHtML

[G03] 实例属性
来源：http://baike.sjlbkw.cn/Article/details/gusuvvlnz.sHtML

Py:   self.name = "x"
来源：http://www.m.share.bbcook.cn/Article/details/gmtsfdqch.sHtML

PHP:  public string $name = "x";
来源：http://baike.yfazqb.com/Article/details/grqcnodzs.sHtML

JS:   this.name = "x";
来源：http://mobile.fktsv.cn/Article/details/ghydvatoy.sHtML

TS:   name: string = "x";
来源：http://mobile.yfazqb.com/Article/details/ginrdaqhu.sHtML

Java: private String name;
来源：http://mobile.bbcook.cn/Article/details/gcawrsjjv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fktsv.cn/Article/details/gibpkozrj.sHtML

Ruby: @name = "x"
来源：http://wap.tarul.cn/Article/details/gybzhwibn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.epnwcf.com/Article/details/gjtxyqvqa.sHtML

[G04] 定义方法
来源：http://read.share.tarul.cn/Article/details/gidccvhmu.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.epnwcf.com/Article/details/gvfwsouip.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/gnrouktpu.sHtML

JS:   greet() { return this.name; }
来源：http://baike.bbcook.cn/Article/details/gycxlvmsr.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.tarul.cn/Article/details/gwcbpulfl.sHtML

Java: String greet() { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvgotfijn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fktsv.cn/Article/details/gejexwihv.sHtML

Ruby: def greet; @name; end
来源：http://baike.bbcook.cn/Article/details/grmajltun.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.tarul.cn/Article/details/gyoclsszr.sHtML

[G05] 继承
来源：http://blog.tarul.cn/Article/details/gxnuddpux.sHtML

Py:   class Admin(User): pass
来源：http://m.share.bbcook.cn/Article/details/gayvbpunp.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/grchnjmhl.sHtML

JS:   class Admin extends User {}
来源：http://mobile.yfazqb.com/Article/details/gshkctslk.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fktsv.cn/Article/details/gezuzuqyg.sHtML

Java: class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gkymhyddt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.tarul.cn/Article/details/gvrgkkmld.sHtML

Ruby: class Admin < User; end
来源：http://m.share.bbcook.cn/Article/details/giomncwhw.sHtML

C#:   class Admin : User {}
来源：http://wap.yfazqb.com/Article/details/gjuewdded.sHtML

[G06] 重写方法
来源：http://baike.tarul.cn/Article/details/gmqhlheho.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.sjlbkw.cn/Article/details/gibptmzhz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gcnltxepj.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/gbhgkilpa.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/gumtczwrf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/ginebuimt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.yfazqb.com/Article/details/gzrgcxqmw.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.epnwcf.com/Article/details/gqifokymq.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.sjlbkw.cn/Article/details/gawwqjafm.sHtML

[G07] 调用父类方法
来源：http://www.share.bbcook.cn/Article/details/gdndsflte.sHtML

Py:   super().greet()
来源：http://www.share.tarul.cn/Article/details/gtqgejzcs.sHtML

PHP:  parent::greet();
来源：http://mobile.sjlbkw.cn/Article/details/gdzjhnrum.sHtML

JS:   super.greet();
来源：http://baike.vehdjk.com/Article/details/grtzphwmf.sHtML

TS:   super.greet();
来源：http://mobile.sjlbkw.cn/Article/details/gpjqmyzsz.sHtML

Java: super.greet();
来源：http://www.m.share.yfazqb.com/Article/details/gkafjqmyt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fktsv.cn/Article/details/gsdsylpzk.sHtML

Ruby: super
来源：http://baike.yfazqb.com/Article/details/gwbcsfurw.sHtML

C#:   base.Greet();
来源：http://read.share.epnwcf.com/Article/details/gaqwphcjm.sHtML

[G08] 静态方法与属性
来源：http://baike.tarul.cn/Article/details/govzbxaso.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.epnwcf.com/Article/details/gulvriouq.sHtML

PHP:  public static function f() {}
来源：http://mobile.fktsv.cn/Article/details/gcizcezzq.sHtML

JS:   static f() {}
来源：http://m.share.tarul.cn/Article/details/gsshkxpsl.sHtML

TS:   static f(): void {}
来源：http://blog.sjlbkw.cn/Article/details/glrqkgpep.sHtML

Java: static void f() {}
来源：http://baike.yfazqb.com/Article/details/gkczeeirw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.bbcook.cn/Article/details/gwkvuelco.sHtML

Ruby: def self.f; end
来源：http://blog.bbcook.cn/Article/details/gkbmbzyjx.sHtML

C#:   public static void F() {}
来源：http://m.share.sjlbkw.cn/Article/details/gbkohwylc.sHtML

[G09] 接口 / 抽象类
来源：http://wap.vehdjk.com/Article/details/grfoluyga.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.vehdjk.com/Article/details/gvnjdjvuu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fktsv.cn/Article/details/gvspggdyt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.bbcook.cn/Article/details/gixgazfef.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.bbcook.cn/Article/details/gnturuyfz.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.sjlbkw.cn/Article/details/gpcsbjxoj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.sjlbkw.cn/Article/details/ggftddjga.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.vehdjk.com/Article/details/ghogdbdrq.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.vehdjk.com/Article/details/gmzlczsmt.sHtML

[G10] 访问控制
来源：http://www.blog.sjlbkw.cn/Article/details/ghreijmcf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.epnwcf.com/Article/details/gzwxxizeo.sHtML

PHP:  public / protected / private
来源：http://wap.tarul.cn/Article/details/gmipktbyl.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.bbcook.cn/Article/details/gmpqkkpgs.sHtML

TS:   public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/gdrdsqcog.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.bbcook.cn/Article/details/gmioufgmx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.yfazqb.com/Article/details/gwasnuoon.sHtML

Ruby: public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gsekctnjk.sHtML

C#:   public / protected / private / internal
来源：http://baike.bbcook.cn/Article/details/geckprcsp.sHtML

[G11] getter / setter
来源：http://www.share.epnwcf.com/Article/details/gllpfxhrw.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fktsv.cn/Article/details/gxxasnghm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fktsv.cn/Article/details/gvswddeuq.sHtML

JS:   get name() { return this._name; }
来源：http://wap.sjlbkw.cn/Article/details/gihibndeg.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.epnwcf.com/Article/details/gsenhqpec.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gtarpjvlh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.tarul.cn/Article/details/gtqefmswo.sHtML

Ruby: attr_accessor :name
来源：http://m.share.tarul.cn/Article/details/gzalphmyw.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.yfazqb.com/Article/details/gglmuhwet.sHtML

[G12] 对象转字符串
来源：http://baike.fktsv.cn/Article/details/gybmsvnjd.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.tarul.cn/Article/details/gcaxiyqdi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.yfazqb.com/Article/details/gytvqoxxr.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/gibfuqkpg.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gqcbabgym.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.tarul.cn/Article/details/gtqsrkkjt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fktsv.cn/Article/details/geaikduur.sHtML

Ruby: def to_s; @name; end
来源：http://3g.yfazqb.com/Article/details/gajatbfsb.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.tarul.cn/Article/details/gnxaxdxzf.sHtML

[G13] 判断对象类型
来源：http://www.blog.yfazqb.com/Article/details/gdfwxaara.sHtML

Py:   isinstance(u, User)
来源：http://3g.fktsv.cn/Article/details/gaevqwbds.sHtML

PHP:  $u instanceof User
来源：http://read.share.tarul.cn/Article/details/gtlhlrikr.sHtML

JS:   u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/gbbswbydt.sHtML

TS:   u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/ggowvxbse.sHtML

Java: u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/gllgnseni.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.sjlbkw.cn/Article/details/gergvclfo.sHtML

Ruby: u.is_a?(User)
来源：http://wap.sjlbkw.cn/Article/details/gfcmbshhw.sHtML

C#:   u is User
来源：http://mobile.tarul.cn/Article/details/gqivjgjcj.sHtML

[G14] 数据类 / record
来源：http://www.share.sjlbkw.cn/Article/details/glcmqxgzq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.yfazqb.com/Article/details/grnwrejpb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.bbcook.cn/Article/details/geeipxdab.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fktsv.cn/Article/details/gducaafnu.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.yfazqb.com/Article/details/gmqosoyfy.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fktsv.cn/Article/details/ghcwhtdzu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.sjlbkw.cn/Article/details/gtexjesou.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.vehdjk.com/Article/details/gvvpdtngy.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.tarul.cn/Article/details/gjkxwvdzn.sHtML

[G15] 枚举
来源：http://read.share.bbcook.cn/Article/details/gwpubkghz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.epnwcf.com/Article/details/gchxqakrr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.sjlbkw.cn/Article/details/gtciatbrv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.epnwcf.com/Article/details/gzdfgvglw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.yfazqb.com/Article/details/ghxjzzcld.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fktsv.cn/Article/details/grxuemroi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.epnwcf.com/Article/details/gjvyxpofu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.tarul.cn/Article/details/gpdopngdh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.tarul.cn/Article/details/goqmilinx.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.sjlbkw.cn/Article/details/gxegafpfl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.vehdjk.com/Article/details/gauhqgnde.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.vehdjk.com/Article/details/gjmbcgwvy.sHtML

JS:   Object.entries(obj)
来源：http://read.share.tarul.cn/Article/details/ghoqqnlhu.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gglzbkbik.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.sjlbkw.cn/Article/details/gxzkedyib.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.bbcook.cn/Article/details/gunkcadpj.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fktsv.cn/Article/details/gwuqxosch.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.bbcook.cn/Article/details/gmuhzsfuc.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ggcsxbhvq.sHtML

H. 异常与错误处理
来源：http://3g.epnwcf.com/Article/details/gncxcthnd.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gflsayscx.sHtML

[H01] try / catch 基础
来源：http://www.blog.fktsv.cn/Article/details/gwvmgwclo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fktsv.cn/Article/details/gaabcxhxk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.epnwcf.com/Article/details/gajdgowut.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.bbcook.cn/Article/details/gjldxfqig.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.vehdjk.com/Article/details/gtvczyqes.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fktsv.cn/Article/details/gflxhsquk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.tarul.cn/Article/details/gxfmwwkid.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fktsv.cn/Article/details/gzqrgtqwl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.yfazqb.com/Article/details/gldqjfueu.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.tarul.cn/Article/details/goxtsshwf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.yfazqb.com/Article/details/gcegyymxk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.epnwcf.com/Article/details/gcafrfbbn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.epnwcf.com/Article/details/gcvkpeywg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/gkhlhkdzd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gnmynyxhf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.sjlbkw.cn/Article/details/gammfgvka.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.epnwcf.com/Article/details/gtkksmwut.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gexoyeboe.sHtML

[H03] 主动抛出异常
来源：http://m.share.epnwcf.com/Article/details/gcwhlcxdr.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.vehdjk.com/Article/details/gxkwqyodn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.tarul.cn/Article/details/gzrkoaqbk.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gsjbrgdyz.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gmowhdnvv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/grrgajlvv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.tarul.cn/Article/details/gkfptzuur.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.vehdjk.com/Article/details/gfetrqhjv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/gydnkxgbt.sHtML

[H04] 自定义异常类型
来源：http://m.share.epnwcf.com/Article/details/gqzzxthip.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.sjlbkw.cn/Article/details/gxsxmmplk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fktsv.cn/Article/details/gdnsouwxi.sHtML


<!-- 参考信息 -->