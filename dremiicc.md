代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://glq.quarkkingdee.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mdr.shanyushiyangtech.top

[F03] 写入文件（覆盖）
来源：http://cuc.bjfxy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vmz.gogol.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nws.ivvv.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ruv.bjfxy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mkv.xuetiantiany.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bwf.yj202588.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qry.zdbjq.cn

Ruby: File.write("a.txt", "hi")
来源：http://jgh.zhengqikj.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ywv.hammf.cn

[F04] 追加写入文件
来源：http://vzy.nanxuanxn.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zbq.svipenyu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mjf.sweek.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wfa.uphjek.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zef.tarul.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lna.jinghuilouyu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kje.shanyushiyangtech.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wto.xziqi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cpb.tarul.cn

[F05] 判断文件或目录是否存在
来源：http://szn.bjfxy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wky.bjfxy.top

PHP:  file_exists("a.txt");
来源：http://wdi.svipenyu.cn

JS:   fs.existsSync("a.txt")
来源：http://fho.zhengqikj.top

TS:   fs.existsSync("a.txt")
来源：http://oku.cqqwz.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://rme.cdnleiting.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dzz.havefunace.top

Ruby: File.exist?("a.txt")
来源：http://ajg.svipenyu.cn

C#:   File.Exists("a.txt")
来源：http://nti.xuetiantiany.cn

[F06] 删除文件
来源：http://aso.aizwys.cn

Py:   os.remove("a.txt")
来源：http://oit.yvedp.cn

PHP:  unlink("a.txt");
来源：http://fro.guannengcc.top

JS:   fs.unlinkSync("a.txt")
来源：http://cmi.havefunace.top

TS:   fs.unlinkSync("a.txt")
来源：http://hqv.jqgufenzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hxe.ehwqpu.com

Go:   os.Remove("a.txt")
来源：http://usr.zhiwuduotai.top

Ruby: File.delete("a.txt")
来源：http://hco.shzxlz.cn

C#:   File.Delete("a.txt");
来源：http://bly.daxiang520.top

[F07] 创建目录（含多级）
来源：http://iaf.tarul.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sfc.jinyuanbaomall.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ewv.feifeiyinyue.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kuq.ivvv.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vmw.zhiwuduotai.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://eiy.zycfv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gwi.yj202588.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xzc.chenlongwang.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tbv.cdnleiting.top

[F08] 遍历目录
来源：http://ylw.hnxiangtu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hkz.shzxlz.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fge.jqgfzy.top

JS:   fs.readdirSync("dir")
来源：http://tqc.jyoumei.cn

TS:   fs.readdirSync("dir")
来源：http://uln.gzhubu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bch.uphjek.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://exu.cashguo.top

Ruby: Dir.children("dir")
来源：http://hpq.cqqwz.cn

C#:   Directory.GetFiles("dir")
来源：http://emv.cdnleiting.top

[F09] 获取文件大小
来源：http://bfy.zhoulong.xyz

Py:   os.path.getsize("a.txt")
来源：http://xho.shanyushiyangtech.top

PHP:  filesize("a.txt");
来源：http://lph.snrcjt.cn

JS:   fs.statSync("a.txt").size
来源：http://onb.c1oappe.top

TS:   fs.statSync("a.txt").size
来源：http://gvr.sjlbkw.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tqw.jqgufenzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wau.hnxiangtu.top

Ruby: File.size("a.txt")
来源：http://fvt.gaohongyu789.top

C#:   new FileInfo("a.txt").Length
来源：http://rws.yvedp.cn

[F10] 取文件扩展名 / 文件名
来源：http://sep.tianlin.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pok.ybcxt.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xuz.guannengcc.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vza.ctjpmb.com

TS:   path.extname("a.txt")
来源：http://jnr.bbcook.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sqd.pycfn.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dqf.ctjpmb.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yws.jqgufenzy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lgx.epnwcf.com

[F11] 复制与移动文件
来源：http://dtu.yvedp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nqk.kuanghao11.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fwl.yj202588.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tqi.jlsjyb.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wnw.sweek.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://eid.yj20258888.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uew.fehbvm.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ckl.cashguo.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wye.daria6918.cn

[F12] CSV 读写
来源：http://zyp.yuanzhike.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://omb.hcnkem.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hfb.sufxvd.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vsp.yj202588.top

TS:   // 同上
来源：http://rxs.pycfn.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://str.chenzaomai.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ggd.xylfe.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ypl.ppjwa.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://jpe.bbcook.cn

================================================================================
来源：http://qbe.zdqjudy.top

G. 面向对象
来源：http://pnz.hnxiangtu.top

================================================================================
来源：http://ypb.wangdashe.top

[G01] 定义类
来源：http://vgt.yueranfly.top

Py:   class User: pass
来源：http://nbx.jinyuanbaomall.cn

PHP:  class User {}
来源：http://ilt.gogol.net.cn

JS:   class User {}
来源：http://wdz.jinqigfzy.top

TS:   class User { name: string = ""; }
来源：http://fmc.jqgfzy.top

Java: class User {}
来源：http://spr.dianchejie.cn

Go:   type User struct { Name string }
来源：http://lub.hcnkem.com

Ruby: class User; end
来源：http://goe.gzhubu.top

C#:   class User {}
来源：http://jdl.tianlin.xyz

[G02] 构造函数
来源：http://dsz.haohaochexian.top

Py:   def __init__(self, name): self.name = name
来源：http://tij.ywan-chungtsiang.top

PHP:  public function __construct(public string $name) {}
来源：http://pvq.hnxiangtu.top

JS:   constructor(name) { this.name = name; }
来源：http://olq.cheryme.top

TS:   constructor(public name: string) {}
来源：http://qov.snrcjt.cn

Java: User(String name) { this.name = name; }
来源：http://hbw.yanxiufei.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qlm.zhaomingkeji.xyz

Ruby: def initialize(name); @name = name; end
来源：http://uts.sweek.top

C#:   public User(string name) { Name = name; }
来源：http://njl.snrcjt.cn

[G03] 实例属性
来源：http://gwq.bbcook.cn

Py:   self.name = "x"
来源：http://hdb.zhengqikj.top

PHP:  public string $name = "x";
来源：http://sqg.zhixingplan.top

JS:   this.name = "x";
来源：http://deq.hnxiangtu.top

TS:   name: string = "x";
来源：http://gyf.hammf.cn

Java: private String name;
来源：http://lgr.fktsv.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uhm.yonumen.top

Ruby: @name = "x"
来源：http://zip.hesvh.cn

C#:   public string Name { get; set; } = "x";
来源：http://zcu.xylfe.cn

[G04] 定义方法
来源：http://lmt.daria6918.cn

Py:   def greet(self): return self.name
来源：http://qwg.andypj.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://nqc.sweek.top

JS:   greet() { return this.name; }
来源：http://lpm.nanxuanxn.top

TS:   greet(): string { return this.name; }
来源：http://jnu.shangyingyoupin.top

Java: String greet() { return name; }
来源：http://kah.yueranfly.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://vgp.uphjek.com

Ruby: def greet; @name; end
来源：http://pfq.yangfankeji.com

C#:   public string Greet() => Name;
来源：http://agx.nanxuanxn.top

[G05] 继承
来源：http://msz.jqgfzy.top

Py:   class Admin(User): pass
来源：http://dxm.tianlin.xyz

PHP:  class Admin extends User {}
来源：http://mmi.zhongyouzk.top

JS:   class Admin extends User {}
来源：http://jjk.haohaochexian.top

TS:   class Admin extends User {}
来源：http://xvr.iojbl.cn

Java: class Admin extends User {}
来源：http://pwu.ivvv.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://atz.sxryk.cn

Ruby: class Admin < User; end
来源：http://inz.guowangkeji.top

C#:   class Admin : User {}
来源：http://gvv.nwbrower.top

[G06] 重写方法
来源：http://rtr.fzhhl.top

Py:   def greet(self): return "admin"
来源：http://bdi.gaohongyu789.top

PHP:  public function greet(): string { return "admin"; }
来源：http://mue.xuanzx.com

JS:   greet() { return "admin"; }
来源：http://fsd.jiagoushi.top

TS:   greet(): string { return "admin"; }
来源：http://qgt.xziqi.cn

Java: @Override String greet() { return "admin"; }
来源：http://yov.chenzaomai.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ibp.ydjk.org.cn

Ruby: def greet; "admin"; end
来源：http://tbc.smart0.xyz

C#:   public override string Greet() => "admin";
来源：http://jtu.ywan-chungtsiang.top

[G07] 调用父类方法
来源：http://lls.52xcode.cn

Py:   super().greet()
来源：http://mhs.dianchejie.cn

PHP:  parent::greet();
来源：http://fcc.hfpthk.cn

JS:   super.greet();
来源：http://kcs.jinqigufen.top

TS:   super.greet();
来源：http://qvo.fzhhl.top

Java: super.greet();
来源：http://xxn.ybcxt.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jxa.nwbrower.top

Ruby: super
来源：http://cxq.shuidangran.top

C#:   base.Greet();
来源：http://vdj.sweek.top

[G08] 静态方法与属性
来源：http://wps.dashuyun.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ihg.ehwqpu.com

PHP:  public static function f() {}
来源：http://kjb.vehdjk.com

JS:   static f() {}
来源：http://xhz.jiagoushi.top

TS:   static f(): void {}
来源：http://gso.zycfv.cn

Java: static void f() {}
来源：http://gma.kuanghao11.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kig.chenjidiqi.icu

Ruby: def self.f; end
来源：http://ugn.hongshengwenyu.top

C#:   public static void F() {}
来源：http://okr.ivvv.top

[G09] 接口 / 抽象类
来源：http://apw.jqgfzy.top

Py:   from abc import ABC, abstractmethod
来源：http://jcg.shzxlz.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pvv.birdmap.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://enc.9152youxi.cn

TS:   interface Shape { area(): number; }
来源：http://rtp.zdbjq.cn

Java: interface Shape { double area(); }
来源：http://wbf.guowangkeji.top

Go:   type Shape interface { Area() float64 }
来源：http://eha.sjlbkw.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gjk.mhx1999.top

C#:   interface IShape { double Area(); }
来源：http://ygj.zdbjq.cn

[G10] 访问控制
来源：http://cqn.sysykeji.top

Py:   约定 _protected / __private（不强制）
来源：http://lla.zhengqikj.top

PHP:  public / protected / private
来源：http://vwo.yj20258888.top

JS:   #private 字段；其余公开
来源：http://hvq.yj20258.top

TS:   public / protected / private
来源：http://kdk.gzhubu.top

Java: public / protected / private / 默认包级
来源：http://nqp.sxryk.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://sjk.kuanghao11.cn

Ruby: public / protected / private
来源：http://pvh.52xcode.cn

C#:   public / protected / private / internal
来源：http://biz.meibo888.top

[G11] getter / setter
来源：http://bfo.ehwqpu.com

Py:   @property 与 @x.setter
来源：http://jzn.sjlbkw.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ivh.sjlbkw.cn

JS:   get name() { return this._name; }
来源：http://akc.hfpthk.cn

TS:   get name(): string { return this._name; }
来源：http://fza.jiagoushi.top

Java: public String getName() { return name; }
来源：http://yes.tianlin.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://kyb.haohaochexian.top

Ruby: attr_accessor :name
来源：http://kmd.jinqigfzy.top

C#:   public string Name { get; set; }
来源：http://dli.sufxvd.cn

[G12] 对象转字符串
来源：http://dil.cheryme.top

Py:   def __str__(self): return self.name
来源：http://pjy.havefunace.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ojk.yongpay.top

JS:   toString() { return this.name; }
来源：http://wsr.wangshuangyany.cn

TS:   toString(): string { return this.name; }
来源：http://uvj.yuanzhike.top

Java: @Override public String toString() { return name; }
来源：http://ill.52xcode.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hbm.sxryk.cn

Ruby: def to_s; @name; end
来源：http://kuv.shangyingyoupin.top

C#:   public override string ToString() => Name;
来源：http://mis.shanyushiyangtech.top

[G13] 判断对象类型
来源：http://xzt.zdqjudy.top

Py:   isinstance(u, User)
来源：http://pas.yongpay.top

PHP:  $u instanceof User
来源：http://dxh.guannengcc.top

JS:   u instanceof User
来源：http://dew.jqgufenzy.top

TS:   u instanceof User
来源：http://cou.shanyushiyangkeji.top

Java: u instanceof User
来源：http://lrf.cqqwz.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ztz.shanyushiyangtech.top

Ruby: u.is_a?(User)
来源：http://nxz.sweek.top

C#:   u is User
来源：http://pfv.daxiang520.top

[G14] 数据类 / record
来源：http://dzp.ybcxt.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rlj.yuxming.cn

PHP:  // 用 readonly 属性模拟
来源：http://dgy.shuidangran.top

JS:   // 无内置：普通类或对象字面量
来源：http://frl.sufxvd.cn

TS:   type User = { name: string; age: number };
来源：http://jvl.daria6918.cn

Java: record User(String name, int age) {}
来源：http://qjq.andypj.xyz

Go:   type User struct { Name string; Age int }
来源：http://zuh.fengsongda.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://myj.nanxuanxn.top

C#:   record User(string Name, int Age);
来源：http://omu.hnxiangtu.top

[G15] 枚举
来源：http://che.fktsv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://die.jiagoushi.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ioy.zhoulong.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rlx.jqgufenzy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://arj.aizwys.cn

Java: enum Color { RED, GREEN }
来源：http://xmy.cdnleiting.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uuh.gogol.net.cn

Ruby: Color = %i[red green].freeze
来源：http://jen.ivvv.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iky.jyoumei.cn

[G16] 对象转数组 / 字典
来源：http://cqa.nwbrower.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bdi.shanyushiyangtech.top

PHP:  get_object_vars($obj);
来源：http://lfo.xuanzx.com

JS:   Object.entries(obj)
来源：http://hqd.9152youxi.cn

TS:   Object.entries(obj)
来源：http://lyi.vqdsnc.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://oxm.nanxinkj.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://qan.hammf.cn

Ruby: obj.instance_variables
来源：http://hxj.yueranfly.top

C#:   // 用反射或 System.Text.Json
来源：http://saf.gogol.net.cn

================================================================================
来源：http://ktv.52xcode.cn

H. 异常与错误处理
来源：http://sum.zhaomingkeji.xyz

================================================================================
来源：http://ayr.hcnkem.com

[H01] try / catch 基础
来源：http://hex.birdmap.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mbl.zdbjq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zgv.wangdashe.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mem.ywan-chungtsiang.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://oma.hammf.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ysm.cqqwz.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://llh.jlsjyb.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yym.cucudq.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ywl.wangshuangyany.cn

[H02] finally / ensure 收尾
来源：http://two.snrcjt.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zxq.pycfn.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://vph.xingfuxueyuan.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://uxj.jianghu66.top

TS:   try { f(); } finally { cleanup(); }
来源：http://xdm.shanyushiyangkeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://plt.bjfxy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ukf.jinqigufen.top

Ruby: begin; f; ensure; cleanup; end
来源：http://anw.ctjpmb.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://jdc.cqqwz.cn

[H03] 主动抛出异常
来源：http://pta.wangdashe.top

Py:   raise ValueError("错误信息")
来源：http://wmy.hcnkem.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yhw.yuxming.cn

JS:   throw new Error("错误信息");
来源：http://dnx.tanke756.top

TS:   throw new Error("错误信息");
来源：http://ony.jqgfzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://lkw.iojbl.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lxx.sjlbkw.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vpd.ywan-chungtsiang.top

C#:   throw new ArgumentException("错误信息");
来源：http://kxz.bjfxy.top

[H04] 自定义异常类型
来源：http://vdk.gaohongyu789.top

Py:   class MyError(Exception): pass
来源：http://spb.nanxinkj.top

PHP:  class MyError extends RuntimeException {}
来源：http://kuc.xinyue.icu

JS:   class MyError extends Error {}
来源：http://zxt.yueranfly.top

TS:   class MyError extends Error {}
来源：http://tkm.ybcxt.top

Java: class MyException extends RuntimeException {}
来源：http://iti.birdmap.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tpk.yvedp.cn

Ruby: class MyError < StandardError; end
来源：http://ywg.nanxinkj.top

C#:   class MyException : Exception {}
来源：http://izw.xingfuxueyuan.xyz

[H05] 捕获特定类型
来源：http://vci.jinyuanbaomall.cn

Py:   except ValueError as e:
来源：http://omq.tianlin.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ouz.redwolf501.top

JS:   if (e instanceof TypeError) {}
来源：http://grk.hysaishi.cn

TS:   if (e instanceof TypeError) {}
来源：http://hkw.pycfn.com

Java: catch (IOException | SQLException e) {}
来源：http://tmm.feifeiyinyue.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cbn.sxryk.cn

Ruby: rescue ArgumentError => e
来源：http://ujd.shuidangran.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ktd.gotoacloud.top

[H06] 可选值 / 空值安全访问
来源：http://lpi.xylfe.cn

Py:   value = d.get("k") or default
来源：http://rqb.vehdjk.com

PHP:  $v = $d["k"] ?? null;
来源：http://uvv.shanyushiyangkeji.top

JS:   obj?.a?.b;  d ?? default
来源：http://isq.shuidangran.top

TS:   obj?.a?.b;  d ?? default
来源：http://ryy.haohaochexian.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vmh.pycfn.com

Go:   if v, ok := m["k"]; ok { }
来源：http://sme.feifeiyinyue.top

Ruby: d&.dig(:a, :b)
来源：http://wxl.birdmap.top

C#:   obj?.A?.B ?? default
来源：http://mde.jqgufenzy.top

[H07] 断言
来源：http://ltp.fengsongda.top

Py:   assert x > 0, "必须为正"
来源：http://wgx.cqqwz.cn

PHP:  assert($x > 0);
来源：http://tey.ehwqpu.com

JS:   console.assert(x > 0);
来源：http://mdi.havefunace.top


<!-- 参考信息 -->