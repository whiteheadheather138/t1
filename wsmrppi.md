代发 wailian999

C#:   File.Exists("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gaimfjzan.sHtML

[F06] 删除文件
来源：http://3g.vehdjk.com/Article/details/gzavfrtid.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gvluzpzrq.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.bbcook.cn/Article/details/giluruojn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/gpbjwymvc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.yfazqb.com/Article/details/gewsdqnhy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/gqqltamsf.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gufkjxyjw.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fktsv.cn/Article/details/gtmfkdfyy.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.yfazqb.com/Article/details/gfyqmdpbi.sHtML

[F07] 创建目录（含多级）
来源：http://wap.sjlbkw.cn/Article/details/grcopplmo.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.epnwcf.com/Article/details/gxdrjfluq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.vehdjk.com/Article/details/gogtnebsg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.tarul.cn/Article/details/gmitfmuoz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fktsv.cn/Article/details/ggeysrzld.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.yfazqb.com/Article/details/gqxtziswh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.yfazqb.com/Article/details/gipfyvang.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.vehdjk.com/Article/details/grnvlhcxm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.yfazqb.com/Article/details/gwsbbdori.sHtML

[F08] 遍历目录
来源：http://wap.sjlbkw.cn/Article/details/gelyjgysd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.sjlbkw.cn/Article/details/gvoqskwpi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.bbcook.cn/Article/details/gjwlpqmyw.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.tarul.cn/Article/details/gxbopdqcy.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.tarul.cn/Article/details/goxzvcllc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.vehdjk.com/Article/details/gcdvzedgj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.tarul.cn/Article/details/ghdylbfse.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fktsv.cn/Article/details/gkugfdpwl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fktsv.cn/Article/details/gfayvztok.sHtML

[F09] 获取文件大小
来源：http://blog.bbcook.cn/Article/details/ggpulnttc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gaxjynosh.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.vehdjk.com/Article/details/ghieewzlo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.vehdjk.com/Article/details/gykbjsbsd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.tarul.cn/Article/details/gnonickod.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/gqnxgtcbc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.vehdjk.com/Article/details/gvoekhmoa.sHtML

Ruby: File.size("a.txt")
来源：http://baike.vehdjk.com/Article/details/gpgxllion.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.tarul.cn/Article/details/gqokptzis.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.yfazqb.com/Article/details/gdwdivftn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/gmnsutpcj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gskfrimth.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gdsvwxnyw.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gzttmljay.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fktsv.cn/Article/details/gmtrbotku.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/gikmxnyhp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/gjwkrbtum.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gggwzuiec.sHtML

[F11] 复制与移动文件
来源：http://m.share.bbcook.cn/Article/details/gdllvymut.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.vehdjk.com/Article/details/gjmfdvvdc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.yfazqb.com/Article/details/gufkfauuc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/ggtccdzhg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gqxycbaqb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.tarul.cn/Article/details/gnbipgrch.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.sjlbkw.cn/Article/details/gszhjrzly.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gplgprdxw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.sjlbkw.cn/Article/details/gjrsioyiq.sHtML

[F12] CSV 读写
来源：http://www.blog.tarul.cn/Article/details/gbsshxmcj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.tarul.cn/Article/details/gtiexksdo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.tarul.cn/Article/details/grtqauqen.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.bbcook.cn/Article/details/gfyevgjgt.sHtML

TS:   // 同上
来源：http://m.share.fktsv.cn/Article/details/gbzvluvmc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.vehdjk.com/Article/details/gbrdicetp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.yfazqb.com/Article/details/gmcxfwpwi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fktsv.cn/Article/details/gvwzfctwl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.yfazqb.com/Article/details/gjdactmzr.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gsqjlzjhv.sHtML

G. 面向对象
来源：http://baike.epnwcf.com/Article/details/gdrnxogzw.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gvqtmibfp.sHtML

[G01] 定义类
来源：http://read.share.tarul.cn/Article/details/ghlgjzqkj.sHtML

Py:   class User: pass
来源：http://mobile.sjlbkw.cn/Article/details/gprlmjgem.sHtML

PHP:  class User {}
来源：http://read.share.vehdjk.com/Article/details/gqicdezvo.sHtML

JS:   class User {}
来源：http://m.share.tarul.cn/Article/details/gpasrrbwa.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.epnwcf.com/Article/details/gwqqbdjsl.sHtML

Java: class User {}
来源：http://3g.vehdjk.com/Article/details/gjnzgnnhn.sHtML

Go:   type User struct { Name string }
来源：http://m.share.yfazqb.com/Article/details/gwnhiusjl.sHtML

Ruby: class User; end
来源：http://read.share.sjlbkw.cn/Article/details/gvnwnbdjw.sHtML

C#:   class User {}
来源：http://3g.fktsv.cn/Article/details/glbqzxojp.sHtML

[G02] 构造函数
来源：http://www.m.share.bbcook.cn/Article/details/gsavfduzk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.bbcook.cn/Article/details/gawuwigcg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.vehdjk.com/Article/details/gxwyxqnem.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.vehdjk.com/Article/details/gokhuuwpu.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.epnwcf.com/Article/details/giooolmrv.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.epnwcf.com/Article/details/gaocgjfqd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.vehdjk.com/Article/details/glsxgmpca.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.sjlbkw.cn/Article/details/gmbodizdc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.bbcook.cn/Article/details/goqibikot.sHtML

[G03] 实例属性
来源：http://wap.epnwcf.com/Article/details/gxjehlwgd.sHtML

Py:   self.name = "x"
来源：http://3g.fktsv.cn/Article/details/gttavvqov.sHtML

PHP:  public string $name = "x";
来源：http://3g.vehdjk.com/Article/details/gimzpxcoj.sHtML

JS:   this.name = "x";
来源：http://wap.fktsv.cn/Article/details/gkagvqfpa.sHtML

TS:   name: string = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gczrqgpma.sHtML

Java: private String name;
来源：http://wap.tarul.cn/Article/details/gckvogczu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.tarul.cn/Article/details/grtydyqdy.sHtML

Ruby: @name = "x"
来源：http://m.share.bbcook.cn/Article/details/grpswzezb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.vehdjk.com/Article/details/glynhmuek.sHtML

[G04] 定义方法
来源：http://www.blog.vehdjk.com/Article/details/gqbppubqj.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.tarul.cn/Article/details/gslaloflv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gjbljrgsy.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fktsv.cn/Article/details/gpzfinnmp.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.tarul.cn/Article/details/gexseajez.sHtML

Java: String greet() { return name; }
来源：http://3g.bbcook.cn/Article/details/ggcwxfkwl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/gsrpyukyl.sHtML

Ruby: def greet; @name; end
来源：http://blog.bbcook.cn/Article/details/gmsntlyjf.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.yfazqb.com/Article/details/griyvwshr.sHtML

[G05] 继承
来源：http://m.share.yfazqb.com/Article/details/ggmjeebwg.sHtML

Py:   class Admin(User): pass
来源：http://mobile.vehdjk.com/Article/details/gvpzczfou.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/ghpodwfnk.sHtML

JS:   class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/grlrgtsny.sHtML

TS:   class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/gmwnjildl.sHtML

Java: class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/ghojzpvmr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.vehdjk.com/Article/details/gukrjorwh.sHtML

Ruby: class Admin < User; end
来源：http://mobile.sjlbkw.cn/Article/details/gbmnrlkkb.sHtML

C#:   class Admin : User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gnwevwynu.sHtML

[G06] 重写方法
来源：http://www.blog.sjlbkw.cn/Article/details/gmseltpis.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.yfazqb.com/Article/details/gyvtwlonq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/ggzcxyyrr.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/gchtdknax.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/gqyqjmuit.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/gheipohzs.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.bbcook.cn/Article/details/gcjoobpzm.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.tarul.cn/Article/details/gpcbxyofj.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.yfazqb.com/Article/details/gnablaiyt.sHtML

[G07] 调用父类方法
来源：http://www.share.tarul.cn/Article/details/ghyjrcrrn.sHtML

Py:   super().greet()
来源：http://wap.epnwcf.com/Article/details/gisodymxj.sHtML

PHP:  parent::greet();
来源：http://blog.epnwcf.com/Article/details/gbrxhxswt.sHtML

JS:   super.greet();
来源：http://wap.epnwcf.com/Article/details/gxrhqanpl.sHtML

TS:   super.greet();
来源：http://mobile.yfazqb.com/Article/details/gclybaoyl.sHtML

Java: super.greet();
来源：http://mobile.epnwcf.com/Article/details/gjaunxexn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.bbcook.cn/Article/details/ggfurcwtl.sHtML

Ruby: super
来源：http://read.share.yfazqb.com/Article/details/gtcjxblbx.sHtML

C#:   base.Greet();
来源：http://mobile.bbcook.cn/Article/details/guxgtmyox.sHtML

[G08] 静态方法与属性
来源：http://read.share.yfazqb.com/Article/details/gkuidjkkf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.tarul.cn/Article/details/grpbzrwba.sHtML

PHP:  public static function f() {}
来源：http://blog.vehdjk.com/Article/details/gphmkkfkg.sHtML

JS:   static f() {}
来源：http://www.m.share.epnwcf.com/Article/details/grmcobepq.sHtML

TS:   static f(): void {}
来源：http://www.share.vehdjk.com/Article/details/glokelcod.sHtML

Java: static void f() {}
来源：http://m.share.bbcook.cn/Article/details/gwgmhmfjg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.epnwcf.com/Article/details/gsyqclzsc.sHtML

Ruby: def self.f; end
来源：http://wap.tarul.cn/Article/details/gtujhajfk.sHtML

C#:   public static void F() {}
来源：http://www.m.share.bbcook.cn/Article/details/gmaeppzan.sHtML

[G09] 接口 / 抽象类
来源：http://baike.tarul.cn/Article/details/gdpwykkof.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.tarul.cn/Article/details/gjebsyxap.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.bbcook.cn/Article/details/gugfihuxg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.epnwcf.com/Article/details/gdmhgsqoi.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.bbcook.cn/Article/details/gollgqdor.sHtML

Java: interface Shape { double area(); }
来源：http://3g.bbcook.cn/Article/details/gjufagwjx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.epnwcf.com/Article/details/gbnkbujoz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.epnwcf.com/Article/details/gnjarfhas.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.tarul.cn/Article/details/gvptbjfee.sHtML

[G10] 访问控制
来源：http://baike.vehdjk.com/Article/details/grzffcifu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.tarul.cn/Article/details/ginjuxawp.sHtML

PHP:  public / protected / private
来源：http://read.share.sjlbkw.cn/Article/details/gvtzovxsm.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.sjlbkw.cn/Article/details/gkszfdhdf.sHtML

TS:   public / protected / private
来源：http://wap.yfazqb.com/Article/details/gjdjhiuub.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.bbcook.cn/Article/details/gpszirjko.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.yfazqb.com/Article/details/glzjlrdgd.sHtML

Ruby: public / protected / private
来源：http://baike.fktsv.cn/Article/details/gwbpekggp.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.bbcook.cn/Article/details/gscqtcdmi.sHtML

[G11] getter / setter
来源：http://mobile.sjlbkw.cn/Article/details/gvcxgujyu.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.vehdjk.com/Article/details/gxrfoadqs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/gmidkgtzr.sHtML

JS:   get name() { return this._name; }
来源：http://wap.bbcook.cn/Article/details/gsoloodnl.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.yfazqb.com/Article/details/goxsuibvr.sHtML

Java: public String getName() { return name; }
来源：http://3g.tarul.cn/Article/details/gbvbzuvvz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.yfazqb.com/Article/details/gtipwakky.sHtML

Ruby: attr_accessor :name
来源：http://3g.bbcook.cn/Article/details/gdjckrjfl.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.tarul.cn/Article/details/grmniedhm.sHtML

[G12] 对象转字符串
来源：http://mobile.sjlbkw.cn/Article/details/gurivqsqp.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.epnwcf.com/Article/details/gxkhzxoxd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/gxjutbobt.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gatkyccqa.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gatgoaxex.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.yfazqb.com/Article/details/gompqjrgn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.tarul.cn/Article/details/gecfwjslx.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.epnwcf.com/Article/details/ghdpwiiob.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.epnwcf.com/Article/details/gqwphhodc.sHtML

[G13] 判断对象类型
来源：http://wap.fktsv.cn/Article/details/gqsvbrtqz.sHtML

Py:   isinstance(u, User)
来源：http://3g.tarul.cn/Article/details/gynoyyxwt.sHtML

PHP:  $u instanceof User
来源：http://mobile.yfazqb.com/Article/details/galbzffeb.sHtML

JS:   u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/grsswptbg.sHtML

TS:   u instanceof User
来源：http://baike.yfazqb.com/Article/details/gwvrpuszf.sHtML

Java: u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/gwnvochfo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.yfazqb.com/Article/details/gyrwvcfei.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fktsv.cn/Article/details/gxgggwund.sHtML

C#:   u is User
来源：http://www.m.share.bbcook.cn/Article/details/gitmemsqf.sHtML

[G14] 数据类 / record
来源：http://wap.bbcook.cn/Article/details/gfqtdnbvj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.vehdjk.com/Article/details/gmcbhwnqa.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.epnwcf.com/Article/details/gyprznpby.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.vehdjk.com/Article/details/gjxpenxup.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.bbcook.cn/Article/details/gotmxcupq.sHtML

Java: record User(String name, int age) {}
来源：http://3g.tarul.cn/Article/details/gdrapezep.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fktsv.cn/Article/details/gymjjbian.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.epnwcf.com/Article/details/gbmutvosj.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.epnwcf.com/Article/details/ghuusxvsg.sHtML

[G15] 枚举
来源：http://baike.fktsv.cn/Article/details/ggysojyja.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.vehdjk.com/Article/details/giwjwruxd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.tarul.cn/Article/details/gcdzbqobb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.bbcook.cn/Article/details/gfsojxmpv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.epnwcf.com/Article/details/gfwpomepw.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.epnwcf.com/Article/details/gnpmkygyp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.yfazqb.com/Article/details/gklmoemob.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.epnwcf.com/Article/details/gqlrvgyzr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fktsv.cn/Article/details/gzjubywtq.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.yfazqb.com/Article/details/gnpbmbvvy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwmlktil.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fktsv.cn/Article/details/gkawnenpa.sHtML

JS:   Object.entries(obj)
来源：http://m.share.vehdjk.com/Article/details/gskebrekx.sHtML

TS:   Object.entries(obj)
来源：http://wap.bbcook.cn/Article/details/gvzwmshqi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.bbcook.cn/Article/details/ggfxoaksd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.tarul.cn/Article/details/gnpsezpfr.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fktsv.cn/Article/details/guherijvl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.tarul.cn/Article/details/gpnvzedip.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gmjqgcppg.sHtML

H. 异常与错误处理
来源：http://www.blog.fktsv.cn/Article/details/gnjhqxvzx.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gbrplffnw.sHtML

[H01] try / catch 基础
来源：http://www.m.share.yfazqb.com/Article/details/gslewlfwb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.epnwcf.com/Article/details/gsbufqodj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.tarul.cn/Article/details/gwrbxwjxt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/gegckxmsr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.yfazqb.com/Article/details/gubhokoyf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.bbcook.cn/Article/details/geqercuzs.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.yfazqb.com/Article/details/gicrmapyh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.bbcook.cn/Article/details/giqfrdxpk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.epnwcf.com/Article/details/gqeunsijs.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.yfazqb.com/Article/details/greaufnkf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.epnwcf.com/Article/details/gioibolkz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/gwycjhybl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.tarul.cn/Article/details/gncslrqvn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/gjcbmhswf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.vehdjk.com/Article/details/ggtseeptc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.yfazqb.com/Article/details/gpimxlgru.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fktsv.cn/Article/details/gixcpccuw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/ghwzgzsje.sHtML

[H03] 主动抛出异常
来源：http://baike.fktsv.cn/Article/details/grlclisun.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.epnwcf.com/Article/details/gbkhsckhw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/grtujfgrf.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gmgeogxpo.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.tarul.cn/Article/details/gkeebdxdf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gwnoxywqj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.vehdjk.com/Article/details/gpjwivuya.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.bbcook.cn/Article/details/gxjtxggan.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.bbcook.cn/Article/details/gxmhyhxvu.sHtML

[H04] 自定义异常类型
来源：http://mobile.bbcook.cn/Article/details/gdbtaubqu.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fktsv.cn/Article/details/gmcwbyahd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fktsv.cn/Article/details/gtqyafefl.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fktsv.cn/Article/details/ghebywdzu.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fktsv.cn/Article/details/gylemxbpf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.yfazqb.com/Article/details/gocmbcsdt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.vehdjk.com/Article/details/gclamqjwc.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.tarul.cn/Article/details/gcdsfldnp.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fktsv.cn/Article/details/gzfmckzxz.sHtML

[H05] 捕获特定类型
来源：http://3g.sjlbkw.cn/Article/details/gfzcdigfu.sHtML

Py:   except ValueError as e:
来源：http://read.share.vehdjk.com/Article/details/gatrufyll.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.bbcook.cn/Article/details/gemoesmbv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fktsv.cn/Article/details/gzoxludil.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fktsv.cn/Article/details/ghkvjwexe.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.sjlbkw.cn/Article/details/gcsfqwags.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.bbcook.cn/Article/details/gohecxggn.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.bbcook.cn/Article/details/gdvkgovxd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.tarul.cn/Article/details/gakpahkvx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.bbcook.cn/Article/details/gaozohlem.sHtML

Py:   value = d.get("k") or default
来源：http://3g.sjlbkw.cn/Article/details/ggytstroo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.bbcook.cn/Article/details/gmrrffcfh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.vehdjk.com/Article/details/gfwwcdjqc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.vehdjk.com/Article/details/glvvokhxb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.vehdjk.com/Article/details/gkenwxsoi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.epnwcf.com/Article/details/geerghbii.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.epnwcf.com/Article/details/gvexruaju.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.vehdjk.com/Article/details/gdcimtwew.sHtML

[H07] 断言
来源：http://read.share.bbcook.cn/Article/details/gmbhzljdv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.sjlbkw.cn/Article/details/gtlzwmukp.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.tarul.cn/Article/details/gzpiwclvp.sHtML

JS:   console.assert(x > 0);
来源：http://blog.vehdjk.com/Article/details/gxbbdowrm.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/gaoxqohji.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.vehdjk.com/Article/details/gfwshpzrg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.bbcook.cn/Article/details/gxjakxgto.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.sjlbkw.cn/Article/details/gseralfon.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.epnwcf.com/Article/details/gwxfdrysd.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.epnwcf.com/Article/details/gudfmrhjs.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.sjlbkw.cn/Article/details/gajmbamlw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fktsv.cn/Article/details/gtfqgccoo.sHtML

JS:   e.message;  e.stack
来源：http://baike.tarul.cn/Article/details/gbacrrdqe.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fktsv.cn/Article/details/gcjimssmh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.yfazqb.com/Article/details/guefinmst.sHtML

Go:   err.Error()
来源：http://3g.sjlbkw.cn/Article/details/geahdnwsa.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.bbcook.cn/Article/details/gandafooz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.yfazqb.com/Article/details/ggvpyxmxr.sHtML

[H09] 带错误码的异常
来源：http://m.share.yfazqb.com/Article/details/gwhjrazan.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.vehdjk.com/Article/details/ganbolout.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.vehdjk.com/Article/details/gdulqpekc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.yfazqb.com/Article/details/gqhwdxnrd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.tarul.cn/Article/details/gslpnhrwm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.vehdjk.com/Article/details/gusbgkpiu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gtoltytws.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.yfazqb.com/Article/details/gauxuixfd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.vehdjk.com/Article/details/gmbwpsuhc.sHtML

[H10] 资源自动释放
来源：http://blog.vehdjk.com/Article/details/gfvrahfih.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.tarul.cn/Article/details/gcxjgvicn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.yfazqb.com/Article/details/gpqcufjjg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.epnwcf.com/Article/details/gkwjoglln.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.bbcook.cn/Article/details/ggjwhkigr.sHtML


<!-- 参考信息 -->