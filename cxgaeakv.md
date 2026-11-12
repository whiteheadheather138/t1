代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vyt.xinyue.icu

================================================================================
来源：http://mon.hcnkem.com

F. 文件与目录
来源：http://wwx.quarkkingdee.top

================================================================================
来源：http://ebk.shuidangran.top

[F01] 读取整个文件
来源：http://hsf.hywenlv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nnu.xziqi.cn

PHP:  file_get_contents("a.txt");
来源：http://ddv.shzxlz.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xrf.guowangkeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hje.cashguo.top

Java: Files.readString(Path.of("a.txt"))
来源：http://uqf.zhengqikj.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://izg.jyoumei.cn

Ruby: File.read("a.txt")
来源：http://icq.dashuyun.cn

C#:   File.ReadAllText("a.txt");
来源：http://kds.tian-w.cn

[F02] 逐行读取文件
来源：http://rms.cashguo.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cin.ppjwa.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pcu.shanyushiyangtech.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wmg.nanxinkj.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gzd.jlsjyb.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lrs.jinqigufen.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oot.jinyuanbaomall.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hzh.xuanzx.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://voe.yj20258888.top

[F03] 写入文件（覆盖）
来源：http://rza.haohaochexian.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dcx.bbcook.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://egu.ctjpmb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dxe.aizwys.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tnp.guannengcc.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qgj.snrcjt.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gdd.zhiwuduotai.top

Ruby: File.write("a.txt", "hi")
来源：http://ysq.ybcxt.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cef.c1oappe.top

[F04] 追加写入文件
来源：http://htr.yanxiufei.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://udt.snrcjt.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ocu.yj20258.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ylo.tian-w.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gji.aizwys.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iwu.jinqigufen.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jlh.fktsv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rit.smart0.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fcr.zycfv.cn

[F05] 判断文件或目录是否存在
来源：http://mzm.hcnkem.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kyl.zhongyouzk.top

PHP:  file_exists("a.txt");
来源：http://tjd.redwolf501.top

JS:   fs.existsSync("a.txt")
来源：http://kuu.ywan-chungtsiang.top

TS:   fs.existsSync("a.txt")
来源：http://mxv.ywan-chungtsiang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ckt.sxryk.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yyy.52xcode.cn

Ruby: File.exist?("a.txt")
来源：http://xbg.yonumen.top

C#:   File.Exists("a.txt")
来源：http://pey.yfazqb.com

[F06] 删除文件
来源：http://opk.dashuyun.cn

Py:   os.remove("a.txt")
来源：http://cvy.sweek.top

PHP:  unlink("a.txt");
来源：http://voc.ehwqpu.com

JS:   fs.unlinkSync("a.txt")
来源：http://zwi.zycfv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dsm.zhoulong.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xsh.redwolf501.top

Go:   os.Remove("a.txt")
来源：http://tys.uphjek.com

Ruby: File.delete("a.txt")
来源：http://hnh.hywenlv.cn

C#:   File.Delete("a.txt");
来源：http://cei.zdqjudy.top

[F07] 创建目录（含多级）
来源：http://qdr.wangshuangyany.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vzw.chenzaomai.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fmw.zdqjudy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vic.sysykeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nmj.yuanzhike.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ckt.fehbvm.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://icl.zdbjq.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ufa.guowangkeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://saw.shanyushiyangkeji.top

[F08] 遍历目录
来源：http://hvc.daria6918.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ejm.hfpthk.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nmt.fktsv.cn

JS:   fs.readdirSync("dir")
来源：http://xmj.yuxming.cn

TS:   fs.readdirSync("dir")
来源：http://mol.nanxinkj.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xnn.wangshuangyany.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zso.jinghuilouyu.cn

Ruby: Dir.children("dir")
来源：http://dst.jinqigfzy.top

C#:   Directory.GetFiles("dir")
来源：http://sys.yj20258.top

[F09] 获取文件大小
来源：http://mdr.chenzaomai.com

Py:   os.path.getsize("a.txt")
来源：http://jpb.sufxvd.cn

PHP:  filesize("a.txt");
来源：http://sfg.zhongyouzk.top

JS:   fs.statSync("a.txt").size
来源：http://ywg.gogol.net.cn

TS:   fs.statSync("a.txt").size
来源：http://cwv.xuetiantiany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ucd.birdmap.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://suu.kuanghao11.cn

Ruby: File.size("a.txt")
来源：http://nws.gaohongyu789.top

C#:   new FileInfo("a.txt").Length
来源：http://tri.hesvh.cn

[F10] 取文件扩展名 / 文件名
来源：http://mcr.dianchejie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tga.jqgufenzy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://foh.jinyuanbaomall.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bil.gzhubu.top

TS:   path.extname("a.txt")
来源：http://zww.aizwys.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vur.cheryme.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://opt.zhongyouzk.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vez.jinghuilouyu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xzq.9152youxi.cn

[F11] 复制与移动文件
来源：http://pfo.chenjidiqi.icu

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vyn.yuxming.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ows.shangyingyoupin.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ris.tarul.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mez.bbcook.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://irg.bjfxy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://djt.dianchejie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dyu.birdmap.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ynk.zdqjudy.top

[F12] CSV 读写
来源：http://rcp.feifeiyinyue.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lcg.sjlbkw.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tke.smart0.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nfq.mhx1999.top

TS:   // 同上
来源：http://fmi.guannengcc.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fgn.wangdashe.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://edm.xziqi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pvv.fehbvm.com

C#:   // 无内置：用 CsvHelper 库
来源：http://spe.jianghu66.top

================================================================================
来源：http://ibx.gzhubu.top

G. 面向对象
来源：http://kgi.guowangkeji.top

================================================================================
来源：http://sgh.hammf.cn

[G01] 定义类
来源：http://egc.zhongyouzk.top

Py:   class User: pass
来源：http://kmk.jinghuilouyu.cn

PHP:  class User {}
来源：http://ggo.tarul.cn

JS:   class User {}
来源：http://nfd.jqgufenzy.top

TS:   class User { name: string = ""; }
来源：http://ppz.cqqwz.cn

Java: class User {}
来源：http://ehc.dashuyun.cn

Go:   type User struct { Name string }
来源：http://hqb.zhijiandao.cn

Ruby: class User; end
来源：http://uah.zhijiandao.cn

C#:   class User {}
来源：http://vmd.sweek.top

[G02] 构造函数
来源：http://upx.mhx1999.top

Py:   def __init__(self, name): self.name = name
来源：http://cyv.fktsv.cn

PHP:  public function __construct(public string $name) {}
来源：http://vgr.zdbjq.cn

JS:   constructor(name) { this.name = name; }
来源：http://ydy.jqgfzy.top

TS:   constructor(public name: string) {}
来源：http://oax.nanxinkj.top

Java: User(String name) { this.name = name; }
来源：http://nwg.epnwcf.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ola.yongpay.top

Ruby: def initialize(name); @name = name; end
来源：http://ewc.sufxvd.cn

C#:   public User(string name) { Name = name; }
来源：http://cpu.hysaishi.cn

[G03] 实例属性
来源：http://acw.dashuyun.cn

Py:   self.name = "x"
来源：http://wel.aizwys.cn

PHP:  public string $name = "x";
来源：http://vph.yuanzhike.top

JS:   this.name = "x";
来源：http://foc.c1oappe.top

TS:   name: string = "x";
来源：http://vvg.epnwcf.com

Java: private String name;
来源：http://vfe.tianlin.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tah.zdbjq.cn

Ruby: @name = "x"
来源：http://lau.jianghu66.top

C#:   public string Name { get; set; } = "x";
来源：http://bab.yonumen.top

[G04] 定义方法
来源：http://kgv.meibo888.top

Py:   def greet(self): return self.name
来源：http://zbt.fehbvm.com

PHP:  public function greet(): string { return $this->name; }
来源：http://szf.c1oappe.top

JS:   greet() { return this.name; }
来源：http://dqb.zhoulong.xyz

TS:   greet(): string { return this.name; }
来源：http://liz.xziqi.cn

Java: String greet() { return name; }
来源：http://rmd.ppjwa.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://axn.jinqigfzy.top

Ruby: def greet; @name; end
来源：http://kul.jianghu66.top

C#:   public string Greet() => Name;
来源：http://qcx.jinqigfzy.top

[G05] 继承
来源：http://loc.wangshuangyany.cn

Py:   class Admin(User): pass
来源：http://zal.vehdjk.com

PHP:  class Admin extends User {}
来源：http://yxa.xziqi.cn

JS:   class Admin extends User {}
来源：http://stg.kuanghao11.cn

TS:   class Admin extends User {}
来源：http://lmu.bjfxy.top

Java: class Admin extends User {}
来源：http://ydu.yfazqb.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wnd.zhixingplan.top

Ruby: class Admin < User; end
来源：http://nyt.nwbrower.top

C#:   class Admin : User {}
来源：http://chg.chenjidiqi.icu

[G06] 重写方法
来源：http://ifv.yongpay.top

Py:   def greet(self): return "admin"
来源：http://szl.zhoulong.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://krt.meibo888.top

JS:   greet() { return "admin"; }
来源：http://dgf.pycfn.com

TS:   greet(): string { return "admin"; }
来源：http://tqq.jinghuilouyu.cn

Java: @Override String greet() { return "admin"; }
来源：http://vbl.yj202588.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uvt.mhx1999.top

Ruby: def greet; "admin"; end
来源：http://bad.jiagoushi.top

C#:   public override string Greet() => "admin";
来源：http://ohm.cdnleiting.top

[G07] 调用父类方法
来源：http://bhw.shuidangran.top

Py:   super().greet()
来源：http://pwz.iojbl.cn

PHP:  parent::greet();
来源：http://psi.fehbvm.com

JS:   super.greet();
来源：http://vip.9152youxi.cn

TS:   super.greet();
来源：http://kvy.ywan-chungtsiang.top

Java: super.greet();
来源：http://oyu.redwolf501.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://law.wangshuangyany.cn

Ruby: super
来源：http://qio.dianchejie.cn

C#:   base.Greet();
来源：http://pmh.xinyue.icu

[G08] 静态方法与属性
来源：http://pin.sjlbkw.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://koc.hnxiangtu.top

PHP:  public static function f() {}
来源：http://zch.yj20258888.top

JS:   static f() {}
来源：http://uxy.sxryk.cn

TS:   static f(): void {}
来源：http://ilo.jyoumei.cn

Java: static void f() {}
来源：http://xjg.sysykeji.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://uuj.xuetiantiany.cn

Ruby: def self.f; end
来源：http://ygh.xuetiantiany.cn

C#:   public static void F() {}
来源：http://vsm.chenzaomai.com

[G09] 接口 / 抽象类
来源：http://qbz.birdmap.top

Py:   from abc import ABC, abstractmethod
来源：http://cwv.iojbl.cn

PHP:  interface Shape { public function area(): float; }
来源：http://eul.yj20258.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://djf.chenjidiqi.icu

TS:   interface Shape { area(): number; }
来源：http://kyt.meibo888.top

Java: interface Shape { double area(); }
来源：http://zky.chenzaomai.com

Go:   type Shape interface { Area() float64 }
来源：http://odx.tarul.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hof.yuanzhike.top

C#:   interface IShape { double Area(); }
来源：http://hmf.gogol.net.cn

[G10] 访问控制
来源：http://jtx.redwolf501.top

Py:   约定 _protected / __private（不强制）
来源：http://gxf.jinqigufen.top

PHP:  public / protected / private
来源：http://blm.jinyuanbaomall.cn

JS:   #private 字段；其余公开
来源：http://msn.nanxinkj.top

TS:   public / protected / private
来源：http://ygm.52xcode.cn

Java: public / protected / private / 默认包级
来源：http://yur.yfazqb.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://dfw.vehdjk.com

Ruby: public / protected / private
来源：http://xbi.dashuyun.cn

C#:   public / protected / private / internal
来源：http://umf.ivvv.top

[G11] getter / setter
来源：http://dxd.yangfankeji.com

Py:   @property 与 @x.setter
来源：http://brq.fehbvm.com

PHP:  public function getName(): string { return $this->name; }
来源：http://bwi.nanxinkj.top

JS:   get name() { return this._name; }
来源：http://vba.hysaishi.cn

TS:   get name(): string { return this._name; }
来源：http://zcs.xziqi.cn

Java: public String getName() { return name; }
来源：http://blu.hnqzz.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://uft.316326.xyz

Ruby: attr_accessor :name
来源：http://kgb.haohaochexian.top

C#:   public string Name { get; set; }
来源：http://ynn.zhixingplan.top

[G12] 对象转字符串
来源：http://pxk.kuanghao11.cn

Py:   def __str__(self): return self.name
来源：http://xzl.vehdjk.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://ees.shanyushiyangtech.top

JS:   toString() { return this.name; }
来源：http://hmv.guowangkeji.top

TS:   toString(): string { return this.name; }
来源：http://zho.shuidangran.top

Java: @Override public String toString() { return name; }
来源：http://heq.ehwqpu.com

Go:   func (u User) String() string { return u.Name }
来源：http://elh.xuanzx.com

Ruby: def to_s; @name; end
来源：http://kgs.bjfxy.top

C#:   public override string ToString() => Name;
来源：http://bza.chenlongwang.top

[G13] 判断对象类型
来源：http://yle.c1oappe.top

Py:   isinstance(u, User)
来源：http://awq.cashguo.top

PHP:  $u instanceof User
来源：http://ufl.pycfn.com

JS:   u instanceof User
来源：http://oqo.cqqwz.cn

TS:   u instanceof User
来源：http://mfo.xuanzx.com

Java: u instanceof User
来源：http://lkt.iojbl.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ayo.zhengqikj.top

Ruby: u.is_a?(User)
来源：http://ryc.0kj1m.cn

C#:   u is User
来源：http://ion.yvedp.cn

[G14] 数据类 / record
来源：http://nsi.zhiwuduotai.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://oxo.aibaodan.cn

PHP:  // 用 readonly 属性模拟
来源：http://htl.mhx1999.top

JS:   // 无内置：普通类或对象字面量
来源：http://ghb.chenlongwang.top

TS:   type User = { name: string; age: number };
来源：http://frb.sxryk.cn

Java: record User(String name, int age) {}
来源：http://emu.shanyushiyangtech.top

Go:   type User struct { Name string; Age int }
来源：http://jes.meibo888.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://twg.xuetiantiany.cn

C#:   record User(string Name, int Age);
来源：http://uzs.sufxvd.cn

[G15] 枚举
来源：http://jne.birdmap.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pez.chenjidiqi.icu

PHP:  enum Color: string { case Red = "red"; }
来源：http://tux.smart0.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wsa.ydjk.org.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://onm.hywenlv.cn

Java: enum Color { RED, GREEN }
来源：http://ugo.cucudq.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://soa.yanxiufei.cn

Ruby: Color = %i[red green].freeze
来源：http://jtt.xuetiantiany.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://efu.ctjpmb.com

[G16] 对象转数组 / 字典
来源：http://taw.jqgufenzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pod.yuanzhike.top

PHP:  get_object_vars($obj);
来源：http://oxe.yanxiufei.cn

JS:   Object.entries(obj)
来源：http://lnt.yvedp.cn

TS:   Object.entries(obj)
来源：http://hwc.cashguo.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://taa.zdbjq.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mli.zhoulong.xyz

Ruby: obj.instance_variables
来源：http://pge.hnxiangtu.top

C#:   // 用反射或 System.Text.Json
来源：http://cym.feifeiyinyue.top

================================================================================
来源：http://hfd.xziqi.cn

H. 异常与错误处理
来源：http://pju.yj20258888.top

================================================================================
来源：http://cec.andypj.xyz

[H01] try / catch 基础
来源：http://mvt.svipenyu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pjh.sysykeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jez.vqdsnc.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hbf.xinyue.icu

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qcr.zhengqikj.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://adh.jyoumei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mug.chenzaomai.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://igf.snrcjt.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ooj.52xcode.cn

[H02] finally / ensure 收尾
来源：http://mpc.shanyushiyangtech.top

Py:   try: f()⏎finally: cleanup()
来源：http://ghc.fengsongda.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://fro.dianchejie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://kxm.fengsongda.top

TS:   try { f(); } finally { cleanup(); }
来源：http://zjf.yonumen.top

Java: try { f(); } finally { cleanup(); }
来源：http://qlx.quarkkingdee.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://hqc.meibo888.top

Ruby: begin; f; ensure; cleanup; end
来源：http://pvk.fzhhl.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ojp.hcnkem.com

[H03] 主动抛出异常
来源：http://iet.fengsongda.top

Py:   raise ValueError("错误信息")
来源：http://exr.yj202588.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bkk.yj20258.top

JS:   throw new Error("错误信息");
来源：http://nar.vqdsnc.cn

TS:   throw new Error("错误信息");
来源：http://dhd.ywan-chungtsiang.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://edb.cheryme.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://obn.0kj1m.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ryk.gaohongyu789.top

C#:   throw new ArgumentException("错误信息");
来源：http://ldt.zycfv.cn

[H04] 自定义异常类型
来源：http://vyq.yvedp.cn

Py:   class MyError(Exception): pass
来源：http://atp.hnxiangtu.top

PHP:  class MyError extends RuntimeException {}
来源：http://ctr.sjlbkw.cn

JS:   class MyError extends Error {}
来源：http://rya.guowangkeji.top

TS:   class MyError extends Error {}
来源：http://ymx.hammf.cn

Java: class MyException extends RuntimeException {}
来源：http://agp.jinqigufen.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xyn.yj202588.top

Ruby: class MyError < StandardError; end
来源：http://apg.jinyuanbaomall.cn

C#:   class MyException : Exception {}
来源：http://srn.jiagoushi.top

[H05] 捕获特定类型
来源：http://vxv.zycfv.cn

Py:   except ValueError as e:
来源：http://woq.zdbjq.cn


<!-- 参考信息 -->