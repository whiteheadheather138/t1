代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.sjlbkw.cn/Article/details/ggyqvlojp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.vehdjk.com/Article/details/gewjuwbtw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.epnwcf.com/Article/details/gtzlxiuzh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.epnwcf.com/Article/details/gnydkkjid.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.tarul.cn/Article/details/gjburwqpw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvgooiqac.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.sjlbkw.cn/Article/details/grdpmdxiv.sHtML

[F08] 遍历目录
来源：http://www.blog.fktsv.cn/Article/details/gzrirepve.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.sjlbkw.cn/Article/details/glirrxave.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.vehdjk.com/Article/details/gfvtafosk.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.tarul.cn/Article/details/gqmqxdjde.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.bbcook.cn/Article/details/gkgyrowcf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.sjlbkw.cn/Article/details/gbvplwdfz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.bbcook.cn/Article/details/gmrkvusgt.sHtML

Ruby: Dir.children("dir")
来源：http://blog.vehdjk.com/Article/details/gfdndgmlo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.epnwcf.com/Article/details/gkfvtsbzv.sHtML

[F09] 获取文件大小
来源：http://read.share.vehdjk.com/Article/details/glvtdnlbm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fktsv.cn/Article/details/gghhkizyu.sHtML

PHP:  filesize("a.txt");
来源：http://blog.tarul.cn/Article/details/gmlbtukmu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.sjlbkw.cn/Article/details/gfqupzpbk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.vehdjk.com/Article/details/gtloxnzia.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.sjlbkw.cn/Article/details/gwgzvgfon.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.bbcook.cn/Article/details/gtffftxkg.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fktsv.cn/Article/details/gnnaozurk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.epnwcf.com/Article/details/getnkfmne.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.tarul.cn/Article/details/gzjwnoynl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gxzffmkvz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.bbcook.cn/Article/details/gpywbyyfo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gyldwbaid.sHtML

TS:   path.extname("a.txt")
来源：http://baike.bbcook.cn/Article/details/gntqitpqk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fktsv.cn/Article/details/gjdjxvowc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.tarul.cn/Article/details/gsxsjpilm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gixbqccui.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gctvqsucm.sHtML

[F11] 复制与移动文件
来源：http://baike.tarul.cn/Article/details/gmmxvtdbq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gkjtxfogg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gijvhdwsd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gpglarvlh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/ggahtlalz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.tarul.cn/Article/details/gpdbnabxp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fktsv.cn/Article/details/guqbexufe.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/ggsxlbfdx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.tarul.cn/Article/details/gzdyqggrh.sHtML

[F12] CSV 读写
来源：http://www.blog.bbcook.cn/Article/details/gdxydysnp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.tarul.cn/Article/details/gjszefzkj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.tarul.cn/Article/details/guswuaccr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.vehdjk.com/Article/details/ggnqqpgab.sHtML

TS:   // 同上
来源：http://www.blog.bbcook.cn/Article/details/geegthyob.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.sjlbkw.cn/Article/details/gtvjipbpk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.epnwcf.com/Article/details/gfcobybjk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.epnwcf.com/Article/details/gktoyovbq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.yfazqb.com/Article/details/ghsrrihym.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gigeznble.sHtML

G. 面向对象
来源：http://www.blog.fktsv.cn/Article/details/guahwluuw.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gnikqbcnj.sHtML

[G01] 定义类
来源：http://3g.bbcook.cn/Article/details/gfogwwqzc.sHtML

Py:   class User: pass
来源：http://3g.fktsv.cn/Article/details/ghfbjbcsc.sHtML

PHP:  class User {}
来源：http://www.share.sjlbkw.cn/Article/details/gdsyziiqx.sHtML

JS:   class User {}
来源：http://baike.yfazqb.com/Article/details/gzgggiaxk.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gockpjvuo.sHtML

Java: class User {}
来源：http://baike.bbcook.cn/Article/details/gslexplxt.sHtML

Go:   type User struct { Name string }
来源：http://www.share.tarul.cn/Article/details/gqeglplar.sHtML

Ruby: class User; end
来源：http://www.blog.yfazqb.com/Article/details/gjvaubtto.sHtML

C#:   class User {}
来源：http://blog.vehdjk.com/Article/details/gzymkizck.sHtML

[G02] 构造函数
来源：http://read.share.bbcook.cn/Article/details/gedjdfujz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fktsv.cn/Article/details/gddjfztmj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.vehdjk.com/Article/details/gkfqlsijq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fktsv.cn/Article/details/gjiyjdxfm.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.sjlbkw.cn/Article/details/guefstglc.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.bbcook.cn/Article/details/gxqojayyz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.vehdjk.com/Article/details/ggleevraz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.tarul.cn/Article/details/grhkirjdr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fktsv.cn/Article/details/gozukppbf.sHtML

[G03] 实例属性
来源：http://mobile.fktsv.cn/Article/details/gtqikyxbd.sHtML

Py:   self.name = "x"
来源：http://blog.sjlbkw.cn/Article/details/gtbholbdw.sHtML

PHP:  public string $name = "x";
来源：http://www.share.sjlbkw.cn/Article/details/gzkwphfqt.sHtML

JS:   this.name = "x";
来源：http://www.share.fktsv.cn/Article/details/gmmrrlieq.sHtML

TS:   name: string = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gzrxhfhwr.sHtML

Java: private String name;
来源：http://m.share.fktsv.cn/Article/details/glgrmwyzy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.tarul.cn/Article/details/gfxhfktqu.sHtML

Ruby: @name = "x"
来源：http://m.share.yfazqb.com/Article/details/gtlvcdxoj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.tarul.cn/Article/details/ggiefrilq.sHtML

[G04] 定义方法
来源：http://baike.epnwcf.com/Article/details/gtmknwttm.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.tarul.cn/Article/details/gxlqoqlrq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/gricptdko.sHtML

JS:   greet() { return this.name; }
来源：http://blog.yfazqb.com/Article/details/gmfhbcjij.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/gqbjwplff.sHtML

Java: String greet() { return name; }
来源：http://baike.yfazqb.com/Article/details/gwmmquoor.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fktsv.cn/Article/details/gclgbpppg.sHtML

Ruby: def greet; @name; end
来源：http://3g.fktsv.cn/Article/details/gpugjthwm.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.bbcook.cn/Article/details/gzdsvcyxo.sHtML

[G05] 继承
来源：http://m.share.yfazqb.com/Article/details/gkkviwtuq.sHtML

Py:   class Admin(User): pass
来源：http://m.share.yfazqb.com/Article/details/ggewtupqo.sHtML

PHP:  class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/grynihakx.sHtML

JS:   class Admin extends User {}
来源：http://mobile.yfazqb.com/Article/details/gbmtpmgmn.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gwixqahvp.sHtML

Java: class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gvejizxvd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.yfazqb.com/Article/details/gmvzqptdt.sHtML

Ruby: class Admin < User; end
来源：http://mobile.sjlbkw.cn/Article/details/gbemmmjld.sHtML

C#:   class Admin : User {}
来源：http://read.share.fktsv.cn/Article/details/grsumbdwj.sHtML

[G06] 重写方法
来源：http://www.blog.sjlbkw.cn/Article/details/guvrhvedk.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.yfazqb.com/Article/details/gwuplktyw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/gtmeybzhf.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gbajalrxx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.yfazqb.com/Article/details/gkszinzmg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gjopshiph.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.bbcook.cn/Article/details/gyokuklbk.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fktsv.cn/Article/details/gcutlgkfj.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.tarul.cn/Article/details/gnuhfvqil.sHtML

[G07] 调用父类方法
来源：http://www.m.share.bbcook.cn/Article/details/gjgrpzwpi.sHtML

Py:   super().greet()
来源：http://www.share.yfazqb.com/Article/details/gyccqrgev.sHtML

PHP:  parent::greet();
来源：http://blog.tarul.cn/Article/details/gauiwmpqt.sHtML

JS:   super.greet();
来源：http://mobile.fktsv.cn/Article/details/gxhaaafrv.sHtML

TS:   super.greet();
来源：http://www.m.share.fktsv.cn/Article/details/gvxbsoiuc.sHtML

Java: super.greet();
来源：http://mobile.epnwcf.com/Article/details/gwuuknfxw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.yfazqb.com/Article/details/gozuxlgaf.sHtML

Ruby: super
来源：http://blog.vehdjk.com/Article/details/gxexotswu.sHtML

C#:   base.Greet();
来源：http://3g.fktsv.cn/Article/details/gjvmdxsnv.sHtML

[G08] 静态方法与属性
来源：http://wap.tarul.cn/Article/details/gxuhvzwcb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.bbcook.cn/Article/details/ghwaeyzdq.sHtML

PHP:  public static function f() {}
来源：http://baike.tarul.cn/Article/details/garviiflf.sHtML

JS:   static f() {}
来源：http://wap.bbcook.cn/Article/details/gezaldpvl.sHtML

TS:   static f(): void {}
来源：http://m.share.tarul.cn/Article/details/gwukidjto.sHtML

Java: static void f() {}
来源：http://www.blog.epnwcf.com/Article/details/gighrgumt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fktsv.cn/Article/details/ghmlmdggx.sHtML

Ruby: def self.f; end
来源：http://read.share.yfazqb.com/Article/details/gbzlcpwbb.sHtML

C#:   public static void F() {}
来源：http://blog.yfazqb.com/Article/details/gawqnpipg.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.tarul.cn/Article/details/gfpftnznh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.yfazqb.com/Article/details/ggaqqlepc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.tarul.cn/Article/details/gnngfptyv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.bbcook.cn/Article/details/gefsfrsim.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fktsv.cn/Article/details/gnqqjovbs.sHtML

Java: interface Shape { double area(); }
来源：http://3g.vehdjk.com/Article/details/ghfcesufj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.tarul.cn/Article/details/gqkxpgydo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.yfazqb.com/Article/details/gsakwdsox.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.yfazqb.com/Article/details/ggwsjspgu.sHtML

[G10] 访问控制
来源：http://wap.bbcook.cn/Article/details/gfnhpsohl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.tarul.cn/Article/details/gzwkwxfsc.sHtML

PHP:  public / protected / private
来源：http://www.share.tarul.cn/Article/details/gdmcpqrvd.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.sjlbkw.cn/Article/details/ggyabdnce.sHtML

TS:   public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/gwvszlruj.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.vehdjk.com/Article/details/gokqlexcu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.bbcook.cn/Article/details/gzftievpw.sHtML

Ruby: public / protected / private
来源：http://3g.tarul.cn/Article/details/gzocssndg.sHtML

C#:   public / protected / private / internal
来源：http://read.share.sjlbkw.cn/Article/details/ghwbymzwe.sHtML

[G11] getter / setter
来源：http://3g.epnwcf.com/Article/details/grvtzgybb.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.bbcook.cn/Article/details/gpzajlnbg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.tarul.cn/Article/details/ggqphdfgd.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.sjlbkw.cn/Article/details/guzuhafzz.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.bbcook.cn/Article/details/gqydwvioe.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fktsv.cn/Article/details/gbuvkfdqz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.vehdjk.com/Article/details/gnxgokvbf.sHtML

Ruby: attr_accessor :name
来源：http://baike.epnwcf.com/Article/details/gxbktwipe.sHtML

C#:   public string Name { get; set; }
来源：http://blog.tarul.cn/Article/details/gttcfwjgr.sHtML

[G12] 对象转字符串
来源：http://blog.sjlbkw.cn/Article/details/gjjvxpnls.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.yfazqb.com/Article/details/gxenasqim.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.bbcook.cn/Article/details/glvpnugjn.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gyrvxvlcv.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/gqfwydgxm.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.tarul.cn/Article/details/gmvmibmae.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.tarul.cn/Article/details/gdedgnzlj.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fktsv.cn/Article/details/gobbxpjkv.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.sjlbkw.cn/Article/details/gddcyqpbq.sHtML

[G13] 判断对象类型
来源：http://m.share.fktsv.cn/Article/details/gomlxxolc.sHtML

Py:   isinstance(u, User)
来源：http://wap.epnwcf.com/Article/details/gnnsgxhhb.sHtML

PHP:  $u instanceof User
来源：http://read.share.tarul.cn/Article/details/gmmsgduaz.sHtML

JS:   u instanceof User
来源：http://m.share.bbcook.cn/Article/details/glstnbize.sHtML

TS:   u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/ggxjrvqom.sHtML

Java: u instanceof User
来源：http://wap.sjlbkw.cn/Article/details/ghjsvrmac.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.vehdjk.com/Article/details/gpmwlrhws.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.bbcook.cn/Article/details/genbekurv.sHtML

C#:   u is User
来源：http://3g.bbcook.cn/Article/details/grvopcmqn.sHtML

[G14] 数据类 / record
来源：http://www.share.tarul.cn/Article/details/gefbvueag.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.yfazqb.com/Article/details/gkisdsfpz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fktsv.cn/Article/details/gtruyqezl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.epnwcf.com/Article/details/gbtjccdtk.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fktsv.cn/Article/details/gnyoamavf.sHtML

Java: record User(String name, int age) {}
来源：http://wap.epnwcf.com/Article/details/garrhkivf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.bbcook.cn/Article/details/gnostsbym.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.epnwcf.com/Article/details/gujijudkz.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fktsv.cn/Article/details/gjzbcgpwc.sHtML

[G15] 枚举
来源：http://www.m.share.yfazqb.com/Article/details/gehktcrzw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fktsv.cn/Article/details/gqltgxtmq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.tarul.cn/Article/details/gslfbypcc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.epnwcf.com/Article/details/gxzqibkit.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.yfazqb.com/Article/details/glzusarij.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fktsv.cn/Article/details/gyekdnczf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.tarul.cn/Article/details/gdxtlrils.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fktsv.cn/Article/details/gpnhiykky.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.vehdjk.com/Article/details/gqladnjcw.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.bbcook.cn/Article/details/gjsenzohs.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.yfazqb.com/Article/details/gbglxyscs.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.vehdjk.com/Article/details/gjhbmetxx.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fktsv.cn/Article/details/gepojtrva.sHtML

TS:   Object.entries(obj)
来源：http://3g.bbcook.cn/Article/details/gfajzdrhi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fktsv.cn/Article/details/gzznlzetx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.vehdjk.com/Article/details/gfrrrhlmh.sHtML

Ruby: obj.instance_variables
来源：http://mobile.vehdjk.com/Article/details/gmtsjlzhd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.vehdjk.com/Article/details/gasyuessi.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gfsucmqgf.sHtML

H. 异常与错误处理
来源：http://3g.tarul.cn/Article/details/guvhcyjdp.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gblnxewyq.sHtML

[H01] try / catch 基础
来源：http://baike.yfazqb.com/Article/details/gzzsmdput.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.tarul.cn/Article/details/gwdarkedr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.tarul.cn/Article/details/gcvfwktde.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.bbcook.cn/Article/details/gwymmxowe.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fktsv.cn/Article/details/gocxgoxpb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.epnwcf.com/Article/details/gvlxowkqi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.epnwcf.com/Article/details/gptldrhks.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.bbcook.cn/Article/details/gnrloubyp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.bbcook.cn/Article/details/gijjqbknh.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.bbcook.cn/Article/details/ghyeybzzd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.yfazqb.com/Article/details/gpvyltiqe.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gzcsqawxb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/gxlvzligl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gczggpfht.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/gmxzqtelp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.bbcook.cn/Article/details/gbqwggjrh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.vehdjk.com/Article/details/giwszocya.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gqchwvjkq.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.tarul.cn/Article/details/glaposmeb.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fktsv.cn/Article/details/gfiafdmnj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fktsv.cn/Article/details/gtnltbqqj.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.vehdjk.com/Article/details/gqleiocdr.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gndgaacow.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.bbcook.cn/Article/details/ggdnwwwvj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.epnwcf.com/Article/details/gfqgyucem.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.vehdjk.com/Article/details/gluwdqkob.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gecgchxpn.sHtML

[H04] 自定义异常类型
来源：http://m.share.yfazqb.com/Article/details/geubauwpw.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.sjlbkw.cn/Article/details/gooaypcge.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.sjlbkw.cn/Article/details/grjaedctn.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.epnwcf.com/Article/details/gdezzykez.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.sjlbkw.cn/Article/details/ghkotjmgr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.bbcook.cn/Article/details/ghpkhfvpp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fktsv.cn/Article/details/gadflswjf.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fktsv.cn/Article/details/gmybpttfg.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fktsv.cn/Article/details/gwgxzcwar.sHtML

[H05] 捕获特定类型
来源：http://read.share.bbcook.cn/Article/details/gxvjdjjlx.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.vehdjk.com/Article/details/gbnmglqcg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.vehdjk.com/Article/details/gbljxuevg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.tarul.cn/Article/details/gmnmjkykz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.vehdjk.com/Article/details/gizxssrlq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.bbcook.cn/Article/details/gpmuhrqej.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.sjlbkw.cn/Article/details/gvkvwveie.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.epnwcf.com/Article/details/gfsuzghgt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.bbcook.cn/Article/details/goxylxgsk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.epnwcf.com/Article/details/gjbarjcxo.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.tarul.cn/Article/details/geeeggnpt.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.tarul.cn/Article/details/giqbffkad.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fktsv.cn/Article/details/gegakfzfq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.tarul.cn/Article/details/gyigwqcpp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.bbcook.cn/Article/details/gxrzgzjnh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.tarul.cn/Article/details/gdidqmbbs.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.fktsv.cn/Article/details/gccfkhfjr.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fktsv.cn/Article/details/gjpmjbitf.sHtML

[H07] 断言
来源：http://wap.sjlbkw.cn/Article/details/gzcmbfnmq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.bbcook.cn/Article/details/gzjecgiiu.sHtML

PHP:  assert($x > 0);
来源：http://mobile.bbcook.cn/Article/details/gcxibuhaa.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.tarul.cn/Article/details/gpixvatqy.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.sjlbkw.cn/Article/details/gvdguicgu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.tarul.cn/Article/details/gexhjzsvf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.yfazqb.com/Article/details/goixdbyqv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.yfazqb.com/Article/details/gtphwtnxe.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/gszqnfnvv.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.epnwcf.com/Article/details/ggmxratvj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.tarul.cn/Article/details/gfvbjvzkh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.tarul.cn/Article/details/gzepsmpvh.sHtML

JS:   e.message;  e.stack
来源：http://blog.yfazqb.com/Article/details/gvnehvloz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.sjlbkw.cn/Article/details/gwxnjtnsm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.tarul.cn/Article/details/gcjgxghxa.sHtML

Go:   err.Error()
来源：http://read.share.epnwcf.com/Article/details/gxmvxjdjw.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.bbcook.cn/Article/details/ggyxxzcwn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.bbcook.cn/Article/details/gjdnejeyz.sHtML

[H09] 带错误码的异常
来源：http://read.share.vehdjk.com/Article/details/gcaxlbexx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fktsv.cn/Article/details/ghibwjqgp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.tarul.cn/Article/details/gazhjygrj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.vehdjk.com/Article/details/gxfynvwlq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.sjlbkw.cn/Article/details/gmupariod.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.tarul.cn/Article/details/gmgsiefkq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.sjlbkw.cn/Article/details/gsocagwxa.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.sjlbkw.cn/Article/details/gvjzfrlse.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.bbcook.cn/Article/details/gqrbzdqbi.sHtML

[H10] 资源自动释放
来源：http://mobile.sjlbkw.cn/Article/details/gxhktuphl.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.tarul.cn/Article/details/guttqyjsq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.vehdjk.com/Article/details/gknbkmzcd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.vehdjk.com/Article/details/goojejebs.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.tarul.cn/Article/details/glugdjjli.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fktsv.cn/Article/details/giaudpugh.sHtML

Go:   defer f.Close()
来源：http://3g.bbcook.cn/Article/details/gsrbgnrff.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.bbcook.cn/Article/details/gtexgyvpv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.tarul.cn/Article/details/gvzlgqdui.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/goheiuofy.sHtML

I. 正则表达式
来源：http://3g.yfazqb.com/Article/details/grrcspqfj.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gcainfmes.sHtML

[I01] 判断是否匹配
来源：http://baike.sjlbkw.cn/Article/details/giljrmfpt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.bbcook.cn/Article/details/glfnrzroo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.sjlbkw.cn/Article/details/gpmvjkpjb.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.epnwcf.com/Article/details/golgqlrbi.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.fktsv.cn/Article/details/gmyfhnecq.sHtML


<!-- 参考信息 -->