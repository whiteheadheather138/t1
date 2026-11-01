代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fktsv.cn/Article/details/gculouwpy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.sjlbkw.cn/Article/details/goghpkpfn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.epnwcf.com/Article/details/gpawrchaw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.sjlbkw.cn/Article/details/guzakjchy.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.sjlbkw.cn/Article/details/gwzpbscgo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fktsv.cn/Article/details/gcklmfvqg.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gzhgeutly.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/guewmighr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/gvcjvialh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/gfnvrpzoe.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.sjlbkw.cn/Article/details/gjltozovu.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gezialnps.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gduapamdm.sHtML

[F06] 删除文件
来源：http://www.share.fktsv.cn/Article/details/gzjhopzfr.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gehxjizzu.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.vehdjk.com/Article/details/ggainsvma.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gchmquhdv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.yfazqb.com/Article/details/gqswncpid.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/gldyydjet.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gutjrajur.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.tarul.cn/Article/details/gcikhlxvj.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.bbcook.cn/Article/details/gtpifjhrk.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.bbcook.cn/Article/details/grbnhssit.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.tarul.cn/Article/details/goxpmqjxs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.epnwcf.com/Article/details/gmeakniiw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.epnwcf.com/Article/details/gylartqug.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fktsv.cn/Article/details/gnybwysvm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.sjlbkw.cn/Article/details/ggovvjgsb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.vehdjk.com/Article/details/gpfgtdfyr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.tarul.cn/Article/details/gixxaudtc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.yfazqb.com/Article/details/gilsxbqeu.sHtML

[F08] 遍历目录
来源：http://baike.vehdjk.com/Article/details/gdbftxcjq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.epnwcf.com/Article/details/gfhesfzbt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.epnwcf.com/Article/details/ggmtespah.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.tarul.cn/Article/details/gbojgurht.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.bbcook.cn/Article/details/gvqhklzzj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.bbcook.cn/Article/details/gbfbgkfgj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.bbcook.cn/Article/details/guqzhcsme.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.yfazqb.com/Article/details/gxvcwbkqw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.tarul.cn/Article/details/glvjjsztw.sHtML

[F09] 获取文件大小
来源：http://wap.fktsv.cn/Article/details/geemqbnbh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.yfazqb.com/Article/details/gpitbslkh.sHtML

PHP:  filesize("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gzfyzkesa.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.yfazqb.com/Article/details/gxrkyzrkr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.yfazqb.com/Article/details/gdrydtvzl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/gepahsrbf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.sjlbkw.cn/Article/details/gkocsvxgp.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gcqszomhj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.epnwcf.com/Article/details/gckfmwnuw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.tarul.cn/Article/details/gmmscastu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/ggexmgylr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.yfazqb.com/Article/details/ghtlabhtq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gwutzrnfm.sHtML

TS:   path.extname("a.txt")
来源：http://baike.epnwcf.com/Article/details/glcvhinbf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fktsv.cn/Article/details/gamkwnvac.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gwyaexeuv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gdujpmopl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/glxujfnsz.sHtML

[F11] 复制与移动文件
来源：http://blog.tarul.cn/Article/details/gxnsawhok.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gqelcsiwd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.bbcook.cn/Article/details/gvwflvthn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/gromchoem.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/ggsakrgvh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.vehdjk.com/Article/details/gawhdahkj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.epnwcf.com/Article/details/gklvtyepx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/gbvwtvedm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fktsv.cn/Article/details/ggdvayfkz.sHtML

[F12] CSV 读写
来源：http://blog.vehdjk.com/Article/details/gofptsfwg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.epnwcf.com/Article/details/guwnexgta.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fktsv.cn/Article/details/guvqjzgkn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.epnwcf.com/Article/details/gjpsfbvyc.sHtML

TS:   // 同上
来源：http://m.share.epnwcf.com/Article/details/ghwmvkfzr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fktsv.cn/Article/details/ggjmjypvj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.epnwcf.com/Article/details/gwgllzzlp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.tarul.cn/Article/details/gubjxerud.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.epnwcf.com/Article/details/gesoqspzc.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gufgwcofq.sHtML

G. 面向对象
来源：http://www.share.fktsv.cn/Article/details/gbvoaqifa.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/grtzapczz.sHtML

[G01] 定义类
来源：http://www.share.bbcook.cn/Article/details/gwmklfdlu.sHtML

Py:   class User: pass
来源：http://blog.vehdjk.com/Article/details/gvmfdhtir.sHtML

PHP:  class User {}
来源：http://baike.bbcook.cn/Article/details/gfgdohdrz.sHtML

JS:   class User {}
来源：http://baike.vehdjk.com/Article/details/gjwgqwmem.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fktsv.cn/Article/details/guwjhspve.sHtML

Java: class User {}
来源：http://read.share.epnwcf.com/Article/details/gjtyuclmj.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.yfazqb.com/Article/details/guwruvfro.sHtML

Ruby: class User; end
来源：http://blog.vehdjk.com/Article/details/geyngvdyj.sHtML

C#:   class User {}
来源：http://www.blog.bbcook.cn/Article/details/gugtkyxaz.sHtML

[G02] 构造函数
来源：http://3g.epnwcf.com/Article/details/gvvsmidhd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.yfazqb.com/Article/details/gzwhllalb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.bbcook.cn/Article/details/gyajljdfp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fktsv.cn/Article/details/gzggiovds.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/getkbdwsg.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fktsv.cn/Article/details/gjehvyqop.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.sjlbkw.cn/Article/details/gopuuutxk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.yfazqb.com/Article/details/gcvipdxdx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.vehdjk.com/Article/details/gnxumjgbr.sHtML

[G03] 实例属性
来源：http://baike.yfazqb.com/Article/details/gkaspxgul.sHtML

Py:   self.name = "x"
来源：http://www.m.share.tarul.cn/Article/details/gjseziizy.sHtML

PHP:  public string $name = "x";
来源：http://m.share.epnwcf.com/Article/details/gffkzqipq.sHtML

JS:   this.name = "x";
来源：http://www.blog.fktsv.cn/Article/details/girhxptsz.sHtML

TS:   name: string = "x";
来源：http://read.share.fktsv.cn/Article/details/gbdbawfhk.sHtML

Java: private String name;
来源：http://baike.fktsv.cn/Article/details/gzedbseny.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.sjlbkw.cn/Article/details/gyxlyrxyw.sHtML

Ruby: @name = "x"
来源：http://m.share.sjlbkw.cn/Article/details/grjmrepvu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.yfazqb.com/Article/details/gkakkahmi.sHtML

[G04] 定义方法
来源：http://read.share.yfazqb.com/Article/details/gqcjfrsnc.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.bbcook.cn/Article/details/gydggrkbh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/gwttxbkjp.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/gmsnnpxmj.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gejjeobht.sHtML

Java: String greet() { return name; }
来源：http://baike.fktsv.cn/Article/details/gqviwzidv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.vehdjk.com/Article/details/gkvrghhgj.sHtML

Ruby: def greet; @name; end
来源：http://www.share.yfazqb.com/Article/details/gnbuwbhpd.sHtML

C#:   public string Greet() => Name;
来源：http://baike.vehdjk.com/Article/details/gsdugycez.sHtML

[G05] 继承
来源：http://read.share.bbcook.cn/Article/details/gjentyypo.sHtML

Py:   class Admin(User): pass
来源：http://read.share.epnwcf.com/Article/details/gpjtjydqv.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gpptjblmb.sHtML

JS:   class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gxleoafch.sHtML

TS:   class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gqsbkjxbb.sHtML

Java: class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gcffadrli.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fktsv.cn/Article/details/gnrnxwpgb.sHtML

Ruby: class Admin < User; end
来源：http://m.share.sjlbkw.cn/Article/details/gndzbejem.sHtML

C#:   class Admin : User {}
来源：http://www.blog.vehdjk.com/Article/details/gqsbcqvyi.sHtML

[G06] 重写方法
来源：http://m.share.fktsv.cn/Article/details/gmypniqsm.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.epnwcf.com/Article/details/gvwjesoki.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gsmqaepbi.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/galdhlxoc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/gwkiiowdb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/gepsemrbz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.epnwcf.com/Article/details/ghdncloqy.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.epnwcf.com/Article/details/giptyfggy.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.sjlbkw.cn/Article/details/gakyjxetx.sHtML

[G07] 调用父类方法
来源：http://www.blog.tarul.cn/Article/details/gdgtycctg.sHtML

Py:   super().greet()
来源：http://m.share.sjlbkw.cn/Article/details/gxjzzdbko.sHtML

PHP:  parent::greet();
来源：http://blog.epnwcf.com/Article/details/gcvoraiqu.sHtML

JS:   super.greet();
来源：http://3g.yfazqb.com/Article/details/gvrxwcfxt.sHtML

TS:   super.greet();
来源：http://www.blog.epnwcf.com/Article/details/gyqyromne.sHtML

Java: super.greet();
来源：http://read.share.tarul.cn/Article/details/gbellfora.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fktsv.cn/Article/details/guhislrxq.sHtML

Ruby: super
来源：http://read.share.fktsv.cn/Article/details/gxuvdntjo.sHtML

C#:   base.Greet();
来源：http://m.share.bbcook.cn/Article/details/gcdsdwxwr.sHtML

[G08] 静态方法与属性
来源：http://m.share.vehdjk.com/Article/details/gilurbmzs.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.epnwcf.com/Article/details/gujjoilqb.sHtML

PHP:  public static function f() {}
来源：http://baike.yfazqb.com/Article/details/gpclsnncw.sHtML

JS:   static f() {}
来源：http://www.share.vehdjk.com/Article/details/gpmtegtpm.sHtML

TS:   static f(): void {}
来源：http://www.share.yfazqb.com/Article/details/gqtpupzex.sHtML

Java: static void f() {}
来源：http://baike.epnwcf.com/Article/details/gzdborusn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.yfazqb.com/Article/details/gnkgdzrvl.sHtML

Ruby: def self.f; end
来源：http://www.share.sjlbkw.cn/Article/details/gwpwjshpr.sHtML

C#:   public static void F() {}
来源：http://www.share.vehdjk.com/Article/details/grwxhdwak.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.vehdjk.com/Article/details/gymeicyvm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.epnwcf.com/Article/details/gttybadzf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.yfazqb.com/Article/details/gyrdzgjuf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.vehdjk.com/Article/details/gtozjlfaq.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.vehdjk.com/Article/details/glsceqlao.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.epnwcf.com/Article/details/ggfopoiju.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.epnwcf.com/Article/details/gsklbdlbq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.vehdjk.com/Article/details/gvrikvisy.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.tarul.cn/Article/details/gppnnxayp.sHtML

[G10] 访问控制
来源：http://m.share.vehdjk.com/Article/details/gibofplhv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fktsv.cn/Article/details/gejzoahch.sHtML

PHP:  public / protected / private
来源：http://m.share.vehdjk.com/Article/details/gjfogcoef.sHtML

JS:   #private 字段；其余公开
来源：http://baike.tarul.cn/Article/details/gomwxrrgl.sHtML

TS:   public / protected / private
来源：http://read.share.yfazqb.com/Article/details/gngrwkpqf.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fktsv.cn/Article/details/ggkhbauyb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.bbcook.cn/Article/details/ggwgnjvto.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fktsv.cn/Article/details/gaybmuxtm.sHtML

C#:   public / protected / private / internal
来源：http://3g.tarul.cn/Article/details/geotkubha.sHtML

[G11] getter / setter
来源：http://wap.yfazqb.com/Article/details/gqwclcpzp.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.vehdjk.com/Article/details/gjpxfzzeh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.yfazqb.com/Article/details/gxjepwstd.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fktsv.cn/Article/details/gsisudnzg.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.vehdjk.com/Article/details/gbriblsbk.sHtML

Java: public String getName() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gmtzastrq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.sjlbkw.cn/Article/details/ggthppoqe.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.epnwcf.com/Article/details/gmxttohsw.sHtML

C#:   public string Name { get; set; }
来源：http://baike.bbcook.cn/Article/details/gjjgykffp.sHtML

[G12] 对象转字符串
来源：http://3g.tarul.cn/Article/details/goprslqaz.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.tarul.cn/Article/details/gfylebuaw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fktsv.cn/Article/details/gthujbqkl.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.sjlbkw.cn/Article/details/gwhdljrre.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/guophohnm.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fktsv.cn/Article/details/gghmdmcrm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.vehdjk.com/Article/details/gyaudeyqt.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fktsv.cn/Article/details/gkqvupbyr.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.epnwcf.com/Article/details/galhdeydh.sHtML

[G13] 判断对象类型
来源：http://read.share.tarul.cn/Article/details/gzbjlwoek.sHtML

Py:   isinstance(u, User)
来源：http://wap.epnwcf.com/Article/details/gubhgwpma.sHtML

PHP:  $u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gdckmzeqg.sHtML

JS:   u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/ggtusogwp.sHtML

TS:   u instanceof User
来源：http://blog.tarul.cn/Article/details/gofpluczw.sHtML

Java: u instanceof User
来源：http://m.share.epnwcf.com/Article/details/guohjjcsh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fktsv.cn/Article/details/gahqteoxy.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.epnwcf.com/Article/details/glxsmlara.sHtML

C#:   u is User
来源：http://read.share.yfazqb.com/Article/details/gbngecraf.sHtML

[G14] 数据类 / record
来源：http://www.share.vehdjk.com/Article/details/gjtkgbkwu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.yfazqb.com/Article/details/ghenurjuz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fktsv.cn/Article/details/gnasznhru.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.yfazqb.com/Article/details/gsukmwjwh.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.yfazqb.com/Article/details/gsobxhyrf.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.tarul.cn/Article/details/gnarhtipx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.tarul.cn/Article/details/gfteofjlx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.vehdjk.com/Article/details/gkcxxyiqf.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.tarul.cn/Article/details/gbskccoyp.sHtML

[G15] 枚举
来源：http://www.share.vehdjk.com/Article/details/gtjxchsok.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.tarul.cn/Article/details/glcenlhca.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.bbcook.cn/Article/details/gjrfmcvjl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.bbcook.cn/Article/details/gxfdcexyq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.yfazqb.com/Article/details/gbxdsqbbm.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.tarul.cn/Article/details/gjhhpoxnp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.epnwcf.com/Article/details/gjhtpydfx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fktsv.cn/Article/details/gsropazwr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.vehdjk.com/Article/details/gucmlgaip.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.sjlbkw.cn/Article/details/gwfcbkqzd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fktsv.cn/Article/details/gzoistagj.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.bbcook.cn/Article/details/gxlmcfvuq.sHtML

JS:   Object.entries(obj)
来源：http://3g.sjlbkw.cn/Article/details/gbhymcdan.sHtML

TS:   Object.entries(obj)
来源：http://wap.yfazqb.com/Article/details/glrofoiac.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.sjlbkw.cn/Article/details/gcdtndtnb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.yfazqb.com/Article/details/gkeatemzn.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.yfazqb.com/Article/details/gqjzruppj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fktsv.cn/Article/details/glcieklvm.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gkypiocre.sHtML

H. 异常与错误处理
来源：http://www.blog.yfazqb.com/Article/details/gxxqvpeus.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gmzafxpwn.sHtML

[H01] try / catch 基础
来源：http://read.share.tarul.cn/Article/details/gokffljel.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.yfazqb.com/Article/details/gmmcksrhi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fktsv.cn/Article/details/guqxcxpbd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.yfazqb.com/Article/details/gqtvfbnyc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.sjlbkw.cn/Article/details/gwfyngdyx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fktsv.cn/Article/details/gcpaibysb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.vehdjk.com/Article/details/goyygvxuv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gqrlycpnq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.sjlbkw.cn/Article/details/gprdgaidn.sHtML

[H02] finally / ensure 收尾
来源：http://baike.sjlbkw.cn/Article/details/gbflccmos.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.epnwcf.com/Article/details/gvtuszdew.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gnsixteku.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gqwehipfy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gkvvachho.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gfchomhsn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fktsv.cn/Article/details/gwhebcoct.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.vehdjk.com/Article/details/grhhvyije.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gmdcqncor.sHtML

[H03] 主动抛出异常
来源：http://m.share.tarul.cn/Article/details/ggksexmdf.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.yfazqb.com/Article/details/gmzttxciv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.epnwcf.com/Article/details/gwxanyllq.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.tarul.cn/Article/details/gbhecngbl.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.tarul.cn/Article/details/gckgvqaju.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.tarul.cn/Article/details/gqxkoetsh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.yfazqb.com/Article/details/gdmrtxhwz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.epnwcf.com/Article/details/giprxxwqt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/gaozlrgib.sHtML

[H04] 自定义异常类型
来源：http://m.share.fktsv.cn/Article/details/gwznfwnjh.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.sjlbkw.cn/Article/details/ghljfkvkx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.yfazqb.com/Article/details/goxsotgqr.sHtML

JS:   class MyError extends Error {}
来源：http://blog.sjlbkw.cn/Article/details/gnilgrwlm.sHtML

TS:   class MyError extends Error {}
来源：http://blog.sjlbkw.cn/Article/details/girrjrjvk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.bbcook.cn/Article/details/gbbetunww.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtygxeqdy.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.vehdjk.com/Article/details/guolulrpf.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.sjlbkw.cn/Article/details/gtnmuinbk.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fktsv.cn/Article/details/gcmcovtmn.sHtML

Py:   except ValueError as e:
来源：http://www.blog.sjlbkw.cn/Article/details/gtzniapss.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.epnwcf.com/Article/details/gyvkcrggp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fktsv.cn/Article/details/gdbejouji.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.tarul.cn/Article/details/gugzylokm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.vehdjk.com/Article/details/gdgzaumuy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.sjlbkw.cn/Article/details/gfdphjtcx.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.vehdjk.com/Article/details/gngaogdcx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.yfazqb.com/Article/details/gvihcxhgd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.vehdjk.com/Article/details/gnigxraio.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fktsv.cn/Article/details/gzfjzcmaw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fktsv.cn/Article/details/googxiimo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.tarul.cn/Article/details/gcbqpwplv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.bbcook.cn/Article/details/gccenasmj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.yfazqb.com/Article/details/gibughzbv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.vehdjk.com/Article/details/goejyazvv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.vehdjk.com/Article/details/gibpokurh.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.epnwcf.com/Article/details/gdtnsfoty.sHtML

[H07] 断言
来源：http://wap.vehdjk.com/Article/details/gjrpuames.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.bbcook.cn/Article/details/gahqeieoo.sHtML

PHP:  assert($x > 0);
来源：http://read.share.epnwcf.com/Article/details/gofgklfoy.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.yfazqb.com/Article/details/gszbuwknp.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.yfazqb.com/Article/details/gbcxvxhaz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.yfazqb.com/Article/details/gkdgaffsz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.vehdjk.com/Article/details/gkbipflhs.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.yfazqb.com/Article/details/gpsdhobia.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gvorzogbs.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.bbcook.cn/Article/details/goeorgfyl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fktsv.cn/Article/details/gqlbhxilf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.vehdjk.com/Article/details/gmlolziey.sHtML

JS:   e.message;  e.stack
来源：http://www.share.epnwcf.com/Article/details/gezhexxjl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.epnwcf.com/Article/details/gzgtkxssg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.vehdjk.com/Article/details/gdpzimxzh.sHtML

Go:   err.Error()
来源：http://3g.epnwcf.com/Article/details/gmbvkzuah.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.sjlbkw.cn/Article/details/gmsbezuiu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.yfazqb.com/Article/details/ghouxtxig.sHtML

[H09] 带错误码的异常
来源：http://3g.bbcook.cn/Article/details/gjkraobzp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.yfazqb.com/Article/details/gqbpkvfwj.sHtML


<!-- 参考信息 -->