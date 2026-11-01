代发 wailian999

Ruby: File.delete("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/glhvnstqg.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.yfazqb.com/Article/details/glbalrwry.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.epnwcf.com/Article/details/gnpfivthn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.vehdjk.com/Article/details/gfbcmcwip.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fktsv.cn/Article/details/ggycfvjti.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.sjlbkw.cn/Article/details/gudfkgpso.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.epnwcf.com/Article/details/geckmgmwj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.bbcook.cn/Article/details/gmkuufwur.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.sjlbkw.cn/Article/details/ggxrnmyap.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.yfazqb.com/Article/details/gmlbsoyce.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.vehdjk.com/Article/details/gtixoboak.sHtML

[F08] 遍历目录
来源：http://mobile.yfazqb.com/Article/details/gnsmmwikd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.epnwcf.com/Article/details/ghueplohq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fktsv.cn/Article/details/gmitiwsye.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gkialynib.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.sjlbkw.cn/Article/details/gofhmzoyp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.yfazqb.com/Article/details/gatvuxlza.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.tarul.cn/Article/details/gdvmchdcc.sHtML

Ruby: Dir.children("dir")
来源：http://3g.yfazqb.com/Article/details/gljrpzlew.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.tarul.cn/Article/details/gxpgprxkp.sHtML

[F09] 获取文件大小
来源：http://wap.bbcook.cn/Article/details/gimfnvavw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gaxsznqms.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gossrbwvs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.tarul.cn/Article/details/gyegkhmbn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.epnwcf.com/Article/details/geqxcqvez.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/gabqhrlrw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.sjlbkw.cn/Article/details/grihzdzxw.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gvxbwovel.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.yfazqb.com/Article/details/gnaspoitv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.epnwcf.com/Article/details/gtjixqatc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gdqengokl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fktsv.cn/Article/details/ggwncmnzy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gjolkijan.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gctnfbxac.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.epnwcf.com/Article/details/gzfbkefvl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gnygetlgw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/ghschmrso.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gqlndbojv.sHtML

[F11] 复制与移动文件
来源：http://mobile.epnwcf.com/Article/details/glwcmrnuu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.bbcook.cn/Article/details/giuaqcniu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.yfazqb.com/Article/details/gdvxfjhrx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/ggkkrksdi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gfolvtogf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.tarul.cn/Article/details/godisrskl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.sjlbkw.cn/Article/details/gfkrtjmuw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/guaybizwp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.bbcook.cn/Article/details/gkfouongo.sHtML

[F12] CSV 读写
来源：http://baike.vehdjk.com/Article/details/gjxoocwyi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.bbcook.cn/Article/details/gibwtkwar.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.tarul.cn/Article/details/gkyyxunby.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.sjlbkw.cn/Article/details/gmcuxshvg.sHtML

TS:   // 同上
来源：http://m.share.tarul.cn/Article/details/gyskdohey.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.epnwcf.com/Article/details/gtdcupdad.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.vehdjk.com/Article/details/gjnrjwktz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.vehdjk.com/Article/details/gtkquobfh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.bbcook.cn/Article/details/gpjrcaniq.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gvbygwvss.sHtML

G. 面向对象
来源：http://blog.sjlbkw.cn/Article/details/gvzcsgkpq.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gjmxqtknz.sHtML

[G01] 定义类
来源：http://blog.vehdjk.com/Article/details/gszlibbxm.sHtML

Py:   class User: pass
来源：http://www.share.vehdjk.com/Article/details/gndakzpra.sHtML

PHP:  class User {}
来源：http://blog.vehdjk.com/Article/details/gzjwutsjz.sHtML

JS:   class User {}
来源：http://mobile.fktsv.cn/Article/details/ggahlknvu.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.tarul.cn/Article/details/gnrzrymwb.sHtML

Java: class User {}
来源：http://m.share.fktsv.cn/Article/details/gxkfeafdj.sHtML

Go:   type User struct { Name string }
来源：http://www.share.vehdjk.com/Article/details/gaxurqchh.sHtML

Ruby: class User; end
来源：http://www.share.epnwcf.com/Article/details/gsnrdgzhy.sHtML

C#:   class User {}
来源：http://www.m.share.yfazqb.com/Article/details/ggxmwkecp.sHtML

[G02] 构造函数
来源：http://www.m.share.vehdjk.com/Article/details/ggnziylty.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fktsv.cn/Article/details/gzvswvumx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.epnwcf.com/Article/details/gijhgszaa.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/gyepsdgxa.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fktsv.cn/Article/details/gwtdnlrsq.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.vehdjk.com/Article/details/gnoocdrqa.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.sjlbkw.cn/Article/details/gceedsrlh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.epnwcf.com/Article/details/gmrgyegah.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fktsv.cn/Article/details/ghnjcjbnn.sHtML

[G03] 实例属性
来源：http://www.blog.tarul.cn/Article/details/gecvideat.sHtML

Py:   self.name = "x"
来源：http://read.share.sjlbkw.cn/Article/details/gudazvbej.sHtML

PHP:  public string $name = "x";
来源：http://www.share.yfazqb.com/Article/details/geyvfynwz.sHtML

JS:   this.name = "x";
来源：http://www.m.share.vehdjk.com/Article/details/grapgkevx.sHtML

TS:   name: string = "x";
来源：http://wap.sjlbkw.cn/Article/details/gctjqhbpc.sHtML

Java: private String name;
来源：http://blog.bbcook.cn/Article/details/ghnietvuj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.epnwcf.com/Article/details/gdhcdsyux.sHtML

Ruby: @name = "x"
来源：http://www.blog.epnwcf.com/Article/details/giebyohia.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.sjlbkw.cn/Article/details/gdfzyzpnm.sHtML

[G04] 定义方法
来源：http://www.share.yfazqb.com/Article/details/gyalhuktj.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.tarul.cn/Article/details/gzelrarvo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gkmhqjcgh.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxaxsxblg.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/gmiolqzwr.sHtML

Java: String greet() { return name; }
来源：http://3g.tarul.cn/Article/details/gsfzkjxdi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fktsv.cn/Article/details/gbdbeeerf.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.vehdjk.com/Article/details/gqwlngdkc.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.vehdjk.com/Article/details/gcpxsrfoo.sHtML

[G05] 继承
来源：http://wap.sjlbkw.cn/Article/details/gmzdsdtax.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.vehdjk.com/Article/details/gqvuxstoo.sHtML

PHP:  class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/gsacdrjko.sHtML

JS:   class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gbryywbih.sHtML

TS:   class Admin extends User {}
来源：http://www.share.vehdjk.com/Article/details/gorpsftdo.sHtML

Java: class Admin extends User {}
来源：http://www.blog.epnwcf.com/Article/details/gglwfrrbj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fktsv.cn/Article/details/gnpdgzjyp.sHtML

Ruby: class Admin < User; end
来源：http://3g.yfazqb.com/Article/details/gxqajslgw.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnsjibuq.sHtML

[G06] 重写方法
来源：http://3g.yfazqb.com/Article/details/gihtjcfao.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.bbcook.cn/Article/details/gtwhloxyb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.tarul.cn/Article/details/gzdsfuoqp.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gpojtxppi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/ginsvdnbj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/gjmgqnlwz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.bbcook.cn/Article/details/gzcjcppjz.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.bbcook.cn/Article/details/gshjhwhlg.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.epnwcf.com/Article/details/gelsoxjix.sHtML

[G07] 调用父类方法
来源：http://baike.vehdjk.com/Article/details/gsvcpnxzs.sHtML

Py:   super().greet()
来源：http://baike.bbcook.cn/Article/details/gsfszsfoc.sHtML

PHP:  parent::greet();
来源：http://blog.sjlbkw.cn/Article/details/gcdzcczzo.sHtML

JS:   super.greet();
来源：http://m.share.fktsv.cn/Article/details/gzpibykxb.sHtML

TS:   super.greet();
来源：http://m.share.sjlbkw.cn/Article/details/gphlbfugk.sHtML

Java: super.greet();
来源：http://www.share.yfazqb.com/Article/details/grbtvtayr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.sjlbkw.cn/Article/details/ghyyopksr.sHtML

Ruby: super
来源：http://blog.vehdjk.com/Article/details/gufoqtdpa.sHtML

C#:   base.Greet();
来源：http://wap.tarul.cn/Article/details/gxrvlmsxx.sHtML

[G08] 静态方法与属性
来源：http://read.share.bbcook.cn/Article/details/gmzfdzthf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.yfazqb.com/Article/details/gggvhnobq.sHtML

PHP:  public static function f() {}
来源：http://read.share.sjlbkw.cn/Article/details/gpfhndlzb.sHtML

JS:   static f() {}
来源：http://3g.vehdjk.com/Article/details/ggskrcehf.sHtML

TS:   static f(): void {}
来源：http://wap.epnwcf.com/Article/details/gochyszsp.sHtML

Java: static void f() {}
来源：http://3g.vehdjk.com/Article/details/gcwrcmtbn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fktsv.cn/Article/details/glvdgddxr.sHtML

Ruby: def self.f; end
来源：http://mobile.epnwcf.com/Article/details/gprctqbul.sHtML

C#:   public static void F() {}
来源：http://blog.fktsv.cn/Article/details/gqtfwbacq.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fktsv.cn/Article/details/gaddoiamo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.yfazqb.com/Article/details/gelkouimi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.vehdjk.com/Article/details/gvqttzzod.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.epnwcf.com/Article/details/godejpudb.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.bbcook.cn/Article/details/gimrlrldq.sHtML

Java: interface Shape { double area(); }
来源：http://baike.bbcook.cn/Article/details/gafopqney.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.bbcook.cn/Article/details/gdqibiblb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.bbcook.cn/Article/details/grpsysjza.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.yfazqb.com/Article/details/gvfvnadgx.sHtML

[G10] 访问控制
来源：http://wap.sjlbkw.cn/Article/details/gkphdzfoi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fktsv.cn/Article/details/gwtbfhrzi.sHtML

PHP:  public / protected / private
来源：http://read.share.tarul.cn/Article/details/gdyymllxp.sHtML

JS:   #private 字段；其余公开
来源：http://wap.bbcook.cn/Article/details/gplqkjvdb.sHtML

TS:   public / protected / private
来源：http://baike.fktsv.cn/Article/details/gigbbjfxo.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.sjlbkw.cn/Article/details/ggndcwcpb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.vehdjk.com/Article/details/goknicmwh.sHtML

Ruby: public / protected / private
来源：http://wap.vehdjk.com/Article/details/gnxvydlgb.sHtML

C#:   public / protected / private / internal
来源：http://3g.epnwcf.com/Article/details/gqkkkcixh.sHtML

[G11] getter / setter
来源：http://baike.yfazqb.com/Article/details/gbqrfesln.sHtML

Py:   @property 与 @x.setter
来源：http://3g.vehdjk.com/Article/details/gbruojtxf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.tarul.cn/Article/details/golejjbkw.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.tarul.cn/Article/details/gtvbyxhei.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.epnwcf.com/Article/details/gooarcelr.sHtML

Java: public String getName() { return name; }
来源：http://blog.fktsv.cn/Article/details/gvkkbdlep.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.vehdjk.com/Article/details/guvvwdduo.sHtML

Ruby: attr_accessor :name
来源：http://baike.fktsv.cn/Article/details/gmhnedjgs.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.epnwcf.com/Article/details/gcngbqctj.sHtML

[G12] 对象转字符串
来源：http://wap.fktsv.cn/Article/details/gawcyyxya.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.bbcook.cn/Article/details/gyjzfqfpp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.bbcook.cn/Article/details/gkhvntmzr.sHtML

JS:   toString() { return this.name; }
来源：http://baike.yfazqb.com/Article/details/gzhixcfll.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.sjlbkw.cn/Article/details/gmglyhhwv.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gytchpldy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.yfazqb.com/Article/details/gifnaufli.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.tarul.cn/Article/details/gtbrmezhx.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.vehdjk.com/Article/details/gawzzdrwf.sHtML

[G13] 判断对象类型
来源：http://www.blog.yfazqb.com/Article/details/ggxvcfnsi.sHtML

Py:   isinstance(u, User)
来源：http://blog.sjlbkw.cn/Article/details/gdkqurfwt.sHtML

PHP:  $u instanceof User
来源：http://read.share.tarul.cn/Article/details/ggmzitudl.sHtML

JS:   u instanceof User
来源：http://mobile.epnwcf.com/Article/details/gnxmetkok.sHtML

TS:   u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/gxwpxfhio.sHtML

Java: u instanceof User
来源：http://3g.sjlbkw.cn/Article/details/gbfjvfgex.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.bbcook.cn/Article/details/gzkxorwdv.sHtML

Ruby: u.is_a?(User)
来源：http://blog.bbcook.cn/Article/details/gwtsplwhl.sHtML

C#:   u is User
来源：http://www.share.fktsv.cn/Article/details/gqqxpfoxn.sHtML

[G14] 数据类 / record
来源：http://wap.tarul.cn/Article/details/gqizptxid.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.bbcook.cn/Article/details/gcpkypwwl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fktsv.cn/Article/details/glnhadhzm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.yfazqb.com/Article/details/gmoobxrcd.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.sjlbkw.cn/Article/details/gjzcaubbq.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.tarul.cn/Article/details/gthigkkda.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.sjlbkw.cn/Article/details/gertrlpjg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.sjlbkw.cn/Article/details/glrblrjrs.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.vehdjk.com/Article/details/gzpdbniqw.sHtML

[G15] 枚举
来源：http://m.share.fktsv.cn/Article/details/gqiolicjb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.sjlbkw.cn/Article/details/gltrjshcv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.bbcook.cn/Article/details/gxehpphlu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.vehdjk.com/Article/details/gkreuxmva.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.epnwcf.com/Article/details/glmkxmpwm.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.vehdjk.com/Article/details/gkjhqsizi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fktsv.cn/Article/details/goubyhkio.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.epnwcf.com/Article/details/gbsxpxlui.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.vehdjk.com/Article/details/grauqpfab.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.tarul.cn/Article/details/gdjscglkt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.sjlbkw.cn/Article/details/gahukpvpr.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.tarul.cn/Article/details/glxuutzxw.sHtML

JS:   Object.entries(obj)
来源：http://wap.sjlbkw.cn/Article/details/gzfqsdiqd.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/giqwnngfx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.tarul.cn/Article/details/gbvjyxewp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fktsv.cn/Article/details/gjtrnmbvc.sHtML

Ruby: obj.instance_variables
来源：http://mobile.yfazqb.com/Article/details/gqivpungg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.bbcook.cn/Article/details/gvqicqmjc.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gqfwqymmf.sHtML

H. 异常与错误处理
来源：http://www.share.yfazqb.com/Article/details/gryjqhheo.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gzycnvoan.sHtML

[H01] try / catch 基础
来源：http://wap.yfazqb.com/Article/details/gkbhqfxdk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fktsv.cn/Article/details/gcwihksfo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.bbcook.cn/Article/details/ggiqrytzo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.bbcook.cn/Article/details/gceqltffe.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.bbcook.cn/Article/details/gislqyjls.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.epnwcf.com/Article/details/gdzjnfjxw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fktsv.cn/Article/details/gyvfuoacq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fktsv.cn/Article/details/gqveaofzn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.tarul.cn/Article/details/gtvdddeng.sHtML

[H02] finally / ensure 收尾
来源：http://blog.bbcook.cn/Article/details/ghymlxqob.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.bbcook.cn/Article/details/grbxzvhik.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gpwkhqwnt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gtwhmsgio.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/ghcwryjbg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gfziqceyk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.tarul.cn/Article/details/gcbgxqtyn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.yfazqb.com/Article/details/gavdwjfxv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.epnwcf.com/Article/details/gjweitwfs.sHtML

[H03] 主动抛出异常
来源：http://www.blog.yfazqb.com/Article/details/gmdvlhldy.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.epnwcf.com/Article/details/gawgiwhkj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/gdxmklxts.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/gmejzjzwh.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.tarul.cn/Article/details/ghwopzeov.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.vehdjk.com/Article/details/gqsqouhdg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.epnwcf.com/Article/details/grewhdike.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.sjlbkw.cn/Article/details/geqjpufix.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gsqbtjvsb.sHtML

[H04] 自定义异常类型
来源：http://3g.yfazqb.com/Article/details/genyzklkv.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fktsv.cn/Article/details/ghsekcfhs.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.epnwcf.com/Article/details/gekfrlyyt.sHtML

JS:   class MyError extends Error {}
来源：http://3g.epnwcf.com/Article/details/gcxjcolov.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.vehdjk.com/Article/details/gdxshrmxx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.bbcook.cn/Article/details/gqnktopgz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.sjlbkw.cn/Article/details/ghxisjblo.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.vehdjk.com/Article/details/grkhblolq.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.vehdjk.com/Article/details/ggtvffvws.sHtML

[H05] 捕获特定类型
来源：http://www.blog.vehdjk.com/Article/details/gyowemdsn.sHtML

Py:   except ValueError as e:
来源：http://read.share.bbcook.cn/Article/details/giptpdddi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.yfazqb.com/Article/details/gjgelxyup.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.bbcook.cn/Article/details/gumvvesip.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fktsv.cn/Article/details/gvepaobip.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.sjlbkw.cn/Article/details/gofaofqzx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.bbcook.cn/Article/details/gbqbnlkar.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fktsv.cn/Article/details/gamfvzuaw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.epnwcf.com/Article/details/gtyxxgxyn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.epnwcf.com/Article/details/gtcwylqrx.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.epnwcf.com/Article/details/gzsxuhgdn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.bbcook.cn/Article/details/ghwwjujnq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.vehdjk.com/Article/details/gxekhzbwq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.yfazqb.com/Article/details/gycgmrbux.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.epnwcf.com/Article/details/gagrqieyz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.epnwcf.com/Article/details/goszwxgrt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.yfazqb.com/Article/details/ghrqqupjq.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.sjlbkw.cn/Article/details/gbtslyprn.sHtML

[H07] 断言
来源：http://www.share.bbcook.cn/Article/details/ggqhfkjgb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.vehdjk.com/Article/details/grezniwgr.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.tarul.cn/Article/details/gogzuujfm.sHtML

JS:   console.assert(x > 0);
来源：http://3g.yfazqb.com/Article/details/ggpjxqwdr.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.vehdjk.com/Article/details/gcodbhlpa.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.yfazqb.com/Article/details/gzptncpno.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.tarul.cn/Article/details/gusgrlpiq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.sjlbkw.cn/Article/details/ghvbwiicd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.vehdjk.com/Article/details/gxstddqkv.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.epnwcf.com/Article/details/gszhhwmko.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.tarul.cn/Article/details/gemnxkudz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.tarul.cn/Article/details/gjonmpqev.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fktsv.cn/Article/details/gpwnkwehk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.vehdjk.com/Article/details/gfgczuklb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fktsv.cn/Article/details/guptztjpr.sHtML

Go:   err.Error()
来源：http://www.m.share.sjlbkw.cn/Article/details/gvswagkcl.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.tarul.cn/Article/details/ghzcezruo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.epnwcf.com/Article/details/gtqmhwkgu.sHtML

[H09] 带错误码的异常
来源：http://3g.vehdjk.com/Article/details/gtilavnvo.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.bbcook.cn/Article/details/gimlmyrwp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fktsv.cn/Article/details/gsskusasd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.epnwcf.com/Article/details/gjslcnwjw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.bbcook.cn/Article/details/gjlhuffiv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.tarul.cn/Article/details/glzzagilt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.bbcook.cn/Article/details/gkuskrcns.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fktsv.cn/Article/details/grkeqggey.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fktsv.cn/Article/details/gsgcqivdt.sHtML

[H10] 资源自动释放
来源：http://blog.epnwcf.com/Article/details/gttoxbhxq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.vehdjk.com/Article/details/gygyrhbhp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.yfazqb.com/Article/details/gkahwyhtz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.epnwcf.com/Article/details/gehgjihnl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.vehdjk.com/Article/details/glksbzeqx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.bbcook.cn/Article/details/ghpbinmjr.sHtML

Go:   defer f.Close()
来源：http://www.share.bbcook.cn/Article/details/gvfvjcelu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.epnwcf.com/Article/details/gqvxrroow.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gguuefvxt.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gdwwzbhcy.sHtML

I. 正则表达式
来源：http://m.share.vehdjk.com/Article/details/gktuthfmb.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/ggogytdnx.sHtML

[I01] 判断是否匹配
来源：http://wap.epnwcf.com/Article/details/gihsgawhy.sHtML


<!-- 参考信息 -->