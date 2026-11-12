代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://acz.yj20258888.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://iuj.fanxiaobao.xyz

[F03] 写入文件（覆盖）
来源：http://beq.vehdjk.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nos.shanyushiyangkeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://dlu.xuetiantiany.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://abr.jlsjyb.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vwy.fktsv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yrv.0kj1m.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vvt.gaohongyu789.top

Ruby: File.write("a.txt", "hi")
来源：http://cxk.wangdashe.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cin.tian-w.cn

[F04] 追加写入文件
来源：http://kko.yueranfly.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ani.316326.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ojh.yuanzhike.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://asz.sweek.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://grd.andypj.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sba.hfpthk.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xlr.jiagoushi.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://epl.gaohongyu789.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hga.zhengqikj.top

[F05] 判断文件或目录是否存在
来源：http://eiw.xinyue.icu

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wix.aizwys.cn

PHP:  file_exists("a.txt");
来源：http://dhe.xuanzx.com

JS:   fs.existsSync("a.txt")
来源：http://umm.zycfv.cn

TS:   fs.existsSync("a.txt")
来源：http://zjx.zhaomingkeji.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://vfu.zhongyouzk.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wql.yanxiufei.cn

Ruby: File.exist?("a.txt")
来源：http://nxq.nwbrower.top

C#:   File.Exists("a.txt")
来源：http://ikl.hcnkem.com

[F06] 删除文件
来源：http://wgj.hongshengwenyu.top

Py:   os.remove("a.txt")
来源：http://yzu.ybcxt.top

PHP:  unlink("a.txt");
来源：http://rqq.xuanzx.com

JS:   fs.unlinkSync("a.txt")
来源：http://poh.chenzaomai.com

TS:   fs.unlinkSync("a.txt")
来源：http://eyq.shanyushiyangtech.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lfu.tian-w.cn

Go:   os.Remove("a.txt")
来源：http://efb.jiagoushi.top

Ruby: File.delete("a.txt")
来源：http://whi.yj20258888.top

C#:   File.Delete("a.txt");
来源：http://cdd.zhiwuduotai.top

[F07] 创建目录（含多级）
来源：http://gzy.ydjk.org.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://iok.fanxiaobao.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yyi.hesvh.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uwd.vqdsnc.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://onb.xingfuxueyuan.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jxn.hywenlv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mys.cdnleiting.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://con.dashuyun.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xuo.316326.xyz

[F08] 遍历目录
来源：http://awt.fanxiaobao.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://koe.xylfe.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xaf.nwbrower.top

JS:   fs.readdirSync("dir")
来源：http://tdy.gotoacloud.top

TS:   fs.readdirSync("dir")
来源：http://pyg.daria6918.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ctc.haohaochexian.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://yog.chenzaomai.com

Ruby: Dir.children("dir")
来源：http://asp.zdqjudy.top

C#:   Directory.GetFiles("dir")
来源：http://mzm.hnxiangtu.top

[F09] 获取文件大小
来源：http://ndq.chenjidiqi.icu

Py:   os.path.getsize("a.txt")
来源：http://cos.jinqigfzy.top

PHP:  filesize("a.txt");
来源：http://bga.daxiang520.top

JS:   fs.statSync("a.txt").size
来源：http://ujh.gzhubu.top

TS:   fs.statSync("a.txt").size
来源：http://qcy.zhongyouzk.top

Java: Files.size(Path.of("a.txt"))
来源：http://vkn.jqgufenzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ydk.yonumen.top

Ruby: File.size("a.txt")
来源：http://rim.iojbl.cn

C#:   new FileInfo("a.txt").Length
来源：http://jee.feifeiyinyue.top

[F10] 取文件扩展名 / 文件名
来源：http://eru.ctjpmb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qql.ybcxt.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dne.sxryk.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xgn.jinqigufen.top

TS:   path.extname("a.txt")
来源：http://owr.jiagoushi.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wiv.hywenlv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://clm.xziqi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hej.wangdashe.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mdo.jianghu66.top

[F11] 复制与移动文件
来源：http://tqb.xinyue.icu

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qsc.daxiang520.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://omc.jianghu66.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://caf.aibaodan.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bve.gogol.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bht.sysykeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jjq.cucudq.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://znf.sjlbkw.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tzp.ywan-chungtsiang.top

[F12] CSV 读写
来源：http://bmk.hywenlv.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hzj.yuanzhike.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ino.jinyuanbaomall.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://aem.yongpay.top

TS:   // 同上
来源：http://bzm.gotoacloud.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mbw.9152youxi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mqm.dianchejie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xyv.ydjk.org.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ipy.guowangkeji.top

================================================================================
来源：http://hjh.yongpay.top

G. 面向对象
来源：http://yiq.havefunace.top

================================================================================
来源：http://upv.yanxiufei.cn

[G01] 定义类
来源：http://foi.tian-w.cn

Py:   class User: pass
来源：http://ymg.zhixingplan.top

PHP:  class User {}
来源：http://oxt.xuetiantiany.cn

JS:   class User {}
来源：http://eqx.gotoacloud.top

TS:   class User { name: string = ""; }
来源：http://gfz.zhoulong.xyz

Java: class User {}
来源：http://oxj.tanke756.top

Go:   type User struct { Name string }
来源：http://ifj.zhoulong.xyz

Ruby: class User; end
来源：http://lnl.sysykeji.top

C#:   class User {}
来源：http://mny.zhaomingkeji.xyz

[G02] 构造函数
来源：http://wet.yuanzhike.top

Py:   def __init__(self, name): self.name = name
来源：http://ybt.shanyushiyangkeji.top

PHP:  public function __construct(public string $name) {}
来源：http://byy.fengsongda.top

JS:   constructor(name) { this.name = name; }
来源：http://dmm.sysykeji.top

TS:   constructor(public name: string) {}
来源：http://thn.yj20258888.top

Java: User(String name) { this.name = name; }
来源：http://cae.jlsjyb.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://thd.jianghu66.top

Ruby: def initialize(name); @name = name; end
来源：http://ylm.nanxinkj.top

C#:   public User(string name) { Name = name; }
来源：http://doy.316326.xyz

[G03] 实例属性
来源：http://ttf.316326.xyz

Py:   self.name = "x"
来源：http://kiq.xylfe.cn

PHP:  public string $name = "x";
来源：http://ayg.xziqi.cn

JS:   this.name = "x";
来源：http://zkl.fehbvm.com

TS:   name: string = "x";
来源：http://kdn.tian-w.cn

Java: private String name;
来源：http://wij.hysaishi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://slr.yvedp.cn

Ruby: @name = "x"
来源：http://kmc.yvedp.cn

C#:   public string Name { get; set; } = "x";
来源：http://uzk.kuanghao11.cn

[G04] 定义方法
来源：http://rta.zhijiandao.cn

Py:   def greet(self): return self.name
来源：http://dwt.vqdsnc.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xuu.dianchejie.cn

JS:   greet() { return this.name; }
来源：http://mgt.jqgfzy.top

TS:   greet(): string { return this.name; }
来源：http://rhb.ehwqpu.com

Java: String greet() { return name; }
来源：http://zak.nanxinkj.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://czc.shzxlz.cn

Ruby: def greet; @name; end
来源：http://jgh.tarul.cn

C#:   public string Greet() => Name;
来源：http://ypb.yuxming.cn

[G05] 继承
来源：http://dey.jiagoushi.top

Py:   class Admin(User): pass
来源：http://jbk.uphjek.com

PHP:  class Admin extends User {}
来源：http://kat.wangdashe.top

JS:   class Admin extends User {}
来源：http://xrv.yuxming.cn

TS:   class Admin extends User {}
来源：http://vvh.yj20258.top

Java: class Admin extends User {}
来源：http://mnl.nanxuanxn.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dan.snrcjt.cn

Ruby: class Admin < User; end
来源：http://cjn.tanke756.top

C#:   class Admin : User {}
来源：http://hyu.cheryme.top

[G06] 重写方法
来源：http://byl.yvedp.cn

Py:   def greet(self): return "admin"
来源：http://xji.9152youxi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://buc.gzhubu.top

JS:   greet() { return "admin"; }
来源：http://mtd.xuanzx.com

TS:   greet(): string { return "admin"; }
来源：http://esw.jianghu66.top

Java: @Override String greet() { return "admin"; }
来源：http://oek.jlsjyb.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bjs.hnxiangtu.top

Ruby: def greet; "admin"; end
来源：http://tnp.fengsongda.top

C#:   public override string Greet() => "admin";
来源：http://okh.jqgfzy.top

[G07] 调用父类方法
来源：http://vnx.tarul.cn

Py:   super().greet()
来源：http://tyb.tian-w.cn

PHP:  parent::greet();
来源：http://far.ivvv.top

JS:   super.greet();
来源：http://uop.redwolf501.top

TS:   super.greet();
来源：http://hrl.cheryme.top

Java: super.greet();
来源：http://gfl.gotoacloud.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vog.daria6918.cn

Ruby: super
来源：http://hjg.fengsongda.top

C#:   base.Greet();
来源：http://qul.dashuyun.cn

[G08] 静态方法与属性
来源：http://kyr.yuxming.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lpw.xuetiantiany.cn

PHP:  public static function f() {}
来源：http://ytg.pengpengdd.cyou

JS:   static f() {}
来源：http://qvi.tian-w.cn

TS:   static f(): void {}
来源：http://wnb.cdnleiting.top

Java: static void f() {}
来源：http://rxk.zdbjq.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kur.cdnleiting.top

Ruby: def self.f; end
来源：http://dnc.cdnleiting.top

C#:   public static void F() {}
来源：http://nkj.fktsv.cn

[G09] 接口 / 抽象类
来源：http://ckt.yonumen.top

Py:   from abc import ABC, abstractmethod
来源：http://zih.zhongyouzk.top

PHP:  interface Shape { public function area(): float; }
来源：http://rzh.jinqigfzy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://plt.ydjk.org.cn

TS:   interface Shape { area(): number; }
来源：http://hpd.zhiwuduotai.top

Java: interface Shape { double area(); }
来源：http://wve.guowangkeji.top

Go:   type Shape interface { Area() float64 }
来源：http://gnt.sxryk.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xeg.zhongyouzk.top

C#:   interface IShape { double Area(); }
来源：http://qrb.quarkkingdee.top

[G10] 访问控制
来源：http://bqn.cqqwz.cn

Py:   约定 _protected / __private（不强制）
来源：http://iue.dianchejie.cn

PHP:  public / protected / private
来源：http://ypm.zhongyouzk.top

JS:   #private 字段；其余公开
来源：http://rbf.mhx1999.top

TS:   public / protected / private
来源：http://cvq.yj202588.top

Java: public / protected / private / 默认包级
来源：http://ozq.pengpengdd.cyou

Go:   首字母大写可导出，小写仅包内可见
来源：http://une.sweek.top

Ruby: public / protected / private
来源：http://chy.zhongyouzk.top

C#:   public / protected / private / internal
来源：http://czm.andypj.xyz

[G11] getter / setter
来源：http://scd.hesvh.cn

Py:   @property 与 @x.setter
来源：http://tuo.kuanghao11.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ryr.hammf.cn

JS:   get name() { return this._name; }
来源：http://ssa.redwolf501.top

TS:   get name(): string { return this._name; }
来源：http://ogz.zhixingplan.top

Java: public String getName() { return name; }
来源：http://hac.jqgufenzy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://qcf.gotoacloud.top

Ruby: attr_accessor :name
来源：http://vcc.zycfv.cn

C#:   public string Name { get; set; }
来源：http://feo.zhijiandao.cn

[G12] 对象转字符串
来源：http://acn.dianchejie.cn

Py:   def __str__(self): return self.name
来源：http://ssu.hnxiangtu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://xcv.xingfuxueyuan.xyz

JS:   toString() { return this.name; }
来源：http://hod.fanxiaobao.xyz

TS:   toString(): string { return this.name; }
来源：http://nkh.birdmap.top

Java: @Override public String toString() { return name; }
来源：http://hla.wangshuangyany.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ykq.sjlbkw.cn

Ruby: def to_s; @name; end
来源：http://hux.nanxinkj.top

C#:   public override string ToString() => Name;
来源：http://aem.zhengqikj.top

[G13] 判断对象类型
来源：http://fbm.zhixingplan.top

Py:   isinstance(u, User)
来源：http://fnq.fanxiaobao.xyz

PHP:  $u instanceof User
来源：http://cbs.xinyue.icu

JS:   u instanceof User
来源：http://jmo.zycfv.cn

TS:   u instanceof User
来源：http://qwh.dianchejie.cn

Java: u instanceof User
来源：http://kqg.xziqi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xkz.shuidangran.top

Ruby: u.is_a?(User)
来源：http://mdv.316326.xyz

C#:   u is User
来源：http://ipe.daxiang520.top

[G14] 数据类 / record
来源：http://gln.meibo888.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fsf.cheryme.top

PHP:  // 用 readonly 属性模拟
来源：http://mql.vehdjk.com

JS:   // 无内置：普通类或对象字面量
来源：http://bnr.xziqi.cn

TS:   type User = { name: string; age: number };
来源：http://dgu.jinqigfzy.top

Java: record User(String name, int age) {}
来源：http://wwt.ybcxt.top

Go:   type User struct { Name string; Age int }
来源：http://rkl.52xcode.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rwp.shangyingyoupin.top

C#:   record User(string Name, int Age);
来源：http://xtb.jyoumei.cn

[G15] 枚举
来源：http://tgr.ehwqpu.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bka.daxiang520.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://umi.tianlin.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://isu.xylfe.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bku.feifeiyinyue.top

Java: enum Color { RED, GREEN }
来源：http://xrd.9152youxi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mxr.daxiang520.top

Ruby: Color = %i[red green].freeze
来源：http://hmd.jinqigufen.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wpk.xingfuxueyuan.xyz

[G16] 对象转数组 / 字典
来源：http://lyx.pycfn.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ege.gogol.net.cn

PHP:  get_object_vars($obj);
来源：http://gbj.zycfv.cn

JS:   Object.entries(obj)
来源：http://zaq.nwbrower.top

TS:   Object.entries(obj)
来源：http://zqx.ppjwa.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lsa.fehbvm.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://hfc.jqgfzy.top

Ruby: obj.instance_variables
来源：http://orh.xuanzx.com

C#:   // 用反射或 System.Text.Json
来源：http://ana.yuxming.cn

================================================================================
来源：http://jle.snrcjt.cn

H. 异常与错误处理
来源：http://chx.wangdashe.top

================================================================================
来源：http://pxa.dashuyun.cn

[H01] try / catch 基础
来源：http://djy.jqgfzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ksa.mhx1999.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://etr.hammf.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cmn.sweek.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://abu.cdnleiting.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rky.ehwqpu.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ief.hesvh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qpz.hnxiangtu.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ahl.yanxiufei.cn

[H02] finally / ensure 收尾
来源：http://ogh.sysykeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://rui.shanyushiyangkeji.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://wdd.guannengcc.top

JS:   try { f(); } finally { cleanup(); }
来源：http://kys.shzxlz.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yqp.ydjk.org.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fko.tian-w.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ghh.bjfxy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://cfd.cashguo.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://aqx.xuetiantiany.cn

[H03] 主动抛出异常
来源：http://wwt.haohaochexian.top

Py:   raise ValueError("错误信息")
来源：http://pat.xuanzx.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ety.hcnkem.com

JS:   throw new Error("错误信息");
来源：http://ngf.gogol.net.cn

TS:   throw new Error("错误信息");
来源：http://xzs.sweek.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://fzb.haohaochexian.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://awr.c1oappe.top

Ruby: raise ArgumentError, "错误信息"
来源：http://elx.nwbrower.top

C#:   throw new ArgumentException("错误信息");
来源：http://cys.yj20258888.top

[H04] 自定义异常类型
来源：http://mtr.fktsv.cn

Py:   class MyError(Exception): pass
来源：http://uym.havefunace.top

PHP:  class MyError extends RuntimeException {}
来源：http://dtq.wangdashe.top

JS:   class MyError extends Error {}
来源：http://oda.xziqi.cn

TS:   class MyError extends Error {}
来源：http://gxd.ybcxt.top

Java: class MyException extends RuntimeException {}
来源：http://eth.zhiwuduotai.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xoa.jiagoushi.top

Ruby: class MyError < StandardError; end
来源：http://yge.epnwcf.com

C#:   class MyException : Exception {}
来源：http://lqo.guannengcc.top

[H05] 捕获特定类型
来源：http://shz.ivvv.top

Py:   except ValueError as e:
来源：http://wqn.guowangkeji.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://iko.yj202588.top

JS:   if (e instanceof TypeError) {}
来源：http://won.chenzaomai.com

TS:   if (e instanceof TypeError) {}
来源：http://pwi.zhengqikj.top

Java: catch (IOException | SQLException e) {}
来源：http://uek.chenzaomai.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ggo.dianchejie.cn

Ruby: rescue ArgumentError => e
来源：http://edk.zhiwuduotai.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wkf.shuidangran.top

[H06] 可选值 / 空值安全访问
来源：http://otx.shuidangran.top

Py:   value = d.get("k") or default
来源：http://bbg.zhiwuduotai.top

PHP:  $v = $d["k"] ?? null;
来源：http://crg.meibo888.top

JS:   obj?.a?.b;  d ?? default
来源：http://xdv.yj20258.top

TS:   obj?.a?.b;  d ?? default
来源：http://biv.daria6918.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gju.yj20258.top

Go:   if v, ok := m["k"]; ok { }
来源：http://jku.nanxinkj.top

Ruby: d&.dig(:a, :b)
来源：http://ujo.aizwys.cn

C#:   obj?.A?.B ?? default
来源：http://ula.zdqjudy.top

[H07] 断言
来源：http://hqp.xuanzx.com

Py:   assert x > 0, "必须为正"
来源：http://dqf.hfpthk.cn

PHP:  assert($x > 0);
来源：http://xqq.dashuyun.cn

JS:   console.assert(x > 0);
来源：http://tzq.guannengcc.top


<!-- 参考信息 -->