代发 wailian999

[F01] 读取整个文件
来源：http://erf.tanke756.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gds.sjlbkw.cn

PHP:  file_get_contents("a.txt");
来源：http://zns.xylfe.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yns.shanyushiyangkeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cjo.jinqigfzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://wfr.pengpengdd.cyou

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zbk.svipenyu.cn

Ruby: File.read("a.txt")
来源：http://eiq.ehwqpu.com

C#:   File.ReadAllText("a.txt");
来源：http://sin.hnxiangtu.top

[F02] 逐行读取文件
来源：http://vqj.cdnleiting.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hpz.snrcjt.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fsm.fanxiaobao.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vjk.hysaishi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://any.chenlongwang.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ezt.jqgufenzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pyx.hywenlv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://svc.smart0.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://iyq.hywenlv.cn

[F03] 写入文件（覆盖）
来源：http://cgd.yuanzhike.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://khj.hesvh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://orw.aizwys.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vab.zhiwuduotai.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ovr.sjlbkw.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jgr.bjfxy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lta.shanyushiyangtech.top

Ruby: File.write("a.txt", "hi")
来源：http://xvb.yfazqb.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qjt.pengpengdd.cyou

[F04] 追加写入文件
来源：http://wtb.shzxlz.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xkg.ydjk.org.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yjp.jlsjyb.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yuz.sweek.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uxr.cucudq.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zlu.shanyushiyangtech.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hnn.hammf.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yot.jqgufenzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vee.yanxiufei.cn

[F05] 判断文件或目录是否存在
来源：http://spb.zhiwuduotai.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://flo.yongpay.top

PHP:  file_exists("a.txt");
来源：http://qbs.ppjwa.cn

JS:   fs.existsSync("a.txt")
来源：http://fyo.cqqwz.cn

TS:   fs.existsSync("a.txt")
来源：http://fgo.zycfv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://afu.zhiwuduotai.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pgq.ywan-chungtsiang.top

Ruby: File.exist?("a.txt")
来源：http://npl.sjlbkw.cn

C#:   File.Exists("a.txt")
来源：http://vxn.zhijiandao.cn

[F06] 删除文件
来源：http://zkz.yongpay.top

Py:   os.remove("a.txt")
来源：http://wov.mhx1999.top

PHP:  unlink("a.txt");
来源：http://wiy.yonumen.top

JS:   fs.unlinkSync("a.txt")
来源：http://wdq.tianlin.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://kim.tian-w.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vir.yangfankeji.com

Go:   os.Remove("a.txt")
来源：http://kyv.0kj1m.cn

Ruby: File.delete("a.txt")
来源：http://eoy.daria6918.cn

C#:   File.Delete("a.txt");
来源：http://usk.xingfuxueyuan.xyz

[F07] 创建目录（含多级）
来源：http://ioz.wangdashe.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rhd.zhengqikj.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://klo.fanxiaobao.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uoi.jiagoushi.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://itz.dianchejie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pkw.chenlongwang.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qmc.jiagoushi.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nwv.daria6918.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ylb.yanxiufei.cn

[F08] 遍历目录
来源：http://jpl.jinghuilouyu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zqz.fengsongda.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vox.aizwys.cn

JS:   fs.readdirSync("dir")
来源：http://czc.xinyue.icu

TS:   fs.readdirSync("dir")
来源：http://wwt.chenjidiqi.icu

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wnq.hesvh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vic.cdnleiting.top

Ruby: Dir.children("dir")
来源：http://viv.aibaodan.cn

C#:   Directory.GetFiles("dir")
来源：http://nfx.fengsongda.top

[F09] 获取文件大小
来源：http://fnf.shanyushiyangtech.top

Py:   os.path.getsize("a.txt")
来源：http://hkf.c1oappe.top

PHP:  filesize("a.txt");
来源：http://mdb.zhijiandao.cn

JS:   fs.statSync("a.txt").size
来源：http://wcy.havefunace.top

TS:   fs.statSync("a.txt").size
来源：http://hmg.wangdashe.top

Java: Files.size(Path.of("a.txt"))
来源：http://sjb.sjlbkw.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tll.gotoacloud.top

Ruby: File.size("a.txt")
来源：http://lfk.redwolf501.top

C#:   new FileInfo("a.txt").Length
来源：http://cbo.tian-w.cn

[F10] 取文件扩展名 / 文件名
来源：http://vmb.jyoumei.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dbd.yuanzhike.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xao.svipenyu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vgq.chenlongwang.top

TS:   path.extname("a.txt")
来源：http://oqt.zhixingplan.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cpk.haohaochexian.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ngg.yueranfly.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jyg.epnwcf.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hgc.c1oappe.top

[F11] 复制与移动文件
来源：http://uze.birdmap.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ucc.yangfankeji.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tmp.fehbvm.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cis.yanxiufei.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nut.zhongyouzk.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lej.chenzaomai.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jmx.hywenlv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rgq.guannengcc.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zrx.jqgufenzy.top

[F12] CSV 读写
来源：http://dwt.zhijiandao.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hmc.xziqi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://drk.tarul.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rxh.zhengqikj.top

TS:   // 同上
来源：http://anh.zhoulong.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yho.chenzaomai.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ule.ctjpmb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yuk.yueranfly.top

C#:   // 无内置：用 CsvHelper 库
来源：http://zjl.shangyingyoupin.top

================================================================================
来源：http://ekn.vqdsnc.cn

G. 面向对象
来源：http://rju.shangyingyoupin.top

================================================================================
来源：http://xuq.xylfe.cn

[G01] 定义类
来源：http://kjr.smart0.xyz

Py:   class User: pass
来源：http://ygw.quarkkingdee.top

PHP:  class User {}
来源：http://xdp.jinyuanbaomall.cn

JS:   class User {}
来源：http://jrd.jinqigufen.top

TS:   class User { name: string = ""; }
来源：http://njp.0kj1m.cn

Java: class User {}
来源：http://bjn.andypj.xyz

Go:   type User struct { Name string }
来源：http://auk.yuanzhike.top

Ruby: class User; end
来源：http://hys.jqgufenzy.top

C#:   class User {}
来源：http://dma.gotoacloud.top

[G02] 构造函数
来源：http://wzw.yueranfly.top

Py:   def __init__(self, name): self.name = name
来源：http://kft.smart0.xyz

PHP:  public function __construct(public string $name) {}
来源：http://svv.jinqigufen.top

JS:   constructor(name) { this.name = name; }
来源：http://hqb.guannengcc.top

TS:   constructor(public name: string) {}
来源：http://hpz.snrcjt.cn

Java: User(String name) { this.name = name; }
来源：http://ybu.jqgufenzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yur.quarkkingdee.top

Ruby: def initialize(name); @name = name; end
来源：http://ush.jinqigfzy.top

C#:   public User(string name) { Name = name; }
来源：http://axi.0kj1m.cn

[G03] 实例属性
来源：http://rdr.epnwcf.com

Py:   self.name = "x"
来源：http://gds.bjfxy.top

PHP:  public string $name = "x";
来源：http://lbj.yongpay.top

JS:   this.name = "x";
来源：http://chr.zhongyouzk.top

TS:   name: string = "x";
来源：http://euv.iojbl.cn

Java: private String name;
来源：http://shi.andypj.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://upp.feifeiyinyue.top

Ruby: @name = "x"
来源：http://hhp.ivvv.top

C#:   public string Name { get; set; } = "x";
来源：http://wxw.andypj.xyz

[G04] 定义方法
来源：http://sbp.zhengqikj.top

Py:   def greet(self): return self.name
来源：http://fkc.yuxming.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wcj.chenlongwang.top

JS:   greet() { return this.name; }
来源：http://put.fzhhl.top

TS:   greet(): string { return this.name; }
来源：http://cjh.ehwqpu.com

Java: String greet() { return name; }
来源：http://bxj.hywenlv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ode.c1oappe.top

Ruby: def greet; @name; end
来源：http://qww.jinqigfzy.top

C#:   public string Greet() => Name;
来源：http://iko.chenzaomai.com

[G05] 继承
来源：http://ppp.jqgfzy.top

Py:   class Admin(User): pass
来源：http://yvl.tanke756.top

PHP:  class Admin extends User {}
来源：http://gtj.fehbvm.com

JS:   class Admin extends User {}
来源：http://huz.0kj1m.cn

TS:   class Admin extends User {}
来源：http://vyz.jyoumei.cn

Java: class Admin extends User {}
来源：http://heh.shanyushiyangtech.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lqp.xuetiantiany.cn

Ruby: class Admin < User; end
来源：http://ptx.sufxvd.cn

C#:   class Admin : User {}
来源：http://rzt.nanxinkj.top

[G06] 重写方法
来源：http://dxp.nwbrower.top

Py:   def greet(self): return "admin"
来源：http://ncf.sweek.top

PHP:  public function greet(): string { return "admin"; }
来源：http://mqc.shuidangran.top

JS:   greet() { return "admin"; }
来源：http://gki.andypj.xyz

TS:   greet(): string { return "admin"; }
来源：http://sts.jqgufenzy.top

Java: @Override String greet() { return "admin"; }
来源：http://sfe.zhengqikj.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uku.jyoumei.cn

Ruby: def greet; "admin"; end
来源：http://qkg.ehwqpu.com

C#:   public override string Greet() => "admin";
来源：http://ure.yanxiufei.cn

[G07] 调用父类方法
来源：http://cvf.xinyue.icu

Py:   super().greet()
来源：http://wpy.birdmap.top

PHP:  parent::greet();
来源：http://trp.hywenlv.cn

JS:   super.greet();
来源：http://brl.yuanzhike.top

TS:   super.greet();
来源：http://ouf.uphjek.com

Java: super.greet();
来源：http://xmz.tian-w.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ciz.tian-w.cn

Ruby: super
来源：http://dnz.andypj.xyz

C#:   base.Greet();
来源：http://uhn.wangdashe.top

[G08] 静态方法与属性
来源：http://nge.jinqigufen.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kau.xinyue.icu

PHP:  public static function f() {}
来源：http://qnb.hcnkem.com

JS:   static f() {}
来源：http://lre.316326.xyz

TS:   static f(): void {}
来源：http://jnd.chenzaomai.com

Java: static void f() {}
来源：http://wbq.zycfv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qof.yfazqb.com

Ruby: def self.f; end
来源：http://oww.havefunace.top

C#:   public static void F() {}
来源：http://zgj.hnxiangtu.top

[G09] 接口 / 抽象类
来源：http://gmt.sysykeji.top

Py:   from abc import ABC, abstractmethod
来源：http://ibe.pengpengdd.cyou

PHP:  interface Shape { public function area(): float; }
来源：http://wyi.iojbl.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zxy.tarul.cn

TS:   interface Shape { area(): number; }
来源：http://cuq.xuetiantiany.cn

Java: interface Shape { double area(); }
来源：http://mpm.jyoumei.cn

Go:   type Shape interface { Area() float64 }
来源：http://mng.shuidangran.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cpw.wangshuangyany.cn

C#:   interface IShape { double Area(); }
来源：http://foy.snrcjt.cn

[G10] 访问控制
来源：http://gnf.zdqjudy.top

Py:   约定 _protected / __private（不强制）
来源：http://ndh.jinqigufen.top

PHP:  public / protected / private
来源：http://mnp.fehbvm.com

JS:   #private 字段；其余公开
来源：http://jiu.pycfn.com

TS:   public / protected / private
来源：http://qcn.jinqigfzy.top

Java: public / protected / private / 默认包级
来源：http://dfz.sysykeji.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://pja.ppjwa.cn

Ruby: public / protected / private
来源：http://qcg.wangshuangyany.cn

C#:   public / protected / private / internal
来源：http://jiz.zycfv.cn

[G11] getter / setter
来源：http://jdi.hnqzz.top

Py:   @property 与 @x.setter
来源：http://pmu.jyoumei.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ine.ehwqpu.com

JS:   get name() { return this._name; }
来源：http://jyt.snrcjt.cn

TS:   get name(): string { return this._name; }
来源：http://gsv.xinyue.icu

Java: public String getName() { return name; }
来源：http://eeu.xuetiantiany.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rbb.epnwcf.com

Ruby: attr_accessor :name
来源：http://apt.tarul.cn

C#:   public string Name { get; set; }
来源：http://tyr.zhoulong.xyz

[G12] 对象转字符串
来源：http://ewb.zhoulong.xyz

Py:   def __str__(self): return self.name
来源：http://bxk.guannengcc.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://uqf.xinyue.icu

JS:   toString() { return this.name; }
来源：http://hfz.jqgfzy.top

TS:   toString(): string { return this.name; }
来源：http://fmk.guowangkeji.top

Java: @Override public String toString() { return name; }
来源：http://udj.hongshengwenyu.top

Go:   func (u User) String() string { return u.Name }
来源：http://fcm.yj202588.top

Ruby: def to_s; @name; end
来源：http://zkm.chenzaomai.com

C#:   public override string ToString() => Name;
来源：http://rvg.sjlbkw.cn

[G13] 判断对象类型
来源：http://yhu.bbcook.cn

Py:   isinstance(u, User)
来源：http://dfd.jianghu66.top

PHP:  $u instanceof User
来源：http://tiw.yj20258.top

JS:   u instanceof User
来源：http://qxe.snrcjt.cn

TS:   u instanceof User
来源：http://jjx.cashguo.top

Java: u instanceof User
来源：http://nzj.xinyue.icu

Go:   u, ok := v.(User)            // 类型断言
来源：http://lyu.hcnkem.com

Ruby: u.is_a?(User)
来源：http://pik.hnqzz.top

C#:   u is User
来源：http://gci.hysaishi.cn

[G14] 数据类 / record
来源：http://snx.ydzc1.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://olg.xuanzx.com

PHP:  // 用 readonly 属性模拟
来源：http://kes.vehdjk.com

JS:   // 无内置：普通类或对象字面量
来源：http://snq.jqgufenzy.top

TS:   type User = { name: string; age: number };
来源：http://axx.tanke756.top

Java: record User(String name, int age) {}
来源：http://paa.fehbvm.com

Go:   type User struct { Name string; Age int }
来源：http://alv.vqdsnc.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://chb.mhx1999.top

C#:   record User(string Name, int Age);
来源：http://yzt.jianghu66.top

[G15] 枚举
来源：http://bzm.gotoacloud.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wbi.316326.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://tgm.cheryme.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hbv.zhoulong.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ede.shanyushiyangtech.top

Java: enum Color { RED, GREEN }
来源：http://yrx.xylfe.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wxs.hammf.cn

Ruby: Color = %i[red green].freeze
来源：http://xrf.iojbl.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://htv.yvedp.cn

[G16] 对象转数组 / 字典
来源：http://opu.jqgufenzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hmt.shuidangran.top

PHP:  get_object_vars($obj);
来源：http://tzp.52xcode.cn

JS:   Object.entries(obj)
来源：http://mkm.havefunace.top

TS:   Object.entries(obj)
来源：http://kby.jlsjyb.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cxx.ehwqpu.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://kzw.jqgufenzy.top

Ruby: obj.instance_variables
来源：http://aog.yongpay.top

C#:   // 用反射或 System.Text.Json
来源：http://zsk.chenlongwang.top

================================================================================
来源：http://jdo.zhongyouzk.top

H. 异常与错误处理
来源：http://mmh.yonumen.top

================================================================================
来源：http://zvp.yangfankeji.com

[H01] try / catch 基础
来源：http://beq.zhaomingkeji.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cwr.cheryme.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://shg.gaohongyu789.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dxg.guannengcc.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rui.kuanghao11.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uaf.xinyue.icu

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tte.haohaochexian.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dhe.yuanzhike.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zoi.hongshengwenyu.top

[H02] finally / ensure 收尾
来源：http://ryb.cqqwz.cn

Py:   try: f()⏎finally: cleanup()
来源：http://phl.epnwcf.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://ftf.dianchejie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://leo.xziqi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tii.tian-w.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hoy.sxryk.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://iyp.jinghuilouyu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jpk.xingfuxueyuan.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://iey.daxiang520.top

[H03] 主动抛出异常
来源：http://rfb.zhongyouzk.top

Py:   raise ValueError("错误信息")
来源：http://vun.zhoulong.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://luy.gaohongyu789.top

JS:   throw new Error("错误信息");
来源：http://aif.havefunace.top

TS:   throw new Error("错误信息");
来源：http://oio.vehdjk.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://xwy.pengpengdd.cyou

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fjr.smart0.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://jll.yj202588.top

C#:   throw new ArgumentException("错误信息");
来源：http://gxv.yj20258.top

[H04] 自定义异常类型
来源：http://yzr.wangdashe.top

Py:   class MyError(Exception): pass
来源：http://qpd.pengpengdd.cyou

PHP:  class MyError extends RuntimeException {}
来源：http://zgy.shuidangran.top

JS:   class MyError extends Error {}
来源：http://zct.yuanzhike.top

TS:   class MyError extends Error {}
来源：http://isu.tianlin.xyz

Java: class MyException extends RuntimeException {}
来源：http://ssw.jlsjyb.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://spd.316326.xyz

Ruby: class MyError < StandardError; end
来源：http://aqj.jyoumei.cn

C#:   class MyException : Exception {}
来源：http://xll.jinqigfzy.top

[H05] 捕获特定类型
来源：http://hdm.yanxiufei.cn

Py:   except ValueError as e:
来源：http://ebh.jqgufenzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://moq.9152youxi.cn

JS:   if (e instanceof TypeError) {}
来源：http://tun.fehbvm.com

TS:   if (e instanceof TypeError) {}
来源：http://twm.sysykeji.top

Java: catch (IOException | SQLException e) {}
来源：http://kzo.gogol.net.cn


<!-- 参考信息 -->