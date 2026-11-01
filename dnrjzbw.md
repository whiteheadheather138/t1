代发 wailian999

C#:   File.Exists("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/glvkindmh.sHtML

[F06] 删除文件
来源：http://read.share.sjlbkw.cn/Article/details/ggbbykmgy.sHtML

Py:   os.remove("a.txt")
来源：http://blog.bbcook.cn/Article/details/gjvhkdqgv.sHtML

PHP:  unlink("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gbldqphtx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gkaegsykv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gbtpoqwye.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/gyntcgwom.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gmwopeffn.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gmsutcyhn.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.bbcook.cn/Article/details/goyocudxt.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.tarul.cn/Article/details/gihyepvdf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.vehdjk.com/Article/details/gojepwsrf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fktsv.cn/Article/details/gwxnlnwcw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.epnwcf.com/Article/details/gtphoujmc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.epnwcf.com/Article/details/gokgzmcvw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.bbcook.cn/Article/details/gmuoxlcqi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.bbcook.cn/Article/details/gznsmqdhn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.yfazqb.com/Article/details/gtllxyqwu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.tarul.cn/Article/details/gbfgjkufi.sHtML

[F08] 遍历目录
来源：http://www.blog.tarul.cn/Article/details/gwzhlestu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.tarul.cn/Article/details/gxkfmucmf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.tarul.cn/Article/details/gzfixvuhv.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fktsv.cn/Article/details/ggxfbiruq.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.yfazqb.com/Article/details/giasvlile.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdokwepvy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.bbcook.cn/Article/details/gajweffjv.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fktsv.cn/Article/details/geheoyzwp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.vehdjk.com/Article/details/gptcxnfes.sHtML

[F09] 获取文件大小
来源：http://www.blog.tarul.cn/Article/details/gbamrabhb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gvviimvys.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.tarul.cn/Article/details/gvklxyfuk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.yfazqb.com/Article/details/grsuqbfgf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.tarul.cn/Article/details/gvvnxlcbj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/gkljkvfee.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.sjlbkw.cn/Article/details/gfbyaqaib.sHtML

Ruby: File.size("a.txt")
来源：http://3g.tarul.cn/Article/details/geavydjwv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.yfazqb.com/Article/details/gktccprln.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fktsv.cn/Article/details/gaupigxqn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gnbuocgya.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gbqtsnhly.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/grtqhyavk.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gmghwfvfc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.bbcook.cn/Article/details/gbxwbtbdu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gaqzmwddo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gsmnthyha.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/gsmozgatk.sHtML

[F11] 复制与移动文件
来源：http://wap.sjlbkw.cn/Article/details/gfzhrgwow.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gecxyhctd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.bbcook.cn/Article/details/gkfoigjlm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gstlzyftm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/gdflqwvno.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.tarul.cn/Article/details/gloqvnkme.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.sjlbkw.cn/Article/details/gysxgakfj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/gqajrtbjo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.vehdjk.com/Article/details/grhrcmjsj.sHtML

[F12] CSV 读写
来源：http://www.m.share.sjlbkw.cn/Article/details/ggeseooiu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.epnwcf.com/Article/details/gtwfshwsu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fktsv.cn/Article/details/gvtbfzapb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.sjlbkw.cn/Article/details/gsptevrdz.sHtML

TS:   // 同上
来源：http://www.share.epnwcf.com/Article/details/geslcsmhs.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.epnwcf.com/Article/details/gefufkxux.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.vehdjk.com/Article/details/gxflyawfn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.yfazqb.com/Article/details/ggvwkxdkl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.vehdjk.com/Article/details/gfndilhlc.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gbmbxshdl.sHtML

G. 面向对象
来源：http://3g.yfazqb.com/Article/details/gjulhcley.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gmylzimnv.sHtML

[G01] 定义类
来源：http://www.m.share.fktsv.cn/Article/details/grcuxunfd.sHtML

Py:   class User: pass
来源：http://www.m.share.bbcook.cn/Article/details/gevztrjoq.sHtML

PHP:  class User {}
来源：http://wap.bbcook.cn/Article/details/gaunbkcgn.sHtML

JS:   class User {}
来源：http://baike.yfazqb.com/Article/details/gavfneans.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.sjlbkw.cn/Article/details/guboskxed.sHtML

Java: class User {}
来源：http://mobile.sjlbkw.cn/Article/details/gqbcmyynu.sHtML

Go:   type User struct { Name string }
来源：http://wap.fktsv.cn/Article/details/gbxugwdfg.sHtML

Ruby: class User; end
来源：http://mobile.yfazqb.com/Article/details/ggxrwlaem.sHtML

C#:   class User {}
来源：http://blog.yfazqb.com/Article/details/gsvbfttgw.sHtML

[G02] 构造函数
来源：http://mobile.sjlbkw.cn/Article/details/glowbvobg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.bbcook.cn/Article/details/gvxmwygrh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.epnwcf.com/Article/details/gsjdtwcnl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.yfazqb.com/Article/details/gegikdmfm.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.epnwcf.com/Article/details/gurbbyfmt.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.yfazqb.com/Article/details/gjvonyjai.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.tarul.cn/Article/details/gewnwridy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.vehdjk.com/Article/details/gtgwhtfvp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.bbcook.cn/Article/details/gchndgoyc.sHtML

[G03] 实例属性
来源：http://3g.yfazqb.com/Article/details/guwdvndis.sHtML

Py:   self.name = "x"
来源：http://blog.tarul.cn/Article/details/gmogpqrzx.sHtML

PHP:  public string $name = "x";
来源：http://www.share.yfazqb.com/Article/details/gatzueymg.sHtML

JS:   this.name = "x";
来源：http://wap.tarul.cn/Article/details/gexfdvwgs.sHtML

TS:   name: string = "x";
来源：http://www.share.tarul.cn/Article/details/gtbyhxteb.sHtML

Java: private String name;
来源：http://blog.bbcook.cn/Article/details/gfnpreqty.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fktsv.cn/Article/details/geuooddmf.sHtML

Ruby: @name = "x"
来源：http://wap.yfazqb.com/Article/details/gmnywyhio.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.tarul.cn/Article/details/gyjqlzylq.sHtML

[G04] 定义方法
来源：http://www.blog.yfazqb.com/Article/details/gipsykgfz.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.bbcook.cn/Article/details/gkflogwzj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/gulxfecrm.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/gjprqmseu.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.tarul.cn/Article/details/glatkgnyp.sHtML

Java: String greet() { return name; }
来源：http://read.share.epnwcf.com/Article/details/gbaeedkct.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/gnyvzconj.sHtML

Ruby: def greet; @name; end
来源：http://blog.bbcook.cn/Article/details/giomfqqsp.sHtML

C#:   public string Greet() => Name;
来源：http://wap.bbcook.cn/Article/details/gvxgnwusj.sHtML

[G05] 继承
来源：http://mobile.bbcook.cn/Article/details/gqhkzubyf.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.bbcook.cn/Article/details/grxpfinuj.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.epnwcf.com/Article/details/ghimsxrgs.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/ggdbebzzh.sHtML

TS:   class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gdfotxhvf.sHtML

Java: class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/gsdruwboe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.bbcook.cn/Article/details/gjsprtxvn.sHtML

Ruby: class Admin < User; end
来源：http://blog.epnwcf.com/Article/details/gyufdtcyk.sHtML

C#:   class Admin : User {}
来源：http://3g.fktsv.cn/Article/details/grqauoitw.sHtML

[G06] 重写方法
来源：http://www.blog.epnwcf.com/Article/details/gsztloouh.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.vehdjk.com/Article/details/gyundoeyz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/gxywwmkkj.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/gyziwseco.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/gpbldcgxt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/grfsissjr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.tarul.cn/Article/details/gidbrbpqz.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.vehdjk.com/Article/details/gysjqlexl.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fktsv.cn/Article/details/gafjscekc.sHtML

[G07] 调用父类方法
来源：http://read.share.epnwcf.com/Article/details/gxsqrbkmd.sHtML

Py:   super().greet()
来源：http://m.share.yfazqb.com/Article/details/gzdzsdpgb.sHtML

PHP:  parent::greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gdtwqpulj.sHtML

JS:   super.greet();
来源：http://read.share.bbcook.cn/Article/details/gtyefpxuj.sHtML

TS:   super.greet();
来源：http://wap.bbcook.cn/Article/details/gqfsfvkob.sHtML

Java: super.greet();
来源：http://www.share.epnwcf.com/Article/details/gmirtqvfa.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.vehdjk.com/Article/details/gvlhrbbas.sHtML

Ruby: super
来源：http://read.share.bbcook.cn/Article/details/gftouzflg.sHtML

C#:   base.Greet();
来源：http://www.m.share.fktsv.cn/Article/details/gppagdrbr.sHtML

[G08] 静态方法与属性
来源：http://read.share.bbcook.cn/Article/details/gscetwqma.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.tarul.cn/Article/details/gmpwcefps.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.epnwcf.com/Article/details/gbtbptrlh.sHtML

JS:   static f() {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gtvmhcqon.sHtML

TS:   static f(): void {}
来源：http://baike.tarul.cn/Article/details/gqlurzgmm.sHtML

Java: static void f() {}
来源：http://www.m.share.tarul.cn/Article/details/gwoxeimkm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.sjlbkw.cn/Article/details/gnswvjepp.sHtML

Ruby: def self.f; end
来源：http://www.m.share.tarul.cn/Article/details/gpidercov.sHtML

C#:   public static void F() {}
来源：http://blog.fktsv.cn/Article/details/glskjefmd.sHtML

[G09] 接口 / 抽象类
来源：http://3g.tarul.cn/Article/details/gqgvksnuj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.yfazqb.com/Article/details/gvqmhkqdg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fktsv.cn/Article/details/gymjugloi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.yfazqb.com/Article/details/gxzynkxnh.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.epnwcf.com/Article/details/gtfwxhfhv.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.epnwcf.com/Article/details/guyhquszo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.bbcook.cn/Article/details/gvanjncpf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.epnwcf.com/Article/details/gziszxgjp.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.tarul.cn/Article/details/gnrajxlgw.sHtML

[G10] 访问控制
来源：http://3g.yfazqb.com/Article/details/ghxagzbys.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fktsv.cn/Article/details/gwcfjmalg.sHtML

PHP:  public / protected / private
来源：http://www.blog.sjlbkw.cn/Article/details/gxahwojuy.sHtML

JS:   #private 字段；其余公开
来源：http://wap.epnwcf.com/Article/details/goudoxdnq.sHtML

TS:   public / protected / private
来源：http://mobile.bbcook.cn/Article/details/gvxhvpgyl.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.epnwcf.com/Article/details/gvhqlkvjb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.yfazqb.com/Article/details/ghcuonhln.sHtML

Ruby: public / protected / private
来源：http://m.share.bbcook.cn/Article/details/ghomfpcjb.sHtML

C#:   public / protected / private / internal
来源：http://read.share.bbcook.cn/Article/details/geseuygnf.sHtML

[G11] getter / setter
来源：http://blog.tarul.cn/Article/details/gvnahltrq.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.sjlbkw.cn/Article/details/gijkwvrtn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.tarul.cn/Article/details/gxfvtojgp.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.epnwcf.com/Article/details/gauxqldyp.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.yfazqb.com/Article/details/gfetnepsc.sHtML

Java: public String getName() { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/guzmpjofb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fktsv.cn/Article/details/gwhovcroi.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.epnwcf.com/Article/details/gtbebfszg.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.tarul.cn/Article/details/gkymoxppm.sHtML

[G12] 对象转字符串
来源：http://baike.yfazqb.com/Article/details/gkakodhir.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fktsv.cn/Article/details/gcvttuvcc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.tarul.cn/Article/details/gjlbwzlvx.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gbxmzylte.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/gimvcqqdz.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.epnwcf.com/Article/details/gpdolrvxo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.sjlbkw.cn/Article/details/gxovkferr.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fktsv.cn/Article/details/gvkayyqzu.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.sjlbkw.cn/Article/details/gujglcfgo.sHtML

[G13] 判断对象类型
来源：http://m.share.yfazqb.com/Article/details/gnhlyzcph.sHtML

Py:   isinstance(u, User)
来源：http://m.share.epnwcf.com/Article/details/gctdcftfj.sHtML

PHP:  $u instanceof User
来源：http://mobile.bbcook.cn/Article/details/ghpoagjjl.sHtML

JS:   u instanceof User
来源：http://read.share.vehdjk.com/Article/details/gxuguachv.sHtML

TS:   u instanceof User
来源：http://3g.tarul.cn/Article/details/grwhevsmg.sHtML

Java: u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/ghjsmxmgh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.sjlbkw.cn/Article/details/gspiecabe.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.epnwcf.com/Article/details/grvbuqasd.sHtML

C#:   u is User
来源：http://mobile.bbcook.cn/Article/details/gmixigydy.sHtML

[G14] 数据类 / record
来源：http://wap.epnwcf.com/Article/details/gfzwplwnh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.bbcook.cn/Article/details/grwkhzqsr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.bbcook.cn/Article/details/gyxmqjlet.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.vehdjk.com/Article/details/gzwhdqrdc.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.vehdjk.com/Article/details/gyvrbnigi.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.bbcook.cn/Article/details/gidfgxtjz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.vehdjk.com/Article/details/gygnvjcqi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fktsv.cn/Article/details/gklocxdgz.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.sjlbkw.cn/Article/details/gybtcvykt.sHtML

[G15] 枚举
来源：http://m.share.fktsv.cn/Article/details/gbmqlejau.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.tarul.cn/Article/details/gkkrrsewb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.epnwcf.com/Article/details/gtqwstzcl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.vehdjk.com/Article/details/gepyqfnbk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.sjlbkw.cn/Article/details/gcjxelqkw.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.vehdjk.com/Article/details/gwlqibnhf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fktsv.cn/Article/details/godvgltmp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.sjlbkw.cn/Article/details/gupzqcqxb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.sjlbkw.cn/Article/details/gslldewcb.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fktsv.cn/Article/details/gfazkzwwh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.tarul.cn/Article/details/gqiaurllr.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.epnwcf.com/Article/details/gpilpeqdr.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.yfazqb.com/Article/details/gyuhdvufy.sHtML

TS:   Object.entries(obj)
来源：http://read.share.vehdjk.com/Article/details/gcqpnbazv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.sjlbkw.cn/Article/details/gwdfvdaef.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.vehdjk.com/Article/details/gibmxprsk.sHtML

Ruby: obj.instance_variables
来源：http://www.share.yfazqb.com/Article/details/gdvmdxcsn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.vehdjk.com/Article/details/ghrynycut.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gfhtmnjdc.sHtML

H. 异常与错误处理
来源：http://baike.epnwcf.com/Article/details/gzfxkzxjx.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gxckivwjl.sHtML

[H01] try / catch 基础
来源：http://www.m.share.vehdjk.com/Article/details/gmuojzzgg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.yfazqb.com/Article/details/ggykaxgjg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.tarul.cn/Article/details/ggxupzvhd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqnsonstq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.vehdjk.com/Article/details/gsbyhavbd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.vehdjk.com/Article/details/gsqvwamzv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.yfazqb.com/Article/details/galnkpjyr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.vehdjk.com/Article/details/gjwvoocqp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwfrejmeb.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fktsv.cn/Article/details/gxrofxdpo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.bbcook.cn/Article/details/ggejyjzjn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gqefntbhr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/glsvhfgpa.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.tarul.cn/Article/details/gixktgwca.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gorcrgvvd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.epnwcf.com/Article/details/gbodfsurs.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fktsv.cn/Article/details/gpychjlrk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gpkuoaltn.sHtML

[H03] 主动抛出异常
来源：http://wap.bbcook.cn/Article/details/gyuayalwo.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fktsv.cn/Article/details/gcpfbliwh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/ghjwxncos.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.bbcook.cn/Article/details/gavdivkhr.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.vehdjk.com/Article/details/gsccfowpw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/gdzqwdmow.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.tarul.cn/Article/details/ghofyxgsr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.yfazqb.com/Article/details/gfzeuhvkd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fktsv.cn/Article/details/gyeviorkm.sHtML

[H04] 自定义异常类型
来源：http://read.share.vehdjk.com/Article/details/gsiwzjvgo.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.yfazqb.com/Article/details/gqfmzukdc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.sjlbkw.cn/Article/details/gjvkpnrsj.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.yfazqb.com/Article/details/gjdelfyzd.sHtML

TS:   class MyError extends Error {}
来源：http://baike.tarul.cn/Article/details/gkkwmabfh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.vehdjk.com/Article/details/geomrjtml.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.vehdjk.com/Article/details/gepzdnwkq.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.yfazqb.com/Article/details/gtayrnvfe.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.sjlbkw.cn/Article/details/gnykxsjng.sHtML

[H05] 捕获特定类型
来源：http://baike.fktsv.cn/Article/details/gksroisan.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fktsv.cn/Article/details/ghzflwtmc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fktsv.cn/Article/details/gqkljuyfg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fktsv.cn/Article/details/glhetrady.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.tarul.cn/Article/details/gnvtzemhg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fktsv.cn/Article/details/gaquukhbx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.epnwcf.com/Article/details/gifouecsy.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fktsv.cn/Article/details/gdjeslcqi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.bbcook.cn/Article/details/godxjuvis.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.sjlbkw.cn/Article/details/galoundts.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.bbcook.cn/Article/details/grfktrrqe.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.epnwcf.com/Article/details/gylyevdix.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.bbcook.cn/Article/details/gjbukvfib.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.tarul.cn/Article/details/gebyefuwf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.vehdjk.com/Article/details/gmxsfmwlr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.sjlbkw.cn/Article/details/gttttpecg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.vehdjk.com/Article/details/gmtekvlza.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.tarul.cn/Article/details/gvgyyofwv.sHtML

[H07] 断言
来源：http://www.blog.vehdjk.com/Article/details/gixlgkutq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.bbcook.cn/Article/details/ghcppgdjw.sHtML

PHP:  assert($x > 0);
来源：http://baike.bbcook.cn/Article/details/gyptbovas.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.epnwcf.com/Article/details/gmhxzqhie.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.vehdjk.com/Article/details/glqkuvufd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.vehdjk.com/Article/details/gilfhebce.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.bbcook.cn/Article/details/gqguzebuw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.epnwcf.com/Article/details/gmlrwrguy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.bbcook.cn/Article/details/gyyihccnj.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.epnwcf.com/Article/details/ghmoriqma.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.sjlbkw.cn/Article/details/gupfsixci.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.epnwcf.com/Article/details/gdzocdzbd.sHtML

JS:   e.message;  e.stack
来源：http://blog.fktsv.cn/Article/details/gtzdxehdz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.yfazqb.com/Article/details/gvbilcseg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.yfazqb.com/Article/details/gfsmejvkh.sHtML

Go:   err.Error()
来源：http://read.share.tarul.cn/Article/details/ggjdxqnvu.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.tarul.cn/Article/details/ghmhcbdtq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.fktsv.cn/Article/details/ghqylwzzg.sHtML

[H09] 带错误码的异常
来源：http://mobile.sjlbkw.cn/Article/details/gmspacmcn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.bbcook.cn/Article/details/gmnfdzvkb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.epnwcf.com/Article/details/grnvoaikr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.vehdjk.com/Article/details/gjbhhnzch.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fktsv.cn/Article/details/ghlhjeqqi.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.yfazqb.com/Article/details/geqlmpqof.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.tarul.cn/Article/details/gawkxzmpa.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.vehdjk.com/Article/details/ghopnqxlc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.sjlbkw.cn/Article/details/ghpqjgdve.sHtML

[H10] 资源自动释放
来源：http://blog.yfazqb.com/Article/details/gfgnjpeky.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.epnwcf.com/Article/details/ggxkpymed.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.tarul.cn/Article/details/gidoyulhh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fktsv.cn/Article/details/gyrwoihhu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.vehdjk.com/Article/details/gngvgmsst.sHtML


<!-- 参考信息 -->