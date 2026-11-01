代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.sjlbkw.cn/Article/details/gqgtmothq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.yfazqb.com/Article/details/gzgtbkjcu.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.sjlbkw.cn/Article/details/gdcyjbmes.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.sjlbkw.cn/Article/details/gufzfhmno.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.vehdjk.com/Article/details/gdluewwxv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.bbcook.cn/Article/details/gagknyfgc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.yfazqb.com/Article/details/gzcjfbzgf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.tarul.cn/Article/details/gqqsjfxup.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.vehdjk.com/Article/details/guxbfykub.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fktsv.cn/Article/details/gvagywaof.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fktsv.cn/Article/details/gtzcbcmry.sHtML

[F04] 追加写入文件
来源：http://blog.fktsv.cn/Article/details/gpgbcopkk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.vehdjk.com/Article/details/gekdkinpy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.bbcook.cn/Article/details/gheminmog.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.vehdjk.com/Article/details/gjjxqaoij.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.bbcook.cn/Article/details/gatmluzvf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.tarul.cn/Article/details/gsavsqgta.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.tarul.cn/Article/details/gptgfbiaz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.sjlbkw.cn/Article/details/glvahysxg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.vehdjk.com/Article/details/ggogfrabx.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.bbcook.cn/Article/details/gozknzmzz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.bbcook.cn/Article/details/gkddeaeie.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.vehdjk.com/Article/details/gypipluiq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gssdjdhri.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/gsydgdinm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/gxedtnhbq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.sjlbkw.cn/Article/details/gegvqjjls.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fktsv.cn/Article/details/ghuplnqvm.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gnmareuzf.sHtML

[F06] 删除文件
来源：http://baike.fktsv.cn/Article/details/gkuwbsawf.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gjosiceuw.sHtML

PHP:  unlink("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gbsfxnted.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gilxatoxp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.vehdjk.com/Article/details/gkvxbayfz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/glnugpyeo.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.bbcook.cn/Article/details/gecwleeou.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fktsv.cn/Article/details/gyjvyjuzv.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fktsv.cn/Article/details/gkkhpamvw.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.yfazqb.com/Article/details/gsltdyuus.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fktsv.cn/Article/details/gsraskgqo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.yfazqb.com/Article/details/gztjzznmz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.yfazqb.com/Article/details/gidqkyypy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.sjlbkw.cn/Article/details/gtpzumclz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fktsv.cn/Article/details/gfzhsrtce.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.bbcook.cn/Article/details/glldwnyos.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.sjlbkw.cn/Article/details/gankajbny.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fktsv.cn/Article/details/ggfqcosol.sHtML

[F08] 遍历目录
来源：http://read.share.fktsv.cn/Article/details/gczoglewf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fktsv.cn/Article/details/ghaxbynvd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.bbcook.cn/Article/details/goguvuoen.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.epnwcf.com/Article/details/gmbkmyrfh.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fktsv.cn/Article/details/ghbgtmptx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fktsv.cn/Article/details/gbyuqmhjx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.vehdjk.com/Article/details/gmuqoxcpx.sHtML

Ruby: Dir.children("dir")
来源：http://blog.yfazqb.com/Article/details/goqeshfim.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.yfazqb.com/Article/details/gkxvluexh.sHtML

[F09] 获取文件大小
来源：http://blog.fktsv.cn/Article/details/gmqzayydt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.yfazqb.com/Article/details/gzllicwwk.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gljjhyoew.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.vehdjk.com/Article/details/gmiktfrcv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.sjlbkw.cn/Article/details/gacmwupjv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/gfplpcsds.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.yfazqb.com/Article/details/glbvvggng.sHtML

Ruby: File.size("a.txt")
来源：http://baike.tarul.cn/Article/details/gxkgpmxrs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.vehdjk.com/Article/details/gtxmvcvws.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.epnwcf.com/Article/details/gsyeafoao.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gaszextal.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.epnwcf.com/Article/details/gzkxyuwhu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/guiamvnxp.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gsvntakig.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fktsv.cn/Article/details/grwhopqoq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gjyrxphhg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/gogdxlvln.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/ghvaqwizl.sHtML

[F11] 复制与移动文件
来源：http://baike.vehdjk.com/Article/details/gmzfrlqyo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/gqhwwflif.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fktsv.cn/Article/details/gptoeazxn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gzldswaeb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/glrwgjqoa.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.sjlbkw.cn/Article/details/gvyrzphvk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.sjlbkw.cn/Article/details/gldzfgwip.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/gkhrcwdrl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.epnwcf.com/Article/details/gdkzhjrbu.sHtML

[F12] CSV 读写
来源：http://www.m.share.bbcook.cn/Article/details/gvfitwvgc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.bbcook.cn/Article/details/gyyvadvkh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.yfazqb.com/Article/details/gvoudssyu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fktsv.cn/Article/details/giducvwzr.sHtML

TS:   // 同上
来源：http://mobile.fktsv.cn/Article/details/ggidufqgj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.bbcook.cn/Article/details/goedpqwux.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.yfazqb.com/Article/details/gzghcdpyb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.epnwcf.com/Article/details/gebiynovb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fktsv.cn/Article/details/ghfeofuwy.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gesbcyper.sHtML

G. 面向对象
来源：http://www.share.tarul.cn/Article/details/gkgakrthp.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/guafnjxgr.sHtML

[G01] 定义类
来源：http://www.blog.sjlbkw.cn/Article/details/gglaqcprr.sHtML

Py:   class User: pass
来源：http://blog.sjlbkw.cn/Article/details/gohhmbysm.sHtML

PHP:  class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gizebpjtj.sHtML

JS:   class User {}
来源：http://www.share.bbcook.cn/Article/details/gudgnjrgi.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.epnwcf.com/Article/details/gbekibuaa.sHtML

Java: class User {}
来源：http://wap.vehdjk.com/Article/details/gmzjcyqix.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fktsv.cn/Article/details/gkiotncce.sHtML

Ruby: class User; end
来源：http://wap.bbcook.cn/Article/details/gfiszgtyk.sHtML

C#:   class User {}
来源：http://read.share.bbcook.cn/Article/details/ghlwgijmt.sHtML

[G02] 构造函数
来源：http://baike.sjlbkw.cn/Article/details/gxyzslirp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.sjlbkw.cn/Article/details/gywrocytb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.sjlbkw.cn/Article/details/gvtttusnz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.yfazqb.com/Article/details/gsovswshx.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.vehdjk.com/Article/details/gqkigqphj.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.sjlbkw.cn/Article/details/geaviqrhq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.bbcook.cn/Article/details/gjdddhjul.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.sjlbkw.cn/Article/details/gncswypbc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbjbuorrm.sHtML

[G03] 实例属性
来源：http://www.share.bbcook.cn/Article/details/gwihzgrpr.sHtML

Py:   self.name = "x"
来源：http://wap.sjlbkw.cn/Article/details/gawqgpdyv.sHtML

PHP:  public string $name = "x";
来源：http://blog.sjlbkw.cn/Article/details/gfcrisrqv.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fktsv.cn/Article/details/gklexvwbi.sHtML

TS:   name: string = "x";
来源：http://wap.bbcook.cn/Article/details/gtmjxswds.sHtML

Java: private String name;
来源：http://3g.bbcook.cn/Article/details/gitzlktzk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.sjlbkw.cn/Article/details/gvsyfcjxc.sHtML

Ruby: @name = "x"
来源：http://3g.sjlbkw.cn/Article/details/gqulizwpa.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.tarul.cn/Article/details/gvmexhhlh.sHtML

[G04] 定义方法
来源：http://mobile.epnwcf.com/Article/details/gtdmqtiti.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fktsv.cn/Article/details/gbfmcahtv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.tarul.cn/Article/details/gjyaoaien.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.vehdjk.com/Article/details/gpsluodab.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/gpkovkaie.sHtML

Java: String greet() { return name; }
来源：http://read.share.tarul.cn/Article/details/guoapwvmr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gcdtiotpl.sHtML

Ruby: def greet; @name; end
来源：http://3g.fktsv.cn/Article/details/gyildnola.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.epnwcf.com/Article/details/gboodvivx.sHtML

[G05] 继承
来源：http://www.blog.bbcook.cn/Article/details/gktajgvwa.sHtML

Py:   class Admin(User): pass
来源：http://baike.bbcook.cn/Article/details/gjgbwtfja.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.sjlbkw.cn/Article/details/gvbiztfou.sHtML

JS:   class Admin extends User {}
来源：http://wap.bbcook.cn/Article/details/glilalztv.sHtML

TS:   class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gacsleaxr.sHtML

Java: class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/gqagdnkdy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fktsv.cn/Article/details/gdabsndmp.sHtML

Ruby: class Admin < User; end
来源：http://baike.bbcook.cn/Article/details/gbldifzxl.sHtML

C#:   class Admin : User {}
来源：http://www.share.tarul.cn/Article/details/gmuuezpju.sHtML

[G06] 重写方法
来源：http://read.share.bbcook.cn/Article/details/gnkdovjtz.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.vehdjk.com/Article/details/gtglifnkd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/gigcrufpx.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.epnwcf.com/Article/details/gdtcbyxkt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gzkuirguz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/gnwyvueyo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.epnwcf.com/Article/details/gimibwflf.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.yfazqb.com/Article/details/gbnohabai.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.yfazqb.com/Article/details/grvbgesbt.sHtML

[G07] 调用父类方法
来源：http://www.blog.bbcook.cn/Article/details/gzszdkzqa.sHtML

Py:   super().greet()
来源：http://read.share.bbcook.cn/Article/details/gkkryverw.sHtML

PHP:  parent::greet();
来源：http://baike.bbcook.cn/Article/details/gilviixjh.sHtML

JS:   super.greet();
来源：http://wap.bbcook.cn/Article/details/gikcnrvjb.sHtML

TS:   super.greet();
来源：http://read.share.yfazqb.com/Article/details/gmlmoqdlh.sHtML

Java: super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gbxbknwgv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.sjlbkw.cn/Article/details/gmwvgharg.sHtML

Ruby: super
来源：http://blog.bbcook.cn/Article/details/gsxpebajs.sHtML

C#:   base.Greet();
来源：http://www.blog.epnwcf.com/Article/details/glperpukb.sHtML

[G08] 静态方法与属性
来源：http://baike.epnwcf.com/Article/details/gknrkpaxx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fktsv.cn/Article/details/gpfxwyyot.sHtML

PHP:  public static function f() {}
来源：http://mobile.yfazqb.com/Article/details/gyrcjyxof.sHtML

JS:   static f() {}
来源：http://mobile.fktsv.cn/Article/details/gskwksvnq.sHtML

TS:   static f(): void {}
来源：http://www.m.share.yfazqb.com/Article/details/gtanvlwpo.sHtML

Java: static void f() {}
来源：http://www.m.share.bbcook.cn/Article/details/gxdxvxbfg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.bbcook.cn/Article/details/gbzjyansi.sHtML

Ruby: def self.f; end
来源：http://read.share.fktsv.cn/Article/details/gcqfdwlxc.sHtML

C#:   public static void F() {}
来源：http://www.share.vehdjk.com/Article/details/gbuazahzp.sHtML

[G09] 接口 / 抽象类
来源：http://3g.bbcook.cn/Article/details/gauubkblu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.vehdjk.com/Article/details/gtwbdinhw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.epnwcf.com/Article/details/gagnxkqyr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.sjlbkw.cn/Article/details/gqakwhaqi.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.epnwcf.com/Article/details/gcbazmwwy.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.bbcook.cn/Article/details/grafuoqqm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fktsv.cn/Article/details/gsiacgvwc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.vehdjk.com/Article/details/gcmqjcqbk.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.epnwcf.com/Article/details/gnnkvttwe.sHtML

[G10] 访问控制
来源：http://wap.yfazqb.com/Article/details/gtroyyolk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.yfazqb.com/Article/details/ghjwugpec.sHtML

PHP:  public / protected / private
来源：http://wap.bbcook.cn/Article/details/ggdmzxmbp.sHtML

JS:   #private 字段；其余公开
来源：http://wap.sjlbkw.cn/Article/details/gpljrgpxg.sHtML

TS:   public / protected / private
来源：http://blog.vehdjk.com/Article/details/gqhxuedun.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fktsv.cn/Article/details/glcwoycur.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.tarul.cn/Article/details/gizcchsju.sHtML

Ruby: public / protected / private
来源：http://m.share.vehdjk.com/Article/details/galkquhes.sHtML

C#:   public / protected / private / internal
来源：http://mobile.yfazqb.com/Article/details/gpfagbvvh.sHtML

[G11] getter / setter
来源：http://3g.epnwcf.com/Article/details/gjxnunwcd.sHtML

Py:   @property 与 @x.setter
来源：http://blog.vehdjk.com/Article/details/gvtqgpxmf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/gssszggpa.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.yfazqb.com/Article/details/gekxlyxwi.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.bbcook.cn/Article/details/ghblrvlar.sHtML

Java: public String getName() { return name; }
来源：http://m.share.yfazqb.com/Article/details/gshdrabyo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gfnvzltpz.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fktsv.cn/Article/details/geckmrmxz.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fktsv.cn/Article/details/gobbhgunf.sHtML

[G12] 对象转字符串
来源：http://3g.fktsv.cn/Article/details/guhdcizss.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.vehdjk.com/Article/details/gqppjnfei.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.sjlbkw.cn/Article/details/grmywldnb.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.vehdjk.com/Article/details/gixfukvcv.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gmxetdxnm.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.yfazqb.com/Article/details/gnhnvmvjg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gnlzlwcbz.sHtML

Ruby: def to_s; @name; end
来源：http://wap.sjlbkw.cn/Article/details/gvbretrhf.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.bbcook.cn/Article/details/glncnukwh.sHtML

[G13] 判断对象类型
来源：http://wap.fktsv.cn/Article/details/gjpvkfhuv.sHtML

Py:   isinstance(u, User)
来源：http://baike.epnwcf.com/Article/details/gaxjrglsq.sHtML

PHP:  $u instanceof User
来源：http://www.share.yfazqb.com/Article/details/gsqemsqam.sHtML

JS:   u instanceof User
来源：http://m.share.sjlbkw.cn/Article/details/gbusalkzf.sHtML

TS:   u instanceof User
来源：http://wap.bbcook.cn/Article/details/gmqjswjux.sHtML

Java: u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/gxqckjvyd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fktsv.cn/Article/details/gibbysvfg.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.tarul.cn/Article/details/gbszcclgm.sHtML

C#:   u is User
来源：http://www.share.fktsv.cn/Article/details/gclbssryh.sHtML

[G14] 数据类 / record
来源：http://www.m.share.tarul.cn/Article/details/gebvvfnjz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fktsv.cn/Article/details/gyiutpblx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fktsv.cn/Article/details/gbhnwwsuu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.epnwcf.com/Article/details/gkhduasgc.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.epnwcf.com/Article/details/ghcwfjvug.sHtML

Java: record User(String name, int age) {}
来源：http://wap.epnwcf.com/Article/details/gplktgtil.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.sjlbkw.cn/Article/details/gagucidbe.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.epnwcf.com/Article/details/gmsqhdfqt.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.epnwcf.com/Article/details/gfiixtybo.sHtML

[G15] 枚举
来源：http://mobile.sjlbkw.cn/Article/details/gtstqdmmx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.tarul.cn/Article/details/ghiqpcasm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.vehdjk.com/Article/details/gpmnupxsn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.vehdjk.com/Article/details/gztxyyftd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gdmiqhhsv.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.vehdjk.com/Article/details/gdchjuzrl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.tarul.cn/Article/details/gkbiiswjv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.bbcook.cn/Article/details/gzogekuib.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.bbcook.cn/Article/details/gocemqedw.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.tarul.cn/Article/details/gdrshtnki.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.sjlbkw.cn/Article/details/gatwclsmf.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.epnwcf.com/Article/details/ghnagqjau.sHtML

JS:   Object.entries(obj)
来源：http://3g.yfazqb.com/Article/details/gsqtofkaa.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fktsv.cn/Article/details/gzhdpjfvb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.epnwcf.com/Article/details/gdacswbka.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fktsv.cn/Article/details/ggkqwigwr.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.bbcook.cn/Article/details/gjafhqrsh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.tarul.cn/Article/details/gmjctwtcb.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gtdjrrzob.sHtML

H. 异常与错误处理
来源：http://wap.vehdjk.com/Article/details/gtayffuvc.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gemoxfnsh.sHtML

[H01] try / catch 基础
来源：http://www.m.share.yfazqb.com/Article/details/gfigadugo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.yfazqb.com/Article/details/gzmkinrcj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.epnwcf.com/Article/details/gnixctpsw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.vehdjk.com/Article/details/gkgguecse.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.bbcook.cn/Article/details/gytngnjqf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.yfazqb.com/Article/details/gggdoysav.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fktsv.cn/Article/details/gufxwkhoc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fktsv.cn/Article/details/gocleewlm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.yfazqb.com/Article/details/gsyvrsjwa.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.yfazqb.com/Article/details/gavmrwela.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.tarul.cn/Article/details/gphffrdyp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gwdfsvyox.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gdzvnhcof.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gcdynvrwb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.yfazqb.com/Article/details/gcoylgzqy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.yfazqb.com/Article/details/gwdjsvtrh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.yfazqb.com/Article/details/gomywfdzq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gcdutpmss.sHtML

[H03] 主动抛出异常
来源：http://blog.fktsv.cn/Article/details/gefjjzwcd.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.sjlbkw.cn/Article/details/gsgviggcf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/glkhrdwcr.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.epnwcf.com/Article/details/ghbotzcsk.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gnndnoite.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gmlhccpif.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.vehdjk.com/Article/details/gdlcuedcn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.epnwcf.com/Article/details/gjchabvsc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/gkyvkhrum.sHtML

[H04] 自定义异常类型
来源：http://read.share.epnwcf.com/Article/details/gauwjdcrt.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fktsv.cn/Article/details/gxrhppqci.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.vehdjk.com/Article/details/gzbdkkaxt.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.yfazqb.com/Article/details/grbbcvqnv.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.tarul.cn/Article/details/gtzrhzddl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.vehdjk.com/Article/details/gawpdpfnu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fktsv.cn/Article/details/gaeghakae.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.sjlbkw.cn/Article/details/glmnqdkej.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.tarul.cn/Article/details/gjkfbjyce.sHtML

[H05] 捕获特定类型
来源：http://blog.yfazqb.com/Article/details/gqmxapjbi.sHtML

Py:   except ValueError as e:
来源：http://blog.epnwcf.com/Article/details/gckhogucy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.yfazqb.com/Article/details/gputvqavz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.vehdjk.com/Article/details/gumsxzlyb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.bbcook.cn/Article/details/gsarzjvyo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.yfazqb.com/Article/details/gqheshqfk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.tarul.cn/Article/details/gypigaxli.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.epnwcf.com/Article/details/geuogvthd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.bbcook.cn/Article/details/gzwafujhb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.vehdjk.com/Article/details/gtiauzdqt.sHtML

Py:   value = d.get("k") or default
来源：http://3g.epnwcf.com/Article/details/gjchahudi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fktsv.cn/Article/details/gsscinvsp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.sjlbkw.cn/Article/details/gtzbiaxab.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.vehdjk.com/Article/details/gbqspefnk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.yfazqb.com/Article/details/gnlashmvc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fktsv.cn/Article/details/gtmnqguaj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.bbcook.cn/Article/details/gcdzvjdiv.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.tarul.cn/Article/details/gheeicxpm.sHtML

[H07] 断言
来源：http://baike.sjlbkw.cn/Article/details/gvutoqdix.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fktsv.cn/Article/details/gglyncrqn.sHtML

PHP:  assert($x > 0);
来源：http://baike.fktsv.cn/Article/details/gbqoclqbr.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.epnwcf.com/Article/details/gvvrbmiir.sHtML


<!-- 参考信息 -->