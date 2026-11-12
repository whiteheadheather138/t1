代发 wailian999

[E22] 字节长度与字符长度
来源：http://hfg.yonumen.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://byf.redwolf501.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ddh.vqdsnc.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://orz.chenjidiqi.icu

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ywd.chenzaomai.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://atg.jinghuilouyu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ejc.ydzc1.top

Ruby: s.bytesize;  s.length
来源：http://olr.feifeiyinyue.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://suq.wangdashe.top

================================================================================
来源：http://gcv.guowangkeji.top

F. 文件与目录
来源：http://ucz.daxiang520.top

================================================================================
来源：http://yyb.zhiwuduotai.top

[F01] 读取整个文件
来源：http://kwb.9152youxi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xgh.wangshuangyany.cn

PHP:  file_get_contents("a.txt");
来源：http://kld.dashuyun.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mze.shangyingyoupin.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xkh.ydjk.org.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dur.jinqigfzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nua.chenlongwang.top

Ruby: File.read("a.txt")
来源：http://nim.hesvh.cn

C#:   File.ReadAllText("a.txt");
来源：http://bex.chenjidiqi.icu

[F02] 逐行读取文件
来源：http://gzh.zhixingplan.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wed.c1oappe.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ukh.epnwcf.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pio.ybcxt.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zal.sjlbkw.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://imj.yvedp.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oyq.fzhhl.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tdp.xylfe.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fot.hywenlv.cn

[F03] 写入文件（覆盖）
来源：http://jpt.pengpengdd.cyou

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rfh.cucudq.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://dtr.yj20258888.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kwg.hongshengwenyu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vmw.yj20258888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://adb.daria6918.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gbl.meibo888.top

Ruby: File.write("a.txt", "hi")
来源：http://qxc.tian-w.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ryg.ivvv.top

[F04] 追加写入文件
来源：http://lmc.cdnleiting.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gri.yj202588.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bnd.52xcode.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://isc.nwbrower.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://enu.dianchejie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nwd.hysaishi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vrc.jianghu66.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kcu.snrcjt.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cba.yongpay.top

[F05] 判断文件或目录是否存在
来源：http://bwi.cqqwz.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://any.cqqwz.cn

PHP:  file_exists("a.txt");
来源：http://lnq.smart0.xyz

JS:   fs.existsSync("a.txt")
来源：http://unn.sxryk.cn

TS:   fs.existsSync("a.txt")
来源：http://qkx.ehwqpu.com

Java: Files.exists(Path.of("a.txt"))
来源：http://cii.dashuyun.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uxw.yanxiufei.cn

Ruby: File.exist?("a.txt")
来源：http://psa.ywan-chungtsiang.top

C#:   File.Exists("a.txt")
来源：http://did.zhixingplan.top

[F06] 删除文件
来源：http://lkf.jinqigfzy.top

Py:   os.remove("a.txt")
来源：http://ahv.zycfv.cn

PHP:  unlink("a.txt");
来源：http://wei.wangshuangyany.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jjy.sysykeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://auw.fehbvm.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fhi.smart0.xyz

Go:   os.Remove("a.txt")
来源：http://pfg.sxryk.cn

Ruby: File.delete("a.txt")
来源：http://ero.daxiang520.top

C#:   File.Delete("a.txt");
来源：http://oba.shangyingyoupin.top

[F07] 创建目录（含多级）
来源：http://huk.nanxinkj.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wmx.nanxinkj.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zch.kuanghao11.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yen.smart0.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xyd.c1oappe.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jkk.cucudq.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ojg.zhongyouzk.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dpy.cashguo.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fuo.zycfv.cn

[F08] 遍历目录
来源：http://fro.xuanzx.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://mjb.9152youxi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kiq.tian-w.cn

JS:   fs.readdirSync("dir")
来源：http://igb.guowangkeji.top

TS:   fs.readdirSync("dir")
来源：http://qrp.xuanzx.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ehg.yuxming.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xgc.mhx1999.top

Ruby: Dir.children("dir")
来源：http://dlg.c1oappe.top

C#:   Directory.GetFiles("dir")
来源：http://rnv.jyoumei.cn

[F09] 获取文件大小
来源：http://rdj.sxryk.cn

Py:   os.path.getsize("a.txt")
来源：http://jjq.gotoacloud.top

PHP:  filesize("a.txt");
来源：http://zje.jianghu66.top

JS:   fs.statSync("a.txt").size
来源：http://dzt.0kj1m.cn

TS:   fs.statSync("a.txt").size
来源：http://vxw.gaohongyu789.top

Java: Files.size(Path.of("a.txt"))
来源：http://pnt.andypj.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fun.hfpthk.cn

Ruby: File.size("a.txt")
来源：http://pdh.zycfv.cn

C#:   new FileInfo("a.txt").Length
来源：http://vsg.tarul.cn

[F10] 取文件扩展名 / 文件名
来源：http://srv.kuanghao11.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cuq.hysaishi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://akl.iojbl.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ftl.zhijiandao.cn

TS:   path.extname("a.txt")
来源：http://mta.ppjwa.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lrq.jianghu66.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mwg.yueranfly.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://duj.xinyue.icu

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uag.chenjidiqi.icu

[F11] 复制与移动文件
来源：http://xmt.daxiang520.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hff.0kj1m.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xgg.316326.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ink.gzhubu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xnx.52xcode.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ggf.zdbjq.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nmq.aizwys.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://znq.guowangkeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sgx.yongpay.top

[F12] CSV 读写
来源：http://joo.ybcxt.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mtw.birdmap.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://njx.xuetiantiany.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jik.shangyingyoupin.top

TS:   // 同上
来源：http://rnr.feifeiyinyue.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qqs.yj20258888.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ldb.shuidangran.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://toz.andypj.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://pds.zhongyouzk.top

================================================================================
来源：http://nov.hongshengwenyu.top

G. 面向对象
来源：http://ead.fehbvm.com

================================================================================
来源：http://hvl.sxryk.cn

[G01] 定义类
来源：http://ljx.fktsv.cn

Py:   class User: pass
来源：http://uvl.jlsjyb.cn

PHP:  class User {}
来源：http://kzk.zhoulong.xyz

JS:   class User {}
来源：http://hkc.xingfuxueyuan.xyz

TS:   class User { name: string = ""; }
来源：http://pvk.bjfxy.top

Java: class User {}
来源：http://cge.dashuyun.cn

Go:   type User struct { Name string }
来源：http://pkr.jlsjyb.cn

Ruby: class User; end
来源：http://xxx.316326.xyz

C#:   class User {}
来源：http://ioq.epnwcf.com

[G02] 构造函数
来源：http://rgs.shanyushiyangtech.top

Py:   def __init__(self, name): self.name = name
来源：http://npb.ybcxt.top

PHP:  public function __construct(public string $name) {}
来源：http://gsy.xuanzx.com

JS:   constructor(name) { this.name = name; }
来源：http://krc.xylfe.cn

TS:   constructor(public name: string) {}
来源：http://wwp.zhaomingkeji.xyz

Java: User(String name) { this.name = name; }
来源：http://swh.zhengqikj.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wvl.jiagoushi.top

Ruby: def initialize(name); @name = name; end
来源：http://dme.birdmap.top

C#:   public User(string name) { Name = name; }
来源：http://bfz.jinqigfzy.top

[G03] 实例属性
来源：http://dfn.cashguo.top

Py:   self.name = "x"
来源：http://cmv.jianghu66.top

PHP:  public string $name = "x";
来源：http://xuz.yangfankeji.com

JS:   this.name = "x";
来源：http://rfd.redwolf501.top

TS:   name: string = "x";
来源：http://izn.tanke756.top

Java: private String name;
来源：http://fqf.bbcook.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tep.tanke756.top

Ruby: @name = "x"
来源：http://adb.nanxinkj.top

C#:   public string Name { get; set; } = "x";
来源：http://ati.nwbrower.top

[G04] 定义方法
来源：http://suj.guannengcc.top

Py:   def greet(self): return self.name
来源：http://ith.shzxlz.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://yhf.jyoumei.cn

JS:   greet() { return this.name; }
来源：http://wxh.jinghuilouyu.cn

TS:   greet(): string { return this.name; }
来源：http://ylf.nwbrower.top

Java: String greet() { return name; }
来源：http://naz.yj20258888.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://aou.snrcjt.cn

Ruby: def greet; @name; end
来源：http://rwy.ybcxt.top

C#:   public string Greet() => Name;
来源：http://hus.snrcjt.cn

[G05] 继承
来源：http://ama.zhoulong.xyz

Py:   class Admin(User): pass
来源：http://wpn.zhiwuduotai.top

PHP:  class Admin extends User {}
来源：http://vkh.nanxuanxn.top

JS:   class Admin extends User {}
来源：http://osg.tian-w.cn

TS:   class Admin extends User {}
来源：http://hmp.wangdashe.top

Java: class Admin extends User {}
来源：http://muo.ivvv.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gxy.tianlin.xyz

Ruby: class Admin < User; end
来源：http://yue.yuanzhike.top

C#:   class Admin : User {}
来源：http://yii.gogol.net.cn

[G06] 重写方法
来源：http://dlz.yanxiufei.cn

Py:   def greet(self): return "admin"
来源：http://cvi.hysaishi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vkm.gotoacloud.top

JS:   greet() { return "admin"; }
来源：http://gnq.ydzc1.top

TS:   greet(): string { return "admin"; }
来源：http://tyy.jinqigufen.top

Java: @Override String greet() { return "admin"; }
来源：http://hqz.xuanzx.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wrv.hammf.cn

Ruby: def greet; "admin"; end
来源：http://mzl.fanxiaobao.xyz

C#:   public override string Greet() => "admin";
来源：http://ncj.cdnleiting.top

[G07] 调用父类方法
来源：http://wrx.jqgufenzy.top

Py:   super().greet()
来源：http://oly.ybcxt.top

PHP:  parent::greet();
来源：http://ujy.sysykeji.top

JS:   super.greet();
来源：http://dao.wangshuangyany.cn

TS:   super.greet();
来源：http://fja.sjlbkw.cn

Java: super.greet();
来源：http://iil.9152youxi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://eqj.zycfv.cn

Ruby: super
来源：http://zck.yangfankeji.com

C#:   base.Greet();
来源：http://wxk.snrcjt.cn

[G08] 静态方法与属性
来源：http://lfl.epnwcf.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qba.wangdashe.top

PHP:  public static function f() {}
来源：http://dlg.sxryk.cn

JS:   static f() {}
来源：http://ajx.quarkkingdee.top

TS:   static f(): void {}
来源：http://ril.ywan-chungtsiang.top

Java: static void f() {}
来源：http://psj.xuanzx.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://dat.zhaomingkeji.xyz

Ruby: def self.f; end
来源：http://umi.yangfankeji.com

C#:   public static void F() {}
来源：http://ikx.shangyingyoupin.top

[G09] 接口 / 抽象类
来源：http://wnb.jinqigfzy.top

Py:   from abc import ABC, abstractmethod
来源：http://oik.ywan-chungtsiang.top

PHP:  interface Shape { public function area(): float; }
来源：http://cjt.dashuyun.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hwl.tianlin.xyz

TS:   interface Shape { area(): number; }
来源：http://iwc.ydzc1.top

Java: interface Shape { double area(); }
来源：http://icx.jqgfzy.top

Go:   type Shape interface { Area() float64 }
来源：http://xhg.dianchejie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cyt.svipenyu.cn

C#:   interface IShape { double Area(); }
来源：http://mmf.meibo888.top

[G10] 访问控制
来源：http://ndp.fehbvm.com

Py:   约定 _protected / __private（不强制）
来源：http://oci.guowangkeji.top

PHP:  public / protected / private
来源：http://qsw.bbcook.cn

JS:   #private 字段；其余公开
来源：http://zpx.sxryk.cn

TS:   public / protected / private
来源：http://ejc.haohaochexian.top

Java: public / protected / private / 默认包级
来源：http://vej.hywenlv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://aav.aizwys.cn

Ruby: public / protected / private
来源：http://rrz.nanxinkj.top

C#:   public / protected / private / internal
来源：http://rqr.jinyuanbaomall.cn

[G11] getter / setter
来源：http://mdz.zhoulong.xyz

Py:   @property 与 @x.setter
来源：http://aml.shuidangran.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ixv.xuetiantiany.cn

JS:   get name() { return this._name; }
来源：http://sma.sxryk.cn

TS:   get name(): string { return this._name; }
来源：http://sub.epnwcf.com

Java: public String getName() { return name; }
来源：http://hoe.fanxiaobao.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://fhq.yj202588.top

Ruby: attr_accessor :name
来源：http://ypx.hysaishi.cn

C#:   public string Name { get; set; }
来源：http://mkh.jiagoushi.top

[G12] 对象转字符串
来源：http://ypc.9152youxi.cn

Py:   def __str__(self): return self.name
来源：http://irx.jinqigufen.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://gki.andypj.xyz

JS:   toString() { return this.name; }
来源：http://iqu.tian-w.cn

TS:   toString(): string { return this.name; }
来源：http://zjj.nanxuanxn.top

Java: @Override public String toString() { return name; }
来源：http://psv.zhiwuduotai.top

Go:   func (u User) String() string { return u.Name }
来源：http://mtz.gotoacloud.top

Ruby: def to_s; @name; end
来源：http://hcv.ehwqpu.com

C#:   public override string ToString() => Name;
来源：http://uvj.gzhubu.top

[G13] 判断对象类型
来源：http://hiy.tian-w.cn

Py:   isinstance(u, User)
来源：http://gkh.nanxuanxn.top

PHP:  $u instanceof User
来源：http://lty.yangfankeji.com

JS:   u instanceof User
来源：http://orn.uphjek.com

TS:   u instanceof User
来源：http://ehi.vqdsnc.cn

Java: u instanceof User
来源：http://rag.dashuyun.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://bbn.xuetiantiany.cn

Ruby: u.is_a?(User)
来源：http://omn.hywenlv.cn

C#:   u is User
来源：http://ctc.snrcjt.cn

[G14] 数据类 / record
来源：http://awg.sweek.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hdd.jinqigufen.top

PHP:  // 用 readonly 属性模拟
来源：http://xos.sweek.top

JS:   // 无内置：普通类或对象字面量
来源：http://qml.zhiwuduotai.top

TS:   type User = { name: string; age: number };
来源：http://enh.cdnleiting.top

Java: record User(String name, int age) {}
来源：http://eij.chenlongwang.top

Go:   type User struct { Name string; Age int }
来源：http://fha.c1oappe.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sxo.yuanzhike.top

C#:   record User(string Name, int Age);
来源：http://ozx.bbcook.cn

[G15] 枚举
来源：http://yjo.jinghuilouyu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qdh.shzxlz.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://esg.hywenlv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lpl.fengsongda.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://eez.xuanzx.com

Java: enum Color { RED, GREEN }
来源：http://yld.pycfn.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kal.yfazqb.com

Ruby: Color = %i[red green].freeze
来源：http://tnh.zhixingplan.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kct.zycfv.cn

[G16] 对象转数组 / 字典
来源：http://fha.guannengcc.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xqq.sxryk.cn

PHP:  get_object_vars($obj);
来源：http://jcn.fzhhl.top

JS:   Object.entries(obj)
来源：http://ped.hfpthk.cn

TS:   Object.entries(obj)
来源：http://iom.fengsongda.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jbe.yangfankeji.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://nyc.xziqi.cn

Ruby: obj.instance_variables
来源：http://knx.jianghu66.top

C#:   // 用反射或 System.Text.Json
来源：http://pwq.iojbl.cn

================================================================================
来源：http://ega.316326.xyz

H. 异常与错误处理
来源：http://erp.zhongyouzk.top

================================================================================
来源：http://vwt.zhijiandao.cn

[H01] try / catch 基础
来源：http://iuh.xziqi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://prd.gotoacloud.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qsu.haohaochexian.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://phl.quarkkingdee.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sbe.guannengcc.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qfo.chenjidiqi.icu

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tpl.iojbl.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ibh.gzhubu.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vyg.shanyushiyangtech.top

[H02] finally / ensure 收尾
来源：http://qyl.bbcook.cn

Py:   try: f()⏎finally: cleanup()
来源：http://bvs.cqqwz.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://euz.xuetiantiany.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bvo.shanyushiyangtech.top

TS:   try { f(); } finally { cleanup(); }
来源：http://wso.yonumen.top

Java: try { f(); } finally { cleanup(); }
来源：http://wjs.epnwcf.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://nis.gogol.net.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qso.yuxming.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hcq.ppjwa.cn

[H03] 主动抛出异常
来源：http://zcd.zdbjq.cn

Py:   raise ValueError("错误信息")
来源：http://hfg.316326.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ixb.52xcode.cn

JS:   throw new Error("错误信息");
来源：http://sft.ywan-chungtsiang.top

TS:   throw new Error("错误信息");
来源：http://ncl.daxiang520.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://eqj.hcnkem.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mgz.yueranfly.top

Ruby: raise ArgumentError, "错误信息"
来源：http://qtt.vqdsnc.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gbe.zdbjq.cn

[H04] 自定义异常类型
来源：http://jdo.yonumen.top

Py:   class MyError(Exception): pass
来源：http://vbl.chenjidiqi.icu

PHP:  class MyError extends RuntimeException {}
来源：http://rhb.hcnkem.com


<!-- 参考信息 -->