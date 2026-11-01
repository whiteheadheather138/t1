代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.tarul.cn/Article/details/galbhoktz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.tarul.cn/Article/details/gtjtqkcwg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.sjlbkw.cn/Article/details/grttiypie.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.tarul.cn/Article/details/gauoccsuu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.sjlbkw.cn/Article/details/gswgcdsij.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.epnwcf.com/Article/details/gcxiawymt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.vehdjk.com/Article/details/gtmzavxef.sHtML

[F08] 遍历目录
来源：http://blog.bbcook.cn/Article/details/gckyqouuj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.tarul.cn/Article/details/gzztryfcb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fktsv.cn/Article/details/gcvgjdgya.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.epnwcf.com/Article/details/gfyyncvvl.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gprtllyse.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.vehdjk.com/Article/details/gvfxhyzwq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.tarul.cn/Article/details/gxzbbhktu.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghoqcygim.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzgoyeyor.sHtML

[F09] 获取文件大小
来源：http://read.share.epnwcf.com/Article/details/guxzdezwr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gxgmozymf.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gjqydeisc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fktsv.cn/Article/details/gcmpcpvvo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.tarul.cn/Article/details/gffkfdrqy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/gbsjcwfft.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.tarul.cn/Article/details/gqfupwesv.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gduxydyji.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.yfazqb.com/Article/details/gpnkpvdps.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.yfazqb.com/Article/details/gifcwqgnp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/gmauevykv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.vehdjk.com/Article/details/gyaermfcg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/ggbrktzns.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gupqcweoq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.vehdjk.com/Article/details/gimykgbhh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gabnzqtxb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/ggfbkqlvb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gbpqhtzzj.sHtML

[F11] 复制与移动文件
来源：http://wap.yfazqb.com/Article/details/gdawcrxvi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gyctcpfyc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.bbcook.cn/Article/details/gloasbtvm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/gqeycpfxw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/glwuwwmco.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.yfazqb.com/Article/details/gddyuqhvy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.tarul.cn/Article/details/gkjewvboo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/gmyekrncn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.yfazqb.com/Article/details/gufualeid.sHtML

[F12] CSV 读写
来源：http://baike.vehdjk.com/Article/details/ggrvzwxnc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.epnwcf.com/Article/details/gqsssyzdf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fktsv.cn/Article/details/gwrqztwzp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.epnwcf.com/Article/details/gblstlfxj.sHtML

TS:   // 同上
来源：http://blog.tarul.cn/Article/details/ggebzhyxe.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.sjlbkw.cn/Article/details/gasffsgmc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.epnwcf.com/Article/details/gtsfbahrp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.sjlbkw.cn/Article/details/gyiuhzxfs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.yfazqb.com/Article/details/gozowfehy.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gahrwhery.sHtML

G. 面向对象
来源：http://www.share.vehdjk.com/Article/details/gkcijtrty.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gsnitfkpd.sHtML

[G01] 定义类
来源：http://read.share.yfazqb.com/Article/details/gtnlbbnba.sHtML

Py:   class User: pass
来源：http://mobile.epnwcf.com/Article/details/gzjwwefbb.sHtML

PHP:  class User {}
来源：http://m.share.vehdjk.com/Article/details/gfxjpbqii.sHtML

JS:   class User {}
来源：http://www.blog.bbcook.cn/Article/details/gnblqkqul.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.yfazqb.com/Article/details/gteyojplr.sHtML

Java: class User {}
来源：http://read.share.vehdjk.com/Article/details/gcvrvqmph.sHtML

Go:   type User struct { Name string }
来源：http://3g.yfazqb.com/Article/details/glstmtuso.sHtML

Ruby: class User; end
来源：http://m.share.sjlbkw.cn/Article/details/gayniykga.sHtML

C#:   class User {}
来源：http://baike.vehdjk.com/Article/details/gniolllvc.sHtML

[G02] 构造函数
来源：http://www.m.share.epnwcf.com/Article/details/grnoicjzc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.vehdjk.com/Article/details/gcvrknsei.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.bbcook.cn/Article/details/ghrmacuab.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.yfazqb.com/Article/details/gsykpmamz.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.tarul.cn/Article/details/gwkpwekag.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.vehdjk.com/Article/details/grtpwdean.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.yfazqb.com/Article/details/gfxurqcsw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.sjlbkw.cn/Article/details/gsjonkhoz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.yfazqb.com/Article/details/gulmludox.sHtML

[G03] 实例属性
来源：http://www.blog.yfazqb.com/Article/details/gtbaneyfo.sHtML

Py:   self.name = "x"
来源：http://3g.yfazqb.com/Article/details/gqluntldy.sHtML

PHP:  public string $name = "x";
来源：http://3g.tarul.cn/Article/details/gqrugwkop.sHtML

JS:   this.name = "x";
来源：http://wap.vehdjk.com/Article/details/gowrduspq.sHtML

TS:   name: string = "x";
来源：http://www.m.share.bbcook.cn/Article/details/gloodhscq.sHtML

Java: private String name;
来源：http://m.share.epnwcf.com/Article/details/gaiastonm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fktsv.cn/Article/details/gkwvwnnlk.sHtML

Ruby: @name = "x"
来源：http://3g.tarul.cn/Article/details/gnvjmwfvx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.sjlbkw.cn/Article/details/gockvufnc.sHtML

[G04] 定义方法
来源：http://wap.bbcook.cn/Article/details/ghajlxkao.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fktsv.cn/Article/details/ghgfumjgu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.tarul.cn/Article/details/gvmzfjqmx.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/gvpispaxb.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gepugaopt.sHtML

Java: String greet() { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gnhjadqqj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.yfazqb.com/Article/details/gvtpygery.sHtML

Ruby: def greet; @name; end
来源：http://3g.fktsv.cn/Article/details/gjwtnvihs.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.bbcook.cn/Article/details/gzlfrvvtq.sHtML

[G05] 继承
来源：http://wap.bbcook.cn/Article/details/gxzuraopr.sHtML

Py:   class Admin(User): pass
来源：http://wap.vehdjk.com/Article/details/geunjabql.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gmxtoawts.sHtML

JS:   class Admin extends User {}
来源：http://mobile.sjlbkw.cn/Article/details/gwpdysspd.sHtML

TS:   class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/gecgaadbh.sHtML

Java: class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gtnsmbtii.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fktsv.cn/Article/details/grdublbrw.sHtML

Ruby: class Admin < User; end
来源：http://mobile.vehdjk.com/Article/details/gqiiyxkqv.sHtML

C#:   class Admin : User {}
来源：http://read.share.sjlbkw.cn/Article/details/gbsimixdm.sHtML

[G06] 重写方法
来源：http://blog.tarul.cn/Article/details/gacdndbwn.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.bbcook.cn/Article/details/ghhywlfqu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gibmmswwu.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gayqfoizk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/gussipymz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.tarul.cn/Article/details/gosztvqmu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.epnwcf.com/Article/details/gkwnrzwqd.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gmongllza.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.bbcook.cn/Article/details/gjtvijour.sHtML

[G07] 调用父类方法
来源：http://3g.yfazqb.com/Article/details/gbjogbxlf.sHtML

Py:   super().greet()
来源：http://wap.epnwcf.com/Article/details/gbcrqrcns.sHtML

PHP:  parent::greet();
来源：http://baike.yfazqb.com/Article/details/gyhacgslo.sHtML

JS:   super.greet();
来源：http://blog.bbcook.cn/Article/details/gopusatyp.sHtML

TS:   super.greet();
来源：http://www.share.tarul.cn/Article/details/godazudie.sHtML

Java: super.greet();
来源：http://baike.bbcook.cn/Article/details/gsnffiabe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.bbcook.cn/Article/details/gezpwkaob.sHtML

Ruby: super
来源：http://m.share.tarul.cn/Article/details/gofxitrld.sHtML

C#:   base.Greet();
来源：http://read.share.sjlbkw.cn/Article/details/gemridqve.sHtML

[G08] 静态方法与属性
来源：http://m.share.vehdjk.com/Article/details/ghyadiwpq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.epnwcf.com/Article/details/gxqifzjho.sHtML

PHP:  public static function f() {}
来源：http://www.share.tarul.cn/Article/details/goyzxtrjn.sHtML

JS:   static f() {}
来源：http://www.blog.epnwcf.com/Article/details/guilmgfws.sHtML

TS:   static f(): void {}
来源：http://wap.tarul.cn/Article/details/gaudmrtes.sHtML

Java: static void f() {}
来源：http://read.share.yfazqb.com/Article/details/gmdpindre.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.sjlbkw.cn/Article/details/gwkqifqvx.sHtML

Ruby: def self.f; end
来源：http://www.blog.fktsv.cn/Article/details/gzrngvdrk.sHtML

C#:   public static void F() {}
来源：http://m.share.vehdjk.com/Article/details/gqewsyorq.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.bbcook.cn/Article/details/gduwyffpr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.vehdjk.com/Article/details/ggdobrsfv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.sjlbkw.cn/Article/details/gkjuwqnqb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.tarul.cn/Article/details/gmqdaajjd.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.epnwcf.com/Article/details/gocxrtfwz.sHtML

Java: interface Shape { double area(); }
来源：http://blog.tarul.cn/Article/details/gflrkojut.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.tarul.cn/Article/details/goegudrcv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fktsv.cn/Article/details/gylrdyyfl.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.vehdjk.com/Article/details/ghshhkvgm.sHtML

[G10] 访问控制
来源：http://wap.bbcook.cn/Article/details/gzopbbauf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.yfazqb.com/Article/details/gkeyfkuuk.sHtML

PHP:  public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/gywwwrfis.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fktsv.cn/Article/details/gqdsikwhg.sHtML

TS:   public / protected / private
来源：http://blog.epnwcf.com/Article/details/gpxbnjtif.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.sjlbkw.cn/Article/details/gossysvgi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.bbcook.cn/Article/details/gnjbrpqgo.sHtML

Ruby: public / protected / private
来源：http://baike.yfazqb.com/Article/details/gbmurshim.sHtML

C#:   public / protected / private / internal
来源：http://m.share.sjlbkw.cn/Article/details/gpcowwvlk.sHtML

[G11] getter / setter
来源：http://www.m.share.sjlbkw.cn/Article/details/gclxrljxi.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.yfazqb.com/Article/details/giikrfbbm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.yfazqb.com/Article/details/gefsghqmc.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.epnwcf.com/Article/details/gsnlasnsl.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.yfazqb.com/Article/details/gfndxxceu.sHtML

Java: public String getName() { return name; }
来源：http://3g.tarul.cn/Article/details/gjpufzbfa.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.tarul.cn/Article/details/gmuyaegmy.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.sjlbkw.cn/Article/details/grorwagzr.sHtML

C#:   public string Name { get; set; }
来源：http://wap.bbcook.cn/Article/details/gjsucdtwc.sHtML

[G12] 对象转字符串
来源：http://www.share.yfazqb.com/Article/details/gydprtxyn.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.epnwcf.com/Article/details/gpucivyze.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.sjlbkw.cn/Article/details/gezdmbnqj.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/gurtvuhnq.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/gnbfnxrxy.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.vehdjk.com/Article/details/gkmgnslko.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.bbcook.cn/Article/details/gasqmgpdk.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fktsv.cn/Article/details/grjfamvnv.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.sjlbkw.cn/Article/details/gzuilnpfg.sHtML

[G13] 判断对象类型
来源：http://www.m.share.bbcook.cn/Article/details/gickwjfie.sHtML

Py:   isinstance(u, User)
来源：http://read.share.epnwcf.com/Article/details/gxizsxkni.sHtML

PHP:  $u instanceof User
来源：http://read.share.epnwcf.com/Article/details/gzrgkgryd.sHtML

JS:   u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/gzbqzcsxj.sHtML

TS:   u instanceof User
来源：http://read.share.vehdjk.com/Article/details/gfvxjqfzw.sHtML

Java: u instanceof User
来源：http://www.m.share.tarul.cn/Article/details/gonpqenmr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.epnwcf.com/Article/details/gbatcvfnz.sHtML

Ruby: u.is_a?(User)
来源：http://3g.vehdjk.com/Article/details/gxytktxte.sHtML

C#:   u is User
来源：http://blog.sjlbkw.cn/Article/details/gigfsmvax.sHtML

[G14] 数据类 / record
来源：http://blog.tarul.cn/Article/details/gqalwsman.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fktsv.cn/Article/details/ggxesrfij.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.yfazqb.com/Article/details/gjplntyjz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.bbcook.cn/Article/details/gklbamtyx.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.tarul.cn/Article/details/gzxluoffk.sHtML

Java: record User(String name, int age) {}
来源：http://blog.yfazqb.com/Article/details/gfyrufdzq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.yfazqb.com/Article/details/gyitacfex.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.yfazqb.com/Article/details/gzhcaxgkg.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.sjlbkw.cn/Article/details/gknhaivvb.sHtML

[G15] 枚举
来源：http://3g.sjlbkw.cn/Article/details/gugdafvgf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.yfazqb.com/Article/details/gjfqnlljq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.yfazqb.com/Article/details/gimvoubxh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.yfazqb.com/Article/details/giaqpvfjy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gykczhctc.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.tarul.cn/Article/details/ghhextsrl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.yfazqb.com/Article/details/grjpzhpyc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fktsv.cn/Article/details/guaoynrjf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fktsv.cn/Article/details/gygxvqkdy.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.epnwcf.com/Article/details/gsuivbbke.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.yfazqb.com/Article/details/gwswfqtso.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.bbcook.cn/Article/details/groyfscqz.sHtML

JS:   Object.entries(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gmamhhxxa.sHtML

TS:   Object.entries(obj)
来源：http://m.share.bbcook.cn/Article/details/gwtiszhta.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.yfazqb.com/Article/details/ggeznjtun.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.tarul.cn/Article/details/grksdxvqv.sHtML

Ruby: obj.instance_variables
来源：http://mobile.yfazqb.com/Article/details/gifygbaru.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fktsv.cn/Article/details/grqmgeaqk.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gvolwoyun.sHtML

H. 异常与错误处理
来源：http://read.share.fktsv.cn/Article/details/gmupatowh.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gqbyveacj.sHtML

[H01] try / catch 基础
来源：http://www.blog.vehdjk.com/Article/details/giictbrop.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.vehdjk.com/Article/details/gplcpzxpv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.bbcook.cn/Article/details/gywoncfue.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.yfazqb.com/Article/details/gknondocc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.bbcook.cn/Article/details/ggeutgyxr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fktsv.cn/Article/details/gzhfgfvtz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fktsv.cn/Article/details/gcmjitwyx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.yfazqb.com/Article/details/gqxjozjhq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.yfazqb.com/Article/details/gwdspqfgj.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fktsv.cn/Article/details/gbcnbwffe.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.epnwcf.com/Article/details/ggplootra.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/guquftrop.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/graavwupq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvtrhyebt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/gepdilyyz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.vehdjk.com/Article/details/guxzoysiv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fktsv.cn/Article/details/gmzthchso.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gbfvikwdi.sHtML

[H03] 主动抛出异常
来源：http://read.share.sjlbkw.cn/Article/details/gzmotiski.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.bbcook.cn/Article/details/goipymhqv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.tarul.cn/Article/details/gylmxaygj.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/ghscavkyo.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gganclann.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.tarul.cn/Article/details/gxmhwqzie.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fktsv.cn/Article/details/gqdhgmmqx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.tarul.cn/Article/details/gxollvlwl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.bbcook.cn/Article/details/gojlreoul.sHtML

[H04] 自定义异常类型
来源：http://www.share.tarul.cn/Article/details/gaqogncng.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fktsv.cn/Article/details/gbiafjihj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fktsv.cn/Article/details/gagethmtl.sHtML

JS:   class MyError extends Error {}
来源：http://wap.sjlbkw.cn/Article/details/gxoxxpykk.sHtML

TS:   class MyError extends Error {}
来源：http://blog.epnwcf.com/Article/details/gtdvytfbv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.sjlbkw.cn/Article/details/geyxukbjt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fktsv.cn/Article/details/gjlftbqox.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.epnwcf.com/Article/details/gdtqlzxpa.sHtML

C#:   class MyException : Exception {}
来源：http://3g.epnwcf.com/Article/details/gglcusqdm.sHtML

[H05] 捕获特定类型
来源：http://baike.yfazqb.com/Article/details/gjkfuhtsj.sHtML

Py:   except ValueError as e:
来源：http://blog.sjlbkw.cn/Article/details/gilknewgz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.yfazqb.com/Article/details/gklafttqh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.tarul.cn/Article/details/gvexfgxvd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.vehdjk.com/Article/details/gdwstxhcp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.epnwcf.com/Article/details/gdkloqzge.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.sjlbkw.cn/Article/details/gkqzodrgb.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.tarul.cn/Article/details/givciktzl.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.bbcook.cn/Article/details/gjrvvtnyc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fktsv.cn/Article/details/gjeopyevq.sHtML

Py:   value = d.get("k") or default
来源：http://3g.epnwcf.com/Article/details/gmlazakdc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.epnwcf.com/Article/details/grgkvsykq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fktsv.cn/Article/details/gkkhmkaac.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.vehdjk.com/Article/details/gjscyfhll.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.vehdjk.com/Article/details/gohhhfzkm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.vehdjk.com/Article/details/gsdqktukp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.bbcook.cn/Article/details/gjjaluwtr.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.bbcook.cn/Article/details/gwlslhqdw.sHtML

[H07] 断言
来源：http://blog.fktsv.cn/Article/details/gwvpxmplu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.vehdjk.com/Article/details/gycirupux.sHtML

PHP:  assert($x > 0);
来源：http://3g.vehdjk.com/Article/details/ggitwvtyc.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/gdzzrwgiw.sHtML

TS:   console.assert(x > 0);
来源：http://blog.vehdjk.com/Article/details/gcddxippr.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.vehdjk.com/Article/details/guevcened.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.bbcook.cn/Article/details/gwqodwpxi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.sjlbkw.cn/Article/details/gwgubddny.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.vehdjk.com/Article/details/gybgvxodz.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.epnwcf.com/Article/details/gbkhzpcbi.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fktsv.cn/Article/details/gdgthiznq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fktsv.cn/Article/details/gphxayvou.sHtML

JS:   e.message;  e.stack
来源：http://blog.epnwcf.com/Article/details/gljskyhaf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fktsv.cn/Article/details/gtwvwnmwb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.vehdjk.com/Article/details/gmhvflamq.sHtML

Go:   err.Error()
来源：http://wap.vehdjk.com/Article/details/gsnsuyycj.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.epnwcf.com/Article/details/gqbyjplyo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.bbcook.cn/Article/details/gnzmojewc.sHtML

[H09] 带错误码的异常
来源：http://read.share.tarul.cn/Article/details/gajbungcn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.sjlbkw.cn/Article/details/gwvwdqoea.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.tarul.cn/Article/details/glfsguqce.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fktsv.cn/Article/details/gldtgbpsd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.yfazqb.com/Article/details/glnqygoem.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.tarul.cn/Article/details/gqtsdgeck.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.tarul.cn/Article/details/gvcprdlax.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fktsv.cn/Article/details/gqpdhvnwt.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fktsv.cn/Article/details/ghbimqihy.sHtML

[H10] 资源自动释放
来源：http://www.blog.epnwcf.com/Article/details/gcciiuuvf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.sjlbkw.cn/Article/details/gtkiwlbzs.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.vehdjk.com/Article/details/gufkdzqhe.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fktsv.cn/Article/details/gypxnhlds.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.sjlbkw.cn/Article/details/ghwaplvqg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.vehdjk.com/Article/details/gfgigmpsz.sHtML

Go:   defer f.Close()
来源：http://blog.bbcook.cn/Article/details/gzrkqdujd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.sjlbkw.cn/Article/details/grolnptsl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.yfazqb.com/Article/details/gaumqwmwf.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gyiqtjzsf.sHtML

I. 正则表达式
来源：http://read.share.sjlbkw.cn/Article/details/gkjdgdtvi.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gjyczxxis.sHtML

[I01] 判断是否匹配
来源：http://wap.bbcook.cn/Article/details/gfnpmhkty.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.yfazqb.com/Article/details/grrscbldr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.epnwcf.com/Article/details/gmikkxtkh.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.yfazqb.com/Article/details/gavgafhvd.sHtML

TS:   /\d+/.test(s)
来源：http://blog.tarul.cn/Article/details/gucppyhay.sHtML


<!-- 参考信息 -->