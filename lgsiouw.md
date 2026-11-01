代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.tarul.cn/Article/details/gmkocjsvs.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.yfazqb.com/Article/details/glcxuasnp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.tarul.cn/Article/details/gwghlobgv.sHtML

[F04] 追加写入文件
来源：http://www.blog.epnwcf.com/Article/details/gbzejbddg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.yfazqb.com/Article/details/gcfrykoel.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.epnwcf.com/Article/details/gjkwvvdyd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.epnwcf.com/Article/details/gkyihjyqx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.epnwcf.com/Article/details/gaonpyotp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fktsv.cn/Article/details/gvtldvefm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.vehdjk.com/Article/details/gerykuwxg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.bbcook.cn/Article/details/gmzxidems.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.bbcook.cn/Article/details/gdfiejqom.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.epnwcf.com/Article/details/ggubzurab.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.vehdjk.com/Article/details/gevtypzyf.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gsqajmetm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.yfazqb.com/Article/details/gknxjnpjs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gccqwfkyu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/gmsezwtui.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.yfazqb.com/Article/details/gouocsybn.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.tarul.cn/Article/details/gnmbdizny.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.epnwcf.com/Article/details/gjjqohvio.sHtML

[F06] 删除文件
来源：http://www.share.epnwcf.com/Article/details/gnodxwrea.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gltiulzhm.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gspypjztg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/goqmgcrkw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gdcjcglxk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/gxnjxdbkv.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/garqsngxf.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gewtcgryj.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.vehdjk.com/Article/details/govdekocb.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.bbcook.cn/Article/details/gyacnftxc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.tarul.cn/Article/details/gahlyjvln.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.yfazqb.com/Article/details/gfyhsomqh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fktsv.cn/Article/details/gikxhovoq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.sjlbkw.cn/Article/details/gygdcaqri.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.yfazqb.com/Article/details/gvabnjpmv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.sjlbkw.cn/Article/details/gnzpmlbas.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.tarul.cn/Article/details/gxmfxqake.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.yfazqb.com/Article/details/guurlbabz.sHtML

[F08] 遍历目录
来源：http://blog.epnwcf.com/Article/details/gzfysckqp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.bbcook.cn/Article/details/gjaaeboqw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.tarul.cn/Article/details/gwgagauuj.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fktsv.cn/Article/details/gombauknw.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fktsv.cn/Article/details/gqoxqmist.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.sjlbkw.cn/Article/details/ghdkzqfbp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.epnwcf.com/Article/details/gxzmbwedi.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fktsv.cn/Article/details/ggsduzwvf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.sjlbkw.cn/Article/details/gnnsksjii.sHtML

[F09] 获取文件大小
来源：http://www.share.bbcook.cn/Article/details/gqllxzkbz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gtvsriedz.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/giyjsitfp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.bbcook.cn/Article/details/gqjbkebpc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.tarul.cn/Article/details/gkslmccvp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/gdnquaxvo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.epnwcf.com/Article/details/grgoiiqbj.sHtML

Ruby: File.size("a.txt")
来源：http://baike.epnwcf.com/Article/details/gripfvtow.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.tarul.cn/Article/details/gxfbntmqu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.yfazqb.com/Article/details/gwewaepxv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/ghqnmtzid.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.epnwcf.com/Article/details/glmtikobh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gsiwktfhw.sHtML

TS:   path.extname("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/giofqehde.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.sjlbkw.cn/Article/details/gcucmtjlj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/gujuzmbhs.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gcrvwlaaz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gxiifbriw.sHtML

[F11] 复制与移动文件
来源：http://baike.vehdjk.com/Article/details/gvcyhbnlf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gnxgrswnf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.vehdjk.com/Article/details/grjywrrmg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/gifxhfsbo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/goglmcxyz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fktsv.cn/Article/details/gtkyehxkw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.tarul.cn/Article/details/gxzbjwjws.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/glsolbwug.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.vehdjk.com/Article/details/gexrgfjju.sHtML

[F12] CSV 读写
来源：http://blog.vehdjk.com/Article/details/geblatcvc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.yfazqb.com/Article/details/gwuhsoccd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.tarul.cn/Article/details/gcehvfdkk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.epnwcf.com/Article/details/gohkskmgz.sHtML

TS:   // 同上
来源：http://www.m.share.bbcook.cn/Article/details/gfranytvd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.tarul.cn/Article/details/grnxcjetr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.vehdjk.com/Article/details/ggdhnptas.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fktsv.cn/Article/details/gmszerwdh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.tarul.cn/Article/details/gasvmzrcd.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gwynfzuzz.sHtML

G. 面向对象
来源：http://mobile.yfazqb.com/Article/details/gkuzrmgbl.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gsyajgfux.sHtML

[G01] 定义类
来源：http://blog.sjlbkw.cn/Article/details/gkslqvyhc.sHtML

Py:   class User: pass
来源：http://blog.epnwcf.com/Article/details/gnaywdlco.sHtML

PHP:  class User {}
来源：http://www.blog.epnwcf.com/Article/details/grhiabqxc.sHtML

JS:   class User {}
来源：http://baike.fktsv.cn/Article/details/gerktjamj.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.bbcook.cn/Article/details/gjxfzoaef.sHtML

Java: class User {}
来源：http://wap.tarul.cn/Article/details/gmssatijt.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.yfazqb.com/Article/details/gxmhwraaz.sHtML

Ruby: class User; end
来源：http://3g.fktsv.cn/Article/details/gvupnpdyj.sHtML

C#:   class User {}
来源：http://read.share.vehdjk.com/Article/details/gpgrpixmw.sHtML

[G02] 构造函数
来源：http://mobile.fktsv.cn/Article/details/gjkrsduni.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.yfazqb.com/Article/details/glaqbrrwt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fktsv.cn/Article/details/giuakoenc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.bbcook.cn/Article/details/gsbbfrcok.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.epnwcf.com/Article/details/gehsbqumg.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.vehdjk.com/Article/details/ghoivwilh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.vehdjk.com/Article/details/gafbfungg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.bbcook.cn/Article/details/gclsesmho.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.tarul.cn/Article/details/gtbceabfj.sHtML

[G03] 实例属性
来源：http://read.share.fktsv.cn/Article/details/gckfjcygk.sHtML

Py:   self.name = "x"
来源：http://www.blog.vehdjk.com/Article/details/gwxidcpkx.sHtML

PHP:  public string $name = "x";
来源：http://baike.epnwcf.com/Article/details/gzewxckts.sHtML

JS:   this.name = "x";
来源：http://wap.tarul.cn/Article/details/gmupownta.sHtML

TS:   name: string = "x";
来源：http://www.m.share.sjlbkw.cn/Article/details/gunzaskpv.sHtML

Java: private String name;
来源：http://wap.tarul.cn/Article/details/gwnvtksny.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.epnwcf.com/Article/details/gxirforkj.sHtML

Ruby: @name = "x"
来源：http://blog.yfazqb.com/Article/details/gnrlyiamw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.yfazqb.com/Article/details/gyvypwsqv.sHtML

[G04] 定义方法
来源：http://read.share.tarul.cn/Article/details/gkesxnrxv.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.yfazqb.com/Article/details/gfygdlvdn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.epnwcf.com/Article/details/gjklnwjin.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/gsafxdsvt.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.bbcook.cn/Article/details/gfskomwgo.sHtML

Java: String greet() { return name; }
来源：http://m.share.yfazqb.com/Article/details/gqmwpjvll.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/gwosdjjuq.sHtML

Ruby: def greet; @name; end
来源：http://blog.epnwcf.com/Article/details/gjmdaqbtr.sHtML

C#:   public string Greet() => Name;
来源：http://wap.sjlbkw.cn/Article/details/gvglxdvqk.sHtML

[G05] 继承
来源：http://www.blog.fktsv.cn/Article/details/gnzetswzu.sHtML

Py:   class Admin(User): pass
来源：http://m.share.tarul.cn/Article/details/gkmxxcsiw.sHtML

PHP:  class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gimzxomxs.sHtML

JS:   class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gbumrdbsg.sHtML

TS:   class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/gumnebfbl.sHtML

Java: class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/gpbzedkby.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.sjlbkw.cn/Article/details/gtaxkqzmk.sHtML

Ruby: class Admin < User; end
来源：http://www.share.yfazqb.com/Article/details/gtguvpgef.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.yfazqb.com/Article/details/gykykeius.sHtML

[G06] 重写方法
来源：http://www.blog.yfazqb.com/Article/details/gutwagjej.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.sjlbkw.cn/Article/details/gyvozmhsd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.yfazqb.com/Article/details/giemuohfd.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/gtfaniqvm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.tarul.cn/Article/details/gaimeqtpv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/gctavlgei.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.tarul.cn/Article/details/gmxiytxqt.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.tarul.cn/Article/details/gmenvsurp.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.yfazqb.com/Article/details/gmhstcehm.sHtML

[G07] 调用父类方法
来源：http://www.m.share.sjlbkw.cn/Article/details/gfrnmkkms.sHtML

Py:   super().greet()
来源：http://blog.yfazqb.com/Article/details/ghafgdmsg.sHtML

PHP:  parent::greet();
来源：http://m.share.sjlbkw.cn/Article/details/gqgrjqywb.sHtML

JS:   super.greet();
来源：http://3g.fktsv.cn/Article/details/gocttqrlp.sHtML

TS:   super.greet();
来源：http://baike.tarul.cn/Article/details/gkrfdhqqk.sHtML

Java: super.greet();
来源：http://www.share.yfazqb.com/Article/details/gyyrvlfai.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.epnwcf.com/Article/details/gmriyhvud.sHtML

Ruby: super
来源：http://3g.fktsv.cn/Article/details/graboxmst.sHtML

C#:   base.Greet();
来源：http://mobile.yfazqb.com/Article/details/grxarrnbr.sHtML

[G08] 静态方法与属性
来源：http://blog.bbcook.cn/Article/details/ghlmfhmlm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.sjlbkw.cn/Article/details/gakuvoolm.sHtML

PHP:  public static function f() {}
来源：http://3g.fktsv.cn/Article/details/gvrgvruil.sHtML

JS:   static f() {}
来源：http://wap.yfazqb.com/Article/details/gtemwtmlf.sHtML

TS:   static f(): void {}
来源：http://3g.fktsv.cn/Article/details/gwykvwmhn.sHtML

Java: static void f() {}
来源：http://www.blog.vehdjk.com/Article/details/gqavnzvvl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.sjlbkw.cn/Article/details/gmlcytgwu.sHtML

Ruby: def self.f; end
来源：http://read.share.tarul.cn/Article/details/ggstilwoj.sHtML

C#:   public static void F() {}
来源：http://wap.epnwcf.com/Article/details/ghxyidnee.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.tarul.cn/Article/details/getgljmeo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.tarul.cn/Article/details/gcbszohbc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fktsv.cn/Article/details/gnypsaeyi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.yfazqb.com/Article/details/grnesttoa.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fktsv.cn/Article/details/gmkhcbvsl.sHtML

Java: interface Shape { double area(); }
来源：http://blog.epnwcf.com/Article/details/gmingzcxb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fktsv.cn/Article/details/gthptykyt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.yfazqb.com/Article/details/gurmotmfq.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.epnwcf.com/Article/details/gfoixtnwb.sHtML

[G10] 访问控制
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqyelbnp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.sjlbkw.cn/Article/details/gfboaemsq.sHtML

PHP:  public / protected / private
来源：http://wap.sjlbkw.cn/Article/details/gtwbxgngy.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.tarul.cn/Article/details/gsvjpxkwd.sHtML

TS:   public / protected / private
来源：http://www.blog.yfazqb.com/Article/details/gtspoqgjg.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.yfazqb.com/Article/details/gpmudlbbk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.yfazqb.com/Article/details/ggimsxncc.sHtML

Ruby: public / protected / private
来源：http://mobile.vehdjk.com/Article/details/gdxnrxhnf.sHtML

C#:   public / protected / private / internal
来源：http://blog.bbcook.cn/Article/details/grnhfidqv.sHtML

[G11] getter / setter
来源：http://m.share.vehdjk.com/Article/details/gdzddpcjc.sHtML

Py:   @property 与 @x.setter
来源：http://wap.sjlbkw.cn/Article/details/grdzhwirm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/gqbjdvicy.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.yfazqb.com/Article/details/gkitzolyx.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.sjlbkw.cn/Article/details/ggfkryyaw.sHtML

Java: public String getName() { return name; }
来源：http://mobile.yfazqb.com/Article/details/gflvzqxaj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.bbcook.cn/Article/details/giqrbrowu.sHtML

Ruby: attr_accessor :name
来源：http://baike.tarul.cn/Article/details/gxmsyyrrt.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fktsv.cn/Article/details/glzpxmkgz.sHtML

[G12] 对象转字符串
来源：http://m.share.sjlbkw.cn/Article/details/gbqcwpblg.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.sjlbkw.cn/Article/details/gssrhwpwe.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/gaxujlbhc.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.sjlbkw.cn/Article/details/gszjxsgpt.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/gyoqzepdr.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.bbcook.cn/Article/details/gsmdbecil.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.bbcook.cn/Article/details/gdoojscxo.sHtML

Ruby: def to_s; @name; end
来源：http://baike.yfazqb.com/Article/details/gbiuswyoi.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.sjlbkw.cn/Article/details/gockhgwbj.sHtML

[G13] 判断对象类型
来源：http://mobile.tarul.cn/Article/details/grujvxroz.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.bbcook.cn/Article/details/gnmilogvm.sHtML

PHP:  $u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/gyqbbzyrd.sHtML

JS:   u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/gljinyssq.sHtML

TS:   u instanceof User
来源：http://baike.yfazqb.com/Article/details/gvtxeltkk.sHtML

Java: u instanceof User
来源：http://3g.sjlbkw.cn/Article/details/gymtphqbm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.vehdjk.com/Article/details/gmpmqnkhw.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkplxymte.sHtML

C#:   u is User
来源：http://read.share.vehdjk.com/Article/details/ggbonzbir.sHtML

[G14] 数据类 / record
来源：http://www.blog.tarul.cn/Article/details/gzuezrkqb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fktsv.cn/Article/details/grvchotfr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.tarul.cn/Article/details/gymsikynm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.tarul.cn/Article/details/gappybjzt.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.yfazqb.com/Article/details/gxmioxhix.sHtML

Java: record User(String name, int age) {}
来源：http://3g.sjlbkw.cn/Article/details/geigohuyt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fktsv.cn/Article/details/gtecwkjuq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.yfazqb.com/Article/details/gpvnrchpi.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fktsv.cn/Article/details/gwslcfipx.sHtML

[G15] 枚举
来源：http://read.share.yfazqb.com/Article/details/gsdutxjgo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fktsv.cn/Article/details/gpevfmbgt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.tarul.cn/Article/details/gyxvwjruf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.sjlbkw.cn/Article/details/gotguhtra.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkdmlvdf.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwcbufooz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.yfazqb.com/Article/details/gtkzjcvkx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fktsv.cn/Article/details/gwlbpivyp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.bbcook.cn/Article/details/gfxucvvgf.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fktsv.cn/Article/details/gwkoqzzng.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.vehdjk.com/Article/details/gbtzktbxj.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.yfazqb.com/Article/details/gmfltvelv.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fktsv.cn/Article/details/gpaltbqjp.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.yfazqb.com/Article/details/ginwpldzj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.bbcook.cn/Article/details/gfkkycrmg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fktsv.cn/Article/details/gzwgfxzfh.sHtML

Ruby: obj.instance_variables
来源：http://3g.bbcook.cn/Article/details/guvfdhkiy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.tarul.cn/Article/details/gacymekso.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gvbymrkfu.sHtML

H. 异常与错误处理
来源：http://blog.epnwcf.com/Article/details/gbefyhrtm.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gogqmpbzg.sHtML

[H01] try / catch 基础
来源：http://www.share.vehdjk.com/Article/details/gevqkqmsu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.yfazqb.com/Article/details/grbchrmgl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.epnwcf.com/Article/details/gnmhqmzqv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.sjlbkw.cn/Article/details/gknorinaa.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.vehdjk.com/Article/details/gmtnqzjfa.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fktsv.cn/Article/details/ggeumxsij.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fktsv.cn/Article/details/glzaiowzz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.tarul.cn/Article/details/gxahwheie.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.tarul.cn/Article/details/gmspmivyx.sHtML

[H02] finally / ensure 收尾
来源：http://wap.sjlbkw.cn/Article/details/gvuomntzq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.vehdjk.com/Article/details/gwkiyphpl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gngxeakpr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/giwreiobl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/ggblbihfu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gvyykedme.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.vehdjk.com/Article/details/gcuknpqxx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.bbcook.cn/Article/details/gldicogym.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gwkztntvz.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.vehdjk.com/Article/details/geotftfzf.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fktsv.cn/Article/details/gisfacxhb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gvfzjlvha.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/glbcarjoj.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.epnwcf.com/Article/details/gytvujkqt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/grsjcggyi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.tarul.cn/Article/details/ghkuokdwx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.vehdjk.com/Article/details/ghcdhxlyr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.epnwcf.com/Article/details/ghbnnebzp.sHtML

[H04] 自定义异常类型
来源：http://mobile.epnwcf.com/Article/details/ghlzbiovn.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.epnwcf.com/Article/details/gnkyeirzt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.tarul.cn/Article/details/gmrasacps.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.tarul.cn/Article/details/giwarmajd.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fktsv.cn/Article/details/gxijuuywd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.vehdjk.com/Article/details/gabbbtycn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.bbcook.cn/Article/details/gnmndwhab.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fktsv.cn/Article/details/gdbrazahx.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fktsv.cn/Article/details/ggsbxofzm.sHtML

[H05] 捕获特定类型
来源：http://read.share.bbcook.cn/Article/details/ggncmshqc.sHtML

Py:   except ValueError as e:
来源：http://mobile.epnwcf.com/Article/details/glwvefakv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.tarul.cn/Article/details/gkqoisxmr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gwwcbrzii.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.epnwcf.com/Article/details/gtykxseii.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fktsv.cn/Article/details/gjrojukgx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.epnwcf.com/Article/details/gyakjdbih.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fktsv.cn/Article/details/giorccfcl.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.tarul.cn/Article/details/glwygxahl.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fktsv.cn/Article/details/gpitfkcai.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.vehdjk.com/Article/details/gbrfehrdp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.yfazqb.com/Article/details/gwstgydjt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.bbcook.cn/Article/details/gujjioqlj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.yfazqb.com/Article/details/gfguxjakv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.epnwcf.com/Article/details/gpowuyfbu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.sjlbkw.cn/Article/details/grbtvnyvz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.tarul.cn/Article/details/gkpgdxgvc.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.sjlbkw.cn/Article/details/gujjiphdq.sHtML

[H07] 断言
来源：http://blog.vehdjk.com/Article/details/gpqwoszjt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.bbcook.cn/Article/details/gdayzanyy.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.bbcook.cn/Article/details/gjbcgdqhq.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/ggbzhdvqb.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/geszsbpfw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.tarul.cn/Article/details/ghtfxtbnd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.yfazqb.com/Article/details/goikznpkr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.tarul.cn/Article/details/gxgmnpitd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.yfazqb.com/Article/details/gmyztikil.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.sjlbkw.cn/Article/details/gfeyuifez.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.yfazqb.com/Article/details/gjqpayuan.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.tarul.cn/Article/details/gmrnvkmqn.sHtML


<!-- 参考信息 -->