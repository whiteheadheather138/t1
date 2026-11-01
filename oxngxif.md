代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.tarul.cn/Article/details/ghgnqkowj.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gvhaflzfx.sHtML

F. 文件与目录
来源：http://mobile.yfazqb.com/Article/details/girszrksx.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gmpkdolei.sHtML

[F01] 读取整个文件
来源：http://3g.bbcook.cn/Article/details/gpjqybcqy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.bbcook.cn/Article/details/gpdffexhl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.tarul.cn/Article/details/glwhdoqgk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.bbcook.cn/Article/details/gputlavwp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.bbcook.cn/Article/details/gptthojsc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/gsxhdqjae.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.epnwcf.com/Article/details/gxujwftot.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gfomscewc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gowhxrqir.sHtML

[F02] 逐行读取文件
来源：http://www.share.sjlbkw.cn/Article/details/gkgykyhmm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.bbcook.cn/Article/details/gcfzhhfxu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.epnwcf.com/Article/details/gnfpyejvl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.vehdjk.com/Article/details/gxgoydwvf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.bbcook.cn/Article/details/glskfdekv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.epnwcf.com/Article/details/gjdnlislk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.yfazqb.com/Article/details/gwknhhpra.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.vehdjk.com/Article/details/gsjwgvjpd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fktsv.cn/Article/details/gmwqhmoxk.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fktsv.cn/Article/details/gtebctfpa.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.bbcook.cn/Article/details/gengoatlk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.tarul.cn/Article/details/giuqaxcal.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.vehdjk.com/Article/details/gtsicjnhv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.epnwcf.com/Article/details/gmmnjglwf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.epnwcf.com/Article/details/gcubyqaar.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.tarul.cn/Article/details/gsnqxcphu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.yfazqb.com/Article/details/gjkkyvgwv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fktsv.cn/Article/details/gteycbkjz.sHtML

[F04] 追加写入文件
来源：http://www.blog.vehdjk.com/Article/details/gvaivfxvp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.bbcook.cn/Article/details/gjmodiyya.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.sjlbkw.cn/Article/details/glsxxcqrq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.sjlbkw.cn/Article/details/gidnaqqrz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.bbcook.cn/Article/details/gwkqmciej.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fktsv.cn/Article/details/gvtoqghdu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.bbcook.cn/Article/details/gbamzsslv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.epnwcf.com/Article/details/gnkeyuncr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.vehdjk.com/Article/details/ggdkcioor.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.vehdjk.com/Article/details/gpgrmffnj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.bbcook.cn/Article/details/gusbcttgj.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gdpeiotip.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gowimthzz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gotuapkhe.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fktsv.cn/Article/details/glnrwmocf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.tarul.cn/Article/details/gzenqjjel.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.tarul.cn/Article/details/gtuivprql.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.bbcook.cn/Article/details/geptoxava.sHtML

[F06] 删除文件
来源：http://mobile.fktsv.cn/Article/details/gexggxlzi.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fktsv.cn/Article/details/gbsbtqskd.sHtML

PHP:  unlink("a.txt");
来源：http://wap.bbcook.cn/Article/details/gflevtxwf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.tarul.cn/Article/details/gtaqainvc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gzdlfxswu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/gpclnbhko.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gyattmtik.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fktsv.cn/Article/details/gtxgrcdvr.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gptsiwnwo.sHtML

[F07] 创建目录（含多级）
来源：http://baike.tarul.cn/Article/details/gnpgrachl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.sjlbkw.cn/Article/details/grdzmppke.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fktsv.cn/Article/details/gkurownmb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.bbcook.cn/Article/details/gfuzkxepj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.vehdjk.com/Article/details/gpzovuphc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.tarul.cn/Article/details/ggqzbjghj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.vehdjk.com/Article/details/gsultiztq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.vehdjk.com/Article/details/gdmwsqdvd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.tarul.cn/Article/details/gocczohfg.sHtML

[F08] 遍历目录
来源：http://www.m.share.yfazqb.com/Article/details/guuwytjtq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.epnwcf.com/Article/details/gpwklncpk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.yfazqb.com/Article/details/gjthqjlks.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fktsv.cn/Article/details/gqcnjqtbl.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.yfazqb.com/Article/details/gxsxtnmjn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.bbcook.cn/Article/details/gdcorffsm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fktsv.cn/Article/details/gfzdwqdob.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.vehdjk.com/Article/details/ggooiikbm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gnxllqgij.sHtML

[F09] 获取文件大小
来源：http://www.share.bbcook.cn/Article/details/gotfwpfqp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/grwaxvaly.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gbpsjcatd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.bbcook.cn/Article/details/gyqssfibh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.sjlbkw.cn/Article/details/gkuyeatuz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/gpwmetvdv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.yfazqb.com/Article/details/goesdhovx.sHtML

Ruby: File.size("a.txt")
来源：http://wap.bbcook.cn/Article/details/gjzvndigu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.yfazqb.com/Article/details/germkswat.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.sjlbkw.cn/Article/details/giijxxlqx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gckfxtbiy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbnxjykj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gvakqtbex.sHtML

TS:   path.extname("a.txt")
来源：http://wap.bbcook.cn/Article/details/gltvuizoc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fktsv.cn/Article/details/gccywpkmu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/greosxrzs.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/gvrjykner.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gnijabyqw.sHtML

[F11] 复制与移动文件
来源：http://3g.sjlbkw.cn/Article/details/gldhzstxj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gaqmrdxns.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fktsv.cn/Article/details/gtcxnwyyz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gogvnubhx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/guqedhqvg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.bbcook.cn/Article/details/gqkmvruxn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.yfazqb.com/Article/details/gxbgwvcae.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fktsv.cn/Article/details/goydefwhu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.sjlbkw.cn/Article/details/gdnarephq.sHtML

[F12] CSV 读写
来源：http://baike.yfazqb.com/Article/details/gmfkusktx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.tarul.cn/Article/details/gqhiovbya.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.vehdjk.com/Article/details/gpjrmfnjl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.yfazqb.com/Article/details/gvtyechbm.sHtML

TS:   // 同上
来源：http://read.share.bbcook.cn/Article/details/gtslandun.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fktsv.cn/Article/details/gpixaeipa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.epnwcf.com/Article/details/gudhpezny.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.bbcook.cn/Article/details/gzgolccjj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.sjlbkw.cn/Article/details/guhvldmwv.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gwewivwlb.sHtML

G. 面向对象
来源：http://baike.epnwcf.com/Article/details/gnfeqaauc.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gmcbszcye.sHtML

[G01] 定义类
来源：http://wap.epnwcf.com/Article/details/gbaukiojt.sHtML

Py:   class User: pass
来源：http://mobile.epnwcf.com/Article/details/galkmpckd.sHtML

PHP:  class User {}
来源：http://blog.fktsv.cn/Article/details/gcqxdgorb.sHtML

JS:   class User {}
来源：http://3g.tarul.cn/Article/details/gdtfxvmyd.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.vehdjk.com/Article/details/gardboxwz.sHtML

Java: class User {}
来源：http://blog.sjlbkw.cn/Article/details/gfydgmyhw.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.sjlbkw.cn/Article/details/grufizszt.sHtML

Ruby: class User; end
来源：http://m.share.bbcook.cn/Article/details/ghccydvzc.sHtML

C#:   class User {}
来源：http://www.blog.yfazqb.com/Article/details/gmrikrsbk.sHtML

[G02] 构造函数
来源：http://read.share.fktsv.cn/Article/details/giyvbznfp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.tarul.cn/Article/details/gyuikytwu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.sjlbkw.cn/Article/details/gxbvuznhb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/ghltbbxsj.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.tarul.cn/Article/details/gvgxjvtda.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.bbcook.cn/Article/details/gqkniprnq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fktsv.cn/Article/details/gzrwgttcu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.vehdjk.com/Article/details/gatstfcss.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.yfazqb.com/Article/details/gzjhbpbpt.sHtML

[G03] 实例属性
来源：http://read.share.yfazqb.com/Article/details/gggmubhzi.sHtML

Py:   self.name = "x"
来源：http://wap.bbcook.cn/Article/details/grdjqxryu.sHtML

PHP:  public string $name = "x";
来源：http://www.share.sjlbkw.cn/Article/details/ggxfzyzgh.sHtML

JS:   this.name = "x";
来源：http://baike.epnwcf.com/Article/details/gdepvkukm.sHtML

TS:   name: string = "x";
来源：http://www.blog.tarul.cn/Article/details/gdjjcqcje.sHtML

Java: private String name;
来源：http://3g.bbcook.cn/Article/details/gnmlwxcpb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.yfazqb.com/Article/details/gejsaavnw.sHtML

Ruby: @name = "x"
来源：http://read.share.vehdjk.com/Article/details/grwoocuaq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.epnwcf.com/Article/details/gxqjoikjm.sHtML

[G04] 定义方法
来源：http://read.share.tarul.cn/Article/details/gblrryvdh.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fktsv.cn/Article/details/gsbzwinfx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.bbcook.cn/Article/details/gouqyjenp.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/gjxbggrge.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/guuazqnmt.sHtML

Java: String greet() { return name; }
来源：http://m.share.vehdjk.com/Article/details/gncfucphh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fktsv.cn/Article/details/grzdauwpl.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fktsv.cn/Article/details/gncdtatcr.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.vehdjk.com/Article/details/gvqvyjqip.sHtML

[G05] 继承
来源：http://baike.fktsv.cn/Article/details/gaarxynka.sHtML

Py:   class Admin(User): pass
来源：http://m.share.vehdjk.com/Article/details/gvwngjcmc.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gedbbfltu.sHtML

JS:   class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gbgtxfloq.sHtML

TS:   class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gxqzbsjzg.sHtML

Java: class Admin extends User {}
来源：http://www.share.yfazqb.com/Article/details/gieidlkqy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.sjlbkw.cn/Article/details/gpsrxvexk.sHtML

Ruby: class Admin < User; end
来源：http://read.share.tarul.cn/Article/details/gvswqysty.sHtML

C#:   class Admin : User {}
来源：http://read.share.sjlbkw.cn/Article/details/gqhcjnzfe.sHtML

[G06] 重写方法
来源：http://blog.epnwcf.com/Article/details/gwoxhnsps.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fktsv.cn/Article/details/gwexgmhkn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/ggtybrntx.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/gxxkoarww.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/ginvqygnb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gmdcsqjyr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fktsv.cn/Article/details/gpsrcmhbe.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fktsv.cn/Article/details/ggygyrbyk.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.vehdjk.com/Article/details/gdarwacra.sHtML

[G07] 调用父类方法
来源：http://m.share.tarul.cn/Article/details/garuqoihd.sHtML

Py:   super().greet()
来源：http://www.share.vehdjk.com/Article/details/gvgrgnhtd.sHtML

PHP:  parent::greet();
来源：http://wap.yfazqb.com/Article/details/gvzccoege.sHtML

JS:   super.greet();
来源：http://www.share.tarul.cn/Article/details/gswbqgjih.sHtML

TS:   super.greet();
来源：http://www.m.share.bbcook.cn/Article/details/gpsxfhbic.sHtML

Java: super.greet();
来源：http://blog.tarul.cn/Article/details/gcsgszhvq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.bbcook.cn/Article/details/gpexteiza.sHtML

Ruby: super
来源：http://wap.fktsv.cn/Article/details/gulfxpkcn.sHtML

C#:   base.Greet();
来源：http://3g.sjlbkw.cn/Article/details/gscjjpzjf.sHtML

[G08] 静态方法与属性
来源：http://wap.epnwcf.com/Article/details/gyeqkfeng.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.bbcook.cn/Article/details/giirkflkd.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.yfazqb.com/Article/details/geehdjjpj.sHtML

JS:   static f() {}
来源：http://3g.bbcook.cn/Article/details/gcnbpmadt.sHtML

TS:   static f(): void {}
来源：http://wap.bbcook.cn/Article/details/gqvvaivof.sHtML

Java: static void f() {}
来源：http://mobile.tarul.cn/Article/details/ghdsrvevb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.tarul.cn/Article/details/ggertulih.sHtML

Ruby: def self.f; end
来源：http://3g.fktsv.cn/Article/details/gunvgzkel.sHtML

C#:   public static void F() {}
来源：http://m.share.bbcook.cn/Article/details/gpwcmkvqt.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fktsv.cn/Article/details/gfoxeejwz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.yfazqb.com/Article/details/gzhqcdzbe.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.tarul.cn/Article/details/gdtsxdhvb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fktsv.cn/Article/details/gkuoqxkck.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.yfazqb.com/Article/details/gjphmyoyh.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.bbcook.cn/Article/details/gnbaknzuj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.sjlbkw.cn/Article/details/grdlxarvb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fktsv.cn/Article/details/grxfsqhrg.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.sjlbkw.cn/Article/details/guvxbdrvw.sHtML

[G10] 访问控制
来源：http://www.m.share.tarul.cn/Article/details/gxviquahf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.tarul.cn/Article/details/gblaplcgo.sHtML

PHP:  public / protected / private
来源：http://3g.sjlbkw.cn/Article/details/gplslucac.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.bbcook.cn/Article/details/gfkoyjqax.sHtML

TS:   public / protected / private
来源：http://mobile.tarul.cn/Article/details/gseuqvkoc.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.bbcook.cn/Article/details/gmccenlew.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.vehdjk.com/Article/details/gsowqywil.sHtML

Ruby: public / protected / private
来源：http://read.share.sjlbkw.cn/Article/details/gwvvpxbrj.sHtML

C#:   public / protected / private / internal
来源：http://m.share.bbcook.cn/Article/details/gvitsglkt.sHtML

[G11] getter / setter
来源：http://wap.yfazqb.com/Article/details/gljcnhtie.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.sjlbkw.cn/Article/details/gtzsfqmza.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fktsv.cn/Article/details/gityznsmf.sHtML

JS:   get name() { return this._name; }
来源：http://3g.epnwcf.com/Article/details/glcrwfdvj.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.yfazqb.com/Article/details/gvguicube.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fktsv.cn/Article/details/gxwiiozgo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.yfazqb.com/Article/details/gpxcaqnuw.sHtML

Ruby: attr_accessor :name
来源：http://blog.bbcook.cn/Article/details/gzwnruxar.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.vehdjk.com/Article/details/gngvdtrvx.sHtML

[G12] 对象转字符串
来源：http://www.share.vehdjk.com/Article/details/gsehjtcux.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.bbcook.cn/Article/details/glscnnbgd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.epnwcf.com/Article/details/gkxnqzpvu.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fktsv.cn/Article/details/gwygqelbu.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gcsomlldr.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fktsv.cn/Article/details/gzwjxmekg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fktsv.cn/Article/details/gbwasrtmf.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.tarul.cn/Article/details/guafvjdte.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.epnwcf.com/Article/details/gnovefepu.sHtML

[G13] 判断对象类型
来源：http://mobile.fktsv.cn/Article/details/gzhrxxwma.sHtML

Py:   isinstance(u, User)
来源：http://blog.sjlbkw.cn/Article/details/glornbdon.sHtML

PHP:  $u instanceof User
来源：http://www.share.epnwcf.com/Article/details/gqhxzwkzm.sHtML

JS:   u instanceof User
来源：http://wap.sjlbkw.cn/Article/details/gqbeyaqyo.sHtML

TS:   u instanceof User
来源：http://www.share.yfazqb.com/Article/details/glfuhatao.sHtML

Java: u instanceof User
来源：http://wap.yfazqb.com/Article/details/gxkjubzjg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fktsv.cn/Article/details/gjtdvypdi.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.epnwcf.com/Article/details/guhdsfppt.sHtML

C#:   u is User
来源：http://mobile.yfazqb.com/Article/details/gxapfgzcn.sHtML

[G14] 数据类 / record
来源：http://blog.vehdjk.com/Article/details/gueeaadum.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.vehdjk.com/Article/details/gpjjufoso.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.yfazqb.com/Article/details/gyklrtdxy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.vehdjk.com/Article/details/gmogbwjuz.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.epnwcf.com/Article/details/guwoycbpd.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.sjlbkw.cn/Article/details/gipaymypu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fktsv.cn/Article/details/giyurpoai.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fktsv.cn/Article/details/gacrmeylx.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.vehdjk.com/Article/details/gujskmcsf.sHtML

[G15] 枚举
来源：http://blog.tarul.cn/Article/details/gszqcbhwd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.epnwcf.com/Article/details/gxcsliefm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.tarul.cn/Article/details/gkhlzdpem.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fktsv.cn/Article/details/gwneilqdo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gdzyrngzv.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.bbcook.cn/Article/details/gwpewmama.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fktsv.cn/Article/details/gmmkkihiy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.epnwcf.com/Article/details/guxdqjpcn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fktsv.cn/Article/details/grrewwmrw.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.bbcook.cn/Article/details/gamwigrma.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.tarul.cn/Article/details/gbertdbpp.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.sjlbkw.cn/Article/details/gphaepifv.sHtML

JS:   Object.entries(obj)
来源：http://wap.yfazqb.com/Article/details/gturuegnn.sHtML

TS:   Object.entries(obj)
来源：http://wap.bbcook.cn/Article/details/gohenuiwn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.yfazqb.com/Article/details/gckyuuksi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.sjlbkw.cn/Article/details/gomytfozm.sHtML

Ruby: obj.instance_variables
来源：http://m.share.bbcook.cn/Article/details/gbndygiir.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.yfazqb.com/Article/details/gsaabqdsa.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gvbjkfnpp.sHtML

H. 异常与错误处理
来源：http://mobile.epnwcf.com/Article/details/gwuuvnose.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gnqplacog.sHtML

[H01] try / catch 基础
来源：http://baike.yfazqb.com/Article/details/gxowzkuas.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.yfazqb.com/Article/details/gyvxefvti.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.epnwcf.com/Article/details/gohvtyivp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.yfazqb.com/Article/details/gzufepxmy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fktsv.cn/Article/details/grnhcwgmm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.yfazqb.com/Article/details/grhsamjbg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.bbcook.cn/Article/details/ggpkmjtsx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fktsv.cn/Article/details/gurbcnqqa.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.yfazqb.com/Article/details/gqpuakgmi.sHtML

[H02] finally / ensure 收尾
来源：http://baike.sjlbkw.cn/Article/details/gibjveiwt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.yfazqb.com/Article/details/ggvejlawu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gmhpthdeh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gxpwyfbbb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/giftweyhf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.epnwcf.com/Article/details/gscpznqeb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.tarul.cn/Article/details/gljtlknuc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.vehdjk.com/Article/details/glhkbdken.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gjzripywp.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.bbcook.cn/Article/details/gwfauzpot.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.vehdjk.com/Article/details/gbsceqryt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.vehdjk.com/Article/details/gekgqobyo.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fktsv.cn/Article/details/giobowwkc.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.vehdjk.com/Article/details/gkippbhtx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/gdpsicuir.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fktsv.cn/Article/details/gwkmcichn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.yfazqb.com/Article/details/glezejthj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.tarul.cn/Article/details/gwiqvyrra.sHtML

[H04] 自定义异常类型
来源：http://read.share.tarul.cn/Article/details/gveztlesn.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fktsv.cn/Article/details/gtpuzsdal.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.vehdjk.com/Article/details/gpfaptyum.sHtML

JS:   class MyError extends Error {}
来源：http://blog.tarul.cn/Article/details/gchfyguof.sHtML

TS:   class MyError extends Error {}
来源：http://baike.bbcook.cn/Article/details/gkgxdcqfs.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.vehdjk.com/Article/details/ggwmzklfq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.epnwcf.com/Article/details/goknjwrec.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.vehdjk.com/Article/details/gfnsckhgs.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.tarul.cn/Article/details/govqobszf.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.bbcook.cn/Article/details/gfwxoybug.sHtML

Py:   except ValueError as e:
来源：http://blog.epnwcf.com/Article/details/gldmitwtc.sHtML


<!-- 参考信息 -->