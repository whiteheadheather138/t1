代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/gygdpzjyy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/gjinmxxnz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gelblrjjq.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.tarul.cn/Article/details/gpafigqva.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.tarul.cn/Article/details/granufyqy.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gunpzwhwv.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fktsv.cn/Article/details/gcuhmvqmz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.tarul.cn/Article/details/gdyumaspk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.bbcook.cn/Article/details/gumnalemt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.vehdjk.com/Article/details/gqbdgfhcb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fktsv.cn/Article/details/gbtbkebzp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.sjlbkw.cn/Article/details/gaxqkyogd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fktsv.cn/Article/details/gwonnlgeu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.sjlbkw.cn/Article/details/gdhzylpsv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.yfazqb.com/Article/details/gfjpdpxas.sHtML

[F08] 遍历目录
来源：http://mobile.vehdjk.com/Article/details/gzioymezh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.bbcook.cn/Article/details/gprwsznyg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.yfazqb.com/Article/details/gibnzciek.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fktsv.cn/Article/details/gvhmdmcgq.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.epnwcf.com/Article/details/gbtuxmhgd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.tarul.cn/Article/details/gdfjlzfrj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.epnwcf.com/Article/details/gkucrrwbo.sHtML

Ruby: Dir.children("dir")
来源：http://baike.tarul.cn/Article/details/gxhggfdpd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.bbcook.cn/Article/details/gzekhgepj.sHtML

[F09] 获取文件大小
来源：http://blog.epnwcf.com/Article/details/gjjbiedfv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gobezfdmk.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gfiqwqzzg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.bbcook.cn/Article/details/gugggmitg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.sjlbkw.cn/Article/details/gyweodpbk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gehgufbcn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.bbcook.cn/Article/details/gjvmxyfut.sHtML

Ruby: File.size("a.txt")
来源：http://baike.bbcook.cn/Article/details/gkaykuywv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fktsv.cn/Article/details/ghbczabbn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.sjlbkw.cn/Article/details/gzfabjdhd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gkkzxbqwl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gtvxamkcc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/gwtdltjlf.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gecmllfqx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.epnwcf.com/Article/details/ggfamfjch.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gyihncjkg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gsbyscxgd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gzquewojl.sHtML

[F11] 复制与移动文件
来源：http://mobile.sjlbkw.cn/Article/details/gzxubqdka.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/gbgimufjv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gphrblvxx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gyreykxrn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/guxpurvcq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.yfazqb.com/Article/details/gvglxywzd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.epnwcf.com/Article/details/gottzcjqn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gixntajgv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fktsv.cn/Article/details/gegwmwdpl.sHtML

[F12] CSV 读写
来源：http://www.blog.fktsv.cn/Article/details/gkqintzer.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.vehdjk.com/Article/details/gnalwxovc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.sjlbkw.cn/Article/details/gjvcjusrk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.epnwcf.com/Article/details/gbykfexrx.sHtML

TS:   // 同上
来源：http://blog.fktsv.cn/Article/details/gujkoxxoq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.tarul.cn/Article/details/gxswfqpry.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.bbcook.cn/Article/details/gdimumrrx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.epnwcf.com/Article/details/gmxsdixig.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.sjlbkw.cn/Article/details/grogcucxw.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/geziurhib.sHtML

G. 面向对象
来源：http://blog.sjlbkw.cn/Article/details/gtciosngl.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gaczvoroy.sHtML

[G01] 定义类
来源：http://www.share.yfazqb.com/Article/details/gstkemlde.sHtML

Py:   class User: pass
来源：http://mobile.sjlbkw.cn/Article/details/gsggenocx.sHtML

PHP:  class User {}
来源：http://3g.vehdjk.com/Article/details/gwkbwemho.sHtML

JS:   class User {}
来源：http://m.share.yfazqb.com/Article/details/gxfoweaxk.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.bbcook.cn/Article/details/gdaibmejq.sHtML

Java: class User {}
来源：http://read.share.epnwcf.com/Article/details/guhphjqsl.sHtML

Go:   type User struct { Name string }
来源：http://3g.fktsv.cn/Article/details/gsinajztz.sHtML

Ruby: class User; end
来源：http://www.m.share.vehdjk.com/Article/details/gltwfjodu.sHtML

C#:   class User {}
来源：http://www.m.share.bbcook.cn/Article/details/giqdsinin.sHtML

[G02] 构造函数
来源：http://blog.vehdjk.com/Article/details/gxmpqogbh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.epnwcf.com/Article/details/gxgorrqnr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.epnwcf.com/Article/details/gfodxuxoq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fktsv.cn/Article/details/grnnqfike.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.tarul.cn/Article/details/graycazki.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.vehdjk.com/Article/details/gofnyihfg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.epnwcf.com/Article/details/gxxlznfcu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.vehdjk.com/Article/details/gbyzzsguu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.vehdjk.com/Article/details/gskyrusaj.sHtML

[G03] 实例属性
来源：http://m.share.epnwcf.com/Article/details/giqxruvvz.sHtML

Py:   self.name = "x"
来源：http://3g.bbcook.cn/Article/details/gghdhyasg.sHtML

PHP:  public string $name = "x";
来源：http://baike.epnwcf.com/Article/details/gklljgazw.sHtML

JS:   this.name = "x";
来源：http://read.share.fktsv.cn/Article/details/gqdiyvewk.sHtML

TS:   name: string = "x";
来源：http://read.share.bbcook.cn/Article/details/gojtdbbwg.sHtML

Java: private String name;
来源：http://baike.bbcook.cn/Article/details/grajzegik.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fktsv.cn/Article/details/gwwndvtba.sHtML

Ruby: @name = "x"
来源：http://www.m.share.epnwcf.com/Article/details/gctvtwqvc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.sjlbkw.cn/Article/details/gnciboops.sHtML

[G04] 定义方法
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdbfvddb.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.yfazqb.com/Article/details/gxtteffqy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.tarul.cn/Article/details/gvmvrrrbr.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/gcrvrjlcg.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.tarul.cn/Article/details/gdwirpyju.sHtML

Java: String greet() { return name; }
来源：http://baike.bbcook.cn/Article/details/gtmcaimea.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/gywuilclq.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gjsbdhizw.sHtML

C#:   public string Greet() => Name;
来源：http://baike.sjlbkw.cn/Article/details/gkqiwmphb.sHtML

[G05] 继承
来源：http://www.m.share.epnwcf.com/Article/details/gbydffgnr.sHtML

Py:   class Admin(User): pass
来源：http://mobile.epnwcf.com/Article/details/glvlsytmb.sHtML

PHP:  class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gmciedmwo.sHtML

JS:   class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/gjzcodgib.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.yfazqb.com/Article/details/gatfynfmu.sHtML

Java: class Admin extends User {}
来源：http://www.share.vehdjk.com/Article/details/gzmyhhvpi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.tarul.cn/Article/details/gynjvasfh.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.vehdjk.com/Article/details/gfywgeskf.sHtML

C#:   class Admin : User {}
来源：http://www.blog.epnwcf.com/Article/details/gbfgmomir.sHtML

[G06] 重写方法
来源：http://www.m.share.tarul.cn/Article/details/gezeivjbq.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.sjlbkw.cn/Article/details/gsyrfnyik.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gyhqfaicx.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/ghvbfqypq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/gsdaknhle.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.yfazqb.com/Article/details/gpqwyjoqk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.bbcook.cn/Article/details/gptiszqhg.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.vehdjk.com/Article/details/gchzhngao.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.tarul.cn/Article/details/gjxreflxa.sHtML

[G07] 调用父类方法
来源：http://www.blog.yfazqb.com/Article/details/gutsdtjxa.sHtML

Py:   super().greet()
来源：http://wap.bbcook.cn/Article/details/gldusctkq.sHtML

PHP:  parent::greet();
来源：http://wap.vehdjk.com/Article/details/gsdphyydq.sHtML

JS:   super.greet();
来源：http://3g.sjlbkw.cn/Article/details/gbeokaetn.sHtML

TS:   super.greet();
来源：http://read.share.vehdjk.com/Article/details/goqafaatw.sHtML

Java: super.greet();
来源：http://3g.vehdjk.com/Article/details/gmkqoyhah.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.bbcook.cn/Article/details/gvotxrvdf.sHtML

Ruby: super
来源：http://3g.bbcook.cn/Article/details/gkkrwtwme.sHtML

C#:   base.Greet();
来源：http://baike.epnwcf.com/Article/details/gzijvedjb.sHtML

[G08] 静态方法与属性
来源：http://blog.tarul.cn/Article/details/gdsljblim.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.bbcook.cn/Article/details/gewyfbres.sHtML

PHP:  public static function f() {}
来源：http://3g.vehdjk.com/Article/details/gwwtlddia.sHtML

JS:   static f() {}
来源：http://wap.vehdjk.com/Article/details/gwzfaylbd.sHtML

TS:   static f(): void {}
来源：http://blog.sjlbkw.cn/Article/details/gnrsmooga.sHtML

Java: static void f() {}
来源：http://read.share.tarul.cn/Article/details/guzrpwbmm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.epnwcf.com/Article/details/gljmdptyg.sHtML

Ruby: def self.f; end
来源：http://www.share.yfazqb.com/Article/details/gmnsoinoi.sHtML

C#:   public static void F() {}
来源：http://m.share.yfazqb.com/Article/details/gefkgckvw.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.bbcook.cn/Article/details/grxxcijqd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.tarul.cn/Article/details/gboilblsf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gywhsniyp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.vehdjk.com/Article/details/gfpbgxtyg.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.bbcook.cn/Article/details/guoejzbgp.sHtML

Java: interface Shape { double area(); }
来源：http://wap.bbcook.cn/Article/details/gxfbyycaw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.epnwcf.com/Article/details/gjptbhcfz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.bbcook.cn/Article/details/gwbpzyqdv.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.bbcook.cn/Article/details/guukgtjkq.sHtML

[G10] 访问控制
来源：http://blog.tarul.cn/Article/details/galjorpzz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.vehdjk.com/Article/details/ggbauhscp.sHtML

PHP:  public / protected / private
来源：http://www.share.vehdjk.com/Article/details/gfkuryimv.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.epnwcf.com/Article/details/gnbpeoexy.sHtML

TS:   public / protected / private
来源：http://www.m.share.fktsv.cn/Article/details/gmzbverbu.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.vehdjk.com/Article/details/glcwghhzr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.sjlbkw.cn/Article/details/galvitskj.sHtML

Ruby: public / protected / private
来源：http://3g.yfazqb.com/Article/details/gmrfpjviz.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fktsv.cn/Article/details/gdtydgtiw.sHtML

[G11] getter / setter
来源：http://www.m.share.yfazqb.com/Article/details/gnwhfhxlg.sHtML

Py:   @property 与 @x.setter
来源：http://baike.vehdjk.com/Article/details/gzmzudluv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.vehdjk.com/Article/details/gqjeanguf.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fktsv.cn/Article/details/gojzupiok.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.sjlbkw.cn/Article/details/gzwxcwrax.sHtML

Java: public String getName() { return name; }
来源：http://3g.epnwcf.com/Article/details/gywaumoot.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.bbcook.cn/Article/details/gjwdtvrxy.sHtML

Ruby: attr_accessor :name
来源：http://m.share.vehdjk.com/Article/details/gomhxiwgx.sHtML

C#:   public string Name { get; set; }
来源：http://3g.sjlbkw.cn/Article/details/gysmcnwqr.sHtML

[G12] 对象转字符串
来源：http://blog.fktsv.cn/Article/details/gzrzyxjki.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.epnwcf.com/Article/details/gzswotvbo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.vehdjk.com/Article/details/gxkxkyljd.sHtML

JS:   toString() { return this.name; }
来源：http://baike.tarul.cn/Article/details/gptpkxnzu.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.vehdjk.com/Article/details/gloizcgfz.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fktsv.cn/Article/details/glrhofxss.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.tarul.cn/Article/details/gtzzbkrmw.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fktsv.cn/Article/details/gttnnbjmi.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.epnwcf.com/Article/details/gutfetdfw.sHtML

[G13] 判断对象类型
来源：http://mobile.fktsv.cn/Article/details/gnyquursh.sHtML

Py:   isinstance(u, User)
来源：http://read.share.bbcook.cn/Article/details/gesmbhwhg.sHtML

PHP:  $u instanceof User
来源：http://m.share.epnwcf.com/Article/details/gvaffhsvw.sHtML

JS:   u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gurnmylbz.sHtML

TS:   u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/glujinkzb.sHtML

Java: u instanceof User
来源：http://3g.sjlbkw.cn/Article/details/gdylkfvzx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.epnwcf.com/Article/details/gkadulyyo.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fktsv.cn/Article/details/gsbnzkjmv.sHtML

C#:   u is User
来源：http://read.share.vehdjk.com/Article/details/gjnbfhtjp.sHtML

[G14] 数据类 / record
来源：http://www.blog.yfazqb.com/Article/details/ghfrjumad.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.epnwcf.com/Article/details/grgfidqzu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.sjlbkw.cn/Article/details/gqcmadmkp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.vehdjk.com/Article/details/gstskpcmk.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.tarul.cn/Article/details/gvyhuafcv.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fktsv.cn/Article/details/gicjpnvlx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fktsv.cn/Article/details/gjtyvfdty.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.vehdjk.com/Article/details/gfvmgqavx.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fktsv.cn/Article/details/guhmkmwxo.sHtML

[G15] 枚举
来源：http://m.share.yfazqb.com/Article/details/gctnxpgnv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fktsv.cn/Article/details/ggbejihvj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.yfazqb.com/Article/details/givimzxzo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.sjlbkw.cn/Article/details/gvjmlhpfn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.bbcook.cn/Article/details/gefassmpm.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.epnwcf.com/Article/details/gygincpsq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.vehdjk.com/Article/details/gwgjftyup.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fktsv.cn/Article/details/gzkefjavp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.sjlbkw.cn/Article/details/gquhrsxds.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.bbcook.cn/Article/details/gatzsbljm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.tarul.cn/Article/details/gloeqdtpu.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.tarul.cn/Article/details/gymitajce.sHtML

JS:   Object.entries(obj)
来源：http://read.share.bbcook.cn/Article/details/gcexspuyr.sHtML

TS:   Object.entries(obj)
来源：http://blog.tarul.cn/Article/details/gfgpafvbw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.vehdjk.com/Article/details/gejcdaxzn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.vehdjk.com/Article/details/gssltundn.sHtML

Ruby: obj.instance_variables
来源：http://wap.bbcook.cn/Article/details/gcjfmcniy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.yfazqb.com/Article/details/glyzlnnwi.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/ganrzkpad.sHtML

H. 异常与错误处理
来源：http://blog.epnwcf.com/Article/details/grospyezi.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gempmoraz.sHtML

[H01] try / catch 基础
来源：http://3g.epnwcf.com/Article/details/gxknjvsee.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.epnwcf.com/Article/details/gtrfujluy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.sjlbkw.cn/Article/details/ggvtzkuhl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fktsv.cn/Article/details/grfhqeqrj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fktsv.cn/Article/details/gzwjfaoeq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fktsv.cn/Article/details/gxpchvrxx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fktsv.cn/Article/details/gmrgunzfk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.tarul.cn/Article/details/gtcnebqsj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fktsv.cn/Article/details/gdojxgrjo.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.tarul.cn/Article/details/gtbaprodv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.epnwcf.com/Article/details/gbiilyten.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/gokcqfsaj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gchcnreya.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/gjakehfcq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/gtotgdvpm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.epnwcf.com/Article/details/gyewqzgpl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fktsv.cn/Article/details/gairhemwj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdicyfxkd.sHtML

[H03] 主动抛出异常
来源：http://wap.yfazqb.com/Article/details/gwjmperfc.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.yfazqb.com/Article/details/gextfonwj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.tarul.cn/Article/details/gwkmhpjxa.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/giodpgmed.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.epnwcf.com/Article/details/gbyzixatc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.yfazqb.com/Article/details/gnemttewh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.bbcook.cn/Article/details/gxkbrzqfc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.tarul.cn/Article/details/gzyiwnrif.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/gpxjnmsxi.sHtML

[H04] 自定义异常类型
来源：http://baike.vehdjk.com/Article/details/ghvverblp.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fktsv.cn/Article/details/gvereeymh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fktsv.cn/Article/details/gsaqgpakg.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.bbcook.cn/Article/details/ggeezkddd.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.bbcook.cn/Article/details/gemwddyfh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.yfazqb.com/Article/details/gnwpihevh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.yfazqb.com/Article/details/gbubqbqwo.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.yfazqb.com/Article/details/gxnhctdda.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.yfazqb.com/Article/details/gtdrgcneh.sHtML

[H05] 捕获特定类型
来源：http://wap.fktsv.cn/Article/details/gyhgujmji.sHtML

Py:   except ValueError as e:
来源：http://www.blog.epnwcf.com/Article/details/gydmynoka.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.tarul.cn/Article/details/gcpssvzgi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.yfazqb.com/Article/details/gaflgalvg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.epnwcf.com/Article/details/goiqkwock.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.tarul.cn/Article/details/gjjxnggmv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.yfazqb.com/Article/details/gtumkrvxd.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.yfazqb.com/Article/details/gyyvxzdby.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.tarul.cn/Article/details/grzxbpwkg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.yfazqb.com/Article/details/gwagmnhpl.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.epnwcf.com/Article/details/gfbiuatji.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.epnwcf.com/Article/details/gymwfgvmq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.vehdjk.com/Article/details/glbjrpwxp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fktsv.cn/Article/details/gwriahdxb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.bbcook.cn/Article/details/gvsrrgdki.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.epnwcf.com/Article/details/gtqqjsatk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.sjlbkw.cn/Article/details/gfzoitdgn.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.vehdjk.com/Article/details/gftcibwxe.sHtML

[H07] 断言
来源：http://baike.vehdjk.com/Article/details/ggkjtvuzx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.tarul.cn/Article/details/gxsusithb.sHtML

PHP:  assert($x > 0);
来源：http://3g.fktsv.cn/Article/details/glbrvljrl.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.yfazqb.com/Article/details/gtcqjmqrd.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.bbcook.cn/Article/details/gkshkjuus.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.epnwcf.com/Article/details/gofhgrpkd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.sjlbkw.cn/Article/details/gbsndyxiz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.tarul.cn/Article/details/gcppqnwwi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.epnwcf.com/Article/details/gdxlqavde.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.sjlbkw.cn/Article/details/gljgfadhv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.epnwcf.com/Article/details/gsgrhonyn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.sjlbkw.cn/Article/details/grgifykbr.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.sjlbkw.cn/Article/details/girmrgzer.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.epnwcf.com/Article/details/grvmpdwso.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.bbcook.cn/Article/details/gwcqfxsmj.sHtML

Go:   err.Error()
来源：http://m.share.fktsv.cn/Article/details/gaejmgtnk.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.yfazqb.com/Article/details/gmynydlsk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.yfazqb.com/Article/details/ggmbijiff.sHtML

[H09] 带错误码的异常
来源：http://blog.bbcook.cn/Article/details/gaqqvbatb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.tarul.cn/Article/details/gxgexsttp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.tarul.cn/Article/details/gufjbozpf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.tarul.cn/Article/details/gdwbjyhzz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.bbcook.cn/Article/details/gbnzeydpj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.epnwcf.com/Article/details/gqyvpwumx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.yfazqb.com/Article/details/gjgnhwikv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.epnwcf.com/Article/details/gwpnqlgys.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.epnwcf.com/Article/details/gnvkxryai.sHtML

[H10] 资源自动释放
来源：http://blog.fktsv.cn/Article/details/gvgvounqp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.tarul.cn/Article/details/gemhipool.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fktsv.cn/Article/details/gfhxbjngc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.epnwcf.com/Article/details/gkvusaknf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.vehdjk.com/Article/details/gsfranxeh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.yfazqb.com/Article/details/gelbjvmgz.sHtML

Go:   defer f.Close()
来源：http://www.share.yfazqb.com/Article/details/gknhgsqlm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.sjlbkw.cn/Article/details/gsfyrggfa.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gcwuvfscz.sHtML


<!-- 参考信息 -->