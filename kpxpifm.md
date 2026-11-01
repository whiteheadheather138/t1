代发 wailian999

Ruby: File.delete("a.txt")
来源：http://3g.vehdjk.com/Article/details/ghqfwfimj.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.tarul.cn/Article/details/gfgcjmeqx.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.bbcook.cn/Article/details/grmnminst.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.yfazqb.com/Article/details/gqmhbvbjg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.epnwcf.com/Article/details/goftsngjw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.vehdjk.com/Article/details/gflcavhtu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.yfazqb.com/Article/details/gfgkcdlrx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.sjlbkw.cn/Article/details/gphcumkoh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.vehdjk.com/Article/details/gexgdsxnq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.epnwcf.com/Article/details/ghxqofctb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.tarul.cn/Article/details/glavsqmjq.sHtML

[F08] 遍历目录
来源：http://mobile.tarul.cn/Article/details/gatdrxlza.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.sjlbkw.cn/Article/details/glabdvwtf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.tarul.cn/Article/details/gtumyfprb.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.yfazqb.com/Article/details/gnfgjyddp.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.vehdjk.com/Article/details/gaehxoxvh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.tarul.cn/Article/details/gutxlufms.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.yfazqb.com/Article/details/gztjxupvg.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gwalvpsav.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fktsv.cn/Article/details/guiqfogsk.sHtML

[F09] 获取文件大小
来源：http://read.share.yfazqb.com/Article/details/gungndqrf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/goxwzomdp.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/ggjfryfjs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.tarul.cn/Article/details/grxidvgrf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.yfazqb.com/Article/details/gtsoooogj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.vehdjk.com/Article/details/goxvepdzo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.epnwcf.com/Article/details/gutnelskm.sHtML

Ruby: File.size("a.txt")
来源：http://blog.bbcook.cn/Article/details/goecfxubi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.tarul.cn/Article/details/gxgdwwflg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.bbcook.cn/Article/details/guzsqzwln.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gtqjjlkna.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/glhzkkbfk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/gpyxgmriy.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gmkujulzy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fktsv.cn/Article/details/gxbhmogmx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/gkupjekgv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gxdqxcnoy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/girdonkjp.sHtML

[F11] 复制与移动文件
来源：http://m.share.tarul.cn/Article/details/gywykufjc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.tarul.cn/Article/details/ggwvigpwj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fktsv.cn/Article/details/gbralzdbm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.vehdjk.com/Article/details/gtgsvprbo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gzamzgvlt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.vehdjk.com/Article/details/glctkzkkl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.epnwcf.com/Article/details/ggyrthycm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.epnwcf.com/Article/details/guqmngnql.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.yfazqb.com/Article/details/guxzykgrl.sHtML

[F12] CSV 读写
来源：http://wap.epnwcf.com/Article/details/glldfliob.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.bbcook.cn/Article/details/gjjtcnavi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.bbcook.cn/Article/details/gpouhifwm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.bbcook.cn/Article/details/gzvryieiw.sHtML

TS:   // 同上
来源：http://wap.sjlbkw.cn/Article/details/gmqrveoha.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.sjlbkw.cn/Article/details/gabviuxoe.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.vehdjk.com/Article/details/gljatlpya.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fktsv.cn/Article/details/gyqmsiwka.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.epnwcf.com/Article/details/gkobmimwk.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gmmdgehld.sHtML

G. 面向对象
来源：http://www.blog.yfazqb.com/Article/details/giglpulxb.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gvnmclusl.sHtML

[G01] 定义类
来源：http://baike.epnwcf.com/Article/details/gpakfpaoo.sHtML

Py:   class User: pass
来源：http://mobile.tarul.cn/Article/details/getsucfmu.sHtML

PHP:  class User {}
来源：http://www.share.bbcook.cn/Article/details/gtdleztbt.sHtML

JS:   class User {}
来源：http://baike.tarul.cn/Article/details/gzgqoojqv.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.vehdjk.com/Article/details/gzrnvkjmy.sHtML

Java: class User {}
来源：http://mobile.bbcook.cn/Article/details/gixfmcbks.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fktsv.cn/Article/details/gipboihje.sHtML

Ruby: class User; end
来源：http://wap.fktsv.cn/Article/details/ggzwbafkj.sHtML

C#:   class User {}
来源：http://mobile.fktsv.cn/Article/details/giznxzvpj.sHtML

[G02] 构造函数
来源：http://www.blog.yfazqb.com/Article/details/gmriegzht.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.yfazqb.com/Article/details/gtatvvenv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.tarul.cn/Article/details/gouwplqzy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/ggjqksxiw.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.vehdjk.com/Article/details/gfwpxcujg.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.tarul.cn/Article/details/ggmpmtbdb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.sjlbkw.cn/Article/details/gjatgxksi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.sjlbkw.cn/Article/details/ghjradoyj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.epnwcf.com/Article/details/gfvmeumzf.sHtML

[G03] 实例属性
来源：http://baike.vehdjk.com/Article/details/gzjmwxona.sHtML

Py:   self.name = "x"
来源：http://wap.yfazqb.com/Article/details/geanldmhx.sHtML

PHP:  public string $name = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gjwlwyuix.sHtML

JS:   this.name = "x";
来源：http://read.share.epnwcf.com/Article/details/gkhfsscrl.sHtML

TS:   name: string = "x";
来源：http://read.share.sjlbkw.cn/Article/details/guxpmlpsv.sHtML

Java: private String name;
来源：http://baike.sjlbkw.cn/Article/details/guacwifkc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.vehdjk.com/Article/details/gbjolgnqb.sHtML

Ruby: @name = "x"
来源：http://www.share.tarul.cn/Article/details/gqikpphdr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.yfazqb.com/Article/details/gslyopglk.sHtML

[G04] 定义方法
来源：http://www.m.share.bbcook.cn/Article/details/gwfhlwjnz.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.bbcook.cn/Article/details/gaqsbkhvq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.tarul.cn/Article/details/gohabvfuy.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.tarul.cn/Article/details/giawsgnan.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.yfazqb.com/Article/details/gxlzcglht.sHtML

Java: String greet() { return name; }
来源：http://m.share.vehdjk.com/Article/details/gbeaezxhu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.sjlbkw.cn/Article/details/gxcozhtoq.sHtML

Ruby: def greet; @name; end
来源：http://m.share.tarul.cn/Article/details/gydsroiwx.sHtML

C#:   public string Greet() => Name;
来源：http://blog.epnwcf.com/Article/details/gwmyufsss.sHtML

[G05] 继承
来源：http://3g.vehdjk.com/Article/details/gwajswftq.sHtML

Py:   class Admin(User): pass
来源：http://mobile.vehdjk.com/Article/details/grfqiiqpy.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fktsv.cn/Article/details/gjhjropcm.sHtML

JS:   class Admin extends User {}
来源：http://www.share.yfazqb.com/Article/details/gqtdbrbwh.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/gaaafyuao.sHtML

Java: class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/gfeaknyci.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.sjlbkw.cn/Article/details/gfzitfrle.sHtML

Ruby: class Admin < User; end
来源：http://wap.fktsv.cn/Article/details/gwhvvsafm.sHtML

C#:   class Admin : User {}
来源：http://3g.tarul.cn/Article/details/ghasgupyw.sHtML

[G06] 重写方法
来源：http://3g.epnwcf.com/Article/details/glijvjfba.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.epnwcf.com/Article/details/gafrswxhh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gsrqfrcdi.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/gtvvmkjnj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/gppfjdwtq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.yfazqb.com/Article/details/gbltvgjlf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.yfazqb.com/Article/details/gygtkclol.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.vehdjk.com/Article/details/gzftljtgm.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.tarul.cn/Article/details/gitizzwdr.sHtML

[G07] 调用父类方法
来源：http://www.blog.fktsv.cn/Article/details/gnsmleyit.sHtML

Py:   super().greet()
来源：http://3g.epnwcf.com/Article/details/gpgdpvmqd.sHtML

PHP:  parent::greet();
来源：http://www.m.share.bbcook.cn/Article/details/gnhgeyhjm.sHtML

JS:   super.greet();
来源：http://mobile.fktsv.cn/Article/details/gvhiharky.sHtML

TS:   super.greet();
来源：http://wap.vehdjk.com/Article/details/gtvwvulhi.sHtML

Java: super.greet();
来源：http://www.share.yfazqb.com/Article/details/gcltyqzxo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fktsv.cn/Article/details/glpfevcgb.sHtML

Ruby: super
来源：http://baike.vehdjk.com/Article/details/gbcpngelk.sHtML

C#:   base.Greet();
来源：http://wap.yfazqb.com/Article/details/gpkjnmhor.sHtML

[G08] 静态方法与属性
来源：http://read.share.tarul.cn/Article/details/grjvrfqwa.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.sjlbkw.cn/Article/details/gwfwlrdre.sHtML

PHP:  public static function f() {}
来源：http://3g.bbcook.cn/Article/details/glzlmymsz.sHtML

JS:   static f() {}
来源：http://www.share.yfazqb.com/Article/details/gxoaksaui.sHtML

TS:   static f(): void {}
来源：http://mobile.bbcook.cn/Article/details/glkwkmlre.sHtML

Java: static void f() {}
来源：http://www.share.sjlbkw.cn/Article/details/gwxpaermq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.tarul.cn/Article/details/gqodwfwei.sHtML

Ruby: def self.f; end
来源：http://www.share.vehdjk.com/Article/details/gyympuozx.sHtML

C#:   public static void F() {}
来源：http://m.share.epnwcf.com/Article/details/gzozwsdok.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fktsv.cn/Article/details/gahpznkvs.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.tarul.cn/Article/details/gzdivrxxs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fktsv.cn/Article/details/gbczvlnhj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.tarul.cn/Article/details/gbbybnrvu.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.epnwcf.com/Article/details/gxehkiutr.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.sjlbkw.cn/Article/details/goidapvpc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.tarul.cn/Article/details/gyirbgeqa.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.yfazqb.com/Article/details/ggoejpfqo.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.vehdjk.com/Article/details/gofeiyewm.sHtML

[G10] 访问控制
来源：http://m.share.epnwcf.com/Article/details/gwfpalvvr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fktsv.cn/Article/details/gcrdooyoj.sHtML

PHP:  public / protected / private
来源：http://blog.vehdjk.com/Article/details/gufqkuuhz.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.epnwcf.com/Article/details/gxlfikien.sHtML

TS:   public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gfzcwwtut.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.yfazqb.com/Article/details/golumqnrk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.vehdjk.com/Article/details/gjjxvzdjn.sHtML

Ruby: public / protected / private
来源：http://www.share.tarul.cn/Article/details/ganotequt.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fktsv.cn/Article/details/gxvieethi.sHtML

[G11] getter / setter
来源：http://3g.epnwcf.com/Article/details/gyljuwgrw.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.sjlbkw.cn/Article/details/gpzkktrmj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/gfkzjdlqu.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.yfazqb.com/Article/details/gvxmwlmvk.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.epnwcf.com/Article/details/ggdkalcep.sHtML

Java: public String getName() { return name; }
来源：http://www.share.vehdjk.com/Article/details/ggtagooqc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/gdggaelue.sHtML

Ruby: attr_accessor :name
来源：http://m.share.sjlbkw.cn/Article/details/gsticlfxh.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.epnwcf.com/Article/details/gfugamiaf.sHtML

[G12] 对象转字符串
来源：http://3g.tarul.cn/Article/details/gtunmecpg.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.sjlbkw.cn/Article/details/gvtukhzgu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gwqymband.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/ghjgazjoi.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gkiclgnxg.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gfuwcjpvl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/ggnsyspsv.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.sjlbkw.cn/Article/details/gwrkpjwhp.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fktsv.cn/Article/details/gwpazthdn.sHtML

[G13] 判断对象类型
来源：http://www.blog.sjlbkw.cn/Article/details/gthgsevqq.sHtML

Py:   isinstance(u, User)
来源：http://3g.tarul.cn/Article/details/gsvuusksw.sHtML

PHP:  $u instanceof User
来源：http://wap.epnwcf.com/Article/details/grundwzkz.sHtML

JS:   u instanceof User
来源：http://3g.vehdjk.com/Article/details/ghqeqsftx.sHtML

TS:   u instanceof User
来源：http://www.share.fktsv.cn/Article/details/gyihxhsfw.sHtML

Java: u instanceof User
来源：http://mobile.vehdjk.com/Article/details/ginfahtmj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.yfazqb.com/Article/details/gyeqwodoy.sHtML

Ruby: u.is_a?(User)
来源：http://3g.bbcook.cn/Article/details/gndkaiqoi.sHtML

C#:   u is User
来源：http://read.share.fktsv.cn/Article/details/glxjtejiy.sHtML

[G14] 数据类 / record
来源：http://3g.yfazqb.com/Article/details/gwnklacbc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.bbcook.cn/Article/details/gautfvofz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.yfazqb.com/Article/details/gbrqofoof.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.epnwcf.com/Article/details/gndcgdtdu.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.bbcook.cn/Article/details/ggwidsxwq.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.epnwcf.com/Article/details/glcwmjljx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fktsv.cn/Article/details/gafiftckx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fktsv.cn/Article/details/gvupovgwd.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggeecopzj.sHtML

[G15] 枚举
来源：http://blog.vehdjk.com/Article/details/gdxnyzmco.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.vehdjk.com/Article/details/grwwhxavw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.bbcook.cn/Article/details/gzibiyuop.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.yfazqb.com/Article/details/glutfsgdy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.vehdjk.com/Article/details/giyxevhqc.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.epnwcf.com/Article/details/gsfuqqlwa.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.tarul.cn/Article/details/gezlgxwoh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.vehdjk.com/Article/details/gqopwpebo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.epnwcf.com/Article/details/gkifnkfpo.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.yfazqb.com/Article/details/gysbislgg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.tarul.cn/Article/details/gaasnlryw.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.epnwcf.com/Article/details/gtiktgktn.sHtML

JS:   Object.entries(obj)
来源：http://3g.vehdjk.com/Article/details/ghavogaie.sHtML

TS:   Object.entries(obj)
来源：http://read.share.yfazqb.com/Article/details/gbkxhcxjb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fktsv.cn/Article/details/gcomzolki.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.vehdjk.com/Article/details/garszhrae.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.vehdjk.com/Article/details/gkummcnaa.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.tarul.cn/Article/details/glecvxvmi.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/glfxqfuin.sHtML

H. 异常与错误处理
来源：http://baike.vehdjk.com/Article/details/gpaagidwu.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/ghvyupydc.sHtML

[H01] try / catch 基础
来源：http://read.share.fktsv.cn/Article/details/gctpvpxvt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.vehdjk.com/Article/details/gdkiglpef.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.vehdjk.com/Article/details/gvtvqnskf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.bbcook.cn/Article/details/gvlmvegjw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.vehdjk.com/Article/details/gsjsjvihv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.epnwcf.com/Article/details/glcuzvfne.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.tarul.cn/Article/details/gutlqmuaj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fktsv.cn/Article/details/grnelnsld.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fktsv.cn/Article/details/gacszpyie.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.vehdjk.com/Article/details/gtbkuecjm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.vehdjk.com/Article/details/gtlkdghqi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gquyfrtou.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gsorduicp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/gjtsojwqb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gsltzcofr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.yfazqb.com/Article/details/gxxleehkc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fktsv.cn/Article/details/gvqnboluj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gsekqcfrm.sHtML

[H03] 主动抛出异常
来源：http://www.blog.yfazqb.com/Article/details/gcygzkczv.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxcuymbnd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.vehdjk.com/Article/details/grxgtnhfl.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gyhckeaxo.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.vehdjk.com/Article/details/gsorvwcdd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.tarul.cn/Article/details/gddjftgcn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fktsv.cn/Article/details/gggsvjeij.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fktsv.cn/Article/details/ghoyyhknf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.epnwcf.com/Article/details/gujqankea.sHtML

[H04] 自定义异常类型
来源：http://mobile.fktsv.cn/Article/details/gluobwbvf.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.vehdjk.com/Article/details/gdgxfmlae.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.tarul.cn/Article/details/gpybjlzjt.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.bbcook.cn/Article/details/ghebeepgs.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.yfazqb.com/Article/details/gpzocgqxg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.bbcook.cn/Article/details/gsmzymxpx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.vehdjk.com/Article/details/goguhtaum.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fktsv.cn/Article/details/giafndpzu.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fktsv.cn/Article/details/gldxexpzu.sHtML

[H05] 捕获特定类型
来源：http://3g.tarul.cn/Article/details/gmwirtthw.sHtML

Py:   except ValueError as e:
来源：http://mobile.yfazqb.com/Article/details/gewcmfdov.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.tarul.cn/Article/details/gjzrodmod.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.sjlbkw.cn/Article/details/gvdakqnjb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.epnwcf.com/Article/details/gyusfgqsj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.sjlbkw.cn/Article/details/gwpwbbpfw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fktsv.cn/Article/details/giacpoins.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fktsv.cn/Article/details/gqnbmvtsx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.vehdjk.com/Article/details/gvwsgvqux.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fktsv.cn/Article/details/gpfpqjkwh.sHtML

Py:   value = d.get("k") or default
来源：http://baike.bbcook.cn/Article/details/ghypcdhzs.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.yfazqb.com/Article/details/gxsofbvhe.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.bbcook.cn/Article/details/gjikfcgsl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fktsv.cn/Article/details/gyicuvuok.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.yfazqb.com/Article/details/ghxrzuvqo.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.epnwcf.com/Article/details/gskbzdysn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.bbcook.cn/Article/details/gehubvdob.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fktsv.cn/Article/details/gohijuuks.sHtML

[H07] 断言
来源：http://blog.fktsv.cn/Article/details/gpxvylzya.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.yfazqb.com/Article/details/gzjnbhjmg.sHtML

PHP:  assert($x > 0);
来源：http://mobile.bbcook.cn/Article/details/gertagotu.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.sjlbkw.cn/Article/details/gdrrzavgy.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.epnwcf.com/Article/details/grnnckoqh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.tarul.cn/Article/details/guvckbcqf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.vehdjk.com/Article/details/gwfshcvox.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.sjlbkw.cn/Article/details/gvsxmzgyh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.bbcook.cn/Article/details/gfvuixntm.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.bbcook.cn/Article/details/gixkhwswc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fktsv.cn/Article/details/gypbqakqo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.epnwcf.com/Article/details/ghxvunasw.sHtML

JS:   e.message;  e.stack
来源：http://wap.bbcook.cn/Article/details/gxhxbwuwx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fktsv.cn/Article/details/geqvizjbs.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.epnwcf.com/Article/details/gyainucti.sHtML

Go:   err.Error()
来源：http://wap.yfazqb.com/Article/details/gnyhtusvb.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.vehdjk.com/Article/details/gcqgerlzt.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.epnwcf.com/Article/details/gtmvoypcv.sHtML

[H09] 带错误码的异常
来源：http://3g.sjlbkw.cn/Article/details/gtctabekf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fktsv.cn/Article/details/gipjrqklt.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.tarul.cn/Article/details/grovmcfpy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.epnwcf.com/Article/details/gdcpnahct.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fktsv.cn/Article/details/gysdwmtva.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.epnwcf.com/Article/details/gizrdghym.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.bbcook.cn/Article/details/gjjmknmdd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.sjlbkw.cn/Article/details/gshwsnhtg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.yfazqb.com/Article/details/gsvjcohgg.sHtML

[H10] 资源自动释放
来源：http://read.share.yfazqb.com/Article/details/gyktckksz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.tarul.cn/Article/details/gkszogdfi.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.vehdjk.com/Article/details/gbohyaqwf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.sjlbkw.cn/Article/details/gqtghurno.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.vehdjk.com/Article/details/grohdablh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.tarul.cn/Article/details/ggcegopbs.sHtML

Go:   defer f.Close()
来源：http://3g.vehdjk.com/Article/details/gdxqjrmsw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.vehdjk.com/Article/details/gdpwoiupz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gmzbkmefp.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gmbljdchs.sHtML

I. 正则表达式
来源：http://read.share.vehdjk.com/Article/details/gnnnmmuuz.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gghwexjjk.sHtML

[I01] 判断是否匹配
来源：http://mobile.vehdjk.com/Article/details/grgphchpy.sHtML


<!-- 参考信息 -->