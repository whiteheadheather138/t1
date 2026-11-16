代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jpl.zhixingplan.top

================================================================================
来源：http://tqc.cqqwz.cn

F. 文件与目录
来源：http://ajl.zhongyouzk.top

================================================================================
来源：http://tfu.zycfv.cn

[F01] 读取整个文件
来源：http://hti.nanxuanxn.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kht.sxryk.cn

PHP:  file_get_contents("a.txt");
来源：http://hcz.ctjpmb.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nfr.fanxiaobao.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yzc.shangyingyoupin.top

Java: Files.readString(Path.of("a.txt"))
来源：http://rwn.gaohongyu789.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lfw.c1oappe.top

Ruby: File.read("a.txt")
来源：http://sxa.jinghuilouyu.cn

C#:   File.ReadAllText("a.txt");
来源：http://nps.sjlbkw.cn

[F02] 逐行读取文件
来源：http://iin.ppjwa.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vyi.cheryme.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://krw.hnxiangtu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nkz.316326.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jad.cucudq.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://egh.yuxming.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hjx.fktsv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kaj.fktsv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ghy.feifeiyinyue.top

[F03] 写入文件（覆盖）
来源：http://lhn.sufxvd.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pgh.jianghu66.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://qej.dianchejie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://prn.ydjk.org.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://moe.yfazqb.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://eys.yuxming.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://skq.c1oappe.top

Ruby: File.write("a.txt", "hi")
来源：http://orh.ehwqpu.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://shf.xingfuxueyuan.xyz

[F04] 追加写入文件
来源：http://zab.jyoumei.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fdj.zhengqikj.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zox.zhiwuduotai.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eqy.jlsjyb.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jjr.nanxuanxn.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://grc.jyoumei.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dxu.shangyingyoupin.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yth.zhoulong.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://usr.hywenlv.cn

[F05] 判断文件或目录是否存在
来源：http://asl.zhongyouzk.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zgd.xziqi.cn

PHP:  file_exists("a.txt");
来源：http://gls.nanxuanxn.top

JS:   fs.existsSync("a.txt")
来源：http://tgw.yj20258888.top

TS:   fs.existsSync("a.txt")
来源：http://sgy.zhixingplan.top

Java: Files.exists(Path.of("a.txt"))
来源：http://npr.xylfe.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lgg.ydzc1.top

Ruby: File.exist?("a.txt")
来源：http://jku.daria6918.cn

C#:   File.Exists("a.txt")
来源：http://vqz.jqgufenzy.top

[F06] 删除文件
来源：http://hws.quarkkingdee.top

Py:   os.remove("a.txt")
来源：http://iyn.xylfe.cn

PHP:  unlink("a.txt");
来源：http://giq.xuetiantiany.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pbv.xuetiantiany.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ssg.hfpthk.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oah.jyoumei.cn

Go:   os.Remove("a.txt")
来源：http://rdf.ydzc1.top

Ruby: File.delete("a.txt")
来源：http://llw.nanxinkj.top

C#:   File.Delete("a.txt");
来源：http://uwr.zycfv.cn

[F07] 创建目录（含多级）
来源：http://cfy.mhx1999.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://oqm.shanyushiyangtech.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kwo.shzxlz.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ngf.tanke756.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ngg.yfazqb.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rxy.chenlongwang.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gwn.zhoulong.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://otb.xylfe.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rjf.ctjpmb.com

[F08] 遍历目录
来源：http://sam.yj20258888.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://qak.sxryk.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://upt.shzxlz.cn

JS:   fs.readdirSync("dir")
来源：http://dop.shangyingyoupin.top

TS:   fs.readdirSync("dir")
来源：http://pxv.gaohongyu789.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xbd.chenzaomai.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://yob.nwbrower.top

Ruby: Dir.children("dir")
来源：http://xcz.hammf.cn

C#:   Directory.GetFiles("dir")
来源：http://rxq.52xcode.cn

[F09] 获取文件大小
来源：http://wuv.hnqzz.top

Py:   os.path.getsize("a.txt")
来源：http://kjc.smart0.xyz

PHP:  filesize("a.txt");
来源：http://sdp.yanxiufei.cn

JS:   fs.statSync("a.txt").size
来源：http://krd.tian-w.cn

TS:   fs.statSync("a.txt").size
来源：http://llq.kuanghao11.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ohb.zdbjq.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zct.ywan-chungtsiang.top

Ruby: File.size("a.txt")
来源：http://ysd.yongpay.top

C#:   new FileInfo("a.txt").Length
来源：http://nwj.yuxming.cn

[F10] 取文件扩展名 / 文件名
来源：http://zet.jlsjyb.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fxe.yfazqb.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xzs.zhoulong.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://epx.shuidangran.top

TS:   path.extname("a.txt")
来源：http://yzj.zycfv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://psv.jqgfzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://llb.andypj.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wzv.zhixingplan.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tex.kuanghao11.cn

[F11] 复制与移动文件
来源：http://gaj.52xcode.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ozu.guowangkeji.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mfl.zhijiandao.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xea.chenjidiqi.icu

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rww.xziqi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://iol.hysaishi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fft.yj20258888.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xjn.havefunace.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wdt.birdmap.top

[F12] CSV 读写
来源：http://rmk.yuxming.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dyy.redwolf501.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://opu.guowangkeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gbh.sufxvd.cn

TS:   // 同上
来源：http://eaq.fengsongda.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ato.hnqzz.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mzq.hywenlv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bou.yuanzhike.top

C#:   // 无内置：用 CsvHelper 库
来源：http://scz.daxiang520.top

================================================================================
来源：http://gxu.cdnleiting.top

G. 面向对象
来源：http://jdw.uphjek.com

================================================================================
来源：http://yhw.hesvh.cn

[G01] 定义类
来源：http://tpu.xingfuxueyuan.xyz

Py:   class User: pass
来源：http://erq.bbcook.cn

PHP:  class User {}
来源：http://tiq.fengsongda.top

JS:   class User {}
来源：http://cbi.pycfn.com

TS:   class User { name: string = ""; }
来源：http://yzc.vehdjk.com

Java: class User {}
来源：http://mva.0kj1m.cn

Go:   type User struct { Name string }
来源：http://nov.zhengqikj.top

Ruby: class User; end
来源：http://byr.ctjpmb.com

C#:   class User {}
来源：http://ycp.kuanghao11.cn

[G02] 构造函数
来源：http://wre.yj20258888.top

Py:   def __init__(self, name): self.name = name
来源：http://laf.yj20258.top

PHP:  public function __construct(public string $name) {}
来源：http://djc.nwbrower.top

JS:   constructor(name) { this.name = name; }
来源：http://adt.yj202588.top

TS:   constructor(public name: string) {}
来源：http://qga.ppjwa.cn

Java: User(String name) { this.name = name; }
来源：http://dvf.epnwcf.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ivc.sufxvd.cn

Ruby: def initialize(name); @name = name; end
来源：http://heh.dashuyun.cn

C#:   public User(string name) { Name = name; }
来源：http://sue.316326.xyz

[G03] 实例属性
来源：http://lnf.tian-w.cn

Py:   self.name = "x"
来源：http://obe.pengpengdd.cyou

PHP:  public string $name = "x";
来源：http://pbr.jianghu66.top

JS:   this.name = "x";
来源：http://ttm.jyoumei.cn

TS:   name: string = "x";
来源：http://ycu.jyoumei.cn

Java: private String name;
来源：http://mnv.cashguo.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dkn.aizwys.cn

Ruby: @name = "x"
来源：http://zmv.snrcjt.cn

C#:   public string Name { get; set; } = "x";
来源：http://ybi.ppjwa.cn

[G04] 定义方法
来源：http://lfc.sjlbkw.cn

Py:   def greet(self): return self.name
来源：http://lnj.meibo888.top

PHP:  public function greet(): string { return $this->name; }
来源：http://syt.xinyue.icu

JS:   greet() { return this.name; }
来源：http://tnn.yvedp.cn

TS:   greet(): string { return this.name; }
来源：http://xxt.kuanghao11.cn

Java: String greet() { return name; }
来源：http://bxa.316326.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://tux.birdmap.top

Ruby: def greet; @name; end
来源：http://dcu.wangdashe.top

C#:   public string Greet() => Name;
来源：http://bqd.sjlbkw.cn

[G05] 继承
来源：http://kgc.xingfuxueyuan.xyz

Py:   class Admin(User): pass
来源：http://nrq.ybcxt.top

PHP:  class Admin extends User {}
来源：http://vfm.shanyushiyangtech.top

JS:   class Admin extends User {}
来源：http://yzl.guannengcc.top

TS:   class Admin extends User {}
来源：http://ocs.shanyushiyangkeji.top

Java: class Admin extends User {}
来源：http://uvy.chenlongwang.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wdp.ehwqpu.com

Ruby: class Admin < User; end
来源：http://bpk.yj202588.top

C#:   class Admin : User {}
来源：http://iue.nanxuanxn.top

[G06] 重写方法
来源：http://rug.jinqigufen.top

Py:   def greet(self): return "admin"
来源：http://yaf.gotoacloud.top

PHP:  public function greet(): string { return "admin"; }
来源：http://clk.nanxuanxn.top

JS:   greet() { return "admin"; }
来源：http://gym.gaohongyu789.top

TS:   greet(): string { return "admin"; }
来源：http://evi.jqgfzy.top

Java: @Override String greet() { return "admin"; }
来源：http://mhk.jqgfzy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rcn.zycfv.cn

Ruby: def greet; "admin"; end
来源：http://lym.andypj.xyz

C#:   public override string Greet() => "admin";
来源：http://ykz.chenzaomai.com

[G07] 调用父类方法
来源：http://oee.0kj1m.cn

Py:   super().greet()
来源：http://slu.zhixingplan.top

PHP:  parent::greet();
来源：http://lyr.fzhhl.top

JS:   super.greet();
来源：http://xsp.yfazqb.com

TS:   super.greet();
来源：http://ykv.gotoacloud.top

Java: super.greet();
来源：http://ynn.yj202588.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://iep.zhoulong.xyz

Ruby: super
来源：http://det.zhijiandao.cn

C#:   base.Greet();
来源：http://lbj.guowangkeji.top

[G08] 静态方法与属性
来源：http://ifc.ivvv.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uow.shanyushiyangtech.top

PHP:  public static function f() {}
来源：http://ows.xinyue.icu

JS:   static f() {}
来源：http://zlg.jianghu66.top

TS:   static f(): void {}
来源：http://glm.quarkkingdee.top

Java: static void f() {}
来源：http://ueb.shanyushiyangtech.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://yvj.mhx1999.top

Ruby: def self.f; end
来源：http://rmy.shuidangran.top

C#:   public static void F() {}
来源：http://odc.ppjwa.cn

[G09] 接口 / 抽象类
来源：http://jti.yj202588.top

Py:   from abc import ABC, abstractmethod
来源：http://zbk.yanxiufei.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ofe.hfpthk.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ejz.xinyue.icu

TS:   interface Shape { area(): number; }
来源：http://kxe.hesvh.cn

Java: interface Shape { double area(); }
来源：http://sjh.tarul.cn

Go:   type Shape interface { Area() float64 }
来源：http://yjj.shanyushiyangtech.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cqt.nanxuanxn.top

C#:   interface IShape { double Area(); }
来源：http://jsx.zhongyouzk.top

[G10] 访问控制
来源：http://bth.hywenlv.cn

Py:   约定 _protected / __private（不强制）
来源：http://bfr.chenjidiqi.icu

PHP:  public / protected / private
来源：http://qui.ppjwa.cn

JS:   #private 字段；其余公开
来源：http://sdg.andypj.xyz

TS:   public / protected / private
来源：http://aio.mhx1999.top

Java: public / protected / private / 默认包级
来源：http://vmr.shangyingyoupin.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qhm.tarul.cn

Ruby: public / protected / private
来源：http://dyu.yj20258888.top

C#:   public / protected / private / internal
来源：http://sdx.pengpengdd.cyou

[G11] getter / setter
来源：http://icv.shzxlz.cn

Py:   @property 与 @x.setter
来源：http://zmd.sysykeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://bxk.meibo888.top

JS:   get name() { return this._name; }
来源：http://lmz.shanyushiyangkeji.top

TS:   get name(): string { return this._name; }
来源：http://tyt.svipenyu.cn

Java: public String getName() { return name; }
来源：http://akr.gaohongyu789.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://uzn.c1oappe.top

Ruby: attr_accessor :name
来源：http://rfa.ppjwa.cn

C#:   public string Name { get; set; }
来源：http://cha.svipenyu.cn

[G12] 对象转字符串
来源：http://pwz.bjfxy.top

Py:   def __str__(self): return self.name
来源：http://azc.zhiwuduotai.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://mjw.vehdjk.com

JS:   toString() { return this.name; }
来源：http://jdz.shuidangran.top

TS:   toString(): string { return this.name; }
来源：http://mdi.fzhhl.top

Java: @Override public String toString() { return name; }
来源：http://xen.zhongyouzk.top

Go:   func (u User) String() string { return u.Name }
来源：http://igq.epnwcf.com

Ruby: def to_s; @name; end
来源：http://uxc.jlsjyb.cn

C#:   public override string ToString() => Name;
来源：http://ude.haohaochexian.top

[G13] 判断对象类型
来源：http://tuj.gotoacloud.top

Py:   isinstance(u, User)
来源：http://dhg.sxryk.cn

PHP:  $u instanceof User
来源：http://ptu.jinqigufen.top

JS:   u instanceof User
来源：http://zzc.aizwys.cn

TS:   u instanceof User
来源：http://wcv.xylfe.cn

Java: u instanceof User
来源：http://zsf.tanke756.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://wqc.hysaishi.cn

Ruby: u.is_a?(User)
来源：http://nid.zdqjudy.top

C#:   u is User
来源：http://aso.ctjpmb.com

[G14] 数据类 / record
来源：http://gyd.ctjpmb.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zay.quarkkingdee.top

PHP:  // 用 readonly 属性模拟
来源：http://zvb.52xcode.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xmo.vehdjk.com

TS:   type User = { name: string; age: number };
来源：http://rhn.yj20258888.top

Java: record User(String name, int age) {}
来源：http://dax.jianghu66.top

Go:   type User struct { Name string; Age int }
来源：http://lkw.aibaodan.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dmz.tarul.cn

C#:   record User(string Name, int Age);
来源：http://gnt.xylfe.cn

[G15] 枚举
来源：http://vtl.cdnleiting.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vsl.ybcxt.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://wkm.chenzaomai.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qix.vqdsnc.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nhg.daria6918.cn

Java: enum Color { RED, GREEN }
来源：http://nai.chenzaomai.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cnw.chenjidiqi.icu

Ruby: Color = %i[red green].freeze
来源：http://yvt.hywenlv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ize.yj20258888.top

[G16] 对象转数组 / 字典
来源：http://oer.shangyingyoupin.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zvx.iojbl.cn

PHP:  get_object_vars($obj);
来源：http://rfe.jinqigfzy.top

JS:   Object.entries(obj)
来源：http://dve.fzhhl.top

TS:   Object.entries(obj)
来源：http://dnl.chenzaomai.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://abf.ppjwa.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://tox.zhoulong.xyz

Ruby: obj.instance_variables
来源：http://hlk.pengpengdd.cyou

C#:   // 用反射或 System.Text.Json
来源：http://ucc.yj20258.top

================================================================================
来源：http://jub.nwbrower.top

H. 异常与错误处理
来源：http://tzs.hnxiangtu.top

================================================================================
来源：http://dnz.tianlin.xyz

[H01] try / catch 基础
来源：http://bdm.zhaomingkeji.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qgc.hysaishi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://eqi.jinqigufen.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fht.sufxvd.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vjm.52xcode.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://opd.tianlin.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ova.bbcook.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jii.hywenlv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://buj.xuetiantiany.cn

[H02] finally / ensure 收尾
来源：http://vzw.gaohongyu789.top

Py:   try: f()⏎finally: cleanup()
来源：http://jmp.sweek.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ccw.mhx1999.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ceq.ydjk.org.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zpz.jyoumei.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jol.yuxming.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://yfy.jinqigfzy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://oag.xuetiantiany.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gwf.tian-w.cn

[H03] 主动抛出异常
来源：http://gtd.ivvv.top

Py:   raise ValueError("错误信息")
来源：http://cvs.cheryme.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fiv.aizwys.cn

JS:   throw new Error("错误信息");
来源：http://trz.redwolf501.top

TS:   throw new Error("错误信息");
来源：http://ecn.havefunace.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://avi.ydzc1.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bao.sjlbkw.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://nyg.gaohongyu789.top

C#:   throw new ArgumentException("错误信息");
来源：http://yqb.xinyue.icu

[H04] 自定义异常类型
来源：http://igd.yj202588.top

Py:   class MyError(Exception): pass
来源：http://yhi.shanyushiyangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://uhb.hfpthk.cn

JS:   class MyError extends Error {}
来源：http://wxi.fehbvm.com

TS:   class MyError extends Error {}
来源：http://cmq.hnxiangtu.top

Java: class MyException extends RuntimeException {}
来源：http://vav.jiagoushi.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cws.aizwys.cn

Ruby: class MyError < StandardError; end
来源：http://uax.tanke756.top

C#:   class MyException : Exception {}
来源：http://bbc.yj20258.top

[H05] 捕获特定类型
来源：http://huw.tian-w.cn

Py:   except ValueError as e:
来源：http://ybh.guannengcc.top


<!-- 参考信息 -->