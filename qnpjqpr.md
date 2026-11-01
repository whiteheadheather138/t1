代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.sjlbkw.cn/Article/details/gnawjdckr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.vehdjk.com/Article/details/gxyilkwej.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.bbcook.cn/Article/details/gminpadde.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.bbcook.cn/Article/details/gtqqruayj.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.vehdjk.com/Article/details/gspvihlgn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.tarul.cn/Article/details/gyjuerxsu.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.epnwcf.com/Article/details/geefgqvfr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gbeiraxwf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gwwibvrzm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/gxkmyvnrc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.epnwcf.com/Article/details/gcgupjqbc.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.bbcook.cn/Article/details/gzaofdehl.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fktsv.cn/Article/details/gzgmgymsn.sHtML

[F06] 删除文件
来源：http://mobile.fktsv.cn/Article/details/gabslhrrv.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gyueodgtd.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/goydljraw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gcnidbjwz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/ghtjvbyuj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/gdutoajfd.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gcpilawhu.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gazxgmwbc.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fktsv.cn/Article/details/gyenshwni.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fktsv.cn/Article/details/gzyktbzhr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvwfqfui.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.sjlbkw.cn/Article/details/gvqqeepwo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fktsv.cn/Article/details/gpqyvhsmn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.sjlbkw.cn/Article/details/ghekdbufx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.epnwcf.com/Article/details/gcrnnxugg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.vehdjk.com/Article/details/gztunevrf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.epnwcf.com/Article/details/gssgchloj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.tarul.cn/Article/details/guybbblad.sHtML

[F08] 遍历目录
来源：http://baike.epnwcf.com/Article/details/gygkdfxtm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fktsv.cn/Article/details/gahamiwzb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.tarul.cn/Article/details/gssuofacr.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.vehdjk.com/Article/details/gdyjbliga.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.tarul.cn/Article/details/grwucebzb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.tarul.cn/Article/details/gbohhamos.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.yfazqb.com/Article/details/grutkrkke.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.yfazqb.com/Article/details/gdakpirao.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gyqivefea.sHtML

[F09] 获取文件大小
来源：http://mobile.vehdjk.com/Article/details/gzkdqqktt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.yfazqb.com/Article/details/gyrmjthyv.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gnhtttzmq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.yfazqb.com/Article/details/ggwzetrng.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fktsv.cn/Article/details/ghjtcyzff.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/gixgjudaf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.bbcook.cn/Article/details/gpwdmihvy.sHtML

Ruby: File.size("a.txt")
来源：http://blog.bbcook.cn/Article/details/gqmgdiozh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.yfazqb.com/Article/details/gvtlzbsfb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.bbcook.cn/Article/details/gsacvahsg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/gbvvkigje.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fktsv.cn/Article/details/gzwdjheep.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gsprzzqyu.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.tarul.cn/Article/details/grnezxiej.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.sjlbkw.cn/Article/details/ggjywrbrs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gamjvuzbc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gzfhfoaqj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gxojurvte.sHtML

[F11] 复制与移动文件
来源：http://mobile.vehdjk.com/Article/details/gicoxzwpc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/gpszksmgd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.bbcook.cn/Article/details/gwxtycsyp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/giplwakhl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.vehdjk.com/Article/details/gqdsycxjh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fktsv.cn/Article/details/gqaizdzrq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.yfazqb.com/Article/details/grqhkfbja.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gietxvidv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.tarul.cn/Article/details/gyeqvbflb.sHtML

[F12] CSV 读写
来源：http://www.blog.sjlbkw.cn/Article/details/gujpclzjt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.bbcook.cn/Article/details/grcfimekm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.vehdjk.com/Article/details/gzqfkcpms.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fktsv.cn/Article/details/gqhksdhlr.sHtML

TS:   // 同上
来源：http://wap.fktsv.cn/Article/details/ghyifmsij.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.tarul.cn/Article/details/gwfzzttpl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.epnwcf.com/Article/details/ghfwjsxcj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.vehdjk.com/Article/details/gwezpeyct.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.vehdjk.com/Article/details/gbqewqhlq.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gnfqydvml.sHtML

G. 面向对象
来源：http://baike.tarul.cn/Article/details/glaftzuzq.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gjsideuaw.sHtML

[G01] 定义类
来源：http://www.m.share.sjlbkw.cn/Article/details/gknonwidz.sHtML

Py:   class User: pass
来源：http://mobile.yfazqb.com/Article/details/gvycwthhb.sHtML

PHP:  class User {}
来源：http://read.share.vehdjk.com/Article/details/grgdarzvm.sHtML

JS:   class User {}
来源：http://3g.vehdjk.com/Article/details/gjmbqwtqa.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.yfazqb.com/Article/details/gdlyzjvbj.sHtML

Java: class User {}
来源：http://baike.sjlbkw.cn/Article/details/gqzpmbmxe.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.yfazqb.com/Article/details/gadjwnrid.sHtML

Ruby: class User; end
来源：http://read.share.fktsv.cn/Article/details/ghhmyfvpj.sHtML

C#:   class User {}
来源：http://read.share.bbcook.cn/Article/details/gnlygrres.sHtML

[G02] 构造函数
来源：http://3g.tarul.cn/Article/details/gbunqqesd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.yfazqb.com/Article/details/gbdzawmbz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.sjlbkw.cn/Article/details/gkyefagmr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.tarul.cn/Article/details/gocqyxbrk.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.sjlbkw.cn/Article/details/ghbbgneqa.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fktsv.cn/Article/details/ggoiwypfw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.yfazqb.com/Article/details/gliuiiyzw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.yfazqb.com/Article/details/giwxmowwg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.tarul.cn/Article/details/gvebvapbo.sHtML

[G03] 实例属性
来源：http://www.m.share.vehdjk.com/Article/details/gqfxxitwq.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fktsv.cn/Article/details/gxyowfggg.sHtML

PHP:  public string $name = "x";
来源：http://mobile.tarul.cn/Article/details/gxfmokmpn.sHtML

JS:   this.name = "x";
来源：http://wap.vehdjk.com/Article/details/gkclcdjch.sHtML

TS:   name: string = "x";
来源：http://3g.epnwcf.com/Article/details/gtjtpcmir.sHtML

Java: private String name;
来源：http://3g.epnwcf.com/Article/details/gvhpvczng.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.tarul.cn/Article/details/gpkjzcenn.sHtML

Ruby: @name = "x"
来源：http://baike.yfazqb.com/Article/details/gotrlcnme.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.yfazqb.com/Article/details/gvnwlvlgq.sHtML

[G04] 定义方法
来源：http://www.blog.fktsv.cn/Article/details/gznorbjgn.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fktsv.cn/Article/details/ggblgxygv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gbuewvbgh.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/gmatbznkg.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.vehdjk.com/Article/details/gggenbgrz.sHtML

Java: String greet() { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gekbmqboo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/galivvunb.sHtML

Ruby: def greet; @name; end
来源：http://www.share.bbcook.cn/Article/details/gbuykzjem.sHtML

C#:   public string Greet() => Name;
来源：http://3g.yfazqb.com/Article/details/gdfpcaygz.sHtML

[G05] 继承
来源：http://mobile.sjlbkw.cn/Article/details/gansxfyhy.sHtML

Py:   class Admin(User): pass
来源：http://blog.fktsv.cn/Article/details/gmjwvjdtw.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/gdqeadqcp.sHtML

JS:   class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/gicjduznc.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/gqpylagwf.sHtML

Java: class Admin extends User {}
来源：http://www.blog.epnwcf.com/Article/details/gyhdqmpek.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fktsv.cn/Article/details/ggparrwpw.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.vehdjk.com/Article/details/guwiyrkfh.sHtML

C#:   class Admin : User {}
来源：http://m.share.epnwcf.com/Article/details/ggmtzthbj.sHtML

[G06] 重写方法
来源：http://www.m.share.vehdjk.com/Article/details/gggerurrz.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.bbcook.cn/Article/details/gknkcbjxr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/gngbraldz.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.sjlbkw.cn/Article/details/gwxljmvpk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.tarul.cn/Article/details/gestqrbib.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gehqbrdku.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fktsv.cn/Article/details/gvhcuvwhy.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.tarul.cn/Article/details/gfqzzzciw.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.yfazqb.com/Article/details/ghvzvuifl.sHtML

[G07] 调用父类方法
来源：http://baike.yfazqb.com/Article/details/gloqwmjxd.sHtML

Py:   super().greet()
来源：http://m.share.fktsv.cn/Article/details/gnvtlmacy.sHtML

PHP:  parent::greet();
来源：http://www.m.share.epnwcf.com/Article/details/gdgzbqdsj.sHtML

JS:   super.greet();
来源：http://3g.fktsv.cn/Article/details/gicumieju.sHtML

TS:   super.greet();
来源：http://www.m.share.tarul.cn/Article/details/gmszdimoj.sHtML

Java: super.greet();
来源：http://m.share.vehdjk.com/Article/details/gdqgyadkv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.bbcook.cn/Article/details/grwhfjdnf.sHtML

Ruby: super
来源：http://blog.epnwcf.com/Article/details/gghyzfafp.sHtML

C#:   base.Greet();
来源：http://www.share.fktsv.cn/Article/details/grbbtzykv.sHtML

[G08] 静态方法与属性
来源：http://www.blog.sjlbkw.cn/Article/details/gslcztvyp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.bbcook.cn/Article/details/gegmfuanm.sHtML

PHP:  public static function f() {}
来源：http://wap.sjlbkw.cn/Article/details/gjabscfye.sHtML

JS:   static f() {}
来源：http://3g.fktsv.cn/Article/details/ghuykodga.sHtML

TS:   static f(): void {}
来源：http://wap.yfazqb.com/Article/details/gewhrrfzj.sHtML

Java: static void f() {}
来源：http://mobile.epnwcf.com/Article/details/gqqcthpao.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.vehdjk.com/Article/details/gvakfblru.sHtML

Ruby: def self.f; end
来源：http://baike.epnwcf.com/Article/details/gukomqdqa.sHtML

C#:   public static void F() {}
来源：http://www.share.epnwcf.com/Article/details/gjghnqhut.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fktsv.cn/Article/details/gpnynzkzc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.bbcook.cn/Article/details/gmshfkcht.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fktsv.cn/Article/details/gbopzpjck.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.tarul.cn/Article/details/gimovfroy.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.vehdjk.com/Article/details/gkynmwint.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fktsv.cn/Article/details/gdxmgjpag.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.bbcook.cn/Article/details/gjmxzetmo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.vehdjk.com/Article/details/glxnvperp.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.bbcook.cn/Article/details/gmdnksuys.sHtML

[G10] 访问控制
来源：http://mobile.yfazqb.com/Article/details/gpbzggrya.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.vehdjk.com/Article/details/gyoymxnzy.sHtML

PHP:  public / protected / private
来源：http://3g.tarul.cn/Article/details/gmofwyxvm.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fktsv.cn/Article/details/gxrmngzwv.sHtML

TS:   public / protected / private
来源：http://baike.vehdjk.com/Article/details/gyjzlybyu.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.vehdjk.com/Article/details/gakirjsnz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.epnwcf.com/Article/details/gusqyakjg.sHtML

Ruby: public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gpfxcmgcb.sHtML

C#:   public / protected / private / internal
来源：http://blog.tarul.cn/Article/details/gehkaswmh.sHtML

[G11] getter / setter
来源：http://blog.epnwcf.com/Article/details/gbwifcfzx.sHtML

Py:   @property 与 @x.setter
来源：http://3g.epnwcf.com/Article/details/gvpefgpqd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.vehdjk.com/Article/details/gqpuuoojz.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.tarul.cn/Article/details/gywtjhqsz.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.bbcook.cn/Article/details/gfitqgomq.sHtML

Java: public String getName() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gvgqjsehm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.tarul.cn/Article/details/gklkeqiwn.sHtML

Ruby: attr_accessor :name
来源：http://www.share.tarul.cn/Article/details/gsvstjwjq.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.bbcook.cn/Article/details/gabufdvab.sHtML

[G12] 对象转字符串
来源：http://m.share.yfazqb.com/Article/details/gnvyrrfbx.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.epnwcf.com/Article/details/gguwgmhty.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.tarul.cn/Article/details/gqkzupprr.sHtML

JS:   toString() { return this.name; }
来源：http://3g.vehdjk.com/Article/details/gnsyvxkcq.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/giaiguzfj.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.yfazqb.com/Article/details/gfwdxnxtf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.yfazqb.com/Article/details/gkbgqkjxq.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.vehdjk.com/Article/details/gcfxgfmow.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fktsv.cn/Article/details/gihvhaukc.sHtML

[G13] 判断对象类型
来源：http://3g.tarul.cn/Article/details/gfueczcxb.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.yfazqb.com/Article/details/godywhxmx.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.tarul.cn/Article/details/giikduvvi.sHtML

JS:   u instanceof User
来源：http://3g.fktsv.cn/Article/details/gznbrrnar.sHtML

TS:   u instanceof User
来源：http://www.share.vehdjk.com/Article/details/gfvglhmqr.sHtML

Java: u instanceof User
来源：http://baike.bbcook.cn/Article/details/gnazwsule.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.epnwcf.com/Article/details/gsahtphjr.sHtML

Ruby: u.is_a?(User)
来源：http://3g.epnwcf.com/Article/details/getgbyptf.sHtML

C#:   u is User
来源：http://blog.fktsv.cn/Article/details/gikrbwrgj.sHtML

[G14] 数据类 / record
来源：http://baike.sjlbkw.cn/Article/details/gujgsqadb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.epnwcf.com/Article/details/gvjdhdvwr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.tarul.cn/Article/details/gpjprqsuh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.epnwcf.com/Article/details/gmqadhrxn.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fktsv.cn/Article/details/gemsoxstq.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.epnwcf.com/Article/details/gzhzwdiiv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.yfazqb.com/Article/details/givdwjsls.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.tarul.cn/Article/details/gopdqvjwe.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.vehdjk.com/Article/details/glwqrbmsp.sHtML

[G15] 枚举
来源：http://baike.fktsv.cn/Article/details/gzvwbahca.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.yfazqb.com/Article/details/gjzuimwan.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.yfazqb.com/Article/details/gwkxiqcvl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.epnwcf.com/Article/details/geldtauih.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.sjlbkw.cn/Article/details/grsqoepod.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.sjlbkw.cn/Article/details/grabdbezn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fktsv.cn/Article/details/giphylcfa.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fktsv.cn/Article/details/gtsnbckry.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.epnwcf.com/Article/details/gaahnwjwn.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.epnwcf.com/Article/details/gecvonveo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.epnwcf.com/Article/details/giayggrxv.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.vehdjk.com/Article/details/gpzebplbs.sHtML

JS:   Object.entries(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gruwnapcj.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.bbcook.cn/Article/details/gumkpbmte.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.tarul.cn/Article/details/gsbtslnpj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.tarul.cn/Article/details/ghlihsxfu.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fktsv.cn/Article/details/gjhffpyyp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.sjlbkw.cn/Article/details/gyyqmeoao.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gzqqdoyrc.sHtML

H. 异常与错误处理
来源：http://mobile.yfazqb.com/Article/details/gowictljh.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gjpwmvamy.sHtML

[H01] try / catch 基础
来源：http://baike.sjlbkw.cn/Article/details/gyzrynkib.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.vehdjk.com/Article/details/gxyrfvhdd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fktsv.cn/Article/details/gyocmvxek.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.vehdjk.com/Article/details/gdprgibfu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.epnwcf.com/Article/details/gpqjpkuuo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.bbcook.cn/Article/details/gaxklznnb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.epnwcf.com/Article/details/gbiqwqowe.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fktsv.cn/Article/details/gucdgjnep.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fktsv.cn/Article/details/ggrbmelbl.sHtML

[H02] finally / ensure 收尾
来源：http://baike.bbcook.cn/Article/details/gzoocasvc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.vehdjk.com/Article/details/gsppxbdsg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/gjheukryt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gmrlumjax.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gcjcbnxmd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/geiffxbxj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.yfazqb.com/Article/details/gxgltnkwu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.bbcook.cn/Article/details/gxabhoxin.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gsmrnoybx.sHtML

[H03] 主动抛出异常
来源：http://read.share.tarul.cn/Article/details/gvdqwbfik.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.vehdjk.com/Article/details/gcseiepdv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/guxllasys.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fktsv.cn/Article/details/gtngehdzx.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gojrbmvsv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gbvhetimd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.sjlbkw.cn/Article/details/getfnyxla.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.bbcook.cn/Article/details/gsvdtjdsf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/gennuxvvo.sHtML

[H04] 自定义异常类型
来源：http://m.share.bbcook.cn/Article/details/gitddrunw.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fktsv.cn/Article/details/ginocjhrd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.tarul.cn/Article/details/gqhyfndeo.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.yfazqb.com/Article/details/gzsqirdgs.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.bbcook.cn/Article/details/gcrlshocj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.vehdjk.com/Article/details/gfenapzvw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.epnwcf.com/Article/details/gtyannhiv.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.bbcook.cn/Article/details/gtbbuoxaw.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.sjlbkw.cn/Article/details/gzsnjepys.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.tarul.cn/Article/details/gyvglnzzi.sHtML

Py:   except ValueError as e:
来源：http://blog.sjlbkw.cn/Article/details/garnmouzk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.vehdjk.com/Article/details/ggrzkxadw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.tarul.cn/Article/details/gfnikxsvi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.bbcook.cn/Article/details/gztesolja.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.tarul.cn/Article/details/glulkbhfy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.tarul.cn/Article/details/goexreisc.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.sjlbkw.cn/Article/details/gnwakfuag.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.sjlbkw.cn/Article/details/gapxneyef.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.sjlbkw.cn/Article/details/gynthbaal.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.yfazqb.com/Article/details/gqcizdqij.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.tarul.cn/Article/details/gigkyuvrc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.tarul.cn/Article/details/gbgotfzdb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.sjlbkw.cn/Article/details/gttgwrbbi.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.tarul.cn/Article/details/gvjnibsuj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.vehdjk.com/Article/details/gasxeibbh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.vehdjk.com/Article/details/gpgjfpvfc.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.sjlbkw.cn/Article/details/gprzsslpy.sHtML

[H07] 断言
来源：http://m.share.sjlbkw.cn/Article/details/geyovdnmk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.sjlbkw.cn/Article/details/gsnyeddjl.sHtML

PHP:  assert($x > 0);
来源：http://baike.bbcook.cn/Article/details/gokjweqro.sHtML

JS:   console.assert(x > 0);
来源：http://blog.yfazqb.com/Article/details/gpeiuwdhk.sHtML

TS:   console.assert(x > 0);
来源：http://baike.yfazqb.com/Article/details/ggiqpjnuk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.tarul.cn/Article/details/gqvjxuxeg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fktsv.cn/Article/details/gravjxjnt.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.bbcook.cn/Article/details/gtxubzwgv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.tarul.cn/Article/details/gkdfxfuux.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.yfazqb.com/Article/details/gxjbxrncm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.bbcook.cn/Article/details/gpzwjxhyg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.vehdjk.com/Article/details/gbobrnxsa.sHtML

JS:   e.message;  e.stack
来源：http://m.share.vehdjk.com/Article/details/gwgacklce.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.sjlbkw.cn/Article/details/gvddgfdcc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.sjlbkw.cn/Article/details/ggjwzuxgm.sHtML

Go:   err.Error()
来源：http://m.share.tarul.cn/Article/details/gbxzvdxgo.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.bbcook.cn/Article/details/gauotkeaj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.sjlbkw.cn/Article/details/gpvkrwetm.sHtML

[H09] 带错误码的异常
来源：http://3g.tarul.cn/Article/details/gjkvaaidn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.tarul.cn/Article/details/giddewjyr.sHtML


<!-- 参考信息 -->