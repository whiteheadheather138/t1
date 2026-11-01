代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.yfazqb.com/Article/details/ghjiqqolu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.tarul.cn/Article/details/gzxktofjs.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.sjlbkw.cn/Article/details/grhzknxqi.sHtML

[F04] 追加写入文件
来源：http://www.blog.vehdjk.com/Article/details/gdlvuthdm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.tarul.cn/Article/details/gqlryprto.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.epnwcf.com/Article/details/gtdhzuhon.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.sjlbkw.cn/Article/details/gehpkhjic.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.yfazqb.com/Article/details/gtylawrih.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.sjlbkw.cn/Article/details/ghfxopdue.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.vehdjk.com/Article/details/guoxbcepb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxihtayuv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.tarul.cn/Article/details/gzstbnmkv.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.sjlbkw.cn/Article/details/gfxrorpzj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.bbcook.cn/Article/details/gexdkaule.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fktsv.cn/Article/details/gtumlzzqi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/gjungnyhq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gzqqekrcq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/gesxlwhqn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.tarul.cn/Article/details/gvxmnoiir.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.yfazqb.com/Article/details/gjknbcnwz.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.yfazqb.com/Article/details/gjikpfqdz.sHtML

[F06] 删除文件
来源：http://www.blog.sjlbkw.cn/Article/details/gpszjtitc.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/giqujxhtv.sHtML

PHP:  unlink("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gccjkmkvx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwzwyxizk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gltjgkoyi.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/gvgcejmva.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/guztpnzgz.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gqyvmfevx.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gpzobgahe.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.sjlbkw.cn/Article/details/gjcfcayib.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.bbcook.cn/Article/details/geylvvceu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.bbcook.cn/Article/details/gcplflgue.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.bbcook.cn/Article/details/gmdhegzlq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fktsv.cn/Article/details/gsefgsica.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.sjlbkw.cn/Article/details/gugmqeonj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fktsv.cn/Article/details/gqohfwmcb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.bbcook.cn/Article/details/gaihrvfbq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.tarul.cn/Article/details/gszlsxxso.sHtML

[F08] 遍历目录
来源：http://www.share.yfazqb.com/Article/details/glissafpb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.tarul.cn/Article/details/gzjkmxdxs.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.epnwcf.com/Article/details/gpnjgqccf.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fktsv.cn/Article/details/gkxyzwflq.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.vehdjk.com/Article/details/gutacszrn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.yfazqb.com/Article/details/gplkqjdpc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.tarul.cn/Article/details/gbianbdui.sHtML

Ruby: Dir.children("dir")
来源：http://baike.sjlbkw.cn/Article/details/gvpopecdg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.sjlbkw.cn/Article/details/geatvxmbi.sHtML

[F09] 获取文件大小
来源：http://mobile.fktsv.cn/Article/details/gdzzmvjvq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gnecthnml.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gxjmzxvnd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.epnwcf.com/Article/details/ghciqbxun.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.epnwcf.com/Article/details/gxlnbduky.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/gqbwulqoa.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.vehdjk.com/Article/details/gbaobznlz.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gpkoihmgr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.vehdjk.com/Article/details/gmdybngrx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.vehdjk.com/Article/details/ghwzsqgtd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/gxtiuxcul.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gnpkzsvtc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gjyodtdtq.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gwggdtbdo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.bbcook.cn/Article/details/gelekjsbu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gtgdkxemv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gerlwczzb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gepzwzdpk.sHtML

[F11] 复制与移动文件
来源：http://3g.vehdjk.com/Article/details/grqtlolpo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gcylqssbg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gwggkjcxf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gmhydplud.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.yfazqb.com/Article/details/gxjaleomc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.sjlbkw.cn/Article/details/gygbkvogo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.sjlbkw.cn/Article/details/gcjymkotr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/gggvyirhm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.vehdjk.com/Article/details/gmtgtsykk.sHtML

[F12] CSV 读写
来源：http://read.share.bbcook.cn/Article/details/gwtuwmkxq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.tarul.cn/Article/details/gewiazcsr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fktsv.cn/Article/details/gjdwemwkv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.vehdjk.com/Article/details/gwevxjwwz.sHtML

TS:   // 同上
来源：http://www.blog.tarul.cn/Article/details/glmlfgars.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.epnwcf.com/Article/details/gvrtdjvjx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.vehdjk.com/Article/details/gnqrkjzdk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.bbcook.cn/Article/details/gdqkmddom.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.bbcook.cn/Article/details/grqkscugs.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gqfzdzyvz.sHtML

G. 面向对象
来源：http://baike.vehdjk.com/Article/details/gssopywpp.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gqmigbirr.sHtML

[G01] 定义类
来源：http://mobile.tarul.cn/Article/details/gjjczpsjl.sHtML

Py:   class User: pass
来源：http://mobile.bbcook.cn/Article/details/gfxdqrdqw.sHtML

PHP:  class User {}
来源：http://baike.vehdjk.com/Article/details/gnbdukilk.sHtML

JS:   class User {}
来源：http://mobile.sjlbkw.cn/Article/details/gijjsiwro.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.sjlbkw.cn/Article/details/gfpygjevp.sHtML

Java: class User {}
来源：http://mobile.tarul.cn/Article/details/gwwqmvxhn.sHtML

Go:   type User struct { Name string }
来源：http://blog.fktsv.cn/Article/details/gcuzmxyjw.sHtML

Ruby: class User; end
来源：http://3g.vehdjk.com/Article/details/groyixqqi.sHtML

C#:   class User {}
来源：http://blog.tarul.cn/Article/details/gnonqtmdf.sHtML

[G02] 构造函数
来源：http://m.share.vehdjk.com/Article/details/gymwazazi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fktsv.cn/Article/details/gsoxhtgqz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.epnwcf.com/Article/details/gmopljaym.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/giugrkzjk.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fktsv.cn/Article/details/gfikdcnch.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.tarul.cn/Article/details/ghyqcwabt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fktsv.cn/Article/details/gtjdicrma.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.yfazqb.com/Article/details/ghvwwmezb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.tarul.cn/Article/details/gtnxouzba.sHtML

[G03] 实例属性
来源：http://www.m.share.fktsv.cn/Article/details/grirpkdqx.sHtML

Py:   self.name = "x"
来源：http://www.share.tarul.cn/Article/details/gmnzhuwpj.sHtML

PHP:  public string $name = "x";
来源：http://3g.vehdjk.com/Article/details/gjtakcjti.sHtML

JS:   this.name = "x";
来源：http://mobile.vehdjk.com/Article/details/gqfqzurfw.sHtML

TS:   name: string = "x";
来源：http://www.blog.tarul.cn/Article/details/gvxuicrux.sHtML

Java: private String name;
来源：http://www.m.share.vehdjk.com/Article/details/gscsstnur.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fktsv.cn/Article/details/gfmqzqubl.sHtML

Ruby: @name = "x"
来源：http://baike.epnwcf.com/Article/details/gnbpuxcsp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.bbcook.cn/Article/details/gjfnphaio.sHtML

[G04] 定义方法
来源：http://3g.bbcook.cn/Article/details/gubzuubxa.sHtML

Py:   def greet(self): return self.name
来源：http://3g.vehdjk.com/Article/details/gwzntdvvc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.vehdjk.com/Article/details/gjhyvqtku.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gbyztmkwt.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.tarul.cn/Article/details/gapvpvrhw.sHtML

Java: String greet() { return name; }
来源：http://www.blog.epnwcf.com/Article/details/gddotissl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.tarul.cn/Article/details/gagtwlrld.sHtML

Ruby: def greet; @name; end
来源：http://3g.fktsv.cn/Article/details/geavcejit.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.tarul.cn/Article/details/gzwolsjsq.sHtML

[G05] 继承
来源：http://wap.yfazqb.com/Article/details/gafzjjshx.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.vehdjk.com/Article/details/gkwnmgqoc.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gyfithsqa.sHtML

JS:   class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/gdhehusxq.sHtML

TS:   class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/gxsfykyuv.sHtML

Java: class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/gdhzvzfpu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fktsv.cn/Article/details/gurjrqisg.sHtML

Ruby: class Admin < User; end
来源：http://read.share.sjlbkw.cn/Article/details/gajtxkaoz.sHtML

C#:   class Admin : User {}
来源：http://read.share.yfazqb.com/Article/details/glubfjujd.sHtML

[G06] 重写方法
来源：http://www.blog.yfazqb.com/Article/details/grkgjgqxs.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.yfazqb.com/Article/details/gmetflmpn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/gjljojphy.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/gkmhczppn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gnqggadar.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/gwfdbdgrb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.bbcook.cn/Article/details/gubkwyiqf.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.epnwcf.com/Article/details/gizygzjgi.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.yfazqb.com/Article/details/gvknzmtqv.sHtML

[G07] 调用父类方法
来源：http://www.blog.bbcook.cn/Article/details/gkdrcvlqn.sHtML

Py:   super().greet()
来源：http://blog.vehdjk.com/Article/details/gvffhfbgn.sHtML

PHP:  parent::greet();
来源：http://wap.bbcook.cn/Article/details/giyjakvbs.sHtML

JS:   super.greet();
来源：http://baike.epnwcf.com/Article/details/gtvdfdugu.sHtML

TS:   super.greet();
来源：http://www.m.share.fktsv.cn/Article/details/ggfsrzsgj.sHtML

Java: super.greet();
来源：http://www.blog.vehdjk.com/Article/details/gwqvccnis.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.bbcook.cn/Article/details/gpvspxach.sHtML

Ruby: super
来源：http://3g.fktsv.cn/Article/details/gnyzxogcu.sHtML

C#:   base.Greet();
来源：http://wap.sjlbkw.cn/Article/details/gesuuydbe.sHtML

[G08] 静态方法与属性
来源：http://blog.yfazqb.com/Article/details/gpcdhidem.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.vehdjk.com/Article/details/gsgiwcsnd.sHtML

PHP:  public static function f() {}
来源：http://3g.sjlbkw.cn/Article/details/gviwimava.sHtML

JS:   static f() {}
来源：http://baike.bbcook.cn/Article/details/glwtslllm.sHtML

TS:   static f(): void {}
来源：http://mobile.fktsv.cn/Article/details/gxjjtvcpa.sHtML

Java: static void f() {}
来源：http://mobile.fktsv.cn/Article/details/gotxkuxzt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.yfazqb.com/Article/details/garrnnttg.sHtML

Ruby: def self.f; end
来源：http://www.share.epnwcf.com/Article/details/gjbjklmpz.sHtML

C#:   public static void F() {}
来源：http://www.blog.tarul.cn/Article/details/gbqmyplfr.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.sjlbkw.cn/Article/details/gnhcvqgww.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.bbcook.cn/Article/details/gjrnmnvko.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.epnwcf.com/Article/details/gonpzogzs.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.yfazqb.com/Article/details/gdjtkoalj.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.tarul.cn/Article/details/glkbxrpcd.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.tarul.cn/Article/details/gqfwihmbh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.vehdjk.com/Article/details/gfjwcsoyg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.epnwcf.com/Article/details/goyhbeann.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fktsv.cn/Article/details/gxoxigtsg.sHtML

[G10] 访问控制
来源：http://www.blog.vehdjk.com/Article/details/goevdxeka.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.yfazqb.com/Article/details/gcffgipjb.sHtML

PHP:  public / protected / private
来源：http://baike.tarul.cn/Article/details/gupwgvixy.sHtML

JS:   #private 字段；其余公开
来源：http://3g.sjlbkw.cn/Article/details/gcmtleuvi.sHtML

TS:   public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/gggkvvnjb.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.vehdjk.com/Article/details/gvfqkjqfd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.bbcook.cn/Article/details/gfggmfkvm.sHtML

Ruby: public / protected / private
来源：http://wap.tarul.cn/Article/details/gumknjmml.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.yfazqb.com/Article/details/gzrxskknr.sHtML

[G11] getter / setter
来源：http://blog.yfazqb.com/Article/details/gwnslaiuf.sHtML

Py:   @property 与 @x.setter
来源：http://blog.sjlbkw.cn/Article/details/gvafcphfq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.yfazqb.com/Article/details/gfjskssrr.sHtML

JS:   get name() { return this._name; }
来源：http://3g.bbcook.cn/Article/details/gmrsvrnjx.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.epnwcf.com/Article/details/gsetzszzy.sHtML

Java: public String getName() { return name; }
来源：http://3g.fktsv.cn/Article/details/gcmwhmiin.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gqxbiesqr.sHtML

Ruby: attr_accessor :name
来源：http://3g.fktsv.cn/Article/details/gnchnrubu.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.epnwcf.com/Article/details/gllnzwsqo.sHtML

[G12] 对象转字符串
来源：http://3g.yfazqb.com/Article/details/gizynxvyy.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.tarul.cn/Article/details/gxpitmvbd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.sjlbkw.cn/Article/details/goxdntvsa.sHtML

JS:   toString() { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gnuvotfzs.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gstojdzqv.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.vehdjk.com/Article/details/gxvetesdd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.vehdjk.com/Article/details/gjxsjxmvk.sHtML

Ruby: def to_s; @name; end
来源：http://3g.tarul.cn/Article/details/gymyontif.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.vehdjk.com/Article/details/gnpbmuasf.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fktsv.cn/Article/details/greuhmgpt.sHtML

Py:   isinstance(u, User)
来源：http://read.share.tarul.cn/Article/details/gctomhasm.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.yfazqb.com/Article/details/ghgozpyjz.sHtML

JS:   u instanceof User
来源：http://m.share.vehdjk.com/Article/details/gtoklurva.sHtML

TS:   u instanceof User
来源：http://m.share.bbcook.cn/Article/details/gygolfcmo.sHtML

Java: u instanceof User
来源：http://baike.yfazqb.com/Article/details/giaocjsbb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.yfazqb.com/Article/details/grwsbqkvn.sHtML

Ruby: u.is_a?(User)
来源：http://wap.vehdjk.com/Article/details/gqcncvxbh.sHtML

C#:   u is User
来源：http://www.m.share.bbcook.cn/Article/details/ggmgohaip.sHtML

[G14] 数据类 / record
来源：http://m.share.vehdjk.com/Article/details/gzyexiirg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.epnwcf.com/Article/details/gehtvqjmi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fktsv.cn/Article/details/gcdgrpnba.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.yfazqb.com/Article/details/gexzanhvx.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.epnwcf.com/Article/details/gauhiqyfp.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.yfazqb.com/Article/details/gvmkqpzcy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.sjlbkw.cn/Article/details/glzxxdith.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.tarul.cn/Article/details/glytjisgy.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.bbcook.cn/Article/details/gumrbspxg.sHtML

[G15] 枚举
来源：http://mobile.fktsv.cn/Article/details/grsikrxdq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.yfazqb.com/Article/details/gucltboao.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.bbcook.cn/Article/details/ghnjovfuc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fktsv.cn/Article/details/gbgqekjpd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fktsv.cn/Article/details/gsusfabdo.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.bbcook.cn/Article/details/gaozysogb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.yfazqb.com/Article/details/ggewwxuph.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.vehdjk.com/Article/details/gtxdaqnfb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.sjlbkw.cn/Article/details/gisjbizpm.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.sjlbkw.cn/Article/details/gutxopwtc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.epnwcf.com/Article/details/gopuoqruk.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.tarul.cn/Article/details/gkfhfouey.sHtML

JS:   Object.entries(obj)
来源：http://mobile.epnwcf.com/Article/details/gydtdqyvt.sHtML

TS:   Object.entries(obj)
来源：http://m.share.vehdjk.com/Article/details/gcljdntva.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.bbcook.cn/Article/details/ghqjnmoxn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.epnwcf.com/Article/details/gxnmcnbzc.sHtML

Ruby: obj.instance_variables
来源：http://wap.epnwcf.com/Article/details/gfiowbmkt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.bbcook.cn/Article/details/giffmgujd.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gnvgxzlgk.sHtML

H. 异常与错误处理
来源：http://wap.yfazqb.com/Article/details/gxrtjimut.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gnndjfcso.sHtML

[H01] try / catch 基础
来源：http://read.share.yfazqb.com/Article/details/ghqdpehbe.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.vehdjk.com/Article/details/gbmtzhbbb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fktsv.cn/Article/details/gwcaapatc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.vehdjk.com/Article/details/gzulylkuk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.epnwcf.com/Article/details/gdiilycfd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.tarul.cn/Article/details/gayovgsjy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.bbcook.cn/Article/details/gxzbayhpy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.epnwcf.com/Article/details/gqjeibhie.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fktsv.cn/Article/details/gxtpstpmp.sHtML

[H02] finally / ensure 收尾
来源：http://wap.tarul.cn/Article/details/gipmotktr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.tarul.cn/Article/details/ggtjaqbkl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.tarul.cn/Article/details/govdhfsgq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/grywscknk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gpyzkvejw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gdaguqpod.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.vehdjk.com/Article/details/gdmoeyvgb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.bbcook.cn/Article/details/gyyzcvagg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gigonakxm.sHtML

[H03] 主动抛出异常
来源：http://baike.fktsv.cn/Article/details/gxplahvpb.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.yfazqb.com/Article/details/glmvdyubk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.tarul.cn/Article/details/glgxjmvft.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fktsv.cn/Article/details/gepyrmcig.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.epnwcf.com/Article/details/gkzdaenks.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.yfazqb.com/Article/details/ggpvzdxjv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.vehdjk.com/Article/details/gnkhlfzqp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fktsv.cn/Article/details/gynawyjow.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.tarul.cn/Article/details/guornqhlh.sHtML

[H04] 自定义异常类型
来源：http://www.blog.yfazqb.com/Article/details/gxgsnmacv.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.vehdjk.com/Article/details/gpzaaiujx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.bbcook.cn/Article/details/gqnumlbzl.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.vehdjk.com/Article/details/gbonzbmbp.sHtML

TS:   class MyError extends Error {}
来源：http://3g.tarul.cn/Article/details/gauuwwgqw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.yfazqb.com/Article/details/gyvweweqj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.tarul.cn/Article/details/gtvbyzanx.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.yfazqb.com/Article/details/gclhulwrt.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.yfazqb.com/Article/details/gchkrrqqd.sHtML

[H05] 捕获特定类型
来源：http://m.share.fktsv.cn/Article/details/gujslfyxh.sHtML

Py:   except ValueError as e:
来源：http://3g.sjlbkw.cn/Article/details/gideqtxkq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.yfazqb.com/Article/details/geocpxado.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fktsv.cn/Article/details/gshmsenex.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.bbcook.cn/Article/details/gntvoonhd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.epnwcf.com/Article/details/gizunzvsu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.epnwcf.com/Article/details/gbmklpgxl.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.yfazqb.com/Article/details/gbirxwokf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.epnwcf.com/Article/details/gqsohgurw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.bbcook.cn/Article/details/giprnffuv.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.epnwcf.com/Article/details/ghogsmhvv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fktsv.cn/Article/details/gfrkssgvf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.sjlbkw.cn/Article/details/ghavoubvk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.sjlbkw.cn/Article/details/gyremcrdt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.vehdjk.com/Article/details/gthrhrxjh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.bbcook.cn/Article/details/goegfyqwo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.epnwcf.com/Article/details/gqziizisn.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.tarul.cn/Article/details/gzkcllriy.sHtML

[H07] 断言
来源：http://mobile.vehdjk.com/Article/details/gjbetkrdc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.tarul.cn/Article/details/gpdsabscz.sHtML

PHP:  assert($x > 0);
来源：http://baike.bbcook.cn/Article/details/gyjyidzrc.sHtML

JS:   console.assert(x > 0);
来源：http://3g.epnwcf.com/Article/details/glcocpjce.sHtML

TS:   console.assert(x > 0);
来源：http://3g.sjlbkw.cn/Article/details/gvcucrmao.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.sjlbkw.cn/Article/details/gzaxtcwcg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.sjlbkw.cn/Article/details/gqrgridlv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.sjlbkw.cn/Article/details/gqrnsxkul.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.tarul.cn/Article/details/gtnhelirk.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.vehdjk.com/Article/details/gzwnngscv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.bbcook.cn/Article/details/grsylfiam.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.yfazqb.com/Article/details/gfoedhwkl.sHtML


<!-- 参考信息 -->