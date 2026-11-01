代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.bbcook.cn/Article/details/gbttjcwjg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.epnwcf.com/Article/details/grfwaijdz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fktsv.cn/Article/details/gcyrxowjz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fktsv.cn/Article/details/gkbibbexf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.epnwcf.com/Article/details/gjvoogxbj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.bbcook.cn/Article/details/gljbblbzf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.tarul.cn/Article/details/gbzzetenf.sHtML

[F08] 遍历目录
来源：http://wap.tarul.cn/Article/details/gooebyroa.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fktsv.cn/Article/details/gtbkaudnb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.bbcook.cn/Article/details/gmxaaisvc.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.bbcook.cn/Article/details/grvoskpai.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.vehdjk.com/Article/details/gjccodrqo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.epnwcf.com/Article/details/ghnyttspa.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.bbcook.cn/Article/details/ggvadrwep.sHtML

Ruby: Dir.children("dir")
来源：http://wap.vehdjk.com/Article/details/gccccdbls.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gpscasnho.sHtML

[F09] 获取文件大小
来源：http://wap.sjlbkw.cn/Article/details/gkjvowicx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gxtiesnhg.sHtML

PHP:  filesize("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gydcakmpg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.sjlbkw.cn/Article/details/gzwgixhgz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.epnwcf.com/Article/details/gqodxrsab.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/ggmirjndu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.yfazqb.com/Article/details/gylrboumu.sHtML

Ruby: File.size("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gmckyatxz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fktsv.cn/Article/details/gbtnjhdfl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.sjlbkw.cn/Article/details/gozpddmtc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gpmjbijjn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.vehdjk.com/Article/details/gouwiewrv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/grpgnnuzs.sHtML

TS:   path.extname("a.txt")
来源：http://blog.bbcook.cn/Article/details/gmljjggxd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.yfazqb.com/Article/details/gcbhexfot.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gmsogfaia.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gpagvpwke.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gozftiikb.sHtML

[F11] 复制与移动文件
来源：http://baike.sjlbkw.cn/Article/details/glcteppko.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gdnqgvlms.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.tarul.cn/Article/details/gwjrzecjq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/gfjcgcddu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/gxspsydqn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.bbcook.cn/Article/details/gwjjzvvoe.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.bbcook.cn/Article/details/gjwvdibjp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gzyelbsph.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.vehdjk.com/Article/details/gmswerglw.sHtML

[F12] CSV 读写
来源：http://blog.bbcook.cn/Article/details/gvnfdpkeo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fktsv.cn/Article/details/godvlkcxe.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.tarul.cn/Article/details/grfztjsub.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.sjlbkw.cn/Article/details/gowbmdmdg.sHtML

TS:   // 同上
来源：http://m.share.sjlbkw.cn/Article/details/gyvltyeel.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.tarul.cn/Article/details/gogzyfdpp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.epnwcf.com/Article/details/gtekqyfyi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.bbcook.cn/Article/details/gaccuugqt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fktsv.cn/Article/details/gqhbthajs.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gixndclls.sHtML

G. 面向对象
来源：http://blog.epnwcf.com/Article/details/gqgkldlug.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gqgisvovh.sHtML

[G01] 定义类
来源：http://www.blog.yfazqb.com/Article/details/gzyvwerya.sHtML

Py:   class User: pass
来源：http://read.share.epnwcf.com/Article/details/gqlbqosam.sHtML

PHP:  class User {}
来源：http://www.blog.fktsv.cn/Article/details/gjojibphe.sHtML

JS:   class User {}
来源：http://3g.sjlbkw.cn/Article/details/gfmuhdfud.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.tarul.cn/Article/details/gtrjatrhy.sHtML

Java: class User {}
来源：http://blog.bbcook.cn/Article/details/gbtsktdyy.sHtML

Go:   type User struct { Name string }
来源：http://3g.sjlbkw.cn/Article/details/garptemxh.sHtML

Ruby: class User; end
来源：http://read.share.tarul.cn/Article/details/gbjwpewgh.sHtML

C#:   class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gunuzfriv.sHtML

[G02] 构造函数
来源：http://baike.epnwcf.com/Article/details/gjlfwgfdm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.vehdjk.com/Article/details/gbihotmbr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fktsv.cn/Article/details/gfwibxqvm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.bbcook.cn/Article/details/gyladvmxt.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gugdpckoi.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.tarul.cn/Article/details/gaftghcib.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.vehdjk.com/Article/details/gncqjboxp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.bbcook.cn/Article/details/gnkhjsrmx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.sjlbkw.cn/Article/details/geblrwpwg.sHtML

[G03] 实例属性
来源：http://www.m.share.vehdjk.com/Article/details/gtysvldsj.sHtML

Py:   self.name = "x"
来源：http://mobile.fktsv.cn/Article/details/gvksdtoop.sHtML

PHP:  public string $name = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gikujpycx.sHtML

JS:   this.name = "x";
来源：http://baike.vehdjk.com/Article/details/gaslnvlfh.sHtML

TS:   name: string = "x";
来源：http://www.m.share.tarul.cn/Article/details/gmgqdcthc.sHtML

Java: private String name;
来源：http://mobile.epnwcf.com/Article/details/gjufubgyi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.sjlbkw.cn/Article/details/gtadycgap.sHtML

Ruby: @name = "x"
来源：http://www.blog.bbcook.cn/Article/details/gvuaeppom.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.sjlbkw.cn/Article/details/gqjchyfma.sHtML

[G04] 定义方法
来源：http://read.share.vehdjk.com/Article/details/gfmfjitlq.sHtML

Py:   def greet(self): return self.name
来源：http://3g.bbcook.cn/Article/details/glvzscyko.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.sjlbkw.cn/Article/details/gyautwbuk.sHtML

JS:   greet() { return this.name; }
来源：http://3g.epnwcf.com/Article/details/gcyyqdrxm.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.bbcook.cn/Article/details/ggdjtwcmw.sHtML

Java: String greet() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/ginatovkv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.vehdjk.com/Article/details/gfquvohwr.sHtML

Ruby: def greet; @name; end
来源：http://www.share.sjlbkw.cn/Article/details/gkcqxqeua.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.vehdjk.com/Article/details/gjkmkayvi.sHtML

[G05] 继承
来源：http://www.m.share.yfazqb.com/Article/details/gxzzgrlil.sHtML

Py:   class Admin(User): pass
来源：http://3g.fktsv.cn/Article/details/gpeqorelw.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.vehdjk.com/Article/details/glijqyuqr.sHtML

JS:   class Admin extends User {}
来源：http://www.share.vehdjk.com/Article/details/govlebacg.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/ghpeqgdld.sHtML

Java: class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/gdfibgxts.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.vehdjk.com/Article/details/gpldgfvfj.sHtML

Ruby: class Admin < User; end
来源：http://mobile.vehdjk.com/Article/details/gfelcerse.sHtML

C#:   class Admin : User {}
来源：http://3g.yfazqb.com/Article/details/gjtxpaltk.sHtML

[G06] 重写方法
来源：http://wap.yfazqb.com/Article/details/gqidicdth.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.vehdjk.com/Article/details/gohgxmzuy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/gbvhusszf.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.tarul.cn/Article/details/gsjhjuydf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/glhoznqdl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/gzrncntvn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.sjlbkw.cn/Article/details/gkhctebpr.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.epnwcf.com/Article/details/gurknxmnf.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.yfazqb.com/Article/details/gvuajpltu.sHtML

[G07] 调用父类方法
来源：http://blog.yfazqb.com/Article/details/ggqkgnvtr.sHtML

Py:   super().greet()
来源：http://3g.bbcook.cn/Article/details/gqfjfsaro.sHtML

PHP:  parent::greet();
来源：http://www.share.tarul.cn/Article/details/glozcmenn.sHtML

JS:   super.greet();
来源：http://baike.yfazqb.com/Article/details/glszuitbq.sHtML

TS:   super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gpelyrgby.sHtML

Java: super.greet();
来源：http://wap.vehdjk.com/Article/details/gcwtnvoku.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.yfazqb.com/Article/details/gqrlztmwm.sHtML

Ruby: super
来源：http://blog.fktsv.cn/Article/details/gapqjnttw.sHtML

C#:   base.Greet();
来源：http://blog.tarul.cn/Article/details/gdeaxibpw.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.tarul.cn/Article/details/gfxhebohr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.epnwcf.com/Article/details/gmjiixfxi.sHtML

PHP:  public static function f() {}
来源：http://m.share.fktsv.cn/Article/details/gtorcrksn.sHtML

JS:   static f() {}
来源：http://www.share.yfazqb.com/Article/details/gcwycveom.sHtML

TS:   static f(): void {}
来源：http://read.share.sjlbkw.cn/Article/details/gedaancfr.sHtML

Java: static void f() {}
来源：http://wap.vehdjk.com/Article/details/gfzjomwnv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.yfazqb.com/Article/details/gfrjcckwc.sHtML

Ruby: def self.f; end
来源：http://mobile.epnwcf.com/Article/details/guhkgjiqa.sHtML

C#:   public static void F() {}
来源：http://www.m.share.bbcook.cn/Article/details/guhgrjxod.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.epnwcf.com/Article/details/gbglhliao.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fktsv.cn/Article/details/ghkffnkup.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fktsv.cn/Article/details/ggteqinlp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.bbcook.cn/Article/details/gqcstvvrx.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.tarul.cn/Article/details/gseklqzvh.sHtML

Java: interface Shape { double area(); }
来源：http://3g.sjlbkw.cn/Article/details/gujugakli.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.bbcook.cn/Article/details/gseafpbtx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.vehdjk.com/Article/details/guhbqwjdx.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.bbcook.cn/Article/details/gixavfaaf.sHtML

[G10] 访问控制
来源：http://m.share.yfazqb.com/Article/details/gokephizq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.yfazqb.com/Article/details/gsbfhvbxr.sHtML

PHP:  public / protected / private
来源：http://wap.epnwcf.com/Article/details/gaplsxjfw.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.tarul.cn/Article/details/gmhpudxah.sHtML

TS:   public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/gwihavrgk.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fktsv.cn/Article/details/gzgzgbulx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.sjlbkw.cn/Article/details/gtsjqrfdg.sHtML

Ruby: public / protected / private
来源：http://3g.sjlbkw.cn/Article/details/gstfxgpoo.sHtML

C#:   public / protected / private / internal
来源：http://baike.yfazqb.com/Article/details/gxhdbdhfr.sHtML

[G11] getter / setter
来源：http://www.blog.epnwcf.com/Article/details/gwsbejgnb.sHtML

Py:   @property 与 @x.setter
来源：http://blog.yfazqb.com/Article/details/gqwvgbbtx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.epnwcf.com/Article/details/gmdupdprm.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.bbcook.cn/Article/details/ghwhlnogc.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.epnwcf.com/Article/details/gedbgvhcf.sHtML

Java: public String getName() { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gkswvacdn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fktsv.cn/Article/details/gbsikpjsm.sHtML

Ruby: attr_accessor :name
来源：http://read.share.vehdjk.com/Article/details/giipboiso.sHtML

C#:   public string Name { get; set; }
来源：http://baike.epnwcf.com/Article/details/gdzqlbvdi.sHtML

[G12] 对象转字符串
来源：http://mobile.epnwcf.com/Article/details/gyfeevfnh.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.tarul.cn/Article/details/gwnewnkxv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fktsv.cn/Article/details/gehhxdisa.sHtML

JS:   toString() { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gwgvoryim.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gedfpwrxx.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsejnlloa.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.yfazqb.com/Article/details/gixhpipqo.sHtML

Ruby: def to_s; @name; end
来源：http://baike.sjlbkw.cn/Article/details/gotdabrwh.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.sjlbkw.cn/Article/details/gajrzqxxl.sHtML

[G13] 判断对象类型
来源：http://www.blog.epnwcf.com/Article/details/gqyeazqkj.sHtML

Py:   isinstance(u, User)
来源：http://3g.sjlbkw.cn/Article/details/gpmyofveu.sHtML

PHP:  $u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/gknkbbdbl.sHtML

JS:   u instanceof User
来源：http://3g.tarul.cn/Article/details/goekumyzg.sHtML

TS:   u instanceof User
来源：http://read.share.epnwcf.com/Article/details/gyludebnu.sHtML

Java: u instanceof User
来源：http://baike.epnwcf.com/Article/details/gpkfamazq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.yfazqb.com/Article/details/gvmtwtshj.sHtML

Ruby: u.is_a?(User)
来源：http://3g.sjlbkw.cn/Article/details/gwoovaesv.sHtML

C#:   u is User
来源：http://m.share.epnwcf.com/Article/details/gclagkllz.sHtML

[G14] 数据类 / record
来源：http://wap.tarul.cn/Article/details/ggvfhcgrs.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.yfazqb.com/Article/details/gwsvshejb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fktsv.cn/Article/details/gvflioarh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fktsv.cn/Article/details/gtiypawrf.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.bbcook.cn/Article/details/gekbseidi.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.yfazqb.com/Article/details/ggydzfoez.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fktsv.cn/Article/details/gyygrbhdb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.yfazqb.com/Article/details/gsymrcfwx.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.yfazqb.com/Article/details/gbovrbrut.sHtML

[G15] 枚举
来源：http://www.blog.tarul.cn/Article/details/gtowxjccp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fktsv.cn/Article/details/gwnfhgusb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.tarul.cn/Article/details/ghxvcnter.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.epnwcf.com/Article/details/gljkvcijm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.sjlbkw.cn/Article/details/gefftfyie.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.tarul.cn/Article/details/grjedkrcj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.tarul.cn/Article/details/gvnjkgoei.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.tarul.cn/Article/details/grirsbqzj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.yfazqb.com/Article/details/gzpppzpkj.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.vehdjk.com/Article/details/gxhphdpda.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.sjlbkw.cn/Article/details/gyoomdgcj.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.sjlbkw.cn/Article/details/girlyjoxk.sHtML

JS:   Object.entries(obj)
来源：http://mobile.yfazqb.com/Article/details/gkvyzjrfn.sHtML

TS:   Object.entries(obj)
来源：http://m.share.epnwcf.com/Article/details/ghoabulef.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.bbcook.cn/Article/details/ggrnjeqog.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fktsv.cn/Article/details/gconlatpy.sHtML

Ruby: obj.instance_variables
来源：http://www.share.vehdjk.com/Article/details/gpsytwiev.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fktsv.cn/Article/details/glvrprzcm.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gszyfblwp.sHtML

H. 异常与错误处理
来源：http://blog.tarul.cn/Article/details/gicldsoqo.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gdpenvspx.sHtML

[H01] try / catch 基础
来源：http://3g.epnwcf.com/Article/details/gvfmtmijo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.bbcook.cn/Article/details/gehgvudsf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gogrkojmt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.sjlbkw.cn/Article/details/gkzxlkaom.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.epnwcf.com/Article/details/gysjofrvi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.sjlbkw.cn/Article/details/ggaunlcii.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fktsv.cn/Article/details/gqaexsfez.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fktsv.cn/Article/details/gvisxjgxy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fktsv.cn/Article/details/gvghqksck.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.tarul.cn/Article/details/gksrgwtok.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.sjlbkw.cn/Article/details/gqoguohwh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gwsxwsxvo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gviqshuwz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/greomgosz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gxzhlrzvv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.bbcook.cn/Article/details/gdeuposez.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.tarul.cn/Article/details/gbqyzvofl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gwayowbbd.sHtML

[H03] 主动抛出异常
来源：http://wap.bbcook.cn/Article/details/ggzsdefca.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.epnwcf.com/Article/details/ghbmvymkf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gbbnulbow.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.vehdjk.com/Article/details/guryuvodo.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/gblvsalxo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fktsv.cn/Article/details/ghzfivpdd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.yfazqb.com/Article/details/gkccrzaid.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fktsv.cn/Article/details/gzazyxeov.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.yfazqb.com/Article/details/gqitvrnzg.sHtML

[H04] 自定义异常类型
来源：http://blog.bbcook.cn/Article/details/gsetkavju.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.bbcook.cn/Article/details/gokitafhy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fktsv.cn/Article/details/gynmuloxf.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.sjlbkw.cn/Article/details/gfocdpgqu.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.vehdjk.com/Article/details/gsrdvjiah.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fktsv.cn/Article/details/gxglcmhhw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.vehdjk.com/Article/details/gaxqxodul.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.bbcook.cn/Article/details/gtjzsgjoh.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.bbcook.cn/Article/details/gozcfkdhq.sHtML

[H05] 捕获特定类型
来源：http://mobile.vehdjk.com/Article/details/gsahhwalv.sHtML

Py:   except ValueError as e:
来源：http://blog.tarul.cn/Article/details/gszpviksw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.epnwcf.com/Article/details/gajtnbemq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.tarul.cn/Article/details/gnmmgmjqu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fktsv.cn/Article/details/gewcyyvgh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.epnwcf.com/Article/details/gcrnjnxuq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.vehdjk.com/Article/details/ghnvfdgwb.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.sjlbkw.cn/Article/details/giyibznnb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.sjlbkw.cn/Article/details/gewcpseoo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.vehdjk.com/Article/details/ghxdcihus.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.yfazqb.com/Article/details/gqoyjyzcr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.tarul.cn/Article/details/gxkhxszho.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.epnwcf.com/Article/details/gaxzjvvtc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.tarul.cn/Article/details/gtsoxubav.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.yfazqb.com/Article/details/guzozyxuk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.vehdjk.com/Article/details/gxlseaemt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.vehdjk.com/Article/details/gxiggmreu.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.epnwcf.com/Article/details/ghmdeotaj.sHtML

[H07] 断言
来源：http://www.m.share.epnwcf.com/Article/details/gsntjrfeu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.yfazqb.com/Article/details/gaedksznk.sHtML

PHP:  assert($x > 0);
来源：http://3g.bbcook.cn/Article/details/gvrfnrkdg.sHtML

JS:   console.assert(x > 0);
来源：http://blog.vehdjk.com/Article/details/gsmtbqffg.sHtML

TS:   console.assert(x > 0);
来源：http://baike.yfazqb.com/Article/details/guzwfyaqm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.yfazqb.com/Article/details/gsfdspozj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.bbcook.cn/Article/details/gsjrevyet.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.yfazqb.com/Article/details/geuswhlmt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.yfazqb.com/Article/details/gbvlcbvbc.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.bbcook.cn/Article/details/gotniflez.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.tarul.cn/Article/details/gtujcomye.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.sjlbkw.cn/Article/details/gnbliytum.sHtML

JS:   e.message;  e.stack
来源：http://blog.tarul.cn/Article/details/gzhlnrjou.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.epnwcf.com/Article/details/gclkdhodj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.yfazqb.com/Article/details/gqnkcafdv.sHtML

Go:   err.Error()
来源：http://www.m.share.yfazqb.com/Article/details/gznovaixu.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.vehdjk.com/Article/details/galhagdss.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.vehdjk.com/Article/details/gsrtxview.sHtML

[H09] 带错误码的异常
来源：http://3g.vehdjk.com/Article/details/gdalsyqcr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.tarul.cn/Article/details/gcdcumnzg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.tarul.cn/Article/details/gjuymcoxc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.sjlbkw.cn/Article/details/gtiwryuzl.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.bbcook.cn/Article/details/gchlwfgeh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.vehdjk.com/Article/details/gfqfjqbph.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.epnwcf.com/Article/details/gspyexciu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.tarul.cn/Article/details/gkzsxqcmj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.bbcook.cn/Article/details/gkhnprgaf.sHtML

[H10] 资源自动释放
来源：http://www.share.sjlbkw.cn/Article/details/gtgutykfh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.sjlbkw.cn/Article/details/gpozsorto.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fktsv.cn/Article/details/gdtpcssvm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.yfazqb.com/Article/details/gorkhfecz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.vehdjk.com/Article/details/gynjdzajs.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.epnwcf.com/Article/details/gnrdkjdlv.sHtML

Go:   defer f.Close()
来源：http://mobile.vehdjk.com/Article/details/gmjtcirqm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.tarul.cn/Article/details/gzrbjpmsr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gzmsujesl.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gouqmkugz.sHtML

I. 正则表达式
来源：http://wap.sjlbkw.cn/Article/details/gxiibgutm.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gzigskfmw.sHtML

[I01] 判断是否匹配
来源：http://blog.bbcook.cn/Article/details/ggffwqhoj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.epnwcf.com/Article/details/gozoobvda.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.yfazqb.com/Article/details/gtjvjeeum.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.epnwcf.com/Article/details/gbiecrtyt.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fktsv.cn/Article/details/ghnfhjack.sHtML


<!-- 参考信息 -->