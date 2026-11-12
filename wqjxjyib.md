代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jpt.guowangkeji.top

================================================================================
来源：http://wbq.gaohongyu789.top

F. 文件与目录
来源：http://qib.aibaodan.cn

================================================================================
来源：http://ahq.smart0.xyz

[F01] 读取整个文件
来源：http://czt.nanxinkj.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wop.mhx1999.top

PHP:  file_get_contents("a.txt");
来源：http://rhd.meibo888.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ffd.hnqzz.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gjf.xuanzx.com

Java: Files.readString(Path.of("a.txt"))
来源：http://slf.c1oappe.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://moy.52xcode.cn

Ruby: File.read("a.txt")
来源：http://awq.ydzc1.top

C#:   File.ReadAllText("a.txt");
来源：http://por.jinqigfzy.top

[F02] 逐行读取文件
来源：http://yyd.yuxming.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tey.daria6918.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nab.pengpengdd.cyou

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://woo.zhiwuduotai.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qre.gzhubu.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lxs.chenlongwang.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://com.cucudq.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dsy.yvedp.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hbh.hesvh.cn

[F03] 写入文件（覆盖）
来源：http://viz.jqgufenzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fam.9152youxi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mis.zhengqikj.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rqj.yvedp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://owk.chenjidiqi.icu

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://aip.daria6918.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bnw.ydjk.org.cn

Ruby: File.write("a.txt", "hi")
来源：http://hmk.ppjwa.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wwk.meibo888.top

[F04] 追加写入文件
来源：http://hob.ctjpmb.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fjh.yangfankeji.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dun.daria6918.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vkd.ctjpmb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jbt.shanyushiyangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://anm.ehwqpu.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cso.dianchejie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dmx.fengsongda.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tdo.jinqigufen.top

[F05] 判断文件或目录是否存在
来源：http://bxd.bjfxy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ntw.cqqwz.cn

PHP:  file_exists("a.txt");
来源：http://ghd.yfazqb.com

JS:   fs.existsSync("a.txt")
来源：http://enk.fktsv.cn

TS:   fs.existsSync("a.txt")
来源：http://rgc.gaohongyu789.top

Java: Files.exists(Path.of("a.txt"))
来源：http://dfn.chenlongwang.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mjl.zhongyouzk.top

Ruby: File.exist?("a.txt")
来源：http://wkk.zhaomingkeji.xyz

C#:   File.Exists("a.txt")
来源：http://etj.nanxinkj.top

[F06] 删除文件
来源：http://zve.yj20258888.top

Py:   os.remove("a.txt")
来源：http://umq.52xcode.cn

PHP:  unlink("a.txt");
来源：http://rdv.jinqigfzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://unk.shanyushiyangtech.top

TS:   fs.unlinkSync("a.txt")
来源：http://qeh.haohaochexian.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nri.pycfn.com

Go:   os.Remove("a.txt")
来源：http://dhp.yuxming.cn

Ruby: File.delete("a.txt")
来源：http://qoo.shuidangran.top

C#:   File.Delete("a.txt");
来源：http://gco.zhongyouzk.top

[F07] 创建目录（含多级）
来源：http://exy.uphjek.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mzk.yvedp.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fst.meibo888.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jlx.hnxiangtu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://img.snrcjt.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://osr.pengpengdd.cyou

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dxt.tianlin.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dbm.wangshuangyany.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://abm.xuanzx.com

[F08] 遍历目录
来源：http://vfa.xuanzx.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://psn.nwbrower.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://joh.pycfn.com

JS:   fs.readdirSync("dir")
来源：http://yoz.yongpay.top

TS:   fs.readdirSync("dir")
来源：http://rkf.cucudq.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dgt.shanyushiyangkeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://vmn.gaohongyu789.top

Ruby: Dir.children("dir")
来源：http://ioe.nwbrower.top

C#:   Directory.GetFiles("dir")
来源：http://zop.yonumen.top

[F09] 获取文件大小
来源：http://xkb.xingfuxueyuan.xyz

Py:   os.path.getsize("a.txt")
来源：http://rtj.yvedp.cn

PHP:  filesize("a.txt");
来源：http://mmx.nanxinkj.top

JS:   fs.statSync("a.txt").size
来源：http://juj.tarul.cn

TS:   fs.statSync("a.txt").size
来源：http://ggy.yongpay.top

Java: Files.size(Path.of("a.txt"))
来源：http://dge.fktsv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zps.jyoumei.cn

Ruby: File.size("a.txt")
来源：http://bky.ehwqpu.com

C#:   new FileInfo("a.txt").Length
来源：http://tyj.ywan-chungtsiang.top

[F10] 取文件扩展名 / 文件名
来源：http://xiv.svipenyu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wva.cashguo.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fsc.hcnkem.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://msi.zdqjudy.top

TS:   path.extname("a.txt")
来源：http://ico.zdbjq.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://suh.hongshengwenyu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rpu.jlsjyb.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://htk.guannengcc.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bxq.zhoulong.xyz

[F11] 复制与移动文件
来源：http://mir.ybcxt.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dny.dashuyun.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://clu.ywan-chungtsiang.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xuj.hesvh.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://syp.52xcode.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xiy.epnwcf.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gmx.jqgufenzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://orq.daxiang520.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qhz.ydjk.org.cn

[F12] CSV 读写
来源：http://aue.chenjidiqi.icu

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nxq.cucudq.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zsm.aibaodan.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nxu.xingfuxueyuan.xyz

TS:   // 同上
来源：http://sbg.yvedp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rkn.meibo888.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://caf.shanyushiyangtech.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yex.sysykeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://vhp.snrcjt.cn

================================================================================
来源：http://dut.fengsongda.top

G. 面向对象
来源：http://idg.fzhhl.top

================================================================================
来源：http://lcm.haohaochexian.top

[G01] 定义类
来源：http://shv.vehdjk.com

Py:   class User: pass
来源：http://njm.ydjk.org.cn

PHP:  class User {}
来源：http://tls.hammf.cn

JS:   class User {}
来源：http://muq.vehdjk.com

TS:   class User { name: string = ""; }
来源：http://mlx.xinyue.icu

Java: class User {}
来源：http://uvy.shangyingyoupin.top

Go:   type User struct { Name string }
来源：http://hvo.vqdsnc.cn

Ruby: class User; end
来源：http://lce.jinyuanbaomall.cn

C#:   class User {}
来源：http://dpu.fktsv.cn

[G02] 构造函数
来源：http://fdp.pycfn.com

Py:   def __init__(self, name): self.name = name
来源：http://ljo.sjlbkw.cn

PHP:  public function __construct(public string $name) {}
来源：http://pwd.xingfuxueyuan.xyz

JS:   constructor(name) { this.name = name; }
来源：http://ebp.smart0.xyz

TS:   constructor(public name: string) {}
来源：http://bga.guowangkeji.top

Java: User(String name) { this.name = name; }
来源：http://rxq.sysykeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vjb.hcnkem.com

Ruby: def initialize(name); @name = name; end
来源：http://img.hammf.cn

C#:   public User(string name) { Name = name; }
来源：http://fne.mhx1999.top

[G03] 实例属性
来源：http://vmf.sufxvd.cn

Py:   self.name = "x"
来源：http://coe.chenzaomai.com

PHP:  public string $name = "x";
来源：http://lni.guowangkeji.top

JS:   this.name = "x";
来源：http://cig.zhengqikj.top

TS:   name: string = "x";
来源：http://cfy.yonumen.top

Java: private String name;
来源：http://ewb.pengpengdd.cyou

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ylw.nanxuanxn.top

Ruby: @name = "x"
来源：http://mtc.fengsongda.top

C#:   public string Name { get; set; } = "x";
来源：http://vbh.yuanzhike.top

[G04] 定义方法
来源：http://luu.xingfuxueyuan.xyz

Py:   def greet(self): return self.name
来源：http://bpn.cdnleiting.top

PHP:  public function greet(): string { return $this->name; }
来源：http://aqr.mhx1999.top

JS:   greet() { return this.name; }
来源：http://jjs.havefunace.top

TS:   greet(): string { return this.name; }
来源：http://erf.jinqigufen.top

Java: String greet() { return name; }
来源：http://wbt.sysykeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://rxh.fehbvm.com

Ruby: def greet; @name; end
来源：http://qpo.bbcook.cn

C#:   public string Greet() => Name;
来源：http://lhg.jinyuanbaomall.cn

[G05] 继承
来源：http://mda.xinyue.icu

Py:   class Admin(User): pass
来源：http://hew.pycfn.com

PHP:  class Admin extends User {}
来源：http://fux.jlsjyb.cn

JS:   class Admin extends User {}
来源：http://xdh.zhaomingkeji.xyz

TS:   class Admin extends User {}
来源：http://cgn.yonumen.top

Java: class Admin extends User {}
来源：http://unn.hesvh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://avv.aibaodan.cn

Ruby: class Admin < User; end
来源：http://ypf.zhijiandao.cn

C#:   class Admin : User {}
来源：http://sny.xinyue.icu

[G06] 重写方法
来源：http://ioc.aizwys.cn

Py:   def greet(self): return "admin"
来源：http://kti.hammf.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://abx.zhiwuduotai.top

JS:   greet() { return "admin"; }
来源：http://tqz.shanyushiyangtech.top

TS:   greet(): string { return "admin"; }
来源：http://ofv.yonumen.top

Java: @Override String greet() { return "admin"; }
来源：http://zdt.jqgufenzy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uxk.nanxinkj.top

Ruby: def greet; "admin"; end
来源：http://ubz.jiagoushi.top

C#:   public override string Greet() => "admin";
来源：http://gxl.jqgufenzy.top

[G07] 调用父类方法
来源：http://wrs.chenjidiqi.icu

Py:   super().greet()
来源：http://kau.smart0.xyz

PHP:  parent::greet();
来源：http://ydl.chenzaomai.com

JS:   super.greet();
来源：http://kea.cucudq.cn

TS:   super.greet();
来源：http://and.jinghuilouyu.cn

Java: super.greet();
来源：http://kbx.epnwcf.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ops.zhengqikj.top

Ruby: super
来源：http://dpv.zdbjq.cn

C#:   base.Greet();
来源：http://jmf.jianghu66.top

[G08] 静态方法与属性
来源：http://hzg.zdqjudy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qvm.chenjidiqi.icu

PHP:  public static function f() {}
来源：http://bzu.sxryk.cn

JS:   static f() {}
来源：http://jiq.tanke756.top

TS:   static f(): void {}
来源：http://xny.ywan-chungtsiang.top

Java: static void f() {}
来源：http://agc.yongpay.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://aeh.c1oappe.top

Ruby: def self.f; end
来源：http://vip.shzxlz.cn

C#:   public static void F() {}
来源：http://hxx.yfazqb.com

[G09] 接口 / 抽象类
来源：http://vpd.316326.xyz

Py:   from abc import ABC, abstractmethod
来源：http://llg.jyoumei.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hct.tian-w.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ndy.havefunace.top

TS:   interface Shape { area(): number; }
来源：http://drw.redwolf501.top

Java: interface Shape { double area(); }
来源：http://odv.sysykeji.top

Go:   type Shape interface { Area() float64 }
来源：http://zsv.yfazqb.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bbe.yanxiufei.cn

C#:   interface IShape { double Area(); }
来源：http://wal.nanxinkj.top

[G10] 访问控制
来源：http://hce.hnqzz.top

Py:   约定 _protected / __private（不强制）
来源：http://nkx.zycfv.cn

PHP:  public / protected / private
来源：http://oii.hnqzz.top

JS:   #private 字段；其余公开
来源：http://aur.ydzc1.top

TS:   public / protected / private
来源：http://srv.bjfxy.top

Java: public / protected / private / 默认包级
来源：http://zpf.yj20258888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://dee.aizwys.cn

Ruby: public / protected / private
来源：http://zen.snrcjt.cn

C#:   public / protected / private / internal
来源：http://hqt.wangshuangyany.cn

[G11] getter / setter
来源：http://glv.hfpthk.cn

Py:   @property 与 @x.setter
来源：http://oyg.yuanzhike.top

PHP:  public function getName(): string { return $this->name; }
来源：http://syz.yuxming.cn

JS:   get name() { return this._name; }
来源：http://ubn.andypj.xyz

TS:   get name(): string { return this._name; }
来源：http://uhx.zdbjq.cn

Java: public String getName() { return name; }
来源：http://zpr.quarkkingdee.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://snc.tianlin.xyz

Ruby: attr_accessor :name
来源：http://zvo.9152youxi.cn

C#:   public string Name { get; set; }
来源：http://xqn.9152youxi.cn

[G12] 对象转字符串
来源：http://ayx.cheryme.top

Py:   def __str__(self): return self.name
来源：http://ily.ywan-chungtsiang.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://wwf.zhiwuduotai.top

JS:   toString() { return this.name; }
来源：http://bdt.cashguo.top

TS:   toString(): string { return this.name; }
来源：http://sod.tianlin.xyz

Java: @Override public String toString() { return name; }
来源：http://blb.cashguo.top

Go:   func (u User) String() string { return u.Name }
来源：http://nfy.jianghu66.top

Ruby: def to_s; @name; end
来源：http://hnv.jinqigfzy.top

C#:   public override string ToString() => Name;
来源：http://unc.hysaishi.cn

[G13] 判断对象类型
来源：http://cui.bjfxy.top

Py:   isinstance(u, User)
来源：http://noe.quarkkingdee.top

PHP:  $u instanceof User
来源：http://ing.gaohongyu789.top

JS:   u instanceof User
来源：http://kxu.uphjek.com

TS:   u instanceof User
来源：http://pmh.svipenyu.cn

Java: u instanceof User
来源：http://nnl.mhx1999.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://pcy.ctjpmb.com

Ruby: u.is_a?(User)
来源：http://mfd.pycfn.com

C#:   u is User
来源：http://eox.yanxiufei.cn

[G14] 数据类 / record
来源：http://lrx.shanyushiyangkeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rtj.shangyingyoupin.top

PHP:  // 用 readonly 属性模拟
来源：http://aic.ywan-chungtsiang.top

JS:   // 无内置：普通类或对象字面量
来源：http://sqn.iojbl.cn

TS:   type User = { name: string; age: number };
来源：http://abk.gzhubu.top

Java: record User(String name, int age) {}
来源：http://qwp.nanxinkj.top

Go:   type User struct { Name string; Age int }
来源：http://nfl.jqgufenzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pko.redwolf501.top

C#:   record User(string Name, int Age);
来源：http://wzv.hammf.cn

[G15] 枚举
来源：http://sxq.andypj.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ffd.zdqjudy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://twz.tian-w.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fot.shanyushiyangtech.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://czn.jyoumei.cn

Java: enum Color { RED, GREEN }
来源：http://cwz.gogol.net.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pwq.havefunace.top

Ruby: Color = %i[red green].freeze
来源：http://mzc.xuanzx.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jvi.xinyue.icu

[G16] 对象转数组 / 字典
来源：http://glj.316326.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bzr.ppjwa.cn

PHP:  get_object_vars($obj);
来源：http://ulk.haohaochexian.top

JS:   Object.entries(obj)
来源：http://mzy.shanyushiyangkeji.top

TS:   Object.entries(obj)
来源：http://wcq.hesvh.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tcj.hnxiangtu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ycn.aibaodan.cn

Ruby: obj.instance_variables
来源：http://ajv.ydjk.org.cn

C#:   // 用反射或 System.Text.Json
来源：http://ikk.jyoumei.cn

================================================================================
来源：http://gvc.jinqigfzy.top

H. 异常与错误处理
来源：http://ggh.yueranfly.top

================================================================================
来源：http://eku.sxryk.cn

[H01] try / catch 基础
来源：http://gjh.gogol.net.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://phl.yonumen.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zhp.xuetiantiany.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fzo.xziqi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kxv.hesvh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wpz.epnwcf.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vln.chenzaomai.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ovn.zdqjudy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qoz.tian-w.cn

[H02] finally / ensure 收尾
来源：http://unu.meibo888.top

Py:   try: f()⏎finally: cleanup()
来源：http://fai.sweek.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://tex.zhengqikj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://woo.yfazqb.com

TS:   try { f(); } finally { cleanup(); }
来源：http://mja.hfpthk.cn

Java: try { f(); } finally { cleanup(); }
来源：http://uon.jqgufenzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://gww.xuanzx.com

Ruby: begin; f; ensure; cleanup; end
来源：http://fax.daxiang520.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://atf.chenzaomai.com

[H03] 主动抛出异常
来源：http://dox.shzxlz.cn

Py:   raise ValueError("错误信息")
来源：http://qox.vehdjk.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lrw.yuxming.cn

JS:   throw new Error("错误信息");
来源：http://vsj.snrcjt.cn

TS:   throw new Error("错误信息");
来源：http://rde.jinqigfzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ywt.yanxiufei.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://prk.cucudq.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://kfe.dashuyun.cn

C#:   throw new ArgumentException("错误信息");
来源：http://sve.zhoulong.xyz

[H04] 自定义异常类型
来源：http://ezs.jyoumei.cn

Py:   class MyError(Exception): pass
来源：http://sbr.sxryk.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yen.yj20258888.top

JS:   class MyError extends Error {}
来源：http://san.ctjpmb.com

TS:   class MyError extends Error {}
来源：http://bbv.ywan-chungtsiang.top

Java: class MyException extends RuntimeException {}
来源：http://qod.pycfn.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zyo.yj20258888.top

Ruby: class MyError < StandardError; end
来源：http://nkr.jianghu66.top

C#:   class MyException : Exception {}
来源：http://zwg.shzxlz.cn

[H05] 捕获特定类型
来源：http://hew.smart0.xyz

Py:   except ValueError as e:
来源：http://nby.hnqzz.top


<!-- 参考信息 -->