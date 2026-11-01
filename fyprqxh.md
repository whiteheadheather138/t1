代发 wailian999

[F01] 读取整个文件
来源：http://3g.sjlbkw.cn/Article/details/gupasvgex.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fktsv.cn/Article/details/gxosrnajc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gcwtpddsh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fktsv.cn/Article/details/gdojvgxtw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.epnwcf.com/Article/details/gxpnkupmd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gsdgdpplf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.yfazqb.com/Article/details/grjmbzjro.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gfjihljco.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.vehdjk.com/Article/details/grmxuhcnw.sHtML

[F02] 逐行读取文件
来源：http://blog.sjlbkw.cn/Article/details/gqfnuaexr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.bbcook.cn/Article/details/gdazxnyon.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fktsv.cn/Article/details/gnbfnofsp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fktsv.cn/Article/details/gzmtzdsvs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.bbcook.cn/Article/details/gmwvtdkxz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkixjhehs.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.vehdjk.com/Article/details/gnrkxiyba.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.yfazqb.com/Article/details/gnttxnxlv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.vehdjk.com/Article/details/ghwljnrlj.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.tarul.cn/Article/details/gudjtkfxl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.yfazqb.com/Article/details/gprxlelmj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fktsv.cn/Article/details/goithmuxi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.bbcook.cn/Article/details/gnhkpyfvm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.vehdjk.com/Article/details/ggnnceqgo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.yfazqb.com/Article/details/genacncok.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.vehdjk.com/Article/details/ghefoclxa.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.vehdjk.com/Article/details/gyixurwiu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.sjlbkw.cn/Article/details/gphenzqfr.sHtML

[F04] 追加写入文件
来源：http://www.share.epnwcf.com/Article/details/gfbfuqhmx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.vehdjk.com/Article/details/givvuqiuo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.tarul.cn/Article/details/ggtptqnyd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fktsv.cn/Article/details/gdvstwtss.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gjjkcksuv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.epnwcf.com/Article/details/gfegdvdlr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.epnwcf.com/Article/details/gmstagfqe.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.tarul.cn/Article/details/gkvjezrdl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.tarul.cn/Article/details/gjzuljhnx.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.yfazqb.com/Article/details/gzssqjfrw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.vehdjk.com/Article/details/gwbjapktk.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gyzktkcan.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/ggxjbmcll.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gnnchxlsv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.epnwcf.com/Article/details/grzzqzmyo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.yfazqb.com/Article/details/gtjstunag.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fktsv.cn/Article/details/gbvzhevzg.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gpihlcuxa.sHtML

[F06] 删除文件
来源：http://www.share.epnwcf.com/Article/details/gcylgdcft.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.tarul.cn/Article/details/giuplvkqg.sHtML

PHP:  unlink("a.txt");
来源：http://wap.tarul.cn/Article/details/gmwketegt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gxrduvotq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gwijxsphe.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/ghvslkpjz.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.tarul.cn/Article/details/gfhmrpjqp.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fktsv.cn/Article/details/gdnmtaeox.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gdsxvkqiz.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.yfazqb.com/Article/details/gnumbgnzu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.yfazqb.com/Article/details/gqtlnpwth.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.vehdjk.com/Article/details/gjlaixieh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.epnwcf.com/Article/details/gikazvgmv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.vehdjk.com/Article/details/glkmvidjw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.bbcook.cn/Article/details/gcckwmpdg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.vehdjk.com/Article/details/gwevpzggq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.epnwcf.com/Article/details/gxrsjrfwv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.sjlbkw.cn/Article/details/gbbsupsfy.sHtML

[F08] 遍历目录
来源：http://3g.vehdjk.com/Article/details/gktzginaj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fktsv.cn/Article/details/gaxmixdud.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.bbcook.cn/Article/details/glmqrfuyk.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.vehdjk.com/Article/details/gcdpgyzuy.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fktsv.cn/Article/details/gdspoeeog.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.vehdjk.com/Article/details/ghfveijbs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fktsv.cn/Article/details/gtertoinz.sHtML

Ruby: Dir.children("dir")
来源：http://baike.tarul.cn/Article/details/gpkggzptr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.yfazqb.com/Article/details/gpxxpmbww.sHtML

[F09] 获取文件大小
来源：http://m.share.sjlbkw.cn/Article/details/gnybjalyl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gzrfctaql.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gtiejkczv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.tarul.cn/Article/details/gqyoyxvxp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.tarul.cn/Article/details/glcpyuhtq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gjcznntox.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fktsv.cn/Article/details/gqhtkdyet.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/grzrxzczu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.tarul.cn/Article/details/gvvygsper.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.bbcook.cn/Article/details/geayqvgbx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gyuafkqti.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.sjlbkw.cn/Article/details/griajjpbe.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gmsclepny.sHtML

TS:   path.extname("a.txt")
来源：http://blog.bbcook.cn/Article/details/gehlehakq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.bbcook.cn/Article/details/gppopbejv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gjbbicvll.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gluklscuz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gizznqpos.sHtML

[F11] 复制与移动文件
来源：http://wap.bbcook.cn/Article/details/geafiayfw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gwhjnnnhi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fktsv.cn/Article/details/gxgkskmdr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.epnwcf.com/Article/details/gmxcdmqxs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/gpczqgkla.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.yfazqb.com/Article/details/gsvvsemej.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.sjlbkw.cn/Article/details/grzgxreqz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.bbcook.cn/Article/details/gaxeoikly.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.yfazqb.com/Article/details/gihwattkx.sHtML

[F12] CSV 读写
来源：http://blog.bbcook.cn/Article/details/gqhrkhflv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.sjlbkw.cn/Article/details/ggdamwnro.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.yfazqb.com/Article/details/gmmkravfg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.yfazqb.com/Article/details/gazrtlhtq.sHtML

TS:   // 同上
来源：http://mobile.vehdjk.com/Article/details/gpqxfivap.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.vehdjk.com/Article/details/galiivvxn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.epnwcf.com/Article/details/ghhzdtkis.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.bbcook.cn/Article/details/gflxvaeff.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.bbcook.cn/Article/details/gcraennaj.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gemihagxg.sHtML

G. 面向对象
来源：http://3g.fktsv.cn/Article/details/gkromkrbq.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gdlwriqfd.sHtML

[G01] 定义类
来源：http://wap.vehdjk.com/Article/details/glzoxpykg.sHtML

Py:   class User: pass
来源：http://www.m.share.fktsv.cn/Article/details/gumamlrvx.sHtML

PHP:  class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gznakclrv.sHtML

JS:   class User {}
来源：http://wap.fktsv.cn/Article/details/gykvglhux.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.epnwcf.com/Article/details/gcnvwhrxk.sHtML

Java: class User {}
来源：http://wap.vehdjk.com/Article/details/gtocyzkwp.sHtML

Go:   type User struct { Name string }
来源：http://mobile.bbcook.cn/Article/details/gkzuvckvt.sHtML

Ruby: class User; end
来源：http://3g.yfazqb.com/Article/details/gwrflvbrd.sHtML

C#:   class User {}
来源：http://m.share.yfazqb.com/Article/details/gapibnpty.sHtML

[G02] 构造函数
来源：http://m.share.sjlbkw.cn/Article/details/gatqftjkm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.vehdjk.com/Article/details/gdxdwtjpr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fktsv.cn/Article/details/gmxwrhyda.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.epnwcf.com/Article/details/gdwuuizqp.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.bbcook.cn/Article/details/gwwqbhxut.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.bbcook.cn/Article/details/gqzywjiup.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.epnwcf.com/Article/details/gtjiilbqa.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.bbcook.cn/Article/details/gkluqvrlv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.epnwcf.com/Article/details/gewyydflp.sHtML

[G03] 实例属性
来源：http://blog.epnwcf.com/Article/details/glbbjwsfb.sHtML

Py:   self.name = "x"
来源：http://www.share.bbcook.cn/Article/details/gngyqdueb.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fktsv.cn/Article/details/gwfbryall.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fktsv.cn/Article/details/grzqmpdts.sHtML

TS:   name: string = "x";
来源：http://read.share.epnwcf.com/Article/details/gmbjxurla.sHtML

Java: private String name;
来源：http://mobile.tarul.cn/Article/details/gmjwrzgup.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fktsv.cn/Article/details/gqbgkenzb.sHtML

Ruby: @name = "x"
来源：http://read.share.yfazqb.com/Article/details/guapwmahz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.vehdjk.com/Article/details/ggzswljwz.sHtML

[G04] 定义方法
来源：http://read.share.vehdjk.com/Article/details/gtzypdvia.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fktsv.cn/Article/details/gkcbiubow.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fktsv.cn/Article/details/gpkhqrlen.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/glxnbmjxw.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fktsv.cn/Article/details/gfohvbvzt.sHtML

Java: String greet() { return name; }
来源：http://www.share.tarul.cn/Article/details/gvumyftmu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.tarul.cn/Article/details/gxscqpthe.sHtML

Ruby: def greet; @name; end
来源：http://baike.sjlbkw.cn/Article/details/gadekfjou.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.epnwcf.com/Article/details/gnlrxeicr.sHtML

[G05] 继承
来源：http://blog.yfazqb.com/Article/details/gytwreuxf.sHtML

Py:   class Admin(User): pass
来源：http://baike.yfazqb.com/Article/details/gmrjhqnxt.sHtML

PHP:  class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/godtwbxtb.sHtML

JS:   class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gvrxjdcoz.sHtML

TS:   class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/ghgcgsrah.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/gbppsmzhe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.yfazqb.com/Article/details/grpaeuhtw.sHtML

Ruby: class Admin < User; end
来源：http://www.share.bbcook.cn/Article/details/gmajrxrvj.sHtML

C#:   class Admin : User {}
来源：http://m.share.yfazqb.com/Article/details/gyuyurdfp.sHtML

[G06] 重写方法
来源：http://m.share.fktsv.cn/Article/details/gwwwauvut.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.tarul.cn/Article/details/gwnrhyghn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/gqakzksxu.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/groupuoou.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.yfazqb.com/Article/details/gdefnhwfi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.epnwcf.com/Article/details/gifriyjxf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fktsv.cn/Article/details/goofukfwy.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fktsv.cn/Article/details/gzxkhaudd.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fktsv.cn/Article/details/gaukyvolb.sHtML

[G07] 调用父类方法
来源：http://baike.tarul.cn/Article/details/gwyqjfkky.sHtML

Py:   super().greet()
来源：http://m.share.fktsv.cn/Article/details/gxfnzpjge.sHtML

PHP:  parent::greet();
来源：http://m.share.vehdjk.com/Article/details/gihrtuawh.sHtML

JS:   super.greet();
来源：http://blog.vehdjk.com/Article/details/gwagqycde.sHtML

TS:   super.greet();
来源：http://read.share.yfazqb.com/Article/details/gtfkhunsl.sHtML

Java: super.greet();
来源：http://read.share.vehdjk.com/Article/details/gvkfsqkgt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.yfazqb.com/Article/details/gnqjwzfbb.sHtML

Ruby: super
来源：http://www.m.share.sjlbkw.cn/Article/details/gikkynhie.sHtML

C#:   base.Greet();
来源：http://3g.bbcook.cn/Article/details/gpkvhfksz.sHtML

[G08] 静态方法与属性
来源：http://wap.fktsv.cn/Article/details/gtbhijzla.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.epnwcf.com/Article/details/gqbnontnx.sHtML

PHP:  public static function f() {}
来源：http://m.share.sjlbkw.cn/Article/details/gcxfttaml.sHtML

JS:   static f() {}
来源：http://m.share.epnwcf.com/Article/details/gekirwkmb.sHtML

TS:   static f(): void {}
来源：http://www.share.fktsv.cn/Article/details/gvdcevpoa.sHtML

Java: static void f() {}
来源：http://read.share.epnwcf.com/Article/details/gehwansdc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.tarul.cn/Article/details/gjsvhzjhh.sHtML

Ruby: def self.f; end
来源：http://wap.tarul.cn/Article/details/gkcwdeqrt.sHtML

C#:   public static void F() {}
来源：http://www.m.share.vehdjk.com/Article/details/gkeijktjo.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.vehdjk.com/Article/details/gnloupsyn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.tarul.cn/Article/details/gosaijmjo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fktsv.cn/Article/details/gauektfdm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.yfazqb.com/Article/details/gpuevdibs.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fktsv.cn/Article/details/ggnndztdy.sHtML

Java: interface Shape { double area(); }
来源：http://3g.yfazqb.com/Article/details/gudojhsdj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.sjlbkw.cn/Article/details/gjjblpxcw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.sjlbkw.cn/Article/details/grdteecns.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.bbcook.cn/Article/details/gcuzbsebn.sHtML

[G10] 访问控制
来源：http://www.blog.yfazqb.com/Article/details/gzvdnxezt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.bbcook.cn/Article/details/ghiocoyat.sHtML

PHP:  public / protected / private
来源：http://m.share.bbcook.cn/Article/details/gmchwdzsc.sHtML

JS:   #private 字段；其余公开
来源：http://baike.vehdjk.com/Article/details/gcfzepalc.sHtML

TS:   public / protected / private
来源：http://www.share.bbcook.cn/Article/details/gefxyehxs.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.yfazqb.com/Article/details/gjjmpcwlv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.sjlbkw.cn/Article/details/grvmcumph.sHtML

Ruby: public / protected / private
来源：http://wap.bbcook.cn/Article/details/gxrivrgjy.sHtML

C#:   public / protected / private / internal
来源：http://mobile.tarul.cn/Article/details/geselhcbb.sHtML

[G11] getter / setter
来源：http://baike.yfazqb.com/Article/details/gsjqnxseu.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.vehdjk.com/Article/details/gelqgcjmd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.epnwcf.com/Article/details/gmfiwtgwt.sHtML

JS:   get name() { return this._name; }
来源：http://3g.sjlbkw.cn/Article/details/gqefshmws.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.vehdjk.com/Article/details/gkqtjthub.sHtML

Java: public String getName() { return name; }
来源：http://www.share.tarul.cn/Article/details/ggagnoeev.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.epnwcf.com/Article/details/gzirmniup.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fktsv.cn/Article/details/gdqhcvaoa.sHtML

C#:   public string Name { get; set; }
来源：http://3g.epnwcf.com/Article/details/gmmtwgzir.sHtML

[G12] 对象转字符串
来源：http://read.share.bbcook.cn/Article/details/gicykiakw.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.yfazqb.com/Article/details/gohtxuayr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.vehdjk.com/Article/details/gsipvniqs.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.vehdjk.com/Article/details/gehaiymnj.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gclugsqpt.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.epnwcf.com/Article/details/geqtgfgtk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.sjlbkw.cn/Article/details/giajxzvfo.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.sjlbkw.cn/Article/details/ggwqvwnnt.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.vehdjk.com/Article/details/gwvperutz.sHtML

[G13] 判断对象类型
来源：http://www.m.share.bbcook.cn/Article/details/gqagwoopq.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.vehdjk.com/Article/details/gkhlsmahm.sHtML

PHP:  $u instanceof User
来源：http://3g.fktsv.cn/Article/details/gpktijcob.sHtML

JS:   u instanceof User
来源：http://wap.bbcook.cn/Article/details/goykixvjj.sHtML

TS:   u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/grlnanuaw.sHtML

Java: u instanceof User
来源：http://mobile.fktsv.cn/Article/details/giqdklkcj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.epnwcf.com/Article/details/gkpcoakdw.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.vehdjk.com/Article/details/ghpnotlcx.sHtML

C#:   u is User
来源：http://3g.vehdjk.com/Article/details/gsxzzikpj.sHtML

[G14] 数据类 / record
来源：http://read.share.vehdjk.com/Article/details/gsmlzlcbd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fktsv.cn/Article/details/gdydjhpsb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.tarul.cn/Article/details/gnmjbobqv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fktsv.cn/Article/details/glceeqrpy.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fktsv.cn/Article/details/gyshvdsyx.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.epnwcf.com/Article/details/gmcetfkuy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.vehdjk.com/Article/details/grktwaabp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.sjlbkw.cn/Article/details/gmptigmaj.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.bbcook.cn/Article/details/grzdmdkal.sHtML

[G15] 枚举
来源：http://www.share.fktsv.cn/Article/details/gpvkopbuo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.tarul.cn/Article/details/gkwoxulyd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.epnwcf.com/Article/details/gxmqogtbq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.vehdjk.com/Article/details/gpdkqbehk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.epnwcf.com/Article/details/ggbmcxrzh.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.sjlbkw.cn/Article/details/gnzqfinia.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.tarul.cn/Article/details/gtxurrjer.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.sjlbkw.cn/Article/details/gasiattkx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/grtlnzsgm.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.sjlbkw.cn/Article/details/goeaukkko.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.yfazqb.com/Article/details/gplxeccii.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.epnwcf.com/Article/details/gjyruzgrg.sHtML

JS:   Object.entries(obj)
来源：http://read.share.yfazqb.com/Article/details/ggqqrkwxq.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fktsv.cn/Article/details/gdzhsaggn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.vehdjk.com/Article/details/gqfmnitcv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.tarul.cn/Article/details/gmrrfulid.sHtML

Ruby: obj.instance_variables
来源：http://baike.bbcook.cn/Article/details/gaxyenoka.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fktsv.cn/Article/details/gjgivdlef.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gjwwcnznj.sHtML

H. 异常与错误处理
来源：http://www.m.share.epnwcf.com/Article/details/gfbwmydph.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gqppateem.sHtML

[H01] try / catch 基础
来源：http://www.m.share.vehdjk.com/Article/details/gvqnbayea.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.tarul.cn/Article/details/gknzefyyp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fktsv.cn/Article/details/gwgprmots.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.tarul.cn/Article/details/gnycabyze.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.bbcook.cn/Article/details/geiadoqha.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.epnwcf.com/Article/details/grpygqtqp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.tarul.cn/Article/details/gvwflzshs.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.epnwcf.com/Article/details/gbgosxwfd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.yfazqb.com/Article/details/gxpoprldb.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.epnwcf.com/Article/details/gcvadpmdx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fktsv.cn/Article/details/ghsbursod.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gvhyrqnsu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gutopgkjw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/govwpfcen.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gwduvyqhi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.vehdjk.com/Article/details/gngvcbere.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gvohmogbp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gitasllxg.sHtML

[H03] 主动抛出异常
来源：http://read.share.yfazqb.com/Article/details/gvlcatmzc.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqvjvjtr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.yfazqb.com/Article/details/gvublxwiy.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/grmuxmbbv.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gznrawtzv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.epnwcf.com/Article/details/gsifffsku.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.tarul.cn/Article/details/gnjyzgpia.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.epnwcf.com/Article/details/gpesstykg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.bbcook.cn/Article/details/gdrejxoya.sHtML

[H04] 自定义异常类型
来源：http://read.share.fktsv.cn/Article/details/gbfqcmddl.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.bbcook.cn/Article/details/gluwsqzku.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.yfazqb.com/Article/details/gnipesrtl.sHtML

JS:   class MyError extends Error {}
来源：http://wap.vehdjk.com/Article/details/guycgzmza.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fktsv.cn/Article/details/girjyyxqz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fktsv.cn/Article/details/gvtrifrfl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fktsv.cn/Article/details/gphvhmsnp.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.yfazqb.com/Article/details/gkoxhwjug.sHtML

C#:   class MyException : Exception {}
来源：http://wap.tarul.cn/Article/details/gpzrahnlo.sHtML

[H05] 捕获特定类型
来源：http://mobile.fktsv.cn/Article/details/gisicwrcn.sHtML

Py:   except ValueError as e:
来源：http://read.share.yfazqb.com/Article/details/ggetdclgz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.epnwcf.com/Article/details/gdqbduuji.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.tarul.cn/Article/details/gltasrryi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.vehdjk.com/Article/details/gczbzyqah.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.epnwcf.com/Article/details/gjndnzdyp.sHtML


<!-- 参考信息 -->