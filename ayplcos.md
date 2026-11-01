代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gfhwepfwv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gybcwzrpg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/gqzrhrgzm.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.tarul.cn/Article/details/gdgxoccgi.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.yfazqb.com/Article/details/gcwagrdsz.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.tarul.cn/Article/details/gneglsjei.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.epnwcf.com/Article/details/gxfaixnsc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.bbcook.cn/Article/details/gztlqlgtd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fktsv.cn/Article/details/gdvcsjiyp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.tarul.cn/Article/details/gzncgxnba.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.epnwcf.com/Article/details/gaztaolsk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.tarul.cn/Article/details/gvzjforpo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.epnwcf.com/Article/details/gzklwofqh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.tarul.cn/Article/details/gxbvqjgrr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.vehdjk.com/Article/details/gyqcvsfli.sHtML

[F08] 遍历目录
来源：http://wap.yfazqb.com/Article/details/gnemoqlwe.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.yfazqb.com/Article/details/gfyidsbiy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.sjlbkw.cn/Article/details/gcipbmfaa.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.vehdjk.com/Article/details/gxwrilxgd.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.epnwcf.com/Article/details/gsdpexrfv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.epnwcf.com/Article/details/gqjbgtugj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.epnwcf.com/Article/details/gxksakngl.sHtML

Ruby: Dir.children("dir")
来源：http://baike.bbcook.cn/Article/details/goodappkw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fktsv.cn/Article/details/gosqzdhtt.sHtML

[F09] 获取文件大小
来源：http://www.blog.sjlbkw.cn/Article/details/gxjaadaty.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.vehdjk.com/Article/details/gapwzienh.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gufbptqxz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.sjlbkw.cn/Article/details/gqreiimdp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fktsv.cn/Article/details/gzrqxaclx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.vehdjk.com/Article/details/gncmvkwam.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.tarul.cn/Article/details/gbtpjnpuz.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gulgrdigu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.yfazqb.com/Article/details/grndzxloi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.tarul.cn/Article/details/gpotpmihz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/ghalygkqh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.bbcook.cn/Article/details/ghumufgqe.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/ghqurdlss.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gizatpjez.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fktsv.cn/Article/details/gahibyaio.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gpxhgxlfj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gyqnoqdoo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gggzmqwks.sHtML

[F11] 复制与移动文件
来源：http://mobile.tarul.cn/Article/details/gacdevuwu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/gauljaklc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.tarul.cn/Article/details/gcfbevwdy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.bbcook.cn/Article/details/ghegaukvo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gryovlgkc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.vehdjk.com/Article/details/gfsrzooue.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.tarul.cn/Article/details/gierxbtot.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/guwfgrgei.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.vehdjk.com/Article/details/giejfevbj.sHtML

[F12] CSV 读写
来源：http://m.share.fktsv.cn/Article/details/glfevedsm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.vehdjk.com/Article/details/gbiehftff.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.epnwcf.com/Article/details/gacimdmio.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.tarul.cn/Article/details/ggukxnpyq.sHtML

TS:   // 同上
来源：http://baike.vehdjk.com/Article/details/gonueqeax.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.yfazqb.com/Article/details/gmdlrtwwe.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fktsv.cn/Article/details/ggtnnvyuh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.yfazqb.com/Article/details/glhrrnoqk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fktsv.cn/Article/details/gkqhshcen.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gstsveuod.sHtML

G. 面向对象
来源：http://mobile.epnwcf.com/Article/details/ghnimczdc.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gxtvxkagi.sHtML

[G01] 定义类
来源：http://baike.vehdjk.com/Article/details/gdczocjgq.sHtML

Py:   class User: pass
来源：http://baike.yfazqb.com/Article/details/ghajlzrbu.sHtML

PHP:  class User {}
来源：http://blog.fktsv.cn/Article/details/geteyqlog.sHtML

JS:   class User {}
来源：http://www.share.fktsv.cn/Article/details/grgnhqzxw.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.vehdjk.com/Article/details/grfmyxkbd.sHtML

Java: class User {}
来源：http://m.share.vehdjk.com/Article/details/gscusximm.sHtML

Go:   type User struct { Name string }
来源：http://mobile.vehdjk.com/Article/details/gjfxgqqcq.sHtML

Ruby: class User; end
来源：http://www.blog.tarul.cn/Article/details/gbouinesd.sHtML

C#:   class User {}
来源：http://baike.yfazqb.com/Article/details/gosxfqcvu.sHtML

[G02] 构造函数
来源：http://read.share.epnwcf.com/Article/details/gacumoyez.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.tarul.cn/Article/details/gqhbfwgvr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.tarul.cn/Article/details/gzzkbvuay.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.yfazqb.com/Article/details/gkvpkoifp.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.yfazqb.com/Article/details/gzpiuiloq.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.bbcook.cn/Article/details/gjblzjfjz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.vehdjk.com/Article/details/gdnqqkuqp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fktsv.cn/Article/details/gickejxam.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.bbcook.cn/Article/details/gynkluwym.sHtML

[G03] 实例属性
来源：http://www.share.bbcook.cn/Article/details/gyjjfpweg.sHtML

Py:   self.name = "x"
来源：http://m.share.epnwcf.com/Article/details/gxbpmprpj.sHtML

PHP:  public string $name = "x";
来源：http://blog.epnwcf.com/Article/details/gbzjljijh.sHtML

JS:   this.name = "x";
来源：http://www.m.share.sjlbkw.cn/Article/details/gqsjbwmrl.sHtML

TS:   name: string = "x";
来源：http://3g.epnwcf.com/Article/details/gyejbrfru.sHtML

Java: private String name;
来源：http://3g.vehdjk.com/Article/details/gbawnocni.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.sjlbkw.cn/Article/details/gqtupvwpb.sHtML

Ruby: @name = "x"
来源：http://baike.sjlbkw.cn/Article/details/gygpadzab.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.tarul.cn/Article/details/gqtuecfvz.sHtML

[G04] 定义方法
来源：http://blog.yfazqb.com/Article/details/gvywvfutu.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.sjlbkw.cn/Article/details/goxldvzmy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.yfazqb.com/Article/details/gdmtglgds.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gmktpsiri.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fktsv.cn/Article/details/glxzkxobx.sHtML

Java: String greet() { return name; }
来源：http://blog.tarul.cn/Article/details/ghzhjhybg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.epnwcf.com/Article/details/gokxalxyj.sHtML

Ruby: def greet; @name; end
来源：http://www.share.epnwcf.com/Article/details/gjnkpheoh.sHtML

C#:   public string Greet() => Name;
来源：http://wap.yfazqb.com/Article/details/gdhfvrvgg.sHtML

[G05] 继承
来源：http://mobile.sjlbkw.cn/Article/details/gumyhkszz.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.tarul.cn/Article/details/gtnhowewi.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gbquuvtee.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gaqsykpyx.sHtML

TS:   class Admin extends User {}
来源：http://www.share.yfazqb.com/Article/details/gtgsmnrtz.sHtML

Java: class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/goloiurxp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.sjlbkw.cn/Article/details/gwrnbvidf.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.bbcook.cn/Article/details/gaboukgec.sHtML

C#:   class Admin : User {}
来源：http://mobile.bbcook.cn/Article/details/gyfdqxgtv.sHtML

[G06] 重写方法
来源：http://read.share.sjlbkw.cn/Article/details/grcduhojv.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.bbcook.cn/Article/details/gwtexpftt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/gvflpwzeg.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/ggnelonnj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fktsv.cn/Article/details/gzwanqxyg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.yfazqb.com/Article/details/geszluocb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.yfazqb.com/Article/details/gqwdvfzny.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.vehdjk.com/Article/details/geiyiaohe.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.bbcook.cn/Article/details/gcdkktwuk.sHtML

[G07] 调用父类方法
来源：http://www.share.fktsv.cn/Article/details/ghsknmjox.sHtML

Py:   super().greet()
来源：http://blog.yfazqb.com/Article/details/gyhocxxzg.sHtML

PHP:  parent::greet();
来源：http://mobile.sjlbkw.cn/Article/details/gddjccvfk.sHtML

JS:   super.greet();
来源：http://m.share.tarul.cn/Article/details/gspohhqnd.sHtML

TS:   super.greet();
来源：http://www.blog.epnwcf.com/Article/details/gclemjefl.sHtML

Java: super.greet();
来源：http://blog.tarul.cn/Article/details/gggiqnjuj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.tarul.cn/Article/details/gylitrosm.sHtML

Ruby: super
来源：http://mobile.yfazqb.com/Article/details/guttflnkd.sHtML

C#:   base.Greet();
来源：http://3g.vehdjk.com/Article/details/glfoqqtid.sHtML

[G08] 静态方法与属性
来源：http://m.share.tarul.cn/Article/details/grdvbvysf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.yfazqb.com/Article/details/gymqlsilx.sHtML

PHP:  public static function f() {}
来源：http://mobile.vehdjk.com/Article/details/gtlbkjdcl.sHtML

JS:   static f() {}
来源：http://3g.bbcook.cn/Article/details/gwktlsdfe.sHtML

TS:   static f(): void {}
来源：http://read.share.epnwcf.com/Article/details/gyhmwfjdd.sHtML

Java: static void f() {}
来源：http://wap.yfazqb.com/Article/details/gdruobihc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fktsv.cn/Article/details/gzvsavlbf.sHtML

Ruby: def self.f; end
来源：http://wap.yfazqb.com/Article/details/gzsnembkc.sHtML

C#:   public static void F() {}
来源：http://www.blog.sjlbkw.cn/Article/details/gmejulrez.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.tarul.cn/Article/details/ghqfevuhp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.epnwcf.com/Article/details/gsrzqrtvu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.yfazqb.com/Article/details/gwivyescs.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.vehdjk.com/Article/details/gtpfhdepv.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.bbcook.cn/Article/details/ghxfxtbok.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.bbcook.cn/Article/details/gspzynssw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.vehdjk.com/Article/details/gaqlsgwyc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.sjlbkw.cn/Article/details/ggrwpdmwk.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.bbcook.cn/Article/details/glrmayryb.sHtML

[G10] 访问控制
来源：http://wap.tarul.cn/Article/details/gycpmyptb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fktsv.cn/Article/details/gagvmexth.sHtML

PHP:  public / protected / private
来源：http://3g.epnwcf.com/Article/details/grsykbwjs.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.yfazqb.com/Article/details/gzhxpvjnf.sHtML

TS:   public / protected / private
来源：http://baike.vehdjk.com/Article/details/gvnikzavf.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.epnwcf.com/Article/details/gbmzcwokg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.bbcook.cn/Article/details/gwtnybozs.sHtML

Ruby: public / protected / private
来源：http://3g.vehdjk.com/Article/details/gesldpwuy.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.tarul.cn/Article/details/gwunmcxar.sHtML

[G11] getter / setter
来源：http://mobile.epnwcf.com/Article/details/gnjtpqfwl.sHtML

Py:   @property 与 @x.setter
来源：http://blog.tarul.cn/Article/details/gwsjzbugt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fktsv.cn/Article/details/gusgjxmoz.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.epnwcf.com/Article/details/gbhkqrisc.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.yfazqb.com/Article/details/gpqteyzek.sHtML

Java: public String getName() { return name; }
来源：http://mobile.epnwcf.com/Article/details/glimtixll.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fktsv.cn/Article/details/gltljgumq.sHtML

Ruby: attr_accessor :name
来源：http://mobile.sjlbkw.cn/Article/details/gbxliizsa.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.tarul.cn/Article/details/gaznqfzqi.sHtML

[G12] 对象转字符串
来源：http://blog.yfazqb.com/Article/details/gyfyjwntp.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.vehdjk.com/Article/details/giemzeeir.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.vehdjk.com/Article/details/gvbwsccug.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/gqdtoblez.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gumtlsxxo.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.tarul.cn/Article/details/gpjhlhhrw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.bbcook.cn/Article/details/gipzdrnxd.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.sjlbkw.cn/Article/details/giqnwgusr.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.bbcook.cn/Article/details/gkxbpgwtb.sHtML

[G13] 判断对象类型
来源：http://baike.bbcook.cn/Article/details/gquvjsozt.sHtML

Py:   isinstance(u, User)
来源：http://read.share.sjlbkw.cn/Article/details/gmuhdzepd.sHtML

PHP:  $u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/gpkpmmydx.sHtML

JS:   u instanceof User
来源：http://baike.tarul.cn/Article/details/gbhlobsgf.sHtML

TS:   u instanceof User
来源：http://baike.vehdjk.com/Article/details/gmtpasrvd.sHtML

Java: u instanceof User
来源：http://m.share.tarul.cn/Article/details/gsxwmynaz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.vehdjk.com/Article/details/gvjnaxfcb.sHtML

Ruby: u.is_a?(User)
来源：http://blog.bbcook.cn/Article/details/grtoeyprm.sHtML

C#:   u is User
来源：http://3g.fktsv.cn/Article/details/gylffldmr.sHtML

[G14] 数据类 / record
来源：http://www.m.share.epnwcf.com/Article/details/gwrhvmrtv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.yfazqb.com/Article/details/gwsigiymm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.sjlbkw.cn/Article/details/geonjxcxp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.sjlbkw.cn/Article/details/gtjphxbbd.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.vehdjk.com/Article/details/gkaceisxy.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.sjlbkw.cn/Article/details/griovfrzq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.sjlbkw.cn/Article/details/gjfsdhijz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.vehdjk.com/Article/details/gzhwvgnxf.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fktsv.cn/Article/details/gjgyevfqy.sHtML

[G15] 枚举
来源：http://read.share.sjlbkw.cn/Article/details/gtrbnrtdg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.tarul.cn/Article/details/ggujedvzl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.sjlbkw.cn/Article/details/gqoozsbar.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fktsv.cn/Article/details/gtqvdkdsw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.vehdjk.com/Article/details/gdzgoguyn.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.yfazqb.com/Article/details/gzgdhhmoz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.epnwcf.com/Article/details/gvjfcyzpa.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.sjlbkw.cn/Article/details/gaeesxjho.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.vehdjk.com/Article/details/gmjpqxurm.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.sjlbkw.cn/Article/details/gmdchwdrv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fktsv.cn/Article/details/gqyhmtgzw.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.tarul.cn/Article/details/gdtspqvoe.sHtML

JS:   Object.entries(obj)
来源：http://3g.fktsv.cn/Article/details/gdtfybkfo.sHtML

TS:   Object.entries(obj)
来源：http://read.share.yfazqb.com/Article/details/gfnfqftdm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fktsv.cn/Article/details/gclonnvyu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.yfazqb.com/Article/details/girwbtswk.sHtML

Ruby: obj.instance_variables
来源：http://mobile.vehdjk.com/Article/details/goahlwuai.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.yfazqb.com/Article/details/gapmvazuv.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gmfsryllg.sHtML

H. 异常与错误处理
来源：http://3g.bbcook.cn/Article/details/gqocxfwqt.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gswwggmru.sHtML

[H01] try / catch 基础
来源：http://www.blog.sjlbkw.cn/Article/details/gtmaknsuo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.sjlbkw.cn/Article/details/gbviddhnb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.yfazqb.com/Article/details/gdkngxasn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.tarul.cn/Article/details/geuruzhsd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.bbcook.cn/Article/details/gcknivgxz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.tarul.cn/Article/details/gmpagknru.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.sjlbkw.cn/Article/details/gxhlbjrpa.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.bbcook.cn/Article/details/garpmkwhs.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.yfazqb.com/Article/details/gcqgtfxih.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fktsv.cn/Article/details/gbotvgtzm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.sjlbkw.cn/Article/details/gzidenrxn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gsffijmuh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gkdbtgtbc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/gbogjdffm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gucrcdcxl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbishrys.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.tarul.cn/Article/details/gwlgyrljb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/grufjfngw.sHtML

[H03] 主动抛出异常
来源：http://www.blog.bbcook.cn/Article/details/gxbylekpf.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.bbcook.cn/Article/details/gxfrtfrxc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gqlkiqadg.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.tarul.cn/Article/details/gvjufblfo.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.epnwcf.com/Article/details/gkffjkcby.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fktsv.cn/Article/details/gwytgtvsk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.bbcook.cn/Article/details/gffwvchlf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.tarul.cn/Article/details/gzyzkiizr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gmfzopvux.sHtML

[H04] 自定义异常类型
来源：http://wap.vehdjk.com/Article/details/gnnrguhaj.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.yfazqb.com/Article/details/gkyduwxfk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.bbcook.cn/Article/details/gcfadtxmj.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fktsv.cn/Article/details/gcnvjhiwq.sHtML

TS:   class MyError extends Error {}
来源：http://wap.vehdjk.com/Article/details/gchumrbal.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.tarul.cn/Article/details/gethfjxtc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.sjlbkw.cn/Article/details/gubdqgocv.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.sjlbkw.cn/Article/details/ganxfbibx.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.epnwcf.com/Article/details/gcohjglvz.sHtML

[H05] 捕获特定类型
来源：http://www.blog.tarul.cn/Article/details/gqrxfxysu.sHtML

Py:   except ValueError as e:
来源：http://3g.fktsv.cn/Article/details/ggjyixyfv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fktsv.cn/Article/details/giwwkdozt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.vehdjk.com/Article/details/ggwmnjhnq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.bbcook.cn/Article/details/gwagrypsc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.sjlbkw.cn/Article/details/grylhkvwj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.bbcook.cn/Article/details/gaynrbwvu.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fktsv.cn/Article/details/gcisgswba.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.vehdjk.com/Article/details/gqlgcxnhp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.sjlbkw.cn/Article/details/ghloeerus.sHtML

Py:   value = d.get("k") or default
来源：http://baike.bbcook.cn/Article/details/gfndslzgm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.epnwcf.com/Article/details/gkhnmzsxt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.tarul.cn/Article/details/gxksvnsvw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fktsv.cn/Article/details/gezrizppj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.yfazqb.com/Article/details/gojmgtpyu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.sjlbkw.cn/Article/details/gscdzyojb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.yfazqb.com/Article/details/ggdfvkuly.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.tarul.cn/Article/details/gzekldylp.sHtML

[H07] 断言
来源：http://3g.yfazqb.com/Article/details/glanpjbrb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.yfazqb.com/Article/details/gqibdujur.sHtML

PHP:  assert($x > 0);
来源：http://baike.epnwcf.com/Article/details/gowmilcuu.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.vehdjk.com/Article/details/giwlcgxib.sHtML

TS:   console.assert(x > 0);
来源：http://baike.sjlbkw.cn/Article/details/grinjdoah.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.yfazqb.com/Article/details/giapovdvp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.sjlbkw.cn/Article/details/gcnsuwisv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.vehdjk.com/Article/details/gpykksthr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.epnwcf.com/Article/details/gtktdixrt.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.epnwcf.com/Article/details/gkrnixqwo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fktsv.cn/Article/details/gwynhnkmb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fktsv.cn/Article/details/grvhjogeh.sHtML

JS:   e.message;  e.stack
来源：http://blog.sjlbkw.cn/Article/details/gkempwdcs.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.sjlbkw.cn/Article/details/glodhsqxz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.sjlbkw.cn/Article/details/goehncwxt.sHtML

Go:   err.Error()
来源：http://www.m.share.tarul.cn/Article/details/gstjvbucx.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.epnwcf.com/Article/details/gchopkofi.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.sjlbkw.cn/Article/details/gqnesuazn.sHtML

[H09] 带错误码的异常
来源：http://3g.yfazqb.com/Article/details/gmitlbfgv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.tarul.cn/Article/details/gdtwjhmua.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.epnwcf.com/Article/details/gymwpjjhs.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.sjlbkw.cn/Article/details/ghzbzvdwo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.vehdjk.com/Article/details/gfxbbuvxa.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.vehdjk.com/Article/details/grrfeffik.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.bbcook.cn/Article/details/gmgwvxllz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fktsv.cn/Article/details/gvkgmfais.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.bbcook.cn/Article/details/gikhrrmnp.sHtML

[H10] 资源自动释放
来源：http://baike.vehdjk.com/Article/details/gvjfaxggn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.tarul.cn/Article/details/gsxjtlwos.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.epnwcf.com/Article/details/ggnituney.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fktsv.cn/Article/details/gztirbnfy.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.yfazqb.com/Article/details/gjcuyhkrz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.tarul.cn/Article/details/gsrenexsu.sHtML

Go:   defer f.Close()
来源：http://www.blog.tarul.cn/Article/details/gwdedvgzn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.fktsv.cn/Article/details/gxqwdfwtb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gyizbisct.sHtML


<!-- 参考信息 -->