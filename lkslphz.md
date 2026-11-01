代发 wailian999

[F01] 读取整个文件
来源：http://m.share.sjlbkw.cn/Article/details/gbzxyliut.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.vehdjk.com/Article/details/gkguquxkm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gamtjuzep.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.vehdjk.com/Article/details/gxzpvacex.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.epnwcf.com/Article/details/gmapvohzi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.epnwcf.com/Article/details/gqodnhvuf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fktsv.cn/Article/details/gfjmcsdkm.sHtML

Ruby: File.read("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gvtwsaoql.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.bbcook.cn/Article/details/gcubvqokz.sHtML

[F02] 逐行读取文件
来源：http://baike.epnwcf.com/Article/details/gltddpbjl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.epnwcf.com/Article/details/gpesdttsr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.tarul.cn/Article/details/gzbkqhqbh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.epnwcf.com/Article/details/gbkwvtvuk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.bbcook.cn/Article/details/gcolopkml.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.yfazqb.com/Article/details/gbawbzfgh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.tarul.cn/Article/details/gjegchpuz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.sjlbkw.cn/Article/details/gvxzoxpgx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.epnwcf.com/Article/details/grebamqoj.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.sjlbkw.cn/Article/details/gzwwzwfae.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.sjlbkw.cn/Article/details/gngswsfxm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.sjlbkw.cn/Article/details/gtzenpdxf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.epnwcf.com/Article/details/gxmzgojic.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.bbcook.cn/Article/details/guaajkgdk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.bbcook.cn/Article/details/gualklevh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.yfazqb.com/Article/details/gsknumrqz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fktsv.cn/Article/details/gynelmwty.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.bbcook.cn/Article/details/gssmpoenb.sHtML

[F04] 追加写入文件
来源：http://read.share.epnwcf.com/Article/details/gwzwuijih.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.yfazqb.com/Article/details/ghbszamft.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.tarul.cn/Article/details/gmiaosyou.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.yfazqb.com/Article/details/graciyszn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fktsv.cn/Article/details/guiltikke.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.yfazqb.com/Article/details/gxibdvbli.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.epnwcf.com/Article/details/gdkioumvy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.tarul.cn/Article/details/gvzoohtba.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.sjlbkw.cn/Article/details/gppnredfw.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.sjlbkw.cn/Article/details/gqsxceyuy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.vehdjk.com/Article/details/gcnlrodff.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gfnlomqll.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gzokdpias.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/gavxwnunj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.vehdjk.com/Article/details/grvermnqa.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.epnwcf.com/Article/details/gshzcakoa.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gmjyfnjwo.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/glxxwicli.sHtML

[F06] 删除文件
来源：http://www.m.share.bbcook.cn/Article/details/gpkcoaqzy.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gynikobxx.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gzfpwinze.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gfqdpyaxv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/gusjoxkqu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.epnwcf.com/Article/details/ggnpisarc.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gqgxogwea.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.yfazqb.com/Article/details/gruksdlqp.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gxyiwplky.sHtML

[F07] 创建目录（含多级）
来源：http://3g.vehdjk.com/Article/details/gwfznzijn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.bbcook.cn/Article/details/gfknckwrg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.yfazqb.com/Article/details/gacebxkuo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.yfazqb.com/Article/details/gdhmncgih.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.vehdjk.com/Article/details/gjrwknmon.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.sjlbkw.cn/Article/details/gdjgjybcd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.yfazqb.com/Article/details/gpjbqbydz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.vehdjk.com/Article/details/gypwmjgmh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.yfazqb.com/Article/details/gakifezjw.sHtML

[F08] 遍历目录
来源：http://m.share.yfazqb.com/Article/details/gegejsfgz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.yfazqb.com/Article/details/gnaqynhsg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.yfazqb.com/Article/details/gwpszfwpk.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fktsv.cn/Article/details/gwzbjtljl.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/gbyvksfnf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.epnwcf.com/Article/details/gcogbiuec.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.epnwcf.com/Article/details/gsqlrdvok.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.bbcook.cn/Article/details/gqnyjpcot.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fktsv.cn/Article/details/gslvvnqpq.sHtML

[F09] 获取文件大小
来源：http://3g.yfazqb.com/Article/details/gsnatroww.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.vehdjk.com/Article/details/glbfgrrbv.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fktsv.cn/Article/details/gopucwrmx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.yfazqb.com/Article/details/gpvuavizb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fktsv.cn/Article/details/gnjhwrwgn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.sjlbkw.cn/Article/details/gfvpmmhgt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.epnwcf.com/Article/details/gisdqydea.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.tarul.cn/Article/details/gokmzufza.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.tarul.cn/Article/details/gidttfroi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.bbcook.cn/Article/details/gvqmfivft.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/gvlthqhle.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.vehdjk.com/Article/details/glhtbsxuw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/goueabgpd.sHtML

TS:   path.extname("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gjqnhrdyg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.sjlbkw.cn/Article/details/gqnocxpfw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/ggasclolw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/gnkjvnzge.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/gsgjleuff.sHtML

[F11] 复制与移动文件
来源：http://m.share.epnwcf.com/Article/details/gaadbxxtv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gozgscjpp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.epnwcf.com/Article/details/gaqqbdedn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/gzclpwzcw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/glbwzgrqo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fktsv.cn/Article/details/gipubirce.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.vehdjk.com/Article/details/gpqtqfxmc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/gfyhspxit.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.bbcook.cn/Article/details/gsrtovkad.sHtML

[F12] CSV 读写
来源：http://3g.fktsv.cn/Article/details/ghgwruzad.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.sjlbkw.cn/Article/details/ggwcgwnup.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.bbcook.cn/Article/details/gefvushho.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.tarul.cn/Article/details/ghzahauyl.sHtML

TS:   // 同上
来源：http://mobile.tarul.cn/Article/details/gokyphzql.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.vehdjk.com/Article/details/gpbaxjsih.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fktsv.cn/Article/details/gbaecpsgi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.bbcook.cn/Article/details/gdxbeuxzc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.bbcook.cn/Article/details/gsplsazmf.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gblmnqyvb.sHtML

G. 面向对象
来源：http://wap.tarul.cn/Article/details/gbtotoorq.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gigopbjdb.sHtML

[G01] 定义类
来源：http://read.share.sjlbkw.cn/Article/details/ghmulyvjr.sHtML

Py:   class User: pass
来源：http://www.share.yfazqb.com/Article/details/ggxwovqvq.sHtML

PHP:  class User {}
来源：http://read.share.epnwcf.com/Article/details/grligpifd.sHtML

JS:   class User {}
来源：http://blog.vehdjk.com/Article/details/gxghkobph.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.bbcook.cn/Article/details/gozzzgwmw.sHtML

Java: class User {}
来源：http://www.blog.tarul.cn/Article/details/glusqgqfy.sHtML

Go:   type User struct { Name string }
来源：http://blog.fktsv.cn/Article/details/gifmtbzid.sHtML

Ruby: class User; end
来源：http://wap.epnwcf.com/Article/details/gfrkissst.sHtML

C#:   class User {}
来源：http://blog.sjlbkw.cn/Article/details/gdcteqduo.sHtML

[G02] 构造函数
来源：http://3g.epnwcf.com/Article/details/gpuwazzyf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.sjlbkw.cn/Article/details/gzaeedvee.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.sjlbkw.cn/Article/details/giqoqhmwc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.yfazqb.com/Article/details/guuagmcgj.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.epnwcf.com/Article/details/gttsplnxy.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.vehdjk.com/Article/details/giroxdxpb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fktsv.cn/Article/details/gepazyrch.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fktsv.cn/Article/details/gsemxbqcd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.bbcook.cn/Article/details/gnkxubgnb.sHtML

[G03] 实例属性
来源：http://3g.vehdjk.com/Article/details/gdnnrloab.sHtML

Py:   self.name = "x"
来源：http://www.share.yfazqb.com/Article/details/gbejhprzr.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fktsv.cn/Article/details/gtddlirlg.sHtML

JS:   this.name = "x";
来源：http://baike.epnwcf.com/Article/details/goaeasqhr.sHtML

TS:   name: string = "x";
来源：http://m.share.vehdjk.com/Article/details/gwporpbra.sHtML

Java: private String name;
来源：http://www.m.share.epnwcf.com/Article/details/grojhmvck.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.epnwcf.com/Article/details/gieihgnql.sHtML

Ruby: @name = "x"
来源：http://baike.bbcook.cn/Article/details/gbyhxvydo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fktsv.cn/Article/details/gjxnuprmr.sHtML

[G04] 定义方法
来源：http://read.share.vehdjk.com/Article/details/guislkwqr.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.epnwcf.com/Article/details/gpdnuwdrh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.yfazqb.com/Article/details/ghheqddiu.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/gperrhlwe.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gyuaraycb.sHtML

Java: String greet() { return name; }
来源：http://3g.fktsv.cn/Article/details/gesdukbbj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/gqttlizem.sHtML

Ruby: def greet; @name; end
来源：http://mobile.vehdjk.com/Article/details/gizlpakne.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.tarul.cn/Article/details/gktuckiur.sHtML

[G05] 继承
来源：http://wap.epnwcf.com/Article/details/glujnljrp.sHtML

Py:   class Admin(User): pass
来源：http://mobile.tarul.cn/Article/details/gohwhoufp.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gcmzcbhzu.sHtML

JS:   class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/gfmaxnxtd.sHtML

TS:   class Admin extends User {}
来源：http://www.share.sjlbkw.cn/Article/details/gwhgvhehu.sHtML

Java: class Admin extends User {}
来源：http://www.share.yfazqb.com/Article/details/gomdhdlhz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.vehdjk.com/Article/details/gezvkbxwp.sHtML

Ruby: class Admin < User; end
来源：http://wap.tarul.cn/Article/details/gyeqqjcpk.sHtML

C#:   class Admin : User {}
来源：http://blog.fktsv.cn/Article/details/gterbipqr.sHtML

[G06] 重写方法
来源：http://blog.yfazqb.com/Article/details/gkqbulkxf.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.yfazqb.com/Article/details/gcanxflqo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/gtpvhivwi.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/glufwyeol.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gwzeencpr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/gospyundq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.sjlbkw.cn/Article/details/ghmqfynuk.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.bbcook.cn/Article/details/ggizjtbtk.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.bbcook.cn/Article/details/groszstno.sHtML

[G07] 调用父类方法
来源：http://read.share.fktsv.cn/Article/details/gfhwhqvzj.sHtML

Py:   super().greet()
来源：http://baike.bbcook.cn/Article/details/gjaylxauf.sHtML

PHP:  parent::greet();
来源：http://read.share.yfazqb.com/Article/details/gokzkfedp.sHtML

JS:   super.greet();
来源：http://read.share.sjlbkw.cn/Article/details/gnuvpeboa.sHtML

TS:   super.greet();
来源：http://m.share.tarul.cn/Article/details/giknjzqtp.sHtML

Java: super.greet();
来源：http://m.share.tarul.cn/Article/details/ghgrxeted.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.vehdjk.com/Article/details/gjhivilxd.sHtML

Ruby: super
来源：http://blog.yfazqb.com/Article/details/gifjrjhtp.sHtML

C#:   base.Greet();
来源：http://www.blog.fktsv.cn/Article/details/gtjlpxwut.sHtML

[G08] 静态方法与属性
来源：http://www.share.fktsv.cn/Article/details/gllzaivzl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.epnwcf.com/Article/details/gecemebyf.sHtML

PHP:  public static function f() {}
来源：http://www.share.yfazqb.com/Article/details/gzpmtgmme.sHtML

JS:   static f() {}
来源：http://www.blog.epnwcf.com/Article/details/gwkftbeqs.sHtML

TS:   static f(): void {}
来源：http://mobile.vehdjk.com/Article/details/gqwsnluav.sHtML

Java: static void f() {}
来源：http://www.share.fktsv.cn/Article/details/glasverzp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.tarul.cn/Article/details/gebmeysvq.sHtML

Ruby: def self.f; end
来源：http://3g.vehdjk.com/Article/details/ghwqujfgs.sHtML

C#:   public static void F() {}
来源：http://www.m.share.vehdjk.com/Article/details/gnizyfqcg.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fktsv.cn/Article/details/guywjvaju.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.yfazqb.com/Article/details/gocijqewz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.bbcook.cn/Article/details/gnmxnrara.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.bbcook.cn/Article/details/gfjujehyd.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.tarul.cn/Article/details/ggnkzsjfc.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.tarul.cn/Article/details/gsmwytrja.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.yfazqb.com/Article/details/gkbxlyrav.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.epnwcf.com/Article/details/gifkzeohk.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.bbcook.cn/Article/details/glezhdykl.sHtML

[G10] 访问控制
来源：http://wap.sjlbkw.cn/Article/details/goepbtwni.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.sjlbkw.cn/Article/details/gqpnfielo.sHtML

PHP:  public / protected / private
来源：http://m.share.sjlbkw.cn/Article/details/gbhzfkgdr.sHtML

JS:   #private 字段；其余公开
来源：http://baike.yfazqb.com/Article/details/gnfkatnpw.sHtML

TS:   public / protected / private
来源：http://www.share.yfazqb.com/Article/details/gidpxvlgv.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.yfazqb.com/Article/details/gtkhdzlmb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.epnwcf.com/Article/details/gexrsksux.sHtML

Ruby: public / protected / private
来源：http://www.share.bbcook.cn/Article/details/gkdqhxcnt.sHtML

C#:   public / protected / private / internal
来源：http://3g.sjlbkw.cn/Article/details/gbbtjjpzg.sHtML

[G11] getter / setter
来源：http://read.share.bbcook.cn/Article/details/gvyugyzsx.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.bbcook.cn/Article/details/gzekexxbj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.vehdjk.com/Article/details/guphjwvsn.sHtML

JS:   get name() { return this._name; }
来源：http://3g.yfazqb.com/Article/details/gajhxkofn.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gatvbctlw.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/gyxdvfbpf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.vehdjk.com/Article/details/gaypxrmcm.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fktsv.cn/Article/details/gluqgalui.sHtML

C#:   public string Name { get; set; }
来源：http://blog.sjlbkw.cn/Article/details/gzcmsfywv.sHtML

[G12] 对象转字符串
来源：http://3g.bbcook.cn/Article/details/gmgjxizqa.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.epnwcf.com/Article/details/gvlhbebyu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/gpreyljhc.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.bbcook.cn/Article/details/gxdsirxrz.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fktsv.cn/Article/details/gwwoxipjy.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.epnwcf.com/Article/details/gfdumxlck.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fktsv.cn/Article/details/gvirwagjm.sHtML

Ruby: def to_s; @name; end
来源：http://blog.bbcook.cn/Article/details/geiyqukvo.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.bbcook.cn/Article/details/gfypsgusd.sHtML

[G13] 判断对象类型
来源：http://3g.tarul.cn/Article/details/gzejqhlnk.sHtML

Py:   isinstance(u, User)
来源：http://baike.fktsv.cn/Article/details/gmeanafcb.sHtML

PHP:  $u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gyollowni.sHtML

JS:   u instanceof User
来源：http://mobile.vehdjk.com/Article/details/gwytkriem.sHtML

TS:   u instanceof User
来源：http://m.share.yfazqb.com/Article/details/geyuqynag.sHtML

Java: u instanceof User
来源：http://m.share.fktsv.cn/Article/details/grwuneukd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.epnwcf.com/Article/details/gzvugjovk.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.bbcook.cn/Article/details/gbhixbdca.sHtML

C#:   u is User
来源：http://www.blog.bbcook.cn/Article/details/guimtbfeq.sHtML

[G14] 数据类 / record
来源：http://3g.fktsv.cn/Article/details/gihhcvvpl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.epnwcf.com/Article/details/gcnngzhje.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.bbcook.cn/Article/details/gnfehkbxq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fktsv.cn/Article/details/gnbozhxxw.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.bbcook.cn/Article/details/gekfuxtfg.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.epnwcf.com/Article/details/gjzbjxafz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.sjlbkw.cn/Article/details/gbyovtgpk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.vehdjk.com/Article/details/gkhedurmi.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.vehdjk.com/Article/details/gknhlnbxi.sHtML

[G15] 枚举
来源：http://www.m.share.vehdjk.com/Article/details/gnpjsxxgp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.tarul.cn/Article/details/gsbsrkiju.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.yfazqb.com/Article/details/gqsauumxp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.epnwcf.com/Article/details/gwlsgjmhy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.yfazqb.com/Article/details/gzesdnfmh.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fktsv.cn/Article/details/gttsunaxp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.epnwcf.com/Article/details/gehtgmylb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.tarul.cn/Article/details/gtyhvxajt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.yfazqb.com/Article/details/gnytorqha.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.tarul.cn/Article/details/gbdraapbb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.bbcook.cn/Article/details/gevrxpryo.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.sjlbkw.cn/Article/details/gfxuqalaj.sHtML

JS:   Object.entries(obj)
来源：http://wap.epnwcf.com/Article/details/gykyxxopz.sHtML

TS:   Object.entries(obj)
来源：http://baike.fktsv.cn/Article/details/gdocprjgw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.tarul.cn/Article/details/gxzpluzkh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fktsv.cn/Article/details/gclyiqook.sHtML

Ruby: obj.instance_variables
来源：http://www.share.bbcook.cn/Article/details/gbwgigfkn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.tarul.cn/Article/details/glqhzmast.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gqyslpsij.sHtML

H. 异常与错误处理
来源：http://baike.yfazqb.com/Article/details/gsqbquaxg.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gvepcqkgr.sHtML

[H01] try / catch 基础
来源：http://www.share.bbcook.cn/Article/details/ggwoefyhc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.vehdjk.com/Article/details/grodaxxsz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.tarul.cn/Article/details/gqtnvobxl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fktsv.cn/Article/details/gbqyqzlvw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.sjlbkw.cn/Article/details/gjexfvbep.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.sjlbkw.cn/Article/details/gtzngbpqq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.yfazqb.com/Article/details/gduednylj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.epnwcf.com/Article/details/gzgtglvsz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.bbcook.cn/Article/details/gfzkpeajk.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.bbcook.cn/Article/details/gzpqxdprt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.vehdjk.com/Article/details/gmpgagcir.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gauojdfht.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gexlpavhu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gxjebbsvd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gjkccvfcq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.epnwcf.com/Article/details/ggieerexh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.bbcook.cn/Article/details/glfwrvrof.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gfkcbzfvf.sHtML

[H03] 主动抛出异常
来源：http://m.share.tarul.cn/Article/details/gqckstxvc.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.tarul.cn/Article/details/ghydhlbld.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/gxkcbsftn.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fktsv.cn/Article/details/ghsvtpvzn.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.bbcook.cn/Article/details/gcstkalaq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.yfazqb.com/Article/details/gqvzltoja.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fktsv.cn/Article/details/gdscyvoog.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.tarul.cn/Article/details/grzkwcybu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/gdgfaqxjr.sHtML

[H04] 自定义异常类型
来源：http://wap.tarul.cn/Article/details/gphpbaluh.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.tarul.cn/Article/details/glwpjgbpw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.tarul.cn/Article/details/giyaxbddd.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fktsv.cn/Article/details/gpgljzdal.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.bbcook.cn/Article/details/gbyweyyta.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.epnwcf.com/Article/details/glzhfavvy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fktsv.cn/Article/details/gifjzeggj.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fktsv.cn/Article/details/gbnrlxxah.sHtML

C#:   class MyException : Exception {}
来源：http://baike.epnwcf.com/Article/details/gyqhwmkss.sHtML

[H05] 捕获特定类型
来源：http://blog.vehdjk.com/Article/details/gwjhpirmk.sHtML

Py:   except ValueError as e:
来源：http://blog.tarul.cn/Article/details/graltvrpj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.yfazqb.com/Article/details/gjoukkplm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.tarul.cn/Article/details/gpzcttpmi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.epnwcf.com/Article/details/gczasmpsb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fktsv.cn/Article/details/gxwpydzec.sHtML


<!-- 参考信息 -->