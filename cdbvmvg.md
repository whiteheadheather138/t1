代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://www.m.share.vehdjk.com/Article/details/gtaudqgqx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.sjlbkw.cn/Article/details/gdowmdstk.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gdrqzsuhg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gkzyfsfez.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/gfspfucib.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/gvbucwvgb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.epnwcf.com/Article/details/gxbloprvu.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.vehdjk.com/Article/details/guhooqoji.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.tarul.cn/Article/details/guukilcgs.sHtML

[F06] 删除文件
来源：http://3g.fktsv.cn/Article/details/gmctwdzsi.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gmwikowzf.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.tarul.cn/Article/details/gjooqukgh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.tarul.cn/Article/details/gzesojwcf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gifwtpmvp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.vehdjk.com/Article/details/gewtjhdhx.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.tarul.cn/Article/details/gtelrnent.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gfyhncrum.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gupjyhggf.sHtML

[F07] 创建目录（含多级）
来源：http://blog.yfazqb.com/Article/details/gijhqjauu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fktsv.cn/Article/details/gtqxhmodh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.epnwcf.com/Article/details/glqofcbfu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fktsv.cn/Article/details/gfxahhtco.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.sjlbkw.cn/Article/details/gajqemlss.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.epnwcf.com/Article/details/gqqsjzjwv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.vehdjk.com/Article/details/gdhdojzoe.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.epnwcf.com/Article/details/gttrnwpis.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.epnwcf.com/Article/details/gjvqohkmq.sHtML

[F08] 遍历目录
来源：http://blog.epnwcf.com/Article/details/gxbcorola.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fktsv.cn/Article/details/glhtnckuu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.tarul.cn/Article/details/gqzyappae.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.epnwcf.com/Article/details/ghsodenmb.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.epnwcf.com/Article/details/gplgxbbgq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fktsv.cn/Article/details/goidzrsva.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.vehdjk.com/Article/details/glzambjmi.sHtML

Ruby: Dir.children("dir")
来源：http://wap.yfazqb.com/Article/details/gapyoahgt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.epnwcf.com/Article/details/gwjbnamgr.sHtML

[F09] 获取文件大小
来源：http://blog.epnwcf.com/Article/details/gsbeaktzs.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.tarul.cn/Article/details/glagnywcn.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gbtbngphg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.tarul.cn/Article/details/gprnqoqko.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.bbcook.cn/Article/details/gbuxyctaz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gmjyycwdp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.epnwcf.com/Article/details/gubfqmsrz.sHtML

Ruby: File.size("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gbouhqxne.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fktsv.cn/Article/details/gkuzmfeye.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.bbcook.cn/Article/details/gqrhjthwu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/gdkvgwzcs.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gstvgtymz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gikvgyvfm.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gcgqykixx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.bbcook.cn/Article/details/gbsnmlusq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gjfigddjw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gbrssytbu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gmktxbbdd.sHtML

[F11] 复制与移动文件
来源：http://www.share.epnwcf.com/Article/details/gcfqfmout.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.vehdjk.com/Article/details/goltmrsck.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.sjlbkw.cn/Article/details/gxybklpli.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gogxgesxd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fktsv.cn/Article/details/gjxbqsfwk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.yfazqb.com/Article/details/gtjgzgiin.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.epnwcf.com/Article/details/gycecspql.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/gzcialxam.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fktsv.cn/Article/details/gzuyjpqaa.sHtML

[F12] CSV 读写
来源：http://blog.fktsv.cn/Article/details/gvveqipbz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.vehdjk.com/Article/details/grivilgbi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.bbcook.cn/Article/details/gaaepxzrw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.sjlbkw.cn/Article/details/gnbbyybrg.sHtML

TS:   // 同上
来源：http://www.m.share.tarul.cn/Article/details/gxyqxcakj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.epnwcf.com/Article/details/gatzxsuoq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.vehdjk.com/Article/details/gdgxzuhee.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.epnwcf.com/Article/details/gyoqrryei.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.yfazqb.com/Article/details/gpmvxfugm.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gfqstburr.sHtML

G. 面向对象
来源：http://www.blog.sjlbkw.cn/Article/details/gixpkconm.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gbipmqnwq.sHtML

[G01] 定义类
来源：http://www.m.share.sjlbkw.cn/Article/details/gdfqduiuu.sHtML

Py:   class User: pass
来源：http://m.share.bbcook.cn/Article/details/gfpwqpubw.sHtML

PHP:  class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gseydlvad.sHtML

JS:   class User {}
来源：http://www.share.bbcook.cn/Article/details/grddhpjbi.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.epnwcf.com/Article/details/gocjjqlcx.sHtML

Java: class User {}
来源：http://mobile.yfazqb.com/Article/details/goaalhurx.sHtML

Go:   type User struct { Name string }
来源：http://read.share.sjlbkw.cn/Article/details/gsmkkeciu.sHtML

Ruby: class User; end
来源：http://baike.sjlbkw.cn/Article/details/gvqbjquiy.sHtML

C#:   class User {}
来源：http://read.share.fktsv.cn/Article/details/gjjdemggx.sHtML

[G02] 构造函数
来源：http://www.blog.yfazqb.com/Article/details/gxsednjmj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.epnwcf.com/Article/details/gvhimflyi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.tarul.cn/Article/details/gzmimcnzo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.tarul.cn/Article/details/gtrbxsczx.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.sjlbkw.cn/Article/details/gayigctpx.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.yfazqb.com/Article/details/gyrjxctmf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.vehdjk.com/Article/details/gigzbcbxy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fktsv.cn/Article/details/gucdxgxsw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fktsv.cn/Article/details/gshwkitbf.sHtML

[G03] 实例属性
来源：http://baike.epnwcf.com/Article/details/gwjzgempe.sHtML

Py:   self.name = "x"
来源：http://www.share.bbcook.cn/Article/details/gusizcvsm.sHtML

PHP:  public string $name = "x";
来源：http://www.share.vehdjk.com/Article/details/gkbubcibb.sHtML

JS:   this.name = "x";
来源：http://www.m.share.sjlbkw.cn/Article/details/gurxnamcd.sHtML

TS:   name: string = "x";
来源：http://blog.vehdjk.com/Article/details/gghldoqqr.sHtML

Java: private String name;
来源：http://www.share.epnwcf.com/Article/details/gnfnmthco.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.epnwcf.com/Article/details/gzaswaocb.sHtML

Ruby: @name = "x"
来源：http://www.share.bbcook.cn/Article/details/gtofdgxhs.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.sjlbkw.cn/Article/details/geieaadcu.sHtML

[G04] 定义方法
来源：http://mobile.bbcook.cn/Article/details/gokipzplg.sHtML

Py:   def greet(self): return self.name
来源：http://wap.tarul.cn/Article/details/gwyhzwnxm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.vehdjk.com/Article/details/gjytkfxel.sHtML

JS:   greet() { return this.name; }
来源：http://baike.epnwcf.com/Article/details/grhfbjqwt.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gerkakkcz.sHtML

Java: String greet() { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gtdigzomr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gpcxxtokh.sHtML

Ruby: def greet; @name; end
来源：http://www.share.vehdjk.com/Article/details/gnfkhixll.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.bbcook.cn/Article/details/gkfbribpo.sHtML

[G05] 继承
来源：http://baike.vehdjk.com/Article/details/gygvjodnz.sHtML

Py:   class Admin(User): pass
来源：http://baike.vehdjk.com/Article/details/glsrkmaor.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/gertymoui.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/gjmvwhxjt.sHtML

TS:   class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/gtiypbtvw.sHtML

Java: class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/gqtvbeeoe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.sjlbkw.cn/Article/details/ghgilpuei.sHtML

Ruby: class Admin < User; end
来源：http://mobile.tarul.cn/Article/details/ggwqxverm.sHtML

C#:   class Admin : User {}
来源：http://www.blog.tarul.cn/Article/details/gcavgsqvh.sHtML

[G06] 重写方法
来源：http://www.share.yfazqb.com/Article/details/gabzlllnw.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.epnwcf.com/Article/details/gbwmqwvzy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/ghjaktxvi.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.sjlbkw.cn/Article/details/gynntbvoa.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/guavgtjtj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.yfazqb.com/Article/details/ggmnofmzp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fktsv.cn/Article/details/gqtwvypio.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.epnwcf.com/Article/details/gnvrvuzqb.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.bbcook.cn/Article/details/gehjrmsso.sHtML

[G07] 调用父类方法
来源：http://baike.fktsv.cn/Article/details/gfefsxqca.sHtML

Py:   super().greet()
来源：http://mobile.vehdjk.com/Article/details/gimhyxnyq.sHtML

PHP:  parent::greet();
来源：http://wap.yfazqb.com/Article/details/gdgctubht.sHtML

JS:   super.greet();
来源：http://read.share.tarul.cn/Article/details/gytbsssml.sHtML

TS:   super.greet();
来源：http://baike.tarul.cn/Article/details/gjyqprlkg.sHtML

Java: super.greet();
来源：http://www.m.share.bbcook.cn/Article/details/gcgayxxkt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.sjlbkw.cn/Article/details/gkzzohbap.sHtML

Ruby: super
来源：http://3g.sjlbkw.cn/Article/details/gthwichji.sHtML

C#:   base.Greet();
来源：http://blog.yfazqb.com/Article/details/grensovic.sHtML

[G08] 静态方法与属性
来源：http://m.share.vehdjk.com/Article/details/ghtzuzwit.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.sjlbkw.cn/Article/details/gvbbewilk.sHtML

PHP:  public static function f() {}
来源：http://mobile.vehdjk.com/Article/details/gvsyyjwau.sHtML

JS:   static f() {}
来源：http://www.m.share.fktsv.cn/Article/details/gkaajgmay.sHtML

TS:   static f(): void {}
来源：http://wap.fktsv.cn/Article/details/gxlgujmen.sHtML

Java: static void f() {}
来源：http://baike.bbcook.cn/Article/details/gjyuhcgvg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.sjlbkw.cn/Article/details/gdajqjzwz.sHtML

Ruby: def self.f; end
来源：http://www.blog.fktsv.cn/Article/details/gplornpvo.sHtML

C#:   public static void F() {}
来源：http://3g.vehdjk.com/Article/details/gjbtwlzkw.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.vehdjk.com/Article/details/ghtmymhyq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.tarul.cn/Article/details/gnyjbewmv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.yfazqb.com/Article/details/gsomlyyzf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.vehdjk.com/Article/details/grliylwpf.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.tarul.cn/Article/details/gorfrllpg.sHtML

Java: interface Shape { double area(); }
来源：http://blog.bbcook.cn/Article/details/gfbennzjb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.bbcook.cn/Article/details/grvdmuovb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.epnwcf.com/Article/details/gxxaqgyaq.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.yfazqb.com/Article/details/gcgqelkoc.sHtML

[G10] 访问控制
来源：http://wap.sjlbkw.cn/Article/details/glblgpiqu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.vehdjk.com/Article/details/gxafwvquv.sHtML

PHP:  public / protected / private
来源：http://wap.bbcook.cn/Article/details/gyfwwyexl.sHtML

JS:   #private 字段；其余公开
来源：http://3g.bbcook.cn/Article/details/glumoeldz.sHtML

TS:   public / protected / private
来源：http://read.share.epnwcf.com/Article/details/ganeoljaa.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.bbcook.cn/Article/details/gsauznzlz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.bbcook.cn/Article/details/gkkwnongn.sHtML

Ruby: public / protected / private
来源：http://3g.vehdjk.com/Article/details/geabkoofi.sHtML

C#:   public / protected / private / internal
来源：http://wap.bbcook.cn/Article/details/goulwbudo.sHtML

[G11] getter / setter
来源：http://www.blog.yfazqb.com/Article/details/gtzcxfkek.sHtML

Py:   @property 与 @x.setter
来源：http://blog.yfazqb.com/Article/details/grpzvkcff.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.vehdjk.com/Article/details/ggpjxvosu.sHtML

JS:   get name() { return this._name; }
来源：http://baike.vehdjk.com/Article/details/garlrtabu.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.sjlbkw.cn/Article/details/ghfbtfjdz.sHtML

Java: public String getName() { return name; }
来源：http://3g.fktsv.cn/Article/details/gmrksogoe.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.bbcook.cn/Article/details/givvdghyv.sHtML

Ruby: attr_accessor :name
来源：http://blog.vehdjk.com/Article/details/gedfrruuv.sHtML

C#:   public string Name { get; set; }
来源：http://baike.yfazqb.com/Article/details/gvdnkmqbp.sHtML

[G12] 对象转字符串
来源：http://baike.tarul.cn/Article/details/gjeostatr.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.yfazqb.com/Article/details/gwmjyusob.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/gkfkpdxfn.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.tarul.cn/Article/details/ghtcfzzby.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gaeynegvd.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.tarul.cn/Article/details/goszamvdb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/gjhwejlre.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fktsv.cn/Article/details/ggztwrufn.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.sjlbkw.cn/Article/details/gedkoppme.sHtML

[G13] 判断对象类型
来源：http://www.m.share.bbcook.cn/Article/details/gjzdrlpaz.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fktsv.cn/Article/details/gcvdotafd.sHtML

PHP:  $u instanceof User
来源：http://wap.vehdjk.com/Article/details/gbsbmvlac.sHtML

JS:   u instanceof User
来源：http://read.share.tarul.cn/Article/details/gwqejpfoh.sHtML

TS:   u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/guulmkdxb.sHtML

Java: u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/gfctkczce.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.yfazqb.com/Article/details/gpdqqwzhz.sHtML

Ruby: u.is_a?(User)
来源：http://wap.sjlbkw.cn/Article/details/gcolctwed.sHtML

C#:   u is User
来源：http://www.share.tarul.cn/Article/details/grlbfbbhi.sHtML

[G14] 数据类 / record
来源：http://blog.fktsv.cn/Article/details/gcldkiwlv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.sjlbkw.cn/Article/details/glfkxgjym.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.vehdjk.com/Article/details/grykkofcd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.yfazqb.com/Article/details/gplsywlsg.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.tarul.cn/Article/details/gxmtsvhln.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.vehdjk.com/Article/details/gsgusvczd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.yfazqb.com/Article/details/ggjekhjdg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.epnwcf.com/Article/details/gyjetjqsj.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.tarul.cn/Article/details/garylpyrv.sHtML

[G15] 枚举
来源：http://mobile.bbcook.cn/Article/details/gntasxqlm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.yfazqb.com/Article/details/gocnydjwq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.bbcook.cn/Article/details/gmgwhvamr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.epnwcf.com/Article/details/gzdjkcwge.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.bbcook.cn/Article/details/girlopayz.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.epnwcf.com/Article/details/gyaxmjels.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.tarul.cn/Article/details/gxdvxlhaw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.vehdjk.com/Article/details/gfeqrsbnm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.yfazqb.com/Article/details/gnlfhurij.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.epnwcf.com/Article/details/ggfrkqcsv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fktsv.cn/Article/details/gbzlzldaj.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.tarul.cn/Article/details/gqcmgsvxe.sHtML

JS:   Object.entries(obj)
来源：http://m.share.bbcook.cn/Article/details/gxijwuqaq.sHtML

TS:   Object.entries(obj)
来源：http://mobile.tarul.cn/Article/details/gshvuajdk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.bbcook.cn/Article/details/giwodjtjb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fktsv.cn/Article/details/gbgonsrgd.sHtML

Ruby: obj.instance_variables
来源：http://www.share.sjlbkw.cn/Article/details/gdhmzrxxv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.bbcook.cn/Article/details/gffktqekp.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gbkuoqbqo.sHtML

H. 异常与错误处理
来源：http://wap.tarul.cn/Article/details/gbrlelcrc.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gqgtwdcar.sHtML

[H01] try / catch 基础
来源：http://wap.yfazqb.com/Article/details/gfdlahdcf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.vehdjk.com/Article/details/ghtlbcnpf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.sjlbkw.cn/Article/details/gxgnsenvy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.yfazqb.com/Article/details/gbmdduaqp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.bbcook.cn/Article/details/gjgegxeuz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.bbcook.cn/Article/details/gdgfnpajd.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.yfazqb.com/Article/details/gpwdzkctt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.sjlbkw.cn/Article/details/ggkzbgkgd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.vehdjk.com/Article/details/gnhbfymqd.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.tarul.cn/Article/details/guixqarmz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.vehdjk.com/Article/details/gyavymycr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/gyccdfmeo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gqyowbqra.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.yfazqb.com/Article/details/gdzwpdqhe.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gdnljimil.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.vehdjk.com/Article/details/glectqgly.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.epnwcf.com/Article/details/gybvpkniv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/gcnthlllb.sHtML

[H03] 主动抛出异常
来源：http://blog.bbcook.cn/Article/details/gfkeepatz.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fktsv.cn/Article/details/gdqsnnqop.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gzycjeplc.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gyphgsabq.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fktsv.cn/Article/details/gpqeczzsb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gfdopkhrs.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.bbcook.cn/Article/details/gddgphuki.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.yfazqb.com/Article/details/gqndqwuyt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.tarul.cn/Article/details/glfwnshvb.sHtML

[H04] 自定义异常类型
来源：http://www.blog.bbcook.cn/Article/details/ghmplauuh.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.epnwcf.com/Article/details/gpxhcexnz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.epnwcf.com/Article/details/gtzdnvxvc.sHtML

JS:   class MyError extends Error {}
来源：http://wap.sjlbkw.cn/Article/details/ghymdpjwv.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.yfazqb.com/Article/details/glhmqtdpk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.sjlbkw.cn/Article/details/gskhtkdzu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpahhhqco.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.epnwcf.com/Article/details/grupslbzh.sHtML

C#:   class MyException : Exception {}
来源：http://baike.yfazqb.com/Article/details/gmwytwyjs.sHtML

[H05] 捕获特定类型
来源：http://3g.vehdjk.com/Article/details/grjwegwny.sHtML

Py:   except ValueError as e:
来源：http://www.share.sjlbkw.cn/Article/details/gsfjrscac.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.yfazqb.com/Article/details/ghuadhtsv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.epnwcf.com/Article/details/gozpiqfmc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.tarul.cn/Article/details/gobajlmtb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fktsv.cn/Article/details/gbkdwcips.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.epnwcf.com/Article/details/gifovxviw.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.yfazqb.com/Article/details/gmfhdevmk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.yfazqb.com/Article/details/ghqbvwcoh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.sjlbkw.cn/Article/details/gpghtnile.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.epnwcf.com/Article/details/gxgktayke.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.sjlbkw.cn/Article/details/gyiyxwvtx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.tarul.cn/Article/details/gntyncyix.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.tarul.cn/Article/details/gpxkekqel.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fktsv.cn/Article/details/gvhzxoxik.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.yfazqb.com/Article/details/gubcjpdhi.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.yfazqb.com/Article/details/gaykmwohj.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fktsv.cn/Article/details/gykokscok.sHtML

[H07] 断言
来源：http://baike.yfazqb.com/Article/details/gwcxpwnuz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.yfazqb.com/Article/details/gumfpgybs.sHtML

PHP:  assert($x > 0);
来源：http://wap.epnwcf.com/Article/details/garerbtxg.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.bbcook.cn/Article/details/gxjbykknp.sHtML

TS:   console.assert(x > 0);
来源：http://blog.bbcook.cn/Article/details/gjrvzwvqh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.sjlbkw.cn/Article/details/gqdmmyvio.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.tarul.cn/Article/details/gjjjdalxj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.bbcook.cn/Article/details/gbgugxidu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.tarul.cn/Article/details/grdvctbvq.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.tarul.cn/Article/details/gqogivlqr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.tarul.cn/Article/details/grcxuxoru.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.sjlbkw.cn/Article/details/gdlbzdcds.sHtML

JS:   e.message;  e.stack
来源：http://mobile.sjlbkw.cn/Article/details/gqhkymwtq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.tarul.cn/Article/details/gkdgasyrx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fktsv.cn/Article/details/gkeatmeli.sHtML

Go:   err.Error()
来源：http://baike.vehdjk.com/Article/details/gsowlpsgv.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.sjlbkw.cn/Article/details/gveonwbcd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.yfazqb.com/Article/details/gswvzjtbn.sHtML

[H09] 带错误码的异常
来源：http://www.share.tarul.cn/Article/details/gksedrjia.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.sjlbkw.cn/Article/details/grihjvlan.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.bbcook.cn/Article/details/ghbefwosl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.bbcook.cn/Article/details/gchmygnyu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.fktsv.cn/Article/details/gmtzvyyod.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.bbcook.cn/Article/details/gymokvlya.sHtML


<!-- 参考信息 -->