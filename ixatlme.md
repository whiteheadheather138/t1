代发 wailian999

C#:   File.Exists("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnhbzkzto.sHtML

[F06] 删除文件
来源：http://3g.yfazqb.com/Article/details/gqygswszp.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gxucwwjsd.sHtML

PHP:  unlink("a.txt");
来源：http://3g.bbcook.cn/Article/details/gumrvakuk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/giyrdetwx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.tarul.cn/Article/details/gtbfqjvbl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gzxjzzeek.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gebjpkdra.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gfeqickdr.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.bbcook.cn/Article/details/gejcldjjm.sHtML

[F07] 创建目录（含多级）
来源：http://3g.vehdjk.com/Article/details/gvnfjsbos.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fktsv.cn/Article/details/grbpxlmca.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fktsv.cn/Article/details/ghafuuvzy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.bbcook.cn/Article/details/gcbceaafo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.bbcook.cn/Article/details/ghsofqzck.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.tarul.cn/Article/details/gfbhzqdec.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.yfazqb.com/Article/details/gonhumtoz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.sjlbkw.cn/Article/details/glhpczife.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.tarul.cn/Article/details/gabbftsld.sHtML

[F08] 遍历目录
来源：http://baike.bbcook.cn/Article/details/gjhiokfpi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.sjlbkw.cn/Article/details/gvvcwutep.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.sjlbkw.cn/Article/details/ghvzxdnyu.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.yfazqb.com/Article/details/gmdlbrqtj.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.bbcook.cn/Article/details/gxkzjvuin.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.sjlbkw.cn/Article/details/gafxhcnxh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.bbcook.cn/Article/details/gyazznioe.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.bbcook.cn/Article/details/gatwqmobj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.epnwcf.com/Article/details/grinjnonv.sHtML

[F09] 获取文件大小
来源：http://3g.vehdjk.com/Article/details/gerwhfggg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzisksfls.sHtML

PHP:  filesize("a.txt");
来源：http://wap.bbcook.cn/Article/details/gdyefinaj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.epnwcf.com/Article/details/gfllonnro.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.bbcook.cn/Article/details/goacugfbs.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/gewjlpnck.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.sjlbkw.cn/Article/details/gjwdygbry.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gjuqfuswz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.tarul.cn/Article/details/gkwmblogj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.epnwcf.com/Article/details/giawgsjzt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/gsqmqzmeb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.vehdjk.com/Article/details/gfievcphe.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gtkfmuuds.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gopkekyvi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.yfazqb.com/Article/details/gsqqbbwmg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/gvrzpgpwm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gcxbwdcot.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqupypyjl.sHtML

[F11] 复制与移动文件
来源：http://m.share.yfazqb.com/Article/details/gzhhynmqx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.vehdjk.com/Article/details/gkhpweunt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.sjlbkw.cn/Article/details/gxvxmzasz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/gkytkfjbk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/gxwtiqmcz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.bbcook.cn/Article/details/gvgpmzrqo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.bbcook.cn/Article/details/gilpavruk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/gruobflqi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.bbcook.cn/Article/details/gtxqqffvy.sHtML

[F12] CSV 读写
来源：http://www.m.share.vehdjk.com/Article/details/gazidcgzn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.epnwcf.com/Article/details/glohwrzjc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.tarul.cn/Article/details/ghoefkbkw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fktsv.cn/Article/details/glkfffdis.sHtML

TS:   // 同上
来源：http://wap.vehdjk.com/Article/details/gxnszanmw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.vehdjk.com/Article/details/gvgfjzzds.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.bbcook.cn/Article/details/gcinzaukx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.tarul.cn/Article/details/gyggunumu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.tarul.cn/Article/details/gfhagcrhn.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gznauscvw.sHtML

G. 面向对象
来源：http://blog.bbcook.cn/Article/details/gdpjgggmn.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gqylhfbnf.sHtML

[G01] 定义类
来源：http://m.share.sjlbkw.cn/Article/details/gapdfaxtu.sHtML

Py:   class User: pass
来源：http://wap.vehdjk.com/Article/details/grnqryqyh.sHtML

PHP:  class User {}
来源：http://m.share.fktsv.cn/Article/details/gmrfjzthu.sHtML

JS:   class User {}
来源：http://m.share.yfazqb.com/Article/details/glcrdgpgl.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.epnwcf.com/Article/details/grehpubar.sHtML

Java: class User {}
来源：http://baike.sjlbkw.cn/Article/details/garzfzxtr.sHtML

Go:   type User struct { Name string }
来源：http://m.share.vehdjk.com/Article/details/gukdhzhxc.sHtML

Ruby: class User; end
来源：http://m.share.yfazqb.com/Article/details/geglhhess.sHtML

C#:   class User {}
来源：http://mobile.bbcook.cn/Article/details/gowltefei.sHtML

[G02] 构造函数
来源：http://baike.bbcook.cn/Article/details/gzmkzmthu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.tarul.cn/Article/details/gemtdfodb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fktsv.cn/Article/details/gdlejqsii.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.tarul.cn/Article/details/gmarwldtj.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.tarul.cn/Article/details/ghlwswqun.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.bbcook.cn/Article/details/ggshpmodt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.yfazqb.com/Article/details/gjdwaawpg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.bbcook.cn/Article/details/gmnbyectg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/gdtqrkwli.sHtML

[G03] 实例属性
来源：http://read.share.vehdjk.com/Article/details/glrjdudjj.sHtML

Py:   self.name = "x"
来源：http://mobile.sjlbkw.cn/Article/details/gmwwodkof.sHtML

PHP:  public string $name = "x";
来源：http://www.share.yfazqb.com/Article/details/gzpbjrbyc.sHtML

JS:   this.name = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gdeysnsqd.sHtML

TS:   name: string = "x";
来源：http://blog.vehdjk.com/Article/details/gjxegfqmm.sHtML

Java: private String name;
来源：http://www.m.share.yfazqb.com/Article/details/ghyaclnvk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.tarul.cn/Article/details/gvhyhdcpg.sHtML

Ruby: @name = "x"
来源：http://wap.tarul.cn/Article/details/guypxneah.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fktsv.cn/Article/details/ggbzoenxw.sHtML

[G04] 定义方法
来源：http://baike.sjlbkw.cn/Article/details/gsipqsqez.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.bbcook.cn/Article/details/gojvawueo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.tarul.cn/Article/details/gshbmymtu.sHtML

JS:   greet() { return this.name; }
来源：http://blog.vehdjk.com/Article/details/geyekchfd.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.tarul.cn/Article/details/gapyxywkc.sHtML

Java: String greet() { return name; }
来源：http://baike.tarul.cn/Article/details/gxrsbrcmc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.sjlbkw.cn/Article/details/gknirwcbu.sHtML

Ruby: def greet; @name; end
来源：http://3g.vehdjk.com/Article/details/gmsfoulmi.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fktsv.cn/Article/details/gpucqgzmk.sHtML

[G05] 继承
来源：http://www.m.share.sjlbkw.cn/Article/details/gzymqqxnf.sHtML

Py:   class Admin(User): pass
来源：http://baike.fktsv.cn/Article/details/gwgepywsh.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/gjdlndddr.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fktsv.cn/Article/details/gvvoxoptl.sHtML

TS:   class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/gwndgrfvm.sHtML

Java: class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/gkxzqadjk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fktsv.cn/Article/details/ggmeummts.sHtML

Ruby: class Admin < User; end
来源：http://3g.yfazqb.com/Article/details/ggtflcpwl.sHtML

C#:   class Admin : User {}
来源：http://read.share.sjlbkw.cn/Article/details/gbldriezn.sHtML

[G06] 重写方法
来源：http://mobile.bbcook.cn/Article/details/gwhinyaxq.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.yfazqb.com/Article/details/gparqwoqu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gcuflytar.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.epnwcf.com/Article/details/gxhglwgqn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/gfxtrxoma.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gimvliswl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.epnwcf.com/Article/details/gzywwzzqk.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.tarul.cn/Article/details/gtjhzdedb.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.vehdjk.com/Article/details/gsswgmyjm.sHtML

[G07] 调用父类方法
来源：http://wap.fktsv.cn/Article/details/gpsuknoag.sHtML

Py:   super().greet()
来源：http://mobile.vehdjk.com/Article/details/gbdjnnysx.sHtML

PHP:  parent::greet();
来源：http://wap.yfazqb.com/Article/details/gbmurnexv.sHtML

JS:   super.greet();
来源：http://3g.bbcook.cn/Article/details/gssdqqzik.sHtML

TS:   super.greet();
来源：http://www.share.tarul.cn/Article/details/gsdhcvnfh.sHtML

Java: super.greet();
来源：http://blog.sjlbkw.cn/Article/details/gehsevupl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.epnwcf.com/Article/details/ggizmajfp.sHtML

Ruby: super
来源：http://baike.epnwcf.com/Article/details/gnrdjtpyr.sHtML

C#:   base.Greet();
来源：http://baike.sjlbkw.cn/Article/details/gmelzccan.sHtML

[G08] 静态方法与属性
来源：http://read.share.vehdjk.com/Article/details/gesdtnzvq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.epnwcf.com/Article/details/gotbfesny.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.tarul.cn/Article/details/grkaolkwh.sHtML

JS:   static f() {}
来源：http://baike.yfazqb.com/Article/details/gheqswiap.sHtML

TS:   static f(): void {}
来源：http://read.share.sjlbkw.cn/Article/details/gvfmgpxar.sHtML

Java: static void f() {}
来源：http://baike.vehdjk.com/Article/details/gwijztgmv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fktsv.cn/Article/details/goyodtcsf.sHtML

Ruby: def self.f; end
来源：http://3g.sjlbkw.cn/Article/details/gyharywdo.sHtML

C#:   public static void F() {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gcyhrqyyv.sHtML

[G09] 接口 / 抽象类
来源：http://3g.bbcook.cn/Article/details/ghoeubqmj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fktsv.cn/Article/details/gwhhommuq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.epnwcf.com/Article/details/gnysqnduj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.vehdjk.com/Article/details/gmwvsbpcu.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.bbcook.cn/Article/details/gzgzssloy.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.vehdjk.com/Article/details/gkzaigmxi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.epnwcf.com/Article/details/guvgwtwyi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.bbcook.cn/Article/details/gzxhhfxip.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.bbcook.cn/Article/details/gqdwnxnyj.sHtML

[G10] 访问控制
来源：http://wap.tarul.cn/Article/details/ggniduqjb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.bbcook.cn/Article/details/gdimxuufb.sHtML

PHP:  public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/gfmjqfcee.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.yfazqb.com/Article/details/gdoqmnbcp.sHtML

TS:   public / protected / private
来源：http://baike.vehdjk.com/Article/details/gpniblnyw.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.yfazqb.com/Article/details/gfhjwbdmr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.sjlbkw.cn/Article/details/gsglcrxnc.sHtML

Ruby: public / protected / private
来源：http://mobile.tarul.cn/Article/details/gcuvcztyq.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fktsv.cn/Article/details/gvvvmnxlk.sHtML

[G11] getter / setter
来源：http://blog.yfazqb.com/Article/details/gstiiwhmp.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.epnwcf.com/Article/details/garepkdwj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.tarul.cn/Article/details/gpicjxwrn.sHtML

JS:   get name() { return this._name; }
来源：http://wap.epnwcf.com/Article/details/gatfccqvx.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.vehdjk.com/Article/details/gntdnngyu.sHtML

Java: public String getName() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gmkfbnmtn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.yfazqb.com/Article/details/gpjdvnrnm.sHtML

Ruby: attr_accessor :name
来源：http://www.share.vehdjk.com/Article/details/gjremwwes.sHtML

C#:   public string Name { get; set; }
来源：http://blog.epnwcf.com/Article/details/gqacrntrk.sHtML

[G12] 对象转字符串
来源：http://www.m.share.tarul.cn/Article/details/gqxbvxfuw.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwtwzrpv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.sjlbkw.cn/Article/details/gpepyxluw.sHtML

JS:   toString() { return this.name; }
来源：http://baike.bbcook.cn/Article/details/gxjqizauy.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.tarul.cn/Article/details/gevwgzinf.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.tarul.cn/Article/details/gtdeeutov.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.sjlbkw.cn/Article/details/gmnnaeuze.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fktsv.cn/Article/details/gvphafpca.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.bbcook.cn/Article/details/gxknhddgs.sHtML

[G13] 判断对象类型
来源：http://blog.fktsv.cn/Article/details/gxpwrtfko.sHtML

Py:   isinstance(u, User)
来源：http://read.share.sjlbkw.cn/Article/details/gzjooewpg.sHtML

PHP:  $u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/gyblyoxds.sHtML

JS:   u instanceof User
来源：http://baike.bbcook.cn/Article/details/gkiscbqnm.sHtML

TS:   u instanceof User
来源：http://3g.sjlbkw.cn/Article/details/gyaldclfg.sHtML

Java: u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/gqlhxbblk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.vehdjk.com/Article/details/gimidftke.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.yfazqb.com/Article/details/gvwrquwep.sHtML

C#:   u is User
来源：http://www.share.tarul.cn/Article/details/gdfzoedbp.sHtML

[G14] 数据类 / record
来源：http://wap.fktsv.cn/Article/details/gskxvhlpx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.bbcook.cn/Article/details/gcbsebjea.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.epnwcf.com/Article/details/gvnvsqtnx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.yfazqb.com/Article/details/gjridnhhs.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.epnwcf.com/Article/details/gdkzgtmet.sHtML

Java: record User(String name, int age) {}
来源：http://blog.sjlbkw.cn/Article/details/gpgpjjlbl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.yfazqb.com/Article/details/gcvrvwfvk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.yfazqb.com/Article/details/gvumurolz.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.sjlbkw.cn/Article/details/guliwuenw.sHtML

[G15] 枚举
来源：http://m.share.yfazqb.com/Article/details/gmgmvjbcy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.vehdjk.com/Article/details/gneaqlhib.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.epnwcf.com/Article/details/gxfpnagmq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.vehdjk.com/Article/details/ggffjofwb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.tarul.cn/Article/details/gzirrnygw.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.epnwcf.com/Article/details/gmpsddtcb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.tarul.cn/Article/details/gvtjjmbss.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.epnwcf.com/Article/details/gimqhjjhr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.vehdjk.com/Article/details/gihxqimpp.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.yfazqb.com/Article/details/gigygxssf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.bbcook.cn/Article/details/grxkjpryx.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.sjlbkw.cn/Article/details/glarrkume.sHtML

JS:   Object.entries(obj)
来源：http://read.share.bbcook.cn/Article/details/gfxoxgaax.sHtML

TS:   Object.entries(obj)
来源：http://3g.yfazqb.com/Article/details/gpyycdwuh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.bbcook.cn/Article/details/ggadxhryd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fktsv.cn/Article/details/gqrurekby.sHtML

Ruby: obj.instance_variables
来源：http://3g.bbcook.cn/Article/details/gkgdiiiaz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.bbcook.cn/Article/details/gaplxuxpb.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/guhsqeurl.sHtML

H. 异常与错误处理
来源：http://www.share.sjlbkw.cn/Article/details/gqrpclajm.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gtjxnylxu.sHtML

[H01] try / catch 基础
来源：http://read.share.tarul.cn/Article/details/gxkikhslz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fktsv.cn/Article/details/glizxloyi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fktsv.cn/Article/details/gnojjpmxh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.yfazqb.com/Article/details/gbchgszuu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.epnwcf.com/Article/details/gpholqans.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.epnwcf.com/Article/details/gnqftbplr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.sjlbkw.cn/Article/details/gmjinfjoq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.vehdjk.com/Article/details/gbdiwzdvs.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.sjlbkw.cn/Article/details/gdvjiwxgd.sHtML

[H02] finally / ensure 收尾
来源：http://baike.epnwcf.com/Article/details/gepfvgihi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.bbcook.cn/Article/details/gvtfjrcdr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gqscxhknj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/glsbgwevq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.vehdjk.com/Article/details/ggwvtzzoc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gkoqjlioj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.epnwcf.com/Article/details/giloalqxo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.tarul.cn/Article/details/gvxyavkfg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gcyhfenek.sHtML

[H03] 主动抛出异常
来源：http://m.share.yfazqb.com/Article/details/gbuorcuwv.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.bbcook.cn/Article/details/gkidfalui.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.epnwcf.com/Article/details/gudlgtigy.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gxepfztfn.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.yfazqb.com/Article/details/gowzfmrtt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/gvksibjxo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.epnwcf.com/Article/details/gjznlyuxd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fktsv.cn/Article/details/gqieprlwi.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.epnwcf.com/Article/details/glzqwwqti.sHtML

[H04] 自定义异常类型
来源：http://wap.yfazqb.com/Article/details/grzwcdaix.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.yfazqb.com/Article/details/gopbjgbgh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fktsv.cn/Article/details/gycamxuxs.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.tarul.cn/Article/details/gnyzbfjoh.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fktsv.cn/Article/details/gcbieombx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.vehdjk.com/Article/details/gsoicfbyy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.epnwcf.com/Article/details/gmnjpaxay.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.tarul.cn/Article/details/gncqhndcy.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.bbcook.cn/Article/details/gbsigmmsz.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fktsv.cn/Article/details/gkyxckwzh.sHtML

Py:   except ValueError as e:
来源：http://mobile.vehdjk.com/Article/details/gvjptkxqn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.vehdjk.com/Article/details/gwwgevjjr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fktsv.cn/Article/details/ghtodbhcd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.yfazqb.com/Article/details/gccstjyjc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.tarul.cn/Article/details/gdwpqfluo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.tarul.cn/Article/details/guiinlyjg.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.vehdjk.com/Article/details/ghnywynez.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.tarul.cn/Article/details/gtmggudly.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.bbcook.cn/Article/details/ggpgooila.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fktsv.cn/Article/details/gokrydbzs.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.tarul.cn/Article/details/gfiunfzoz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.yfazqb.com/Article/details/goiuohhui.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.sjlbkw.cn/Article/details/guufgwyqb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.bbcook.cn/Article/details/giussfhnx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.bbcook.cn/Article/details/gdkhbcibs.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.fktsv.cn/Article/details/gvpsugkuy.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.bbcook.cn/Article/details/gjnyxykml.sHtML

[H07] 断言
来源：http://www.share.yfazqb.com/Article/details/grwioapfk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fktsv.cn/Article/details/ggdpnykyc.sHtML

PHP:  assert($x > 0);
来源：http://mobile.epnwcf.com/Article/details/gcbcztzok.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.yfazqb.com/Article/details/gboqdzwer.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.bbcook.cn/Article/details/gvsmvxexw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.bbcook.cn/Article/details/gqcxiwial.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.epnwcf.com/Article/details/gpxqedunj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.yfazqb.com/Article/details/ggsjqgjnv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/gwyitewmn.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fktsv.cn/Article/details/geydycqhd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.epnwcf.com/Article/details/ggxkhpjiq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.vehdjk.com/Article/details/gowrhpmhl.sHtML

JS:   e.message;  e.stack
来源：http://3g.vehdjk.com/Article/details/gcbpjbssx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.yfazqb.com/Article/details/gmejeqsyz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.yfazqb.com/Article/details/gkfsbkepa.sHtML

Go:   err.Error()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzgkyszqo.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.epnwcf.com/Article/details/gqnhmyxvu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.bbcook.cn/Article/details/galyigcir.sHtML

[H09] 带错误码的异常
来源：http://www.blog.epnwcf.com/Article/details/gtsxcsndj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.bbcook.cn/Article/details/gsrwrygol.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.yfazqb.com/Article/details/ggrlcvjcs.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.vehdjk.com/Article/details/gvvpdqpho.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.epnwcf.com/Article/details/gzsiznibs.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.sjlbkw.cn/Article/details/gfxtbboeu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.tarul.cn/Article/details/ggbdcgkyr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.yfazqb.com/Article/details/gazymhxcr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.sjlbkw.cn/Article/details/gszvbrwox.sHtML

[H10] 资源自动释放
来源：http://wap.bbcook.cn/Article/details/gqtrtqrxy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.yfazqb.com/Article/details/gabyvmtol.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.epnwcf.com/Article/details/gtngdadoh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.vehdjk.com/Article/details/gycxjucgw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.vehdjk.com/Article/details/gchfbywnu.sHtML


<!-- 参考信息 -->