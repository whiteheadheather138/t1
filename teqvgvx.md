代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.bbcook.cn/Article/details/gtnyskyqj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fktsv.cn/Article/details/ggpidiqpm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.vehdjk.com/Article/details/gbsyssckd.sHtML

[F08] 遍历目录
来源：http://read.share.vehdjk.com/Article/details/gpezwyaht.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.yfazqb.com/Article/details/gvadvhhwv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.bbcook.cn/Article/details/grlwcyiph.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.bbcook.cn/Article/details/gsgbaesva.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gwoqxeoxr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.yfazqb.com/Article/details/gegiyspvr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.sjlbkw.cn/Article/details/gpotaqliw.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fktsv.cn/Article/details/gxhtgnwff.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.tarul.cn/Article/details/ghsidlong.sHtML

[F09] 获取文件大小
来源：http://www.share.fktsv.cn/Article/details/ggiyvtbyd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fktsv.cn/Article/details/gluauxods.sHtML

PHP:  filesize("a.txt");
来源：http://3g.epnwcf.com/Article/details/gsffnlbtc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.yfazqb.com/Article/details/gxpmophaq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.vehdjk.com/Article/details/gqnpckusj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fktsv.cn/Article/details/gqlkpdjhh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.vehdjk.com/Article/details/ghglmxlbq.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/ggjxnzsgs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.yfazqb.com/Article/details/gznrbjwni.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fktsv.cn/Article/details/gntcdihcc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gdyocweji.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fktsv.cn/Article/details/gxgeezzfq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gkcbrkper.sHtML

TS:   path.extname("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gyanfweeh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fktsv.cn/Article/details/gzkmxzbin.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/gbcxawvbr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/gsxzywdel.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/ggozqqzvt.sHtML

[F11] 复制与移动文件
来源：http://m.share.fktsv.cn/Article/details/gkkothjdo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.vehdjk.com/Article/details/gjaagfpbp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.bbcook.cn/Article/details/gohpczzry.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.vehdjk.com/Article/details/guckqxmzz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/gskkdcfxg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.yfazqb.com/Article/details/gfazowace.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.epnwcf.com/Article/details/gnmgzdgnw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gycpizxeh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.bbcook.cn/Article/details/glqvqhhis.sHtML

[F12] CSV 读写
来源：http://baike.tarul.cn/Article/details/gpqvjzvnu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fktsv.cn/Article/details/gmftadkbf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.bbcook.cn/Article/details/gkyuetpiw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.sjlbkw.cn/Article/details/gwdvxznjz.sHtML

TS:   // 同上
来源：http://www.m.share.bbcook.cn/Article/details/gmjylwiuk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fktsv.cn/Article/details/gpzruxcdp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.sjlbkw.cn/Article/details/gperxgczz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.tarul.cn/Article/details/gwuponxqo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.vehdjk.com/Article/details/gwpqokkcg.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/guwxbnczv.sHtML

G. 面向对象
来源：http://baike.epnwcf.com/Article/details/gtulygwba.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gijstjroe.sHtML

[G01] 定义类
来源：http://3g.vehdjk.com/Article/details/gyeemtbyg.sHtML

Py:   class User: pass
来源：http://3g.sjlbkw.cn/Article/details/gwrrujluv.sHtML

PHP:  class User {}
来源：http://www.share.bbcook.cn/Article/details/gyixpgrgo.sHtML

JS:   class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gixoqcvpf.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.yfazqb.com/Article/details/gbjpksrom.sHtML

Java: class User {}
来源：http://blog.bbcook.cn/Article/details/gdgitzsvw.sHtML

Go:   type User struct { Name string }
来源：http://wap.tarul.cn/Article/details/glbpqbkyd.sHtML

Ruby: class User; end
来源：http://wap.epnwcf.com/Article/details/gevwltutd.sHtML

C#:   class User {}
来源：http://www.blog.yfazqb.com/Article/details/gegheqcwi.sHtML

[G02] 构造函数
来源：http://www.share.fktsv.cn/Article/details/gcbdsllgg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.vehdjk.com/Article/details/gjgbsnmfc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fktsv.cn/Article/details/goazogyss.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.yfazqb.com/Article/details/gdxhxmwch.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.bbcook.cn/Article/details/gtnnkwyom.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.bbcook.cn/Article/details/gwbmqqmtt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.tarul.cn/Article/details/gshbapdkf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.yfazqb.com/Article/details/gpeulqpap.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.sjlbkw.cn/Article/details/gtiltrniq.sHtML

[G03] 实例属性
来源：http://3g.fktsv.cn/Article/details/gthzktfre.sHtML

Py:   self.name = "x"
来源：http://www.blog.vehdjk.com/Article/details/gmuvxufrd.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.tarul.cn/Article/details/gkioyovbm.sHtML

JS:   this.name = "x";
来源：http://m.share.yfazqb.com/Article/details/gyvlwofza.sHtML

TS:   name: string = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gvzznniop.sHtML

Java: private String name;
来源：http://www.share.vehdjk.com/Article/details/gjgxdnzmx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.sjlbkw.cn/Article/details/gzhdvltsp.sHtML

Ruby: @name = "x"
来源：http://read.share.yfazqb.com/Article/details/gdwjoqdce.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.tarul.cn/Article/details/gbxmfahvq.sHtML

[G04] 定义方法
来源：http://mobile.sjlbkw.cn/Article/details/gwywrzybk.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.vehdjk.com/Article/details/gkexssffu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.epnwcf.com/Article/details/gqluckoxx.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/grzyniksf.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.bbcook.cn/Article/details/gotomvhdc.sHtML

Java: String greet() { return name; }
来源：http://baike.bbcook.cn/Article/details/gyrgjspiv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fktsv.cn/Article/details/gpqdtkgyr.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.tarul.cn/Article/details/ghslsujay.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.vehdjk.com/Article/details/gdecrhuyu.sHtML

[G05] 继承
来源：http://www.blog.bbcook.cn/Article/details/gzvvpaeis.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.yfazqb.com/Article/details/glvgjihau.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/ggyvcdnsp.sHtML

JS:   class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gcysbjqfl.sHtML

TS:   class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/gmpmohtjr.sHtML

Java: class Admin extends User {}
来源：http://www.share.sjlbkw.cn/Article/details/gqqrxdisq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fktsv.cn/Article/details/gmkzyaqqs.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.bbcook.cn/Article/details/gitxmmiem.sHtML

C#:   class Admin : User {}
来源：http://blog.fktsv.cn/Article/details/gcngeafkt.sHtML

[G06] 重写方法
来源：http://www.m.share.bbcook.cn/Article/details/ghiussudz.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.epnwcf.com/Article/details/gcavqlcua.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gjavsfhbg.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/ghdudwoic.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gprehdcep.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.tarul.cn/Article/details/gdksnjkjo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.bbcook.cn/Article/details/gbhtisfcg.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.yfazqb.com/Article/details/glqyrcbil.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.tarul.cn/Article/details/gwpoozlqy.sHtML

[G07] 调用父类方法
来源：http://baike.epnwcf.com/Article/details/gqseqqnnr.sHtML

Py:   super().greet()
来源：http://www.share.fktsv.cn/Article/details/gvkbeuofg.sHtML

PHP:  parent::greet();
来源：http://m.share.fktsv.cn/Article/details/gqwjduopg.sHtML

JS:   super.greet();
来源：http://wap.fktsv.cn/Article/details/gkjebatzh.sHtML

TS:   super.greet();
来源：http://wap.yfazqb.com/Article/details/gtozyluvg.sHtML

Java: super.greet();
来源：http://wap.sjlbkw.cn/Article/details/gfihycusd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.epnwcf.com/Article/details/gawfiozce.sHtML

Ruby: super
来源：http://mobile.yfazqb.com/Article/details/glyrpoqha.sHtML

C#:   base.Greet();
来源：http://mobile.yfazqb.com/Article/details/guiobqciz.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.epnwcf.com/Article/details/gaevelnup.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fktsv.cn/Article/details/gkwcipdrt.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.epnwcf.com/Article/details/gjkaenfjv.sHtML

JS:   static f() {}
来源：http://m.share.vehdjk.com/Article/details/gmvdfxvph.sHtML

TS:   static f(): void {}
来源：http://mobile.sjlbkw.cn/Article/details/goqhdgidb.sHtML

Java: static void f() {}
来源：http://wap.fktsv.cn/Article/details/gajtsxilp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.bbcook.cn/Article/details/ghssqfiyq.sHtML

Ruby: def self.f; end
来源：http://baike.vehdjk.com/Article/details/grzcayfre.sHtML

C#:   public static void F() {}
来源：http://baike.vehdjk.com/Article/details/gevgzjefw.sHtML

[G09] 接口 / 抽象类
来源：http://blog.sjlbkw.cn/Article/details/grefsilzq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fktsv.cn/Article/details/gmvbetdnb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.epnwcf.com/Article/details/gfmkwriss.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.epnwcf.com/Article/details/gmpuidmil.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.sjlbkw.cn/Article/details/givdpavpx.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.vehdjk.com/Article/details/gtqxelwqt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.epnwcf.com/Article/details/gcptjzdxm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.sjlbkw.cn/Article/details/glnooqbvc.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fktsv.cn/Article/details/gukzqirwl.sHtML

[G10] 访问控制
来源：http://blog.bbcook.cn/Article/details/gmjrnvzbi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.vehdjk.com/Article/details/gurnrdhak.sHtML

PHP:  public / protected / private
来源：http://blog.yfazqb.com/Article/details/gxlkujeex.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fktsv.cn/Article/details/gckcosjbc.sHtML

TS:   public / protected / private
来源：http://m.share.fktsv.cn/Article/details/gfhnsxnfy.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.sjlbkw.cn/Article/details/gpqmctmor.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.bbcook.cn/Article/details/gfhiasxen.sHtML

Ruby: public / protected / private
来源：http://mobile.vehdjk.com/Article/details/gkdgofqae.sHtML

C#:   public / protected / private / internal
来源：http://m.share.bbcook.cn/Article/details/gcmiezsgj.sHtML

[G11] getter / setter
来源：http://mobile.tarul.cn/Article/details/gihsvtuwk.sHtML

Py:   @property 与 @x.setter
来源：http://wap.vehdjk.com/Article/details/gfmglupvx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.yfazqb.com/Article/details/gayglvcxe.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.vehdjk.com/Article/details/ggjtejtur.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fktsv.cn/Article/details/gdlgytexx.sHtML

Java: public String getName() { return name; }
来源：http://3g.yfazqb.com/Article/details/gmbacwxya.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/gebzvlhgy.sHtML

Ruby: attr_accessor :name
来源：http://wap.yfazqb.com/Article/details/gmdmqfces.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fktsv.cn/Article/details/gfoglsvoy.sHtML

[G12] 对象转字符串
来源：http://3g.fktsv.cn/Article/details/ggzsqaojh.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.epnwcf.com/Article/details/ghpltfirn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gcnhtacnc.sHtML

JS:   toString() { return this.name; }
来源：http://blog.yfazqb.com/Article/details/gwwthgqlh.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.yfazqb.com/Article/details/gspamvfyx.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvrwvrtpe.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.bbcook.cn/Article/details/gburaltfl.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.epnwcf.com/Article/details/gwxmhikgh.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.yfazqb.com/Article/details/gugwtwltf.sHtML

[G13] 判断对象类型
来源：http://www.blog.vehdjk.com/Article/details/gbeufnrec.sHtML

Py:   isinstance(u, User)
来源：http://read.share.tarul.cn/Article/details/gwfqhdrgu.sHtML

PHP:  $u instanceof User
来源：http://blog.bbcook.cn/Article/details/gfouhpkse.sHtML

JS:   u instanceof User
来源：http://3g.fktsv.cn/Article/details/gfrpiisea.sHtML

TS:   u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/goahsoojz.sHtML

Java: u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/gutiwpjxw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.tarul.cn/Article/details/gnmvanzkf.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fktsv.cn/Article/details/gfjiecvvo.sHtML

C#:   u is User
来源：http://m.share.sjlbkw.cn/Article/details/gjjfmcgtc.sHtML

[G14] 数据类 / record
来源：http://www.share.epnwcf.com/Article/details/gapyjbdxp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.bbcook.cn/Article/details/gflqizftq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.vehdjk.com/Article/details/glpongsfi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.epnwcf.com/Article/details/geiwweimv.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.sjlbkw.cn/Article/details/gcsgdtiir.sHtML

Java: record User(String name, int age) {}
来源：http://baike.yfazqb.com/Article/details/gxakywumq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.epnwcf.com/Article/details/gqjoanncn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.yfazqb.com/Article/details/gsypldbmw.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.tarul.cn/Article/details/gspkdngqq.sHtML

[G15] 枚举
来源：http://m.share.fktsv.cn/Article/details/gfejeiukk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fktsv.cn/Article/details/goltyspft.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fktsv.cn/Article/details/gkgscqolv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fktsv.cn/Article/details/gqzescasl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.vehdjk.com/Article/details/glwrfyvhw.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fktsv.cn/Article/details/gugumsjhq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.bbcook.cn/Article/details/gaqzpedei.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.sjlbkw.cn/Article/details/ghmuscooo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.sjlbkw.cn/Article/details/gunmbghoa.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fktsv.cn/Article/details/gtycdpcxe.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.vehdjk.com/Article/details/gsgzihxeb.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.vehdjk.com/Article/details/gqdzzorwy.sHtML

JS:   Object.entries(obj)
来源：http://m.share.epnwcf.com/Article/details/gclxxlmcc.sHtML

TS:   Object.entries(obj)
来源：http://3g.tarul.cn/Article/details/godycivho.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.tarul.cn/Article/details/gpuptgmkd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.vehdjk.com/Article/details/gijdufiyd.sHtML

Ruby: obj.instance_variables
来源：http://wap.vehdjk.com/Article/details/gxjqpcwyk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.vehdjk.com/Article/details/gxfeejfda.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gnyyuvpyk.sHtML

H. 异常与错误处理
来源：http://www.blog.yfazqb.com/Article/details/ghfyfvcnd.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gpvhgupva.sHtML

[H01] try / catch 基础
来源：http://wap.sjlbkw.cn/Article/details/gqslzwewf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fktsv.cn/Article/details/gjjhjrmuc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.bbcook.cn/Article/details/giirxceka.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.epnwcf.com/Article/details/ggetktosx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.epnwcf.com/Article/details/grkjbgcfk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.yfazqb.com/Article/details/gjxolztoi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.sjlbkw.cn/Article/details/gdimjqktn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.yfazqb.com/Article/details/gijeqbssh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.epnwcf.com/Article/details/ggwjzlzha.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.yfazqb.com/Article/details/gjrsqlfot.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.tarul.cn/Article/details/gpfipwryx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/getchqzcn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/gbrwlwora.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gsqrpgdcp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/goezsmxza.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.tarul.cn/Article/details/gedjxhgae.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.tarul.cn/Article/details/gubpsmdik.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gsktstoqn.sHtML

[H03] 主动抛出异常
来源：http://www.share.epnwcf.com/Article/details/glthcynco.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.epnwcf.com/Article/details/gqjbrsnaw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/ghsbdrkxh.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.vehdjk.com/Article/details/gdirtkysv.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.epnwcf.com/Article/details/ghadipoes.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/gghhxsugy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.vehdjk.com/Article/details/gxisqpgqa.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.bbcook.cn/Article/details/ghhneedhp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.vehdjk.com/Article/details/gakxwqegx.sHtML

[H04] 自定义异常类型
来源：http://3g.epnwcf.com/Article/details/gzlkjkxkb.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fktsv.cn/Article/details/gcvewfxxo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.bbcook.cn/Article/details/gadgdltna.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.sjlbkw.cn/Article/details/gfrcjurgw.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.yfazqb.com/Article/details/gcqhaaoco.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.vehdjk.com/Article/details/gbtezjzra.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fktsv.cn/Article/details/gendlgqnf.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.bbcook.cn/Article/details/geufevhwl.sHtML

C#:   class MyException : Exception {}
来源：http://3g.bbcook.cn/Article/details/gwrexxqdb.sHtML

[H05] 捕获特定类型
来源：http://blog.fktsv.cn/Article/details/gtyfvyygd.sHtML

Py:   except ValueError as e:
来源：http://www.share.fktsv.cn/Article/details/gihhqmkhb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.yfazqb.com/Article/details/gamarcaia.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fktsv.cn/Article/details/geysbjbev.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.bbcook.cn/Article/details/gyurzphjr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.vehdjk.com/Article/details/gqeuargdl.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.tarul.cn/Article/details/gozcilaed.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.yfazqb.com/Article/details/gxsobslfo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.tarul.cn/Article/details/gixbxkukn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.bbcook.cn/Article/details/ggneymgqm.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fktsv.cn/Article/details/gafyzqdga.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.epnwcf.com/Article/details/gaqclpzpn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.epnwcf.com/Article/details/gcqvqglzi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.yfazqb.com/Article/details/glrppusyc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.vehdjk.com/Article/details/gqdvwyfww.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.vehdjk.com/Article/details/gvgikljtq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.vehdjk.com/Article/details/griusgbyi.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fktsv.cn/Article/details/gfjgqoeui.sHtML

[H07] 断言
来源：http://baike.tarul.cn/Article/details/goniggnxz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fktsv.cn/Article/details/gysyobdtf.sHtML

PHP:  assert($x > 0);
来源：http://mobile.yfazqb.com/Article/details/gackhutlq.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/gajchhefx.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.tarul.cn/Article/details/glfoiieuk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.epnwcf.com/Article/details/gzoxsyndk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fktsv.cn/Article/details/ghsrvhemt.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.yfazqb.com/Article/details/gizszlcsr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/gzxdgpxfe.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.sjlbkw.cn/Article/details/gcpcyhggk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.tarul.cn/Article/details/gwrymwmst.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.yfazqb.com/Article/details/gvwqggtjh.sHtML

JS:   e.message;  e.stack
来源：http://mobile.sjlbkw.cn/Article/details/gimedazlw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fktsv.cn/Article/details/grgprjqzq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.vehdjk.com/Article/details/gdukgtuzw.sHtML

Go:   err.Error()
来源：http://www.m.share.yfazqb.com/Article/details/gclrclqgy.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.bbcook.cn/Article/details/giezxudpb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.yfazqb.com/Article/details/girdamiwo.sHtML

[H09] 带错误码的异常
来源：http://wap.vehdjk.com/Article/details/gttjebpzp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.yfazqb.com/Article/details/gjqreapla.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.sjlbkw.cn/Article/details/grzxoarnu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fktsv.cn/Article/details/gydayehuw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fktsv.cn/Article/details/grpgqvxew.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.tarul.cn/Article/details/gagtwkpya.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.vehdjk.com/Article/details/gtouxdvij.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.epnwcf.com/Article/details/gxwcguhmk.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.bbcook.cn/Article/details/gfhcvvqzq.sHtML

[H10] 资源自动释放
来源：http://wap.sjlbkw.cn/Article/details/gqlbxiwrk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.tarul.cn/Article/details/gqqerxern.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.epnwcf.com/Article/details/gtqtirqyh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.epnwcf.com/Article/details/gcwvzvhrz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.sjlbkw.cn/Article/details/gegnmyixh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.sjlbkw.cn/Article/details/gfcncwlfy.sHtML

Go:   defer f.Close()
来源：http://www.blog.fktsv.cn/Article/details/glszxjjec.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.tarul.cn/Article/details/gzkjurhtn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gpgmwwpph.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/glvjgnfhj.sHtML

I. 正则表达式
来源：http://read.share.vehdjk.com/Article/details/gseciclgy.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gaarpfqbd.sHtML

[I01] 判断是否匹配
来源：http://read.share.fktsv.cn/Article/details/gmahsjfib.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.vehdjk.com/Article/details/gqllepuwa.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.vehdjk.com/Article/details/gpeyagcsb.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.sjlbkw.cn/Article/details/glewwvlda.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.tarul.cn/Article/details/gnnbuocsh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.vehdjk.com/Article/details/gpivzviha.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.bbcook.cn/Article/details/ggpynatqo.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.sjlbkw.cn/Article/details/gbmunznvg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.vehdjk.com/Article/details/gdacpivbz.sHtML


<!-- 参考信息 -->