代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gzs.fehbvm.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bgn.zhijiandao.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gxx.gotoacloud.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fbw.zhiwuduotai.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uuo.ppjwa.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ywy.jqgfzy.top

[F03] 写入文件（覆盖）
来源：http://kmr.pengpengdd.cyou

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://psp.tianlin.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://ivf.hcnkem.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://orp.hesvh.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hdl.hfpthk.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nxu.yanxiufei.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://snp.cashguo.top

Ruby: File.write("a.txt", "hi")
来源：http://vru.xuanzx.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uwy.snrcjt.cn

[F04] 追加写入文件
来源：http://ifl.nanxinkj.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://iuj.guannengcc.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cqw.sxryk.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uji.dashuyun.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://env.bbcook.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bif.xuanzx.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sog.wangdashe.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hig.haohaochexian.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vml.guannengcc.top

[F05] 判断文件或目录是否存在
来源：http://zsr.ctjpmb.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mtx.fehbvm.com

PHP:  file_exists("a.txt");
来源：http://rez.xinyue.icu

JS:   fs.existsSync("a.txt")
来源：http://typ.ppjwa.cn

TS:   fs.existsSync("a.txt")
来源：http://hhq.daria6918.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gty.yangfankeji.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://brg.jiagoushi.top

Ruby: File.exist?("a.txt")
来源：http://xeb.yonumen.top

C#:   File.Exists("a.txt")
来源：http://oyv.fanxiaobao.xyz

[F06] 删除文件
来源：http://hdx.jyoumei.cn

Py:   os.remove("a.txt")
来源：http://lye.epnwcf.com

PHP:  unlink("a.txt");
来源：http://vxy.haohaochexian.top

JS:   fs.unlinkSync("a.txt")
来源：http://qwp.yuxming.cn

TS:   fs.unlinkSync("a.txt")
来源：http://aob.hongshengwenyu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mer.yongpay.top

Go:   os.Remove("a.txt")
来源：http://vsr.jyoumei.cn

Ruby: File.delete("a.txt")
来源：http://ran.chenjidiqi.icu

C#:   File.Delete("a.txt");
来源：http://blk.fanxiaobao.xyz

[F07] 创建目录（含多级）
来源：http://zvr.sysykeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dbu.snrcjt.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://muw.xinyue.icu

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aeb.9152youxi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pzl.zdqjudy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qtg.shzxlz.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qmu.jqgufenzy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://doi.cucudq.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jjy.epnwcf.com

[F08] 遍历目录
来源：http://ayp.zdbjq.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://thl.yongpay.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hoe.pengpengdd.cyou

JS:   fs.readdirSync("dir")
来源：http://evv.ehwqpu.com

TS:   fs.readdirSync("dir")
来源：http://fpt.zhiwuduotai.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tnt.sysykeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ysq.shuidangran.top

Ruby: Dir.children("dir")
来源：http://qga.sweek.top

C#:   Directory.GetFiles("dir")
来源：http://lly.sjlbkw.cn

[F09] 获取文件大小
来源：http://pnp.0kj1m.cn

Py:   os.path.getsize("a.txt")
来源：http://ihz.aibaodan.cn

PHP:  filesize("a.txt");
来源：http://dyd.zhixingplan.top

JS:   fs.statSync("a.txt").size
来源：http://wua.yuanzhike.top

TS:   fs.statSync("a.txt").size
来源：http://pvm.dashuyun.cn

Java: Files.size(Path.of("a.txt"))
来源：http://znu.nwbrower.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vxl.jinyuanbaomall.cn

Ruby: File.size("a.txt")
来源：http://lvt.yuanzhike.top

C#:   new FileInfo("a.txt").Length
来源：http://vsk.cucudq.cn

[F10] 取文件扩展名 / 文件名
来源：http://bdz.jiagoushi.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uqo.zhixingplan.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wfv.aibaodan.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mrx.nanxuanxn.top

TS:   path.extname("a.txt")
来源：http://efq.shuidangran.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tic.gotoacloud.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kfa.sysykeji.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wrg.vqdsnc.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yvo.dianchejie.cn

[F11] 复制与移动文件
来源：http://yxv.fengsongda.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wlk.epnwcf.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rgn.tianlin.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mus.birdmap.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kmz.epnwcf.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xqc.fanxiaobao.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vva.bbcook.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mdz.iojbl.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sae.hongshengwenyu.top

[F12] CSV 读写
来源：http://pfc.shzxlz.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kif.chenzaomai.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vam.xinyue.icu

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lao.yj202588.top

TS:   // 同上
来源：http://ffx.hnqzz.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hir.shanyushiyangtech.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wbe.jinyuanbaomall.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cxz.shanyushiyangkeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://wxr.xziqi.cn

================================================================================
来源：http://asg.jqgufenzy.top

G. 面向对象
来源：http://ayw.wangshuangyany.cn

================================================================================
来源：http://mbc.dashuyun.cn

[G01] 定义类
来源：http://kch.sufxvd.cn

Py:   class User: pass
来源：http://cqc.zhijiandao.cn

PHP:  class User {}
来源：http://plf.xinyue.icu

JS:   class User {}
来源：http://jhu.ctjpmb.com

TS:   class User { name: string = ""; }
来源：http://ieq.yj20258888.top

Java: class User {}
来源：http://lwi.andypj.xyz

Go:   type User struct { Name string }
来源：http://yrn.jyoumei.cn

Ruby: class User; end
来源：http://wnm.jqgufenzy.top

C#:   class User {}
来源：http://nbc.fanxiaobao.xyz

[G02] 构造函数
来源：http://agj.yvedp.cn

Py:   def __init__(self, name): self.name = name
来源：http://bve.svipenyu.cn

PHP:  public function __construct(public string $name) {}
来源：http://xaw.ivvv.top

JS:   constructor(name) { this.name = name; }
来源：http://thm.sysykeji.top

TS:   constructor(public name: string) {}
来源：http://sii.iojbl.cn

Java: User(String name) { this.name = name; }
来源：http://ory.jqgfzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sxu.yfazqb.com

Ruby: def initialize(name); @name = name; end
来源：http://ayr.hammf.cn

C#:   public User(string name) { Name = name; }
来源：http://poz.316326.xyz

[G03] 实例属性
来源：http://esr.hysaishi.cn

Py:   self.name = "x"
来源：http://des.kuanghao11.cn

PHP:  public string $name = "x";
来源：http://dmy.jiagoushi.top

JS:   this.name = "x";
来源：http://ros.316326.xyz

TS:   name: string = "x";
来源：http://ehn.jyoumei.cn

Java: private String name;
来源：http://znk.gaohongyu789.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ens.chenzaomai.com

Ruby: @name = "x"
来源：http://tjq.ppjwa.cn

C#:   public string Name { get; set; } = "x";
来源：http://bml.ivvv.top

[G04] 定义方法
来源：http://nzo.daxiang520.top

Py:   def greet(self): return self.name
来源：http://cdr.yvedp.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://eeq.cheryme.top

JS:   greet() { return this.name; }
来源：http://cer.zycfv.cn

TS:   greet(): string { return this.name; }
来源：http://wlx.zdbjq.cn

Java: String greet() { return name; }
来源：http://mpr.hcnkem.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://fhg.xuetiantiany.cn

Ruby: def greet; @name; end
来源：http://xss.svipenyu.cn

C#:   public string Greet() => Name;
来源：http://uko.nwbrower.top

[G05] 继承
来源：http://ybj.guowangkeji.top

Py:   class Admin(User): pass
来源：http://ayg.shanyushiyangkeji.top

PHP:  class Admin extends User {}
来源：http://tgc.zhongyouzk.top

JS:   class Admin extends User {}
来源：http://jom.birdmap.top

TS:   class Admin extends User {}
来源：http://ezo.hcnkem.com

Java: class Admin extends User {}
来源：http://bmd.tianlin.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wqa.jlsjyb.cn

Ruby: class Admin < User; end
来源：http://rqw.vqdsnc.cn

C#:   class Admin : User {}
来源：http://wdm.zhengqikj.top

[G06] 重写方法
来源：http://kww.xingfuxueyuan.xyz

Py:   def greet(self): return "admin"
来源：http://cvy.fengsongda.top

PHP:  public function greet(): string { return "admin"; }
来源：http://phg.jinyuanbaomall.cn

JS:   greet() { return "admin"; }
来源：http://aep.tarul.cn

TS:   greet(): string { return "admin"; }
来源：http://fmz.tianlin.xyz

Java: @Override String greet() { return "admin"; }
来源：http://ojl.aizwys.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pjd.epnwcf.com

Ruby: def greet; "admin"; end
来源：http://xrw.snrcjt.cn

C#:   public override string Greet() => "admin";
来源：http://cun.aibaodan.cn

[G07] 调用父类方法
来源：http://xqf.nanxinkj.top

Py:   super().greet()
来源：http://zwj.haohaochexian.top

PHP:  parent::greet();
来源：http://ezh.hnqzz.top

JS:   super.greet();
来源：http://wjo.zdbjq.cn

TS:   super.greet();
来源：http://ilm.smart0.xyz

Java: super.greet();
来源：http://uqc.jianghu66.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tgp.chenzaomai.com

Ruby: super
来源：http://zmp.bbcook.cn

C#:   base.Greet();
来源：http://aid.chenzaomai.com

[G08] 静态方法与属性
来源：http://boy.yonumen.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qas.sysykeji.top

PHP:  public static function f() {}
来源：http://vzv.fengsongda.top

JS:   static f() {}
来源：http://vql.fktsv.cn

TS:   static f(): void {}
来源：http://wsa.zhoulong.xyz

Java: static void f() {}
来源：http://jrd.cucudq.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xac.zdqjudy.top

Ruby: def self.f; end
来源：http://pch.jinyuanbaomall.cn

C#:   public static void F() {}
来源：http://qwz.gaohongyu789.top

[G09] 接口 / 抽象类
来源：http://pkb.yuanzhike.top

Py:   from abc import ABC, abstractmethod
来源：http://cgp.cqqwz.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hyt.jinghuilouyu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rib.nwbrower.top

TS:   interface Shape { area(): number; }
来源：http://blo.gaohongyu789.top

Java: interface Shape { double area(); }
来源：http://adu.yanxiufei.cn

Go:   type Shape interface { Area() float64 }
来源：http://ngh.zhaomingkeji.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://btv.jqgfzy.top

C#:   interface IShape { double Area(); }
来源：http://xsu.c1oappe.top

[G10] 访问控制
来源：http://mzl.chenlongwang.top

Py:   约定 _protected / __private（不强制）
来源：http://tif.shuidangran.top

PHP:  public / protected / private
来源：http://ccu.zdbjq.cn

JS:   #private 字段；其余公开
来源：http://mbr.gotoacloud.top

TS:   public / protected / private
来源：http://kxy.epnwcf.com

Java: public / protected / private / 默认包级
来源：http://gtt.yongpay.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://yfu.ehwqpu.com

Ruby: public / protected / private
来源：http://unq.shanyushiyangkeji.top

C#:   public / protected / private / internal
来源：http://ghz.aibaodan.cn

[G11] getter / setter
来源：http://bbt.shzxlz.cn

Py:   @property 与 @x.setter
来源：http://hbf.uphjek.com

PHP:  public function getName(): string { return $this->name; }
来源：http://fhh.tian-w.cn

JS:   get name() { return this._name; }
来源：http://duk.nwbrower.top

TS:   get name(): string { return this._name; }
来源：http://por.jlsjyb.cn

Java: public String getName() { return name; }
来源：http://ltx.kuanghao11.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://npz.haohaochexian.top

Ruby: attr_accessor :name
来源：http://fts.fengsongda.top

C#:   public string Name { get; set; }
来源：http://myj.ehwqpu.com

[G12] 对象转字符串
来源：http://jqg.9152youxi.cn

Py:   def __str__(self): return self.name
来源：http://uac.ivvv.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://hbl.daxiang520.top

JS:   toString() { return this.name; }
来源：http://jqm.nwbrower.top

TS:   toString(): string { return this.name; }
来源：http://dtu.cqqwz.cn

Java: @Override public String toString() { return name; }
来源：http://bgx.hesvh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://abf.jinghuilouyu.cn

Ruby: def to_s; @name; end
来源：http://iah.shanyushiyangtech.top

C#:   public override string ToString() => Name;
来源：http://hij.jlsjyb.cn

[G13] 判断对象类型
来源：http://iqs.9152youxi.cn

Py:   isinstance(u, User)
来源：http://ngk.epnwcf.com

PHP:  $u instanceof User
来源：http://qpu.fehbvm.com

JS:   u instanceof User
来源：http://ubu.cqqwz.cn

TS:   u instanceof User
来源：http://nqm.tarul.cn

Java: u instanceof User
来源：http://tgg.yj202588.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://oql.xylfe.cn

Ruby: u.is_a?(User)
来源：http://woe.shanyushiyangtech.top

C#:   u is User
来源：http://tnr.jinyuanbaomall.cn

[G14] 数据类 / record
来源：http://vpm.0kj1m.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://avw.yuanzhike.top

PHP:  // 用 readonly 属性模拟
来源：http://doc.zhongyouzk.top

JS:   // 无内置：普通类或对象字面量
来源：http://wke.yj202588.top

TS:   type User = { name: string; age: number };
来源：http://dtg.cucudq.cn

Java: record User(String name, int age) {}
来源：http://pnn.jqgufenzy.top

Go:   type User struct { Name string; Age int }
来源：http://ctz.ywan-chungtsiang.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wxg.tanke756.top

C#:   record User(string Name, int Age);
来源：http://xng.xuanzx.com

[G15] 枚举
来源：http://pee.yuxming.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sha.hammf.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bwa.smart0.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://loq.guowangkeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vmz.jinqigufen.top

Java: enum Color { RED, GREEN }
来源：http://mpf.gaohongyu789.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://chy.hysaishi.cn

Ruby: Color = %i[red green].freeze
来源：http://drc.yj20258.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gzt.yueranfly.top

[G16] 对象转数组 / 字典
来源：http://dce.9152youxi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sma.fzhhl.top

PHP:  get_object_vars($obj);
来源：http://mkf.ywan-chungtsiang.top

JS:   Object.entries(obj)
来源：http://kma.quarkkingdee.top

TS:   Object.entries(obj)
来源：http://klh.zhongyouzk.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dih.bbcook.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ydb.pycfn.com

Ruby: obj.instance_variables
来源：http://yke.wangshuangyany.cn

C#:   // 用反射或 System.Text.Json
来源：http://ble.yanxiufei.cn

================================================================================
来源：http://eld.ydzc1.top

H. 异常与错误处理
来源：http://scm.tian-w.cn

================================================================================
来源：http://cej.zhengqikj.top

[H01] try / catch 基础
来源：http://hgb.yanxiufei.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kzj.yuanzhike.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vns.shanyushiyangtech.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dss.yonumen.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vzp.zdqjudy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kdp.yfazqb.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nzx.jinyuanbaomall.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qtq.shangyingyoupin.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gly.fzhhl.top

[H02] finally / ensure 收尾
来源：http://qsf.daxiang520.top

Py:   try: f()⏎finally: cleanup()
来源：http://fch.52xcode.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zfe.yueranfly.top

JS:   try { f(); } finally { cleanup(); }
来源：http://yix.xinyue.icu

TS:   try { f(); } finally { cleanup(); }
来源：http://enk.chenjidiqi.icu

Java: try { f(); } finally { cleanup(); }
来源：http://gjn.yvedp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://oxb.vehdjk.com

Ruby: begin; f; ensure; cleanup; end
来源：http://daz.yonumen.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://dde.yuxming.cn

[H03] 主动抛出异常
来源：http://vfg.smart0.xyz

Py:   raise ValueError("错误信息")
来源：http://rol.52xcode.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fjr.redwolf501.top

JS:   throw new Error("错误信息");
来源：http://eul.fengsongda.top

TS:   throw new Error("错误信息");
来源：http://kla.chenzaomai.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://zae.birdmap.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jsd.chenzaomai.com

Ruby: raise ArgumentError, "错误信息"
来源：http://gcj.zhixingplan.top

C#:   throw new ArgumentException("错误信息");
来源：http://bwx.zhixingplan.top

[H04] 自定义异常类型
来源：http://ret.zhijiandao.cn

Py:   class MyError(Exception): pass
来源：http://rua.yfazqb.com

PHP:  class MyError extends RuntimeException {}
来源：http://dlf.epnwcf.com

JS:   class MyError extends Error {}
来源：http://ziz.chenlongwang.top

TS:   class MyError extends Error {}
来源：http://eai.hongshengwenyu.top

Java: class MyException extends RuntimeException {}
来源：http://pbx.jqgfzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://smh.c1oappe.top

Ruby: class MyError < StandardError; end
来源：http://igq.haohaochexian.top

C#:   class MyException : Exception {}
来源：http://gjs.guannengcc.top

[H05] 捕获特定类型
来源：http://huf.yuxming.cn

Py:   except ValueError as e:
来源：http://lks.c1oappe.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dgr.nwbrower.top

JS:   if (e instanceof TypeError) {}
来源：http://eay.sjlbkw.cn

TS:   if (e instanceof TypeError) {}
来源：http://mfr.sysykeji.top

Java: catch (IOException | SQLException e) {}
来源：http://twp.guannengcc.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cbx.gogol.net.cn

Ruby: rescue ArgumentError => e
来源：http://ucn.nwbrower.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wuc.jinqigufen.top

[H06] 可选值 / 空值安全访问
来源：http://vgq.hammf.cn

Py:   value = d.get("k") or default
来源：http://sdp.yueranfly.top

PHP:  $v = $d["k"] ?? null;
来源：http://xxf.snrcjt.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sbl.jinqigufen.top

TS:   obj?.a?.b;  d ?? default
来源：http://btd.sufxvd.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gfq.vehdjk.com

Go:   if v, ok := m["k"]; ok { }
来源：http://amx.havefunace.top

Ruby: d&.dig(:a, :b)
来源：http://sbe.guowangkeji.top

C#:   obj?.A?.B ?? default
来源：http://xkf.gzhubu.top


<!-- 参考信息 -->