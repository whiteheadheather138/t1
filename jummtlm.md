代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/gjwwfoygg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.tarul.cn/Article/details/glujddaeu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.tarul.cn/Article/details/gbxjypdsq.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gshfkmaor.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gdcaibksj.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gtlotoamk.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.bbcook.cn/Article/details/gjrxhrhix.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.yfazqb.com/Article/details/glzotgkoq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.epnwcf.com/Article/details/gtvpjxyia.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fktsv.cn/Article/details/gppwwqbuy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.sjlbkw.cn/Article/details/gdxycfwhj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.vehdjk.com/Article/details/gmqniwmdz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.sjlbkw.cn/Article/details/gfylzlfaf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.epnwcf.com/Article/details/gygdvjvfc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fktsv.cn/Article/details/giauuvlbs.sHtML

[F08] 遍历目录
来源：http://mobile.fktsv.cn/Article/details/gceskjwxb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.sjlbkw.cn/Article/details/gzirhrdyn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.tarul.cn/Article/details/gpxgfudqp.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.epnwcf.com/Article/details/gtdrerufd.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fktsv.cn/Article/details/gyrahdccw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.yfazqb.com/Article/details/gqmsfahbl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gcznvghcf.sHtML

Ruby: Dir.children("dir")
来源：http://wap.bbcook.cn/Article/details/gevabrmew.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.yfazqb.com/Article/details/glnpvhqtg.sHtML

[F09] 获取文件大小
来源：http://read.share.bbcook.cn/Article/details/gidxejfoe.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fktsv.cn/Article/details/geuqlehcn.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gtnretuwu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.vehdjk.com/Article/details/ganltgjrk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.yfazqb.com/Article/details/gvkhtplbw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gnfkxtsdp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.tarul.cn/Article/details/gambmsjpo.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fktsv.cn/Article/details/ggwdihkjb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.vehdjk.com/Article/details/grulbqkae.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.vehdjk.com/Article/details/gaiwmuujs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.tarul.cn/Article/details/gfdgmqrmd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gmsisnzqw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gbhhddvkd.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gmlrnhufd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.yfazqb.com/Article/details/gmfhvetqk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/gikpcofzt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/grdmxpvui.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gfgsnwsly.sHtML

[F11] 复制与移动文件
来源：http://mobile.sjlbkw.cn/Article/details/gdnyqkoys.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gpenirlpt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.epnwcf.com/Article/details/gswzcdyiy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/gyvikfvlv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/gbciyrfgp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.yfazqb.com/Article/details/gapsoevmf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.epnwcf.com/Article/details/gbahmulwp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/gdeawxccd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.vehdjk.com/Article/details/guwoldprc.sHtML

[F12] CSV 读写
来源：http://3g.bbcook.cn/Article/details/gsfwadudu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fktsv.cn/Article/details/gnpxykfpe.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.bbcook.cn/Article/details/gnwzscqeh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.yfazqb.com/Article/details/gnfxygdsp.sHtML

TS:   // 同上
来源：http://wap.epnwcf.com/Article/details/gcszckfyr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.tarul.cn/Article/details/gvlflowuk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.tarul.cn/Article/details/gucarqxjo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.yfazqb.com/Article/details/gbcyfokfa.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.tarul.cn/Article/details/gbdutebon.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gtbrcrbru.sHtML

G. 面向对象
来源：http://m.share.yfazqb.com/Article/details/gaxfziojv.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/geekmzpzx.sHtML

[G01] 定义类
来源：http://m.share.yfazqb.com/Article/details/gcfobichs.sHtML

Py:   class User: pass
来源：http://blog.yfazqb.com/Article/details/gwwhbtdms.sHtML

PHP:  class User {}
来源：http://baike.epnwcf.com/Article/details/gpnwgriwd.sHtML

JS:   class User {}
来源：http://blog.vehdjk.com/Article/details/gidresjiw.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.tarul.cn/Article/details/gmydeoksh.sHtML

Java: class User {}
来源：http://mobile.epnwcf.com/Article/details/gpxsxlhry.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fktsv.cn/Article/details/gtawdleyn.sHtML

Ruby: class User; end
来源：http://blog.sjlbkw.cn/Article/details/gxchkgdyr.sHtML

C#:   class User {}
来源：http://baike.yfazqb.com/Article/details/glwgkeeqp.sHtML

[G02] 构造函数
来源：http://3g.sjlbkw.cn/Article/details/goxijhlfp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.sjlbkw.cn/Article/details/glcpdapdr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.yfazqb.com/Article/details/gcnwxklsb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.bbcook.cn/Article/details/ggytgxjef.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.tarul.cn/Article/details/gtpqnfesh.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.tarul.cn/Article/details/gumlaclir.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.sjlbkw.cn/Article/details/gfanywwwt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.sjlbkw.cn/Article/details/glhnzwtsf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fktsv.cn/Article/details/gycupsuah.sHtML

[G03] 实例属性
来源：http://mobile.fktsv.cn/Article/details/gbfbdpixd.sHtML

Py:   self.name = "x"
来源：http://baike.epnwcf.com/Article/details/gqoggvujc.sHtML

PHP:  public string $name = "x";
来源：http://www.share.vehdjk.com/Article/details/ghpoczmke.sHtML

JS:   this.name = "x";
来源：http://3g.vehdjk.com/Article/details/gzrzbvmln.sHtML

TS:   name: string = "x";
来源：http://www.blog.epnwcf.com/Article/details/gtwybymwk.sHtML

Java: private String name;
来源：http://www.blog.vehdjk.com/Article/details/gymfdaxpx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.yfazqb.com/Article/details/gtujkwgim.sHtML

Ruby: @name = "x"
来源：http://baike.tarul.cn/Article/details/gftyaehhp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.sjlbkw.cn/Article/details/ghifezmfx.sHtML

[G04] 定义方法
来源：http://m.share.tarul.cn/Article/details/ggageiiax.sHtML

Py:   def greet(self): return self.name
来源：http://3g.vehdjk.com/Article/details/geclgnryk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gonoqscle.sHtML

JS:   greet() { return this.name; }
来源：http://wap.bbcook.cn/Article/details/gvlejwvez.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/gavrdgsmy.sHtML

Java: String greet() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gkqsgwdly.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fktsv.cn/Article/details/giwwdjpzu.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fktsv.cn/Article/details/grpswuhcd.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.tarul.cn/Article/details/gsipqdltr.sHtML

[G05] 继承
来源：http://3g.fktsv.cn/Article/details/gkdrcyukm.sHtML

Py:   class Admin(User): pass
来源：http://baike.epnwcf.com/Article/details/gtddujlmt.sHtML

PHP:  class Admin extends User {}
来源：http://baike.epnwcf.com/Article/details/gmatlhmdj.sHtML

JS:   class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gpsqmeutu.sHtML

TS:   class Admin extends User {}
来源：http://mobile.tarul.cn/Article/details/gbkflzsmn.sHtML

Java: class Admin extends User {}
来源：http://mobile.fktsv.cn/Article/details/gkvreelwg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.tarul.cn/Article/details/guqlwxnbd.sHtML

Ruby: class Admin < User; end
来源：http://3g.fktsv.cn/Article/details/gbkvmpsqc.sHtML

C#:   class Admin : User {}
来源：http://blog.yfazqb.com/Article/details/gundawrjj.sHtML

[G06] 重写方法
来源：http://3g.bbcook.cn/Article/details/glneznniw.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.epnwcf.com/Article/details/gwzmfessv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gizswwgxl.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.vehdjk.com/Article/details/gxmhhwetg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gzfeevonc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.tarul.cn/Article/details/gvwhtupxt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.vehdjk.com/Article/details/gtahnuptz.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fktsv.cn/Article/details/gaaokppgx.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.epnwcf.com/Article/details/glgvooyfr.sHtML

[G07] 调用父类方法
来源：http://3g.fktsv.cn/Article/details/gmofniqbf.sHtML

Py:   super().greet()
来源：http://www.m.share.vehdjk.com/Article/details/ghpndxnxu.sHtML

PHP:  parent::greet();
来源：http://blog.vehdjk.com/Article/details/gdfodlmyh.sHtML

JS:   super.greet();
来源：http://wap.fktsv.cn/Article/details/gzqhtnvrz.sHtML

TS:   super.greet();
来源：http://www.m.share.yfazqb.com/Article/details/gprykusxw.sHtML

Java: super.greet();
来源：http://baike.sjlbkw.cn/Article/details/gttzvjaiy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.yfazqb.com/Article/details/gdmalvdmw.sHtML

Ruby: super
来源：http://baike.yfazqb.com/Article/details/gqfdpnvxf.sHtML

C#:   base.Greet();
来源：http://m.share.yfazqb.com/Article/details/gidscmflc.sHtML

[G08] 静态方法与属性
来源：http://read.share.sjlbkw.cn/Article/details/gpluzjzoo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.yfazqb.com/Article/details/gwyloiqsk.sHtML

PHP:  public static function f() {}
来源：http://baike.tarul.cn/Article/details/ggvboettd.sHtML

JS:   static f() {}
来源：http://wap.fktsv.cn/Article/details/gehqkuhhp.sHtML

TS:   static f(): void {}
来源：http://baike.fktsv.cn/Article/details/glnxyhvhy.sHtML

Java: static void f() {}
来源：http://3g.vehdjk.com/Article/details/gblxkytge.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.bbcook.cn/Article/details/gprxxwtrp.sHtML

Ruby: def self.f; end
来源：http://m.share.fktsv.cn/Article/details/gajuieyzj.sHtML

C#:   public static void F() {}
来源：http://mobile.tarul.cn/Article/details/gfbowvjgc.sHtML

[G09] 接口 / 抽象类
来源：http://blog.bbcook.cn/Article/details/gforlrlzo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.sjlbkw.cn/Article/details/gqnzxubht.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fktsv.cn/Article/details/gupfhvtah.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.vehdjk.com/Article/details/gfebueook.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.tarul.cn/Article/details/gshpdybmf.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.yfazqb.com/Article/details/gsgkfbrbj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.sjlbkw.cn/Article/details/goropffxj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.yfazqb.com/Article/details/ghqjyqzxi.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.bbcook.cn/Article/details/ggttysyxe.sHtML

[G10] 访问控制
来源：http://mobile.sjlbkw.cn/Article/details/gxlytkwpg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.epnwcf.com/Article/details/gftvikflj.sHtML

PHP:  public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/gwzsjnkwe.sHtML

JS:   #private 字段；其余公开
来源：http://3g.epnwcf.com/Article/details/gkzdxqozf.sHtML

TS:   public / protected / private
来源：http://mobile.epnwcf.com/Article/details/gqmfywebd.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.bbcook.cn/Article/details/gwqagpblb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.tarul.cn/Article/details/ggvmuaedy.sHtML

Ruby: public / protected / private
来源：http://wap.tarul.cn/Article/details/giaiteeen.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.epnwcf.com/Article/details/gablpsyct.sHtML

[G11] getter / setter
来源：http://m.share.vehdjk.com/Article/details/gnxrtshlx.sHtML

Py:   @property 与 @x.setter
来源：http://wap.vehdjk.com/Article/details/gcgbytdwh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.tarul.cn/Article/details/guqubdckk.sHtML

JS:   get name() { return this._name; }
来源：http://wap.vehdjk.com/Article/details/gwlxdklxt.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.sjlbkw.cn/Article/details/gkuuhxmnj.sHtML

Java: public String getName() { return name; }
来源：http://wap.bbcook.cn/Article/details/gwiusfhnh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.tarul.cn/Article/details/gtvesfggi.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.tarul.cn/Article/details/ggltqtbfx.sHtML

C#:   public string Name { get; set; }
来源：http://wap.yfazqb.com/Article/details/gndqwlqex.sHtML

[G12] 对象转字符串
来源：http://www.m.share.bbcook.cn/Article/details/guenxpjfk.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.vehdjk.com/Article/details/ghmzkxens.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.epnwcf.com/Article/details/gxkylzyiq.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fktsv.cn/Article/details/gcfsmfkeb.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.tarul.cn/Article/details/gyouphnhy.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.bbcook.cn/Article/details/gbvhmfoca.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzmovwgfk.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.sjlbkw.cn/Article/details/ggcaqflxw.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.vehdjk.com/Article/details/gqaghmyrg.sHtML

[G13] 判断对象类型
来源：http://read.share.vehdjk.com/Article/details/gytshebnb.sHtML

Py:   isinstance(u, User)
来源：http://3g.yfazqb.com/Article/details/glsowreet.sHtML

PHP:  $u instanceof User
来源：http://m.share.yfazqb.com/Article/details/gqfgkfvqe.sHtML

JS:   u instanceof User
来源：http://baike.bbcook.cn/Article/details/gkfzihuur.sHtML

TS:   u instanceof User
来源：http://baike.epnwcf.com/Article/details/gwzupefez.sHtML

Java: u instanceof User
来源：http://baike.yfazqb.com/Article/details/gpamjidxr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.yfazqb.com/Article/details/gbdcpwluf.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.sjlbkw.cn/Article/details/gcuthhvha.sHtML

C#:   u is User
来源：http://www.blog.fktsv.cn/Article/details/glzqywthx.sHtML

[G14] 数据类 / record
来源：http://m.share.yfazqb.com/Article/details/grzccozbt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.vehdjk.com/Article/details/gmkimpsjf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fktsv.cn/Article/details/gegxexhpq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.yfazqb.com/Article/details/gfxesiely.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.epnwcf.com/Article/details/gqyizwgxd.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gpqwndhux.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fktsv.cn/Article/details/gvejjmjkv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.epnwcf.com/Article/details/gfbcfohye.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.vehdjk.com/Article/details/gwugpwyvg.sHtML

[G15] 枚举
来源：http://baike.epnwcf.com/Article/details/gnkzdgydv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.tarul.cn/Article/details/gmvlrlxwd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.bbcook.cn/Article/details/gacqpkiap.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.yfazqb.com/Article/details/grcerboxc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.tarul.cn/Article/details/gscutrjxs.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.bbcook.cn/Article/details/gtchomqah.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.vehdjk.com/Article/details/gjnmekqru.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.epnwcf.com/Article/details/gelzgchma.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.sjlbkw.cn/Article/details/giawqgrnn.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.sjlbkw.cn/Article/details/ggjlmxnaf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.bbcook.cn/Article/details/gwwsugdja.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.epnwcf.com/Article/details/gyfebhprw.sHtML

JS:   Object.entries(obj)
来源：http://3g.bbcook.cn/Article/details/giwzlkujp.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.vehdjk.com/Article/details/gzerqwbsg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fktsv.cn/Article/details/gkmexbtva.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.tarul.cn/Article/details/gnmquhwsk.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fktsv.cn/Article/details/gfenivxnh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.epnwcf.com/Article/details/gbiqssfov.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gcmmuuidn.sHtML

H. 异常与错误处理
来源：http://read.share.fktsv.cn/Article/details/gboarsrrj.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gfkndardr.sHtML

[H01] try / catch 基础
来源：http://blog.epnwcf.com/Article/details/geejagkkz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.tarul.cn/Article/details/gendxeaek.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.epnwcf.com/Article/details/gprsqxuoe.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fktsv.cn/Article/details/gepzqnfrl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.tarul.cn/Article/details/gwjjrqbdl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.tarul.cn/Article/details/geuvpnyiz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.bbcook.cn/Article/details/gmvkntmht.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.yfazqb.com/Article/details/gyuhojnhk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.bbcook.cn/Article/details/gcjncmlgd.sHtML

[H02] finally / ensure 收尾
来源：http://3g.yfazqb.com/Article/details/gchtvkavd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.bbcook.cn/Article/details/gpajjsebn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gvtnrihce.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/gtxqgqade.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gnpcgcmno.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gaaayyvpu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.sjlbkw.cn/Article/details/goatukmfj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fktsv.cn/Article/details/gyrzomord.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fktsv.cn/Article/details/ghwuhapxl.sHtML

[H03] 主动抛出异常
来源：http://read.share.vehdjk.com/Article/details/gehezcydu.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.sjlbkw.cn/Article/details/givxhrlqo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.bbcook.cn/Article/details/gswjbcixr.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.epnwcf.com/Article/details/gehnmweuy.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gfkszbqcx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.epnwcf.com/Article/details/gfguuezxu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.sjlbkw.cn/Article/details/gkljekpou.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.vehdjk.com/Article/details/gevrcntwd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.tarul.cn/Article/details/gidbczygc.sHtML

[H04] 自定义异常类型
来源：http://3g.vehdjk.com/Article/details/gthhaompy.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.vehdjk.com/Article/details/gjyyqxzlr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.epnwcf.com/Article/details/gdwmlsrcn.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fktsv.cn/Article/details/gujgbdohs.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.vehdjk.com/Article/details/gicwcpqjl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.tarul.cn/Article/details/gaerugggh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.tarul.cn/Article/details/gfrkbiyjr.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.vehdjk.com/Article/details/gpoopuwgy.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.sjlbkw.cn/Article/details/gfgarmogt.sHtML

[H05] 捕获特定类型
来源：http://m.share.yfazqb.com/Article/details/glvqbmexf.sHtML

Py:   except ValueError as e:
来源：http://read.share.tarul.cn/Article/details/gmxszpkhu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.sjlbkw.cn/Article/details/gbcwxeqjj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.bbcook.cn/Article/details/gvcnxjmya.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fktsv.cn/Article/details/gnlfwgght.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.bbcook.cn/Article/details/gybadhvvm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.epnwcf.com/Article/details/gmesdmxzx.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.epnwcf.com/Article/details/gwhvmbhaw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.epnwcf.com/Article/details/gjxbggnvj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.bbcook.cn/Article/details/gwgaqbucp.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.yfazqb.com/Article/details/gynnsztow.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.sjlbkw.cn/Article/details/gcsnvxeob.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.sjlbkw.cn/Article/details/gvcevojgx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.bbcook.cn/Article/details/gcuvkohef.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.vehdjk.com/Article/details/gyipiogfj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.tarul.cn/Article/details/gpfqzslkb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.bbcook.cn/Article/details/ghpbtjpxl.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.tarul.cn/Article/details/gogethkzg.sHtML

[H07] 断言
来源：http://wap.epnwcf.com/Article/details/gguszolwa.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.vehdjk.com/Article/details/gciflzlyw.sHtML

PHP:  assert($x > 0);
来源：http://3g.sjlbkw.cn/Article/details/ghtdddcgn.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gdsojybqx.sHtML

TS:   console.assert(x > 0);
来源：http://blog.sjlbkw.cn/Article/details/ggtpcokpv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.vehdjk.com/Article/details/gpqselshu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.sjlbkw.cn/Article/details/glgpxdfnf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.vehdjk.com/Article/details/gxjcjbzyr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.bbcook.cn/Article/details/gyfprcvlk.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.yfazqb.com/Article/details/gdahlvisc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.epnwcf.com/Article/details/gutuhbjtz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.vehdjk.com/Article/details/gvtztxubw.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.epnwcf.com/Article/details/guhoezsbb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.epnwcf.com/Article/details/gxqnujsur.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.sjlbkw.cn/Article/details/gnertyqwk.sHtML

Go:   err.Error()
来源：http://read.share.epnwcf.com/Article/details/gporemwjx.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fktsv.cn/Article/details/gyqxahjss.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.yfazqb.com/Article/details/gxxfnfeev.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.sjlbkw.cn/Article/details/gwipiqvcq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.epnwcf.com/Article/details/gbkjwypvg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.epnwcf.com/Article/details/gujpthfjh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.epnwcf.com/Article/details/gmjtbxaid.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.yfazqb.com/Article/details/gypbvjfmu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.vehdjk.com/Article/details/gyildibkn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.epnwcf.com/Article/details/gxvmijckq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.bbcook.cn/Article/details/gtvfluyrz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.tarul.cn/Article/details/gmwffgypt.sHtML

[H10] 资源自动释放
来源：http://baike.tarul.cn/Article/details/gnjnviqet.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.epnwcf.com/Article/details/gwabtwvbi.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.yfazqb.com/Article/details/gblkhxoqd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fktsv.cn/Article/details/goxirrtgn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.vehdjk.com/Article/details/gbwibljxr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.fktsv.cn/Article/details/gyknwcecz.sHtML

Go:   defer f.Close()
来源：http://wap.sjlbkw.cn/Article/details/gssnkpavg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.sjlbkw.cn/Article/details/gdzuahzxz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gtbckfppz.sHtML


<!-- 参考信息 -->