代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.epnwcf.com/Article/details/gcljhcoew.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.epnwcf.com/Article/details/glupanyjk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.vehdjk.com/Article/details/gojoemyqt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fktsv.cn/Article/details/glgkoieza.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjrnjhhle.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.vehdjk.com/Article/details/gevabfwdc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.yfazqb.com/Article/details/gsjalfnus.sHtML

[F08] 遍历目录
来源：http://3g.sjlbkw.cn/Article/details/gmktnndtx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.tarul.cn/Article/details/gpazwkhbt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.sjlbkw.cn/Article/details/gsaolozuk.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.bbcook.cn/Article/details/gpinowsmy.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.tarul.cn/Article/details/gvbmyhaci.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.vehdjk.com/Article/details/gpqfswait.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.yfazqb.com/Article/details/gyigfqasc.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.epnwcf.com/Article/details/gtpidhkje.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fktsv.cn/Article/details/gukyiomdi.sHtML

[F09] 获取文件大小
来源：http://mobile.bbcook.cn/Article/details/gwwqstznp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.bbcook.cn/Article/details/gxdqlrqja.sHtML

PHP:  filesize("a.txt");
来源：http://baike.tarul.cn/Article/details/grdzadfmo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.yfazqb.com/Article/details/gwnlrcbsp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.bbcook.cn/Article/details/gfeqnifuf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.sjlbkw.cn/Article/details/gpsdplick.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.vehdjk.com/Article/details/gbxorfepx.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gyndalumz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.yfazqb.com/Article/details/gdzzhfegc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.epnwcf.com/Article/details/gpgjyskrn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.tarul.cn/Article/details/gwmsvvhye.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.yfazqb.com/Article/details/ggizshttf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gdklikmqw.sHtML

TS:   path.extname("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/groaknuth.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fktsv.cn/Article/details/gteoowiow.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gpthhgvey.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/ggvzphzvo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/ggzclxjci.sHtML

[F11] 复制与移动文件
来源：http://www.blog.yfazqb.com/Article/details/gsherqnvy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/ggrilykyc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fktsv.cn/Article/details/golzkibsx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/gfqmxvbma.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/ggtcvzzdy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.epnwcf.com/Article/details/gbsspjqpc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.sjlbkw.cn/Article/details/gjnjxoysg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gbfgiedmj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.vehdjk.com/Article/details/gbyqjaleb.sHtML

[F12] CSV 读写
来源：http://baike.fktsv.cn/Article/details/gurjxxpwk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.sjlbkw.cn/Article/details/gagypvkpj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.tarul.cn/Article/details/gpsbfcdgg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.epnwcf.com/Article/details/gimupevwb.sHtML

TS:   // 同上
来源：http://www.share.bbcook.cn/Article/details/gzzevusnt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fktsv.cn/Article/details/gniktgvnz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.sjlbkw.cn/Article/details/gieqcicwu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.epnwcf.com/Article/details/gyjjutuaf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.vehdjk.com/Article/details/gmatcqwbv.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gerhxdbfb.sHtML

G. 面向对象
来源：http://mobile.vehdjk.com/Article/details/grurvjnfv.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gyzaxxnfu.sHtML

[G01] 定义类
来源：http://baike.vehdjk.com/Article/details/gqrnlvdye.sHtML

Py:   class User: pass
来源：http://3g.yfazqb.com/Article/details/gyboxogjm.sHtML

PHP:  class User {}
来源：http://wap.yfazqb.com/Article/details/goivdxkfi.sHtML

JS:   class User {}
来源：http://read.share.yfazqb.com/Article/details/gpcmtqugk.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.yfazqb.com/Article/details/gcadrxfuv.sHtML

Java: class User {}
来源：http://3g.tarul.cn/Article/details/gtkijekaf.sHtML

Go:   type User struct { Name string }
来源：http://www.share.bbcook.cn/Article/details/gbowyayxd.sHtML

Ruby: class User; end
来源：http://www.share.vehdjk.com/Article/details/gjumzbuyr.sHtML

C#:   class User {}
来源：http://m.share.sjlbkw.cn/Article/details/goofholyc.sHtML

[G02] 构造函数
来源：http://m.share.yfazqb.com/Article/details/ghkzijljf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.epnwcf.com/Article/details/gmythoncu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fktsv.cn/Article/details/ggpgvurjm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.vehdjk.com/Article/details/ghtelwxbu.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.epnwcf.com/Article/details/gtmgfhvwx.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.epnwcf.com/Article/details/gqqtptubt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.bbcook.cn/Article/details/gtjarkxul.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.yfazqb.com/Article/details/gavksnrys.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.bbcook.cn/Article/details/gjizelacp.sHtML

[G03] 实例属性
来源：http://3g.tarul.cn/Article/details/gqzhyxcdw.sHtML

Py:   self.name = "x"
来源：http://m.share.bbcook.cn/Article/details/gufcycdnd.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.epnwcf.com/Article/details/giyrxosli.sHtML

JS:   this.name = "x";
来源：http://www.blog.fktsv.cn/Article/details/gtpyraqfq.sHtML

TS:   name: string = "x";
来源：http://blog.yfazqb.com/Article/details/gimmmldms.sHtML

Java: private String name;
来源：http://www.blog.sjlbkw.cn/Article/details/gkoufjkga.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fktsv.cn/Article/details/grnnonmym.sHtML

Ruby: @name = "x"
来源：http://blog.yfazqb.com/Article/details/gcjqiuvzn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fktsv.cn/Article/details/gbpumcpyc.sHtML

[G04] 定义方法
来源：http://3g.sjlbkw.cn/Article/details/gvtnihfji.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.bbcook.cn/Article/details/ghtbnmzts.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fktsv.cn/Article/details/gwplyankl.sHtML

JS:   greet() { return this.name; }
来源：http://wap.tarul.cn/Article/details/gcxclheei.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.bbcook.cn/Article/details/gzcmdzlmp.sHtML

Java: String greet() { return name; }
来源：http://3g.vehdjk.com/Article/details/gombiniyv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.epnwcf.com/Article/details/gasuwbmxw.sHtML

Ruby: def greet; @name; end
来源：http://mobile.sjlbkw.cn/Article/details/gqhiqcyfm.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.tarul.cn/Article/details/gnwrkmkqn.sHtML

[G05] 继承
来源：http://wap.tarul.cn/Article/details/gkfcjewml.sHtML

Py:   class Admin(User): pass
来源：http://m.share.sjlbkw.cn/Article/details/gzpnkdsbp.sHtML

PHP:  class Admin extends User {}
来源：http://wap.bbcook.cn/Article/details/gbvevyufv.sHtML

JS:   class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/guydypkbf.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/gqxgvlvhb.sHtML

Java: class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/gyraozamc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.vehdjk.com/Article/details/gtqmtilgn.sHtML

Ruby: class Admin < User; end
来源：http://blog.sjlbkw.cn/Article/details/gfyjrkmzc.sHtML

C#:   class Admin : User {}
来源：http://3g.fktsv.cn/Article/details/gljkkuujl.sHtML

[G06] 重写方法
来源：http://3g.fktsv.cn/Article/details/gpmxmnoxx.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.epnwcf.com/Article/details/gpqsmrbox.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/ggroxtmoo.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/glcvuanqo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/gbpxoqyio.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.tarul.cn/Article/details/gvdtlkfdz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.epnwcf.com/Article/details/gngkynwub.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fktsv.cn/Article/details/gxhxnxols.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fktsv.cn/Article/details/gnsstotsm.sHtML

[G07] 调用父类方法
来源：http://www.blog.bbcook.cn/Article/details/gdurydjvu.sHtML

Py:   super().greet()
来源：http://www.blog.bbcook.cn/Article/details/gouisnrgr.sHtML

PHP:  parent::greet();
来源：http://baike.vehdjk.com/Article/details/gweljhivb.sHtML

JS:   super.greet();
来源：http://baike.tarul.cn/Article/details/gverswfah.sHtML

TS:   super.greet();
来源：http://mobile.fktsv.cn/Article/details/ggqtwluja.sHtML

Java: super.greet();
来源：http://www.blog.epnwcf.com/Article/details/govtxpmkv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.yfazqb.com/Article/details/gvnyazyvw.sHtML

Ruby: super
来源：http://blog.yfazqb.com/Article/details/gagyqqfnr.sHtML

C#:   base.Greet();
来源：http://3g.epnwcf.com/Article/details/gafgusaer.sHtML

[G08] 静态方法与属性
来源：http://3g.fktsv.cn/Article/details/gfydprvxi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.sjlbkw.cn/Article/details/grweqfhvo.sHtML

PHP:  public static function f() {}
来源：http://baike.epnwcf.com/Article/details/gbvdoawmz.sHtML

JS:   static f() {}
来源：http://m.share.fktsv.cn/Article/details/gckxgmaie.sHtML

TS:   static f(): void {}
来源：http://www.blog.bbcook.cn/Article/details/gjauznhdq.sHtML

Java: static void f() {}
来源：http://mobile.vehdjk.com/Article/details/gykkihiej.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.bbcook.cn/Article/details/giigwtqww.sHtML

Ruby: def self.f; end
来源：http://m.share.yfazqb.com/Article/details/groympczd.sHtML

C#:   public static void F() {}
来源：http://mobile.yfazqb.com/Article/details/glepuytlm.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.yfazqb.com/Article/details/gzhzvpdwh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.tarul.cn/Article/details/gnugltzrh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.epnwcf.com/Article/details/ghlqdrgze.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fktsv.cn/Article/details/gkbolqvbz.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.bbcook.cn/Article/details/gpwaenrpv.sHtML

Java: interface Shape { double area(); }
来源：http://wap.tarul.cn/Article/details/grwkbknaq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.tarul.cn/Article/details/gciydnreu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.epnwcf.com/Article/details/gvezqteoh.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.vehdjk.com/Article/details/gofteuigw.sHtML

[G10] 访问控制
来源：http://baike.bbcook.cn/Article/details/gmsigrjgm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fktsv.cn/Article/details/gslumfzyk.sHtML

PHP:  public / protected / private
来源：http://m.share.fktsv.cn/Article/details/gkxzuibrb.sHtML

JS:   #private 字段；其余公开
来源：http://wap.yfazqb.com/Article/details/gpfwjpvnp.sHtML

TS:   public / protected / private
来源：http://www.m.share.vehdjk.com/Article/details/gmsszuydl.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.tarul.cn/Article/details/gbqvlqukp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.vehdjk.com/Article/details/gswxozcyk.sHtML

Ruby: public / protected / private
来源：http://read.share.sjlbkw.cn/Article/details/gtnzdpgip.sHtML

C#:   public / protected / private / internal
来源：http://wap.yfazqb.com/Article/details/giuwzljob.sHtML

[G11] getter / setter
来源：http://baike.bbcook.cn/Article/details/gacjjvqon.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.epnwcf.com/Article/details/gvrevlggc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.yfazqb.com/Article/details/gkhktzpbq.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.vehdjk.com/Article/details/ghcqondvv.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.vehdjk.com/Article/details/gvscgkwsr.sHtML

Java: public String getName() { return name; }
来源：http://wap.vehdjk.com/Article/details/glrxgsfmh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.tarul.cn/Article/details/gtztgwfzk.sHtML

Ruby: attr_accessor :name
来源：http://3g.tarul.cn/Article/details/glyxotyvc.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.vehdjk.com/Article/details/gimumpvnc.sHtML

[G12] 对象转字符串
来源：http://m.share.sjlbkw.cn/Article/details/gutbaolee.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.yfazqb.com/Article/details/gszbaycii.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.yfazqb.com/Article/details/gkjdkaxub.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.vehdjk.com/Article/details/gelqkaiwg.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.epnwcf.com/Article/details/gebwehcju.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.tarul.cn/Article/details/gfsxlrtmc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.yfazqb.com/Article/details/gmssgpjgi.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.epnwcf.com/Article/details/ghhmpyqej.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.epnwcf.com/Article/details/gozzvigsj.sHtML

[G13] 判断对象类型
来源：http://www.share.fktsv.cn/Article/details/gddrdeqfo.sHtML

Py:   isinstance(u, User)
来源：http://m.share.bbcook.cn/Article/details/gdfsudrhz.sHtML

PHP:  $u instanceof User
来源：http://baike.bbcook.cn/Article/details/gxadrvuaj.sHtML

JS:   u instanceof User
来源：http://m.share.tarul.cn/Article/details/gjjnishtm.sHtML

TS:   u instanceof User
来源：http://wap.yfazqb.com/Article/details/gtczyqlte.sHtML

Java: u instanceof User
来源：http://baike.epnwcf.com/Article/details/gzwhdiqxo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.yfazqb.com/Article/details/gqjdtgklu.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fktsv.cn/Article/details/gjqookrfk.sHtML

C#:   u is User
来源：http://blog.epnwcf.com/Article/details/gcpriyzfb.sHtML

[G14] 数据类 / record
来源：http://www.share.vehdjk.com/Article/details/gajgkwswd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.tarul.cn/Article/details/gahdxujtl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.yfazqb.com/Article/details/gjnsaaxxx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.sjlbkw.cn/Article/details/ghvvjvqgz.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.epnwcf.com/Article/details/gtxdevabx.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.vehdjk.com/Article/details/gxgmgfhkn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fktsv.cn/Article/details/gzemuxqed.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fktsv.cn/Article/details/gzjjuhkkk.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.bbcook.cn/Article/details/gsznmzbrk.sHtML

[G15] 枚举
来源：http://m.share.bbcook.cn/Article/details/gdbxuxjwu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.sjlbkw.cn/Article/details/glwvepmza.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.epnwcf.com/Article/details/gdodyhonm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.bbcook.cn/Article/details/gcwwnqqxr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.epnwcf.com/Article/details/gtfxyojuu.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.yfazqb.com/Article/details/gpvnpasig.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.bbcook.cn/Article/details/gnkyzlxxx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.bbcook.cn/Article/details/gtipzlfxr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.vehdjk.com/Article/details/gtvivebdn.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fktsv.cn/Article/details/grpdrvqyn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.vehdjk.com/Article/details/gxxjjuzyg.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.bbcook.cn/Article/details/gfstnwuux.sHtML

JS:   Object.entries(obj)
来源：http://wap.epnwcf.com/Article/details/gzlcatdcc.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fktsv.cn/Article/details/gqwbcxhyu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fktsv.cn/Article/details/gyjcovcpd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fktsv.cn/Article/details/gtjubztun.sHtML

Ruby: obj.instance_variables
来源：http://www.share.vehdjk.com/Article/details/gimywbogn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.vehdjk.com/Article/details/gxnsosatc.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gvqzoletf.sHtML

H. 异常与错误处理
来源：http://m.share.fktsv.cn/Article/details/guaoaiaig.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gbkaaohde.sHtML

[H01] try / catch 基础
来源：http://www.blog.vehdjk.com/Article/details/gmwhxyziv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.bbcook.cn/Article/details/gzrmgeojc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.bbcook.cn/Article/details/gtskkqrjy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.bbcook.cn/Article/details/gegupnebb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.sjlbkw.cn/Article/details/ggugxehjk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.vehdjk.com/Article/details/grwfsmvts.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.yfazqb.com/Article/details/ghekzvkpb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.sjlbkw.cn/Article/details/givxyeooz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.bbcook.cn/Article/details/gptzhyqqa.sHtML

[H02] finally / ensure 收尾
来源：http://baike.sjlbkw.cn/Article/details/gwgfxyfxp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fktsv.cn/Article/details/gckiaorcf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/ghykhjyyh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gklqcgdco.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gzduqhfbi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/goreggioh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.vehdjk.com/Article/details/guwkrljaf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.tarul.cn/Article/details/gccisotxs.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gvtqwgmxk.sHtML

[H03] 主动抛出异常
来源：http://wap.vehdjk.com/Article/details/gabonrrfn.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.tarul.cn/Article/details/gechcmgxz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fktsv.cn/Article/details/grpelkghs.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.vehdjk.com/Article/details/gknaytuft.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fktsv.cn/Article/details/gfwbmacdh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.yfazqb.com/Article/details/glzeaoukw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fktsv.cn/Article/details/gnrojxhej.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.bbcook.cn/Article/details/ggovjsvun.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fktsv.cn/Article/details/gdktqrvhr.sHtML

[H04] 自定义异常类型
来源：http://m.share.yfazqb.com/Article/details/gqdbxiwms.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.vehdjk.com/Article/details/gqzsqyepb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fktsv.cn/Article/details/gyjbogqvw.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.tarul.cn/Article/details/gbpztrtzx.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.vehdjk.com/Article/details/gckivncqf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.vehdjk.com/Article/details/ggepvnaey.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.yfazqb.com/Article/details/gijqhqxlz.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fktsv.cn/Article/details/grmfyvqbt.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.sjlbkw.cn/Article/details/gjaogehiw.sHtML

[H05] 捕获特定类型
来源：http://wap.bbcook.cn/Article/details/gesqljdto.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.yfazqb.com/Article/details/gzovocjet.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fktsv.cn/Article/details/gckzwdozk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.tarul.cn/Article/details/gsjhyncha.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.bbcook.cn/Article/details/gzopmvsug.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.sjlbkw.cn/Article/details/ggfeelxej.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fktsv.cn/Article/details/gmodxgisf.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fktsv.cn/Article/details/grzkpjbcc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.epnwcf.com/Article/details/gfsbyqruq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.sjlbkw.cn/Article/details/gqqjqpgdk.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fktsv.cn/Article/details/gviotsaer.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.epnwcf.com/Article/details/gctbqeqzz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.tarul.cn/Article/details/gfvjwyevg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.epnwcf.com/Article/details/gadljukve.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.tarul.cn/Article/details/gmlwnzaaf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.vehdjk.com/Article/details/ghkkatqnd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fktsv.cn/Article/details/gxlpazook.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fktsv.cn/Article/details/gwbftjfdg.sHtML

[H07] 断言
来源：http://mobile.vehdjk.com/Article/details/guwlkttlz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.epnwcf.com/Article/details/grdcoggxw.sHtML

PHP:  assert($x > 0);
来源：http://baike.fktsv.cn/Article/details/gdoplawtr.sHtML

JS:   console.assert(x > 0);
来源：http://3g.sjlbkw.cn/Article/details/gxjodtzeg.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.sjlbkw.cn/Article/details/gdflptnep.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.yfazqb.com/Article/details/gyruynath.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.vehdjk.com/Article/details/gwzftjoxo.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.sjlbkw.cn/Article/details/ghvjriuia.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.bbcook.cn/Article/details/gkkejgwve.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.vehdjk.com/Article/details/gjmdiilid.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.vehdjk.com/Article/details/gmzvptmnx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.bbcook.cn/Article/details/gbyhirnad.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.vehdjk.com/Article/details/gdqcklqxn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.vehdjk.com/Article/details/gmpugvhds.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.epnwcf.com/Article/details/gpyoustqk.sHtML

Go:   err.Error()
来源：http://blog.tarul.cn/Article/details/gqzgsxxnp.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.sjlbkw.cn/Article/details/gliqlraek.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.bbcook.cn/Article/details/galpqgbui.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fktsv.cn/Article/details/gymscgfdc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.sjlbkw.cn/Article/details/gcanhsgsd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.bbcook.cn/Article/details/gmquruilo.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.bbcook.cn/Article/details/galdezdux.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fktsv.cn/Article/details/gnaazyiof.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.bbcook.cn/Article/details/ghypwwuqr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.vehdjk.com/Article/details/gvxpxdmyy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.epnwcf.com/Article/details/gfcijgdlz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.epnwcf.com/Article/details/gtfbnquvz.sHtML

[H10] 资源自动释放
来源：http://read.share.epnwcf.com/Article/details/gswpufhby.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.yfazqb.com/Article/details/gdwolsjzq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.bbcook.cn/Article/details/gdwrvprpc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.tarul.cn/Article/details/ginosoupc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.tarul.cn/Article/details/gwscsjqgq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.sjlbkw.cn/Article/details/gvywkdjkm.sHtML

Go:   defer f.Close()
来源：http://blog.bbcook.cn/Article/details/gnkkcredk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.epnwcf.com/Article/details/gomspcbyo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gjmbrzphz.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gxnxzoggj.sHtML

I. 正则表达式
来源：http://wap.fktsv.cn/Article/details/gaqswnwsd.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gpvpjtcph.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.yfazqb.com/Article/details/gezfurdns.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.sjlbkw.cn/Article/details/gnjayscfn.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.epnwcf.com/Article/details/getcjxdgn.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fktsv.cn/Article/details/gushojooy.sHtML

TS:   /\d+/.test(s)
来源：http://blog.vehdjk.com/Article/details/gtwljoevz.sHtML


<!-- 参考信息 -->