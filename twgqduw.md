代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gvoalhwwk.sHtML

[F02] 逐行读取文件
来源：http://mobile.bbcook.cn/Article/details/gfdrefciw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.bbcook.cn/Article/details/gmcfzmlue.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.epnwcf.com/Article/details/gjdqljzjs.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.epnwcf.com/Article/details/gtieimjgj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.tarul.cn/Article/details/gcjjmehdv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.tarul.cn/Article/details/gqtiwrtrs.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.yfazqb.com/Article/details/glhgozsnh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.sjlbkw.cn/Article/details/glkksogjl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.epnwcf.com/Article/details/gvdiyxfim.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fktsv.cn/Article/details/gmdhhksnb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.bbcook.cn/Article/details/glcrcitgi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.yfazqb.com/Article/details/gqugdujzq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.yfazqb.com/Article/details/guozwfnnl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.yfazqb.com/Article/details/gdmwdlxdd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.sjlbkw.cn/Article/details/gdxnnnmne.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.vehdjk.com/Article/details/gxgonkhax.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.vehdjk.com/Article/details/gdkzjpcyb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fktsv.cn/Article/details/gjwzhhvvh.sHtML

[F04] 追加写入文件
来源：http://read.share.yfazqb.com/Article/details/gzvgprfyd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.sjlbkw.cn/Article/details/gqppgufou.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.yfazqb.com/Article/details/gqyxntjtu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.vehdjk.com/Article/details/gqyxtlrob.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.vehdjk.com/Article/details/gsnhfpgjj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.bbcook.cn/Article/details/gsqlvfasb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.bbcook.cn/Article/details/gxafiqaht.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.yfazqb.com/Article/details/gauwgpjgf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.sjlbkw.cn/Article/details/gabjszdew.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.bbcook.cn/Article/details/gykmabrcx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fktsv.cn/Article/details/ggfqrfvqb.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.epnwcf.com/Article/details/gxqfcqtnc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/geowqxfbu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gsgvvjgbc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/gewolgmuk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.vehdjk.com/Article/details/gynhbzpqh.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/grjxvfwok.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fktsv.cn/Article/details/gvvnoxnif.sHtML

[F06] 删除文件
来源：http://www.blog.fktsv.cn/Article/details/gjzpurwfn.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.tarul.cn/Article/details/gytgojmcp.sHtML

PHP:  unlink("a.txt");
来源：http://3g.bbcook.cn/Article/details/glhvgrnvb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/ghrrqiqxp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gtxfnlqhz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fktsv.cn/Article/details/gyrnyrzou.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.yfazqb.com/Article/details/gslulzfec.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fktsv.cn/Article/details/gcumjpnrx.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gcqxyumih.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.epnwcf.com/Article/details/gkgjzkrby.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.yfazqb.com/Article/details/gggrpadss.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.tarul.cn/Article/details/graaogxbh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.epnwcf.com/Article/details/ghhfowhnh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.bbcook.cn/Article/details/gxawxjdbi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fktsv.cn/Article/details/ghfvurpjw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.epnwcf.com/Article/details/gljejiovp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.bbcook.cn/Article/details/glvxkvbar.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.bbcook.cn/Article/details/getrsybto.sHtML

[F08] 遍历目录
来源：http://wap.epnwcf.com/Article/details/ggyoknwhf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.yfazqb.com/Article/details/gzkeohxus.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.epnwcf.com/Article/details/gnkuwtkfv.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.bbcook.cn/Article/details/gxuwincne.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fktsv.cn/Article/details/ghtnmwrcj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.sjlbkw.cn/Article/details/girbjgcwj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fktsv.cn/Article/details/gnkfoalen.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gpaisbgtx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.bbcook.cn/Article/details/gqachrsxk.sHtML

[F09] 获取文件大小
来源：http://baike.epnwcf.com/Article/details/gxtzadkwu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnzxjckiu.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gsbnnslcp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.epnwcf.com/Article/details/ghjontbue.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.bbcook.cn/Article/details/gcptbxbos.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gpzklnezz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.yfazqb.com/Article/details/gqnxscnqx.sHtML

Ruby: File.size("a.txt")
来源：http://baike.yfazqb.com/Article/details/gctrawoyo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.yfazqb.com/Article/details/gtgqsrrrz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.bbcook.cn/Article/details/gcgqosjra.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gerctajnf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.bbcook.cn/Article/details/geuqzjcvk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/gjhohussu.sHtML

TS:   path.extname("a.txt")
来源：http://wap.yfazqb.com/Article/details/gqsvrdwvg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.yfazqb.com/Article/details/ggvebpybl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gcbuekghv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gsdusuzyl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gcezjirym.sHtML

[F11] 复制与移动文件
来源：http://wap.yfazqb.com/Article/details/gjjbkqefo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/ggxpvlhdi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gnlsjqzcg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gzpkfsbvw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gfzwjlygm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.yfazqb.com/Article/details/gjqkggybw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.sjlbkw.cn/Article/details/gwjzivvuo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/guyibtnvt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fktsv.cn/Article/details/gqyvbjzlo.sHtML

[F12] CSV 读写
来源：http://wap.yfazqb.com/Article/details/gldzdwydg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.epnwcf.com/Article/details/ghcnglbiy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.vehdjk.com/Article/details/gtczaqyqa.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.sjlbkw.cn/Article/details/gnqnmutvh.sHtML

TS:   // 同上
来源：http://wap.vehdjk.com/Article/details/gsibmvhll.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.tarul.cn/Article/details/gegyurlff.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.vehdjk.com/Article/details/gnfpbomic.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.tarul.cn/Article/details/gytmhzipq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.epnwcf.com/Article/details/gauxiclyf.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gybcbaemb.sHtML

G. 面向对象
来源：http://www.blog.tarul.cn/Article/details/gtlycbbni.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/ghwqeybwz.sHtML

[G01] 定义类
来源：http://wap.fktsv.cn/Article/details/gyfodjpka.sHtML

Py:   class User: pass
来源：http://3g.yfazqb.com/Article/details/gjarqqtgz.sHtML

PHP:  class User {}
来源：http://wap.fktsv.cn/Article/details/gswykspsv.sHtML

JS:   class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gokkawkic.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.epnwcf.com/Article/details/gihvnogmb.sHtML

Java: class User {}
来源：http://mobile.fktsv.cn/Article/details/gjlkojraj.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.bbcook.cn/Article/details/guiyvflbh.sHtML

Ruby: class User; end
来源：http://wap.epnwcf.com/Article/details/gwcmfield.sHtML

C#:   class User {}
来源：http://wap.vehdjk.com/Article/details/gzxydeizu.sHtML

[G02] 构造函数
来源：http://www.m.share.yfazqb.com/Article/details/gnkuxsekk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.bbcook.cn/Article/details/grzuhhbqr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.yfazqb.com/Article/details/gyepjlzug.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.bbcook.cn/Article/details/gzjezzddu.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.bbcook.cn/Article/details/gztgrvame.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fktsv.cn/Article/details/gsfyrfqbp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.sjlbkw.cn/Article/details/gtgooivyt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.yfazqb.com/Article/details/gzbxymcqw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.sjlbkw.cn/Article/details/gfoajddei.sHtML

[G03] 实例属性
来源：http://wap.epnwcf.com/Article/details/gpizxkvuk.sHtML

Py:   self.name = "x"
来源：http://blog.sjlbkw.cn/Article/details/gfbblewcy.sHtML

PHP:  public string $name = "x";
来源：http://read.share.yfazqb.com/Article/details/gztvqiehx.sHtML

JS:   this.name = "x";
来源：http://wap.epnwcf.com/Article/details/ggjtphxut.sHtML

TS:   name: string = "x";
来源：http://read.share.fktsv.cn/Article/details/gkvqsjwoc.sHtML

Java: private String name;
来源：http://3g.bbcook.cn/Article/details/gpnomsgpt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fktsv.cn/Article/details/gbufautdt.sHtML

Ruby: @name = "x"
来源：http://3g.fktsv.cn/Article/details/gserratxe.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.epnwcf.com/Article/details/gwdxibvdj.sHtML

[G04] 定义方法
来源：http://blog.sjlbkw.cn/Article/details/gdbkiaeuw.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fktsv.cn/Article/details/glqmsjwzn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.sjlbkw.cn/Article/details/gkhwcyqqa.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.tarul.cn/Article/details/grqktlbad.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gplgxcarf.sHtML

Java: String greet() { return name; }
来源：http://www.share.tarul.cn/Article/details/gorbwcaeo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.epnwcf.com/Article/details/gcywpemcx.sHtML

Ruby: def greet; @name; end
来源：http://mobile.vehdjk.com/Article/details/gkipdkuym.sHtML

C#:   public string Greet() => Name;
来源：http://blog.tarul.cn/Article/details/gijqvnmyp.sHtML

[G05] 继承
来源：http://mobile.tarul.cn/Article/details/gkbhopqye.sHtML

Py:   class Admin(User): pass
来源：http://m.share.yfazqb.com/Article/details/gtuzrbwvu.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.epnwcf.com/Article/details/gdheuhpkv.sHtML

JS:   class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/gpxmqclhf.sHtML

TS:   class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/gerqkvcru.sHtML

Java: class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/gmjksmorq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.vehdjk.com/Article/details/gfqkpwzkj.sHtML

Ruby: class Admin < User; end
来源：http://mobile.epnwcf.com/Article/details/gywqwyafl.sHtML

C#:   class Admin : User {}
来源：http://blog.tarul.cn/Article/details/gelkgfnvd.sHtML

[G06] 重写方法
来源：http://3g.bbcook.cn/Article/details/grmgnxdob.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.tarul.cn/Article/details/gdnhopxsc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/gpudumpof.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fktsv.cn/Article/details/gvjjsbcwc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/gqaaqnjqs.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/gvxfjalns.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.tarul.cn/Article/details/gotpziuba.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.sjlbkw.cn/Article/details/gxxkoycze.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fktsv.cn/Article/details/gdwctqjto.sHtML

[G07] 调用父类方法
来源：http://www.share.epnwcf.com/Article/details/glxomvcch.sHtML

Py:   super().greet()
来源：http://www.m.share.fktsv.cn/Article/details/geqehmnkc.sHtML

PHP:  parent::greet();
来源：http://www.blog.fktsv.cn/Article/details/gwybhrryt.sHtML

JS:   super.greet();
来源：http://m.share.yfazqb.com/Article/details/guuqmhksr.sHtML

TS:   super.greet();
来源：http://www.share.fktsv.cn/Article/details/gwrfznsfw.sHtML

Java: super.greet();
来源：http://www.blog.vehdjk.com/Article/details/gyjmraqtr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.epnwcf.com/Article/details/gpttusvyr.sHtML

Ruby: super
来源：http://read.share.epnwcf.com/Article/details/gilthzelk.sHtML

C#:   base.Greet();
来源：http://wap.bbcook.cn/Article/details/gdnefwnma.sHtML

[G08] 静态方法与属性
来源：http://mobile.tarul.cn/Article/details/gbtmkriio.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fktsv.cn/Article/details/glgeuziaa.sHtML

PHP:  public static function f() {}
来源：http://mobile.fktsv.cn/Article/details/ggbbmcehg.sHtML

JS:   static f() {}
来源：http://read.share.tarul.cn/Article/details/getggmuve.sHtML

TS:   static f(): void {}
来源：http://mobile.vehdjk.com/Article/details/gybqrlajm.sHtML

Java: static void f() {}
来源：http://blog.epnwcf.com/Article/details/gnsgvqcxh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.tarul.cn/Article/details/gjrxkfhly.sHtML

Ruby: def self.f; end
来源：http://blog.epnwcf.com/Article/details/gpatdeltk.sHtML

C#:   public static void F() {}
来源：http://baike.sjlbkw.cn/Article/details/goqnkpzmu.sHtML

[G09] 接口 / 抽象类
来源：http://baike.tarul.cn/Article/details/gejvnjvcx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fktsv.cn/Article/details/gfppehwpz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.tarul.cn/Article/details/gofaejkth.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.epnwcf.com/Article/details/ggrvybnur.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.vehdjk.com/Article/details/gffgtiutq.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.vehdjk.com/Article/details/gvuiddfme.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.tarul.cn/Article/details/gforhzvfu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.tarul.cn/Article/details/gwwpjyhsk.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.yfazqb.com/Article/details/gjjchejot.sHtML

[G10] 访问控制
来源：http://3g.epnwcf.com/Article/details/gnyswnlya.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.epnwcf.com/Article/details/ggcqthfae.sHtML

PHP:  public / protected / private
来源：http://wap.epnwcf.com/Article/details/gfeomnzul.sHtML

JS:   #private 字段；其余公开
来源：http://blog.sjlbkw.cn/Article/details/gtnczmdcv.sHtML

TS:   public / protected / private
来源：http://www.share.vehdjk.com/Article/details/ghkpbkkkg.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fktsv.cn/Article/details/gpsynxzks.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.vehdjk.com/Article/details/gcswqdkdy.sHtML

Ruby: public / protected / private
来源：http://m.share.epnwcf.com/Article/details/ghrdflade.sHtML

C#:   public / protected / private / internal
来源：http://read.share.sjlbkw.cn/Article/details/gskansupz.sHtML

[G11] getter / setter
来源：http://mobile.vehdjk.com/Article/details/gsdnxlepl.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fktsv.cn/Article/details/glgycoqsy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.vehdjk.com/Article/details/gerndpkvd.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gmflrowph.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.sjlbkw.cn/Article/details/gwegdldaq.sHtML

Java: public String getName() { return name; }
来源：http://mobile.tarul.cn/Article/details/glmmplwef.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.yfazqb.com/Article/details/gstdbzlyd.sHtML

Ruby: attr_accessor :name
来源：http://wap.vehdjk.com/Article/details/geklozpyz.sHtML

C#:   public string Name { get; set; }
来源：http://wap.bbcook.cn/Article/details/gyntynkxs.sHtML

[G12] 对象转字符串
来源：http://m.share.epnwcf.com/Article/details/ghfrmszlv.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.sjlbkw.cn/Article/details/goaexegzk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gutpfoegp.sHtML

JS:   toString() { return this.name; }
来源：http://baike.yfazqb.com/Article/details/grohneljc.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gzbsseslb.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fktsv.cn/Article/details/ganotxscl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.tarul.cn/Article/details/gaefzhvfg.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.vehdjk.com/Article/details/gyhpmursn.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.tarul.cn/Article/details/gtpvoimzz.sHtML

[G13] 判断对象类型
来源：http://m.share.bbcook.cn/Article/details/gogfmkhzb.sHtML

Py:   isinstance(u, User)
来源：http://baike.yfazqb.com/Article/details/gvdbbhfgu.sHtML

PHP:  $u instanceof User
来源：http://m.share.vehdjk.com/Article/details/gqbqdwfbs.sHtML

JS:   u instanceof User
来源：http://baike.bbcook.cn/Article/details/gupuijukt.sHtML

TS:   u instanceof User
来源：http://m.share.epnwcf.com/Article/details/ghbalorvv.sHtML

Java: u instanceof User
来源：http://m.share.vehdjk.com/Article/details/gfjyrutdd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.vehdjk.com/Article/details/gzxejuooe.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.vehdjk.com/Article/details/ggomgfssm.sHtML

C#:   u is User
来源：http://mobile.vehdjk.com/Article/details/gdtuvabfn.sHtML

[G14] 数据类 / record
来源：http://baike.epnwcf.com/Article/details/gqmohvwjo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.yfazqb.com/Article/details/gdtkuncoz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.bbcook.cn/Article/details/gttkrmlsu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fktsv.cn/Article/details/gplosxbce.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.vehdjk.com/Article/details/ghoqogslg.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.epnwcf.com/Article/details/grggrnjvi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.bbcook.cn/Article/details/gczjlekaw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.yfazqb.com/Article/details/glrpmjlfi.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.tarul.cn/Article/details/gxemcofzc.sHtML

[G15] 枚举
来源：http://baike.epnwcf.com/Article/details/grkfodhew.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.vehdjk.com/Article/details/gxdudcjwt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.yfazqb.com/Article/details/gxudzvhfi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.tarul.cn/Article/details/gvxhvugsz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.epnwcf.com/Article/details/gkpaoeqdy.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.bbcook.cn/Article/details/gjftoanbu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.bbcook.cn/Article/details/gxedvhiio.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fktsv.cn/Article/details/gzlzpylbq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.epnwcf.com/Article/details/gceouhqfa.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fktsv.cn/Article/details/gxpwrcyeo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.bbcook.cn/Article/details/geomqupob.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.vehdjk.com/Article/details/grdotubnq.sHtML

JS:   Object.entries(obj)
来源：http://wap.bbcook.cn/Article/details/gzujspbez.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gzqedfbtr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.bbcook.cn/Article/details/gzjcabndo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.yfazqb.com/Article/details/gqnngflin.sHtML

Ruby: obj.instance_variables
来源：http://m.share.tarul.cn/Article/details/gocutmhco.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.tarul.cn/Article/details/gmwbfmksk.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/ghuvfqzxd.sHtML

H. 异常与错误处理
来源：http://www.blog.yfazqb.com/Article/details/gguntecyr.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gningqtys.sHtML

[H01] try / catch 基础
来源：http://wap.yfazqb.com/Article/details/ghdigoimq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.epnwcf.com/Article/details/gjeakpwxj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.epnwcf.com/Article/details/gmejlqvqn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.yfazqb.com/Article/details/grddqaahr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.bbcook.cn/Article/details/gcdkkqgaw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.tarul.cn/Article/details/gqolxfhvo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.yfazqb.com/Article/details/gekyvcwwo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.epnwcf.com/Article/details/grcbqtddf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.epnwcf.com/Article/details/gcojprdtb.sHtML

[H02] finally / ensure 收尾
来源：http://3g.sjlbkw.cn/Article/details/guluhcmmh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.sjlbkw.cn/Article/details/gxawrnilk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.epnwcf.com/Article/details/gutqjtgvy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/grwsytanb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.epnwcf.com/Article/details/goaikchrf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.bbcook.cn/Article/details/gotguflaf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.epnwcf.com/Article/details/geubfcqmy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.bbcook.cn/Article/details/gjbfnnwdb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fktsv.cn/Article/details/glofithcm.sHtML

[H03] 主动抛出异常
来源：http://m.share.fktsv.cn/Article/details/gzzxfogpa.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fktsv.cn/Article/details/gipgwdwwa.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.tarul.cn/Article/details/gmfmuhfin.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.epnwcf.com/Article/details/gpoakfbsg.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gkioibsyj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gsxyacvsu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.bbcook.cn/Article/details/gtoxqeyod.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.sjlbkw.cn/Article/details/gmztzazzi.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gwznxxeyq.sHtML

[H04] 自定义异常类型
来源：http://blog.yfazqb.com/Article/details/gcwsvqabb.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.bbcook.cn/Article/details/gozqnccth.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.sjlbkw.cn/Article/details/gvaoupxew.sHtML

JS:   class MyError extends Error {}
来源：http://3g.bbcook.cn/Article/details/ghknujdiz.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.epnwcf.com/Article/details/gkzevstfx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.epnwcf.com/Article/details/gbrxzcqtb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.yfazqb.com/Article/details/giuycgcbi.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.yfazqb.com/Article/details/gmtvfywdm.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.bbcook.cn/Article/details/gnepmgozv.sHtML

[H05] 捕获特定类型
来源：http://m.share.vehdjk.com/Article/details/gjmlwcjbs.sHtML

Py:   except ValueError as e:
来源：http://m.share.fktsv.cn/Article/details/gtgkoutjo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.yfazqb.com/Article/details/gczizmlhg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.epnwcf.com/Article/details/gkxmygyaj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fktsv.cn/Article/details/gblfxwmrl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.epnwcf.com/Article/details/gjggaisdw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.tarul.cn/Article/details/ghkwmvblr.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.bbcook.cn/Article/details/gikfofkja.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.vehdjk.com/Article/details/gsmkiwctm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.vehdjk.com/Article/details/gbndcphse.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.tarul.cn/Article/details/gnvollyyf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.vehdjk.com/Article/details/gunbattsa.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.vehdjk.com/Article/details/gonrotxsl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.vehdjk.com/Article/details/gzhkksoca.sHtML


<!-- 参考信息 -->