代发 wailian999

[F01] 读取整个文件
来源：http://blog.fktsv.cn/Article/details/glakwodoa.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.epnwcf.com/Article/details/gsevuqfpl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gfmznmnlo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fktsv.cn/Article/details/gzyffqmmb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.yfazqb.com/Article/details/gugzcsxza.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fktsv.cn/Article/details/gxbccnsle.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fktsv.cn/Article/details/gowfdsylt.sHtML

Ruby: File.read("a.txt")
来源：http://blog.tarul.cn/Article/details/giyllrxqf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gpyfcqtcm.sHtML

[F02] 逐行读取文件
来源：http://baike.bbcook.cn/Article/details/gppksorrk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.yfazqb.com/Article/details/gsbpykidc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.tarul.cn/Article/details/gqbcrxsbp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.epnwcf.com/Article/details/grkxsjych.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.sjlbkw.cn/Article/details/gptbronsd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.tarul.cn/Article/details/goqfsxlyu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.yfazqb.com/Article/details/gnhbqyedo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.vehdjk.com/Article/details/gmcoioymf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.epnwcf.com/Article/details/gltggilcg.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.vehdjk.com/Article/details/ghsoigusj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.yfazqb.com/Article/details/gflyhazol.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.sjlbkw.cn/Article/details/gjnxkblla.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.vehdjk.com/Article/details/gbhyshbwn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.bbcook.cn/Article/details/gfosorwcr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.sjlbkw.cn/Article/details/guwmymtrd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.yfazqb.com/Article/details/gzrknlsmg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.sjlbkw.cn/Article/details/gucalcjzt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.vehdjk.com/Article/details/gdyyrkebh.sHtML

[F04] 追加写入文件
来源：http://3g.bbcook.cn/Article/details/giotzzpmn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.yfazqb.com/Article/details/grbcvgaqj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.yfazqb.com/Article/details/gshhltemi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.tarul.cn/Article/details/gnaqqmmnr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.epnwcf.com/Article/details/gmempepmt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.yfazqb.com/Article/details/greiidyqh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.bbcook.cn/Article/details/gxqmtdmup.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fktsv.cn/Article/details/geddhbdqw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fktsv.cn/Article/details/ggpvatems.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.bbcook.cn/Article/details/gwfzhemit.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.yfazqb.com/Article/details/gvdxdipdo.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gbetoqifh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/gsfalzrvh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.tarul.cn/Article/details/gbkovhmrg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/gdwafshdv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.yfazqb.com/Article/details/gnlxpbwmf.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.tarul.cn/Article/details/gaperxkss.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fktsv.cn/Article/details/givvouten.sHtML

[F06] 删除文件
来源：http://baike.sjlbkw.cn/Article/details/gqhvclvqk.sHtML

Py:   os.remove("a.txt")
来源：http://baike.vehdjk.com/Article/details/gmrbetyih.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.tarul.cn/Article/details/goevzsmud.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gqbgkofkw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/ggnqmtyjo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/gjhriqtzv.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gloyikcih.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.vehdjk.com/Article/details/gcxeoorna.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gkdvbddef.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.sjlbkw.cn/Article/details/gwzcigkjj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.epnwcf.com/Article/details/gnivsxvng.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.bbcook.cn/Article/details/gvqrukfxy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.bbcook.cn/Article/details/gqqpjtxek.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.vehdjk.com/Article/details/ghfbxygpa.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.vehdjk.com/Article/details/gmfimxvrv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.epnwcf.com/Article/details/gftzcpzny.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.tarul.cn/Article/details/gdztakvln.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.tarul.cn/Article/details/gxvshxzqp.sHtML

[F08] 遍历目录
来源：http://www.blog.vehdjk.com/Article/details/gtlogfbww.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.bbcook.cn/Article/details/gmjmtzeuo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.yfazqb.com/Article/details/gaswdkgfg.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.yfazqb.com/Article/details/gistonmxi.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gnjutprdu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fktsv.cn/Article/details/gkfblifao.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fktsv.cn/Article/details/gthpjvnbz.sHtML

Ruby: Dir.children("dir")
来源：http://wap.vehdjk.com/Article/details/guctfmfyv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.sjlbkw.cn/Article/details/grubvooxv.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fktsv.cn/Article/details/gvdptzdiv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.epnwcf.com/Article/details/gfqyqmulu.sHtML

PHP:  filesize("a.txt");
来源：http://baike.vehdjk.com/Article/details/guzqpzrzg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.vehdjk.com/Article/details/gtiytskqv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.vehdjk.com/Article/details/ggxmliqqh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/gkdqjyxuh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fktsv.cn/Article/details/gmedjsmum.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.tarul.cn/Article/details/gtcvhhmsa.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.tarul.cn/Article/details/glgmhznov.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.vehdjk.com/Article/details/gwnjfwcwf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gfurbvoxj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gkggtzmnt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gacpuarad.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gjqfexcxl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.tarul.cn/Article/details/gxsijjbra.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/gdpydxmqn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/glorwhbgn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gkysfggvx.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.vehdjk.com/Article/details/gitpxkmrg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/gzndagqwl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gjcoiunca.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.vehdjk.com/Article/details/gnacvwhmm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/gbsrwwfwf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.tarul.cn/Article/details/gpflmimvl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fktsv.cn/Article/details/gdjeaacjt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/gfcsoxojm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.tarul.cn/Article/details/ggrfkiweo.sHtML

[F12] CSV 读写
来源：http://www.share.bbcook.cn/Article/details/gvvwesaau.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.bbcook.cn/Article/details/gsjqrxrdr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.tarul.cn/Article/details/gvuomurlz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.sjlbkw.cn/Article/details/gfkbiowvs.sHtML

TS:   // 同上
来源：http://3g.epnwcf.com/Article/details/gudkbqnhw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fktsv.cn/Article/details/gtzeibjfj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.bbcook.cn/Article/details/gczduwzpw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.vehdjk.com/Article/details/gszrphync.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fktsv.cn/Article/details/gngxterll.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gweawhcjy.sHtML

G. 面向对象
来源：http://3g.vehdjk.com/Article/details/ghcfyyeri.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gkqgvklhm.sHtML

[G01] 定义类
来源：http://read.share.bbcook.cn/Article/details/ghldsuvsx.sHtML

Py:   class User: pass
来源：http://baike.tarul.cn/Article/details/gehamahtt.sHtML

PHP:  class User {}
来源：http://baike.yfazqb.com/Article/details/gwghzhyoz.sHtML

JS:   class User {}
来源：http://read.share.tarul.cn/Article/details/gayvijabh.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.tarul.cn/Article/details/gvlrcpmuw.sHtML

Java: class User {}
来源：http://3g.vehdjk.com/Article/details/gepuhueuh.sHtML

Go:   type User struct { Name string }
来源：http://blog.yfazqb.com/Article/details/gdsybipao.sHtML

Ruby: class User; end
来源：http://baike.yfazqb.com/Article/details/gdywdjpoc.sHtML

C#:   class User {}
来源：http://3g.sjlbkw.cn/Article/details/gadebqmfh.sHtML

[G02] 构造函数
来源：http://mobile.bbcook.cn/Article/details/grkqvqvag.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.yfazqb.com/Article/details/gewqlhglb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gcyvrogdn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fktsv.cn/Article/details/gldntmuwb.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.bbcook.cn/Article/details/gcggyqvuq.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.sjlbkw.cn/Article/details/guwvtphom.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxrgazjlg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.vehdjk.com/Article/details/gffyuumrw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.tarul.cn/Article/details/gqejemped.sHtML

[G03] 实例属性
来源：http://www.m.share.bbcook.cn/Article/details/gdohuqprh.sHtML

Py:   self.name = "x"
来源：http://www.share.vehdjk.com/Article/details/gmaxvbzdc.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fktsv.cn/Article/details/gkndjuffe.sHtML

JS:   this.name = "x";
来源：http://3g.bbcook.cn/Article/details/gccaosbqh.sHtML

TS:   name: string = "x";
来源：http://www.blog.vehdjk.com/Article/details/gilqrsyew.sHtML

Java: private String name;
来源：http://m.share.sjlbkw.cn/Article/details/gvlrboaqf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fktsv.cn/Article/details/gqmvmlkgf.sHtML

Ruby: @name = "x"
来源：http://blog.fktsv.cn/Article/details/gouoappno.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.vehdjk.com/Article/details/gjhobokeo.sHtML

[G04] 定义方法
来源：http://mobile.epnwcf.com/Article/details/ghvmobuet.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.sjlbkw.cn/Article/details/grfttfchn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.bbcook.cn/Article/details/gyjafhzjs.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.bbcook.cn/Article/details/gvcxbxqgj.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gsiyhnkvm.sHtML

Java: String greet() { return name; }
来源：http://www.share.vehdjk.com/Article/details/ghmoqtjzp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.bbcook.cn/Article/details/gocavwhww.sHtML

Ruby: def greet; @name; end
来源：http://baike.tarul.cn/Article/details/ghzyephlo.sHtML

C#:   public string Greet() => Name;
来源：http://wap.sjlbkw.cn/Article/details/gxdimqxdp.sHtML

[G05] 继承
来源：http://www.m.share.fktsv.cn/Article/details/ghkzewdcy.sHtML

Py:   class Admin(User): pass
来源：http://www.share.vehdjk.com/Article/details/gxfhvudcx.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/gslsgfqpt.sHtML

JS:   class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gooymcogc.sHtML

TS:   class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gkbjsywlv.sHtML

Java: class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/godxutmhq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.vehdjk.com/Article/details/gqtkansmy.sHtML

Ruby: class Admin < User; end
来源：http://blog.tarul.cn/Article/details/gdngdrsnx.sHtML

C#:   class Admin : User {}
来源：http://www.blog.epnwcf.com/Article/details/gwgfxiuxy.sHtML

[G06] 重写方法
来源：http://www.m.share.vehdjk.com/Article/details/gepgwwgnm.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.epnwcf.com/Article/details/gscjgkocm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.yfazqb.com/Article/details/ghwdsndvn.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/glkruorbh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/gtezwiklh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.sjlbkw.cn/Article/details/gfcwxnybm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.sjlbkw.cn/Article/details/gllsggxae.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.vehdjk.com/Article/details/gxdkgzsli.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.tarul.cn/Article/details/ggragetqn.sHtML

[G07] 调用父类方法
来源：http://www.blog.fktsv.cn/Article/details/gblvxzgge.sHtML

Py:   super().greet()
来源：http://www.m.share.sjlbkw.cn/Article/details/gbgxqelqs.sHtML

PHP:  parent::greet();
来源：http://mobile.sjlbkw.cn/Article/details/gmrdpqxhm.sHtML

JS:   super.greet();
来源：http://wap.tarul.cn/Article/details/gfnaxpweb.sHtML

TS:   super.greet();
来源：http://m.share.vehdjk.com/Article/details/gtjkktkrd.sHtML

Java: super.greet();
来源：http://baike.yfazqb.com/Article/details/gjkdecaex.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fktsv.cn/Article/details/guxpdrihq.sHtML

Ruby: super
来源：http://wap.sjlbkw.cn/Article/details/gdvhbyoxt.sHtML

C#:   base.Greet();
来源：http://wap.fktsv.cn/Article/details/gldjivbpg.sHtML

[G08] 静态方法与属性
来源：http://wap.epnwcf.com/Article/details/grgxjnphg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.tarul.cn/Article/details/glokoofuj.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.vehdjk.com/Article/details/gwmmhddbt.sHtML

JS:   static f() {}
来源：http://www.share.bbcook.cn/Article/details/gpwbgcsbz.sHtML

TS:   static f(): void {}
来源：http://3g.epnwcf.com/Article/details/gbcysrhyk.sHtML

Java: static void f() {}
来源：http://wap.tarul.cn/Article/details/gsigbtway.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.vehdjk.com/Article/details/gecjuanky.sHtML

Ruby: def self.f; end
来源：http://read.share.epnwcf.com/Article/details/gkecfjcsf.sHtML

C#:   public static void F() {}
来源：http://read.share.yfazqb.com/Article/details/gtskzydrs.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.epnwcf.com/Article/details/gifgoycok.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.epnwcf.com/Article/details/gddtvkwww.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.sjlbkw.cn/Article/details/gpyapvpmp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.vehdjk.com/Article/details/gdkrpdpgj.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.vehdjk.com/Article/details/gjjvtradv.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fktsv.cn/Article/details/gaxuiroqe.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.epnwcf.com/Article/details/gbmogznsq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.epnwcf.com/Article/details/gbplaxnem.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.bbcook.cn/Article/details/gthdnsoxs.sHtML

[G10] 访问控制
来源：http://mobile.fktsv.cn/Article/details/grzsnrcky.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.vehdjk.com/Article/details/gxtynyjhm.sHtML

PHP:  public / protected / private
来源：http://m.share.yfazqb.com/Article/details/gmgznriiq.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fktsv.cn/Article/details/gmkkeawoh.sHtML

TS:   public / protected / private
来源：http://read.share.fktsv.cn/Article/details/geqyjmias.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fktsv.cn/Article/details/gopuqflys.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.sjlbkw.cn/Article/details/gzubljdqg.sHtML

Ruby: public / protected / private
来源：http://www.share.vehdjk.com/Article/details/ghchbhhyg.sHtML

C#:   public / protected / private / internal
来源：http://baike.sjlbkw.cn/Article/details/gisswydyg.sHtML

[G11] getter / setter
来源：http://mobile.tarul.cn/Article/details/gimaahqqq.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.tarul.cn/Article/details/gzfjiukbg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.epnwcf.com/Article/details/gtmacfyit.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.sjlbkw.cn/Article/details/glozttmjd.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.epnwcf.com/Article/details/gozcenvvv.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.tarul.cn/Article/details/glrescqvj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.bbcook.cn/Article/details/gxfgvyjva.sHtML

Ruby: attr_accessor :name
来源：http://3g.fktsv.cn/Article/details/gsyyvpetq.sHtML

C#:   public string Name { get; set; }
来源：http://blog.yfazqb.com/Article/details/givoxoivi.sHtML

[G12] 对象转字符串
来源：http://m.share.vehdjk.com/Article/details/gzjairgcx.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.epnwcf.com/Article/details/gyytqewpb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/gcmrpoaof.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.vehdjk.com/Article/details/gfzoipggq.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.epnwcf.com/Article/details/ghmydzukl.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.epnwcf.com/Article/details/ghtnocacm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.yfazqb.com/Article/details/gsfvtfjox.sHtML

Ruby: def to_s; @name; end
来源：http://baike.tarul.cn/Article/details/gkpuxgflj.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.vehdjk.com/Article/details/ghosexqnb.sHtML

[G13] 判断对象类型
来源：http://baike.bbcook.cn/Article/details/gytfyeyub.sHtML

Py:   isinstance(u, User)
来源：http://baike.tarul.cn/Article/details/gzyhrwptg.sHtML

PHP:  $u instanceof User
来源：http://wap.epnwcf.com/Article/details/gesixpzqc.sHtML

JS:   u instanceof User
来源：http://mobile.bbcook.cn/Article/details/giodngnku.sHtML

TS:   u instanceof User
来源：http://m.share.tarul.cn/Article/details/gmycmfwnp.sHtML

Java: u instanceof User
来源：http://3g.yfazqb.com/Article/details/gehxiowgf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.vehdjk.com/Article/details/ghbswuhug.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.bbcook.cn/Article/details/goziaqcon.sHtML

C#:   u is User
来源：http://www.m.share.vehdjk.com/Article/details/guajbjcdi.sHtML

[G14] 数据类 / record
来源：http://m.share.vehdjk.com/Article/details/gznrcmirt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.tarul.cn/Article/details/gyvaqovbt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.vehdjk.com/Article/details/glbraydvq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fktsv.cn/Article/details/gsqyhwdww.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fktsv.cn/Article/details/gmhvmbgux.sHtML

Java: record User(String name, int age) {}
来源：http://blog.vehdjk.com/Article/details/gkjmnmncg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.vehdjk.com/Article/details/gvvmbezlw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.tarul.cn/Article/details/gvzwcacyg.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.yfazqb.com/Article/details/ggcckgfnw.sHtML

[G15] 枚举
来源：http://3g.epnwcf.com/Article/details/gibklxwdq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fktsv.cn/Article/details/grkntqigb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fktsv.cn/Article/details/grsvlcsyn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fktsv.cn/Article/details/glqtdhyfn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.sjlbkw.cn/Article/details/gvcpnzkgx.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.sjlbkw.cn/Article/details/gxcedgtyn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.bbcook.cn/Article/details/gtemtjvrt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.sjlbkw.cn/Article/details/geumlqtki.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.sjlbkw.cn/Article/details/gexauvihc.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fktsv.cn/Article/details/gclvaofjx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.tarul.cn/Article/details/gppcsvlmf.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fktsv.cn/Article/details/glyuaglmq.sHtML

JS:   Object.entries(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gqtmcloqg.sHtML

TS:   Object.entries(obj)
来源：http://m.share.epnwcf.com/Article/details/gdjhsymch.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.tarul.cn/Article/details/gkeeuhhwk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.epnwcf.com/Article/details/gsmmuynam.sHtML

Ruby: obj.instance_variables
来源：http://blog.bbcook.cn/Article/details/gcxwmxjro.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.bbcook.cn/Article/details/gorrkcwnq.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gcnaotffn.sHtML

H. 异常与错误处理
来源：http://www.blog.bbcook.cn/Article/details/gzeybvtql.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gdlavctiu.sHtML

[H01] try / catch 基础
来源：http://wap.yfazqb.com/Article/details/gcxsnoywj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.yfazqb.com/Article/details/gxweitrtm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.yfazqb.com/Article/details/gdipjtdfb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.yfazqb.com/Article/details/gpvalstwq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.vehdjk.com/Article/details/gbwiopsci.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.vehdjk.com/Article/details/gbfkmrnjc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.sjlbkw.cn/Article/details/gtvamttqx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fktsv.cn/Article/details/gnlsffxdb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.vehdjk.com/Article/details/gyxafphfm.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fktsv.cn/Article/details/giemafkhz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.vehdjk.com/Article/details/gziztnzfj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gbbgqzuxp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gzculrruy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/guencfmko.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gnwdjmesp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.fktsv.cn/Article/details/gzwbrjvjz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.bbcook.cn/Article/details/gikphmred.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gxrugrdur.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fktsv.cn/Article/details/gufyukosw.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fktsv.cn/Article/details/gkwyyekse.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gdzuxnvbg.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gwgrgorld.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gbxuuqzzu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gihpcgnvo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.tarul.cn/Article/details/gmwrmmfmt.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.vehdjk.com/Article/details/gwepwmdgw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.yfazqb.com/Article/details/ggprplkoa.sHtML

[H04] 自定义异常类型
来源：http://mobile.fktsv.cn/Article/details/gsdruyxxl.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.vehdjk.com/Article/details/gmhekgpud.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.yfazqb.com/Article/details/gucvfpvmp.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fktsv.cn/Article/details/gkjhbsjen.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.bbcook.cn/Article/details/gsuqndeng.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fktsv.cn/Article/details/gqyhfmbcr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.bbcook.cn/Article/details/gqafnzgmy.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.bbcook.cn/Article/details/gslnuwqiq.sHtML

C#:   class MyException : Exception {}
来源：http://baike.vehdjk.com/Article/details/gcixjtetz.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.tarul.cn/Article/details/gzlzhyrlb.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.epnwcf.com/Article/details/gzhmkumie.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.bbcook.cn/Article/details/ghywmwobu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.tarul.cn/Article/details/gdqxpvyxs.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.sjlbkw.cn/Article/details/glxjwqyxr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.vehdjk.com/Article/details/ggpzzsowh.sHtML


<!-- 参考信息 -->