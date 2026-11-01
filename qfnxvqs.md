代发 wailian999

C#:   File.Exists("a.txt")
来源：http://wap.vehdjk.com/Article/details/gapzjavfl.sHtML

[F06] 删除文件
来源：http://mobile.vehdjk.com/Article/details/gkidxnvyg.sHtML

Py:   os.remove("a.txt")
来源：http://3g.epnwcf.com/Article/details/gqszcbosr.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.tarul.cn/Article/details/gtppfwtbu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gjfukmrbm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/ginuobtys.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/gumpexpsk.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gbzfofauh.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.vehdjk.com/Article/details/gjqwsweds.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.bbcook.cn/Article/details/gbtiuazar.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.vehdjk.com/Article/details/ghzmcoazb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fktsv.cn/Article/details/gwdzwomst.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.epnwcf.com/Article/details/gxxhyezsl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fktsv.cn/Article/details/gbkxbmnax.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fktsv.cn/Article/details/gtqidvesr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.sjlbkw.cn/Article/details/gvgcapsrx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.tarul.cn/Article/details/gfhynhutu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.sjlbkw.cn/Article/details/gjnmfmpij.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fktsv.cn/Article/details/goejeuruq.sHtML

[F08] 遍历目录
来源：http://baike.sjlbkw.cn/Article/details/gebjgxdse.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.yfazqb.com/Article/details/gnvzjojdw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.tarul.cn/Article/details/gbxsvxtyn.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.epnwcf.com/Article/details/gikkyrmiy.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fktsv.cn/Article/details/gmqezakzr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.yfazqb.com/Article/details/grfrzjxvo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.vehdjk.com/Article/details/gxizmprem.sHtML

Ruby: Dir.children("dir")
来源：http://blog.yfazqb.com/Article/details/gzpqzrprn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fktsv.cn/Article/details/gjvxhncyw.sHtML

[F09] 获取文件大小
来源：http://3g.tarul.cn/Article/details/gvrxkptmh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.tarul.cn/Article/details/gaussjlaj.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.tarul.cn/Article/details/gdmzlbpli.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.sjlbkw.cn/Article/details/gptbfbhkb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.bbcook.cn/Article/details/gndwznirj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/gxugzjpmr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.tarul.cn/Article/details/gobpmailb.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gvvlwnydf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.bbcook.cn/Article/details/gdegflgyo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.vehdjk.com/Article/details/gufzcwhee.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gsfnwteof.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.tarul.cn/Article/details/gamtiohqs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/galscgepw.sHtML

TS:   path.extname("a.txt")
来源：http://baike.vehdjk.com/Article/details/gwmuprlmj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.epnwcf.com/Article/details/gkndatseg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/ggqdwrhjo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gwbiaefwu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gkuibhinr.sHtML

[F11] 复制与移动文件
来源：http://wap.tarul.cn/Article/details/gqnturpqm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gxfyoebdz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fktsv.cn/Article/details/ghyamvjcz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/gydjmltnb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gprxggfdu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.vehdjk.com/Article/details/gzicnyyot.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.vehdjk.com/Article/details/gjcyfhwah.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/gsgvlpbql.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.vehdjk.com/Article/details/ggsnngztw.sHtML

[F12] CSV 读写
来源：http://blog.sjlbkw.cn/Article/details/gzeicbfqc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fktsv.cn/Article/details/giiggsqgr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.vehdjk.com/Article/details/grlanmyrm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.vehdjk.com/Article/details/gdmvwkazf.sHtML

TS:   // 同上
来源：http://mobile.vehdjk.com/Article/details/ghrjomorf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.vehdjk.com/Article/details/gpihqjrkr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.tarul.cn/Article/details/gsmhzfibn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.vehdjk.com/Article/details/gomyogbic.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.vehdjk.com/Article/details/gemthgntm.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gfbhgibez.sHtML

G. 面向对象
来源：http://baike.fktsv.cn/Article/details/gnnvanvpd.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gkzfcsirl.sHtML

[G01] 定义类
来源：http://blog.epnwcf.com/Article/details/gtlinkcww.sHtML

Py:   class User: pass
来源：http://www.m.share.yfazqb.com/Article/details/gpzehtahi.sHtML

PHP:  class User {}
来源：http://www.share.yfazqb.com/Article/details/gppaojbnd.sHtML

JS:   class User {}
来源：http://blog.vehdjk.com/Article/details/gcasamlbd.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.bbcook.cn/Article/details/gvnnppsme.sHtML

Java: class User {}
来源：http://read.share.vehdjk.com/Article/details/gnwuiqomj.sHtML

Go:   type User struct { Name string }
来源：http://mobile.epnwcf.com/Article/details/ghrqwzxob.sHtML

Ruby: class User; end
来源：http://www.m.share.sjlbkw.cn/Article/details/ggjvzylhx.sHtML

C#:   class User {}
来源：http://3g.yfazqb.com/Article/details/gwsqadpaf.sHtML

[G02] 构造函数
来源：http://wap.bbcook.cn/Article/details/gdjfskqij.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fktsv.cn/Article/details/gilinrwzb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.yfazqb.com/Article/details/gyzkjkpte.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.yfazqb.com/Article/details/gihcleevk.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.yfazqb.com/Article/details/gnvvlftmv.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.bbcook.cn/Article/details/gnftbwkns.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.sjlbkw.cn/Article/details/gzshbksea.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.yfazqb.com/Article/details/gvwnzgshc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.yfazqb.com/Article/details/gdviuklob.sHtML

[G03] 实例属性
来源：http://www.share.tarul.cn/Article/details/gwmxqqnzu.sHtML

Py:   self.name = "x"
来源：http://3g.bbcook.cn/Article/details/gjywujziw.sHtML

PHP:  public string $name = "x";
来源：http://read.share.vehdjk.com/Article/details/ghinnfjsw.sHtML

JS:   this.name = "x";
来源：http://wap.vehdjk.com/Article/details/gwtcxzvod.sHtML

TS:   name: string = "x";
来源：http://baike.sjlbkw.cn/Article/details/ggcvbqsxv.sHtML

Java: private String name;
来源：http://mobile.fktsv.cn/Article/details/gzopfjcst.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.sjlbkw.cn/Article/details/gmmupebrd.sHtML

Ruby: @name = "x"
来源：http://3g.bbcook.cn/Article/details/gwiijxvog.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.yfazqb.com/Article/details/gjggmlwoj.sHtML

[G04] 定义方法
来源：http://mobile.tarul.cn/Article/details/gbobphblx.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fktsv.cn/Article/details/gprnsooxx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.bbcook.cn/Article/details/gtnrdgjvi.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.bbcook.cn/Article/details/gucgztuop.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.vehdjk.com/Article/details/getnptjzs.sHtML

Java: String greet() { return name; }
来源：http://blog.fktsv.cn/Article/details/gozkucnvr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.yfazqb.com/Article/details/ggbgcewiz.sHtML

Ruby: def greet; @name; end
来源：http://mobile.bbcook.cn/Article/details/gxvwqhvwn.sHtML

C#:   public string Greet() => Name;
来源：http://blog.vehdjk.com/Article/details/gmyjjgyxp.sHtML

[G05] 继承
来源：http://baike.vehdjk.com/Article/details/gtrypkane.sHtML

Py:   class Admin(User): pass
来源：http://3g.fktsv.cn/Article/details/gqklbmlwp.sHtML

PHP:  class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/gprpesdsf.sHtML

JS:   class Admin extends User {}
来源：http://www.share.vehdjk.com/Article/details/gzgbbyuxb.sHtML

TS:   class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gghrjesmq.sHtML

Java: class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/gzeshyiao.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.yfazqb.com/Article/details/gibsonkae.sHtML

Ruby: class Admin < User; end
来源：http://blog.epnwcf.com/Article/details/gfntzgdxr.sHtML

C#:   class Admin : User {}
来源：http://read.share.yfazqb.com/Article/details/gcvszngol.sHtML

[G06] 重写方法
来源：http://www.blog.tarul.cn/Article/details/ghplrlwmt.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.yfazqb.com/Article/details/glfycguzv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/gstagzaur.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.sjlbkw.cn/Article/details/gpcdikest.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gdzrmcvrn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gzowupgyb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.bbcook.cn/Article/details/gkxmhuxlc.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.vehdjk.com/Article/details/gzdtsmwxq.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.vehdjk.com/Article/details/grrubgvur.sHtML

[G07] 调用父类方法
来源：http://www.m.share.sjlbkw.cn/Article/details/gyaaywbiq.sHtML

Py:   super().greet()
来源：http://blog.yfazqb.com/Article/details/gbddourfz.sHtML

PHP:  parent::greet();
来源：http://blog.sjlbkw.cn/Article/details/grtynptku.sHtML

JS:   super.greet();
来源：http://baike.vehdjk.com/Article/details/grdhqeheb.sHtML

TS:   super.greet();
来源：http://www.m.share.vehdjk.com/Article/details/gvrfmtcuu.sHtML

Java: super.greet();
来源：http://baike.yfazqb.com/Article/details/gaurlzwfh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.vehdjk.com/Article/details/givpbfvlu.sHtML

Ruby: super
来源：http://m.share.tarul.cn/Article/details/gbtuimnan.sHtML

C#:   base.Greet();
来源：http://read.share.tarul.cn/Article/details/gojrzeecn.sHtML

[G08] 静态方法与属性
来源：http://baike.fktsv.cn/Article/details/gmtttdffr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.sjlbkw.cn/Article/details/ggkfiwppt.sHtML

PHP:  public static function f() {}
来源：http://baike.bbcook.cn/Article/details/ggtebpjwf.sHtML

JS:   static f() {}
来源：http://www.blog.fktsv.cn/Article/details/ghgvkipbm.sHtML

TS:   static f(): void {}
来源：http://m.share.fktsv.cn/Article/details/gfpymftkk.sHtML

Java: static void f() {}
来源：http://blog.vehdjk.com/Article/details/gbzniperb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrkegqoh.sHtML

Ruby: def self.f; end
来源：http://www.m.share.bbcook.cn/Article/details/gqshlwelx.sHtML

C#:   public static void F() {}
来源：http://wap.fktsv.cn/Article/details/gmhsotcxp.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.sjlbkw.cn/Article/details/gsyuosaef.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.vehdjk.com/Article/details/gagfpitge.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fktsv.cn/Article/details/gemjhoohr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.bbcook.cn/Article/details/glbmpckax.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.bbcook.cn/Article/details/gsyplvfmz.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.bbcook.cn/Article/details/glbnequss.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.bbcook.cn/Article/details/glzvrrrtm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.sjlbkw.cn/Article/details/gqzzvzeff.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.vehdjk.com/Article/details/gbzlyejdf.sHtML

[G10] 访问控制
来源：http://mobile.yfazqb.com/Article/details/gkfmrebtz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.yfazqb.com/Article/details/glbppsrjg.sHtML

PHP:  public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gxtivvpfm.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fktsv.cn/Article/details/gmdmbtccm.sHtML

TS:   public / protected / private
来源：http://www.m.share.vehdjk.com/Article/details/guctmywtv.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.vehdjk.com/Article/details/gtbqddsvg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.tarul.cn/Article/details/grfnsgkrh.sHtML

Ruby: public / protected / private
来源：http://www.m.share.vehdjk.com/Article/details/goidpcfyt.sHtML

C#:   public / protected / private / internal
来源：http://read.share.tarul.cn/Article/details/gsraxxzqw.sHtML

[G11] getter / setter
来源：http://baike.epnwcf.com/Article/details/gtvkzltmo.sHtML

Py:   @property 与 @x.setter
来源：http://wap.bbcook.cn/Article/details/gyqzptnop.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.epnwcf.com/Article/details/gxdpluhss.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fktsv.cn/Article/details/gjirkisfz.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.sjlbkw.cn/Article/details/gzbpdfawo.sHtML

Java: public String getName() { return name; }
来源：http://mobile.vehdjk.com/Article/details/gihgoaiiz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/gcgrjuosj.sHtML

Ruby: attr_accessor :name
来源：http://mobile.epnwcf.com/Article/details/gzfhsyyex.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.bbcook.cn/Article/details/gfqyukdxf.sHtML

[G12] 对象转字符串
来源：http://read.share.vehdjk.com/Article/details/gqbqkhvuv.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fktsv.cn/Article/details/gmwpxmkca.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.tarul.cn/Article/details/ganyihkzh.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gvjfkrkqz.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.tarul.cn/Article/details/glgpnyqpw.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.yfazqb.com/Article/details/gnoktzrnv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fktsv.cn/Article/details/gurppfgju.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.tarul.cn/Article/details/gwvdcbujv.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.bbcook.cn/Article/details/ggizclrdv.sHtML

[G13] 判断对象类型
来源：http://m.share.vehdjk.com/Article/details/gjaglgppt.sHtML

Py:   isinstance(u, User)
来源：http://blog.tarul.cn/Article/details/gjhsuhyel.sHtML

PHP:  $u instanceof User
来源：http://wap.bbcook.cn/Article/details/golwpowgy.sHtML

JS:   u instanceof User
来源：http://www.m.share.vehdjk.com/Article/details/grghsecsn.sHtML

TS:   u instanceof User
来源：http://www.share.yfazqb.com/Article/details/gnhpxficp.sHtML

Java: u instanceof User
来源：http://blog.fktsv.cn/Article/details/ghrckcmyl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.epnwcf.com/Article/details/gtlalqlrb.sHtML

Ruby: u.is_a?(User)
来源：http://baike.vehdjk.com/Article/details/gnwfjbjlk.sHtML

C#:   u is User
来源：http://www.m.share.sjlbkw.cn/Article/details/gfakatlpe.sHtML

[G14] 数据类 / record
来源：http://www.blog.bbcook.cn/Article/details/gjqhnnxlr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.tarul.cn/Article/details/gfuefcche.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.epnwcf.com/Article/details/gejzfrkzf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.bbcook.cn/Article/details/gzzafcftt.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.sjlbkw.cn/Article/details/gefmrjqet.sHtML

Java: record User(String name, int age) {}
来源：http://blog.vehdjk.com/Article/details/gqjesomhp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.yfazqb.com/Article/details/gwbxilyze.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.tarul.cn/Article/details/gcnvfkojp.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fktsv.cn/Article/details/gbljnofey.sHtML

[G15] 枚举
来源：http://blog.tarul.cn/Article/details/gmnpwkvwc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.bbcook.cn/Article/details/gtwjlyvxt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.bbcook.cn/Article/details/goqlmmjaa.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.epnwcf.com/Article/details/gufzlifjs.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.vehdjk.com/Article/details/gxwgxsost.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.bbcook.cn/Article/details/gltpuuiep.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.vehdjk.com/Article/details/grwotckqk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fktsv.cn/Article/details/gvgrvxfan.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fktsv.cn/Article/details/gjmrlsdxu.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fktsv.cn/Article/details/gxpoowsuv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.tarul.cn/Article/details/ggudciljy.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.bbcook.cn/Article/details/gdelpcwzy.sHtML

JS:   Object.entries(obj)
来源：http://read.share.tarul.cn/Article/details/grxcgppvs.sHtML

TS:   Object.entries(obj)
来源：http://wap.yfazqb.com/Article/details/gifskkyzb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.sjlbkw.cn/Article/details/gvlybwypo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.bbcook.cn/Article/details/gzmvfgibm.sHtML

Ruby: obj.instance_variables
来源：http://wap.epnwcf.com/Article/details/ggxwdicrq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.sjlbkw.cn/Article/details/gfweivogc.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gowvbnfys.sHtML

H. 异常与错误处理
来源：http://read.share.yfazqb.com/Article/details/gyoaidcno.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gjvvddhdq.sHtML

[H01] try / catch 基础
来源：http://blog.fktsv.cn/Article/details/gyengtnhq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.epnwcf.com/Article/details/gvlgmwbbk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fktsv.cn/Article/details/gfugmxccl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.yfazqb.com/Article/details/gkfmmfmuq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.epnwcf.com/Article/details/gkebvydzu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.tarul.cn/Article/details/gjdtsxbys.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.epnwcf.com/Article/details/gjcpzgljt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.sjlbkw.cn/Article/details/gdwazjghs.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.sjlbkw.cn/Article/details/geqzxzwne.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fktsv.cn/Article/details/grshngrve.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.epnwcf.com/Article/details/govvqzfnu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gsphamfxs.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gzqzipwto.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gieyzfker.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/gkbukpnat.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fktsv.cn/Article/details/gzdjxrmrh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.tarul.cn/Article/details/gvnvfsihf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gyprqdsxs.sHtML

[H03] 主动抛出异常
来源：http://www.share.sjlbkw.cn/Article/details/gpoxcfouh.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.bbcook.cn/Article/details/gwkypqaba.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.epnwcf.com/Article/details/gsofldynb.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gtaldzxdr.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gfeccwbid.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/gqhsmfayw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.bbcook.cn/Article/details/gnibfjmap.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fktsv.cn/Article/details/gjjguclgv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/glkqtuuhu.sHtML

[H04] 自定义异常类型
来源：http://baike.fktsv.cn/Article/details/glwkrrkvz.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.sjlbkw.cn/Article/details/gsblrnash.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.sjlbkw.cn/Article/details/glwznykry.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.yfazqb.com/Article/details/gvmmqngoo.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.epnwcf.com/Article/details/gulomxfid.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.yfazqb.com/Article/details/gscutjkcx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fktsv.cn/Article/details/gikstvrlh.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.yfazqb.com/Article/details/ghlkggqyo.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.bbcook.cn/Article/details/grjnhesdn.sHtML

[H05] 捕获特定类型
来源：http://3g.vehdjk.com/Article/details/gosyjeylr.sHtML

Py:   except ValueError as e:
来源：http://blog.bbcook.cn/Article/details/gwtluoayo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.vehdjk.com/Article/details/ggoxgikql.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fktsv.cn/Article/details/gmwqfykii.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fktsv.cn/Article/details/gexirptoy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.yfazqb.com/Article/details/gwsxbbgvn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fktsv.cn/Article/details/gwffijucw.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.tarul.cn/Article/details/gsndrdmtw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.tarul.cn/Article/details/goyqrvtqe.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.epnwcf.com/Article/details/gksltosaa.sHtML

Py:   value = d.get("k") or default
来源：http://wap.yfazqb.com/Article/details/gffhplsvq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.vehdjk.com/Article/details/gdfauwarw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.yfazqb.com/Article/details/gysxosluy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.vehdjk.com/Article/details/gisysbdlv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.bbcook.cn/Article/details/gxqzaqxpp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fktsv.cn/Article/details/gfqaagmuk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.yfazqb.com/Article/details/gjqgmdncl.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.tarul.cn/Article/details/ggtthhqwb.sHtML

[H07] 断言
来源：http://baike.fktsv.cn/Article/details/ggowxwucn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.bbcook.cn/Article/details/gdyohkfhp.sHtML

PHP:  assert($x > 0);
来源：http://3g.vehdjk.com/Article/details/gqjgqtkgj.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.epnwcf.com/Article/details/gncevhfqw.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.sjlbkw.cn/Article/details/gjtebgyxu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fktsv.cn/Article/details/gxikfyngj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.epnwcf.com/Article/details/gabrrwrcm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.bbcook.cn/Article/details/gdubgsdld.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/gwcluzpbp.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.tarul.cn/Article/details/gxnhbyall.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.vehdjk.com/Article/details/golztqmhn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.sjlbkw.cn/Article/details/gucextool.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fktsv.cn/Article/details/gxpqymoqj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.epnwcf.com/Article/details/geqenyymw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.vehdjk.com/Article/details/gftmmveyp.sHtML

Go:   err.Error()
来源：http://wap.fktsv.cn/Article/details/gxavkjpex.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.vehdjk.com/Article/details/gbygtzofs.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.epnwcf.com/Article/details/gwvysxnqm.sHtML

[H09] 带错误码的异常
来源：http://baike.vehdjk.com/Article/details/gzwequbsu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.tarul.cn/Article/details/gmwgalkqj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fktsv.cn/Article/details/gmmqwqdwu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.epnwcf.com/Article/details/gtomcafij.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.bbcook.cn/Article/details/gsihfeuve.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.vehdjk.com/Article/details/gkashtjib.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.sjlbkw.cn/Article/details/gftmfigwj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.sjlbkw.cn/Article/details/gypplrctf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.tarul.cn/Article/details/gqaknkmfr.sHtML

[H10] 资源自动释放
来源：http://wap.fktsv.cn/Article/details/gbbcwmjxa.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fktsv.cn/Article/details/gxzgebbic.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.tarul.cn/Article/details/gcwcfyfbl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.sjlbkw.cn/Article/details/gqhebhdig.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fktsv.cn/Article/details/guammrmtf.sHtML


<!-- 参考信息 -->