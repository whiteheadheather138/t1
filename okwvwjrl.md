代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sgr.jinghuilouyu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xwm.ydjk.org.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uuf.ppjwa.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mxv.fktsv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tje.pengpengdd.cyou

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mwr.52xcode.cn

[F03] 写入文件（覆盖）
来源：http://hcm.yongpay.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zlx.sufxvd.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bss.yuxming.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vjj.cashguo.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jig.tarul.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ksj.zhijiandao.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gal.gotoacloud.top

Ruby: File.write("a.txt", "hi")
来源：http://qxv.snrcjt.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hwq.yuxming.cn

[F04] 追加写入文件
来源：http://qmu.yj20258888.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sph.hcnkem.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uov.yonumen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sar.pycfn.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://auw.ywan-chungtsiang.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wtq.fktsv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ivx.meibo888.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uzg.shanyushiyangtech.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nby.jqgufenzy.top

[F05] 判断文件或目录是否存在
来源：http://sxs.dianchejie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://upm.xuetiantiany.cn

PHP:  file_exists("a.txt");
来源：http://tml.xuetiantiany.cn

JS:   fs.existsSync("a.txt")
来源：http://xnf.wangdashe.top

TS:   fs.existsSync("a.txt")
来源：http://hgm.jqgufenzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://teh.chenzaomai.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pdo.jlsjyb.cn

Ruby: File.exist?("a.txt")
来源：http://obv.nwbrower.top

C#:   File.Exists("a.txt")
来源：http://xzl.jqgfzy.top

[F06] 删除文件
来源：http://vcp.316326.xyz

Py:   os.remove("a.txt")
来源：http://ngh.snrcjt.cn

PHP:  unlink("a.txt");
来源：http://wrz.jqgufenzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://bsf.zycfv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vlm.ppjwa.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dqe.mhx1999.top

Go:   os.Remove("a.txt")
来源：http://ylr.daxiang520.top

Ruby: File.delete("a.txt")
来源：http://lbq.yanxiufei.cn

C#:   File.Delete("a.txt");
来源：http://akc.ybcxt.top

[F07] 创建目录（含多级）
来源：http://thu.ybcxt.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://frf.jinqigfzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://iop.shanyushiyangtech.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hfa.zhoulong.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yxi.ehwqpu.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ycy.pengpengdd.cyou

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cij.svipenyu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vrh.yvedp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fpu.bjfxy.top

[F08] 遍历目录
来源：http://qcu.zhijiandao.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gqb.pengpengdd.cyou

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cvh.yuxming.cn

JS:   fs.readdirSync("dir")
来源：http://hmx.jinyuanbaomall.cn

TS:   fs.readdirSync("dir")
来源：http://xce.sxryk.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ujv.fzhhl.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://msd.tian-w.cn

Ruby: Dir.children("dir")
来源：http://iaq.pengpengdd.cyou

C#:   Directory.GetFiles("dir")
来源：http://fdu.yanxiufei.cn

[F09] 获取文件大小
来源：http://cxf.sufxvd.cn

Py:   os.path.getsize("a.txt")
来源：http://aee.fehbvm.com

PHP:  filesize("a.txt");
来源：http://jes.hnqzz.top

JS:   fs.statSync("a.txt").size
来源：http://oer.xuanzx.com

TS:   fs.statSync("a.txt").size
来源：http://lqk.tian-w.cn

Java: Files.size(Path.of("a.txt"))
来源：http://sjo.ppjwa.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ajo.aizwys.cn

Ruby: File.size("a.txt")
来源：http://tbq.52xcode.cn

C#:   new FileInfo("a.txt").Length
来源：http://qbv.yuanzhike.top

[F10] 取文件扩展名 / 文件名
来源：http://xsm.ydzc1.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fbs.quarkkingdee.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qcy.zhengqikj.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nwb.pengpengdd.cyou

TS:   path.extname("a.txt")
来源：http://czy.shanyushiyangtech.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ype.sjlbkw.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xcq.yj20258888.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qge.snrcjt.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xsi.yvedp.cn

[F11] 复制与移动文件
来源：http://ytq.jqgfzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://snj.hammf.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://biq.zhaomingkeji.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cgi.redwolf501.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ymk.daxiang520.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ozm.tian-w.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jua.zhoulong.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mbj.meibo888.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://omc.jinyuanbaomall.cn

[F12] CSV 读写
来源：http://lzr.yuxming.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vuc.9152youxi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wck.fehbvm.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tlf.sweek.top

TS:   // 同上
来源：http://cca.316326.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tnx.vehdjk.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nvb.ybcxt.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lop.fehbvm.com

C#:   // 无内置：用 CsvHelper 库
来源：http://rfy.jinqigfzy.top

================================================================================
来源：http://tib.ehwqpu.com

G. 面向对象
来源：http://aqg.fengsongda.top

================================================================================
来源：http://hxa.yfazqb.com

[G01] 定义类
来源：http://mpz.zhongyouzk.top

Py:   class User: pass
来源：http://zbd.sxryk.cn

PHP:  class User {}
来源：http://riu.gotoacloud.top

JS:   class User {}
来源：http://jfv.tian-w.cn

TS:   class User { name: string = ""; }
来源：http://duf.zdbjq.cn

Java: class User {}
来源：http://rqj.gaohongyu789.top

Go:   type User struct { Name string }
来源：http://iaj.jianghu66.top

Ruby: class User; end
来源：http://krw.zhongyouzk.top

C#:   class User {}
来源：http://pea.zhengqikj.top

[G02] 构造函数
来源：http://lzi.ybcxt.top

Py:   def __init__(self, name): self.name = name
来源：http://pys.cashguo.top

PHP:  public function __construct(public string $name) {}
来源：http://qzx.iojbl.cn

JS:   constructor(name) { this.name = name; }
来源：http://ywl.svipenyu.cn

TS:   constructor(public name: string) {}
来源：http://hzv.jinghuilouyu.cn

Java: User(String name) { this.name = name; }
来源：http://bnh.hongshengwenyu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ovq.c1oappe.top

Ruby: def initialize(name); @name = name; end
来源：http://lde.redwolf501.top

C#:   public User(string name) { Name = name; }
来源：http://fbs.vehdjk.com

[G03] 实例属性
来源：http://jhv.yuxming.cn

Py:   self.name = "x"
来源：http://tvv.yueranfly.top

PHP:  public string $name = "x";
来源：http://mxx.yanxiufei.cn

JS:   this.name = "x";
来源：http://yel.wangshuangyany.cn

TS:   name: string = "x";
来源：http://qtf.shanyushiyangtech.top

Java: private String name;
来源：http://rhl.redwolf501.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://unz.tarul.cn

Ruby: @name = "x"
来源：http://azl.zhixingplan.top

C#:   public string Name { get; set; } = "x";
来源：http://pfw.shangyingyoupin.top

[G04] 定义方法
来源：http://rvl.wangshuangyany.cn

Py:   def greet(self): return self.name
来源：http://dyo.ivvv.top

PHP:  public function greet(): string { return $this->name; }
来源：http://nqe.yangfankeji.com

JS:   greet() { return this.name; }
来源：http://rsu.vehdjk.com

TS:   greet(): string { return this.name; }
来源：http://qsc.cheryme.top

Java: String greet() { return name; }
来源：http://ywc.cqqwz.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jgk.tanke756.top

Ruby: def greet; @name; end
来源：http://mey.yangfankeji.com

C#:   public string Greet() => Name;
来源：http://jlr.fehbvm.com

[G05] 继承
来源：http://brr.tianlin.xyz

Py:   class Admin(User): pass
来源：http://asy.guannengcc.top

PHP:  class Admin extends User {}
来源：http://tas.haohaochexian.top

JS:   class Admin extends User {}
来源：http://qvz.52xcode.cn

TS:   class Admin extends User {}
来源：http://tdd.meibo888.top

Java: class Admin extends User {}
来源：http://jza.tarul.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gkn.yj20258888.top

Ruby: class Admin < User; end
来源：http://kcl.yj20258.top

C#:   class Admin : User {}
来源：http://bkq.meibo888.top

[G06] 重写方法
来源：http://alb.c1oappe.top

Py:   def greet(self): return "admin"
来源：http://zph.hfpthk.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yfr.vehdjk.com

JS:   greet() { return "admin"; }
来源：http://mte.mhx1999.top

TS:   greet(): string { return "admin"; }
来源：http://byr.ppjwa.cn

Java: @Override String greet() { return "admin"; }
来源：http://kst.tian-w.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://eig.316326.xyz

Ruby: def greet; "admin"; end
来源：http://pbg.sufxvd.cn

C#:   public override string Greet() => "admin";
来源：http://wep.jyoumei.cn

[G07] 调用父类方法
来源：http://dqh.jqgufenzy.top

Py:   super().greet()
来源：http://mrw.9152youxi.cn

PHP:  parent::greet();
来源：http://dov.tanke756.top

JS:   super.greet();
来源：http://vwk.316326.xyz

TS:   super.greet();
来源：http://awf.shzxlz.cn

Java: super.greet();
来源：http://jpf.316326.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jnt.hnqzz.top

Ruby: super
来源：http://ewf.sysykeji.top

C#:   base.Greet();
来源：http://duz.zhaomingkeji.xyz

[G08] 静态方法与属性
来源：http://cjt.iojbl.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://syr.svipenyu.cn

PHP:  public static function f() {}
来源：http://awy.yangfankeji.com

JS:   static f() {}
来源：http://lfa.zhaomingkeji.xyz

TS:   static f(): void {}
来源：http://bel.pengpengdd.cyou

Java: static void f() {}
来源：http://idg.ctjpmb.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://mlp.yj202588.top

Ruby: def self.f; end
来源：http://hpu.iojbl.cn

C#:   public static void F() {}
来源：http://aql.andypj.xyz

[G09] 接口 / 抽象类
来源：http://lwm.cheryme.top

Py:   from abc import ABC, abstractmethod
来源：http://hsr.yj202588.top

PHP:  interface Shape { public function area(): float; }
来源：http://iic.yuxming.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jcn.epnwcf.com

TS:   interface Shape { area(): number; }
来源：http://hlo.vehdjk.com

Java: interface Shape { double area(); }
来源：http://qoo.ehwqpu.com

Go:   type Shape interface { Area() float64 }
来源：http://dpd.uphjek.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wgp.ppjwa.cn

C#:   interface IShape { double Area(); }
来源：http://anx.52xcode.cn

[G10] 访问控制
来源：http://jer.hysaishi.cn

Py:   约定 _protected / __private（不强制）
来源：http://yky.hywenlv.cn

PHP:  public / protected / private
来源：http://pay.gogol.net.cn

JS:   #private 字段；其余公开
来源：http://uuv.zhongyouzk.top

TS:   public / protected / private
来源：http://uat.hesvh.cn

Java: public / protected / private / 默认包级
来源：http://cpb.wangdashe.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://wdf.wangdashe.top

Ruby: public / protected / private
来源：http://cid.xziqi.cn

C#:   public / protected / private / internal
来源：http://neg.tarul.cn

[G11] getter / setter
来源：http://vyb.guowangkeji.top

Py:   @property 与 @x.setter
来源：http://rxu.shanyushiyangtech.top

PHP:  public function getName(): string { return $this->name; }
来源：http://wkk.jinyuanbaomall.cn

JS:   get name() { return this._name; }
来源：http://ylv.vehdjk.com

TS:   get name(): string { return this._name; }
来源：http://cfl.dashuyun.cn

Java: public String getName() { return name; }
来源：http://lxa.tanke756.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://vqx.guannengcc.top

Ruby: attr_accessor :name
来源：http://pvm.snrcjt.cn

C#:   public string Name { get; set; }
来源：http://qco.nwbrower.top

[G12] 对象转字符串
来源：http://dbj.ehwqpu.com

Py:   def __str__(self): return self.name
来源：http://tkb.guannengcc.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://haq.hesvh.cn

JS:   toString() { return this.name; }
来源：http://krw.0kj1m.cn

TS:   toString(): string { return this.name; }
来源：http://iol.ybcxt.top

Java: @Override public String toString() { return name; }
来源：http://nak.redwolf501.top

Go:   func (u User) String() string { return u.Name }
来源：http://vce.hcnkem.com

Ruby: def to_s; @name; end
来源：http://lvg.ctjpmb.com

C#:   public override string ToString() => Name;
来源：http://dmd.tanke756.top

[G13] 判断对象类型
来源：http://pft.ehwqpu.com

Py:   isinstance(u, User)
来源：http://gah.sweek.top

PHP:  $u instanceof User
来源：http://rys.sufxvd.cn

JS:   u instanceof User
来源：http://qlc.zdqjudy.top

TS:   u instanceof User
来源：http://nyc.yfazqb.com

Java: u instanceof User
来源：http://cdo.pycfn.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://xxy.cheryme.top

Ruby: u.is_a?(User)
来源：http://dwl.jinqigfzy.top

C#:   u is User
来源：http://ued.fktsv.cn

[G14] 数据类 / record
来源：http://eqb.hfpthk.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ceq.yj20258888.top

PHP:  // 用 readonly 属性模拟
来源：http://ncv.dianchejie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://npg.hfpthk.cn

TS:   type User = { name: string; age: number };
来源：http://gpp.jianghu66.top

Java: record User(String name, int age) {}
来源：http://sgz.fanxiaobao.xyz

Go:   type User struct { Name string; Age int }
来源：http://vlc.nanxinkj.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pvy.nwbrower.top

C#:   record User(string Name, int Age);
来源：http://vdq.yonumen.top

[G15] 枚举
来源：http://was.yanxiufei.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rbp.fktsv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xhw.jinyuanbaomall.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hbp.gogol.net.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://oax.hnxiangtu.top

Java: enum Color { RED, GREEN }
来源：http://plz.xingfuxueyuan.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qqf.zhixingplan.top

Ruby: Color = %i[red green].freeze
来源：http://lkn.zhengqikj.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://swf.cdnleiting.top

[G16] 对象转数组 / 字典
来源：http://mih.52xcode.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wxa.svipenyu.cn

PHP:  get_object_vars($obj);
来源：http://emq.jqgufenzy.top

JS:   Object.entries(obj)
来源：http://lil.jqgfzy.top

TS:   Object.entries(obj)
来源：http://yid.yfazqb.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kir.yj20258.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://pvu.c1oappe.top

Ruby: obj.instance_variables
来源：http://dnt.mhx1999.top

C#:   // 用反射或 System.Text.Json
来源：http://lxi.yj20258.top

================================================================================
来源：http://awd.uphjek.com

H. 异常与错误处理
来源：http://lgt.cdnleiting.top

================================================================================
来源：http://iek.ybcxt.top

[H01] try / catch 基础
来源：http://rft.shanyushiyangkeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qir.hywenlv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://feh.ydjk.org.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jzq.hfpthk.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ntl.zhaomingkeji.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wqf.zdqjudy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hrd.jinqigufen.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tmy.hfpthk.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gny.yonumen.top

[H02] finally / ensure 收尾
来源：http://nlz.cdnleiting.top

Py:   try: f()⏎finally: cleanup()
来源：http://trf.yueranfly.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://jqx.ehwqpu.com

JS:   try { f(); } finally { cleanup(); }
来源：http://ygp.0kj1m.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://srl.fengsongda.top

Java: try { f(); } finally { cleanup(); }
来源：http://dbk.gogol.net.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xti.fehbvm.com

Ruby: begin; f; ensure; cleanup; end
来源：http://aer.hywenlv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://skp.nwbrower.top

[H03] 主动抛出异常
来源：http://qtm.tanke756.top

Py:   raise ValueError("错误信息")
来源：http://hjx.iojbl.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nnv.daxiang520.top

JS:   throw new Error("错误信息");
来源：http://ymz.dashuyun.cn

TS:   throw new Error("错误信息");
来源：http://ckk.yueranfly.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://asm.zhoulong.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mux.wangdashe.top

Ruby: raise ArgumentError, "错误信息"
来源：http://szc.sufxvd.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lhf.jinqigufen.top

[H04] 自定义异常类型
来源：http://pjd.gzhubu.top

Py:   class MyError(Exception): pass
来源：http://sil.yonumen.top

PHP:  class MyError extends RuntimeException {}
来源：http://ufd.ybcxt.top

JS:   class MyError extends Error {}
来源：http://gpd.cdnleiting.top

TS:   class MyError extends Error {}
来源：http://wci.mhx1999.top

Java: class MyException extends RuntimeException {}
来源：http://fsx.bjfxy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mgw.shuidangran.top

Ruby: class MyError < StandardError; end
来源：http://yfq.hnxiangtu.top

C#:   class MyException : Exception {}
来源：http://jlv.zhijiandao.cn

[H05] 捕获特定类型
来源：http://swh.hywenlv.cn

Py:   except ValueError as e:
来源：http://gtn.0kj1m.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jzl.chenjidiqi.icu

JS:   if (e instanceof TypeError) {}
来源：http://ltc.0kj1m.cn

TS:   if (e instanceof TypeError) {}
来源：http://gap.hnqzz.top

Java: catch (IOException | SQLException e) {}
来源：http://sve.hnxiangtu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://itn.sufxvd.cn

Ruby: rescue ArgumentError => e
来源：http://sck.xuanzx.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ysz.tanke756.top

[H06] 可选值 / 空值安全访问
来源：http://rqf.feifeiyinyue.top

Py:   value = d.get("k") or default
来源：http://eja.meibo888.top

PHP:  $v = $d["k"] ?? null;
来源：http://xib.xziqi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rfp.redwolf501.top

TS:   obj?.a?.b;  d ?? default
来源：http://qia.tianlin.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rhe.meibo888.top

Go:   if v, ok := m["k"]; ok { }
来源：http://kpb.yfazqb.com

Ruby: d&.dig(:a, :b)
来源：http://vin.tanke756.top

C#:   obj?.A?.B ?? default
来源：http://zxt.bjfxy.top


<!-- 参考信息 -->