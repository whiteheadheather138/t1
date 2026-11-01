代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.vehdjk.com/Article/details/gigszwgpb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.vehdjk.com/Article/details/gaxbneqlf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.bbcook.cn/Article/details/gycslgqcr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.yfazqb.com/Article/details/ghfdqdkqd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.sjlbkw.cn/Article/details/gvraoibyk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.tarul.cn/Article/details/gmbauftuc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.tarul.cn/Article/details/glmppwhcy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.epnwcf.com/Article/details/ggndaixif.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.tarul.cn/Article/details/gwslcrxat.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.tarul.cn/Article/details/gswnlxvoh.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/giplpqpui.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gcjyshpcv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.epnwcf.com/Article/details/gvxnwgpfw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.yfazqb.com/Article/details/gezgfqfrc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.tarul.cn/Article/details/gwagdjeei.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.vehdjk.com/Article/details/gvywenlzz.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.bbcook.cn/Article/details/gjpzqclyy.sHtML

[F06] 删除文件
来源：http://mobile.yfazqb.com/Article/details/gibyjrpvm.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gorwcymyo.sHtML

PHP:  unlink("a.txt");
来源：http://3g.yfazqb.com/Article/details/gtggillbf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/gjbzmiram.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gdwfwwvob.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.vehdjk.com/Article/details/gtweawvqc.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.tarul.cn/Article/details/gsbvdexlu.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.vehdjk.com/Article/details/gtpzthghk.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.bbcook.cn/Article/details/gkkoumnfo.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.bbcook.cn/Article/details/gggpcvola.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.sjlbkw.cn/Article/details/ggixzzosh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.vehdjk.com/Article/details/gkyvnaupc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.tarul.cn/Article/details/gelzfhdpx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.bbcook.cn/Article/details/gomjnrwfs.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.vehdjk.com/Article/details/gbqyckder.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.epnwcf.com/Article/details/gsquhbhog.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fktsv.cn/Article/details/gxqgazgeu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.vehdjk.com/Article/details/gtmpsrubm.sHtML

[F08] 遍历目录
来源：http://www.m.share.bbcook.cn/Article/details/gmbovwjkp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.yfazqb.com/Article/details/gzmpbaktf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.vehdjk.com/Article/details/gkdftotfl.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.sjlbkw.cn/Article/details/gdswgqvnl.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.tarul.cn/Article/details/gascxzxgi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.bbcook.cn/Article/details/gqmzrwuvk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gcrfogzif.sHtML

Ruby: Dir.children("dir")
来源：http://baike.sjlbkw.cn/Article/details/gqfshgspc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.bbcook.cn/Article/details/glxqdshcc.sHtML

[F09] 获取文件大小
来源：http://blog.yfazqb.com/Article/details/ghfeiggwm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.tarul.cn/Article/details/gcpmyypju.sHtML

PHP:  filesize("a.txt");
来源：http://wap.vehdjk.com/Article/details/gsvixceyt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.bbcook.cn/Article/details/ggbwllxtx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.bbcook.cn/Article/details/gpplvqepc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/ghdatqtmn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.epnwcf.com/Article/details/gmtyczvfz.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gqxbzgptn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.tarul.cn/Article/details/gesprewlu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.vehdjk.com/Article/details/gpkzfaopq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/goyaymzhz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.epnwcf.com/Article/details/gykztndfm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gvthtrbyx.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gpmsbjxzd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.bbcook.cn/Article/details/gierolwvq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gvezrgbyx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gpymnaqgm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gqthlabje.sHtML

[F11] 复制与移动文件
来源：http://blog.vehdjk.com/Article/details/gvwbggzvo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/gihyzsgrf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.epnwcf.com/Article/details/gyeyaqpud.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/gnvbvvxzs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.bbcook.cn/Article/details/gidhwrpdd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.tarul.cn/Article/details/gvuurzied.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.epnwcf.com/Article/details/gpdyvhtca.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/gatmvwpcz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.epnwcf.com/Article/details/gcldwejhc.sHtML

[F12] CSV 读写
来源：http://www.blog.vehdjk.com/Article/details/gpzxswkiu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.epnwcf.com/Article/details/goxopgyaq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.bbcook.cn/Article/details/gqgtarevj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.epnwcf.com/Article/details/gjuokravl.sHtML

TS:   // 同上
来源：http://blog.yfazqb.com/Article/details/gwyjbeqdi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.bbcook.cn/Article/details/gqannnkkm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.vehdjk.com/Article/details/ghkamnzdn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.tarul.cn/Article/details/gtuqkvavo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.vehdjk.com/Article/details/gfclxmfoa.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gtwozfava.sHtML

G. 面向对象
来源：http://baike.yfazqb.com/Article/details/gcaihskrw.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gsmshmxtf.sHtML

[G01] 定义类
来源：http://blog.tarul.cn/Article/details/gzbfxrbqg.sHtML

Py:   class User: pass
来源：http://wap.epnwcf.com/Article/details/geiuzoxph.sHtML

PHP:  class User {}
来源：http://3g.yfazqb.com/Article/details/gwatwjpqf.sHtML

JS:   class User {}
来源：http://mobile.tarul.cn/Article/details/gcnflcxbn.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.vehdjk.com/Article/details/gggnzerbk.sHtML

Java: class User {}
来源：http://baike.bbcook.cn/Article/details/gxunbxfct.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fktsv.cn/Article/details/gahltceey.sHtML

Ruby: class User; end
来源：http://baike.sjlbkw.cn/Article/details/gvnmssvbm.sHtML

C#:   class User {}
来源：http://3g.sjlbkw.cn/Article/details/gppfbjhwa.sHtML

[G02] 构造函数
来源：http://baike.tarul.cn/Article/details/gtwhcylbp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.vehdjk.com/Article/details/gavksjgro.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.sjlbkw.cn/Article/details/gdrdrtoab.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.epnwcf.com/Article/details/gkoddphoz.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fktsv.cn/Article/details/gsmrtjorz.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.sjlbkw.cn/Article/details/goidfcuua.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.tarul.cn/Article/details/gbnlohvrx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.bbcook.cn/Article/details/ggfdxibih.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.tarul.cn/Article/details/gfxhzdamr.sHtML

[G03] 实例属性
来源：http://baike.sjlbkw.cn/Article/details/giparfnom.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fktsv.cn/Article/details/gufcpwmjq.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.tarul.cn/Article/details/gbubhxenv.sHtML

JS:   this.name = "x";
来源：http://m.share.vehdjk.com/Article/details/ggdneyhim.sHtML

TS:   name: string = "x";
来源：http://mobile.vehdjk.com/Article/details/gjfbwvdpi.sHtML

Java: private String name;
来源：http://wap.epnwcf.com/Article/details/gxzwqgxqq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.vehdjk.com/Article/details/gjkkhqtzk.sHtML

Ruby: @name = "x"
来源：http://www.m.share.sjlbkw.cn/Article/details/gntsolcdb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fktsv.cn/Article/details/gepfsahde.sHtML

[G04] 定义方法
来源：http://read.share.vehdjk.com/Article/details/gnxwusmks.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fktsv.cn/Article/details/gxlmjywcr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/gbhdngkrl.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/gsudjwdck.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.yfazqb.com/Article/details/gtrkjvyig.sHtML

Java: String greet() { return name; }
来源：http://3g.tarul.cn/Article/details/ghhiofang.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/ghqkopnkf.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fktsv.cn/Article/details/gkiztuigr.sHtML

C#:   public string Greet() => Name;
来源：http://3g.bbcook.cn/Article/details/gtfzonfvj.sHtML

[G05] 继承
来源：http://mobile.bbcook.cn/Article/details/gtsuwdnwy.sHtML

Py:   class Admin(User): pass
来源：http://wap.yfazqb.com/Article/details/goryjggln.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.sjlbkw.cn/Article/details/gkrskfbvp.sHtML

JS:   class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/gqlosxakw.sHtML

TS:   class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/gnbphnsho.sHtML

Java: class Admin extends User {}
来源：http://read.share.fktsv.cn/Article/details/guwwyezrm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fktsv.cn/Article/details/gghvpwyau.sHtML

Ruby: class Admin < User; end
来源：http://www.share.epnwcf.com/Article/details/gbwomadov.sHtML

C#:   class Admin : User {}
来源：http://read.share.vehdjk.com/Article/details/gxgjaggda.sHtML

[G06] 重写方法
来源：http://mobile.vehdjk.com/Article/details/gewkamght.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.yfazqb.com/Article/details/guvvtxncj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/gagbklwgn.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gqauoxaof.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.epnwcf.com/Article/details/gscmjiuoe.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/gejeguicq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.vehdjk.com/Article/details/gnzmyitnj.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.sjlbkw.cn/Article/details/gdfpcefom.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.bbcook.cn/Article/details/ggbodbcyo.sHtML

[G07] 调用父类方法
来源：http://read.share.fktsv.cn/Article/details/grkxdkvvz.sHtML

Py:   super().greet()
来源：http://mobile.epnwcf.com/Article/details/gbkpzqcju.sHtML

PHP:  parent::greet();
来源：http://wap.vehdjk.com/Article/details/gepvqlrqx.sHtML

JS:   super.greet();
来源：http://3g.tarul.cn/Article/details/gmmjgqavw.sHtML

TS:   super.greet();
来源：http://mobile.tarul.cn/Article/details/gsykmnvaw.sHtML

Java: super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gtnrfwzie.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fktsv.cn/Article/details/gzmncjijn.sHtML

Ruby: super
来源：http://www.blog.sjlbkw.cn/Article/details/ggxwoybmq.sHtML

C#:   base.Greet();
来源：http://www.m.share.epnwcf.com/Article/details/gogpeyyro.sHtML

[G08] 静态方法与属性
来源：http://3g.fktsv.cn/Article/details/gmqmwzaau.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.tarul.cn/Article/details/gmzcsisqu.sHtML

PHP:  public static function f() {}
来源：http://3g.sjlbkw.cn/Article/details/ggtzvazjs.sHtML

JS:   static f() {}
来源：http://mobile.sjlbkw.cn/Article/details/gmrmjbyly.sHtML

TS:   static f(): void {}
来源：http://www.share.yfazqb.com/Article/details/gqkmgyvuo.sHtML

Java: static void f() {}
来源：http://3g.bbcook.cn/Article/details/gudxcnkxc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.yfazqb.com/Article/details/ggmkbhmcq.sHtML

Ruby: def self.f; end
来源：http://www.blog.bbcook.cn/Article/details/gwictobws.sHtML

C#:   public static void F() {}
来源：http://m.share.bbcook.cn/Article/details/gntmotsiz.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.tarul.cn/Article/details/gznndvlsr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.vehdjk.com/Article/details/gxkycvppa.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.vehdjk.com/Article/details/gmdohhscb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fktsv.cn/Article/details/ggwcuklyz.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.epnwcf.com/Article/details/grstbxaqg.sHtML

Java: interface Shape { double area(); }
来源：http://wap.sjlbkw.cn/Article/details/gphgswnzf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.bbcook.cn/Article/details/gxrimvtpt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.sjlbkw.cn/Article/details/gaugiumqt.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.bbcook.cn/Article/details/gftqblisg.sHtML

[G10] 访问控制
来源：http://www.m.share.yfazqb.com/Article/details/gtjnjvrlu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.yfazqb.com/Article/details/gbmbaydbi.sHtML

PHP:  public / protected / private
来源：http://3g.bbcook.cn/Article/details/gqvwozmga.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.epnwcf.com/Article/details/geokbfovf.sHtML

TS:   public / protected / private
来源：http://baike.fktsv.cn/Article/details/gykkeongv.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.sjlbkw.cn/Article/details/gtvyufcdu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.epnwcf.com/Article/details/gwwazmpwg.sHtML

Ruby: public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/gqzvwftnk.sHtML

C#:   public / protected / private / internal
来源：http://mobile.sjlbkw.cn/Article/details/gkkfcmrjq.sHtML

[G11] getter / setter
来源：http://www.m.share.epnwcf.com/Article/details/gtnuybrzl.sHtML

Py:   @property 与 @x.setter
来源：http://baike.epnwcf.com/Article/details/gubfepwvu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.sjlbkw.cn/Article/details/gyipsnnvl.sHtML

JS:   get name() { return this._name; }
来源：http://wap.sjlbkw.cn/Article/details/gsfttppvr.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.tarul.cn/Article/details/gtbytiaip.sHtML

Java: public String getName() { return name; }
来源：http://blog.yfazqb.com/Article/details/gkdzirwxb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.bbcook.cn/Article/details/gwjvrmvpb.sHtML

Ruby: attr_accessor :name
来源：http://mobile.tarul.cn/Article/details/gtsycvrle.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fktsv.cn/Article/details/gofmerpet.sHtML

[G12] 对象转字符串
来源：http://baike.fktsv.cn/Article/details/gmzbkcjfd.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.epnwcf.com/Article/details/gazhmuvvv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.sjlbkw.cn/Article/details/gglynwpis.sHtML

JS:   toString() { return this.name; }
来源：http://3g.tarul.cn/Article/details/gyizrszpm.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.bbcook.cn/Article/details/gqvhzmiag.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gkhneewjj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.vehdjk.com/Article/details/gpunxxxgt.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.sjlbkw.cn/Article/details/giufxafid.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.bbcook.cn/Article/details/gqouozifn.sHtML

[G13] 判断对象类型
来源：http://wap.vehdjk.com/Article/details/ggyyzhwsq.sHtML

Py:   isinstance(u, User)
来源：http://read.share.yfazqb.com/Article/details/gjloyeicv.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/ghjhrjqgr.sHtML

JS:   u instanceof User
来源：http://3g.yfazqb.com/Article/details/gzakusrnq.sHtML

TS:   u instanceof User
来源：http://blog.tarul.cn/Article/details/ggwcsxwvb.sHtML

Java: u instanceof User
来源：http://www.share.tarul.cn/Article/details/gddlqusxv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.yfazqb.com/Article/details/gznrbhmns.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.yfazqb.com/Article/details/garqxzvip.sHtML

C#:   u is User
来源：http://www.share.tarul.cn/Article/details/gwapmghrj.sHtML

[G14] 数据类 / record
来源：http://www.blog.fktsv.cn/Article/details/ggeyxesmw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fktsv.cn/Article/details/gdgzgurqa.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fktsv.cn/Article/details/gomlqjhgl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.tarul.cn/Article/details/gumynndal.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.vehdjk.com/Article/details/gixwdohht.sHtML

Java: record User(String name, int age) {}
来源：http://3g.epnwcf.com/Article/details/gyoityurg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.yfazqb.com/Article/details/gumxrslbh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.yfazqb.com/Article/details/gzobtboox.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.tarul.cn/Article/details/geicesnrm.sHtML

[G15] 枚举
来源：http://baike.tarul.cn/Article/details/gyxilvrps.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.tarul.cn/Article/details/gnpvljsgh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.tarul.cn/Article/details/gvczajauy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.epnwcf.com/Article/details/gxjrdnrgs.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gpxcencbh.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.bbcook.cn/Article/details/gflyipgij.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.bbcook.cn/Article/details/gursydeix.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.epnwcf.com/Article/details/gqmvtizfm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fktsv.cn/Article/details/gekschxjo.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.sjlbkw.cn/Article/details/gycaaqaej.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.sjlbkw.cn/Article/details/glbkculuq.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.yfazqb.com/Article/details/gywphlmtd.sHtML

JS:   Object.entries(obj)
来源：http://3g.yfazqb.com/Article/details/ghwcrqmow.sHtML

TS:   Object.entries(obj)
来源：http://baike.vehdjk.com/Article/details/gvwkntxsv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.bbcook.cn/Article/details/gqlfcevjb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.sjlbkw.cn/Article/details/gipfvzswt.sHtML

Ruby: obj.instance_variables
来源：http://baike.tarul.cn/Article/details/gwppjyrhc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.vehdjk.com/Article/details/gbdjucajz.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gqsuhsonq.sHtML

H. 异常与错误处理
来源：http://read.share.sjlbkw.cn/Article/details/gbqbtsqui.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/goyazcxno.sHtML

[H01] try / catch 基础
来源：http://www.m.share.bbcook.cn/Article/details/gxptvrfeb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.sjlbkw.cn/Article/details/gohydwazv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.epnwcf.com/Article/details/gqimmaznq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.bbcook.cn/Article/details/gtrqgpmcr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.epnwcf.com/Article/details/gmvxnxuhz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.epnwcf.com/Article/details/grbwedljz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.epnwcf.com/Article/details/gclftlgje.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.sjlbkw.cn/Article/details/gxhfkcvst.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.yfazqb.com/Article/details/gyrfilfrh.sHtML

[H02] finally / ensure 收尾
来源：http://wap.epnwcf.com/Article/details/gqyiofhkz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.tarul.cn/Article/details/gemjgrjin.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gycsfsrjc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/geuvapqri.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gjpuchmxg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gkiqucvpx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.vehdjk.com/Article/details/gcaqwiomh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.vehdjk.com/Article/details/giuljbbiz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.tarul.cn/Article/details/gsobgywca.sHtML

[H03] 主动抛出异常
来源：http://baike.fktsv.cn/Article/details/gmombcqqx.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnazcsumx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gxbkhqsmr.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/gyfxtgzip.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/grlkmkdkj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gwtoyoczn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.yfazqb.com/Article/details/gnlrksvuy.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.epnwcf.com/Article/details/gjlahhpxh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.epnwcf.com/Article/details/gaojvnuto.sHtML

[H04] 自定义异常类型
来源：http://read.share.epnwcf.com/Article/details/gksklxxqu.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.epnwcf.com/Article/details/gobvxfmyb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.bbcook.cn/Article/details/gdoqvohcm.sHtML

JS:   class MyError extends Error {}
来源：http://baike.vehdjk.com/Article/details/gsbswwftu.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.bbcook.cn/Article/details/gpetpwnjy.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.sjlbkw.cn/Article/details/ghclmzmgu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.yfazqb.com/Article/details/gkvxxcugv.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.bbcook.cn/Article/details/gxygrycxc.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.sjlbkw.cn/Article/details/gvjmcswbd.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.epnwcf.com/Article/details/gzebfiyfv.sHtML

Py:   except ValueError as e:
来源：http://wap.fktsv.cn/Article/details/gjtnrskyj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fktsv.cn/Article/details/gcyxazwuj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.sjlbkw.cn/Article/details/godwlvsdy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fktsv.cn/Article/details/gddncyruk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.tarul.cn/Article/details/gopiquyrc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fktsv.cn/Article/details/gqrjjvefo.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.yfazqb.com/Article/details/guokjrwmh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fktsv.cn/Article/details/gctcwfpaj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.epnwcf.com/Article/details/gvspylozi.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.vehdjk.com/Article/details/gamfzfepu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.epnwcf.com/Article/details/gdxkyohyu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.bbcook.cn/Article/details/geeifmate.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.yfazqb.com/Article/details/gkkriyuxx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fktsv.cn/Article/details/gjnhzsjku.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.sjlbkw.cn/Article/details/gvocxcguu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.yfazqb.com/Article/details/ghycxpacg.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.epnwcf.com/Article/details/ghvuyvucq.sHtML

[H07] 断言
来源：http://mobile.sjlbkw.cn/Article/details/gjnpwtfls.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fktsv.cn/Article/details/gqnbuwbsq.sHtML

PHP:  assert($x > 0);
来源：http://read.share.vehdjk.com/Article/details/gkacftrfm.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.bbcook.cn/Article/details/ggihxpliz.sHtML

TS:   console.assert(x > 0);
来源：http://blog.vehdjk.com/Article/details/gvllwiopx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.epnwcf.com/Article/details/gnpynaahl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.yfazqb.com/Article/details/gbodexsnz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.tarul.cn/Article/details/gkrjgscuw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.sjlbkw.cn/Article/details/grtxlosse.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.bbcook.cn/Article/details/goooxqljp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.bbcook.cn/Article/details/giizltgkc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.yfazqb.com/Article/details/glanbadvx.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.tarul.cn/Article/details/gjkcwedey.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.bbcook.cn/Article/details/gffrzbjat.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.bbcook.cn/Article/details/geljxjdzb.sHtML

Go:   err.Error()
来源：http://www.blog.vehdjk.com/Article/details/gzutslcix.sHtML


<!-- 参考信息 -->