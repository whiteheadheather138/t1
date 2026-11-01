代发 wailian999

Ruby: File.delete("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gadvarsux.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.vehdjk.com/Article/details/gasbstiwx.sHtML

[F07] 创建目录（含多级）
来源：http://blog.epnwcf.com/Article/details/gdbijmpng.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.sjlbkw.cn/Article/details/gnreuavdt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.yfazqb.com/Article/details/gemwdpihc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.vehdjk.com/Article/details/gtaurwiul.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.tarul.cn/Article/details/gwsqnifno.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.bbcook.cn/Article/details/gdxlnofpz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.bbcook.cn/Article/details/gtijvpyqa.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.yfazqb.com/Article/details/gwwurpzpw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fktsv.cn/Article/details/gaanaxkqe.sHtML

[F08] 遍历目录
来源：http://baike.fktsv.cn/Article/details/ggkxdwbtr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.sjlbkw.cn/Article/details/gxiwwhdau.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.vehdjk.com/Article/details/gzotixccl.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.sjlbkw.cn/Article/details/gnndvckop.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.tarul.cn/Article/details/gcqnoosvk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.epnwcf.com/Article/details/gpqtghsbc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.sjlbkw.cn/Article/details/getkqwqvg.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.yfazqb.com/Article/details/gmtuhwbvv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.epnwcf.com/Article/details/gprzvqjee.sHtML

[F09] 获取文件大小
来源：http://baike.sjlbkw.cn/Article/details/gkgbinano.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gujixinmu.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gsyjlocpz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fktsv.cn/Article/details/gikvwamyh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.bbcook.cn/Article/details/gdyukeiww.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/gdgcnrgzs.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.epnwcf.com/Article/details/gzcxgmmsd.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fktsv.cn/Article/details/gyfwnuwms.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.sjlbkw.cn/Article/details/gpywnioiz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fktsv.cn/Article/details/gnnqnrkew.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.tarul.cn/Article/details/gyzewzict.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.tarul.cn/Article/details/gqcowkjck.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gnxyirbsm.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gqxvsxgld.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.sjlbkw.cn/Article/details/grbzujjqu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gsiiohzoh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/gfqdsjswa.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gegwgogmy.sHtML

[F11] 复制与移动文件
来源：http://mobile.fktsv.cn/Article/details/gtwmaxcqg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gyzqbeuhk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/giruymoho.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/gmanbfnsp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/gbfzntpaj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.sjlbkw.cn/Article/details/glxdclzfm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fktsv.cn/Article/details/gbfyfrvif.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/gvkxqlxty.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.epnwcf.com/Article/details/gkjtoyluh.sHtML

[F12] CSV 读写
来源：http://www.blog.bbcook.cn/Article/details/gzzyzergw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.tarul.cn/Article/details/gfgzuffon.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.bbcook.cn/Article/details/gdlfhecmj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.bbcook.cn/Article/details/gmqidnljm.sHtML

TS:   // 同上
来源：http://www.m.share.epnwcf.com/Article/details/gkygsgtae.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.tarul.cn/Article/details/gcaeibiae.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fktsv.cn/Article/details/gezvsdhyv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.sjlbkw.cn/Article/details/gztwrihdc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.bbcook.cn/Article/details/gapzthrye.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gnzzvgiea.sHtML

G. 面向对象
来源：http://wap.bbcook.cn/Article/details/gyvezdrnj.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gebfycrse.sHtML

[G01] 定义类
来源：http://mobile.bbcook.cn/Article/details/gxdnhqoxx.sHtML

Py:   class User: pass
来源：http://www.blog.sjlbkw.cn/Article/details/gebifgxxg.sHtML

PHP:  class User {}
来源：http://wap.tarul.cn/Article/details/gksvzchba.sHtML

JS:   class User {}
来源：http://wap.vehdjk.com/Article/details/gnofykgxw.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.tarul.cn/Article/details/ghhpyvsze.sHtML

Java: class User {}
来源：http://www.share.sjlbkw.cn/Article/details/gxlsoymlw.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.bbcook.cn/Article/details/gvvmjhmhn.sHtML

Ruby: class User; end
来源：http://mobile.sjlbkw.cn/Article/details/gidwjrkpi.sHtML

C#:   class User {}
来源：http://www.blog.tarul.cn/Article/details/gfgbsyvmb.sHtML

[G02] 构造函数
来源：http://baike.tarul.cn/Article/details/gekwhnffv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.bbcook.cn/Article/details/gdzqlwivd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.sjlbkw.cn/Article/details/gkrmvecsz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fktsv.cn/Article/details/gbakqeuwc.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.epnwcf.com/Article/details/gextnfabm.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.vehdjk.com/Article/details/gtubugrtm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.epnwcf.com/Article/details/ghyzghvjg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.bbcook.cn/Article/details/giulrsuin.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.tarul.cn/Article/details/gyexpqpne.sHtML

[G03] 实例属性
来源：http://blog.yfazqb.com/Article/details/gicicdfkm.sHtML

Py:   self.name = "x"
来源：http://www.share.fktsv.cn/Article/details/gzddevgio.sHtML

PHP:  public string $name = "x";
来源：http://baike.tarul.cn/Article/details/gmrwzjcwn.sHtML

JS:   this.name = "x";
来源：http://www.m.share.bbcook.cn/Article/details/gnnhwqbjy.sHtML

TS:   name: string = "x";
来源：http://www.blog.bbcook.cn/Article/details/gszbdcfcr.sHtML

Java: private String name;
来源：http://mobile.tarul.cn/Article/details/gqvigfjwg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.bbcook.cn/Article/details/ghukpbyja.sHtML

Ruby: @name = "x"
来源：http://m.share.yfazqb.com/Article/details/goytctxqs.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.sjlbkw.cn/Article/details/glwmrajpc.sHtML

[G04] 定义方法
来源：http://baike.vehdjk.com/Article/details/gywzajwga.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.epnwcf.com/Article/details/ghjqfdfmb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fktsv.cn/Article/details/gkzlneyrq.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.vehdjk.com/Article/details/gizgilxas.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/gdtwxwwhm.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.tarul.cn/Article/details/giyibiuls.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.yfazqb.com/Article/details/gafpnvoka.sHtML

Ruby: def greet; @name; end
来源：http://blog.vehdjk.com/Article/details/gucvqhlmn.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fktsv.cn/Article/details/gvilwilxn.sHtML

[G05] 继承
来源：http://baike.vehdjk.com/Article/details/gwsvmcwtm.sHtML

Py:   class Admin(User): pass
来源：http://read.share.tarul.cn/Article/details/gqmbchnuy.sHtML

PHP:  class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/gvoyczzbq.sHtML

JS:   class Admin extends User {}
来源：http://www.share.sjlbkw.cn/Article/details/ghaqyywtr.sHtML

TS:   class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gqeglqtgr.sHtML

Java: class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/gnsujllml.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.yfazqb.com/Article/details/gmwwostep.sHtML

Ruby: class Admin < User; end
来源：http://m.share.vehdjk.com/Article/details/guitkttyi.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.epnwcf.com/Article/details/gldrpqsok.sHtML

[G06] 重写方法
来源：http://www.m.share.yfazqb.com/Article/details/glzvyxrst.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fktsv.cn/Article/details/gmwmnlyoy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gsaqxqwze.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/ghhtfdicq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gbjayytfw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/gkjmbzuck.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.tarul.cn/Article/details/gxnbkudnf.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fktsv.cn/Article/details/gprqrnlxb.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fktsv.cn/Article/details/gslkebgjp.sHtML

[G07] 调用父类方法
来源：http://m.share.tarul.cn/Article/details/geoxgyhbh.sHtML

Py:   super().greet()
来源：http://baike.epnwcf.com/Article/details/gzayshuxv.sHtML

PHP:  parent::greet();
来源：http://baike.epnwcf.com/Article/details/gmqmgkefu.sHtML

JS:   super.greet();
来源：http://blog.vehdjk.com/Article/details/giivytded.sHtML

TS:   super.greet();
来源：http://read.share.vehdjk.com/Article/details/ggjmclqlh.sHtML

Java: super.greet();
来源：http://m.share.yfazqb.com/Article/details/gysmjyrta.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.tarul.cn/Article/details/gqcncgpjn.sHtML

Ruby: super
来源：http://www.share.vehdjk.com/Article/details/gfvkdcdsy.sHtML

C#:   base.Greet();
来源：http://m.share.fktsv.cn/Article/details/glkeqobac.sHtML

[G08] 静态方法与属性
来源：http://mobile.epnwcf.com/Article/details/gjhlrpynn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.sjlbkw.cn/Article/details/gzqbexcsm.sHtML

PHP:  public static function f() {}
来源：http://www.share.yfazqb.com/Article/details/gvzrnsorr.sHtML

JS:   static f() {}
来源：http://baike.yfazqb.com/Article/details/gxnllzfeq.sHtML

TS:   static f(): void {}
来源：http://mobile.epnwcf.com/Article/details/gkhiqtjst.sHtML

Java: static void f() {}
来源：http://mobile.vehdjk.com/Article/details/gvpjdgvdj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.epnwcf.com/Article/details/gelbhgxmd.sHtML

Ruby: def self.f; end
来源：http://mobile.bbcook.cn/Article/details/gcyvspwqa.sHtML

C#:   public static void F() {}
来源：http://mobile.sjlbkw.cn/Article/details/gaknzlbnm.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fktsv.cn/Article/details/gryglnyvp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fktsv.cn/Article/details/gxhyldkiu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.epnwcf.com/Article/details/gyqzslgse.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.tarul.cn/Article/details/giijhouih.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.tarul.cn/Article/details/ggkzylyoi.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fktsv.cn/Article/details/gdviqkwyr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdezjwjju.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.bbcook.cn/Article/details/gxezcbsln.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.yfazqb.com/Article/details/grzqmqlnj.sHtML

[G10] 访问控制
来源：http://wap.tarul.cn/Article/details/ghzpcgeuv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.tarul.cn/Article/details/gfxvjuddz.sHtML

PHP:  public / protected / private
来源：http://baike.tarul.cn/Article/details/gzixuhvzb.sHtML

JS:   #private 字段；其余公开
来源：http://wap.sjlbkw.cn/Article/details/gcodttjok.sHtML

TS:   public / protected / private
来源：http://3g.bbcook.cn/Article/details/gscoituje.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.epnwcf.com/Article/details/gqbotxxgi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.bbcook.cn/Article/details/gudmpramy.sHtML

Ruby: public / protected / private
来源：http://www.m.share.epnwcf.com/Article/details/ggepzzdau.sHtML

C#:   public / protected / private / internal
来源：http://baike.yfazqb.com/Article/details/gjoepsdgg.sHtML

[G11] getter / setter
来源：http://mobile.yfazqb.com/Article/details/gtroxtavk.sHtML

Py:   @property 与 @x.setter
来源：http://3g.vehdjk.com/Article/details/gvwqptyvs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.vehdjk.com/Article/details/goqfdhejn.sHtML

JS:   get name() { return this._name; }
来源：http://baike.sjlbkw.cn/Article/details/grxddyisz.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fktsv.cn/Article/details/gnmwfskkl.sHtML

Java: public String getName() { return name; }
来源：http://baike.sjlbkw.cn/Article/details/gzhxeykpo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.tarul.cn/Article/details/gqungexna.sHtML

Ruby: attr_accessor :name
来源：http://read.share.bbcook.cn/Article/details/gzzercrzo.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.vehdjk.com/Article/details/gydbffexn.sHtML

[G12] 对象转字符串
来源：http://3g.epnwcf.com/Article/details/gbqogjpko.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.bbcook.cn/Article/details/gyigfowei.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.tarul.cn/Article/details/gqrewmvez.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/gskpicrfx.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.vehdjk.com/Article/details/gynpyjugl.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.yfazqb.com/Article/details/glkalcnfh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.bbcook.cn/Article/details/ggpflptnh.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fktsv.cn/Article/details/guziuhpzv.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fktsv.cn/Article/details/gocwfppnv.sHtML

[G13] 判断对象类型
来源：http://read.share.bbcook.cn/Article/details/gynafytao.sHtML

Py:   isinstance(u, User)
来源：http://3g.vehdjk.com/Article/details/gsmbpqafg.sHtML

PHP:  $u instanceof User
来源：http://m.share.vehdjk.com/Article/details/gbeduuivd.sHtML

JS:   u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/gzcuihluw.sHtML

TS:   u instanceof User
来源：http://www.share.bbcook.cn/Article/details/gbvitgytt.sHtML

Java: u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/guxseuicn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.sjlbkw.cn/Article/details/gnswvifyv.sHtML

Ruby: u.is_a?(User)
来源：http://blog.yfazqb.com/Article/details/geilavtme.sHtML

C#:   u is User
来源：http://mobile.yfazqb.com/Article/details/gzalwbyyn.sHtML

[G14] 数据类 / record
来源：http://wap.bbcook.cn/Article/details/gizooallk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.yfazqb.com/Article/details/gsrvkvlkf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.vehdjk.com/Article/details/gtfhappxh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.bbcook.cn/Article/details/gewzlbvof.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.bbcook.cn/Article/details/gzrnyzhde.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.epnwcf.com/Article/details/gbtitoiqr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fktsv.cn/Article/details/glxfpujwl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.yfazqb.com/Article/details/gmimkkyhp.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.vehdjk.com/Article/details/gxqcwljsc.sHtML

[G15] 枚举
来源：http://blog.vehdjk.com/Article/details/gpvxyclza.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fktsv.cn/Article/details/gyxphhtcp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.tarul.cn/Article/details/gzpscebuw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.vehdjk.com/Article/details/gbungerry.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.bbcook.cn/Article/details/gtgaeeahg.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fktsv.cn/Article/details/gtkxnalzi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.yfazqb.com/Article/details/ghjkjpjqb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.epnwcf.com/Article/details/gzcxuyhpa.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.epnwcf.com/Article/details/gllhuaffg.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.yfazqb.com/Article/details/gtfkhapev.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.epnwcf.com/Article/details/gfpjwgryq.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.tarul.cn/Article/details/gbrnrbcvg.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gvmxfllgz.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/ghenftaat.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.epnwcf.com/Article/details/guxdbmfgh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.bbcook.cn/Article/details/gflxnsqrr.sHtML

Ruby: obj.instance_variables
来源：http://3g.epnwcf.com/Article/details/gxgypnppc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.epnwcf.com/Article/details/ggzkxparz.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gfnkwihip.sHtML

H. 异常与错误处理
来源：http://www.blog.sjlbkw.cn/Article/details/gfzzegwce.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gqglyamsr.sHtML

[H01] try / catch 基础
来源：http://www.share.sjlbkw.cn/Article/details/gtwlxfugt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.vehdjk.com/Article/details/gxhapikst.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.tarul.cn/Article/details/ghpcrscjk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.vehdjk.com/Article/details/gycuiauet.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fktsv.cn/Article/details/grkrfxkaj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.bbcook.cn/Article/details/gjdhcolel.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.bbcook.cn/Article/details/gxevcwuuc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.vehdjk.com/Article/details/geoqkbtpc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.bbcook.cn/Article/details/gaxckbuyx.sHtML

[H02] finally / ensure 收尾
来源：http://wap.vehdjk.com/Article/details/gzpahqeov.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.epnwcf.com/Article/details/ghtgswrcn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gqrsgucat.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/ghuodblgr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gxwzfcgcy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gbplxcbzj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.sjlbkw.cn/Article/details/gegwclsyn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.bbcook.cn/Article/details/gwkqprjca.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/gqjzqifvg.sHtML

[H03] 主动抛出异常
来源：http://www.share.vehdjk.com/Article/details/gxzforwaz.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.sjlbkw.cn/Article/details/grrbejzqn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/gnccdzyeg.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gvixnaurf.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fktsv.cn/Article/details/gyhvcfdlr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.tarul.cn/Article/details/glvxfslvx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fktsv.cn/Article/details/getvmwidh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.tarul.cn/Article/details/gvvbdjwdu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gpfrvkbqx.sHtML

[H04] 自定义异常类型
来源：http://3g.vehdjk.com/Article/details/gyvgpxjdx.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.yfazqb.com/Article/details/gdcqgjxfm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.vehdjk.com/Article/details/gcfwfmuqu.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.yfazqb.com/Article/details/gojuuyupf.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.epnwcf.com/Article/details/gjueyydjy.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fktsv.cn/Article/details/gkxggqsen.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.bbcook.cn/Article/details/ghnrhljss.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.epnwcf.com/Article/details/geruyjlwy.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fktsv.cn/Article/details/gjdmiafgu.sHtML

[H05] 捕获特定类型
来源：http://wap.sjlbkw.cn/Article/details/gdkyltuay.sHtML

Py:   except ValueError as e:
来源：http://m.share.epnwcf.com/Article/details/gbozgrggs.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.sjlbkw.cn/Article/details/gqlgygiig.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.tarul.cn/Article/details/gvamtzljl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.vehdjk.com/Article/details/goufykkje.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.epnwcf.com/Article/details/gpsgziwje.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.yfazqb.com/Article/details/ggwsiuyhn.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.epnwcf.com/Article/details/gwlrswmlf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.bbcook.cn/Article/details/glkggpuob.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.sjlbkw.cn/Article/details/goydoiisg.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.tarul.cn/Article/details/gsvsgewgh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.tarul.cn/Article/details/gkiticujo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.yfazqb.com/Article/details/gcoitmpbv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fktsv.cn/Article/details/glilgoqnu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fktsv.cn/Article/details/ghmijyckq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.bbcook.cn/Article/details/glrhvcbcy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.tarul.cn/Article/details/gmcqfmowp.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.tarul.cn/Article/details/gmyijfspp.sHtML

[H07] 断言
来源：http://www.share.tarul.cn/Article/details/glmowkwes.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fktsv.cn/Article/details/gpuvwlvpg.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/ggictwamr.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fktsv.cn/Article/details/gkveeadtk.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/giaieiwrc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.epnwcf.com/Article/details/gpxkxqrly.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.yfazqb.com/Article/details/gbdowivtf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fktsv.cn/Article/details/grgcwknyd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.yfazqb.com/Article/details/gawpteeiu.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.tarul.cn/Article/details/gdbjdozwg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.vehdjk.com/Article/details/ggomolcpr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.sjlbkw.cn/Article/details/gevsfjngl.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.sjlbkw.cn/Article/details/geqkrvkup.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.yfazqb.com/Article/details/gbaxsvpue.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.sjlbkw.cn/Article/details/gqdrppcdn.sHtML

Go:   err.Error()
来源：http://wap.bbcook.cn/Article/details/gigegaipw.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.tarul.cn/Article/details/gvkfxcmdr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.epnwcf.com/Article/details/gyyuhvkbt.sHtML

[H09] 带错误码的异常
来源：http://m.share.bbcook.cn/Article/details/gohczkbik.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.bbcook.cn/Article/details/gykkeusux.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.yfazqb.com/Article/details/ghqffhwpp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.bbcook.cn/Article/details/gfvcaghmx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.sjlbkw.cn/Article/details/gathhkdwu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.sjlbkw.cn/Article/details/girdkfmzh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.tarul.cn/Article/details/gvkgqjkqg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.vehdjk.com/Article/details/glutghrtk.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.sjlbkw.cn/Article/details/gbsitpzvf.sHtML

[H10] 资源自动释放
来源：http://m.share.epnwcf.com/Article/details/gpoctgxap.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.tarul.cn/Article/details/gtqomfmth.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.tarul.cn/Article/details/gmetetpxa.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.vehdjk.com/Article/details/gfolmotxb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.sjlbkw.cn/Article/details/gzerljlwl.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.tarul.cn/Article/details/grsjyalwf.sHtML

Go:   defer f.Close()
来源：http://blog.sjlbkw.cn/Article/details/gezgpbycl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.tarul.cn/Article/details/gyeastmdt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.fktsv.cn/Article/details/gvqlxdkng.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gfehdqmno.sHtML

I. 正则表达式
来源：http://www.share.sjlbkw.cn/Article/details/gnvbhxebu.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gxtvngbtw.sHtML

[I01] 判断是否匹配
来源：http://www.blog.sjlbkw.cn/Article/details/ghjypfdfr.sHtML


<!-- 参考信息 -->