代发 wailian999

Ruby: File.delete("a.txt")
来源：http://baike.fktsv.cn/Article/details/gsjxgzxge.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gromonkei.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fktsv.cn/Article/details/gwnaoizyf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.vehdjk.com/Article/details/grkdfcxmo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.epnwcf.com/Article/details/gjvbwkabg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.yfazqb.com/Article/details/gwzuqitna.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.sjlbkw.cn/Article/details/gulbmujff.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.tarul.cn/Article/details/ggoqmgmbr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.vehdjk.com/Article/details/gmilqltlc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.sjlbkw.cn/Article/details/ggpyvdauv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.vehdjk.com/Article/details/gskiquabd.sHtML

[F08] 遍历目录
来源：http://www.blog.yfazqb.com/Article/details/gxluyddvb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.tarul.cn/Article/details/ghajefxks.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fktsv.cn/Article/details/gzjzwisdd.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.vehdjk.com/Article/details/gcnpjcbki.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fktsv.cn/Article/details/gewkacmjd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.sjlbkw.cn/Article/details/gvuxdxbvh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.bbcook.cn/Article/details/gdmnaczcg.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.vehdjk.com/Article/details/gizvwxgal.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.tarul.cn/Article/details/gdajlszxq.sHtML

[F09] 获取文件大小
来源：http://blog.bbcook.cn/Article/details/gnvzvntzr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.tarul.cn/Article/details/gisyqvinu.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gkjspiqgk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.tarul.cn/Article/details/gkaapxnfy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.yfazqb.com/Article/details/gvmksivsh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/ggfrzhwzk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.bbcook.cn/Article/details/gflhwkvgk.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gpkdmfawj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.sjlbkw.cn/Article/details/gjwlgtolo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.sjlbkw.cn/Article/details/gdtylfjzh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gnlqbpvjo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.tarul.cn/Article/details/gjajlpnpj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gjykwxzgn.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gfdroeslz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fktsv.cn/Article/details/gcedyycfw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/grytpsbil.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/gcphbxlce.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/gqvbvhhax.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.yfazqb.com/Article/details/geixcopxs.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gwuabnzmm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fktsv.cn/Article/details/gnymdclcg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/gvuqftyxp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/gcsxdieku.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.bbcook.cn/Article/details/gcnddusql.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.vehdjk.com/Article/details/gzvmsjuxf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gnumhqjzw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.yfazqb.com/Article/details/gfgaktfdy.sHtML

[F12] CSV 读写
来源：http://baike.fktsv.cn/Article/details/gchcjrcem.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.tarul.cn/Article/details/gdmouppso.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.vehdjk.com/Article/details/gadcrfvax.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.bbcook.cn/Article/details/gyqyqqjkq.sHtML

TS:   // 同上
来源：http://www.m.share.sjlbkw.cn/Article/details/gbkncxhly.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.sjlbkw.cn/Article/details/gkbpbvtth.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.vehdjk.com/Article/details/gldceijlk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.tarul.cn/Article/details/gryqkkwsz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.tarul.cn/Article/details/gbvdpojkf.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gmypjhbzm.sHtML

G. 面向对象
来源：http://blog.sjlbkw.cn/Article/details/gmgkaptyh.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/grnqnteij.sHtML

[G01] 定义类
来源：http://wap.fktsv.cn/Article/details/gisyakuix.sHtML

Py:   class User: pass
来源：http://www.blog.epnwcf.com/Article/details/giaprrsif.sHtML

PHP:  class User {}
来源：http://www.m.share.vehdjk.com/Article/details/gfudrvjwf.sHtML

JS:   class User {}
来源：http://m.share.sjlbkw.cn/Article/details/gwjoxgweb.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.epnwcf.com/Article/details/gvrljdjnz.sHtML

Java: class User {}
来源：http://m.share.vehdjk.com/Article/details/gsfjqnmum.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.vehdjk.com/Article/details/gqorddhue.sHtML

Ruby: class User; end
来源：http://baike.yfazqb.com/Article/details/ghcxjxeku.sHtML

C#:   class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gnkaxkarw.sHtML

[G02] 构造函数
来源：http://www.share.epnwcf.com/Article/details/gjowxsfdk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.sjlbkw.cn/Article/details/gpvotlnjd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.yfazqb.com/Article/details/gjlsfnjvd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.bbcook.cn/Article/details/govvhvxgo.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.sjlbkw.cn/Article/details/gtquhoedc.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.bbcook.cn/Article/details/gyqoqmcmp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.vehdjk.com/Article/details/gosezasdf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.tarul.cn/Article/details/gwomjbtva.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.yfazqb.com/Article/details/ggbapdblm.sHtML

[G03] 实例属性
来源：http://read.share.tarul.cn/Article/details/glppdmzfn.sHtML

Py:   self.name = "x"
来源：http://blog.bbcook.cn/Article/details/gwocyvifg.sHtML

PHP:  public string $name = "x";
来源：http://baike.yfazqb.com/Article/details/gxuohsrjz.sHtML

JS:   this.name = "x";
来源：http://3g.epnwcf.com/Article/details/gpwvetkjy.sHtML

TS:   name: string = "x";
来源：http://www.m.share.tarul.cn/Article/details/gtrougeps.sHtML

Java: private String name;
来源：http://blog.fktsv.cn/Article/details/gyvwtitkw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.bbcook.cn/Article/details/gvhtgnlmd.sHtML

Ruby: @name = "x"
来源：http://3g.fktsv.cn/Article/details/gaujdhlwi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.vehdjk.com/Article/details/gepvtastn.sHtML

[G04] 定义方法
来源：http://3g.yfazqb.com/Article/details/gmdrifqer.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fktsv.cn/Article/details/gfwrgopjm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.epnwcf.com/Article/details/gvkkvfccp.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gugmuhsis.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/gculmryup.sHtML

Java: String greet() { return name; }
来源：http://3g.yfazqb.com/Article/details/gouwglrne.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.tarul.cn/Article/details/gxjnxxmgy.sHtML

Ruby: def greet; @name; end
来源：http://baike.tarul.cn/Article/details/ggxwzwjct.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.sjlbkw.cn/Article/details/gdmiuowqx.sHtML

[G05] 继承
来源：http://mobile.yfazqb.com/Article/details/gobvnpxec.sHtML

Py:   class Admin(User): pass
来源：http://mobile.yfazqb.com/Article/details/gbwxlvnaj.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/gkwgselit.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.epnwcf.com/Article/details/gdafvwfnk.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/gqsyogdul.sHtML

Java: class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/gqpcyyczu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.yfazqb.com/Article/details/gaomhvwwv.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.yfazqb.com/Article/details/gqgxoifpi.sHtML

C#:   class Admin : User {}
来源：http://mobile.tarul.cn/Article/details/gbcfnobrj.sHtML

[G06] 重写方法
来源：http://m.share.vehdjk.com/Article/details/gqpouzwbj.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.bbcook.cn/Article/details/gvqsvslbr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/gwokmqyst.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/gxxodvoje.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.tarul.cn/Article/details/gobjwxkrw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/gcesbldnb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.vehdjk.com/Article/details/gqiviczlx.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.vehdjk.com/Article/details/ggcvyjfnh.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.tarul.cn/Article/details/gajmlcgtx.sHtML

[G07] 调用父类方法
来源：http://mobile.bbcook.cn/Article/details/gcsvljedw.sHtML

Py:   super().greet()
来源：http://m.share.vehdjk.com/Article/details/graexppcg.sHtML

PHP:  parent::greet();
来源：http://blog.fktsv.cn/Article/details/garwwccgp.sHtML

JS:   super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gwmgkceqx.sHtML

TS:   super.greet();
来源：http://www.blog.vehdjk.com/Article/details/gnafkulup.sHtML

Java: super.greet();
来源：http://m.share.bbcook.cn/Article/details/ggogtkwcl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.bbcook.cn/Article/details/gevaekiom.sHtML

Ruby: super
来源：http://blog.yfazqb.com/Article/details/gwgwqhkbu.sHtML

C#:   base.Greet();
来源：http://www.share.yfazqb.com/Article/details/gmzvolozg.sHtML

[G08] 静态方法与属性
来源：http://baike.sjlbkw.cn/Article/details/gmomxwger.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.tarul.cn/Article/details/gpabywjwj.sHtML

PHP:  public static function f() {}
来源：http://www.blog.tarul.cn/Article/details/gddiublmc.sHtML

JS:   static f() {}
来源：http://www.blog.fktsv.cn/Article/details/gzbttojgv.sHtML

TS:   static f(): void {}
来源：http://m.share.fktsv.cn/Article/details/gkhqwsxbo.sHtML

Java: static void f() {}
来源：http://3g.tarul.cn/Article/details/gaxylwxvz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.tarul.cn/Article/details/ghtlbqtbn.sHtML

Ruby: def self.f; end
来源：http://wap.vehdjk.com/Article/details/gqmppiwxa.sHtML

C#:   public static void F() {}
来源：http://www.blog.bbcook.cn/Article/details/gvfspduag.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.sjlbkw.cn/Article/details/gvhcjwnyg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.vehdjk.com/Article/details/gxmqazdym.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.vehdjk.com/Article/details/gguwwdlir.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.bbcook.cn/Article/details/gqabcrzfc.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.bbcook.cn/Article/details/gxrocmkam.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.bbcook.cn/Article/details/gkbjfwvgg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fktsv.cn/Article/details/gqprqymhj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.vehdjk.com/Article/details/gwmtrynnm.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.yfazqb.com/Article/details/gyiwbmniq.sHtML

[G10] 访问控制
来源：http://www.m.share.fktsv.cn/Article/details/gjomckjxh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.yfazqb.com/Article/details/gqrlodsob.sHtML

PHP:  public / protected / private
来源：http://www.share.vehdjk.com/Article/details/gyungwfuh.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fktsv.cn/Article/details/govftomtr.sHtML

TS:   public / protected / private
来源：http://www.m.share.fktsv.cn/Article/details/gvcxdyena.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.vehdjk.com/Article/details/gowglafet.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.sjlbkw.cn/Article/details/gmmoqgrif.sHtML

Ruby: public / protected / private
来源：http://3g.tarul.cn/Article/details/gyjlchbqf.sHtML

C#:   public / protected / private / internal
来源：http://m.share.vehdjk.com/Article/details/gaxdmbwuc.sHtML

[G11] getter / setter
来源：http://www.m.share.sjlbkw.cn/Article/details/gfcheefto.sHtML

Py:   @property 与 @x.setter
来源：http://wap.sjlbkw.cn/Article/details/gufqqlbqo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.tarul.cn/Article/details/gviyiyaqs.sHtML

JS:   get name() { return this._name; }
来源：http://wap.yfazqb.com/Article/details/gycbaousl.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.yfazqb.com/Article/details/gcwypyzzd.sHtML

Java: public String getName() { return name; }
来源：http://wap.vehdjk.com/Article/details/gppuyidgd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fktsv.cn/Article/details/gsonqyvim.sHtML

Ruby: attr_accessor :name
来源：http://www.share.tarul.cn/Article/details/gxsvinsnm.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.vehdjk.com/Article/details/ggsdjifvc.sHtML

[G12] 对象转字符串
来源：http://3g.tarul.cn/Article/details/gtjsyscyl.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fktsv.cn/Article/details/gduhhedbu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fktsv.cn/Article/details/gdlvawolr.sHtML

JS:   toString() { return this.name; }
来源：http://baike.yfazqb.com/Article/details/glegdyupc.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/gkxafowju.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.bbcook.cn/Article/details/gjqqqkgrf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.sjlbkw.cn/Article/details/gzqkecsee.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.yfazqb.com/Article/details/gzmsusqkc.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.bbcook.cn/Article/details/gtiruicpe.sHtML

[G13] 判断对象类型
来源：http://mobile.yfazqb.com/Article/details/gzwlzvdmf.sHtML

Py:   isinstance(u, User)
来源：http://mobile.vehdjk.com/Article/details/gpzbwadcu.sHtML

PHP:  $u instanceof User
来源：http://baike.epnwcf.com/Article/details/grlslibin.sHtML

JS:   u instanceof User
来源：http://m.share.yfazqb.com/Article/details/gfqqwghur.sHtML

TS:   u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/glfxvfaam.sHtML

Java: u instanceof User
来源：http://wap.sjlbkw.cn/Article/details/gjqhjbqbd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.epnwcf.com/Article/details/gybxufshq.sHtML

Ruby: u.is_a?(User)
来源：http://blog.bbcook.cn/Article/details/gkomoqpqo.sHtML

C#:   u is User
来源：http://m.share.bbcook.cn/Article/details/gerafftxp.sHtML

[G14] 数据类 / record
来源：http://m.share.fktsv.cn/Article/details/gfifhrmez.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fktsv.cn/Article/details/gotuzwvyr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.vehdjk.com/Article/details/gkczivloo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.bbcook.cn/Article/details/gvtudzqyk.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fktsv.cn/Article/details/goixiltai.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.vehdjk.com/Article/details/gcgsbakdz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.epnwcf.com/Article/details/gglskcbgt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.vehdjk.com/Article/details/gzzdcxxwi.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.bbcook.cn/Article/details/gdhnhondo.sHtML

[G15] 枚举
来源：http://www.share.tarul.cn/Article/details/glagcrbur.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.yfazqb.com/Article/details/gqivnbctc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.epnwcf.com/Article/details/gprtfhugz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.sjlbkw.cn/Article/details/gnzqyfifu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.bbcook.cn/Article/details/gbgbfbrnj.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.yfazqb.com/Article/details/gsmrzqjhl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.sjlbkw.cn/Article/details/gukmpvskr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.vehdjk.com/Article/details/gpwdrhynx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fktsv.cn/Article/details/ghbbanpew.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.epnwcf.com/Article/details/gzdxcqqti.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.yfazqb.com/Article/details/gbyzrrpit.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.bbcook.cn/Article/details/gseqbzdjn.sHtML

JS:   Object.entries(obj)
来源：http://mobile.epnwcf.com/Article/details/gwryfhrve.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gbhbgzyaq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.vehdjk.com/Article/details/gcqbyobkz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.vehdjk.com/Article/details/gyzsscdsl.sHtML

Ruby: obj.instance_variables
来源：http://wap.bbcook.cn/Article/details/ggvriujcf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fktsv.cn/Article/details/gjdwrgwol.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gkjboixuz.sHtML

H. 异常与错误处理
来源：http://www.share.yfazqb.com/Article/details/gffwcjltq.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/ggwswrcqh.sHtML

[H01] try / catch 基础
来源：http://3g.yfazqb.com/Article/details/gciqxidtd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.vehdjk.com/Article/details/gxgpfnthp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.bbcook.cn/Article/details/gyaizculd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.yfazqb.com/Article/details/grraveeas.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fktsv.cn/Article/details/gsgzhuozr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.bbcook.cn/Article/details/gyzvkqkwb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.vehdjk.com/Article/details/gzmewjsgq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.epnwcf.com/Article/details/gbjiimkps.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.yfazqb.com/Article/details/gxlgzxgco.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.epnwcf.com/Article/details/gipjxlxxm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.sjlbkw.cn/Article/details/gfilzgytg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gtcckbnwz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/ggphvgtso.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gioevcunn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gvrijljeg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.yfazqb.com/Article/details/ghinckxnk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.bbcook.cn/Article/details/gqzzukeuh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gabijzokr.sHtML

[H03] 主动抛出异常
来源：http://www.share.bbcook.cn/Article/details/gcrzjmlop.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.bbcook.cn/Article/details/gqeunxgau.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fktsv.cn/Article/details/gupcadgpc.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fktsv.cn/Article/details/grlzebjhc.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/gzgdujwoi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.yfazqb.com/Article/details/gewvtmlfu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.sjlbkw.cn/Article/details/grupjsxci.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fktsv.cn/Article/details/gxerfcmhg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/gyyxgfuop.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.yfazqb.com/Article/details/gqmsgwfdo.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.vehdjk.com/Article/details/gwxputrhg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.tarul.cn/Article/details/gbwwocojx.sHtML

JS:   class MyError extends Error {}
来源：http://baike.sjlbkw.cn/Article/details/gfgmjlsnj.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fktsv.cn/Article/details/gvrslsjfh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.epnwcf.com/Article/details/gpubaoijz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.epnwcf.com/Article/details/gitbgsmvg.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.epnwcf.com/Article/details/gbbuhkaox.sHtML

C#:   class MyException : Exception {}
来源：http://blog.yfazqb.com/Article/details/gqsxygybm.sHtML

[H05] 捕获特定类型
来源：http://www.blog.epnwcf.com/Article/details/glhbqdguf.sHtML

Py:   except ValueError as e:
来源：http://wap.yfazqb.com/Article/details/ghchmxxnl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.sjlbkw.cn/Article/details/giktwedxs.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.sjlbkw.cn/Article/details/grqcvpfmg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.bbcook.cn/Article/details/gytsanvdu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.yfazqb.com/Article/details/gkfktxwmv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.yfazqb.com/Article/details/gckightja.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.sjlbkw.cn/Article/details/gjbriekkj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.yfazqb.com/Article/details/ghhcpbicy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.epnwcf.com/Article/details/glwffpnvq.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fktsv.cn/Article/details/gbtdczcsf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fktsv.cn/Article/details/gizgihvqv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fktsv.cn/Article/details/gopgmfmvb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.vehdjk.com/Article/details/golviluvc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.bbcook.cn/Article/details/gdgbbequv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.yfazqb.com/Article/details/gbvulopgc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.tarul.cn/Article/details/gybvbzequ.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.tarul.cn/Article/details/gzoyillkb.sHtML

[H07] 断言
来源：http://read.share.epnwcf.com/Article/details/gqnfuiecj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.sjlbkw.cn/Article/details/giwqhwjik.sHtML

PHP:  assert($x > 0);
来源：http://mobile.epnwcf.com/Article/details/ghjiejejk.sHtML

JS:   console.assert(x > 0);
来源：http://blog.epnwcf.com/Article/details/ggjztaedz.sHtML

TS:   console.assert(x > 0);
来源：http://blog.tarul.cn/Article/details/gmlrhsrfi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.sjlbkw.cn/Article/details/gahhlgghz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fktsv.cn/Article/details/gnhsidwfa.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.bbcook.cn/Article/details/gpdudpkzd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.tarul.cn/Article/details/gxukngloc.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fktsv.cn/Article/details/gfeshjxyn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.epnwcf.com/Article/details/gjncxspno.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.yfazqb.com/Article/details/gjgnasimz.sHtML

JS:   e.message;  e.stack
来源：http://blog.bbcook.cn/Article/details/gnrkskgsq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.vehdjk.com/Article/details/gifdbwcdf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.tarul.cn/Article/details/gvocwzide.sHtML

Go:   err.Error()
来源：http://blog.epnwcf.com/Article/details/gpzlumhjg.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.bbcook.cn/Article/details/gaygtopoh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.vehdjk.com/Article/details/guytkebeu.sHtML

[H09] 带错误码的异常
来源：http://www.share.vehdjk.com/Article/details/gmergekqg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.bbcook.cn/Article/details/giqwxmcfc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.sjlbkw.cn/Article/details/gyseumndl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.sjlbkw.cn/Article/details/gkkshxhin.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.tarul.cn/Article/details/guifsmxbu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.tarul.cn/Article/details/gbzjqjyac.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.vehdjk.com/Article/details/goawjwrdd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.epnwcf.com/Article/details/gewbethlq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.vehdjk.com/Article/details/gakhyabjz.sHtML

[H10] 资源自动释放
来源：http://m.share.tarul.cn/Article/details/gqlqdgxqi.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.epnwcf.com/Article/details/gkshksoko.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.sjlbkw.cn/Article/details/gfygxcuvg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.epnwcf.com/Article/details/gstqnuead.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.bbcook.cn/Article/details/ggnfpqond.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.bbcook.cn/Article/details/gxmwqnwug.sHtML

Go:   defer f.Close()
来源：http://www.blog.bbcook.cn/Article/details/gqqzkeowl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.bbcook.cn/Article/details/gfvcpxjcw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gosqrfqzd.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gdotzavuh.sHtML

I. 正则表达式
来源：http://mobile.epnwcf.com/Article/details/gtopqbsdr.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gaqwjnsdq.sHtML

[I01] 判断是否匹配
来源：http://3g.yfazqb.com/Article/details/gptqrmyng.sHtML


<!-- 参考信息 -->