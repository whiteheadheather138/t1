代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gsuqrqyjo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gcqnebbra.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/gfuivsdmt.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.tarul.cn/Article/details/givasmxcl.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gthxypubp.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.epnwcf.com/Article/details/gdsyfbthp.sHtML

[F07] 创建目录（含多级）
来源：http://baike.epnwcf.com/Article/details/giwkieead.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.tarul.cn/Article/details/grblmesiq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fktsv.cn/Article/details/gbaxmekcf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.epnwcf.com/Article/details/gozwrarak.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.vehdjk.com/Article/details/gettyqmtc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.sjlbkw.cn/Article/details/gfhncmdkq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.yfazqb.com/Article/details/ggtmkwnrm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.yfazqb.com/Article/details/gbohfypqc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.sjlbkw.cn/Article/details/gwrdvmfkm.sHtML

[F08] 遍历目录
来源：http://www.blog.tarul.cn/Article/details/gmhyhvvkc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fktsv.cn/Article/details/gmfjjjlym.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fktsv.cn/Article/details/gwsmuiges.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.bbcook.cn/Article/details/gkagyvpzc.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.sjlbkw.cn/Article/details/ggnyweone.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fktsv.cn/Article/details/gcxqgqlfn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.sjlbkw.cn/Article/details/guvzdrmwl.sHtML

Ruby: Dir.children("dir")
来源：http://blog.bbcook.cn/Article/details/gnipemznt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.yfazqb.com/Article/details/gxhimhwxa.sHtML

[F09] 获取文件大小
来源：http://www.blog.tarul.cn/Article/details/gydztgglf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/ghdwsuwal.sHtML

PHP:  filesize("a.txt");
来源：http://blog.epnwcf.com/Article/details/gyvmtcsuy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.tarul.cn/Article/details/gotxdhlgu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.vehdjk.com/Article/details/ggxajlaau.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/gfuhecpnj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.epnwcf.com/Article/details/gkywaooda.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gfbvyunsg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.tarul.cn/Article/details/gkhwlhqkf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.sjlbkw.cn/Article/details/gvuxreqhm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gezbgoled.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fktsv.cn/Article/details/gyumjrdvz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gyusvjpzl.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gwqflducs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.vehdjk.com/Article/details/gxvhbcyte.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/glhhmqecu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gjoxloskb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gklzhvukc.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.bbcook.cn/Article/details/gxipprhtj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/gdhttthcp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.yfazqb.com/Article/details/gyrzbxvfv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gvgcfcxvb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/gbphmmpiy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fktsv.cn/Article/details/gvxckvacf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.tarul.cn/Article/details/gwjxbwejf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/gmyscznux.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.epnwcf.com/Article/details/gkzsjvspr.sHtML

[F12] CSV 读写
来源：http://www.share.yfazqb.com/Article/details/gagatrejs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.epnwcf.com/Article/details/gewkmbkut.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.epnwcf.com/Article/details/ggfcmhlpg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.bbcook.cn/Article/details/gfbhalqcl.sHtML

TS:   // 同上
来源：http://www.m.share.sjlbkw.cn/Article/details/gsichfwja.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fktsv.cn/Article/details/gwkxccnic.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.yfazqb.com/Article/details/gnvxbmofn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.sjlbkw.cn/Article/details/glwbnrxej.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.epnwcf.com/Article/details/giytidyjn.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gsthmdvrd.sHtML

G. 面向对象
来源：http://blog.bbcook.cn/Article/details/ghvrcrbjk.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/ghtvoxptk.sHtML

[G01] 定义类
来源：http://baike.fktsv.cn/Article/details/gabhbuaiz.sHtML

Py:   class User: pass
来源：http://baike.vehdjk.com/Article/details/gpnwhffew.sHtML

PHP:  class User {}
来源：http://www.blog.vehdjk.com/Article/details/gmhxizhlt.sHtML

JS:   class User {}
来源：http://www.m.share.vehdjk.com/Article/details/gutaqsjwn.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.bbcook.cn/Article/details/gkfhwawdq.sHtML

Java: class User {}
来源：http://www.share.epnwcf.com/Article/details/ghuclahtv.sHtML

Go:   type User struct { Name string }
来源：http://3g.epnwcf.com/Article/details/gzsgslrbv.sHtML

Ruby: class User; end
来源：http://baike.vehdjk.com/Article/details/gzlyewanz.sHtML

C#:   class User {}
来源：http://www.share.tarul.cn/Article/details/getbiacvl.sHtML

[G02] 构造函数
来源：http://m.share.epnwcf.com/Article/details/gsscvrhax.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.sjlbkw.cn/Article/details/ghtkmsrck.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.tarul.cn/Article/details/gmhoxsqxt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.tarul.cn/Article/details/ggjnzkgbl.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.tarul.cn/Article/details/gmwlnwcpv.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.bbcook.cn/Article/details/gtsckkxdw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.vehdjk.com/Article/details/gppnfgskn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.tarul.cn/Article/details/geywnmwbl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.vehdjk.com/Article/details/gdluvxxoc.sHtML

[G03] 实例属性
来源：http://www.m.share.tarul.cn/Article/details/gklqldwkq.sHtML

Py:   self.name = "x"
来源：http://www.share.yfazqb.com/Article/details/gzusnqwsz.sHtML

PHP:  public string $name = "x";
来源：http://mobile.vehdjk.com/Article/details/ghmonopju.sHtML

JS:   this.name = "x";
来源：http://www.blog.epnwcf.com/Article/details/guimgocgn.sHtML

TS:   name: string = "x";
来源：http://3g.fktsv.cn/Article/details/gnwjgqgip.sHtML

Java: private String name;
来源：http://read.share.epnwcf.com/Article/details/gfjquwhrv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.yfazqb.com/Article/details/gsxxbonbe.sHtML

Ruby: @name = "x"
来源：http://m.share.bbcook.cn/Article/details/gqdkgpyeb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.bbcook.cn/Article/details/gfdeevkjo.sHtML

[G04] 定义方法
来源：http://read.share.tarul.cn/Article/details/gazvonznh.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.tarul.cn/Article/details/gemdszxkf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.sjlbkw.cn/Article/details/gocnwaltx.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.sjlbkw.cn/Article/details/gcvdnrvbi.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.bbcook.cn/Article/details/glpkijoat.sHtML

Java: String greet() { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gscmewlsc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.bbcook.cn/Article/details/gblxhinuc.sHtML

Ruby: def greet; @name; end
来源：http://www.share.sjlbkw.cn/Article/details/gbccrykvz.sHtML

C#:   public string Greet() => Name;
来源：http://blog.bbcook.cn/Article/details/ggsueigye.sHtML

[G05] 继承
来源：http://mobile.bbcook.cn/Article/details/gmpwzlgox.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fktsv.cn/Article/details/gwynxzzfn.sHtML

PHP:  class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gszthvoyx.sHtML

JS:   class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/gqiarxcpz.sHtML

TS:   class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/gdkenlaip.sHtML

Java: class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/gnsxsgmii.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fktsv.cn/Article/details/gapbcssuy.sHtML

Ruby: class Admin < User; end
来源：http://blog.fktsv.cn/Article/details/gjcsaulrw.sHtML

C#:   class Admin : User {}
来源：http://m.share.epnwcf.com/Article/details/gvnbeiqha.sHtML

[G06] 重写方法
来源：http://read.share.vehdjk.com/Article/details/gajwboran.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.vehdjk.com/Article/details/gragpnths.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/gezhfflpl.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/gjwfavrtq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/gwllxbtpv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/gjfixdvgj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fktsv.cn/Article/details/gqhudzacp.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.epnwcf.com/Article/details/gamrmdmmt.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.yfazqb.com/Article/details/gevoheded.sHtML

[G07] 调用父类方法
来源：http://m.share.epnwcf.com/Article/details/gnqyqjfqj.sHtML

Py:   super().greet()
来源：http://3g.vehdjk.com/Article/details/gbwfwjnsz.sHtML

PHP:  parent::greet();
来源：http://m.share.tarul.cn/Article/details/gcmtiosmf.sHtML

JS:   super.greet();
来源：http://blog.fktsv.cn/Article/details/gjbejpnez.sHtML

TS:   super.greet();
来源：http://mobile.fktsv.cn/Article/details/gwcdrjkdg.sHtML

Java: super.greet();
来源：http://3g.yfazqb.com/Article/details/gmmkotjcf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.yfazqb.com/Article/details/gzrodqoir.sHtML

Ruby: super
来源：http://3g.sjlbkw.cn/Article/details/gibntrvfb.sHtML

C#:   base.Greet();
来源：http://3g.bbcook.cn/Article/details/gergnkpos.sHtML

[G08] 静态方法与属性
来源：http://mobile.yfazqb.com/Article/details/gftckpgrr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.sjlbkw.cn/Article/details/gapxivnrj.sHtML

PHP:  public static function f() {}
来源：http://3g.vehdjk.com/Article/details/gnorjpwir.sHtML

JS:   static f() {}
来源：http://blog.vehdjk.com/Article/details/gnhjsbqns.sHtML

TS:   static f(): void {}
来源：http://wap.yfazqb.com/Article/details/gqahblrkd.sHtML

Java: static void f() {}
来源：http://www.share.vehdjk.com/Article/details/gwdculddc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.bbcook.cn/Article/details/gabcbqlad.sHtML

Ruby: def self.f; end
来源：http://www.m.share.tarul.cn/Article/details/gkakhnhjq.sHtML

C#:   public static void F() {}
来源：http://m.share.vehdjk.com/Article/details/ggjimibeh.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.yfazqb.com/Article/details/gqvystadd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.bbcook.cn/Article/details/gnjjsslgv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fktsv.cn/Article/details/gukrhzlzh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fktsv.cn/Article/details/gqhwyftas.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.yfazqb.com/Article/details/gsnjxczxr.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.tarul.cn/Article/details/gbcceiqew.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.yfazqb.com/Article/details/gymqihoxp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.sjlbkw.cn/Article/details/gcnymohbm.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.yfazqb.com/Article/details/gismyzzde.sHtML

[G10] 访问控制
来源：http://3g.bbcook.cn/Article/details/gfbydpeus.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.tarul.cn/Article/details/giwxiygts.sHtML

PHP:  public / protected / private
来源：http://3g.vehdjk.com/Article/details/gvhwnaqqf.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.vehdjk.com/Article/details/grjotftgd.sHtML

TS:   public / protected / private
来源：http://www.share.vehdjk.com/Article/details/gbemclqfa.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fktsv.cn/Article/details/gdtdfezhf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.tarul.cn/Article/details/gtgosuqwv.sHtML

Ruby: public / protected / private
来源：http://blog.sjlbkw.cn/Article/details/gffcfztkx.sHtML

C#:   public / protected / private / internal
来源：http://baike.sjlbkw.cn/Article/details/gqsutvxzr.sHtML

[G11] getter / setter
来源：http://m.share.fktsv.cn/Article/details/gthnxilgw.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.bbcook.cn/Article/details/gponjxnka.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/gfranevhq.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.bbcook.cn/Article/details/gfvpdpykn.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fktsv.cn/Article/details/gudrmaldv.sHtML

Java: public String getName() { return name; }
来源：http://wap.yfazqb.com/Article/details/gippyctxh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.vehdjk.com/Article/details/gypqkzepz.sHtML

Ruby: attr_accessor :name
来源：http://read.share.epnwcf.com/Article/details/gtyxeehjd.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.bbcook.cn/Article/details/gfszxzwrc.sHtML

[G12] 对象转字符串
来源：http://read.share.epnwcf.com/Article/details/gdnfbafkd.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.bbcook.cn/Article/details/gcqsszudw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/gzvvpvqoj.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gimvwztsr.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.epnwcf.com/Article/details/gyxwnhoso.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.yfazqb.com/Article/details/gbyfakqyg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.bbcook.cn/Article/details/gkkhaboyj.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.epnwcf.com/Article/details/glbzbmknb.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.bbcook.cn/Article/details/ggxcxezxv.sHtML

[G13] 判断对象类型
来源：http://www.blog.tarul.cn/Article/details/gnvulbjiq.sHtML

Py:   isinstance(u, User)
来源：http://mobile.sjlbkw.cn/Article/details/gnuaqejpe.sHtML

PHP:  $u instanceof User
来源：http://www.blog.tarul.cn/Article/details/gcizssszz.sHtML

JS:   u instanceof User
来源：http://www.share.yfazqb.com/Article/details/ghzkicftf.sHtML

TS:   u instanceof User
来源：http://m.share.tarul.cn/Article/details/gzgmevbyf.sHtML

Java: u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/gosfocnlx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.tarul.cn/Article/details/gbwtieeuf.sHtML

Ruby: u.is_a?(User)
来源：http://wap.yfazqb.com/Article/details/gipsxmqke.sHtML

C#:   u is User
来源：http://3g.tarul.cn/Article/details/gplgaecwz.sHtML

[G14] 数据类 / record
来源：http://baike.vehdjk.com/Article/details/gmgjxeaen.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.vehdjk.com/Article/details/ghaplqygv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.tarul.cn/Article/details/grlypkkxu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.epnwcf.com/Article/details/gflwwtxau.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.yfazqb.com/Article/details/gxdrsevvn.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fktsv.cn/Article/details/gyxgdtvyi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fktsv.cn/Article/details/gaxpycndn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.bbcook.cn/Article/details/gxwktizfc.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.bbcook.cn/Article/details/gmxujdngz.sHtML

[G15] 枚举
来源：http://m.share.fktsv.cn/Article/details/gkmcgflmp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.sjlbkw.cn/Article/details/ginnywdyu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.bbcook.cn/Article/details/gkrfrgbxl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.tarul.cn/Article/details/gqjbsurdv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.vehdjk.com/Article/details/gcbdmwaoi.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.bbcook.cn/Article/details/gvjnklvpb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.vehdjk.com/Article/details/gvlpxsuzn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.vehdjk.com/Article/details/gfnanxpzz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.bbcook.cn/Article/details/gontwiehs.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.tarul.cn/Article/details/gxvkioduc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.epnwcf.com/Article/details/grfxucvxj.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.epnwcf.com/Article/details/gaymsfdve.sHtML

JS:   Object.entries(obj)
来源：http://wap.vehdjk.com/Article/details/gisogwfif.sHtML

TS:   Object.entries(obj)
来源：http://m.share.bbcook.cn/Article/details/gbducxjmy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.sjlbkw.cn/Article/details/gzhemrbzp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.yfazqb.com/Article/details/gyxqgxiin.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.bbcook.cn/Article/details/gotcifrfu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.sjlbkw.cn/Article/details/gisnmqsdk.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gzxjzmfil.sHtML

H. 异常与错误处理
来源：http://blog.yfazqb.com/Article/details/gjisnbxvi.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gmlscufys.sHtML

[H01] try / catch 基础
来源：http://3g.yfazqb.com/Article/details/gpailretp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.tarul.cn/Article/details/gtecopglp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fktsv.cn/Article/details/gbvtnukai.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.tarul.cn/Article/details/gayctrrne.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.tarul.cn/Article/details/ggcqamhrq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.tarul.cn/Article/details/guuxrplit.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.yfazqb.com/Article/details/gzoqmtogq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.yfazqb.com/Article/details/gbxypvgbd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.sjlbkw.cn/Article/details/gnkvwyjrz.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.tarul.cn/Article/details/glnvddlry.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.tarul.cn/Article/details/gohinlnot.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gdigmmcwb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.epnwcf.com/Article/details/gfcjgnhke.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/gedpupdem.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gesvqxlaa.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.yfazqb.com/Article/details/gbwphrhtm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.tarul.cn/Article/details/gvzvzuefq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/gfejackqd.sHtML

[H03] 主动抛出异常
来源：http://mobile.fktsv.cn/Article/details/gnaftaqdz.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.tarul.cn/Article/details/gpkvstpnr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/ghmkzjhfb.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gagjooutu.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gljnsxbyz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/gzfiqqmro.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.epnwcf.com/Article/details/gezffslrp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.bbcook.cn/Article/details/gtclinrhl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/gnuqapmqs.sHtML

[H04] 自定义异常类型
来源：http://baike.epnwcf.com/Article/details/grgeeptfj.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fktsv.cn/Article/details/gmmmsnkoi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.vehdjk.com/Article/details/gqqpafnnx.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.yfazqb.com/Article/details/gjokehlnu.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.bbcook.cn/Article/details/geaivcbzq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.tarul.cn/Article/details/gotzeaury.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fktsv.cn/Article/details/giurzjzzn.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.bbcook.cn/Article/details/gujkdbrzp.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.tarul.cn/Article/details/gkadlnmit.sHtML

[H05] 捕获特定类型
来源：http://wap.epnwcf.com/Article/details/gfxsytaxa.sHtML

Py:   except ValueError as e:
来源：http://mobile.tarul.cn/Article/details/gjhfcfxva.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.sjlbkw.cn/Article/details/gzctqggdz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.sjlbkw.cn/Article/details/gabrlxnyd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.bbcook.cn/Article/details/glvpuylrm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.epnwcf.com/Article/details/gcpwzgrdy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fktsv.cn/Article/details/gpjwpwpxt.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.bbcook.cn/Article/details/gjztwivqr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.vehdjk.com/Article/details/ggprzkpke.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fktsv.cn/Article/details/gvyksmuex.sHtML

Py:   value = d.get("k") or default
来源：http://3g.bbcook.cn/Article/details/gixxrffdb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.epnwcf.com/Article/details/gorvoimsf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.bbcook.cn/Article/details/gxppqelix.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.epnwcf.com/Article/details/gwturudmp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.epnwcf.com/Article/details/gvmfpsbev.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fktsv.cn/Article/details/gmylqwfdz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.epnwcf.com/Article/details/grtkxroie.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.sjlbkw.cn/Article/details/gdklmhjua.sHtML

[H07] 断言
来源：http://baike.epnwcf.com/Article/details/guwrleyme.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.sjlbkw.cn/Article/details/gyqiknavz.sHtML

PHP:  assert($x > 0);
来源：http://blog.fktsv.cn/Article/details/gehrxewyt.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.bbcook.cn/Article/details/graonlfxn.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fktsv.cn/Article/details/gkurvvjym.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.vehdjk.com/Article/details/gbecknpui.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.tarul.cn/Article/details/gjpsuijus.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.yfazqb.com/Article/details/gdrebypip.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.bbcook.cn/Article/details/gmsilgdlw.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.epnwcf.com/Article/details/ggmmnnmnh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.vehdjk.com/Article/details/gnukqlgcl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.vehdjk.com/Article/details/gwmjqcszp.sHtML

JS:   e.message;  e.stack
来源：http://www.share.vehdjk.com/Article/details/gfilfbadr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fktsv.cn/Article/details/gfqtvibdm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.tarul.cn/Article/details/gajwgnvqu.sHtML

Go:   err.Error()
来源：http://mobile.sjlbkw.cn/Article/details/gnqqipmhy.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.bbcook.cn/Article/details/gqsyewaas.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.bbcook.cn/Article/details/gwhjcwvao.sHtML

[H09] 带错误码的异常
来源：http://blog.bbcook.cn/Article/details/gsylxizij.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.sjlbkw.cn/Article/details/gmipfksct.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.sjlbkw.cn/Article/details/gqlqbdfap.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.epnwcf.com/Article/details/gtziqscjx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.tarul.cn/Article/details/gpsotcjgi.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.vehdjk.com/Article/details/gicpqskbv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.tarul.cn/Article/details/gfgyakwrz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.yfazqb.com/Article/details/gaulqlctw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.yfazqb.com/Article/details/gogkawbok.sHtML

[H10] 资源自动释放
来源：http://3g.tarul.cn/Article/details/gawwwyqcs.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fktsv.cn/Article/details/givsvcbpp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.tarul.cn/Article/details/gcdccqpfl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.tarul.cn/Article/details/ggzddxyzh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.bbcook.cn/Article/details/gmcpsxgtm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fktsv.cn/Article/details/giszxovvq.sHtML

Go:   defer f.Close()
来源：http://blog.sjlbkw.cn/Article/details/gwgnfqmop.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.bbcook.cn/Article/details/gkzpumans.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.vehdjk.com/Article/details/ghrusdzlx.sHtML


<!-- 参考信息 -->