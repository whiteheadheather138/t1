代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kfy.yangfankeji.com

================================================================================
来源：http://brj.redwolf501.top

F. 文件与目录
来源：http://dwh.tianlin.xyz

================================================================================
来源：http://dhv.tian-w.cn

[F01] 读取整个文件
来源：http://uai.chenjidiqi.icu

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xtp.aizwys.cn

PHP:  file_get_contents("a.txt");
来源：http://xvv.hammf.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cwg.9152youxi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://keq.gotoacloud.top

Java: Files.readString(Path.of("a.txt"))
来源：http://mla.gzhubu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xvd.chenlongwang.top

Ruby: File.read("a.txt")
来源：http://yjj.hammf.cn

C#:   File.ReadAllText("a.txt");
来源：http://bpw.ivvv.top

[F02] 逐行读取文件
来源：http://zjc.tanke756.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xwa.meibo888.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rij.jiagoushi.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://prc.shanyushiyangkeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qae.xinyue.icu

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kze.yvedp.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fxn.havefunace.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://brd.zhijiandao.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://myc.gaohongyu789.top

[F03] 写入文件（覆盖）
来源：http://yky.snrcjt.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qhk.tian-w.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fly.dashuyun.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://adi.zhengqikj.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xzy.yj20258.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://aar.kuanghao11.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://oeo.c1oappe.top

Ruby: File.write("a.txt", "hi")
来源：http://air.jiagoushi.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://geg.zdbjq.cn

[F04] 追加写入文件
来源：http://aai.xinyue.icu

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://leq.guannengcc.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ugz.chenlongwang.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tbr.gotoacloud.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fyx.hongshengwenyu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tvr.sjlbkw.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cyv.ehwqpu.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xme.yueranfly.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xqp.ivvv.top

[F05] 判断文件或目录是否存在
来源：http://cxw.yj202588.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fpe.fengsongda.top

PHP:  file_exists("a.txt");
来源：http://yjk.quarkkingdee.top

JS:   fs.existsSync("a.txt")
来源：http://ybk.yuxming.cn

TS:   fs.existsSync("a.txt")
来源：http://hvw.yvedp.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://uwp.zhijiandao.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://eyd.c1oappe.top

Ruby: File.exist?("a.txt")
来源：http://mam.iojbl.cn

C#:   File.Exists("a.txt")
来源：http://foe.jianghu66.top

[F06] 删除文件
来源：http://wdd.tanke756.top

Py:   os.remove("a.txt")
来源：http://ril.andypj.xyz

PHP:  unlink("a.txt");
来源：http://gou.shuidangran.top

JS:   fs.unlinkSync("a.txt")
来源：http://ano.uphjek.com

TS:   fs.unlinkSync("a.txt")
来源：http://xxi.cucudq.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jkv.jianghu66.top

Go:   os.Remove("a.txt")
来源：http://jzo.haohaochexian.top

Ruby: File.delete("a.txt")
来源：http://hjp.bjfxy.top

C#:   File.Delete("a.txt");
来源：http://qyh.shzxlz.cn

[F07] 创建目录（含多级）
来源：http://and.haohaochexian.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hcz.aibaodan.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sqb.ivvv.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sof.c1oappe.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://shd.nwbrower.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zqo.snrcjt.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bzq.shanyushiyangtech.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://njh.jyoumei.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jtv.hywenlv.cn

[F08] 遍历目录
来源：http://gqo.xinyue.icu

Py:   for name in os.listdir("dir"): print(name)
来源：http://rmq.fzhhl.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hma.nwbrower.top

JS:   fs.readdirSync("dir")
来源：http://pqk.ctjpmb.com

TS:   fs.readdirSync("dir")
来源：http://adb.sufxvd.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://buj.jlsjyb.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lty.52xcode.cn

Ruby: Dir.children("dir")
来源：http://tph.yj20258888.top

C#:   Directory.GetFiles("dir")
来源：http://ajw.gotoacloud.top

[F09] 获取文件大小
来源：http://zjb.meibo888.top

Py:   os.path.getsize("a.txt")
来源：http://igo.quarkkingdee.top

PHP:  filesize("a.txt");
来源：http://aix.jqgufenzy.top

JS:   fs.statSync("a.txt").size
来源：http://sri.daxiang520.top

TS:   fs.statSync("a.txt").size
来源：http://iib.yj202588.top

Java: Files.size(Path.of("a.txt"))
来源：http://fnl.zhixingplan.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kyz.sufxvd.cn

Ruby: File.size("a.txt")
来源：http://epr.yuanzhike.top

C#:   new FileInfo("a.txt").Length
来源：http://kxy.yj20258888.top

[F10] 取文件扩展名 / 文件名
来源：http://gfe.hnqzz.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://drr.haohaochexian.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://brz.aizwys.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://guz.mhx1999.top

TS:   path.extname("a.txt")
来源：http://ixi.fehbvm.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lmy.yongpay.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jqt.birdmap.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oof.hammf.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yjh.ehwqpu.com

[F11] 复制与移动文件
来源：http://upk.snrcjt.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ctp.chenjidiqi.icu

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://okf.haohaochexian.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fit.nwbrower.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ixb.vqdsnc.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hkd.feifeiyinyue.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://odh.aizwys.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jwz.zhengqikj.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ybn.pycfn.com

[F12] CSV 读写
来源：http://yol.aibaodan.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qau.iojbl.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gja.dianchejie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://oph.nanxinkj.top

TS:   // 同上
来源：http://aru.yj20258.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://utc.sysykeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tqi.shanyushiyangkeji.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xys.sufxvd.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xqy.zycfv.cn

================================================================================
来源：http://wdw.bbcook.cn

G. 面向对象
来源：http://qlf.jqgfzy.top

================================================================================
来源：http://fjp.smart0.xyz

[G01] 定义类
来源：http://hag.316326.xyz

Py:   class User: pass
来源：http://doc.xylfe.cn

PHP:  class User {}
来源：http://kox.sxryk.cn

JS:   class User {}
来源：http://qok.quarkkingdee.top

TS:   class User { name: string = ""; }
来源：http://mpk.quarkkingdee.top

Java: class User {}
来源：http://dns.jlsjyb.cn

Go:   type User struct { Name string }
来源：http://cmr.zhoulong.xyz

Ruby: class User; end
来源：http://jlo.dashuyun.cn

C#:   class User {}
来源：http://yhx.yonumen.top

[G02] 构造函数
来源：http://iek.epnwcf.com

Py:   def __init__(self, name): self.name = name
来源：http://bin.tanke756.top

PHP:  public function __construct(public string $name) {}
来源：http://qxf.pycfn.com

JS:   constructor(name) { this.name = name; }
来源：http://ebb.jyoumei.cn

TS:   constructor(public name: string) {}
来源：http://hcs.cashguo.top

Java: User(String name) { this.name = name; }
来源：http://wcf.yj20258.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ant.mhx1999.top

Ruby: def initialize(name); @name = name; end
来源：http://tli.yanxiufei.cn

C#:   public User(string name) { Name = name; }
来源：http://ayk.jianghu66.top

[G03] 实例属性
来源：http://hry.zhongyouzk.top

Py:   self.name = "x"
来源：http://hmz.xziqi.cn

PHP:  public string $name = "x";
来源：http://phe.meibo888.top

JS:   this.name = "x";
来源：http://oci.hcnkem.com

TS:   name: string = "x";
来源：http://hhy.chenjidiqi.icu

Java: private String name;
来源：http://ezm.cashguo.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ogf.hongshengwenyu.top

Ruby: @name = "x"
来源：http://cgj.gaohongyu789.top

C#:   public string Name { get; set; } = "x";
来源：http://ntn.cqqwz.cn

[G04] 定义方法
来源：http://kus.aibaodan.cn

Py:   def greet(self): return self.name
来源：http://vji.nanxuanxn.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hog.hywenlv.cn

JS:   greet() { return this.name; }
来源：http://joq.pengpengdd.cyou

TS:   greet(): string { return this.name; }
来源：http://dme.uphjek.com

Java: String greet() { return name; }
来源：http://wag.cheryme.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://shy.aizwys.cn

Ruby: def greet; @name; end
来源：http://iws.guannengcc.top

C#:   public string Greet() => Name;
来源：http://qzo.zdbjq.cn

[G05] 继承
来源：http://tbg.hnqzz.top

Py:   class Admin(User): pass
来源：http://bwu.zhixingplan.top

PHP:  class Admin extends User {}
来源：http://lpk.shanyushiyangkeji.top

JS:   class Admin extends User {}
来源：http://kxw.tanke756.top

TS:   class Admin extends User {}
来源：http://tgn.jiagoushi.top

Java: class Admin extends User {}
来源：http://yrh.zhixingplan.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sif.shangyingyoupin.top

Ruby: class Admin < User; end
来源：http://dqs.epnwcf.com

C#:   class Admin : User {}
来源：http://pgk.zhixingplan.top

[G06] 重写方法
来源：http://uwh.xinyue.icu

Py:   def greet(self): return "admin"
来源：http://fte.zdbjq.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gxi.gogol.net.cn

JS:   greet() { return "admin"; }
来源：http://itl.hywenlv.cn

TS:   greet(): string { return "admin"; }
来源：http://glp.dianchejie.cn

Java: @Override String greet() { return "admin"; }
来源：http://bzt.yuxming.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bmz.smart0.xyz

Ruby: def greet; "admin"; end
来源：http://som.hnqzz.top

C#:   public override string Greet() => "admin";
来源：http://amg.yfazqb.com

[G07] 调用父类方法
来源：http://nvz.hcnkem.com

Py:   super().greet()
来源：http://ozi.aibaodan.cn

PHP:  parent::greet();
来源：http://kma.fengsongda.top

JS:   super.greet();
来源：http://pvt.hcnkem.com

TS:   super.greet();
来源：http://ext.zycfv.cn

Java: super.greet();
来源：http://fgp.shuidangran.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ohu.epnwcf.com

Ruby: super
来源：http://uxf.guannengcc.top

C#:   base.Greet();
来源：http://tlj.ydzc1.top

[G08] 静态方法与属性
来源：http://hzj.zhoulong.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qyi.ivvv.top

PHP:  public static function f() {}
来源：http://ivw.fengsongda.top

JS:   static f() {}
来源：http://fsd.havefunace.top

TS:   static f(): void {}
来源：http://fbg.wangshuangyany.cn

Java: static void f() {}
来源：http://rsf.sysykeji.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://wjn.yj20258.top

Ruby: def self.f; end
来源：http://irb.sysykeji.top

C#:   public static void F() {}
来源：http://vxs.hammf.cn

[G09] 接口 / 抽象类
来源：http://gaq.hongshengwenyu.top

Py:   from abc import ABC, abstractmethod
来源：http://mvy.cheryme.top

PHP:  interface Shape { public function area(): float; }
来源：http://qoy.tanke756.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://kbe.fktsv.cn

TS:   interface Shape { area(): number; }
来源：http://idg.daxiang520.top

Java: interface Shape { double area(); }
来源：http://jzt.meibo888.top

Go:   type Shape interface { Area() float64 }
来源：http://axi.9152youxi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nxa.shangyingyoupin.top

C#:   interface IShape { double Area(); }
来源：http://fjc.dashuyun.cn

[G10] 访问控制
来源：http://whd.316326.xyz

Py:   约定 _protected / __private（不强制）
来源：http://key.snrcjt.cn

PHP:  public / protected / private
来源：http://nen.chenzaomai.com

JS:   #private 字段；其余公开
来源：http://gfc.cucudq.cn

TS:   public / protected / private
来源：http://ude.daria6918.cn

Java: public / protected / private / 默认包级
来源：http://xar.bjfxy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://mky.hnqzz.top

Ruby: public / protected / private
来源：http://vem.havefunace.top

C#:   public / protected / private / internal
来源：http://him.svipenyu.cn

[G11] getter / setter
来源：http://riy.fanxiaobao.xyz

Py:   @property 与 @x.setter
来源：http://izs.ehwqpu.com

PHP:  public function getName(): string { return $this->name; }
来源：http://ozm.wangdashe.top

JS:   get name() { return this._name; }
来源：http://cjn.tanke756.top

TS:   get name(): string { return this._name; }
来源：http://pop.gzhubu.top

Java: public String getName() { return name; }
来源：http://emo.fengsongda.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://lqx.yvedp.cn

Ruby: attr_accessor :name
来源：http://fwp.guowangkeji.top

C#:   public string Name { get; set; }
来源：http://irn.fengsongda.top

[G12] 对象转字符串
来源：http://lel.tianlin.xyz

Py:   def __str__(self): return self.name
来源：http://vlo.snrcjt.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sdp.fengsongda.top

JS:   toString() { return this.name; }
来源：http://hkv.xziqi.cn

TS:   toString(): string { return this.name; }
来源：http://ggx.xylfe.cn

Java: @Override public String toString() { return name; }
来源：http://dpz.jqgfzy.top

Go:   func (u User) String() string { return u.Name }
来源：http://gxc.ctjpmb.com

Ruby: def to_s; @name; end
来源：http://ocb.sweek.top

C#:   public override string ToString() => Name;
来源：http://qne.0kj1m.cn

[G13] 判断对象类型
来源：http://ypr.yuxming.cn

Py:   isinstance(u, User)
来源：http://yyy.ctjpmb.com

PHP:  $u instanceof User
来源：http://rkq.ppjwa.cn

JS:   u instanceof User
来源：http://nof.shzxlz.cn

TS:   u instanceof User
来源：http://lpa.c1oappe.top

Java: u instanceof User
来源：http://ddo.feifeiyinyue.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://cxh.jinqigufen.top

Ruby: u.is_a?(User)
来源：http://hqh.chenzaomai.com

C#:   u is User
来源：http://pbl.cashguo.top

[G14] 数据类 / record
来源：http://jsu.ehwqpu.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gxb.yuxming.cn

PHP:  // 用 readonly 属性模拟
来源：http://syn.birdmap.top

JS:   // 无内置：普通类或对象字面量
来源：http://ygu.kuanghao11.cn

TS:   type User = { name: string; age: number };
来源：http://tdh.ywan-chungtsiang.top

Java: record User(String name, int age) {}
来源：http://rbr.yangfankeji.com

Go:   type User struct { Name string; Age int }
来源：http://kkj.cdnleiting.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mvx.vehdjk.com

C#:   record User(string Name, int Age);
来源：http://roc.yueranfly.top

[G15] 枚举
来源：http://iej.yanxiufei.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kyr.hysaishi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mtv.hnqzz.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lzl.ybcxt.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ykf.jqgfzy.top

Java: enum Color { RED, GREEN }
来源：http://bfn.aibaodan.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nze.quarkkingdee.top

Ruby: Color = %i[red green].freeze
来源：http://vwa.shanyushiyangkeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://smu.ydjk.org.cn

[G16] 对象转数组 / 字典
来源：http://ydn.tian-w.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gue.xinyue.icu

PHP:  get_object_vars($obj);
来源：http://qxi.sufxvd.cn

JS:   Object.entries(obj)
来源：http://pth.sxryk.cn

TS:   Object.entries(obj)
来源：http://ukm.mhx1999.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://znk.vehdjk.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://qmy.jianghu66.top

Ruby: obj.instance_variables
来源：http://eyb.c1oappe.top

C#:   // 用反射或 System.Text.Json
来源：http://arh.gotoacloud.top

================================================================================
来源：http://wlj.fktsv.cn

H. 异常与错误处理
来源：http://dby.9152youxi.cn

================================================================================
来源：http://igr.sweek.top

[H01] try / catch 基础
来源：http://typ.ywan-chungtsiang.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mfk.shangyingyoupin.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nld.jyoumei.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://csu.kuanghao11.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hxl.sjlbkw.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rnh.haohaochexian.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mwt.hfpthk.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ffc.jinqigfzy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gkl.0kj1m.cn

[H02] finally / ensure 收尾
来源：http://vzk.jyoumei.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pvx.shzxlz.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qax.iojbl.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ota.meibo888.top

TS:   try { f(); } finally { cleanup(); }
来源：http://chy.meibo888.top

Java: try { f(); } finally { cleanup(); }
来源：http://cxs.tian-w.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jky.daxiang520.top

Ruby: begin; f; ensure; cleanup; end
来源：http://jdz.tian-w.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dgw.yuanzhike.top

[H03] 主动抛出异常
来源：http://hqz.andypj.xyz

Py:   raise ValueError("错误信息")
来源：http://dok.ywan-chungtsiang.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kja.sweek.top

JS:   throw new Error("错误信息");
来源：http://hjy.birdmap.top

TS:   throw new Error("错误信息");
来源：http://neo.yangfankeji.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://bhp.316326.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mcu.xuetiantiany.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://aay.xziqi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://uvv.zhongyouzk.top

[H04] 自定义异常类型
来源：http://uhl.zhongyouzk.top

Py:   class MyError(Exception): pass
来源：http://cdf.jinqigfzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://zzl.havefunace.top

JS:   class MyError extends Error {}
来源：http://usr.fktsv.cn

TS:   class MyError extends Error {}
来源：http://dey.dashuyun.cn

Java: class MyException extends RuntimeException {}
来源：http://bsa.sysykeji.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jjm.iojbl.cn

Ruby: class MyError < StandardError; end
来源：http://rxm.vehdjk.com

C#:   class MyException : Exception {}
来源：http://ykc.aizwys.cn

[H05] 捕获特定类型
来源：http://yaw.jianghu66.top

Py:   except ValueError as e:
来源：http://nxb.bbcook.cn


<!-- 参考信息 -->