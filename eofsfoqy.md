代发 wailian999

[F09] 获取文件大小
来源：http://uhx.ehwqpu.com

Py:   os.path.getsize("a.txt")
来源：http://erf.tian-w.cn

PHP:  filesize("a.txt");
来源：http://egk.yueranfly.top

JS:   fs.statSync("a.txt").size
来源：http://ofd.daria6918.cn

TS:   fs.statSync("a.txt").size
来源：http://ocr.zhengqikj.top

Java: Files.size(Path.of("a.txt"))
来源：http://xzx.52xcode.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://smg.nanxuanxn.top

Ruby: File.size("a.txt")
来源：http://chr.tianlin.xyz

C#:   new FileInfo("a.txt").Length
来源：http://owr.gotoacloud.top

[F10] 取文件扩展名 / 文件名
来源：http://nyb.snrcjt.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zns.meibo888.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mfd.daxiang520.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dpm.wangshuangyany.cn

TS:   path.extname("a.txt")
来源：http://ksd.zhoulong.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wnw.jianghu66.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ytl.shzxlz.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tzy.ydzc1.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zqv.shuidangran.top

[F11] 复制与移动文件
来源：http://mjb.zycfv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ivp.jianghu66.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dyx.nanxinkj.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lcv.uphjek.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nwg.wangshuangyany.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jdi.xingfuxueyuan.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://oro.xziqi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hkz.jqgfzy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nod.hnxiangtu.top

[F12] CSV 读写
来源：http://elz.zdbjq.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://svj.xuetiantiany.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://udo.yonumen.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vsg.chenlongwang.top

TS:   // 同上
来源：http://ptp.gotoacloud.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://npz.hywenlv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://osc.jianghu66.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vvb.snrcjt.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://jea.redwolf501.top

================================================================================
来源：http://xle.zycfv.cn

G. 面向对象
来源：http://nha.tarul.cn

================================================================================
来源：http://xgf.uphjek.com

[G01] 定义类
来源：http://bbx.dashuyun.cn

Py:   class User: pass
来源：http://vpy.chenlongwang.top

PHP:  class User {}
来源：http://dnk.zycfv.cn

JS:   class User {}
来源：http://knp.dashuyun.cn

TS:   class User { name: string = ""; }
来源：http://hts.sysykeji.top

Java: class User {}
来源：http://shb.tanke756.top

Go:   type User struct { Name string }
来源：http://kru.zhijiandao.cn

Ruby: class User; end
来源：http://dbu.jinqigufen.top

C#:   class User {}
来源：http://swz.yuxming.cn

[G02] 构造函数
来源：http://qnp.jinghuilouyu.cn

Py:   def __init__(self, name): self.name = name
来源：http://pfu.hcnkem.com

PHP:  public function __construct(public string $name) {}
来源：http://pwf.smart0.xyz

JS:   constructor(name) { this.name = name; }
来源：http://tke.zhaomingkeji.xyz

TS:   constructor(public name: string) {}
来源：http://rgd.yvedp.cn

Java: User(String name) { this.name = name; }
来源：http://wjy.shuidangran.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yqv.sweek.top

Ruby: def initialize(name); @name = name; end
来源：http://tdg.ydzc1.top

C#:   public User(string name) { Name = name; }
来源：http://wry.hnxiangtu.top

[G03] 实例属性
来源：http://vmp.jinghuilouyu.cn

Py:   self.name = "x"
来源：http://nob.zhoulong.xyz

PHP:  public string $name = "x";
来源：http://yka.shangyingyoupin.top

JS:   this.name = "x";
来源：http://srg.haohaochexian.top

TS:   name: string = "x";
来源：http://vvj.zhixingplan.top

Java: private String name;
来源：http://bkp.daxiang520.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rph.hongshengwenyu.top

Ruby: @name = "x"
来源：http://bzo.xuanzx.com

C#:   public string Name { get; set; } = "x";
来源：http://wbj.fehbvm.com

[G04] 定义方法
来源：http://wkc.sxryk.cn

Py:   def greet(self): return self.name
来源：http://zpe.dianchejie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ulx.nwbrower.top

JS:   greet() { return this.name; }
来源：http://lkj.yj20258888.top

TS:   greet(): string { return this.name; }
来源：http://ggp.fanxiaobao.xyz

Java: String greet() { return name; }
来源：http://psb.mhx1999.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://lkp.dianchejie.cn

Ruby: def greet; @name; end
来源：http://phj.nanxinkj.top

C#:   public string Greet() => Name;
来源：http://jfz.kuanghao11.cn

[G05] 继承
来源：http://vuu.nanxinkj.top

Py:   class Admin(User): pass
来源：http://dia.yueranfly.top

PHP:  class Admin extends User {}
来源：http://ajw.yangfankeji.com

JS:   class Admin extends User {}
来源：http://ozn.52xcode.cn

TS:   class Admin extends User {}
来源：http://uft.jqgfzy.top

Java: class Admin extends User {}
来源：http://ljk.zhaomingkeji.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gtv.sweek.top

Ruby: class Admin < User; end
来源：http://vrq.svipenyu.cn

C#:   class Admin : User {}
来源：http://ojc.yj20258.top

[G06] 重写方法
来源：http://oaq.gogol.net.cn

Py:   def greet(self): return "admin"
来源：http://itc.aizwys.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nbl.vqdsnc.cn

JS:   greet() { return "admin"; }
来源：http://mpn.zhaomingkeji.xyz

TS:   greet(): string { return "admin"; }
来源：http://wlr.ehwqpu.com

Java: @Override String greet() { return "admin"; }
来源：http://oop.sjlbkw.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://met.52xcode.cn

Ruby: def greet; "admin"; end
来源：http://sus.jqgfzy.top

C#:   public override string Greet() => "admin";
来源：http://zig.sweek.top

[G07] 调用父类方法
来源：http://svw.jyoumei.cn

Py:   super().greet()
来源：http://zwg.yvedp.cn

PHP:  parent::greet();
来源：http://mii.jinyuanbaomall.cn

JS:   super.greet();
来源：http://slj.hnxiangtu.top

TS:   super.greet();
来源：http://elc.ehwqpu.com

Java: super.greet();
来源：http://dzz.zhaomingkeji.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zeb.shzxlz.cn

Ruby: super
来源：http://fkh.fanxiaobao.xyz

C#:   base.Greet();
来源：http://olb.haohaochexian.top

[G08] 静态方法与属性
来源：http://ohf.mhx1999.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vku.jlsjyb.cn

PHP:  public static function f() {}
来源：http://mlk.yuanzhike.top

JS:   static f() {}
来源：http://akd.shanyushiyangkeji.top

TS:   static f(): void {}
来源：http://ito.hywenlv.cn

Java: static void f() {}
来源：http://ygx.xziqi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ocr.gzhubu.top

Ruby: def self.f; end
来源：http://ctc.gzhubu.top

C#:   public static void F() {}
来源：http://cty.cashguo.top

[G09] 接口 / 抽象类
来源：http://umr.gzhubu.top

Py:   from abc import ABC, abstractmethod
来源：http://sqp.havefunace.top

PHP:  interface Shape { public function area(): float; }
来源：http://dsm.fzhhl.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://opn.jinghuilouyu.cn

TS:   interface Shape { area(): number; }
来源：http://smo.cdnleiting.top

Java: interface Shape { double area(); }
来源：http://yxi.yanxiufei.cn

Go:   type Shape interface { Area() float64 }
来源：http://dau.gzhubu.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wxa.wangdashe.top

C#:   interface IShape { double Area(); }
来源：http://peq.nanxuanxn.top

[G10] 访问控制
来源：http://tqx.gogol.net.cn

Py:   约定 _protected / __private（不强制）
来源：http://vue.svipenyu.cn

PHP:  public / protected / private
来源：http://jsn.0kj1m.cn

JS:   #private 字段；其余公开
来源：http://vkg.epnwcf.com

TS:   public / protected / private
来源：http://unh.yuanzhike.top

Java: public / protected / private / 默认包级
来源：http://kbe.tian-w.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://wst.wangdashe.top

Ruby: public / protected / private
来源：http://ddj.yfazqb.com

C#:   public / protected / private / internal
来源：http://fdl.daria6918.cn

[G11] getter / setter
来源：http://wfa.daxiang520.top

Py:   @property 与 @x.setter
来源：http://urm.fehbvm.com

PHP:  public function getName(): string { return $this->name; }
来源：http://tvc.ywan-chungtsiang.top

JS:   get name() { return this._name; }
来源：http://jpw.shangyingyoupin.top

TS:   get name(): string { return this._name; }
来源：http://mis.zhongyouzk.top

Java: public String getName() { return name; }
来源：http://mdw.cashguo.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://njo.cdnleiting.top

Ruby: attr_accessor :name
来源：http://lez.meibo888.top

C#:   public string Name { get; set; }
来源：http://jcu.zdbjq.cn

[G12] 对象转字符串
来源：http://ssu.pengpengdd.cyou

Py:   def __str__(self): return self.name
来源：http://hte.fehbvm.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://sws.pycfn.com

JS:   toString() { return this.name; }
来源：http://inh.jianghu66.top

TS:   toString(): string { return this.name; }
来源：http://yud.daria6918.cn

Java: @Override public String toString() { return name; }
来源：http://zsj.jqgufenzy.top

Go:   func (u User) String() string { return u.Name }
来源：http://ksl.fanxiaobao.xyz

Ruby: def to_s; @name; end
来源：http://yhp.hnqzz.top

C#:   public override string ToString() => Name;
来源：http://fbv.tian-w.cn

[G13] 判断对象类型
来源：http://mpb.jinyuanbaomall.cn

Py:   isinstance(u, User)
来源：http://vkc.shanyushiyangtech.top

PHP:  $u instanceof User
来源：http://iqm.xingfuxueyuan.xyz

JS:   u instanceof User
来源：http://vks.pengpengdd.cyou

TS:   u instanceof User
来源：http://vvr.zhaomingkeji.xyz

Java: u instanceof User
来源：http://kmf.ybcxt.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://gte.xziqi.cn

Ruby: u.is_a?(User)
来源：http://mmg.gzhubu.top

C#:   u is User
来源：http://pfp.xingfuxueyuan.xyz

[G14] 数据类 / record
来源：http://ror.jqgfzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jhs.yfazqb.com

PHP:  // 用 readonly 属性模拟
来源：http://rju.hesvh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://egg.jyoumei.cn

TS:   type User = { name: string; age: number };
来源：http://qls.shzxlz.cn

Java: record User(String name, int age) {}
来源：http://zns.tian-w.cn

Go:   type User struct { Name string; Age int }
来源：http://drp.cheryme.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lpf.jinqigfzy.top

C#:   record User(string Name, int Age);
来源：http://zli.bbcook.cn

[G15] 枚举
来源：http://zdy.hfpthk.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qff.zhaomingkeji.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://xbb.kuanghao11.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zvv.feifeiyinyue.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qmb.cucudq.cn

Java: enum Color { RED, GREEN }
来源：http://voq.jqgfzy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bgr.aibaodan.cn

Ruby: Color = %i[red green].freeze
来源：http://rst.hcnkem.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://aiq.gaohongyu789.top

[G16] 对象转数组 / 字典
来源：http://eaz.0kj1m.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mxi.daria6918.cn

PHP:  get_object_vars($obj);
来源：http://ggv.ivvv.top

JS:   Object.entries(obj)
来源：http://nvv.jinghuilouyu.cn

TS:   Object.entries(obj)
来源：http://cpn.smart0.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ofz.jinqigufen.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://wpd.dashuyun.cn

Ruby: obj.instance_variables
来源：http://syh.daxiang520.top

C#:   // 用反射或 System.Text.Json
来源：http://fpw.wangdashe.top

================================================================================
来源：http://ynw.sjlbkw.cn

H. 异常与错误处理
来源：http://syr.hnqzz.top

================================================================================
来源：http://wap.chenzaomai.com

[H01] try / catch 基础
来源：http://iri.xuanzx.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xua.guowangkeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vxc.vehdjk.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jny.aibaodan.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mye.cdnleiting.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://epp.cdnleiting.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vmc.guowangkeji.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bfc.haohaochexian.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kow.zycfv.cn

[H02] finally / ensure 收尾
来源：http://azo.birdmap.top

Py:   try: f()⏎finally: cleanup()
来源：http://rze.fanxiaobao.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://uge.jiagoushi.top

JS:   try { f(); } finally { cleanup(); }
来源：http://gjq.xylfe.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://hcc.gotoacloud.top

Java: try { f(); } finally { cleanup(); }
来源：http://fsv.guowangkeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://tef.vehdjk.com

Ruby: begin; f; ensure; cleanup; end
来源：http://imz.yongpay.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://vkn.hesvh.cn

[H03] 主动抛出异常
来源：http://txu.fanxiaobao.xyz

Py:   raise ValueError("错误信息")
来源：http://cnh.zhaomingkeji.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pnk.guannengcc.top

JS:   throw new Error("错误信息");
来源：http://dhs.xziqi.cn

TS:   throw new Error("错误信息");
来源：http://mhx.dianchejie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://eut.pycfn.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://byt.redwolf501.top

Ruby: raise ArgumentError, "错误信息"
来源：http://tmb.tian-w.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zre.sysykeji.top

[H04] 自定义异常类型
来源：http://bfe.daxiang520.top

Py:   class MyError(Exception): pass
来源：http://fma.svipenyu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vuq.zhaomingkeji.xyz

JS:   class MyError extends Error {}
来源：http://ohm.birdmap.top

TS:   class MyError extends Error {}
来源：http://soj.shanyushiyangkeji.top

Java: class MyException extends RuntimeException {}
来源：http://msr.shangyingyoupin.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://glo.cucudq.cn

Ruby: class MyError < StandardError; end
来源：http://ysj.fanxiaobao.xyz

C#:   class MyException : Exception {}
来源：http://fso.zdqjudy.top

[H05] 捕获特定类型
来源：http://sih.gaohongyu789.top

Py:   except ValueError as e:
来源：http://aqp.jinyuanbaomall.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ocz.jianghu66.top

JS:   if (e instanceof TypeError) {}
来源：http://wrs.yangfankeji.com

TS:   if (e instanceof TypeError) {}
来源：http://frc.andypj.xyz

Java: catch (IOException | SQLException e) {}
来源：http://low.yuanzhike.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://snf.ydjk.org.cn

Ruby: rescue ArgumentError => e
来源：http://loi.chenzaomai.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dte.jinqigufen.top

[H06] 可选值 / 空值安全访问
来源：http://nyf.zhaomingkeji.xyz

Py:   value = d.get("k") or default
来源：http://ksl.yfazqb.com

PHP:  $v = $d["k"] ?? null;
来源：http://tzh.chenlongwang.top

JS:   obj?.a?.b;  d ?? default
来源：http://emm.shanyushiyangtech.top

TS:   obj?.a?.b;  d ?? default
来源：http://txh.fanxiaobao.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://trx.zhijiandao.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://pwm.zycfv.cn

Ruby: d&.dig(:a, :b)
来源：http://ace.9152youxi.cn

C#:   obj?.A?.B ?? default
来源：http://pwg.bjfxy.top

[H07] 断言
来源：http://fha.xziqi.cn

Py:   assert x > 0, "必须为正"
来源：http://dxm.zhaomingkeji.xyz

PHP:  assert($x > 0);
来源：http://rxy.fengsongda.top

JS:   console.assert(x > 0);
来源：http://lvx.yanxiufei.cn

TS:   console.assert(x > 0);
来源：http://ekw.jqgufenzy.top

Java: assert x > 0 : "必须为正";
来源：http://vpv.shangyingyoupin.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vvn.jiagoushi.top

Ruby: raise "必须为正" unless x > 0
来源：http://mxm.snrcjt.cn

C#:   Debug.Assert(x > 0);
来源：http://apo.tarul.cn

[H08] 获取错误信息与堆栈
来源：http://umk.svipenyu.cn

Py:   str(e);  traceback.format_exc()
来源：http://jky.quarkkingdee.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jdq.nanxuanxn.top

JS:   e.message;  e.stack
来源：http://yem.yuanzhike.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://unq.nwbrower.top

Java: e.getMessage();  e.printStackTrace()
来源：http://maz.zhengqikj.top

Go:   err.Error()
来源：http://hqb.bbcook.cn

Ruby: e.message;  e.backtrace
来源：http://kpu.yj20258.top

C#:   e.Message;  e.StackTrace
来源：http://wqe.dashuyun.cn

[H09] 带错误码的异常
来源：http://kde.xylfe.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wqm.fanxiaobao.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://qgd.ywan-chungtsiang.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ybo.quarkkingdee.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://apc.ehwqpu.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fro.jianghu66.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://amq.guannengcc.top

Ruby: raise MyError.new("fail", 500)
来源：http://zmv.cashguo.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zvh.snrcjt.cn

[H10] 资源自动释放
来源：http://sjw.yj20258888.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://weq.ctjpmb.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lar.tarul.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://odj.zhengqikj.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bke.tianlin.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://aqt.jianghu66.top

Go:   defer f.Close()
来源：http://nrf.yangfankeji.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kkf.sxryk.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ncj.xinyue.icu

================================================================================
来源：http://axs.zhixingplan.top

I. 正则表达式
来源：http://qky.xuanzx.com

================================================================================
来源：http://jzd.yj20258.top

[I01] 判断是否匹配
来源：http://pug.yueranfly.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ihs.jinqigufen.top

PHP:  preg_match('/\d+/', $s);
来源：http://zsd.cashguo.top

JS:   /\d+/.test(s)
来源：http://ygn.pengpengdd.cyou

TS:   /\d+/.test(s)
来源：http://oxh.jyoumei.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ljx.zdqjudy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xek.yj20258.top

Ruby: s.match?(/\d+/)
来源：http://xib.yueranfly.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://czd.ivvv.top

[I02] 提取所有匹配
来源：http://sly.jlsjyb.cn

Py:   re.findall(r"\d+", s)
来源：http://lyz.birdmap.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ypd.fzhhl.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zox.pycfn.com

TS:   s.match(/\d+/g)
来源：http://nmc.iojbl.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pab.zhongyouzk.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://oce.daria6918.cn

Ruby: s.scan(/\d+/)
来源：http://cxk.smart0.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://upv.sysykeji.top

[I03] 提取捕获分组
来源：http://soy.nanxinkj.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yns.hongshengwenyu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ahv.ehwqpu.com


<!-- 参考信息 -->