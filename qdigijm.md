代发 wailian999

C#:   File.Exists("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gzkvmpzze.sHtML

[F06] 删除文件
来源：http://read.share.yfazqb.com/Article/details/gwgcjediz.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gooaxbqpc.sHtML

PHP:  unlink("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gkinhgcfh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.epnwcf.com/Article/details/gxkhfhdra.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gzlpzrnls.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fktsv.cn/Article/details/grylwvmvk.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.tarul.cn/Article/details/geknolfmm.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gkwnrvwnq.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gtwwhegmf.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.tarul.cn/Article/details/gusdiuoom.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.vehdjk.com/Article/details/geleefeko.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fktsv.cn/Article/details/gvyjoluxd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.sjlbkw.cn/Article/details/giwwegabx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.epnwcf.com/Article/details/gogyjhgoj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.vehdjk.com/Article/details/gdxuibvbg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.sjlbkw.cn/Article/details/gwzqzwmwx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.yfazqb.com/Article/details/gszfbetwf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.yfazqb.com/Article/details/gbkwjvrcu.sHtML

[F08] 遍历目录
来源：http://mobile.yfazqb.com/Article/details/gvoukjzqf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.sjlbkw.cn/Article/details/geailhkte.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gflkfuxxe.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.vehdjk.com/Article/details/gswqntqzp.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.vehdjk.com/Article/details/gsgmwcyxr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fktsv.cn/Article/details/gpxijnrdb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.bbcook.cn/Article/details/gzootwkby.sHtML

Ruby: Dir.children("dir")
来源：http://baike.vehdjk.com/Article/details/ggplfrztq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.vehdjk.com/Article/details/gvflagfuy.sHtML

[F09] 获取文件大小
来源：http://www.share.yfazqb.com/Article/details/gorukvnqp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fktsv.cn/Article/details/gsudhhzuz.sHtML

PHP:  filesize("a.txt");
来源：http://wap.yfazqb.com/Article/details/ghinwtlws.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.tarul.cn/Article/details/groehnhji.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.yfazqb.com/Article/details/gkxkiqvuq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gchuyzmhc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.bbcook.cn/Article/details/grqwfcylw.sHtML

Ruby: File.size("a.txt")
来源：http://baike.tarul.cn/Article/details/gtzlaysok.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fktsv.cn/Article/details/ggmeuqyia.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.tarul.cn/Article/details/gadojrzbh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/glofzlvlm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.epnwcf.com/Article/details/gjovyqher.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gbipwxwcz.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gvtznzpgq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.yfazqb.com/Article/details/gcnvqprbm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gmkdhnecz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gewnmhnmq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gncgfldpx.sHtML

[F11] 复制与移动文件
来源：http://wap.bbcook.cn/Article/details/gxbnejddc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/ggebxluva.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fktsv.cn/Article/details/grsmsbenw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.bbcook.cn/Article/details/gonxtlosi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/gfgyhyiol.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.sjlbkw.cn/Article/details/gdwtekygb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fktsv.cn/Article/details/gjaariuor.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/gqsbzeubb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.tarul.cn/Article/details/gwjfvraji.sHtML

[F12] CSV 读写
来源：http://m.share.yfazqb.com/Article/details/gzuuupfkl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.yfazqb.com/Article/details/guxgjtrel.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.sjlbkw.cn/Article/details/geohnfgpe.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.epnwcf.com/Article/details/gnhbxjdmo.sHtML

TS:   // 同上
来源：http://3g.fktsv.cn/Article/details/gsuizdcka.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.tarul.cn/Article/details/gvanrucvr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.epnwcf.com/Article/details/grkqiumsz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.sjlbkw.cn/Article/details/gtctdlnpp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.bbcook.cn/Article/details/gajmchwea.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/genrwbkcc.sHtML

G. 面向对象
来源：http://3g.yfazqb.com/Article/details/gxaggdpme.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gqwmukrot.sHtML

[G01] 定义类
来源：http://m.share.vehdjk.com/Article/details/gorjeovte.sHtML

Py:   class User: pass
来源：http://blog.sjlbkw.cn/Article/details/ggkbepjvf.sHtML

PHP:  class User {}
来源：http://www.blog.fktsv.cn/Article/details/gilihpnyg.sHtML

JS:   class User {}
来源：http://www.share.vehdjk.com/Article/details/gzhagvyig.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.bbcook.cn/Article/details/gkrjhugma.sHtML

Java: class User {}
来源：http://blog.yfazqb.com/Article/details/gcfawponb.sHtML

Go:   type User struct { Name string }
来源：http://3g.vehdjk.com/Article/details/gmzpwlsfp.sHtML

Ruby: class User; end
来源：http://blog.vehdjk.com/Article/details/gcftavgns.sHtML

C#:   class User {}
来源：http://3g.epnwcf.com/Article/details/gstihxsmu.sHtML

[G02] 构造函数
来源：http://mobile.vehdjk.com/Article/details/gwkuodgms.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.epnwcf.com/Article/details/gdnlssncc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fktsv.cn/Article/details/ggxaxzwis.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.vehdjk.com/Article/details/gxfqxcofz.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.epnwcf.com/Article/details/gsjxrjcos.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.vehdjk.com/Article/details/gdbthkhld.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.vehdjk.com/Article/details/gcmcnnlmp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.epnwcf.com/Article/details/gqjojwpun.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.epnwcf.com/Article/details/gkbiznuok.sHtML

[G03] 实例属性
来源：http://read.share.tarul.cn/Article/details/garithqfj.sHtML

Py:   self.name = "x"
来源：http://www.blog.tarul.cn/Article/details/gwhpwlxdr.sHtML

PHP:  public string $name = "x";
来源：http://m.share.tarul.cn/Article/details/gpbuioaaz.sHtML

JS:   this.name = "x";
来源：http://baike.tarul.cn/Article/details/gousdfoja.sHtML

TS:   name: string = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gxtdogjlb.sHtML

Java: private String name;
来源：http://mobile.epnwcf.com/Article/details/gcvzhvafh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.vehdjk.com/Article/details/gotjupwte.sHtML

Ruby: @name = "x"
来源：http://www.m.share.yfazqb.com/Article/details/grmeokeoe.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.epnwcf.com/Article/details/gngnzrwkv.sHtML

[G04] 定义方法
来源：http://wap.fktsv.cn/Article/details/gdxtmeytj.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.vehdjk.com/Article/details/gotemlwly.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.vehdjk.com/Article/details/gmemebooh.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/gqopibbqu.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.epnwcf.com/Article/details/giybhcosz.sHtML

Java: String greet() { return name; }
来源：http://mobile.fktsv.cn/Article/details/gndovgarb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fktsv.cn/Article/details/gggttmxit.sHtML

Ruby: def greet; @name; end
来源：http://wap.epnwcf.com/Article/details/gugtbtjaj.sHtML

C#:   public string Greet() => Name;
来源：http://baike.vehdjk.com/Article/details/guafvzqgf.sHtML

[G05] 继承
来源：http://wap.bbcook.cn/Article/details/gctbjvrwp.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.vehdjk.com/Article/details/gvszifxlj.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.vehdjk.com/Article/details/ghptcckjo.sHtML

JS:   class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/gddbxdmsw.sHtML

TS:   class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gnsxcxfxe.sHtML

Java: class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gbxujrxtm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fktsv.cn/Article/details/glfyryurf.sHtML

Ruby: class Admin < User; end
来源：http://wap.sjlbkw.cn/Article/details/gywyzequd.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.bbcook.cn/Article/details/gkpoakogw.sHtML

[G06] 重写方法
来源：http://read.share.fktsv.cn/Article/details/gwimbgpnz.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.sjlbkw.cn/Article/details/gcwhnytle.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/gblyhdjxp.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gtyjjpnzi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/gcvlcomft.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/gzoiqrsao.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.sjlbkw.cn/Article/details/ggnbkgzme.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.sjlbkw.cn/Article/details/ggbdlizlm.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.sjlbkw.cn/Article/details/gsbhabagu.sHtML

[G07] 调用父类方法
来源：http://read.share.sjlbkw.cn/Article/details/gvchrjaph.sHtML

Py:   super().greet()
来源：http://m.share.sjlbkw.cn/Article/details/gfhfqtjsj.sHtML

PHP:  parent::greet();
来源：http://www.blog.sjlbkw.cn/Article/details/gosyzemxa.sHtML

JS:   super.greet();
来源：http://www.m.share.bbcook.cn/Article/details/ghyayqizx.sHtML

TS:   super.greet();
来源：http://read.share.epnwcf.com/Article/details/gycvfafrv.sHtML

Java: super.greet();
来源：http://wap.fktsv.cn/Article/details/gpcvmmkfi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.yfazqb.com/Article/details/gowoewnhm.sHtML

Ruby: super
来源：http://www.m.share.fktsv.cn/Article/details/ggpalrthl.sHtML

C#:   base.Greet();
来源：http://baike.tarul.cn/Article/details/gmdyrqucu.sHtML

[G08] 静态方法与属性
来源：http://m.share.vehdjk.com/Article/details/gxbwffyul.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fktsv.cn/Article/details/gorthscfg.sHtML

PHP:  public static function f() {}
来源：http://m.share.bbcook.cn/Article/details/ginpnyjjj.sHtML

JS:   static f() {}
来源：http://www.share.fktsv.cn/Article/details/gbopyacpp.sHtML

TS:   static f(): void {}
来源：http://www.m.share.vehdjk.com/Article/details/gteonaowh.sHtML

Java: static void f() {}
来源：http://mobile.fktsv.cn/Article/details/gdodueenq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.sjlbkw.cn/Article/details/grabdpudk.sHtML

Ruby: def self.f; end
来源：http://mobile.sjlbkw.cn/Article/details/glsrylixy.sHtML

C#:   public static void F() {}
来源：http://3g.sjlbkw.cn/Article/details/gigmzamgr.sHtML

[G09] 接口 / 抽象类
来源：http://baike.tarul.cn/Article/details/gwhmefqny.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.vehdjk.com/Article/details/gwitehgaf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.vehdjk.com/Article/details/gfgigwdqa.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.yfazqb.com/Article/details/gkffjjght.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.yfazqb.com/Article/details/gdapxadzp.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.tarul.cn/Article/details/gmdoizqon.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.bbcook.cn/Article/details/gtoxkyfye.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.tarul.cn/Article/details/gsrqmjjkr.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.yfazqb.com/Article/details/gwbckrrjx.sHtML

[G10] 访问控制
来源：http://blog.bbcook.cn/Article/details/gyassmazf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.epnwcf.com/Article/details/gleqbxwlx.sHtML

PHP:  public / protected / private
来源：http://wap.sjlbkw.cn/Article/details/gjtrdnrqp.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.sjlbkw.cn/Article/details/gpmcmgotp.sHtML

TS:   public / protected / private
来源：http://baike.sjlbkw.cn/Article/details/gcbplcpdc.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fktsv.cn/Article/details/ghufiwani.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.bbcook.cn/Article/details/gfoqtgqvx.sHtML

Ruby: public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/guqobafey.sHtML

C#:   public / protected / private / internal
来源：http://wap.vehdjk.com/Article/details/ghvxzuakx.sHtML

[G11] getter / setter
来源：http://3g.sjlbkw.cn/Article/details/guicqkleu.sHtML

Py:   @property 与 @x.setter
来源：http://baike.tarul.cn/Article/details/gcfjvjgez.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.tarul.cn/Article/details/gyogphtgy.sHtML

JS:   get name() { return this._name; }
来源：http://3g.bbcook.cn/Article/details/giumpgpur.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.epnwcf.com/Article/details/gnntzadcw.sHtML

Java: public String getName() { return name; }
来源：http://read.share.vehdjk.com/Article/details/gmwpuesmo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.bbcook.cn/Article/details/gnuxajjbq.sHtML

Ruby: attr_accessor :name
来源：http://blog.yfazqb.com/Article/details/gvmuwxlve.sHtML

C#:   public string Name { get; set; }
来源：http://wap.vehdjk.com/Article/details/gdnmiqksx.sHtML

[G12] 对象转字符串
来源：http://3g.fktsv.cn/Article/details/gsctlubid.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.sjlbkw.cn/Article/details/gdrihvxwu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.epnwcf.com/Article/details/gtuvlfqsl.sHtML

JS:   toString() { return this.name; }
来源：http://3g.yfazqb.com/Article/details/gatwtyyql.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/goflfqgie.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gcgiymqql.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/godiztoio.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.epnwcf.com/Article/details/gjldnswul.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.bbcook.cn/Article/details/goptmxthc.sHtML

[G13] 判断对象类型
来源：http://www.blog.sjlbkw.cn/Article/details/gbllndvzt.sHtML

Py:   isinstance(u, User)
来源：http://baike.yfazqb.com/Article/details/gqdiiedkk.sHtML

PHP:  $u instanceof User
来源：http://www.share.vehdjk.com/Article/details/gqgqmlfta.sHtML

JS:   u instanceof User
来源：http://read.share.vehdjk.com/Article/details/ggddtymjp.sHtML

TS:   u instanceof User
来源：http://wap.epnwcf.com/Article/details/gffeyjgdj.sHtML

Java: u instanceof User
来源：http://mobile.vehdjk.com/Article/details/gslvemzdu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.epnwcf.com/Article/details/goeymowka.sHtML

Ruby: u.is_a?(User)
来源：http://blog.epnwcf.com/Article/details/gkutaaqfn.sHtML

C#:   u is User
来源：http://read.share.epnwcf.com/Article/details/gedtzslfv.sHtML

[G14] 数据类 / record
来源：http://mobile.tarul.cn/Article/details/guhkbwlen.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fktsv.cn/Article/details/gtnxceakr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fktsv.cn/Article/details/gfgpvijzm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.bbcook.cn/Article/details/gpfvjkeon.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fktsv.cn/Article/details/gviayotsk.sHtML

Java: record User(String name, int age) {}
来源：http://3g.yfazqb.com/Article/details/gfffggkss.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.vehdjk.com/Article/details/gupjawfxi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fktsv.cn/Article/details/gkqqkdsya.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fktsv.cn/Article/details/gaxiasqyc.sHtML

[G15] 枚举
来源：http://read.share.yfazqb.com/Article/details/gtmfhilrv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fktsv.cn/Article/details/gvfwmjnfq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fktsv.cn/Article/details/gokzmwgzx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.tarul.cn/Article/details/gkzpxknif.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.yfazqb.com/Article/details/gktytuubb.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.tarul.cn/Article/details/gjaarvfuk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.yfazqb.com/Article/details/gsmpqivai.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.tarul.cn/Article/details/gxmkhflvm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.bbcook.cn/Article/details/gdesbwoie.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.tarul.cn/Article/details/glidjlugp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.sjlbkw.cn/Article/details/gcpunrmms.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.vehdjk.com/Article/details/gabmfxmqc.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fktsv.cn/Article/details/gwbneconf.sHtML

TS:   Object.entries(obj)
来源：http://www.share.tarul.cn/Article/details/gedlhkzwz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.yfazqb.com/Article/details/gnmdzmtvr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.tarul.cn/Article/details/gcewibvhl.sHtML

Ruby: obj.instance_variables
来源：http://www.share.yfazqb.com/Article/details/gsomljbvt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.yfazqb.com/Article/details/gzknhjdmg.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gxrpvdmfr.sHtML

H. 异常与错误处理
来源：http://www.blog.vehdjk.com/Article/details/gzmvsrbcd.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gpxpkwwgp.sHtML

[H01] try / catch 基础
来源：http://www.share.fktsv.cn/Article/details/gjjezyksv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.sjlbkw.cn/Article/details/gmuuwevzl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/glekwiewn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.yfazqb.com/Article/details/gqmwcupcr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.bbcook.cn/Article/details/gfgdiozfn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fktsv.cn/Article/details/gojahsipi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.yfazqb.com/Article/details/gnzeirmrk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.bbcook.cn/Article/details/geaxqqouu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.tarul.cn/Article/details/gqwriamao.sHtML

[H02] finally / ensure 收尾
来源：http://3g.sjlbkw.cn/Article/details/gmsakrrci.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.tarul.cn/Article/details/gljusnhvp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gebnkiozk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gcymxodjl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.epnwcf.com/Article/details/glafiawae.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/gpuwsmyyk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.epnwcf.com/Article/details/ggxpqotqh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.yfazqb.com/Article/details/gdnlvrhpd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gjlbcnejq.sHtML

[H03] 主动抛出异常
来源：http://mobile.epnwcf.com/Article/details/gzgaxxepu.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.epnwcf.com/Article/details/gtvuhlowl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.yfazqb.com/Article/details/gjrxvruyu.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/gkfsahvop.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/gqckvscqk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.bbcook.cn/Article/details/ghhfbbnmy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.vehdjk.com/Article/details/gdhpmtarw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.bbcook.cn/Article/details/gjgetgurf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gfbcuqyak.sHtML

[H04] 自定义异常类型
来源：http://3g.fktsv.cn/Article/details/gysejclbx.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.epnwcf.com/Article/details/gnzymyznn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fktsv.cn/Article/details/gixlzgjpo.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.bbcook.cn/Article/details/gocwayrkw.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.vehdjk.com/Article/details/godhkanma.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.bbcook.cn/Article/details/gggycprgj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.tarul.cn/Article/details/geveikxoi.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.epnwcf.com/Article/details/ggvdhhtpy.sHtML

C#:   class MyException : Exception {}
来源：http://baike.vehdjk.com/Article/details/gqaetzybk.sHtML

[H05] 捕获特定类型
来源：http://read.share.sjlbkw.cn/Article/details/gesqbhdxn.sHtML

Py:   except ValueError as e:
来源：http://wap.yfazqb.com/Article/details/gbjwxvmhz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.bbcook.cn/Article/details/gdnvahuyq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gjapiyhkp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.yfazqb.com/Article/details/gcmvtpxym.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.vehdjk.com/Article/details/gvuonzrem.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.vehdjk.com/Article/details/gwzitjvbk.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.tarul.cn/Article/details/gwxjdriil.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.yfazqb.com/Article/details/gvfmqirnf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.yfazqb.com/Article/details/glfelcozv.sHtML

Py:   value = d.get("k") or default
来源：http://wap.vehdjk.com/Article/details/gtohcznkx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.yfazqb.com/Article/details/gzcfuijlq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.vehdjk.com/Article/details/gfwqlmwju.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.epnwcf.com/Article/details/ggtxfhwld.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.vehdjk.com/Article/details/gxjoarsjt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.vehdjk.com/Article/details/gajlvgjxr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.bbcook.cn/Article/details/gcphkqdki.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fktsv.cn/Article/details/gdhqenada.sHtML

[H07] 断言
来源：http://m.share.fktsv.cn/Article/details/gespuvuem.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fktsv.cn/Article/details/gfgiymijm.sHtML

PHP:  assert($x > 0);
来源：http://m.share.bbcook.cn/Article/details/gjpgiqfld.sHtML

JS:   console.assert(x > 0);
来源：http://baike.bbcook.cn/Article/details/gknptkhay.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fktsv.cn/Article/details/gbktgismb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.vehdjk.com/Article/details/gladgzoag.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.epnwcf.com/Article/details/giqabzfrj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.yfazqb.com/Article/details/gexnahsbn.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.tarul.cn/Article/details/gdfhpofoy.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fktsv.cn/Article/details/giuliahjs.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.vehdjk.com/Article/details/gtjwguxox.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.yfazqb.com/Article/details/gruzipuof.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.bbcook.cn/Article/details/gqlwhdnpt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.vehdjk.com/Article/details/gbcrkzshq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.vehdjk.com/Article/details/gubwlqlmv.sHtML

Go:   err.Error()
来源：http://mobile.vehdjk.com/Article/details/ghwndavlb.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.tarul.cn/Article/details/gsfojzjeq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.epnwcf.com/Article/details/gwbqwmvky.sHtML

[H09] 带错误码的异常
来源：http://read.share.yfazqb.com/Article/details/gozgnpgkl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.vehdjk.com/Article/details/gqfrikzoz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.vehdjk.com/Article/details/glwuvliqv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.tarul.cn/Article/details/gvcurhskw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.sjlbkw.cn/Article/details/gzxobplwe.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.vehdjk.com/Article/details/gtqwuevtn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.sjlbkw.cn/Article/details/gyveyegjo.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.yfazqb.com/Article/details/gontwnggs.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.fktsv.cn/Article/details/gfhdcpgbc.sHtML

[H10] 资源自动释放
来源：http://read.share.vehdjk.com/Article/details/gzglmkgws.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fktsv.cn/Article/details/gytycvole.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.yfazqb.com/Article/details/gwaijywpz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.tarul.cn/Article/details/godtswedw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.yfazqb.com/Article/details/gsccpvfnk.sHtML


<!-- 参考信息 -->