代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aoz.fanxiaobao.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zgt.smart0.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://iee.hysaishi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gcu.yj202588.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dmy.epnwcf.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ydt.aibaodan.cn

[F03] 写入文件（覆盖）
来源：http://jyr.zhoulong.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ewi.cdnleiting.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://cuh.sufxvd.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pub.jinqigufen.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://swb.zhaomingkeji.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jng.sysykeji.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mmz.wangdashe.top

Ruby: File.write("a.txt", "hi")
来源：http://psy.jinyuanbaomall.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cgp.gaohongyu789.top

[F04] 追加写入文件
来源：http://jly.haohaochexian.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wkg.daxiang520.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vzo.quarkkingdee.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xmp.fehbvm.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yok.xingfuxueyuan.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vlh.ehwqpu.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bsc.ppjwa.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ott.yj20258888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uag.haohaochexian.top

[F05] 判断文件或目录是否存在
来源：http://izd.yuxming.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lst.jiagoushi.top

PHP:  file_exists("a.txt");
来源：http://dqb.bjfxy.top

JS:   fs.existsSync("a.txt")
来源：http://dfo.xuanzx.com

TS:   fs.existsSync("a.txt")
来源：http://ghc.fehbvm.com

Java: Files.exists(Path.of("a.txt"))
来源：http://kcp.jinqigfzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rzh.sweek.top

Ruby: File.exist?("a.txt")
来源：http://ryo.zhixingplan.top

C#:   File.Exists("a.txt")
来源：http://pzj.wangshuangyany.cn

[F06] 删除文件
来源：http://xdo.9152youxi.cn

Py:   os.remove("a.txt")
来源：http://mgz.hongshengwenyu.top

PHP:  unlink("a.txt");
来源：http://gnn.shuidangran.top

JS:   fs.unlinkSync("a.txt")
来源：http://pae.xuanzx.com

TS:   fs.unlinkSync("a.txt")
来源：http://xwg.kuanghao11.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rxb.smart0.xyz

Go:   os.Remove("a.txt")
来源：http://xww.cqqwz.cn

Ruby: File.delete("a.txt")
来源：http://hrz.sxryk.cn

C#:   File.Delete("a.txt");
来源：http://bgd.zhixingplan.top

[F07] 创建目录（含多级）
来源：http://ncp.tarul.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jpv.jiagoushi.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jcd.fehbvm.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xnw.xziqi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wlu.zhijiandao.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://phd.9152youxi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gvj.hcnkem.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://olf.zhoulong.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mhj.chenjidiqi.icu

[F08] 遍历目录
来源：http://dzv.sxryk.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://nki.yueranfly.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wmg.jyoumei.cn

JS:   fs.readdirSync("dir")
来源：http://xtk.hcnkem.com

TS:   fs.readdirSync("dir")
来源：http://qqk.meibo888.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mdm.jqgfzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://vnt.xylfe.cn

Ruby: Dir.children("dir")
来源：http://gcp.guannengcc.top

C#:   Directory.GetFiles("dir")
来源：http://dhr.dashuyun.cn

[F09] 获取文件大小
来源：http://mln.fehbvm.com

Py:   os.path.getsize("a.txt")
来源：http://vgz.fktsv.cn

PHP:  filesize("a.txt");
来源：http://wvf.fengsongda.top

JS:   fs.statSync("a.txt").size
来源：http://srz.zhijiandao.cn

TS:   fs.statSync("a.txt").size
来源：http://iju.jinyuanbaomall.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rfe.vqdsnc.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://eci.pycfn.com

Ruby: File.size("a.txt")
来源：http://xlt.shzxlz.cn

C#:   new FileInfo("a.txt").Length
来源：http://jux.nwbrower.top

[F10] 取文件扩展名 / 文件名
来源：http://pke.smart0.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kni.316326.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://iax.sweek.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://emi.shanyushiyangtech.top

TS:   path.extname("a.txt")
来源：http://qzn.tianlin.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tau.chenzaomai.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nhc.zhiwuduotai.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://efi.jianghu66.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jmu.ybcxt.top

[F11] 复制与移动文件
来源：http://ixu.meibo888.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tpy.tianlin.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ckf.jqgfzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hju.52xcode.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fjv.chenjidiqi.icu

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gty.quarkkingdee.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wzv.vqdsnc.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gmz.daxiang520.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tyl.dashuyun.cn

[F12] CSV 读写
来源：http://xgi.sufxvd.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tsn.yongpay.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gmd.redwolf501.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fwf.hnqzz.top

TS:   // 同上
来源：http://qer.fanxiaobao.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ack.fanxiaobao.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wxo.yj202588.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hia.sjlbkw.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tqe.zhijiandao.cn

================================================================================
来源：http://ulo.dianchejie.cn

G. 面向对象
来源：http://gud.hnxiangtu.top

================================================================================
来源：http://nge.chenzaomai.com

[G01] 定义类
来源：http://uxc.jinghuilouyu.cn

Py:   class User: pass
来源：http://kip.ydzc1.top

PHP:  class User {}
来源：http://oow.yuxming.cn

JS:   class User {}
来源：http://xko.sxryk.cn

TS:   class User { name: string = ""; }
来源：http://mqk.xinyue.icu

Java: class User {}
来源：http://rgy.andypj.xyz

Go:   type User struct { Name string }
来源：http://lve.jqgufenzy.top

Ruby: class User; end
来源：http://zld.pengpengdd.cyou

C#:   class User {}
来源：http://qpf.hysaishi.cn

[G02] 构造函数
来源：http://txt.ywan-chungtsiang.top

Py:   def __init__(self, name): self.name = name
来源：http://asf.hnqzz.top

PHP:  public function __construct(public string $name) {}
来源：http://thg.nanxinkj.top

JS:   constructor(name) { this.name = name; }
来源：http://olf.iojbl.cn

TS:   constructor(public name: string) {}
来源：http://mcv.zhijiandao.cn

Java: User(String name) { this.name = name; }
来源：http://dnd.nanxuanxn.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kde.zhongyouzk.top

Ruby: def initialize(name); @name = name; end
来源：http://rjp.jqgufenzy.top

C#:   public User(string name) { Name = name; }
来源：http://gta.jinghuilouyu.cn

[G03] 实例属性
来源：http://uzd.yj20258.top

Py:   self.name = "x"
来源：http://nph.dianchejie.cn

PHP:  public string $name = "x";
来源：http://gjl.pycfn.com

JS:   this.name = "x";
来源：http://fqt.tianlin.xyz

TS:   name: string = "x";
来源：http://tpc.ehwqpu.com

Java: private String name;
来源：http://rbc.jqgfzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rhn.sxryk.cn

Ruby: @name = "x"
来源：http://bco.cashguo.top

C#:   public string Name { get; set; } = "x";
来源：http://lfs.chenzaomai.com

[G04] 定义方法
来源：http://axg.zhixingplan.top

Py:   def greet(self): return self.name
来源：http://yro.yongpay.top

PHP:  public function greet(): string { return $this->name; }
来源：http://caq.sufxvd.cn

JS:   greet() { return this.name; }
来源：http://bds.yonumen.top

TS:   greet(): string { return this.name; }
来源：http://qfz.epnwcf.com

Java: String greet() { return name; }
来源：http://dab.sweek.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://odm.ctjpmb.com

Ruby: def greet; @name; end
来源：http://kmk.zhiwuduotai.top

C#:   public string Greet() => Name;
来源：http://atu.aizwys.cn

[G05] 继承
来源：http://mcp.0kj1m.cn

Py:   class Admin(User): pass
来源：http://riz.hywenlv.cn

PHP:  class Admin extends User {}
来源：http://yuq.gotoacloud.top

JS:   class Admin extends User {}
来源：http://fet.wangdashe.top

TS:   class Admin extends User {}
来源：http://lks.shanyushiyangkeji.top

Java: class Admin extends User {}
来源：http://zgh.zhaomingkeji.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://axl.uphjek.com

Ruby: class Admin < User; end
来源：http://nxu.yj20258888.top

C#:   class Admin : User {}
来源：http://yum.zdqjudy.top

[G06] 重写方法
来源：http://ysx.tianlin.xyz

Py:   def greet(self): return "admin"
来源：http://ryl.shuidangran.top

PHP:  public function greet(): string { return "admin"; }
来源：http://wkk.sjlbkw.cn

JS:   greet() { return "admin"; }
来源：http://kdu.dashuyun.cn

TS:   greet(): string { return "admin"; }
来源：http://fdk.ppjwa.cn

Java: @Override String greet() { return "admin"; }
来源：http://yqt.cqqwz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qmm.haohaochexian.top

Ruby: def greet; "admin"; end
来源：http://hnu.guowangkeji.top

C#:   public override string Greet() => "admin";
来源：http://kkn.gaohongyu789.top

[G07] 调用父类方法
来源：http://zec.jlsjyb.cn

Py:   super().greet()
来源：http://svz.tanke756.top

PHP:  parent::greet();
来源：http://eqi.daria6918.cn

JS:   super.greet();
来源：http://ndd.hesvh.cn

TS:   super.greet();
来源：http://xyy.tian-w.cn

Java: super.greet();
来源：http://hgv.yj20258.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://igb.bbcook.cn

Ruby: super
来源：http://zmv.xuanzx.com

C#:   base.Greet();
来源：http://dzm.9152youxi.cn

[G08] 静态方法与属性
来源：http://cde.tian-w.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rzk.yuanzhike.top

PHP:  public static function f() {}
来源：http://qvj.daxiang520.top

JS:   static f() {}
来源：http://gjz.zdbjq.cn

TS:   static f(): void {}
来源：http://hld.zhiwuduotai.top

Java: static void f() {}
来源：http://qdi.wangdashe.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://nsl.hcnkem.com

Ruby: def self.f; end
来源：http://vxm.haohaochexian.top

C#:   public static void F() {}
来源：http://dxy.9152youxi.cn

[G09] 接口 / 抽象类
来源：http://uai.xuetiantiany.cn

Py:   from abc import ABC, abstractmethod
来源：http://ini.hcnkem.com

PHP:  interface Shape { public function area(): float; }
来源：http://mjs.shzxlz.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://gix.jianghu66.top

TS:   interface Shape { area(): number; }
来源：http://ruq.shzxlz.cn

Java: interface Shape { double area(); }
来源：http://oux.ywan-chungtsiang.top

Go:   type Shape interface { Area() float64 }
来源：http://rmt.shangyingyoupin.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fpu.chenlongwang.top

C#:   interface IShape { double Area(); }
来源：http://edg.ctjpmb.com

[G10] 访问控制
来源：http://pmu.sxryk.cn

Py:   约定 _protected / __private（不强制）
来源：http://zqk.jinqigufen.top

PHP:  public / protected / private
来源：http://oav.fengsongda.top

JS:   #private 字段；其余公开
来源：http://pso.aizwys.cn

TS:   public / protected / private
来源：http://fhz.guannengcc.top

Java: public / protected / private / 默认包级
来源：http://kle.ybcxt.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ufb.zycfv.cn

Ruby: public / protected / private
来源：http://qjz.guannengcc.top

C#:   public / protected / private / internal
来源：http://ofw.zhongyouzk.top

[G11] getter / setter
来源：http://icv.xingfuxueyuan.xyz

Py:   @property 与 @x.setter
来源：http://azv.jyoumei.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ukk.xziqi.cn

JS:   get name() { return this._name; }
来源：http://ixi.daxiang520.top

TS:   get name(): string { return this._name; }
来源：http://kyr.epnwcf.com

Java: public String getName() { return name; }
来源：http://twf.ppjwa.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ybv.quarkkingdee.top

Ruby: attr_accessor :name
来源：http://jxy.yanxiufei.cn

C#:   public string Name { get; set; }
来源：http://bsw.guannengcc.top

[G12] 对象转字符串
来源：http://jam.smart0.xyz

Py:   def __str__(self): return self.name
来源：http://yap.hnxiangtu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://gmp.chenlongwang.top

JS:   toString() { return this.name; }
来源：http://nxl.hammf.cn

TS:   toString(): string { return this.name; }
来源：http://eyq.snrcjt.cn

Java: @Override public String toString() { return name; }
来源：http://nev.c1oappe.top

Go:   func (u User) String() string { return u.Name }
来源：http://nem.hywenlv.cn

Ruby: def to_s; @name; end
来源：http://upg.zycfv.cn

C#:   public override string ToString() => Name;
来源：http://zld.0kj1m.cn

[G13] 判断对象类型
来源：http://fux.sweek.top

Py:   isinstance(u, User)
来源：http://dla.xingfuxueyuan.xyz

PHP:  $u instanceof User
来源：http://efq.ydjk.org.cn

JS:   u instanceof User
来源：http://nrx.316326.xyz

TS:   u instanceof User
来源：http://ppo.andypj.xyz

Java: u instanceof User
来源：http://cav.chenjidiqi.icu

Go:   u, ok := v.(User)            // 类型断言
来源：http://hwq.dianchejie.cn

Ruby: u.is_a?(User)
来源：http://zrn.quarkkingdee.top

C#:   u is User
来源：http://vta.hywenlv.cn

[G14] 数据类 / record
来源：http://clo.zhiwuduotai.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ivs.aizwys.cn

PHP:  // 用 readonly 属性模拟
来源：http://mez.vqdsnc.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vml.cqqwz.cn

TS:   type User = { name: string; age: number };
来源：http://iaq.ehwqpu.com

Java: record User(String name, int age) {}
来源：http://zde.tarul.cn

Go:   type User struct { Name string; Age int }
来源：http://iug.yuxming.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://efp.uphjek.com

C#:   record User(string Name, int Age);
来源：http://tyf.ctjpmb.com

[G15] 枚举
来源：http://ddu.9152youxi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mop.hfpthk.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://axs.cheryme.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ciz.yuxming.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rqf.guannengcc.top

Java: enum Color { RED, GREEN }
来源：http://awg.jinqigfzy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dui.guowangkeji.top

Ruby: Color = %i[red green].freeze
来源：http://rrk.zhijiandao.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rgk.pycfn.com

[G16] 对象转数组 / 字典
来源：http://mjj.9152youxi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xbl.chenlongwang.top

PHP:  get_object_vars($obj);
来源：http://rpi.meibo888.top

JS:   Object.entries(obj)
来源：http://mbf.zdqjudy.top

TS:   Object.entries(obj)
来源：http://dzu.shanyushiyangtech.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bdr.fehbvm.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://lxc.sweek.top

Ruby: obj.instance_variables
来源：http://yqa.pycfn.com

C#:   // 用反射或 System.Text.Json
来源：http://oot.zhengqikj.top

================================================================================
来源：http://rho.mhx1999.top

H. 异常与错误处理
来源：http://mbs.yuxming.cn

================================================================================
来源：http://ymq.wangshuangyany.cn

[H01] try / catch 基础
来源：http://vrm.bjfxy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gzz.ywan-chungtsiang.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ddh.yj202588.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vbp.ctjpmb.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://igj.jqgufenzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jfw.hongshengwenyu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://etd.nanxinkj.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://elf.zhengqikj.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lan.fehbvm.com

[H02] finally / ensure 收尾
来源：http://nnk.hongshengwenyu.top

Py:   try: f()⏎finally: cleanup()
来源：http://wce.cheryme.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://swn.shanyushiyangkeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://yao.jinqigfzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ujb.zhongyouzk.top

Java: try { f(); } finally { cleanup(); }
来源：http://zcm.jyoumei.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jxq.cashguo.top

Ruby: begin; f; ensure; cleanup; end
来源：http://jke.9152youxi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ewd.shanyushiyangkeji.top

[H03] 主动抛出异常
来源：http://zss.sweek.top

Py:   raise ValueError("错误信息")
来源：http://qzc.guannengcc.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vuq.dashuyun.cn

JS:   throw new Error("错误信息");
来源：http://lex.sysykeji.top

TS:   throw new Error("错误信息");
来源：http://xmi.fehbvm.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://omw.yangfankeji.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tlm.xuanzx.com

Ruby: raise ArgumentError, "错误信息"
来源：http://cgr.fktsv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wgh.chenlongwang.top

[H04] 自定义异常类型
来源：http://nql.0kj1m.cn

Py:   class MyError(Exception): pass
来源：http://dsz.gaohongyu789.top

PHP:  class MyError extends RuntimeException {}
来源：http://egf.jqgufenzy.top

JS:   class MyError extends Error {}
来源：http://whv.jyoumei.cn

TS:   class MyError extends Error {}
来源：http://ebd.jlsjyb.cn

Java: class MyException extends RuntimeException {}
来源：http://ecq.c1oappe.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jkc.zhongyouzk.top

Ruby: class MyError < StandardError; end
来源：http://ejr.tanke756.top

C#:   class MyException : Exception {}
来源：http://nyf.jinghuilouyu.cn

[H05] 捕获特定类型
来源：http://ojm.chenlongwang.top

Py:   except ValueError as e:
来源：http://wlh.tarul.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://azo.yueranfly.top

JS:   if (e instanceof TypeError) {}
来源：http://oyw.ydjk.org.cn

TS:   if (e instanceof TypeError) {}
来源：http://pbb.yj20258888.top

Java: catch (IOException | SQLException e) {}
来源：http://qhv.fehbvm.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tgd.aibaodan.cn

Ruby: rescue ArgumentError => e
来源：http://ydt.yfazqb.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ywp.jianghu66.top

[H06] 可选值 / 空值安全访问
来源：http://xfx.jianghu66.top

Py:   value = d.get("k") or default
来源：http://tmo.yonumen.top

PHP:  $v = $d["k"] ?? null;
来源：http://ihl.sufxvd.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ncg.shanyushiyangtech.top

TS:   obj?.a?.b;  d ?? default
来源：http://qjy.yuxming.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fqe.hongshengwenyu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://htf.zdbjq.cn

Ruby: d&.dig(:a, :b)
来源：http://mrp.gaohongyu789.top

C#:   obj?.A?.B ?? default
来源：http://kha.iojbl.cn


<!-- 参考信息 -->