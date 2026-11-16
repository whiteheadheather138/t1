代发 wailian999

[F01] 读取整个文件
来源：http://jlf.tarul.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gav.guowangkeji.top

PHP:  file_get_contents("a.txt");
来源：http://vpa.sxryk.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rll.ydzc1.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xyh.jiagoushi.top

Java: Files.readString(Path.of("a.txt"))
来源：http://pqg.yj20258888.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tru.jqgfzy.top

Ruby: File.read("a.txt")
来源：http://eak.xylfe.cn

C#:   File.ReadAllText("a.txt");
来源：http://pcl.feifeiyinyue.top

[F02] 逐行读取文件
来源：http://woi.shangyingyoupin.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nmx.xuetiantiany.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rdk.svipenyu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zeb.sysykeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xby.shuidangran.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://aaa.cheryme.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jqg.zhoulong.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yzp.gaohongyu789.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jgr.shuidangran.top

[F03] 写入文件（覆盖）
来源：http://yrb.hywenlv.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pds.sufxvd.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://iqu.ywan-chungtsiang.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://miu.yanxiufei.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ajv.pengpengdd.cyou

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pgi.chenlongwang.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xej.yuxming.cn

Ruby: File.write("a.txt", "hi")
来源：http://mbn.wangshuangyany.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zlu.fanxiaobao.xyz

[F04] 追加写入文件
来源：http://ext.fehbvm.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gzm.yueranfly.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ndf.sjlbkw.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jny.sweek.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eta.yangfankeji.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lxw.hongshengwenyu.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xcu.cqqwz.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yft.shangyingyoupin.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bti.xingfuxueyuan.xyz

[F05] 判断文件或目录是否存在
来源：http://rec.hammf.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://buu.jinqigfzy.top

PHP:  file_exists("a.txt");
来源：http://lld.xziqi.cn

JS:   fs.existsSync("a.txt")
来源：http://kln.yuanzhike.top

TS:   fs.existsSync("a.txt")
来源：http://vvz.9152youxi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://giw.cdnleiting.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fei.jinqigfzy.top

Ruby: File.exist?("a.txt")
来源：http://dtj.yuxming.cn

C#:   File.Exists("a.txt")
来源：http://ejd.zycfv.cn

[F06] 删除文件
来源：http://xqx.guowangkeji.top

Py:   os.remove("a.txt")
来源：http://zcp.xuanzx.com

PHP:  unlink("a.txt");
来源：http://pyd.redwolf501.top

JS:   fs.unlinkSync("a.txt")
来源：http://kny.yfazqb.com

TS:   fs.unlinkSync("a.txt")
来源：http://kof.shzxlz.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ffa.ydzc1.top

Go:   os.Remove("a.txt")
来源：http://xgz.pengpengdd.cyou

Ruby: File.delete("a.txt")
来源：http://qzl.cashguo.top

C#:   File.Delete("a.txt");
来源：http://wuf.yj20258888.top

[F07] 创建目录（含多级）
来源：http://oct.jianghu66.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fcc.hywenlv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mgz.0kj1m.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ney.zhaomingkeji.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://myp.jyoumei.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hrr.bbcook.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rrc.kuanghao11.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oah.hywenlv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://aii.smart0.xyz

[F08] 遍历目录
来源：http://vfd.zhoulong.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://dva.hesvh.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ypz.yj20258.top

JS:   fs.readdirSync("dir")
来源：http://uyq.xinyue.icu

TS:   fs.readdirSync("dir")
来源：http://dev.gzhubu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gyg.gogol.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://mlq.hywenlv.cn

Ruby: Dir.children("dir")
来源：http://usm.fktsv.cn

C#:   Directory.GetFiles("dir")
来源：http://qpe.xziqi.cn

[F09] 获取文件大小
来源：http://avl.ybcxt.top

Py:   os.path.getsize("a.txt")
来源：http://ggw.smart0.xyz

PHP:  filesize("a.txt");
来源：http://gro.nanxinkj.top

JS:   fs.statSync("a.txt").size
来源：http://yfz.yueranfly.top

TS:   fs.statSync("a.txt").size
来源：http://wrh.sxryk.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mcg.shzxlz.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cat.redwolf501.top

Ruby: File.size("a.txt")
来源：http://kck.shzxlz.cn

C#:   new FileInfo("a.txt").Length
来源：http://gfi.xziqi.cn

[F10] 取文件扩展名 / 文件名
来源：http://ikt.gaohongyu789.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://onz.fanxiaobao.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://esv.fktsv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cmp.meibo888.top

TS:   path.extname("a.txt")
来源：http://lxl.tianlin.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ori.xuanzx.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sak.yj202588.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://aqq.jlsjyb.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lpo.yj20258888.top

[F11] 复制与移动文件
来源：http://uyx.316326.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://aod.jinqigfzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hqh.c1oappe.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uqk.pengpengdd.cyou

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vym.andypj.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://myk.nanxinkj.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fro.sxryk.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rsd.gzhubu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mcj.nanxuanxn.top

[F12] CSV 读写
来源：http://ynr.yj20258888.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hqa.bjfxy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nxz.redwolf501.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vuv.aizwys.cn

TS:   // 同上
来源：http://xbn.jinyuanbaomall.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://txi.havefunace.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vhh.hnqzz.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jci.yvedp.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xry.ehwqpu.com

================================================================================
来源：http://syl.yonumen.top

G. 面向对象
来源：http://guo.zhijiandao.cn

================================================================================
来源：http://pza.yj202588.top

[G01] 定义类
来源：http://wmg.guannengcc.top

Py:   class User: pass
来源：http://ycl.nwbrower.top

PHP:  class User {}
来源：http://vkq.ydjk.org.cn

JS:   class User {}
来源：http://trh.yueranfly.top

TS:   class User { name: string = ""; }
来源：http://gjn.zycfv.cn

Java: class User {}
来源：http://ptb.meibo888.top

Go:   type User struct { Name string }
来源：http://kph.fengsongda.top

Ruby: class User; end
来源：http://xrp.smart0.xyz

C#:   class User {}
来源：http://fko.epnwcf.com

[G02] 构造函数
来源：http://tzy.ydjk.org.cn

Py:   def __init__(self, name): self.name = name
来源：http://zju.svipenyu.cn

PHP:  public function __construct(public string $name) {}
来源：http://kzw.uphjek.com

JS:   constructor(name) { this.name = name; }
来源：http://qqc.shangyingyoupin.top

TS:   constructor(public name: string) {}
来源：http://ibf.9152youxi.cn

Java: User(String name) { this.name = name; }
来源：http://vsr.xziqi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jls.zhongyouzk.top

Ruby: def initialize(name); @name = name; end
来源：http://wmk.shanyushiyangtech.top

C#:   public User(string name) { Name = name; }
来源：http://itp.fanxiaobao.xyz

[G03] 实例属性
来源：http://kim.tarul.cn

Py:   self.name = "x"
来源：http://sld.nwbrower.top

PHP:  public string $name = "x";
来源：http://vws.9152youxi.cn

JS:   this.name = "x";
来源：http://fmo.dianchejie.cn

TS:   name: string = "x";
来源：http://eve.jinqigufen.top

Java: private String name;
来源：http://uwu.ivvv.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ojl.zhiwuduotai.top

Ruby: @name = "x"
来源：http://ixh.yj20258.top

C#:   public string Name { get; set; } = "x";
来源：http://cmm.fzhhl.top

[G04] 定义方法
来源：http://qcd.meibo888.top

Py:   def greet(self): return self.name
来源：http://dls.xuanzx.com

PHP:  public function greet(): string { return $this->name; }
来源：http://eps.jqgfzy.top

JS:   greet() { return this.name; }
来源：http://oan.c1oappe.top

TS:   greet(): string { return this.name; }
来源：http://wah.zhijiandao.cn

Java: String greet() { return name; }
来源：http://mpe.xuanzx.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://kny.jinqigufen.top

Ruby: def greet; @name; end
来源：http://uur.gaohongyu789.top

C#:   public string Greet() => Name;
来源：http://jic.ppjwa.cn

[G05] 继承
来源：http://art.chenzaomai.com

Py:   class Admin(User): pass
来源：http://hpm.jyoumei.cn

PHP:  class Admin extends User {}
来源：http://vhi.iojbl.cn

JS:   class Admin extends User {}
来源：http://pxt.yongpay.top

TS:   class Admin extends User {}
来源：http://upn.iojbl.cn

Java: class Admin extends User {}
来源：http://dzk.9152youxi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mzl.zhixingplan.top

Ruby: class Admin < User; end
来源：http://foz.tarul.cn

C#:   class Admin : User {}
来源：http://mub.yongpay.top

[G06] 重写方法
来源：http://muz.yj202588.top

Py:   def greet(self): return "admin"
来源：http://pzm.dashuyun.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mgv.mhx1999.top

JS:   greet() { return "admin"; }
来源：http://myp.uphjek.com

TS:   greet(): string { return "admin"; }
来源：http://vnk.zhoulong.xyz

Java: @Override String greet() { return "admin"; }
来源：http://gmb.pycfn.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nws.epnwcf.com

Ruby: def greet; "admin"; end
来源：http://rqj.jinqigfzy.top

C#:   public override string Greet() => "admin";
来源：http://wdi.fengsongda.top

[G07] 调用父类方法
来源：http://fxe.svipenyu.cn

Py:   super().greet()
来源：http://zmy.jinghuilouyu.cn

PHP:  parent::greet();
来源：http://fkn.ehwqpu.com

JS:   super.greet();
来源：http://ecw.guowangkeji.top

TS:   super.greet();
来源：http://doc.wangdashe.top

Java: super.greet();
来源：http://far.jianghu66.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://eoh.hesvh.cn

Ruby: super
来源：http://tqe.jinyuanbaomall.cn

C#:   base.Greet();
来源：http://ljy.52xcode.cn

[G08] 静态方法与属性
来源：http://hws.gzhubu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://oik.yangfankeji.com

PHP:  public static function f() {}
来源：http://vpm.yj202588.top

JS:   static f() {}
来源：http://jhw.zhaomingkeji.xyz

TS:   static f(): void {}
来源：http://fmu.gogol.net.cn

Java: static void f() {}
来源：http://dwf.jinyuanbaomall.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://crm.gotoacloud.top

Ruby: def self.f; end
来源：http://idi.zhongyouzk.top

C#:   public static void F() {}
来源：http://rid.gzhubu.top

[G09] 接口 / 抽象类
来源：http://pzq.cheryme.top

Py:   from abc import ABC, abstractmethod
来源：http://lyi.zhixingplan.top

PHP:  interface Shape { public function area(): float; }
来源：http://waz.tianlin.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://ior.feifeiyinyue.top

TS:   interface Shape { area(): number; }
来源：http://mkd.cqqwz.cn

Java: interface Shape { double area(); }
来源：http://iuu.nanxuanxn.top

Go:   type Shape interface { Area() float64 }
来源：http://fde.zhixingplan.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yny.chenzaomai.com

C#:   interface IShape { double Area(); }
来源：http://rbe.shuidangran.top

[G10] 访问控制
来源：http://vee.ehwqpu.com

Py:   约定 _protected / __private（不强制）
来源：http://ben.uphjek.com

PHP:  public / protected / private
来源：http://tyv.fanxiaobao.xyz

JS:   #private 字段；其余公开
来源：http://kln.shzxlz.cn

TS:   public / protected / private
来源：http://pxo.yj20258888.top

Java: public / protected / private / 默认包级
来源：http://umm.ctjpmb.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://fhe.jqgufenzy.top

Ruby: public / protected / private
来源：http://ltd.jlsjyb.cn

C#:   public / protected / private / internal
来源：http://rwp.ppjwa.cn

[G11] getter / setter
来源：http://rip.zhaomingkeji.xyz

Py:   @property 与 @x.setter
来源：http://dlk.havefunace.top

PHP:  public function getName(): string { return $this->name; }
来源：http://xni.svipenyu.cn

JS:   get name() { return this._name; }
来源：http://xen.guannengcc.top

TS:   get name(): string { return this._name; }
来源：http://hnr.hongshengwenyu.top

Java: public String getName() { return name; }
来源：http://jkf.yfazqb.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://ags.jinghuilouyu.cn

Ruby: attr_accessor :name
来源：http://qbt.xingfuxueyuan.xyz

C#:   public string Name { get; set; }
来源：http://bqa.shanyushiyangtech.top

[G12] 对象转字符串
来源：http://vdp.316326.xyz

Py:   def __str__(self): return self.name
来源：http://mto.yfazqb.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://zph.hysaishi.cn

JS:   toString() { return this.name; }
来源：http://dpm.quarkkingdee.top

TS:   toString(): string { return this.name; }
来源：http://yqx.dianchejie.cn

Java: @Override public String toString() { return name; }
来源：http://xco.havefunace.top

Go:   func (u User) String() string { return u.Name }
来源：http://tjz.hongshengwenyu.top

Ruby: def to_s; @name; end
来源：http://hbs.xuetiantiany.cn

C#:   public override string ToString() => Name;
来源：http://swg.fktsv.cn

[G13] 判断对象类型
来源：http://fkt.gzhubu.top

Py:   isinstance(u, User)
来源：http://xdn.yvedp.cn

PHP:  $u instanceof User
来源：http://rqz.iojbl.cn

JS:   u instanceof User
来源：http://gsw.yj20258.top

TS:   u instanceof User
来源：http://dxb.meibo888.top

Java: u instanceof User
来源：http://kcj.yfazqb.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://pkk.aizwys.cn

Ruby: u.is_a?(User)
来源：http://rnr.yuanzhike.top

C#:   u is User
来源：http://kzx.sufxvd.cn

[G14] 数据类 / record
来源：http://wro.fzhhl.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kfy.havefunace.top

PHP:  // 用 readonly 属性模拟
来源：http://jsr.xziqi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://hgs.hammf.cn

TS:   type User = { name: string; age: number };
来源：http://zsv.wangshuangyany.cn

Java: record User(String name, int age) {}
来源：http://njv.vehdjk.com

Go:   type User struct { Name string; Age int }
来源：http://maq.shangyingyoupin.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lil.hysaishi.cn

C#:   record User(string Name, int Age);
来源：http://jrw.zycfv.cn

[G15] 枚举
来源：http://pgu.ydzc1.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://atg.shuidangran.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://srv.hnxiangtu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jgw.hywenlv.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wxh.snrcjt.cn

Java: enum Color { RED, GREEN }
来源：http://tkt.zhengqikj.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cuk.chenlongwang.top

Ruby: Color = %i[red green].freeze
来源：http://zgx.yonumen.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rpu.cdnleiting.top

[G16] 对象转数组 / 字典
来源：http://rse.chenlongwang.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kti.hysaishi.cn

PHP:  get_object_vars($obj);
来源：http://uqk.pengpengdd.cyou

JS:   Object.entries(obj)
来源：http://wfl.tianlin.xyz

TS:   Object.entries(obj)
来源：http://ooy.xinyue.icu

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hxj.meibo888.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://bdz.chenlongwang.top

Ruby: obj.instance_variables
来源：http://tln.cucudq.cn

C#:   // 用反射或 System.Text.Json
来源：http://puf.zdqjudy.top

================================================================================
来源：http://ryc.fehbvm.com

H. 异常与错误处理
来源：http://qda.chenjidiqi.icu

================================================================================
来源：http://stm.xziqi.cn

[H01] try / catch 基础
来源：http://gzn.yueranfly.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://iqy.chenjidiqi.icu

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hwy.ehwqpu.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vyg.fktsv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bem.havefunace.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fcv.meibo888.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cdv.cashguo.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://iqw.jlsjyb.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zmm.aibaodan.cn

[H02] finally / ensure 收尾
来源：http://wax.fengsongda.top

Py:   try: f()⏎finally: cleanup()
来源：http://wnx.fengsongda.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://nya.jqgufenzy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://acb.zhijiandao.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://aax.snrcjt.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hcf.nanxinkj.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://gee.yj20258888.top

Ruby: begin; f; ensure; cleanup; end
来源：http://coo.c1oappe.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://tub.ctjpmb.com

[H03] 主动抛出异常
来源：http://wlk.zhongyouzk.top

Py:   raise ValueError("错误信息")
来源：http://ikz.havefunace.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ggv.xuetiantiany.cn

JS:   throw new Error("错误信息");
来源：http://ggz.chenlongwang.top

TS:   throw new Error("错误信息");
来源：http://btm.sufxvd.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pcz.aizwys.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lsf.jqgfzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://iyk.yj20258.top

C#:   throw new ArgumentException("错误信息");
来源：http://bpq.bbcook.cn

[H04] 自定义异常类型
来源：http://jra.feifeiyinyue.top

Py:   class MyError(Exception): pass
来源：http://byb.jinyuanbaomall.cn

PHP:  class MyError extends RuntimeException {}
来源：http://zxh.hongshengwenyu.top

JS:   class MyError extends Error {}
来源：http://ony.jyoumei.cn

TS:   class MyError extends Error {}
来源：http://zsa.wangdashe.top

Java: class MyException extends RuntimeException {}
来源：http://dvl.andypj.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://erq.xziqi.cn

Ruby: class MyError < StandardError; end
来源：http://qzw.gzhubu.top

C#:   class MyException : Exception {}
来源：http://zww.bjfxy.top

[H05] 捕获特定类型
来源：http://rcf.zdqjudy.top

Py:   except ValueError as e:
来源：http://xlm.chenzaomai.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tkw.sweek.top

JS:   if (e instanceof TypeError) {}
来源：http://afo.meibo888.top

TS:   if (e instanceof TypeError) {}
来源：http://bgo.316326.xyz

Java: catch (IOException | SQLException e) {}
来源：http://wuj.jqgfzy.top


<!-- 参考信息 -->