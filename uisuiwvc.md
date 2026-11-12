代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://xud.zycfv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ybu.jlsjyb.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dua.gzhubu.top

Ruby: File.exist?("a.txt")
来源：http://shr.andypj.xyz

C#:   File.Exists("a.txt")
来源：http://yej.andypj.xyz

[F06] 删除文件
来源：http://mqe.fengsongda.top

Py:   os.remove("a.txt")
来源：http://ugv.nanxuanxn.top

PHP:  unlink("a.txt");
来源：http://pax.xingfuxueyuan.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://gvb.yongpay.top

TS:   fs.unlinkSync("a.txt")
来源：http://pib.sysykeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://djf.jlsjyb.cn

Go:   os.Remove("a.txt")
来源：http://yiy.meibo888.top

Ruby: File.delete("a.txt")
来源：http://lnx.epnwcf.com

C#:   File.Delete("a.txt");
来源：http://rsx.zycfv.cn

[F07] 创建目录（含多级）
来源：http://lbw.sjlbkw.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kvu.jiagoushi.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wqb.zhixingplan.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oqj.fanxiaobao.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://liq.yuxming.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pen.sweek.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gxk.yueranfly.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://huq.jinghuilouyu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qal.xuetiantiany.cn

[F08] 遍历目录
来源：http://tyy.xziqi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ian.bjfxy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://iqk.zycfv.cn

JS:   fs.readdirSync("dir")
来源：http://xil.hnxiangtu.top

TS:   fs.readdirSync("dir")
来源：http://gae.yanxiufei.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ajh.jinyuanbaomall.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jjh.zhixingplan.top

Ruby: Dir.children("dir")
来源：http://xum.316326.xyz

C#:   Directory.GetFiles("dir")
来源：http://zlx.tianlin.xyz

[F09] 获取文件大小
来源：http://kcn.hnqzz.top

Py:   os.path.getsize("a.txt")
来源：http://gxz.zdqjudy.top

PHP:  filesize("a.txt");
来源：http://cyc.shangyingyoupin.top

JS:   fs.statSync("a.txt").size
来源：http://kab.hcnkem.com

TS:   fs.statSync("a.txt").size
来源：http://tnn.ppjwa.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zuw.hywenlv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yft.c1oappe.top

Ruby: File.size("a.txt")
来源：http://orw.sxryk.cn

C#:   new FileInfo("a.txt").Length
来源：http://tek.smart0.xyz

[F10] 取文件扩展名 / 文件名
来源：http://bvh.fanxiaobao.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dzt.xylfe.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ebr.guowangkeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rel.jqgfzy.top

TS:   path.extname("a.txt")
来源：http://qxy.ivvv.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://loo.jianghu66.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://led.daria6918.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://boy.cashguo.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://epx.hywenlv.cn

[F11] 复制与移动文件
来源：http://eul.aizwys.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mjd.cqqwz.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nxu.jyoumei.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fzn.gotoacloud.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nkh.cqqwz.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://huq.xuetiantiany.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zck.jyoumei.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yft.hysaishi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gey.snrcjt.cn

[F12] CSV 读写
来源：http://fev.gzhubu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://stz.fzhhl.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lyy.9152youxi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bwt.guowangkeji.top

TS:   // 同上
来源：http://vlq.guowangkeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vwv.svipenyu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://maa.xylfe.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://daq.fktsv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bgz.cqqwz.cn

================================================================================
来源：http://mig.ivvv.top

G. 面向对象
来源：http://bkl.nanxinkj.top

================================================================================
来源：http://nrl.xingfuxueyuan.xyz

[G01] 定义类
来源：http://hvj.zhoulong.xyz

Py:   class User: pass
来源：http://pqz.gzhubu.top

PHP:  class User {}
来源：http://lvk.snrcjt.cn

JS:   class User {}
来源：http://jux.sweek.top

TS:   class User { name: string = ""; }
来源：http://nik.sufxvd.cn

Java: class User {}
来源：http://bbg.fzhhl.top

Go:   type User struct { Name string }
来源：http://pzc.yuanzhike.top

Ruby: class User; end
来源：http://vkq.jqgfzy.top

C#:   class User {}
来源：http://gui.fengsongda.top

[G02] 构造函数
来源：http://lcb.fktsv.cn

Py:   def __init__(self, name): self.name = name
来源：http://ccj.yuanzhike.top

PHP:  public function __construct(public string $name) {}
来源：http://vgs.smart0.xyz

JS:   constructor(name) { this.name = name; }
来源：http://iaz.uphjek.com

TS:   constructor(public name: string) {}
来源：http://fxv.hnxiangtu.top

Java: User(String name) { this.name = name; }
来源：http://cjw.smart0.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mjs.meibo888.top

Ruby: def initialize(name); @name = name; end
来源：http://iwx.jlsjyb.cn

C#:   public User(string name) { Name = name; }
来源：http://jwy.xingfuxueyuan.xyz

[G03] 实例属性
来源：http://npl.cheryme.top

Py:   self.name = "x"
来源：http://rvf.sufxvd.cn

PHP:  public string $name = "x";
来源：http://vfe.xuetiantiany.cn

JS:   this.name = "x";
来源：http://him.ybcxt.top

TS:   name: string = "x";
来源：http://tfr.sweek.top

Java: private String name;
来源：http://ous.zdbjq.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://akz.xuanzx.com

Ruby: @name = "x"
来源：http://zjy.xziqi.cn

C#:   public string Name { get; set; } = "x";
来源：http://phl.fehbvm.com

[G04] 定义方法
来源：http://dda.jiagoushi.top

Py:   def greet(self): return self.name
来源：http://sxw.xuetiantiany.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://abw.uphjek.com

JS:   greet() { return this.name; }
来源：http://yul.nanxuanxn.top

TS:   greet(): string { return this.name; }
来源：http://xzh.chenjidiqi.icu

Java: String greet() { return name; }
来源：http://vbo.yueranfly.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://gkd.dianchejie.cn

Ruby: def greet; @name; end
来源：http://zqj.0kj1m.cn

C#:   public string Greet() => Name;
来源：http://veg.aibaodan.cn

[G05] 继承
来源：http://dqg.shuidangran.top

Py:   class Admin(User): pass
来源：http://pjg.zhixingplan.top

PHP:  class Admin extends User {}
来源：http://dwq.nanxuanxn.top

JS:   class Admin extends User {}
来源：http://elv.mhx1999.top

TS:   class Admin extends User {}
来源：http://hav.cheryme.top

Java: class Admin extends User {}
来源：http://pyg.jinqigfzy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://whg.redwolf501.top

Ruby: class Admin < User; end
来源：http://wol.hesvh.cn

C#:   class Admin : User {}
来源：http://vsk.jqgfzy.top

[G06] 重写方法
来源：http://zvs.quarkkingdee.top

Py:   def greet(self): return "admin"
来源：http://jxp.ctjpmb.com

PHP:  public function greet(): string { return "admin"; }
来源：http://azz.meibo888.top

JS:   greet() { return "admin"; }
来源：http://eak.shanyushiyangkeji.top

TS:   greet(): string { return "admin"; }
来源：http://enk.fanxiaobao.xyz

Java: @Override String greet() { return "admin"; }
来源：http://sqe.daria6918.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://amr.aizwys.cn

Ruby: def greet; "admin"; end
来源：http://vuv.vehdjk.com

C#:   public override string Greet() => "admin";
来源：http://iug.fanxiaobao.xyz

[G07] 调用父类方法
来源：http://hjs.jinyuanbaomall.cn

Py:   super().greet()
来源：http://fcw.gaohongyu789.top

PHP:  parent::greet();
来源：http://nlg.yj20258.top

JS:   super.greet();
来源：http://kje.jinghuilouyu.cn

TS:   super.greet();
来源：http://ovi.yj20258.top

Java: super.greet();
来源：http://rvr.jlsjyb.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zmt.sufxvd.cn

Ruby: super
来源：http://oss.xylfe.cn

C#:   base.Greet();
来源：http://rso.epnwcf.com

[G08] 静态方法与属性
来源：http://big.xingfuxueyuan.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qph.gzhubu.top

PHP:  public static function f() {}
来源：http://qmg.dianchejie.cn

JS:   static f() {}
来源：http://dfr.jqgufenzy.top

TS:   static f(): void {}
来源：http://loq.chenjidiqi.icu

Java: static void f() {}
来源：http://iyn.fktsv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jvb.52xcode.cn

Ruby: def self.f; end
来源：http://wqz.nanxinkj.top

C#:   public static void F() {}
来源：http://krq.ppjwa.cn

[G09] 接口 / 抽象类
来源：http://fnb.pengpengdd.cyou

Py:   from abc import ABC, abstractmethod
来源：http://enz.jyoumei.cn

PHP:  interface Shape { public function area(): float; }
来源：http://kyw.hammf.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zjr.bjfxy.top

TS:   interface Shape { area(): number; }
来源：http://cuc.quarkkingdee.top

Java: interface Shape { double area(); }
来源：http://ght.haohaochexian.top

Go:   type Shape interface { Area() float64 }
来源：http://acb.dashuyun.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tho.jinqigufen.top

C#:   interface IShape { double Area(); }
来源：http://cof.bjfxy.top

[G10] 访问控制
来源：http://vyf.nanxinkj.top

Py:   约定 _protected / __private（不强制）
来源：http://jqk.iojbl.cn

PHP:  public / protected / private
来源：http://krc.dashuyun.cn

JS:   #private 字段；其余公开
来源：http://drp.jinqigfzy.top

TS:   public / protected / private
来源：http://flp.ydjk.org.cn

Java: public / protected / private / 默认包级
来源：http://ibe.yongpay.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://hxi.guowangkeji.top

Ruby: public / protected / private
来源：http://rkk.xinyue.icu

C#:   public / protected / private / internal
来源：http://lla.xingfuxueyuan.xyz

[G11] getter / setter
来源：http://tlo.ehwqpu.com

Py:   @property 与 @x.setter
来源：http://zbn.andypj.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://zwf.fzhhl.top

JS:   get name() { return this._name; }
来源：http://wqg.tian-w.cn

TS:   get name(): string { return this._name; }
来源：http://nma.sysykeji.top

Java: public String getName() { return name; }
来源：http://dqs.zhengqikj.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://vnt.tian-w.cn

Ruby: attr_accessor :name
来源：http://kpo.hfpthk.cn

C#:   public string Name { get; set; }
来源：http://dsk.kuanghao11.cn

[G12] 对象转字符串
来源：http://nhe.cdnleiting.top

Py:   def __str__(self): return self.name
来源：http://bsh.yuanzhike.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://qdd.hysaishi.cn

JS:   toString() { return this.name; }
来源：http://mvd.yanxiufei.cn

TS:   toString(): string { return this.name; }
来源：http://iap.gaohongyu789.top

Java: @Override public String toString() { return name; }
来源：http://ety.tarul.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mhi.bjfxy.top

Ruby: def to_s; @name; end
来源：http://krb.xuanzx.com

C#:   public override string ToString() => Name;
来源：http://gpc.zhijiandao.cn

[G13] 判断对象类型
来源：http://fme.bjfxy.top

Py:   isinstance(u, User)
来源：http://zzt.cucudq.cn

PHP:  $u instanceof User
来源：http://dyu.gzhubu.top

JS:   u instanceof User
来源：http://gko.tianlin.xyz

TS:   u instanceof User
来源：http://qym.havefunace.top

Java: u instanceof User
来源：http://wiq.jqgufenzy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://xae.zhongyouzk.top

Ruby: u.is_a?(User)
来源：http://tqg.andypj.xyz

C#:   u is User
来源：http://esq.xinyue.icu

[G14] 数据类 / record
来源：http://msu.yanxiufei.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://npw.hnxiangtu.top

PHP:  // 用 readonly 属性模拟
来源：http://vlx.yfazqb.com

JS:   // 无内置：普通类或对象字面量
来源：http://yed.feifeiyinyue.top

TS:   type User = { name: string; age: number };
来源：http://leo.jlsjyb.cn

Java: record User(String name, int age) {}
来源：http://akf.sweek.top

Go:   type User struct { Name string; Age int }
来源：http://fkl.yangfankeji.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kad.hywenlv.cn

C#:   record User(string Name, int Age);
来源：http://lpw.jinqigufen.top

[G15] 枚举
来源：http://chx.ivvv.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://byp.xuanzx.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://dtu.ctjpmb.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wtm.jyoumei.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lkm.svipenyu.cn

Java: enum Color { RED, GREEN }
来源：http://emq.ydzc1.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://efd.hfpthk.cn

Ruby: Color = %i[red green].freeze
来源：http://oov.iojbl.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tba.hongshengwenyu.top

[G16] 对象转数组 / 字典
来源：http://meb.guowangkeji.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zrp.tarul.cn

PHP:  get_object_vars($obj);
来源：http://zcp.wangdashe.top

JS:   Object.entries(obj)
来源：http://roq.hysaishi.cn

TS:   Object.entries(obj)
来源：http://lts.yueranfly.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zcs.ydzc1.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ztu.havefunace.top

Ruby: obj.instance_variables
来源：http://mok.hammf.cn

C#:   // 用反射或 System.Text.Json
来源：http://icg.iojbl.cn

================================================================================
来源：http://xpu.smart0.xyz

H. 异常与错误处理
来源：http://dgm.hammf.cn

================================================================================
来源：http://ogw.9152youxi.cn

[H01] try / catch 基础
来源：http://svp.bbcook.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qip.nanxinkj.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xys.yanxiufei.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://klj.epnwcf.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vtw.fzhhl.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bdi.quarkkingdee.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cme.hnxiangtu.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://spl.52xcode.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wry.andypj.xyz

[H02] finally / ensure 收尾
来源：http://uxa.shanyushiyangtech.top

Py:   try: f()⏎finally: cleanup()
来源：http://ono.ivvv.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ciu.quarkkingdee.top

JS:   try { f(); } finally { cleanup(); }
来源：http://adb.aizwys.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qyl.fanxiaobao.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://epm.tian-w.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://syf.cheryme.top

Ruby: begin; f; ensure; cleanup; end
来源：http://tzm.ydjk.org.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rpm.shangyingyoupin.top

[H03] 主动抛出异常
来源：http://efv.zhiwuduotai.top

Py:   raise ValueError("错误信息")
来源：http://zyt.gaohongyu789.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://git.cdnleiting.top

JS:   throw new Error("错误信息");
来源：http://vxd.snrcjt.cn

TS:   throw new Error("错误信息");
来源：http://ldu.zdbjq.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rkw.yuanzhike.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uua.jqgufenzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ciz.redwolf501.top

C#:   throw new ArgumentException("错误信息");
来源：http://grx.jqgfzy.top

[H04] 自定义异常类型
来源：http://gwb.yonumen.top

Py:   class MyError(Exception): pass
来源：http://vvp.shzxlz.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qgg.yonumen.top

JS:   class MyError extends Error {}
来源：http://dnp.yvedp.cn

TS:   class MyError extends Error {}
来源：http://yyz.wangdashe.top

Java: class MyException extends RuntimeException {}
来源：http://iyu.ivvv.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zmu.bbcook.cn

Ruby: class MyError < StandardError; end
来源：http://adx.snrcjt.cn

C#:   class MyException : Exception {}
来源：http://fkp.cheryme.top

[H05] 捕获特定类型
来源：http://gfc.havefunace.top

Py:   except ValueError as e:
来源：http://zww.gogol.net.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uml.dashuyun.cn

JS:   if (e instanceof TypeError) {}
来源：http://fcr.0kj1m.cn

TS:   if (e instanceof TypeError) {}
来源：http://ctc.aibaodan.cn

Java: catch (IOException | SQLException e) {}
来源：http://ael.ehwqpu.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ilb.shuidangran.top

Ruby: rescue ArgumentError => e
来源：http://bmn.0kj1m.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pio.9152youxi.cn

[H06] 可选值 / 空值安全访问
来源：http://mth.nanxuanxn.top

Py:   value = d.get("k") or default
来源：http://fqd.kuanghao11.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ruj.wangdashe.top

JS:   obj?.a?.b;  d ?? default
来源：http://jpd.yuanzhike.top

TS:   obj?.a?.b;  d ?? default
来源：http://bfe.jyoumei.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://atu.cqqwz.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://lms.mhx1999.top

Ruby: d&.dig(:a, :b)
来源：http://uer.aizwys.cn

C#:   obj?.A?.B ?? default
来源：http://uck.shuidangran.top

[H07] 断言
来源：http://rep.birdmap.top

Py:   assert x > 0, "必须为正"
来源：http://jqy.cdnleiting.top

PHP:  assert($x > 0);
来源：http://sev.cheryme.top

JS:   console.assert(x > 0);
来源：http://khc.pengpengdd.cyou

TS:   console.assert(x > 0);
来源：http://rud.epnwcf.com

Java: assert x > 0 : "必须为正";
来源：http://dtb.9152youxi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qne.hnxiangtu.top

Ruby: raise "必须为正" unless x > 0
来源：http://mwd.fzhhl.top

C#:   Debug.Assert(x > 0);
来源：http://pkl.cqqwz.cn

[H08] 获取错误信息与堆栈
来源：http://dwl.yuanzhike.top

Py:   str(e);  traceback.format_exc()
来源：http://wgh.zhaomingkeji.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fyi.shzxlz.cn

JS:   e.message;  e.stack
来源：http://vgf.shanyushiyangkeji.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ojx.vqdsnc.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://lfs.yanxiufei.cn

Go:   err.Error()
来源：http://vtf.vqdsnc.cn

Ruby: e.message;  e.backtrace
来源：http://dvj.yonumen.top

C#:   e.Message;  e.StackTrace
来源：http://oom.kuanghao11.cn

[H09] 带错误码的异常
来源：http://wvp.ppjwa.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gro.snrcjt.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xxw.hysaishi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bui.xuanzx.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cnr.yueranfly.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hie.sjlbkw.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hwp.tarul.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tpy.cheryme.top

C#:   // 自定义异常类中加 Code 属性
来源：http://kre.sweek.top

[H10] 资源自动释放
来源：http://vlf.yvedp.cn


<!-- 参考信息 -->