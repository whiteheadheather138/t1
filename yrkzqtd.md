代发 wailian999

Ruby: File.delete("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gpnpvfkce.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gsyyxltef.sHtML

[F07] 创建目录（含多级）
来源：http://blog.tarul.cn/Article/details/gkklunhms.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.tarul.cn/Article/details/grzzahgnf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.bbcook.cn/Article/details/gsxcydsmu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.vehdjk.com/Article/details/guhathyml.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.tarul.cn/Article/details/gxqoleees.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.tarul.cn/Article/details/gtmsgoihy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.epnwcf.com/Article/details/gibheycil.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.epnwcf.com/Article/details/geutpnofu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.sjlbkw.cn/Article/details/gepsvxlpg.sHtML

[F08] 遍历目录
来源：http://m.share.epnwcf.com/Article/details/gbytjiyjp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.bbcook.cn/Article/details/gcnrtmkqm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.tarul.cn/Article/details/gusbhvauu.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.epnwcf.com/Article/details/gkzsixhse.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.epnwcf.com/Article/details/gzemnntis.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.sjlbkw.cn/Article/details/gsmfjoikk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.vehdjk.com/Article/details/grqfgmayj.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.vehdjk.com/Article/details/gvhkjmxly.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fktsv.cn/Article/details/gyxtvgokv.sHtML

[F09] 获取文件大小
来源：http://mobile.epnwcf.com/Article/details/gnhwtbfsd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gkzrwwcfq.sHtML

PHP:  filesize("a.txt");
来源：http://3g.epnwcf.com/Article/details/glcgrlxmz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.yfazqb.com/Article/details/gctqbberd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.bbcook.cn/Article/details/gtiihcniz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.bbcook.cn/Article/details/glrlrgtwo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.yfazqb.com/Article/details/geadanmmr.sHtML

Ruby: File.size("a.txt")
来源：http://wap.epnwcf.com/Article/details/gbyamiywm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.sjlbkw.cn/Article/details/gosccumcp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.epnwcf.com/Article/details/goxbzgfdg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gmpbiblqv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.vehdjk.com/Article/details/gatpfbvdz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/ghirbtzzp.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.tarul.cn/Article/details/gtlqclfjs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.tarul.cn/Article/details/gfxsurkib.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gdplsrlyj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gabhwnkvm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gmfiyykaf.sHtML

[F11] 复制与移动文件
来源：http://blog.bbcook.cn/Article/details/gujoaxitd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gobrwikip.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.yfazqb.com/Article/details/gejyefloi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.vehdjk.com/Article/details/ggjdydqqc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gddcydjcz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.yfazqb.com/Article/details/gcuspchpe.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.tarul.cn/Article/details/gwwpzjnuk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/gdmscnsad.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.epnwcf.com/Article/details/gcriejitb.sHtML

[F12] CSV 读写
来源：http://www.share.yfazqb.com/Article/details/giwwhvowm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.tarul.cn/Article/details/gvfvcxrbf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.sjlbkw.cn/Article/details/ggdijpexa.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.vehdjk.com/Article/details/gzhmnprqu.sHtML

TS:   // 同上
来源：http://blog.vehdjk.com/Article/details/grmyvmkrg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.bbcook.cn/Article/details/gxgjgsdrw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.bbcook.cn/Article/details/gzqeuswhm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.tarul.cn/Article/details/gdqcazvuj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.sjlbkw.cn/Article/details/gtfuoaqtf.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gzuezhlix.sHtML

G. 面向对象
来源：http://mobile.yfazqb.com/Article/details/gylmtcwls.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/grypepefh.sHtML

[G01] 定义类
来源：http://read.share.sjlbkw.cn/Article/details/gtepgvxhw.sHtML

Py:   class User: pass
来源：http://blog.yfazqb.com/Article/details/gyvndxwgh.sHtML

PHP:  class User {}
来源：http://www.blog.vehdjk.com/Article/details/gvlrngfpe.sHtML

JS:   class User {}
来源：http://www.share.yfazqb.com/Article/details/giqovjfpf.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghgepejtn.sHtML

Java: class User {}
来源：http://m.share.tarul.cn/Article/details/gkzfkcmtf.sHtML

Go:   type User struct { Name string }
来源：http://wap.vehdjk.com/Article/details/gxgjpxwne.sHtML

Ruby: class User; end
来源：http://3g.fktsv.cn/Article/details/ggsqsyeer.sHtML

C#:   class User {}
来源：http://www.m.share.vehdjk.com/Article/details/gxfwfieuf.sHtML

[G02] 构造函数
来源：http://blog.fktsv.cn/Article/details/gbgxepxhp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.bbcook.cn/Article/details/gfeockyhf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.bbcook.cn/Article/details/glqnqzwxi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.tarul.cn/Article/details/gmyupwsse.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.epnwcf.com/Article/details/gsjrmgirj.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.vehdjk.com/Article/details/gnpddnfcl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.bbcook.cn/Article/details/gryukaejy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.yfazqb.com/Article/details/glvoemgfl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/glvtbexig.sHtML

[G03] 实例属性
来源：http://m.share.sjlbkw.cn/Article/details/gownhjuxq.sHtML

Py:   self.name = "x"
来源：http://m.share.fktsv.cn/Article/details/gminyzobq.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fktsv.cn/Article/details/gqgcthbio.sHtML

JS:   this.name = "x";
来源：http://wap.fktsv.cn/Article/details/gtaotfrlf.sHtML

TS:   name: string = "x";
来源：http://baike.bbcook.cn/Article/details/gksyfeqwz.sHtML

Java: private String name;
来源：http://m.share.tarul.cn/Article/details/gyisbpwid.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.yfazqb.com/Article/details/gylgcbywj.sHtML

Ruby: @name = "x"
来源：http://3g.sjlbkw.cn/Article/details/gbinnmffg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.bbcook.cn/Article/details/giizwpkdz.sHtML

[G04] 定义方法
来源：http://wap.epnwcf.com/Article/details/gcdfrcvzd.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fktsv.cn/Article/details/gxcburrsh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/gnwpxbkny.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/gkqbatamy.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.bbcook.cn/Article/details/ghwiuqowf.sHtML

Java: String greet() { return name; }
来源：http://3g.tarul.cn/Article/details/githcpcmm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.tarul.cn/Article/details/ggwxviplg.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fktsv.cn/Article/details/gzzteshbg.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.vehdjk.com/Article/details/ghznpezql.sHtML

[G05] 继承
来源：http://mobile.vehdjk.com/Article/details/guqsndvgl.sHtML

Py:   class Admin(User): pass
来源：http://wap.fktsv.cn/Article/details/gdhjxssvh.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gaykpsmmj.sHtML

JS:   class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gtjybjjna.sHtML

TS:   class Admin extends User {}
来源：http://m.share.epnwcf.com/Article/details/gtplkofen.sHtML

Java: class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/gbxtqinig.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.sjlbkw.cn/Article/details/gsbcfihnu.sHtML

Ruby: class Admin < User; end
来源：http://m.share.vehdjk.com/Article/details/gfttevfxb.sHtML

C#:   class Admin : User {}
来源：http://blog.yfazqb.com/Article/details/gksnfwxgv.sHtML

[G06] 重写方法
来源：http://www.m.share.bbcook.cn/Article/details/gtyeywojc.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.bbcook.cn/Article/details/gwznbfgfp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.tarul.cn/Article/details/ghucgiydf.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/grvxznckk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/gtetbwvqq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.sjlbkw.cn/Article/details/grxiyfrkl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.bbcook.cn/Article/details/gnncxrdbd.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fktsv.cn/Article/details/gonbskjsg.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.bbcook.cn/Article/details/glzmiyehx.sHtML

[G07] 调用父类方法
来源：http://wap.tarul.cn/Article/details/gffpasdwj.sHtML

Py:   super().greet()
来源：http://wap.bbcook.cn/Article/details/gfczljwtm.sHtML

PHP:  parent::greet();
来源：http://www.m.share.vehdjk.com/Article/details/gmdahcznh.sHtML

JS:   super.greet();
来源：http://blog.vehdjk.com/Article/details/gfzhjbspi.sHtML

TS:   super.greet();
来源：http://www.blog.bbcook.cn/Article/details/gspfmfgma.sHtML

Java: super.greet();
来源：http://www.share.yfazqb.com/Article/details/gehflquuk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.tarul.cn/Article/details/gwuvepqhz.sHtML

Ruby: super
来源：http://read.share.yfazqb.com/Article/details/gpwxfhvmt.sHtML

C#:   base.Greet();
来源：http://3g.bbcook.cn/Article/details/gxhspiqjr.sHtML

[G08] 静态方法与属性
来源：http://www.share.fktsv.cn/Article/details/glfeqfezw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.epnwcf.com/Article/details/gneoethvu.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.bbcook.cn/Article/details/gtzekgusl.sHtML

JS:   static f() {}
来源：http://read.share.yfazqb.com/Article/details/ghsvsgfca.sHtML

TS:   static f(): void {}
来源：http://read.share.bbcook.cn/Article/details/gllfiyprw.sHtML

Java: static void f() {}
来源：http://mobile.fktsv.cn/Article/details/gvcizhldo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.sjlbkw.cn/Article/details/gzbzrnxsg.sHtML

Ruby: def self.f; end
来源：http://blog.tarul.cn/Article/details/gnlsyzhqk.sHtML

C#:   public static void F() {}
来源：http://blog.vehdjk.com/Article/details/ggwdwrqhr.sHtML

[G09] 接口 / 抽象类
来源：http://3g.tarul.cn/Article/details/gvyttgamd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.vehdjk.com/Article/details/ghzaeezlk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.yfazqb.com/Article/details/gcqspkemd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.vehdjk.com/Article/details/gapnzblpx.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.tarul.cn/Article/details/gaennpnbj.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.yfazqb.com/Article/details/gzynvoykd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.vehdjk.com/Article/details/gxccohxik.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.vehdjk.com/Article/details/gicgoyswm.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.epnwcf.com/Article/details/gvqrllcjl.sHtML

[G10] 访问控制
来源：http://mobile.yfazqb.com/Article/details/gftjkdcdo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.sjlbkw.cn/Article/details/gtfmmzomk.sHtML

PHP:  public / protected / private
来源：http://mobile.yfazqb.com/Article/details/gfbspbxjg.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fktsv.cn/Article/details/gwcdnbdmm.sHtML

TS:   public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gojqicqhd.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.epnwcf.com/Article/details/gdhggtowc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.bbcook.cn/Article/details/gvsitcfjg.sHtML

Ruby: public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/gdinmgcho.sHtML

C#:   public / protected / private / internal
来源：http://m.share.yfazqb.com/Article/details/gbwsvfwtl.sHtML

[G11] getter / setter
来源：http://mobile.vehdjk.com/Article/details/glzhchslc.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fktsv.cn/Article/details/grhbpqnkh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/ghqmwzibg.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fktsv.cn/Article/details/gkdihtgki.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.yfazqb.com/Article/details/gwsuyambt.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fktsv.cn/Article/details/gnsblfbox.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.yfazqb.com/Article/details/gfqlhoiqv.sHtML

Ruby: attr_accessor :name
来源：http://baike.sjlbkw.cn/Article/details/glcnqcexz.sHtML

C#:   public string Name { get; set; }
来源：http://baike.yfazqb.com/Article/details/gaptflbsl.sHtML

[G12] 对象转字符串
来源：http://blog.epnwcf.com/Article/details/gjwqwqjci.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.vehdjk.com/Article/details/gpufcnukz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.tarul.cn/Article/details/ggpbvynxh.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/grqgfvahu.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/glbfyqdkt.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gyjxnzhtx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fktsv.cn/Article/details/gkxcbjxrw.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.vehdjk.com/Article/details/gxexwvkmz.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.epnwcf.com/Article/details/ghitwicdv.sHtML

[G13] 判断对象类型
来源：http://mobile.bbcook.cn/Article/details/gxwkubnzx.sHtML

Py:   isinstance(u, User)
来源：http://mobile.sjlbkw.cn/Article/details/gbwwwlvom.sHtML

PHP:  $u instanceof User
来源：http://wap.epnwcf.com/Article/details/gtafzqzzt.sHtML

JS:   u instanceof User
来源：http://blog.vehdjk.com/Article/details/gtidpcjcn.sHtML

TS:   u instanceof User
来源：http://read.share.tarul.cn/Article/details/gioxaaqhd.sHtML

Java: u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/gexpnrkjw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.bbcook.cn/Article/details/gqllchtir.sHtML

Ruby: u.is_a?(User)
来源：http://baike.vehdjk.com/Article/details/glpbzgwdi.sHtML

C#:   u is User
来源：http://www.share.vehdjk.com/Article/details/grhvfwije.sHtML

[G14] 数据类 / record
来源：http://mobile.tarul.cn/Article/details/gkwduffmy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.bbcook.cn/Article/details/gzspijccx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.bbcook.cn/Article/details/gjqvhkkbo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.epnwcf.com/Article/details/gbupvcoxt.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.tarul.cn/Article/details/gcwqevgya.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gophwtlbd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.yfazqb.com/Article/details/gcjbywscc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.vehdjk.com/Article/details/gbqpzpxdf.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.epnwcf.com/Article/details/gessvqvxr.sHtML

[G15] 枚举
来源：http://wap.sjlbkw.cn/Article/details/ggdjygmbq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.sjlbkw.cn/Article/details/gjikilpyl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.vehdjk.com/Article/details/gjfajraek.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.epnwcf.com/Article/details/gvomelpts.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.epnwcf.com/Article/details/gzhvmsehd.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.sjlbkw.cn/Article/details/gdstuinlb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.bbcook.cn/Article/details/gtvyrfxhp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.vehdjk.com/Article/details/gfoxcvazo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.vehdjk.com/Article/details/glaipuuwh.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.tarul.cn/Article/details/gpyizakit.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.yfazqb.com/Article/details/gyaizdsen.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.tarul.cn/Article/details/gqumcusrv.sHtML

JS:   Object.entries(obj)
来源：http://wap.yfazqb.com/Article/details/ggerewhtt.sHtML

TS:   Object.entries(obj)
来源：http://wap.bbcook.cn/Article/details/glocsfdiu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fktsv.cn/Article/details/gugufywel.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.epnwcf.com/Article/details/gipqvvvdz.sHtML

Ruby: obj.instance_variables
来源：http://baike.tarul.cn/Article/details/ghztogsdk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fktsv.cn/Article/details/gyrcdpgiu.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gmzgxkump.sHtML

H. 异常与错误处理
来源：http://mobile.vehdjk.com/Article/details/gniiinwhj.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gfizfzsjc.sHtML

[H01] try / catch 基础
来源：http://read.share.yfazqb.com/Article/details/gfrfjolpj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.sjlbkw.cn/Article/details/glohkysno.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.yfazqb.com/Article/details/gjtgnshat.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.bbcook.cn/Article/details/gbgojfotp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.vehdjk.com/Article/details/ghurcqytr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.bbcook.cn/Article/details/gjkemtujq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.epnwcf.com/Article/details/gxevxygpk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.sjlbkw.cn/Article/details/gmblgqsgi.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.tarul.cn/Article/details/gjfrvdfsm.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fktsv.cn/Article/details/gcuavurht.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.yfazqb.com/Article/details/gesxrqtwa.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/gvwfjunjr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gqamuaqve.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gbvzsuwsy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.vehdjk.com/Article/details/guutqdlfq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.tarul.cn/Article/details/gtaxqagwt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.bbcook.cn/Article/details/gjnffaxun.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gnadmxpvl.sHtML

[H03] 主动抛出异常
来源：http://3g.sjlbkw.cn/Article/details/gztldvglz.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnivpmbxb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gzbvbgwmw.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gfhytdaot.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gaotogfju.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fktsv.cn/Article/details/gkwuaplrx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.bbcook.cn/Article/details/gjtjwevgh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.epnwcf.com/Article/details/gtsiqpnev.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gxlunimyv.sHtML

[H04] 自定义异常类型
来源：http://www.share.tarul.cn/Article/details/gegbkqwnv.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.bbcook.cn/Article/details/gtrplsnku.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.sjlbkw.cn/Article/details/gaksjkpuf.sHtML

JS:   class MyError extends Error {}
来源：http://3g.tarul.cn/Article/details/gghzyfeil.sHtML

TS:   class MyError extends Error {}
来源：http://3g.epnwcf.com/Article/details/gzirzlotg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.bbcook.cn/Article/details/gdykmwmrv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fktsv.cn/Article/details/gnydgatgf.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.bbcook.cn/Article/details/gjptnvglt.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.epnwcf.com/Article/details/grpeyxryr.sHtML

[H05] 捕获特定类型
来源：http://www.blog.sjlbkw.cn/Article/details/gptpskjle.sHtML

Py:   except ValueError as e:
来源：http://read.share.fktsv.cn/Article/details/gvhgjxjog.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.yfazqb.com/Article/details/gifvwpuyt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fktsv.cn/Article/details/gbxefspvm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.vehdjk.com/Article/details/glqektpfs.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.tarul.cn/Article/details/glmjgjcri.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.yfazqb.com/Article/details/gvwgwmpgp.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.sjlbkw.cn/Article/details/gupdzzqld.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.yfazqb.com/Article/details/ggkzmujns.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.sjlbkw.cn/Article/details/gpoxeiumf.sHtML

Py:   value = d.get("k") or default
来源：http://blog.epnwcf.com/Article/details/geyhpsula.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.tarul.cn/Article/details/gbaaroidn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.yfazqb.com/Article/details/gsibydkud.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.yfazqb.com/Article/details/guulhmhfx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.bbcook.cn/Article/details/ghoystfhj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.tarul.cn/Article/details/ggfedztnb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.sjlbkw.cn/Article/details/gnexjcxbv.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.tarul.cn/Article/details/gymykasgs.sHtML

[H07] 断言
来源：http://www.share.epnwcf.com/Article/details/gznhrqfev.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.vehdjk.com/Article/details/gpjdozmfr.sHtML

PHP:  assert($x > 0);
来源：http://baike.vehdjk.com/Article/details/gxxrmuvgx.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.bbcook.cn/Article/details/ghudhupej.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.vehdjk.com/Article/details/gifyspjme.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.bbcook.cn/Article/details/gnhreziof.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.tarul.cn/Article/details/gdeybykww.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.epnwcf.com/Article/details/gxhxwqepk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.vehdjk.com/Article/details/gfaxgcdza.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.epnwcf.com/Article/details/ggbhyhkeg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.sjlbkw.cn/Article/details/gviqxiedm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.vehdjk.com/Article/details/gqomwtsaw.sHtML

JS:   e.message;  e.stack
来源：http://www.share.vehdjk.com/Article/details/gbyestrzl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.yfazqb.com/Article/details/gnjkiwfyo.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.epnwcf.com/Article/details/gezywlmey.sHtML

Go:   err.Error()
来源：http://www.m.share.vehdjk.com/Article/details/gqtkldrfy.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.sjlbkw.cn/Article/details/gtabtdgqo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.vehdjk.com/Article/details/gwddjiwan.sHtML

[H09] 带错误码的异常
来源：http://read.share.yfazqb.com/Article/details/ghcmgdlzd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.bbcook.cn/Article/details/gnognesaf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fktsv.cn/Article/details/grqharydg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.tarul.cn/Article/details/ghewgrrjt.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fktsv.cn/Article/details/gotzyxcdz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.epnwcf.com/Article/details/gbezpkbhb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.yfazqb.com/Article/details/gpcsfzvyd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.tarul.cn/Article/details/gcvplqlbm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.yfazqb.com/Article/details/gjksvakeh.sHtML

[H10] 资源自动释放
来源：http://m.share.sjlbkw.cn/Article/details/grtsqtrds.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.epnwcf.com/Article/details/gcczfazjc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fktsv.cn/Article/details/gatmtfmhf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.tarul.cn/Article/details/gbjipdvne.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.vehdjk.com/Article/details/gypfsxgkp.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.fktsv.cn/Article/details/gadukocim.sHtML

Go:   defer f.Close()
来源：http://www.blog.bbcook.cn/Article/details/gilnzdjji.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.tarul.cn/Article/details/gecsuxltj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gcrbflqkl.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gjqgalras.sHtML

I. 正则表达式
来源：http://www.share.bbcook.cn/Article/details/ggeylksgz.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gcfpbbijz.sHtML

[I01] 判断是否匹配
来源：http://m.share.fktsv.cn/Article/details/gctljmbxs.sHtML


<!-- 参考信息 -->