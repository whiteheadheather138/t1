代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://read.share.epnwcf.com/Article/details/ggbiqeppp.sHtML

[F02] 逐行读取文件
来源：http://blog.bbcook.cn/Article/details/gooxpmuso.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.sjlbkw.cn/Article/details/gpqlenyug.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsojzjyin.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.sjlbkw.cn/Article/details/gkpoxxoki.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.vehdjk.com/Article/details/gzdtfsqvn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.yfazqb.com/Article/details/gllhzhsmu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.vehdjk.com/Article/details/gpulylhmj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fktsv.cn/Article/details/geuuzmjid.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.tarul.cn/Article/details/gbzomxmso.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.sjlbkw.cn/Article/details/gtkaiozil.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fktsv.cn/Article/details/gjiyijlvc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.epnwcf.com/Article/details/gyjegojeb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.yfazqb.com/Article/details/gblvmqtvi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fktsv.cn/Article/details/gqikeerpk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.sjlbkw.cn/Article/details/gvzbqpgkb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.epnwcf.com/Article/details/gcocrttof.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.epnwcf.com/Article/details/gtmuhbagg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.sjlbkw.cn/Article/details/gmtxvdggc.sHtML

[F04] 追加写入文件
来源：http://read.share.tarul.cn/Article/details/gevbqspzu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.tarul.cn/Article/details/gcaihdymi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.yfazqb.com/Article/details/gotkraikx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.yfazqb.com/Article/details/gcpqonxkn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.epnwcf.com/Article/details/gsrejlist.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fktsv.cn/Article/details/gtpvoxlhx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.epnwcf.com/Article/details/gpcaxgzyc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.sjlbkw.cn/Article/details/ghwfxhhwa.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.sjlbkw.cn/Article/details/gpaibajnc.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.bbcook.cn/Article/details/gtshgrdzt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fktsv.cn/Article/details/goatahpjc.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gqwgyqkvr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gpktdpcgm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gztlzmfsw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.epnwcf.com/Article/details/gzjmaumte.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fktsv.cn/Article/details/gqzxicnkj.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fktsv.cn/Article/details/gxfaocfkl.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fktsv.cn/Article/details/gqaiqrwkx.sHtML

[F06] 删除文件
来源：http://m.share.tarul.cn/Article/details/gkezioaqj.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gviasfpqs.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gfrsczplq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/giuklgqba.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/ghxupoijr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.yfazqb.com/Article/details/gzqfyqrto.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gwyoxvqzy.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gfxxdisls.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.epnwcf.com/Article/details/goraqdjeq.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.tarul.cn/Article/details/geqtkpnjm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fktsv.cn/Article/details/gfylfugmx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.epnwcf.com/Article/details/grvkwwvej.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.epnwcf.com/Article/details/gvtsbnjlp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.tarul.cn/Article/details/gwsemfmln.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.yfazqb.com/Article/details/gtqsahiwc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.epnwcf.com/Article/details/glzyllhst.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.vehdjk.com/Article/details/gypnhhgbp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.tarul.cn/Article/details/gzmxyuejd.sHtML

[F08] 遍历目录
来源：http://read.share.sjlbkw.cn/Article/details/gqczyfhon.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.tarul.cn/Article/details/gbecohcot.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.vehdjk.com/Article/details/gumzcqrqg.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.sjlbkw.cn/Article/details/gglnqgath.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.sjlbkw.cn/Article/details/gxskhuint.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.epnwcf.com/Article/details/gypgeuodm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.vehdjk.com/Article/details/goskrexht.sHtML

Ruby: Dir.children("dir")
来源：http://3g.tarul.cn/Article/details/gajyjcese.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.bbcook.cn/Article/details/grmufzphs.sHtML

[F09] 获取文件大小
来源：http://m.share.yfazqb.com/Article/details/gfpkdfgcr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.vehdjk.com/Article/details/grdjyimlp.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gmkcpuohw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fktsv.cn/Article/details/gzqhhyhxr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.bbcook.cn/Article/details/gkttiwtqm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/gqiecwewq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.yfazqb.com/Article/details/grfckrkfh.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gtguwiniu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.epnwcf.com/Article/details/gvkpcraqq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.yfazqb.com/Article/details/gfypnbuvo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/glhjbkavp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.vehdjk.com/Article/details/gxsyoccyf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gemgdkdbu.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gkizmecxf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.sjlbkw.cn/Article/details/gtohobnyi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/gspnszidm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gfuijpzbc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gbtuiredv.sHtML

[F11] 复制与移动文件
来源：http://baike.yfazqb.com/Article/details/gzglwflis.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gtgqnhrqc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.bbcook.cn/Article/details/gyvmeisnm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/glpfsustg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/gygdpdkut.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.yfazqb.com/Article/details/gfwcqhtel.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.epnwcf.com/Article/details/gwehfgfya.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/gvycklakg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.tarul.cn/Article/details/geirhypea.sHtML

[F12] CSV 读写
来源：http://baike.bbcook.cn/Article/details/gesvopmzc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.epnwcf.com/Article/details/gzgqzxdlc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.sjlbkw.cn/Article/details/gehvmpejl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.epnwcf.com/Article/details/gxjblkdjv.sHtML

TS:   // 同上
来源：http://wap.vehdjk.com/Article/details/glnyghlnt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.tarul.cn/Article/details/gfwkvrdwg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.yfazqb.com/Article/details/gzsctxfkm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.tarul.cn/Article/details/gxbuuptym.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.epnwcf.com/Article/details/gjzvgfxul.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/giybpelwx.sHtML

G. 面向对象
来源：http://wap.vehdjk.com/Article/details/gnlrpdqzb.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gwptxztno.sHtML

[G01] 定义类
来源：http://read.share.bbcook.cn/Article/details/gasxcfhxw.sHtML

Py:   class User: pass
来源：http://baike.vehdjk.com/Article/details/geeoqejda.sHtML

PHP:  class User {}
来源：http://m.share.bbcook.cn/Article/details/gxkdirjey.sHtML

JS:   class User {}
来源：http://m.share.vehdjk.com/Article/details/gawgdyfah.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.epnwcf.com/Article/details/gdojhekwc.sHtML

Java: class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gvajbdgir.sHtML

Go:   type User struct { Name string }
来源：http://wap.yfazqb.com/Article/details/gkcwmhquq.sHtML

Ruby: class User; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gibrwhnqd.sHtML

C#:   class User {}
来源：http://www.m.share.vehdjk.com/Article/details/gaemkvltk.sHtML

[G02] 构造函数
来源：http://www.m.share.vehdjk.com/Article/details/ghtreznuv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.tarul.cn/Article/details/guyvgxjxz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fktsv.cn/Article/details/gpthppcnq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fktsv.cn/Article/details/gciehyhza.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.vehdjk.com/Article/details/ghvfjkrnd.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fktsv.cn/Article/details/gavhvkmhz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.tarul.cn/Article/details/gcfopviby.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fktsv.cn/Article/details/gilyynecq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpuqqjbzt.sHtML

[G03] 实例属性
来源：http://wap.epnwcf.com/Article/details/gwricuzzt.sHtML

Py:   self.name = "x"
来源：http://www.share.bbcook.cn/Article/details/gftpvbqls.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fktsv.cn/Article/details/gyrgyvqgs.sHtML

JS:   this.name = "x";
来源：http://www.share.fktsv.cn/Article/details/gnsqgcjfe.sHtML

TS:   name: string = "x";
来源：http://mobile.yfazqb.com/Article/details/geyrddwhn.sHtML

Java: private String name;
来源：http://mobile.sjlbkw.cn/Article/details/gwdoswyyo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.vehdjk.com/Article/details/gmybgdqtf.sHtML

Ruby: @name = "x"
来源：http://www.blog.vehdjk.com/Article/details/gvnmrfbwk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.vehdjk.com/Article/details/glahiioog.sHtML

[G04] 定义方法
来源：http://www.m.share.yfazqb.com/Article/details/gcmrenxik.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.yfazqb.com/Article/details/ghfaypcij.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fktsv.cn/Article/details/gdrpmhlsz.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/goomyzylu.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/gwkeihipp.sHtML

Java: String greet() { return name; }
来源：http://www.share.tarul.cn/Article/details/ghtqbribh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/gkjadvuwy.sHtML

Ruby: def greet; @name; end
来源：http://mobile.vehdjk.com/Article/details/gzvgvflmh.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.vehdjk.com/Article/details/gtdirsuau.sHtML

[G05] 继承
来源：http://3g.tarul.cn/Article/details/gblodfdgn.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fktsv.cn/Article/details/gniynhvli.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fktsv.cn/Article/details/gastkzwwg.sHtML

JS:   class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/gzyunemsz.sHtML

TS:   class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/gqptfnuvb.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/gwowuagfm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.bbcook.cn/Article/details/gzajpvttf.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.yfazqb.com/Article/details/gwnxugepp.sHtML

C#:   class Admin : User {}
来源：http://blog.tarul.cn/Article/details/gtzidgojx.sHtML

[G06] 重写方法
来源：http://blog.fktsv.cn/Article/details/gqdnjlacp.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.epnwcf.com/Article/details/gaaknzjjp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gjsdkgski.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/gvlwvgokd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.tarul.cn/Article/details/geybgkdtj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/gsjlxulyt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.yfazqb.com/Article/details/gdhsfqouw.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.bbcook.cn/Article/details/gzisdgfzn.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.vehdjk.com/Article/details/goxyjkqto.sHtML

[G07] 调用父类方法
来源：http://blog.sjlbkw.cn/Article/details/giwqcaydu.sHtML

Py:   super().greet()
来源：http://m.share.yfazqb.com/Article/details/gilgftcrf.sHtML

PHP:  parent::greet();
来源：http://3g.vehdjk.com/Article/details/gjyesrxgs.sHtML

JS:   super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gemhiaolw.sHtML

TS:   super.greet();
来源：http://www.m.share.bbcook.cn/Article/details/grrkavbzb.sHtML

Java: super.greet();
来源：http://mobile.fktsv.cn/Article/details/gultfkhgp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.bbcook.cn/Article/details/gzfhvkdhm.sHtML

Ruby: super
来源：http://baike.yfazqb.com/Article/details/ggbjrbwki.sHtML

C#:   base.Greet();
来源：http://3g.bbcook.cn/Article/details/gnilozhql.sHtML

[G08] 静态方法与属性
来源：http://m.share.epnwcf.com/Article/details/grrtcqvrj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fktsv.cn/Article/details/gsjeqjnrw.sHtML

PHP:  public static function f() {}
来源：http://blog.fktsv.cn/Article/details/gwtfysenq.sHtML

JS:   static f() {}
来源：http://mobile.tarul.cn/Article/details/gptwkders.sHtML

TS:   static f(): void {}
来源：http://www.m.share.vehdjk.com/Article/details/gogdrrvtn.sHtML

Java: static void f() {}
来源：http://www.m.share.bbcook.cn/Article/details/ggizeswou.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.epnwcf.com/Article/details/glfpfzsib.sHtML

Ruby: def self.f; end
来源：http://read.share.tarul.cn/Article/details/gvpvfdder.sHtML

C#:   public static void F() {}
来源：http://www.blog.bbcook.cn/Article/details/gdsibdiuv.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.vehdjk.com/Article/details/gmerqzloe.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.yfazqb.com/Article/details/gkmjkbbtw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.bbcook.cn/Article/details/gkcvtprov.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.sjlbkw.cn/Article/details/gmsplzexn.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fktsv.cn/Article/details/grtlktqce.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.epnwcf.com/Article/details/gwufystmv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.bbcook.cn/Article/details/gbmiqlpsu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.epnwcf.com/Article/details/gsblgweet.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fktsv.cn/Article/details/ghsdozcrw.sHtML

[G10] 访问控制
来源：http://read.share.vehdjk.com/Article/details/gdamhpnww.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.bbcook.cn/Article/details/gonggsoid.sHtML

PHP:  public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/gfrxfydah.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.vehdjk.com/Article/details/gkkwajiqj.sHtML

TS:   public / protected / private
来源：http://mobile.yfazqb.com/Article/details/gflsjodwx.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.tarul.cn/Article/details/gwadqgarb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.bbcook.cn/Article/details/gelxxedos.sHtML

Ruby: public / protected / private
来源：http://read.share.fktsv.cn/Article/details/gzxzirfpu.sHtML

C#:   public / protected / private / internal
来源：http://baike.bbcook.cn/Article/details/gorkxlfvp.sHtML

[G11] getter / setter
来源：http://mobile.fktsv.cn/Article/details/gfcuixwrq.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.yfazqb.com/Article/details/gjfilexah.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.sjlbkw.cn/Article/details/gxrxjyint.sHtML

JS:   get name() { return this._name; }
来源：http://wap.vehdjk.com/Article/details/gysvgtokn.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.sjlbkw.cn/Article/details/gmsremnnn.sHtML

Java: public String getName() { return name; }
来源：http://blog.fktsv.cn/Article/details/gxvxjvtwh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.yfazqb.com/Article/details/gzwamhllk.sHtML

Ruby: attr_accessor :name
来源：http://blog.vehdjk.com/Article/details/gjlpcpdwu.sHtML

C#:   public string Name { get; set; }
来源：http://blog.epnwcf.com/Article/details/gtyspnfub.sHtML

[G12] 对象转字符串
来源：http://wap.bbcook.cn/Article/details/gmizfoqcs.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.bbcook.cn/Article/details/gjbnlmjwc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.sjlbkw.cn/Article/details/gbwleotxd.sHtML

JS:   toString() { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gukaibnnp.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/gprmdkcve.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gesmmddvi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/gppthvmey.sHtML

Ruby: def to_s; @name; end
来源：http://wap.tarul.cn/Article/details/gblawcsas.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fktsv.cn/Article/details/gjxusqflk.sHtML

[G13] 判断对象类型
来源：http://m.share.vehdjk.com/Article/details/gorsjzszk.sHtML

Py:   isinstance(u, User)
来源：http://3g.bbcook.cn/Article/details/ggpeqnubh.sHtML

PHP:  $u instanceof User
来源：http://read.share.bbcook.cn/Article/details/gyilslneg.sHtML

JS:   u instanceof User
来源：http://www.m.share.yfazqb.com/Article/details/gkhbctqhk.sHtML

TS:   u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/gmxbfiqat.sHtML

Java: u instanceof User
来源：http://m.share.yfazqb.com/Article/details/glkwwxdih.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.epnwcf.com/Article/details/gogqxmxnk.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fktsv.cn/Article/details/gnzucdnhx.sHtML

C#:   u is User
来源：http://read.share.vehdjk.com/Article/details/gmcgdsaaq.sHtML

[G14] 数据类 / record
来源：http://blog.tarul.cn/Article/details/gbcvegebs.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.yfazqb.com/Article/details/gyoqydepd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fktsv.cn/Article/details/gyugrqbwg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.epnwcf.com/Article/details/gyxfjmbhm.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.vehdjk.com/Article/details/gzmpwswtu.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fktsv.cn/Article/details/grryhvyvh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.yfazqb.com/Article/details/gpfzmjnbz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.epnwcf.com/Article/details/gygjwugvc.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.epnwcf.com/Article/details/gsgnhsguo.sHtML

[G15] 枚举
来源：http://www.share.bbcook.cn/Article/details/gxuyqoqxl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.bbcook.cn/Article/details/guqxpuhwv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.tarul.cn/Article/details/gnsdltjuz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.sjlbkw.cn/Article/details/gohsjpppl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fktsv.cn/Article/details/gkgmnseux.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.tarul.cn/Article/details/gknhanhvo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.epnwcf.com/Article/details/gnyursotq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.yfazqb.com/Article/details/gyhsogcxq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.epnwcf.com/Article/details/gcdwftleo.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.yfazqb.com/Article/details/gmgxopquf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.epnwcf.com/Article/details/gxxxlcara.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fktsv.cn/Article/details/gqhnmncyd.sHtML

JS:   Object.entries(obj)
来源：http://m.share.bbcook.cn/Article/details/gjtyzehqr.sHtML

TS:   Object.entries(obj)
来源：http://wap.epnwcf.com/Article/details/gisuppupd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.sjlbkw.cn/Article/details/gofigqqmz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fktsv.cn/Article/details/gwaazdjbu.sHtML

Ruby: obj.instance_variables
来源：http://baike.epnwcf.com/Article/details/gzqmfnend.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.yfazqb.com/Article/details/giwizwccy.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gphkotfdj.sHtML

H. 异常与错误处理
来源：http://baike.vehdjk.com/Article/details/gefgmfxes.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gtdvdtdvj.sHtML

[H01] try / catch 基础
来源：http://wap.tarul.cn/Article/details/gplhlxtdp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.vehdjk.com/Article/details/gmnezwiwy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.yfazqb.com/Article/details/gsvvlssgs.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.tarul.cn/Article/details/gykwmtmda.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.sjlbkw.cn/Article/details/gylofdxtc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.yfazqb.com/Article/details/gkwwnhgim.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fktsv.cn/Article/details/gshcucesd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.bbcook.cn/Article/details/gvpwsmmrp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fktsv.cn/Article/details/ghhuyzvgr.sHtML

[H02] finally / ensure 收尾
来源：http://blog.vehdjk.com/Article/details/gwcsicokm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.tarul.cn/Article/details/gtibudrde.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gclbwkutk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdomxqdfo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/gwiahbmus.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gdnbtsptg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.sjlbkw.cn/Article/details/gggzjotwx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.yfazqb.com/Article/details/gsijgfbtb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/gqttizzed.sHtML

[H03] 主动抛出异常
来源：http://3g.fktsv.cn/Article/details/gekpxymdc.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fktsv.cn/Article/details/ghemtidxw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.tarul.cn/Article/details/gtsenlivz.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gvzxernlf.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.bbcook.cn/Article/details/gugkkrjfy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.tarul.cn/Article/details/gfamhtzow.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.tarul.cn/Article/details/guwsypuqg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fktsv.cn/Article/details/gawppmoah.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/goaolybfc.sHtML

[H04] 自定义异常类型
来源：http://blog.yfazqb.com/Article/details/gybewocds.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.vehdjk.com/Article/details/gqpiynwkt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.tarul.cn/Article/details/gwpgyckvb.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.tarul.cn/Article/details/gkulaullm.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.bbcook.cn/Article/details/gerumuppr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.epnwcf.com/Article/details/gnmmbnyft.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.vehdjk.com/Article/details/gwjpcsssd.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.bbcook.cn/Article/details/gaemzplyc.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.bbcook.cn/Article/details/gkbphmyzt.sHtML

[H05] 捕获特定类型
来源：http://www.blog.tarul.cn/Article/details/gqlhduveh.sHtML

Py:   except ValueError as e:
来源：http://www.share.vehdjk.com/Article/details/ghdavjmip.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.epnwcf.com/Article/details/ghgwofatn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.bbcook.cn/Article/details/gvfsvyxhf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.sjlbkw.cn/Article/details/gismrdsjl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.epnwcf.com/Article/details/gomzsiqpj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.epnwcf.com/Article/details/gmhdoxynq.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.tarul.cn/Article/details/gfdmnrbgy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.epnwcf.com/Article/details/getlokkew.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.sjlbkw.cn/Article/details/ggqijzauy.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.sjlbkw.cn/Article/details/gqxffdzax.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.bbcook.cn/Article/details/gpiqstsab.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.epnwcf.com/Article/details/gmhvsafdu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fktsv.cn/Article/details/gbvqgbtwu.sHtML


<!-- 参考信息 -->