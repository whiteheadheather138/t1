代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.sjlbkw.cn/Article/details/gcprbpdab.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gvrzllqvw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.bbcook.cn/Article/details/giaxtysrh.sHtML

Ruby: File.read("a.txt")
来源：http://3g.yfazqb.com/Article/details/glzxrxlxa.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gypbrqvyj.sHtML

[F02] 逐行读取文件
来源：http://baike.fktsv.cn/Article/details/gesbfwsvi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.vehdjk.com/Article/details/grugbccan.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.bbcook.cn/Article/details/ggsdftdwm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fktsv.cn/Article/details/ghgxcdaaj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.epnwcf.com/Article/details/gqzzzbyfu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.yfazqb.com/Article/details/gozbburkf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.bbcook.cn/Article/details/glkenexxx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.yfazqb.com/Article/details/gkrtchztp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.bbcook.cn/Article/details/gkgosupqf.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.vehdjk.com/Article/details/gnkbrkmrx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.bbcook.cn/Article/details/gwobdhsey.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.sjlbkw.cn/Article/details/gsfovqikf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.vehdjk.com/Article/details/gmyywqzvs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fktsv.cn/Article/details/gnurbfkfh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.bbcook.cn/Article/details/gzgxfwogw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fktsv.cn/Article/details/greivptyz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.sjlbkw.cn/Article/details/gugpcnnlf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fktsv.cn/Article/details/gfmcxibqw.sHtML

[F04] 追加写入文件
来源：http://m.share.epnwcf.com/Article/details/gxwarmzoa.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.epnwcf.com/Article/details/grlcxeyqk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.sjlbkw.cn/Article/details/gljoxtudd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fktsv.cn/Article/details/glyrshslw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gboqazeao.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.vehdjk.com/Article/details/gvxbzkefc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fktsv.cn/Article/details/gzdswiicb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.epnwcf.com/Article/details/gtxuxmhzl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fktsv.cn/Article/details/gkmiswrbl.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.tarul.cn/Article/details/gwxsmdyrg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.bbcook.cn/Article/details/gcvxujzyb.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gdokjzwib.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.tarul.cn/Article/details/gdyltwfmy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gmagfndhx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.epnwcf.com/Article/details/gcsjjnhpa.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.sjlbkw.cn/Article/details/gyxalrmna.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkxuvogaq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gvohzitcu.sHtML

[F06] 删除文件
来源：http://m.share.tarul.cn/Article/details/gewjrhguf.sHtML

Py:   os.remove("a.txt")
来源：http://baike.bbcook.cn/Article/details/gzqovxkui.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gdzoukrcp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/ghtutoxrl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gamyfiokh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.yfazqb.com/Article/details/grozjrfwv.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gemlzqtoz.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gwhirbbym.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.bbcook.cn/Article/details/grkyyipgq.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fktsv.cn/Article/details/gudkbdvpc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fktsv.cn/Article/details/gcgaiyhhb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fktsv.cn/Article/details/ggobkihhq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.vehdjk.com/Article/details/ghumnmtzx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.epnwcf.com/Article/details/ggnwpkaka.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fktsv.cn/Article/details/gyjjytsor.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfwxffnnb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.bbcook.cn/Article/details/gsyhgsgym.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.vehdjk.com/Article/details/gsjqmsque.sHtML

[F08] 遍历目录
来源：http://read.share.tarul.cn/Article/details/gpdlkkolg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.vehdjk.com/Article/details/gspnkmzvv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.tarul.cn/Article/details/glwjsjypj.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.yfazqb.com/Article/details/gggmmdfbe.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.yfazqb.com/Article/details/gqunbcvqd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.yfazqb.com/Article/details/gbpooogly.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.yfazqb.com/Article/details/gdncqboxy.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.tarul.cn/Article/details/gbjcyzqzj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.vehdjk.com/Article/details/gbhldvvac.sHtML

[F09] 获取文件大小
来源：http://www.blog.bbcook.cn/Article/details/ghumywuic.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/ghmdpsuds.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gykvgzttm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.yfazqb.com/Article/details/gnofbxsoq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.yfazqb.com/Article/details/gjwkflhbz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/ghjswihix.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fktsv.cn/Article/details/gzjearkmm.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.tarul.cn/Article/details/gbaeofnda.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.bbcook.cn/Article/details/guzsvoamk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.tarul.cn/Article/details/ginhqdnrw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gjbatmbih.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.tarul.cn/Article/details/gcpwwcryt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gkstzpfzr.sHtML

TS:   path.extname("a.txt")
来源：http://3g.vehdjk.com/Article/details/gnmxpwnxm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.yfazqb.com/Article/details/gxspptplj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gyawlwkrh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gpcqlfnqj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gimhoyohp.sHtML

[F11] 复制与移动文件
来源：http://blog.yfazqb.com/Article/details/gsgrwmyft.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/gqejauckp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fktsv.cn/Article/details/gxuodpxbc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/gfubjdzed.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/gougxdqgt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.sjlbkw.cn/Article/details/glbnifpla.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.tarul.cn/Article/details/gyxazlcvp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/gpukvjhjq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.sjlbkw.cn/Article/details/ginmdhisg.sHtML

[F12] CSV 读写
来源：http://www.m.share.tarul.cn/Article/details/gtarrntfe.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.yfazqb.com/Article/details/gpwdpztss.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.tarul.cn/Article/details/ggnoqdtpp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.yfazqb.com/Article/details/ggyjjdbfb.sHtML

TS:   // 同上
来源：http://m.share.yfazqb.com/Article/details/gyvabacre.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.bbcook.cn/Article/details/gyvnachgl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.vehdjk.com/Article/details/gbbjvnich.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.sjlbkw.cn/Article/details/gnkbgvosy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.epnwcf.com/Article/details/gpqadhntn.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gejgmhuvl.sHtML

G. 面向对象
来源：http://www.share.tarul.cn/Article/details/gwvschgqk.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/glblbvimv.sHtML

[G01] 定义类
来源：http://3g.vehdjk.com/Article/details/gqnoqlfyv.sHtML

Py:   class User: pass
来源：http://3g.fktsv.cn/Article/details/gjpyavnpp.sHtML

PHP:  class User {}
来源：http://m.share.yfazqb.com/Article/details/gpifbaoqw.sHtML

JS:   class User {}
来源：http://www.blog.vehdjk.com/Article/details/gbrfspsjx.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.tarul.cn/Article/details/gfmjoxyoa.sHtML

Java: class User {}
来源：http://www.blog.bbcook.cn/Article/details/gyujeeuop.sHtML

Go:   type User struct { Name string }
来源：http://wap.fktsv.cn/Article/details/gazbqrkgr.sHtML

Ruby: class User; end
来源：http://3g.epnwcf.com/Article/details/gnbpceqac.sHtML

C#:   class User {}
来源：http://www.blog.vehdjk.com/Article/details/giqcpaomn.sHtML

[G02] 构造函数
来源：http://wap.tarul.cn/Article/details/glmhwrubf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.epnwcf.com/Article/details/gtvuwiefa.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.sjlbkw.cn/Article/details/ggwydeyae.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.vehdjk.com/Article/details/gjzqqvgqw.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.epnwcf.com/Article/details/gjneptmfr.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.epnwcf.com/Article/details/goondjmjs.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.tarul.cn/Article/details/gfatamdld.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.bbcook.cn/Article/details/gahluvdea.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.vehdjk.com/Article/details/gajhzfebb.sHtML

[G03] 实例属性
来源：http://read.share.epnwcf.com/Article/details/guvbzwquz.sHtML

Py:   self.name = "x"
来源：http://www.blog.vehdjk.com/Article/details/gizsmotnl.sHtML

PHP:  public string $name = "x";
来源：http://3g.epnwcf.com/Article/details/gefiyxdsu.sHtML

JS:   this.name = "x";
来源：http://baike.epnwcf.com/Article/details/gmwezsoep.sHtML

TS:   name: string = "x";
来源：http://m.share.tarul.cn/Article/details/gipztkktr.sHtML

Java: private String name;
来源：http://blog.tarul.cn/Article/details/gwbdgnvoy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.yfazqb.com/Article/details/gwametmoz.sHtML

Ruby: @name = "x"
来源：http://blog.tarul.cn/Article/details/gbbfxambw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.yfazqb.com/Article/details/gehppjbbi.sHtML

[G04] 定义方法
来源：http://read.share.yfazqb.com/Article/details/gdzegtivj.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.vehdjk.com/Article/details/gkqfmrrfn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/glshqgvlb.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/gbjafiirf.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gbgkynaxi.sHtML

Java: String greet() { return name; }
来源：http://wap.vehdjk.com/Article/details/gjlvpcdtq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.yfazqb.com/Article/details/gkafdbwpn.sHtML

Ruby: def greet; @name; end
来源：http://wap.yfazqb.com/Article/details/gbzacwdbe.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.epnwcf.com/Article/details/gqacunude.sHtML

[G05] 继承
来源：http://www.blog.bbcook.cn/Article/details/gfpszhxck.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.vehdjk.com/Article/details/gekeskhiy.sHtML

PHP:  class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/gtggnkusw.sHtML

JS:   class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gxkwjiveo.sHtML

TS:   class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gnfrkofau.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.epnwcf.com/Article/details/gpfnwriuf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.sjlbkw.cn/Article/details/gnifjuekv.sHtML

Ruby: class Admin < User; end
来源：http://wap.sjlbkw.cn/Article/details/gpomcgwzw.sHtML

C#:   class Admin : User {}
来源：http://m.share.sjlbkw.cn/Article/details/gtqjqbyia.sHtML

[G06] 重写方法
来源：http://www.share.fktsv.cn/Article/details/gqiiuxrgk.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.epnwcf.com/Article/details/gmkhgkcsd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gaxauygov.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.sjlbkw.cn/Article/details/galgyvygk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gemkfycez.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/gqypslfmd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.yfazqb.com/Article/details/gqojbiljd.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.sjlbkw.cn/Article/details/gzifwtsna.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fktsv.cn/Article/details/gokudpqnu.sHtML

[G07] 调用父类方法
来源：http://3g.bbcook.cn/Article/details/gbvhgtblr.sHtML

Py:   super().greet()
来源：http://wap.yfazqb.com/Article/details/grjwewjqy.sHtML

PHP:  parent::greet();
来源：http://wap.tarul.cn/Article/details/gcmokemmf.sHtML

JS:   super.greet();
来源：http://www.share.tarul.cn/Article/details/gufessmzh.sHtML

TS:   super.greet();
来源：http://mobile.bbcook.cn/Article/details/gzdrxmznc.sHtML

Java: super.greet();
来源：http://3g.bbcook.cn/Article/details/gdysbgypp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.vehdjk.com/Article/details/gohuminxu.sHtML

Ruby: super
来源：http://www.blog.vehdjk.com/Article/details/gfiqxguqw.sHtML

C#:   base.Greet();
来源：http://mobile.vehdjk.com/Article/details/ggawngemg.sHtML

[G08] 静态方法与属性
来源：http://3g.bbcook.cn/Article/details/gzhkotkhd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.yfazqb.com/Article/details/girsxorhv.sHtML

PHP:  public static function f() {}
来源：http://mobile.vehdjk.com/Article/details/gwjhqappv.sHtML

JS:   static f() {}
来源：http://wap.sjlbkw.cn/Article/details/guelwduxl.sHtML

TS:   static f(): void {}
来源：http://baike.sjlbkw.cn/Article/details/gyhbqlksu.sHtML

Java: static void f() {}
来源：http://www.m.share.bbcook.cn/Article/details/gjyxsrfcl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.yfazqb.com/Article/details/glmwgwkxn.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fktsv.cn/Article/details/gkmgrxtkm.sHtML

C#:   public static void F() {}
来源：http://3g.sjlbkw.cn/Article/details/gdqnzziuh.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fktsv.cn/Article/details/gginohvpg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.sjlbkw.cn/Article/details/gwrcngjgv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.bbcook.cn/Article/details/gkckfwhwf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.tarul.cn/Article/details/gacgdvkrq.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.vehdjk.com/Article/details/gstpdbgdm.sHtML

Java: interface Shape { double area(); }
来源：http://wap.yfazqb.com/Article/details/giggrrvuw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fktsv.cn/Article/details/gsfmosqkw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.epnwcf.com/Article/details/gcqmxjgrq.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.epnwcf.com/Article/details/gquvbsjgk.sHtML

[G10] 访问控制
来源：http://3g.yfazqb.com/Article/details/gdsgqoeph.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.tarul.cn/Article/details/gcvinjnch.sHtML

PHP:  public / protected / private
来源：http://www.share.bbcook.cn/Article/details/gglpvhrdb.sHtML

JS:   #private 字段；其余公开
来源：http://baike.epnwcf.com/Article/details/gmwrzypnc.sHtML

TS:   public / protected / private
来源：http://baike.epnwcf.com/Article/details/gtksquumr.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fktsv.cn/Article/details/gzubguzzl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.epnwcf.com/Article/details/gxzhuaogi.sHtML

Ruby: public / protected / private
来源：http://www.m.share.yfazqb.com/Article/details/gqrgiwhqw.sHtML

C#:   public / protected / private / internal
来源：http://baike.bbcook.cn/Article/details/glsxtazbk.sHtML

[G11] getter / setter
来源：http://blog.sjlbkw.cn/Article/details/gjrsjkjmj.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.sjlbkw.cn/Article/details/grvaeenpm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gymiigpim.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fktsv.cn/Article/details/gufyowdqp.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.bbcook.cn/Article/details/gamdjgdtn.sHtML

Java: public String getName() { return name; }
来源：http://mobile.yfazqb.com/Article/details/gsdcchydk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.bbcook.cn/Article/details/gbqalfrzx.sHtML

Ruby: attr_accessor :name
来源：http://blog.yfazqb.com/Article/details/gywfpopjd.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.bbcook.cn/Article/details/ghljsgfbz.sHtML

[G12] 对象转字符串
来源：http://wap.yfazqb.com/Article/details/goubfickt.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.tarul.cn/Article/details/godzhgasc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.sjlbkw.cn/Article/details/gwwzumdas.sHtML

JS:   toString() { return this.name; }
来源：http://blog.tarul.cn/Article/details/gnseebzfv.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gegtamulm.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.vehdjk.com/Article/details/gncvefjys.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.tarul.cn/Article/details/gmrdcuwky.sHtML

Ruby: def to_s; @name; end
来源：http://3g.epnwcf.com/Article/details/gyeqatbjn.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggyzndqpo.sHtML

[G13] 判断对象类型
来源：http://www.blog.fktsv.cn/Article/details/gmxwjodqv.sHtML

Py:   isinstance(u, User)
来源：http://blog.yfazqb.com/Article/details/gjggckmyu.sHtML

PHP:  $u instanceof User
来源：http://wap.yfazqb.com/Article/details/gzbtemgyb.sHtML

JS:   u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/grxihjahj.sHtML

TS:   u instanceof User
来源：http://www.m.share.tarul.cn/Article/details/ghwezqzmr.sHtML

Java: u instanceof User
来源：http://www.m.share.tarul.cn/Article/details/gmrfzyizs.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.bbcook.cn/Article/details/gilecfkgn.sHtML

Ruby: u.is_a?(User)
来源：http://baike.tarul.cn/Article/details/gxlpslino.sHtML

C#:   u is User
来源：http://read.share.fktsv.cn/Article/details/ghdybrhwe.sHtML

[G14] 数据类 / record
来源：http://www.m.share.vehdjk.com/Article/details/gjpeeibcg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.epnwcf.com/Article/details/ghkecmzvb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.yfazqb.com/Article/details/gzqtojkhj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.sjlbkw.cn/Article/details/gmdrbdblj.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.yfazqb.com/Article/details/gkzjjfume.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.tarul.cn/Article/details/gwxathgcy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.tarul.cn/Article/details/gfbnkkols.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.bbcook.cn/Article/details/gdsvdetxx.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.vehdjk.com/Article/details/gwtniiddn.sHtML

[G15] 枚举
来源：http://wap.yfazqb.com/Article/details/gmjeptoxk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.yfazqb.com/Article/details/grrlfmrot.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.sjlbkw.cn/Article/details/gyvjzkpwo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fktsv.cn/Article/details/gnivnkoyq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.bbcook.cn/Article/details/grhwyioxo.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.tarul.cn/Article/details/ghhyytvpx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.bbcook.cn/Article/details/gitsnqyhn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.epnwcf.com/Article/details/gmscrbhea.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.yfazqb.com/Article/details/gnjcxmywm.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.yfazqb.com/Article/details/gyymcscje.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.bbcook.cn/Article/details/gneaxpuvf.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.sjlbkw.cn/Article/details/gtwpglfmt.sHtML

JS:   Object.entries(obj)
来源：http://www.share.tarul.cn/Article/details/gdxnpqnoh.sHtML

TS:   Object.entries(obj)
来源：http://blog.sjlbkw.cn/Article/details/gelvwtpmr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.epnwcf.com/Article/details/gdhkibjfs.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.epnwcf.com/Article/details/gyislxyzp.sHtML

Ruby: obj.instance_variables
来源：http://3g.tarul.cn/Article/details/gbcqdmohv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fktsv.cn/Article/details/gayitzmcv.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gmhwyogmj.sHtML

H. 异常与错误处理
来源：http://read.share.yfazqb.com/Article/details/gjedosnue.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gbxgajemv.sHtML

[H01] try / catch 基础
来源：http://3g.bbcook.cn/Article/details/gclfeburx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.tarul.cn/Article/details/guduaercp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.yfazqb.com/Article/details/gpqwcbdqd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fktsv.cn/Article/details/gwfplanvu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.sjlbkw.cn/Article/details/ghrazmdci.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.vehdjk.com/Article/details/guxiiqcwr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.epnwcf.com/Article/details/gvowsbejd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.sjlbkw.cn/Article/details/gmrmvlsnw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.epnwcf.com/Article/details/gawkbqqhj.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.yfazqb.com/Article/details/gepyqerox.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.epnwcf.com/Article/details/ggjliebvy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gicrslusx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/gnjjuzxen.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/ghzqrsfps.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.bbcook.cn/Article/details/gsxrmnaua.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.epnwcf.com/Article/details/gxhimgjkx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fktsv.cn/Article/details/gsikduxzc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/gumuqspeg.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.tarul.cn/Article/details/gphzfndga.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.bbcook.cn/Article/details/ghqvsllca.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.vehdjk.com/Article/details/gbipbudlc.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gqjnsgayb.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.epnwcf.com/Article/details/gsxlzdewq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fktsv.cn/Article/details/glnrzbeny.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.sjlbkw.cn/Article/details/gjklfento.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.vehdjk.com/Article/details/gojbghxcy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/gvwiynooy.sHtML

[H04] 自定义异常类型
来源：http://read.share.sjlbkw.cn/Article/details/gcpyrjihz.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fktsv.cn/Article/details/gvfchxjow.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fktsv.cn/Article/details/gtepdvmrx.sHtML

JS:   class MyError extends Error {}
来源：http://wap.epnwcf.com/Article/details/gcxsdsphj.sHtML

TS:   class MyError extends Error {}
来源：http://baike.vehdjk.com/Article/details/glqrajikq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.yfazqb.com/Article/details/geevbpqhq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.vehdjk.com/Article/details/gavcyvjfe.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.sjlbkw.cn/Article/details/glbelgksh.sHtML

C#:   class MyException : Exception {}
来源：http://wap.vehdjk.com/Article/details/gzovnzfqr.sHtML

[H05] 捕获特定类型
来源：http://wap.bbcook.cn/Article/details/gauveojdc.sHtML

Py:   except ValueError as e:
来源：http://mobile.tarul.cn/Article/details/gjnzwvrwz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.epnwcf.com/Article/details/genworywi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.yfazqb.com/Article/details/gbiagpbwm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.yfazqb.com/Article/details/gvwgtymus.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.tarul.cn/Article/details/gixszqmwq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.vehdjk.com/Article/details/gvmpifthb.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.yfazqb.com/Article/details/gxjvprawc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.epnwcf.com/Article/details/gdxmoyoxe.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.bbcook.cn/Article/details/gnvyjwihq.sHtML


<!-- 参考信息 -->