代发 wailian999

[F01] 读取整个文件
来源：http://ida.meibo888.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lnq.iojbl.cn

PHP:  file_get_contents("a.txt");
来源：http://azz.yfazqb.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ffs.iojbl.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lom.ybcxt.top

Java: Files.readString(Path.of("a.txt"))
来源：http://pbc.jinghuilouyu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bav.svipenyu.cn

Ruby: File.read("a.txt")
来源：http://atk.daria6918.cn

C#:   File.ReadAllText("a.txt");
来源：http://lwb.chenzaomai.com

[F02] 逐行读取文件
来源：http://piy.ywan-chungtsiang.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jvd.shzxlz.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gdr.zycfv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pgb.shuidangran.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://awl.redwolf501.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://umm.zhijiandao.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://knh.zhongyouzk.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pfp.zhiwuduotai.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pxq.zhijiandao.cn

[F03] 写入文件（覆盖）
来源：http://lav.meibo888.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ese.wangshuangyany.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://omk.xingfuxueyuan.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vcd.gotoacloud.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ead.pengpengdd.cyou

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xou.uphjek.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lpp.52xcode.cn

Ruby: File.write("a.txt", "hi")
来源：http://wwb.sweek.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jit.pengpengdd.cyou

[F04] 追加写入文件
来源：http://apd.yj20258.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://efj.cqqwz.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hiw.guowangkeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fks.xziqi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lsi.xziqi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fbd.andypj.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://muz.tarul.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qgh.xingfuxueyuan.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cld.nanxinkj.top

[F05] 判断文件或目录是否存在
来源：http://isk.xuanzx.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bkx.nanxuanxn.top

PHP:  file_exists("a.txt");
来源：http://kgk.xziqi.cn

JS:   fs.existsSync("a.txt")
来源：http://gua.316326.xyz

TS:   fs.existsSync("a.txt")
来源：http://gyd.zdbjq.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://sgs.zdqjudy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jdy.zhixingplan.top

Ruby: File.exist?("a.txt")
来源：http://hfd.smart0.xyz

C#:   File.Exists("a.txt")
来源：http://ptr.svipenyu.cn

[F06] 删除文件
来源：http://yeq.cdnleiting.top

Py:   os.remove("a.txt")
来源：http://rmj.nanxinkj.top

PHP:  unlink("a.txt");
来源：http://bgd.daria6918.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ngi.pengpengdd.cyou

TS:   fs.unlinkSync("a.txt")
来源：http://pym.jinyuanbaomall.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tqf.pengpengdd.cyou

Go:   os.Remove("a.txt")
来源：http://ebh.yongpay.top

Ruby: File.delete("a.txt")
来源：http://qvg.yuxming.cn

C#:   File.Delete("a.txt");
来源：http://wzm.jinqigufen.top

[F07] 创建目录（含多级）
来源：http://vhz.mhx1999.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mzd.uphjek.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://alk.birdmap.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://clc.yfazqb.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gah.sxryk.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bxo.vehdjk.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pag.birdmap.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ltu.jlsjyb.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://soj.tian-w.cn

[F08] 遍历目录
来源：http://vfv.gzhubu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://cpe.gaohongyu789.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lbi.tanke756.top

JS:   fs.readdirSync("dir")
来源：http://xhz.sufxvd.cn

TS:   fs.readdirSync("dir")
来源：http://lhv.mhx1999.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ujw.tianlin.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://izv.tanke756.top

Ruby: Dir.children("dir")
来源：http://flp.sjlbkw.cn

C#:   Directory.GetFiles("dir")
来源：http://iqx.jinghuilouyu.cn

[F09] 获取文件大小
来源：http://nff.redwolf501.top

Py:   os.path.getsize("a.txt")
来源：http://vvp.daxiang520.top

PHP:  filesize("a.txt");
来源：http://spi.fktsv.cn

JS:   fs.statSync("a.txt").size
来源：http://atm.sxryk.cn

TS:   fs.statSync("a.txt").size
来源：http://vtn.ivvv.top

Java: Files.size(Path.of("a.txt"))
来源：http://xmx.ppjwa.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wax.yfazqb.com

Ruby: File.size("a.txt")
来源：http://fyh.jqgfzy.top

C#:   new FileInfo("a.txt").Length
来源：http://lau.zdbjq.cn

[F10] 取文件扩展名 / 文件名
来源：http://les.xylfe.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yqq.cucudq.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zyf.pycfn.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cah.pengpengdd.cyou

TS:   path.extname("a.txt")
来源：http://esg.daxiang520.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cqq.yj20258.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jif.zdqjudy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zoc.ywan-chungtsiang.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://woh.ctjpmb.com

[F11] 复制与移动文件
来源：http://rlj.xingfuxueyuan.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gtg.jiagoushi.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mml.hongshengwenyu.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wgb.jqgufenzy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bjx.zhijiandao.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ede.epnwcf.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lqr.gogol.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wtj.ydzc1.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zxk.birdmap.top

[F12] CSV 读写
来源：http://mqr.zhaomingkeji.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gtc.meibo888.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cdg.jyoumei.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mmw.zhoulong.xyz

TS:   // 同上
来源：http://kzc.meibo888.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bvj.vqdsnc.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vgz.yfazqb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xaf.jqgufenzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://sze.daxiang520.top

================================================================================
来源：http://pth.ydjk.org.cn

G. 面向对象
来源：http://ste.hysaishi.cn

================================================================================
来源：http://jyt.yongpay.top

[G01] 定义类
来源：http://rvb.fktsv.cn

Py:   class User: pass
来源：http://ztk.kuanghao11.cn

PHP:  class User {}
来源：http://xta.yj202588.top

JS:   class User {}
来源：http://wxq.kuanghao11.cn

TS:   class User { name: string = ""; }
来源：http://omv.xuetiantiany.cn

Java: class User {}
来源：http://hzj.bjfxy.top

Go:   type User struct { Name string }
来源：http://nlz.sufxvd.cn

Ruby: class User; end
来源：http://bno.quarkkingdee.top

C#:   class User {}
来源：http://wdd.xuetiantiany.cn

[G02] 构造函数
来源：http://yrm.zhaomingkeji.xyz

Py:   def __init__(self, name): self.name = name
来源：http://cph.zhongyouzk.top

PHP:  public function __construct(public string $name) {}
来源：http://ntp.birdmap.top

JS:   constructor(name) { this.name = name; }
来源：http://bsm.yangfankeji.com

TS:   constructor(public name: string) {}
来源：http://mya.wangdashe.top

Java: User(String name) { this.name = name; }
来源：http://kul.ehwqpu.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pch.hysaishi.cn

Ruby: def initialize(name); @name = name; end
来源：http://mfn.sjlbkw.cn

C#:   public User(string name) { Name = name; }
来源：http://suo.shzxlz.cn

[G03] 实例属性
来源：http://puk.hysaishi.cn

Py:   self.name = "x"
来源：http://tjf.tarul.cn

PHP:  public string $name = "x";
来源：http://xlf.xylfe.cn

JS:   this.name = "x";
来源：http://azk.xziqi.cn

TS:   name: string = "x";
来源：http://eae.hesvh.cn

Java: private String name;
来源：http://zfl.fanxiaobao.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qfl.zhiwuduotai.top

Ruby: @name = "x"
来源：http://iix.vqdsnc.cn

C#:   public string Name { get; set; } = "x";
来源：http://ekm.sweek.top

[G04] 定义方法
来源：http://xid.zdbjq.cn

Py:   def greet(self): return self.name
来源：http://hbx.yueranfly.top

PHP:  public function greet(): string { return $this->name; }
来源：http://geg.sjlbkw.cn

JS:   greet() { return this.name; }
来源：http://yqi.hesvh.cn

TS:   greet(): string { return this.name; }
来源：http://oyr.chenlongwang.top

Java: String greet() { return name; }
来源：http://hwc.dianchejie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pgz.yanxiufei.cn

Ruby: def greet; @name; end
来源：http://zor.hnqzz.top

C#:   public string Greet() => Name;
来源：http://hxg.aizwys.cn

[G05] 继承
来源：http://bcg.sysykeji.top

Py:   class Admin(User): pass
来源：http://toi.gzhubu.top

PHP:  class Admin extends User {}
来源：http://omz.aizwys.cn

JS:   class Admin extends User {}
来源：http://hlh.hongshengwenyu.top

TS:   class Admin extends User {}
来源：http://zez.hesvh.cn

Java: class Admin extends User {}
来源：http://geb.yj20258.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://aba.jqgufenzy.top

Ruby: class Admin < User; end
来源：http://ill.andypj.xyz

C#:   class Admin : User {}
来源：http://ofc.zdqjudy.top

[G06] 重写方法
来源：http://qre.jiagoushi.top

Py:   def greet(self): return "admin"
来源：http://yyv.fktsv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wtt.yuanzhike.top

JS:   greet() { return "admin"; }
来源：http://bnb.jinghuilouyu.cn

TS:   greet(): string { return "admin"; }
来源：http://znp.hnqzz.top

Java: @Override String greet() { return "admin"; }
来源：http://use.xziqi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gfc.hcnkem.com

Ruby: def greet; "admin"; end
来源：http://fsx.cheryme.top

C#:   public override string Greet() => "admin";
来源：http://brt.yj202588.top

[G07] 调用父类方法
来源：http://yob.zhijiandao.cn

Py:   super().greet()
来源：http://wnn.gzhubu.top

PHP:  parent::greet();
来源：http://woz.meibo888.top

JS:   super.greet();
来源：http://wtj.ppjwa.cn

TS:   super.greet();
来源：http://ure.hesvh.cn

Java: super.greet();
来源：http://sfb.nwbrower.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sam.yonumen.top

Ruby: super
来源：http://ylr.epnwcf.com

C#:   base.Greet();
来源：http://peo.tarul.cn

[G08] 静态方法与属性
来源：http://hyg.yuxming.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://djv.zdqjudy.top

PHP:  public static function f() {}
来源：http://gaf.52xcode.cn

JS:   static f() {}
来源：http://vwb.iojbl.cn

TS:   static f(): void {}
来源：http://flk.jianghu66.top

Java: static void f() {}
来源：http://nsk.fehbvm.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://hxv.redwolf501.top

Ruby: def self.f; end
来源：http://krf.cucudq.cn

C#:   public static void F() {}
来源：http://yly.jiagoushi.top

[G09] 接口 / 抽象类
来源：http://kmz.fanxiaobao.xyz

Py:   from abc import ABC, abstractmethod
来源：http://tsq.nanxinkj.top

PHP:  interface Shape { public function area(): float; }
来源：http://eyq.gzhubu.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://eel.0kj1m.cn

TS:   interface Shape { area(): number; }
来源：http://fkj.yuanzhike.top

Java: interface Shape { double area(); }
来源：http://znb.shanyushiyangtech.top

Go:   type Shape interface { Area() float64 }
来源：http://lvr.chenlongwang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wjx.fanxiaobao.xyz

C#:   interface IShape { double Area(); }
来源：http://gec.wangdashe.top

[G10] 访问控制
来源：http://lyr.zhengqikj.top

Py:   约定 _protected / __private（不强制）
来源：http://lre.hysaishi.cn

PHP:  public / protected / private
来源：http://fnb.shangyingyoupin.top

JS:   #private 字段；其余公开
来源：http://nwx.ivvv.top

TS:   public / protected / private
来源：http://lhx.gaohongyu789.top

Java: public / protected / private / 默认包级
来源：http://mpt.zhengqikj.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://xxd.feifeiyinyue.top

Ruby: public / protected / private
来源：http://abp.shanyushiyangtech.top

C#:   public / protected / private / internal
来源：http://hjo.cqqwz.cn

[G11] getter / setter
来源：http://phs.xingfuxueyuan.xyz

Py:   @property 与 @x.setter
来源：http://rlx.shuidangran.top

PHP:  public function getName(): string { return $this->name; }
来源：http://wjn.guannengcc.top

JS:   get name() { return this._name; }
来源：http://eiq.shzxlz.cn

TS:   get name(): string { return this._name; }
来源：http://nlj.andypj.xyz

Java: public String getName() { return name; }
来源：http://msi.jlsjyb.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://krh.ehwqpu.com

Ruby: attr_accessor :name
来源：http://ccl.daxiang520.top

C#:   public string Name { get; set; }
来源：http://wcf.jiagoushi.top

[G12] 对象转字符串
来源：http://vqi.shzxlz.cn

Py:   def __str__(self): return self.name
来源：http://jcs.hammf.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jus.chenlongwang.top

JS:   toString() { return this.name; }
来源：http://efv.c1oappe.top

TS:   toString(): string { return this.name; }
来源：http://hax.mhx1999.top

Java: @Override public String toString() { return name; }
来源：http://wka.zdqjudy.top

Go:   func (u User) String() string { return u.Name }
来源：http://vfv.52xcode.cn

Ruby: def to_s; @name; end
来源：http://goe.ppjwa.cn

C#:   public override string ToString() => Name;
来源：http://cii.pengpengdd.cyou

[G13] 判断对象类型
来源：http://lum.9152youxi.cn

Py:   isinstance(u, User)
来源：http://pcw.havefunace.top

PHP:  $u instanceof User
来源：http://mhi.xingfuxueyuan.xyz

JS:   u instanceof User
来源：http://gbw.0kj1m.cn

TS:   u instanceof User
来源：http://mnn.jqgfzy.top

Java: u instanceof User
来源：http://idl.0kj1m.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ozf.cdnleiting.top

Ruby: u.is_a?(User)
来源：http://uos.zhaomingkeji.xyz

C#:   u is User
来源：http://ios.vqdsnc.cn

[G14] 数据类 / record
来源：http://ecl.fzhhl.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mdr.hysaishi.cn

PHP:  // 用 readonly 属性模拟
来源：http://uhz.zhengqikj.top

JS:   // 无内置：普通类或对象字面量
来源：http://wxq.jianghu66.top

TS:   type User = { name: string; age: number };
来源：http://gnx.zycfv.cn

Java: record User(String name, int age) {}
来源：http://rkk.haohaochexian.top

Go:   type User struct { Name string; Age int }
来源：http://knb.tianlin.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rzh.nanxinkj.top

C#:   record User(string Name, int Age);
来源：http://lju.cqqwz.cn

[G15] 枚举
来源：http://ptv.tarul.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bnn.yongpay.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://yrd.guannengcc.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fqh.zhijiandao.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bbp.havefunace.top

Java: enum Color { RED, GREEN }
来源：http://crb.smart0.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pdh.fktsv.cn

Ruby: Color = %i[red green].freeze
来源：http://bcl.shanyushiyangkeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xhs.yongpay.top

[G16] 对象转数组 / 字典
来源：http://nut.fanxiaobao.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://naw.shangyingyoupin.top

PHP:  get_object_vars($obj);
来源：http://zxr.cqqwz.cn

JS:   Object.entries(obj)
来源：http://jgo.bjfxy.top

TS:   Object.entries(obj)
来源：http://dto.jinyuanbaomall.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ywv.aizwys.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://lmx.cheryme.top

Ruby: obj.instance_variables
来源：http://uxu.tarul.cn

C#:   // 用反射或 System.Text.Json
来源：http://gzz.jqgfzy.top

================================================================================
来源：http://icq.jinqigfzy.top

H. 异常与错误处理
来源：http://ibg.daxiang520.top

================================================================================
来源：http://aac.cdnleiting.top

[H01] try / catch 基础
来源：http://cyq.wangdashe.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hve.bjfxy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mol.ppjwa.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yvm.c1oappe.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uce.yuxming.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jex.havefunace.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lrv.pengpengdd.cyou

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://luj.0kj1m.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pae.fanxiaobao.xyz

[H02] finally / ensure 收尾
来源：http://plp.zhaomingkeji.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://vtk.havefunace.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://lig.sxryk.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qzd.zhongyouzk.top

TS:   try { f(); } finally { cleanup(); }
来源：http://dpj.ydjk.org.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xxp.yonumen.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://iee.gogol.net.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bba.yj202588.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ass.tanke756.top

[H03] 主动抛出异常
来源：http://gsd.tarul.cn

Py:   raise ValueError("错误信息")
来源：http://gdk.yj20258.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qkz.redwolf501.top

JS:   throw new Error("错误信息");
来源：http://fkf.316326.xyz

TS:   throw new Error("错误信息");
来源：http://xez.guannengcc.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ghc.xziqi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uss.shuidangran.top

Ruby: raise ArgumentError, "错误信息"
来源：http://lhs.yongpay.top

C#:   throw new ArgumentException("错误信息");
来源：http://vmd.316326.xyz

[H04] 自定义异常类型
来源：http://xno.jinghuilouyu.cn

Py:   class MyError(Exception): pass
来源：http://mxh.shangyingyoupin.top

PHP:  class MyError extends RuntimeException {}
来源：http://unw.0kj1m.cn

JS:   class MyError extends Error {}
来源：http://egl.jqgufenzy.top

TS:   class MyError extends Error {}
来源：http://mao.hnxiangtu.top

Java: class MyException extends RuntimeException {}
来源：http://lrf.sysykeji.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://imd.gotoacloud.top

Ruby: class MyError < StandardError; end
来源：http://rhq.yongpay.top

C#:   class MyException : Exception {}
来源：http://dcs.birdmap.top

[H05] 捕获特定类型
来源：http://nsm.ydjk.org.cn

Py:   except ValueError as e:
来源：http://ais.jiagoushi.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qur.c1oappe.top

JS:   if (e instanceof TypeError) {}
来源：http://hye.jinqigufen.top

TS:   if (e instanceof TypeError) {}
来源：http://qkl.jinyuanbaomall.cn

Java: catch (IOException | SQLException e) {}
来源：http://vso.shzxlz.cn


<!-- 参考信息 -->