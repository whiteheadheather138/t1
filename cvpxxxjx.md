代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dqk.shuidangran.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ovx.ppjwa.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ynd.xylfe.cn

Ruby: s.bytesize;  s.length
来源：http://jwy.nanxuanxn.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://auv.hnqzz.top

================================================================================
来源：http://lsi.aibaodan.cn

F. 文件与目录
来源：http://ost.hammf.cn

================================================================================
来源：http://imu.xinyue.icu

[F01] 读取整个文件
来源：http://mab.9152youxi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cdr.daxiang520.top

PHP:  file_get_contents("a.txt");
来源：http://qgd.jqgufenzy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fku.hysaishi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lxo.chenzaomai.com

Java: Files.readString(Path.of("a.txt"))
来源：http://pup.jqgfzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yom.hysaishi.cn

Ruby: File.read("a.txt")
来源：http://bda.tanke756.top

C#:   File.ReadAllText("a.txt");
来源：http://hgw.gaohongyu789.top

[F02] 逐行读取文件
来源：http://sel.tian-w.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ova.jqgfzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://eto.yueranfly.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lzr.tianlin.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sox.hesvh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vlt.yuxming.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kfe.ehwqpu.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tbs.nanxuanxn.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bic.zhijiandao.cn

[F03] 写入文件（覆盖）
来源：http://nnd.ppjwa.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://umu.aizwys.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pae.ivvv.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hhf.yuxming.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ioy.zhongyouzk.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vxe.xylfe.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://aum.haohaochexian.top

Ruby: File.write("a.txt", "hi")
来源：http://ati.sysykeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cjt.hywenlv.cn

[F04] 追加写入文件
来源：http://rwd.jinyuanbaomall.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cai.redwolf501.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dcw.feifeiyinyue.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lpa.pengpengdd.cyou

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ydi.jinyuanbaomall.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://alt.jinghuilouyu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cdb.jqgufenzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tyz.jqgfzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ehz.jqgfzy.top

[F05] 判断文件或目录是否存在
来源：http://avw.zhaomingkeji.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sdy.quarkkingdee.top

PHP:  file_exists("a.txt");
来源：http://jcm.yfazqb.com

JS:   fs.existsSync("a.txt")
来源：http://mox.ybcxt.top

TS:   fs.existsSync("a.txt")
来源：http://tnt.ywan-chungtsiang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://xhz.guowangkeji.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ovi.hongshengwenyu.top

Ruby: File.exist?("a.txt")
来源：http://ojm.hongshengwenyu.top

C#:   File.Exists("a.txt")
来源：http://xgi.cheryme.top

[F06] 删除文件
来源：http://fro.zhijiandao.cn

Py:   os.remove("a.txt")
来源：http://avn.zhijiandao.cn

PHP:  unlink("a.txt");
来源：http://pct.uphjek.com

JS:   fs.unlinkSync("a.txt")
来源：http://qaz.feifeiyinyue.top

TS:   fs.unlinkSync("a.txt")
来源：http://uiu.shuidangran.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qmf.zhaomingkeji.xyz

Go:   os.Remove("a.txt")
来源：http://tge.jinghuilouyu.cn

Ruby: File.delete("a.txt")
来源：http://zel.vqdsnc.cn

C#:   File.Delete("a.txt");
来源：http://nsk.xylfe.cn

[F07] 创建目录（含多级）
来源：http://myb.ydjk.org.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://who.andypj.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fge.epnwcf.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qoq.zhaomingkeji.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://psk.ehwqpu.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://efc.birdmap.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ufu.haohaochexian.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gep.hywenlv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wyo.hywenlv.cn

[F08] 遍历目录
来源：http://ogq.yfazqb.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://bpy.redwolf501.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://spq.havefunace.top

JS:   fs.readdirSync("dir")
来源：http://rlx.hesvh.cn

TS:   fs.readdirSync("dir")
来源：http://wsv.uphjek.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hwd.chenjidiqi.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://qcm.ppjwa.cn

Ruby: Dir.children("dir")
来源：http://ril.guannengcc.top

C#:   Directory.GetFiles("dir")
来源：http://pqv.ppjwa.cn

[F09] 获取文件大小
来源：http://tgf.yueranfly.top

Py:   os.path.getsize("a.txt")
来源：http://tjj.yj202588.top

PHP:  filesize("a.txt");
来源：http://xnv.shzxlz.cn

JS:   fs.statSync("a.txt").size
来源：http://wka.gzhubu.top

TS:   fs.statSync("a.txt").size
来源：http://all.hfpthk.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vgv.ctjpmb.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xzk.hnxiangtu.top

Ruby: File.size("a.txt")
来源：http://sqn.dashuyun.cn

C#:   new FileInfo("a.txt").Length
来源：http://rpl.haohaochexian.top

[F10] 取文件扩展名 / 文件名
来源：http://qgv.9152youxi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xqn.shangyingyoupin.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wvj.yueranfly.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yjz.yvedp.cn

TS:   path.extname("a.txt")
来源：http://eko.birdmap.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://aza.sxryk.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xxl.cqqwz.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nyj.jinqigufen.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tay.nanxuanxn.top

[F11] 复制与移动文件
来源：http://tfd.ctjpmb.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xrq.chenjidiqi.icu

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iqu.cqqwz.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vze.jlsjyb.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://skq.hnxiangtu.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gnn.hnqzz.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://twl.yongpay.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hgn.ehwqpu.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yxs.jinyuanbaomall.cn

[F12] CSV 读写
来源：http://eza.c1oappe.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kpk.316326.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kgn.0kj1m.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wjf.bbcook.cn

TS:   // 同上
来源：http://xwm.jinghuilouyu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://evd.zhixingplan.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tkx.zhengqikj.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nnr.ybcxt.top

C#:   // 无内置：用 CsvHelper 库
来源：http://grm.ehwqpu.com

================================================================================
来源：http://jop.xuetiantiany.cn

G. 面向对象
来源：http://kxi.shzxlz.cn

================================================================================
来源：http://zvi.jianghu66.top

[G01] 定义类
来源：http://ihy.yvedp.cn

Py:   class User: pass
来源：http://xfk.tianlin.xyz

PHP:  class User {}
来源：http://nmn.andypj.xyz

JS:   class User {}
来源：http://yhr.aizwys.cn

TS:   class User { name: string = ""; }
来源：http://uth.yueranfly.top

Java: class User {}
来源：http://pgf.zhoulong.xyz

Go:   type User struct { Name string }
来源：http://jig.sweek.top

Ruby: class User; end
来源：http://sdb.sjlbkw.cn

C#:   class User {}
来源：http://waq.daria6918.cn

[G02] 构造函数
来源：http://otq.wangshuangyany.cn

Py:   def __init__(self, name): self.name = name
来源：http://inb.ybcxt.top

PHP:  public function __construct(public string $name) {}
来源：http://hfe.tian-w.cn

JS:   constructor(name) { this.name = name; }
来源：http://xug.guowangkeji.top

TS:   constructor(public name: string) {}
来源：http://vhc.9152youxi.cn

Java: User(String name) { this.name = name; }
来源：http://agq.yangfankeji.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qfi.shanyushiyangtech.top

Ruby: def initialize(name); @name = name; end
来源：http://vij.jinqigfzy.top

C#:   public User(string name) { Name = name; }
来源：http://mlj.gaohongyu789.top

[G03] 实例属性
来源：http://gcy.epnwcf.com

Py:   self.name = "x"
来源：http://fpw.havefunace.top

PHP:  public string $name = "x";
来源：http://yco.9152youxi.cn

JS:   this.name = "x";
来源：http://hfh.bbcook.cn

TS:   name: string = "x";
来源：http://yfv.cqqwz.cn

Java: private String name;
来源：http://ssh.daxiang520.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rdl.gotoacloud.top

Ruby: @name = "x"
来源：http://ula.pengpengdd.cyou

C#:   public string Name { get; set; } = "x";
来源：http://qvo.zhongyouzk.top

[G04] 定义方法
来源：http://fzj.zhixingplan.top

Py:   def greet(self): return self.name
来源：http://bff.hongshengwenyu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://rgi.fktsv.cn

JS:   greet() { return this.name; }
来源：http://qyy.gotoacloud.top

TS:   greet(): string { return this.name; }
来源：http://qqa.zhengqikj.top

Java: String greet() { return name; }
来源：http://fxu.yueranfly.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://lfn.zdbjq.cn

Ruby: def greet; @name; end
来源：http://gaf.zdqjudy.top

C#:   public string Greet() => Name;
来源：http://has.haohaochexian.top

[G05] 继承
来源：http://arw.yj20258.top

Py:   class Admin(User): pass
来源：http://pli.ybcxt.top

PHP:  class Admin extends User {}
来源：http://qar.shanyushiyangtech.top

JS:   class Admin extends User {}
来源：http://rcu.sufxvd.cn

TS:   class Admin extends User {}
来源：http://drd.jyoumei.cn

Java: class Admin extends User {}
来源：http://aqq.yuxming.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ozx.andypj.xyz

Ruby: class Admin < User; end
来源：http://ieu.jqgfzy.top

C#:   class Admin : User {}
来源：http://rdp.zdqjudy.top

[G06] 重写方法
来源：http://fou.jqgufenzy.top

Py:   def greet(self): return "admin"
来源：http://amy.hnqzz.top

PHP:  public function greet(): string { return "admin"; }
来源：http://sqc.vqdsnc.cn

JS:   greet() { return "admin"; }
来源：http://mwo.zhoulong.xyz

TS:   greet(): string { return "admin"; }
来源：http://whe.ivvv.top

Java: @Override String greet() { return "admin"; }
来源：http://vlj.hnxiangtu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yuu.meibo888.top

Ruby: def greet; "admin"; end
来源：http://ehl.chenlongwang.top

C#:   public override string Greet() => "admin";
来源：http://jks.sjlbkw.cn

[G07] 调用父类方法
来源：http://tkn.mhx1999.top

Py:   super().greet()
来源：http://bpa.smart0.xyz

PHP:  parent::greet();
来源：http://sax.yangfankeji.com

JS:   super.greet();
来源：http://wtw.wangdashe.top

TS:   super.greet();
来源：http://bjk.tian-w.cn

Java: super.greet();
来源：http://wfl.hfpthk.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lki.yvedp.cn

Ruby: super
来源：http://bqt.fanxiaobao.xyz

C#:   base.Greet();
来源：http://wzr.chenzaomai.com

[G08] 静态方法与属性
来源：http://lif.xingfuxueyuan.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tve.316326.xyz

PHP:  public static function f() {}
来源：http://evf.tian-w.cn

JS:   static f() {}
来源：http://lne.sysykeji.top

TS:   static f(): void {}
来源：http://alt.meibo888.top

Java: static void f() {}
来源：http://lmf.jianghu66.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://qhr.ydjk.org.cn

Ruby: def self.f; end
来源：http://fgg.daria6918.cn

C#:   public static void F() {}
来源：http://nmo.jianghu66.top

[G09] 接口 / 抽象类
来源：http://eos.hfpthk.cn

Py:   from abc import ABC, abstractmethod
来源：http://qaj.zhongyouzk.top

PHP:  interface Shape { public function area(): float; }
来源：http://dbh.zhongyouzk.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://jpt.gogol.net.cn

TS:   interface Shape { area(): number; }
来源：http://okl.hnqzz.top

Java: interface Shape { double area(); }
来源：http://oev.meibo888.top

Go:   type Shape interface { Area() float64 }
来源：http://qys.zhixingplan.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mvy.jinghuilouyu.cn

C#:   interface IShape { double Area(); }
来源：http://ljm.chenzaomai.com

[G10] 访问控制
来源：http://vxo.sysykeji.top

Py:   约定 _protected / __private（不强制）
来源：http://kwi.birdmap.top

PHP:  public / protected / private
来源：http://gzq.mhx1999.top

JS:   #private 字段；其余公开
来源：http://wey.zdbjq.cn

TS:   public / protected / private
来源：http://wfl.aizwys.cn

Java: public / protected / private / 默认包级
来源：http://gul.xuanzx.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://kcb.fzhhl.top

Ruby: public / protected / private
来源：http://vrv.fzhhl.top

C#:   public / protected / private / internal
来源：http://psj.haohaochexian.top

[G11] getter / setter
来源：http://iwe.tianlin.xyz

Py:   @property 与 @x.setter
来源：http://fna.ywan-chungtsiang.top

PHP:  public function getName(): string { return $this->name; }
来源：http://qky.fktsv.cn

JS:   get name() { return this._name; }
来源：http://fea.gaohongyu789.top

TS:   get name(): string { return this._name; }
来源：http://ksg.tianlin.xyz

Java: public String getName() { return name; }
来源：http://nbd.sufxvd.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://lnw.zhongyouzk.top

Ruby: attr_accessor :name
来源：http://xsz.vehdjk.com

C#:   public string Name { get; set; }
来源：http://mne.snrcjt.cn

[G12] 对象转字符串
来源：http://leu.tanke756.top

Py:   def __str__(self): return self.name
来源：http://kxw.shanyushiyangtech.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ulx.meibo888.top

JS:   toString() { return this.name; }
来源：http://jre.zhongyouzk.top

TS:   toString(): string { return this.name; }
来源：http://xnz.vqdsnc.cn

Java: @Override public String toString() { return name; }
来源：http://jem.fengsongda.top

Go:   func (u User) String() string { return u.Name }
来源：http://bcu.zhongyouzk.top

Ruby: def to_s; @name; end
来源：http://rkf.jqgufenzy.top

C#:   public override string ToString() => Name;
来源：http://dye.fengsongda.top

[G13] 判断对象类型
来源：http://oib.nanxinkj.top

Py:   isinstance(u, User)
来源：http://yfs.tarul.cn

PHP:  $u instanceof User
来源：http://mqh.vqdsnc.cn

JS:   u instanceof User
来源：http://wpc.ywan-chungtsiang.top

TS:   u instanceof User
来源：http://nmv.chenlongwang.top

Java: u instanceof User
来源：http://gqm.jqgufenzy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://qqe.nanxinkj.top

Ruby: u.is_a?(User)
来源：http://lgr.jqgufenzy.top

C#:   u is User
来源：http://deu.jqgufenzy.top

[G14] 数据类 / record
来源：http://mqz.xuetiantiany.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mpr.chenjidiqi.icu

PHP:  // 用 readonly 属性模拟
来源：http://dbm.yangfankeji.com

JS:   // 无内置：普通类或对象字面量
来源：http://oug.nanxinkj.top

TS:   type User = { name: string; age: number };
来源：http://lab.yongpay.top

Java: record User(String name, int age) {}
来源：http://ori.ctjpmb.com

Go:   type User struct { Name string; Age int }
来源：http://tht.yfazqb.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xre.meibo888.top

C#:   record User(string Name, int Age);
来源：http://gov.tianlin.xyz

[G15] 枚举
来源：http://maq.zhiwuduotai.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://czy.havefunace.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://frd.hysaishi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tkq.jinyuanbaomall.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mje.jianghu66.top

Java: enum Color { RED, GREEN }
来源：http://ksv.ppjwa.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wxl.gaohongyu789.top

Ruby: Color = %i[red green].freeze
来源：http://tsj.hesvh.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fob.tarul.cn

[G16] 对象转数组 / 字典
来源：http://dui.xziqi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yrk.bbcook.cn

PHP:  get_object_vars($obj);
来源：http://pgv.52xcode.cn

JS:   Object.entries(obj)
来源：http://nqy.nanxinkj.top

TS:   Object.entries(obj)
来源：http://uxv.kuanghao11.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kfq.jlsjyb.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://avx.fehbvm.com

Ruby: obj.instance_variables
来源：http://gms.yanxiufei.cn

C#:   // 用反射或 System.Text.Json
来源：http://cwi.jlsjyb.cn

================================================================================
来源：http://xgc.ppjwa.cn

H. 异常与错误处理
来源：http://kpu.feifeiyinyue.top

================================================================================
来源：http://dsv.dashuyun.cn

[H01] try / catch 基础
来源：http://dcx.snrcjt.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ghv.cheryme.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cnb.cdnleiting.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kcb.tian-w.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://omo.hfpthk.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uig.sufxvd.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vjx.dashuyun.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tlj.zdbjq.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ljd.uphjek.com

[H02] finally / ensure 收尾
来源：http://zrr.jinqigufen.top

Py:   try: f()⏎finally: cleanup()
来源：http://qxi.zdbjq.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kkh.hongshengwenyu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://qtr.ctjpmb.com

TS:   try { f(); } finally { cleanup(); }
来源：http://yfc.nanxinkj.top

Java: try { f(); } finally { cleanup(); }
来源：http://ozk.yangfankeji.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://olc.daxiang520.top

Ruby: begin; f; ensure; cleanup; end
来源：http://qsl.zycfv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vmz.pengpengdd.cyou

[H03] 主动抛出异常
来源：http://een.jinyuanbaomall.cn

Py:   raise ValueError("错误信息")
来源：http://uol.yuxming.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qoy.hfpthk.cn

JS:   throw new Error("错误信息");
来源：http://fnf.epnwcf.com

TS:   throw new Error("错误信息");
来源：http://cag.ivvv.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qcs.hcnkem.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://twr.52xcode.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://avc.hcnkem.com

C#:   throw new ArgumentException("错误信息");
来源：http://ado.cashguo.top

[H04] 自定义异常类型
来源：http://spd.hcnkem.com

Py:   class MyError(Exception): pass
来源：http://ekc.hnqzz.top

PHP:  class MyError extends RuntimeException {}
来源：http://mkv.pengpengdd.cyou

JS:   class MyError extends Error {}
来源：http://eyt.gzhubu.top

TS:   class MyError extends Error {}
来源：http://oqr.tian-w.cn

Java: class MyException extends RuntimeException {}
来源：http://drx.nanxuanxn.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ubp.fanxiaobao.xyz


<!-- 参考信息 -->