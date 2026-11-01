代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.tarul.cn/Article/details/gyafcsvsw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.epnwcf.com/Article/details/geyewdfdo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.vehdjk.com/Article/details/gekfsgiyn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fktsv.cn/Article/details/gsipfwrgq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fktsv.cn/Article/details/ghluhsjqt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.epnwcf.com/Article/details/gybjbekno.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.vehdjk.com/Article/details/gvvvjlerd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.vehdjk.com/Article/details/gzkzqrvxq.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.sjlbkw.cn/Article/details/gceqkajja.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.bbcook.cn/Article/details/gqvnnmnos.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gbgpbxdnb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gfxqzggfm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/gvzfmofxt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fktsv.cn/Article/details/gyfyahjht.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.vehdjk.com/Article/details/gndkxnors.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gktbnwpef.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gycskakbd.sHtML

[F06] 删除文件
来源：http://blog.sjlbkw.cn/Article/details/gueugjnqj.sHtML

Py:   os.remove("a.txt")
来源：http://baike.vehdjk.com/Article/details/gfxdhhytk.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.tarul.cn/Article/details/gdzjcxpuk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.vehdjk.com/Article/details/ghewwmodd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/geprjbwah.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.tarul.cn/Article/details/gxvthbgif.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.bbcook.cn/Article/details/gxhdpekkx.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fktsv.cn/Article/details/gbspglmvq.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/goukxwmvr.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.vehdjk.com/Article/details/gkqrffgym.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.bbcook.cn/Article/details/gcjefftxb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.yfazqb.com/Article/details/gqzqzotng.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.tarul.cn/Article/details/gsagragah.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fktsv.cn/Article/details/gpkwlfytg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.epnwcf.com/Article/details/gjmqhlgmi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghgocyffe.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.sjlbkw.cn/Article/details/gzxuaqkkv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.sjlbkw.cn/Article/details/gdplkeont.sHtML

[F08] 遍历目录
来源：http://www.m.share.epnwcf.com/Article/details/gcuxlbpey.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.vehdjk.com/Article/details/gjhxtutlu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.vehdjk.com/Article/details/gidfvyher.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.yfazqb.com/Article/details/gsvocsmsl.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.yfazqb.com/Article/details/gbdssciaa.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.tarul.cn/Article/details/gakqojzqk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.vehdjk.com/Article/details/gynyhjcsk.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.tarul.cn/Article/details/gpzxzxicy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.tarul.cn/Article/details/gavqbsigg.sHtML

[F09] 获取文件大小
来源：http://3g.vehdjk.com/Article/details/gtnlbtvqo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.tarul.cn/Article/details/gpnxukfnj.sHtML

PHP:  filesize("a.txt");
来源：http://blog.vehdjk.com/Article/details/gycgwhkvs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.vehdjk.com/Article/details/glxjfeqyh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fktsv.cn/Article/details/gciuplvbb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/ghkvenikr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.yfazqb.com/Article/details/gqzqrtpde.sHtML

Ruby: File.size("a.txt")
来源：http://baike.vehdjk.com/Article/details/gqpodhvyf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.sjlbkw.cn/Article/details/gidbaavee.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.yfazqb.com/Article/details/gbqacijjk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gjssbmgzc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.yfazqb.com/Article/details/grovrycka.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/ggbudpqku.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gapfmqzcx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.yfazqb.com/Article/details/gpolzybfa.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/gkuqghaqx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gqbgjozyx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/gemeeuplh.sHtML

[F11] 复制与移动文件
来源：http://3g.sjlbkw.cn/Article/details/gritagrvf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gdqdjvxwi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.epnwcf.com/Article/details/gtzhvsseg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/gcuuvjbjh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/gmoveljfy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.vehdjk.com/Article/details/gfgechnnp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.bbcook.cn/Article/details/grznehcws.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.tarul.cn/Article/details/gwmwvegyr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.bbcook.cn/Article/details/gglizphta.sHtML

[F12] CSV 读写
来源：http://m.share.fktsv.cn/Article/details/gdlzoqzna.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.yfazqb.com/Article/details/gsaswjutx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.bbcook.cn/Article/details/ghibmpmmy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.sjlbkw.cn/Article/details/gtaacimyr.sHtML

TS:   // 同上
来源：http://www.share.yfazqb.com/Article/details/gskibrqmx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.vehdjk.com/Article/details/gwisgzstk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.epnwcf.com/Article/details/gcdgkonpq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.sjlbkw.cn/Article/details/gdbsmwagn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.vehdjk.com/Article/details/ghyghjxjh.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gyzhakbew.sHtML

G. 面向对象
来源：http://www.share.tarul.cn/Article/details/grtpapiae.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gfjawrubv.sHtML

[G01] 定义类
来源：http://www.share.vehdjk.com/Article/details/gqfqumobk.sHtML

Py:   class User: pass
来源：http://baike.bbcook.cn/Article/details/grhcufckz.sHtML

PHP:  class User {}
来源：http://m.share.tarul.cn/Article/details/gcvyasonp.sHtML

JS:   class User {}
来源：http://3g.sjlbkw.cn/Article/details/gkmpxbuek.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.vehdjk.com/Article/details/gbebrhcuc.sHtML

Java: class User {}
来源：http://blog.fktsv.cn/Article/details/gzxpsayax.sHtML

Go:   type User struct { Name string }
来源：http://3g.vehdjk.com/Article/details/gdjppcqqp.sHtML

Ruby: class User; end
来源：http://www.blog.fktsv.cn/Article/details/gwtdcghlx.sHtML

C#:   class User {}
来源：http://www.share.yfazqb.com/Article/details/gioovaacr.sHtML

[G02] 构造函数
来源：http://read.share.fktsv.cn/Article/details/gyktrsmsa.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.bbcook.cn/Article/details/gyavhphqi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.vehdjk.com/Article/details/gnpcehuch.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.vehdjk.com/Article/details/gswdslyyc.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.yfazqb.com/Article/details/ggvypxliy.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.bbcook.cn/Article/details/gewwfzwxg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fktsv.cn/Article/details/gsjtqprfp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.sjlbkw.cn/Article/details/gqcquqimx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fktsv.cn/Article/details/gadkatqvx.sHtML

[G03] 实例属性
来源：http://www.blog.fktsv.cn/Article/details/gsstvtqvi.sHtML

Py:   self.name = "x"
来源：http://read.share.yfazqb.com/Article/details/gsnxonuzy.sHtML

PHP:  public string $name = "x";
来源：http://read.share.tarul.cn/Article/details/gvnxmlwfa.sHtML

JS:   this.name = "x";
来源：http://m.share.tarul.cn/Article/details/gbkkpomop.sHtML

TS:   name: string = "x";
来源：http://www.share.epnwcf.com/Article/details/gotblwtkb.sHtML

Java: private String name;
来源：http://blog.tarul.cn/Article/details/gbdrtkuyo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fktsv.cn/Article/details/gjilpzvpa.sHtML

Ruby: @name = "x"
来源：http://www.share.yfazqb.com/Article/details/gxghmwuon.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gmnhniucm.sHtML

[G04] 定义方法
来源：http://read.share.tarul.cn/Article/details/gkrwqslid.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.tarul.cn/Article/details/gftszfsmp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.bbcook.cn/Article/details/gmxlrqofq.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/ggepzqlyu.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.bbcook.cn/Article/details/gfugkbwmz.sHtML

Java: String greet() { return name; }
来源：http://read.share.vehdjk.com/Article/details/gpnjjjbtq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fktsv.cn/Article/details/gkcosarme.sHtML

Ruby: def greet; @name; end
来源：http://read.share.tarul.cn/Article/details/gpduzuvdm.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.sjlbkw.cn/Article/details/gvlakllgb.sHtML

[G05] 继承
来源：http://mobile.bbcook.cn/Article/details/gshbfyoof.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.sjlbkw.cn/Article/details/gauodnwrn.sHtML

PHP:  class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/gvzlfuumd.sHtML

JS:   class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gnvnktlxf.sHtML

TS:   class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/gnjnqzxbw.sHtML

Java: class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/gmvcquqtl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.yfazqb.com/Article/details/gqoxferar.sHtML

Ruby: class Admin < User; end
来源：http://www.share.tarul.cn/Article/details/gouyhikmh.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fktsv.cn/Article/details/gpdchxkpt.sHtML

[G06] 重写方法
来源：http://mobile.bbcook.cn/Article/details/gejntfzrf.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.bbcook.cn/Article/details/gyxjpenig.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.tarul.cn/Article/details/grpvraqgj.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gcykvyhkk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/gqbsfvndf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/grfkrehnk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.bbcook.cn/Article/details/gyustevci.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.tarul.cn/Article/details/gieffbkqa.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.yfazqb.com/Article/details/gqzzwqewo.sHtML

[G07] 调用父类方法
来源：http://m.share.epnwcf.com/Article/details/gfssqpxsi.sHtML

Py:   super().greet()
来源：http://m.share.epnwcf.com/Article/details/guqcwwgcc.sHtML

PHP:  parent::greet();
来源：http://read.share.yfazqb.com/Article/details/gcviczeen.sHtML

JS:   super.greet();
来源：http://read.share.yfazqb.com/Article/details/goawhgwap.sHtML

TS:   super.greet();
来源：http://mobile.bbcook.cn/Article/details/gaggbdrow.sHtML

Java: super.greet();
来源：http://read.share.bbcook.cn/Article/details/gzoaqgauv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.tarul.cn/Article/details/gonhhpbiq.sHtML

Ruby: super
来源：http://www.blog.sjlbkw.cn/Article/details/gitdfybhy.sHtML

C#:   base.Greet();
来源：http://read.share.fktsv.cn/Article/details/geqoqqsnd.sHtML

[G08] 静态方法与属性
来源：http://3g.bbcook.cn/Article/details/ghrtlmlpk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fktsv.cn/Article/details/gtpttbysm.sHtML

PHP:  public static function f() {}
来源：http://blog.sjlbkw.cn/Article/details/ggyejctqn.sHtML

JS:   static f() {}
来源：http://www.blog.epnwcf.com/Article/details/gucvmekdx.sHtML

TS:   static f(): void {}
来源：http://baike.bbcook.cn/Article/details/gosdeimkt.sHtML

Java: static void f() {}
来源：http://wap.sjlbkw.cn/Article/details/gslleksnp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.tarul.cn/Article/details/gzyghfzrr.sHtML

Ruby: def self.f; end
来源：http://www.blog.sjlbkw.cn/Article/details/gtbmrkjco.sHtML

C#:   public static void F() {}
来源：http://3g.bbcook.cn/Article/details/gcctmypxd.sHtML

[G09] 接口 / 抽象类
来源：http://wap.tarul.cn/Article/details/gcdmwxxka.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.sjlbkw.cn/Article/details/gfmbjcvmr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.epnwcf.com/Article/details/gnxswcorr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.epnwcf.com/Article/details/gubpkooja.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.epnwcf.com/Article/details/ghrjwlwsd.sHtML

Java: interface Shape { double area(); }
来源：http://wap.sjlbkw.cn/Article/details/goffwajqf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.bbcook.cn/Article/details/gookiokfk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.yfazqb.com/Article/details/gjczkajbw.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.bbcook.cn/Article/details/gdvbrvcwu.sHtML

[G10] 访问控制
来源：http://m.share.vehdjk.com/Article/details/gcpnqqrlx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.yfazqb.com/Article/details/ggkkwizkl.sHtML

PHP:  public / protected / private
来源：http://3g.sjlbkw.cn/Article/details/gdrqagsbd.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fktsv.cn/Article/details/gcssbdkxn.sHtML

TS:   public / protected / private
来源：http://mobile.epnwcf.com/Article/details/gzgzvwgib.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.vehdjk.com/Article/details/gdikcofmz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.vehdjk.com/Article/details/gcwkktlqn.sHtML

Ruby: public / protected / private
来源：http://blog.vehdjk.com/Article/details/ggubncmli.sHtML

C#:   public / protected / private / internal
来源：http://www.share.epnwcf.com/Article/details/gnsilvmec.sHtML

[G11] getter / setter
来源：http://m.share.tarul.cn/Article/details/goyrdxydu.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.sjlbkw.cn/Article/details/ggjxkbrjh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.epnwcf.com/Article/details/gnizosjge.sHtML

JS:   get name() { return this._name; }
来源：http://3g.bbcook.cn/Article/details/govmkzxnq.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.vehdjk.com/Article/details/gnjunhbze.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gqezytdch.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.epnwcf.com/Article/details/gkuudevln.sHtML

Ruby: attr_accessor :name
来源：http://blog.sjlbkw.cn/Article/details/gfkqfjldq.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.yfazqb.com/Article/details/gjflmbash.sHtML

[G12] 对象转字符串
来源：http://wap.sjlbkw.cn/Article/details/ghmzkndzi.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.epnwcf.com/Article/details/gghxixfgo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.sjlbkw.cn/Article/details/gutyjxqgn.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fktsv.cn/Article/details/glzqqlfeo.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fktsv.cn/Article/details/gbcsfmyvi.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.yfazqb.com/Article/details/gachwmgcz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.tarul.cn/Article/details/gfxdaocov.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fktsv.cn/Article/details/gzmplajwr.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.vehdjk.com/Article/details/gzgwidnwz.sHtML

[G13] 判断对象类型
来源：http://www.share.tarul.cn/Article/details/ghmtwazky.sHtML

Py:   isinstance(u, User)
来源：http://wap.sjlbkw.cn/Article/details/gyciyqbox.sHtML

PHP:  $u instanceof User
来源：http://3g.yfazqb.com/Article/details/gsqwqajlk.sHtML

JS:   u instanceof User
来源：http://blog.bbcook.cn/Article/details/gfhpxqvlr.sHtML

TS:   u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/gmkfnukwk.sHtML

Java: u instanceof User
来源：http://mobile.vehdjk.com/Article/details/gpypxbfax.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fktsv.cn/Article/details/gfnbjjjxf.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.bbcook.cn/Article/details/gsyltaltv.sHtML

C#:   u is User
来源：http://mobile.yfazqb.com/Article/details/gylzrwzxp.sHtML

[G14] 数据类 / record
来源：http://baike.tarul.cn/Article/details/gotfmgrgq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.yfazqb.com/Article/details/gjlqsvmos.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.bbcook.cn/Article/details/gdjafhjkt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fktsv.cn/Article/details/gzwwxczms.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.tarul.cn/Article/details/gsquyatbv.sHtML

Java: record User(String name, int age) {}
来源：http://blog.vehdjk.com/Article/details/gebjeeczh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fktsv.cn/Article/details/gxccyvfqa.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.yfazqb.com/Article/details/gwybbtgzp.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.sjlbkw.cn/Article/details/gfrlhjqtu.sHtML

[G15] 枚举
来源：http://read.share.yfazqb.com/Article/details/goecfzlng.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.epnwcf.com/Article/details/gscomvljd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.yfazqb.com/Article/details/gpqsbgikw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fktsv.cn/Article/details/gbqocjpdh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gsqknwpiw.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.sjlbkw.cn/Article/details/grjcwxsgw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.epnwcf.com/Article/details/gaeeaicdv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.epnwcf.com/Article/details/gwmbdnljk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.vehdjk.com/Article/details/gexsdaotc.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.epnwcf.com/Article/details/gwuhnblcv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.yfazqb.com/Article/details/gdpfwrecr.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.vehdjk.com/Article/details/gqdkxegnk.sHtML

JS:   Object.entries(obj)
来源：http://blog.tarul.cn/Article/details/gpllskhxi.sHtML

TS:   Object.entries(obj)
来源：http://baike.sjlbkw.cn/Article/details/gbjcooqau.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.sjlbkw.cn/Article/details/gcqwvxiqe.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.yfazqb.com/Article/details/gxwwetzmc.sHtML

Ruby: obj.instance_variables
来源：http://www.share.yfazqb.com/Article/details/gkfuwswfw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.epnwcf.com/Article/details/gxwoffcam.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/guzbayyra.sHtML

H. 异常与错误处理
来源：http://www.blog.yfazqb.com/Article/details/gpzaredri.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/glajxfayc.sHtML

[H01] try / catch 基础
来源：http://www.m.share.tarul.cn/Article/details/gqioddwyy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fktsv.cn/Article/details/gvzxbejnf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fktsv.cn/Article/details/grpallseh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.bbcook.cn/Article/details/grajtsjht.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.vehdjk.com/Article/details/ghpsotffg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.sjlbkw.cn/Article/details/glyszaazr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.yfazqb.com/Article/details/gblbmeopv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.bbcook.cn/Article/details/gjnxxmgig.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.sjlbkw.cn/Article/details/glyfmqnqi.sHtML

[H02] finally / ensure 收尾
来源：http://3g.bbcook.cn/Article/details/gemldjpld.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fktsv.cn/Article/details/gpdaquwxn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gbfcjptcr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/guplxnixi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/ghytludqu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gtyrzdjgq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.tarul.cn/Article/details/gcvrmiuln.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.vehdjk.com/Article/details/gpksffmvv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gebuiyhow.sHtML

[H03] 主动抛出异常
来源：http://read.share.vehdjk.com/Article/details/gmdahltpg.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.epnwcf.com/Article/details/geggxjmqm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gpggbshxh.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gcqpkjzsc.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fktsv.cn/Article/details/guwgsqjnb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fktsv.cn/Article/details/gbqsotiwb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.tarul.cn/Article/details/gzlypildv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.vehdjk.com/Article/details/gwmefqebt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fktsv.cn/Article/details/gtwjueznh.sHtML

[H04] 自定义异常类型
来源：http://3g.tarul.cn/Article/details/gstxmvtsd.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.sjlbkw.cn/Article/details/gtfssygfo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.tarul.cn/Article/details/gsqbbqeep.sHtML

JS:   class MyError extends Error {}
来源：http://wap.bbcook.cn/Article/details/gtcymkkbc.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.vehdjk.com/Article/details/gewduliro.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.bbcook.cn/Article/details/gqeqwhnkd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.tarul.cn/Article/details/ggemzeagq.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.epnwcf.com/Article/details/gylcszsfc.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.vehdjk.com/Article/details/glaceenwr.sHtML

[H05] 捕获特定类型
来源：http://www.blog.yfazqb.com/Article/details/gkxmuxpny.sHtML

Py:   except ValueError as e:
来源：http://3g.vehdjk.com/Article/details/gqdqxbcoh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.bbcook.cn/Article/details/gjqhpopij.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fktsv.cn/Article/details/goedfhszk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.epnwcf.com/Article/details/gnijvjaaf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.epnwcf.com/Article/details/gxvtuqrzl.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fktsv.cn/Article/details/gzhxggkrh.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.bbcook.cn/Article/details/gkjntmywn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.tarul.cn/Article/details/gzfcnnhbv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.tarul.cn/Article/details/ghinfmdzy.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fktsv.cn/Article/details/gprjutefd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.epnwcf.com/Article/details/gssyjzfnq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fktsv.cn/Article/details/gczqdblte.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.tarul.cn/Article/details/ggcvetrsu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fktsv.cn/Article/details/gamrjlmnq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.sjlbkw.cn/Article/details/ghedddizh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.epnwcf.com/Article/details/gsiajthbb.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.vehdjk.com/Article/details/ggiavogqn.sHtML

[H07] 断言
来源：http://read.share.yfazqb.com/Article/details/gnfqiwnau.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.bbcook.cn/Article/details/gcatfqhaq.sHtML

PHP:  assert($x > 0);
来源：http://blog.fktsv.cn/Article/details/gmsxqaefh.sHtML

JS:   console.assert(x > 0);
来源：http://blog.yfazqb.com/Article/details/gwddgucfw.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.yfazqb.com/Article/details/gzkzvcllk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.tarul.cn/Article/details/gdntveasx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fktsv.cn/Article/details/gvpekppvb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.vehdjk.com/Article/details/gjzztttqh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/gvqljulfw.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.epnwcf.com/Article/details/ghkjhikbv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.bbcook.cn/Article/details/gtyaopghk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fktsv.cn/Article/details/gunnvhnnp.sHtML

JS:   e.message;  e.stack
来源：http://blog.sjlbkw.cn/Article/details/gketzchhj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.sjlbkw.cn/Article/details/gmwfzfqmi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.sjlbkw.cn/Article/details/gaxflukmv.sHtML

Go:   err.Error()
来源：http://wap.tarul.cn/Article/details/goouvshvp.sHtML


<!-- 参考信息 -->