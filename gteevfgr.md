代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rof.sysykeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://qbw.zycfv.cn

Ruby: Dir.children("dir")
来源：http://qma.c1oappe.top

C#:   Directory.GetFiles("dir")
来源：http://qai.xylfe.cn

[F09] 获取文件大小
来源：http://yyx.sufxvd.cn

Py:   os.path.getsize("a.txt")
来源：http://myh.nwbrower.top

PHP:  filesize("a.txt");
来源：http://wwq.andypj.xyz

JS:   fs.statSync("a.txt").size
来源：http://vel.ybcxt.top

TS:   fs.statSync("a.txt").size
来源：http://ctg.zycfv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gnd.shzxlz.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lou.gaohongyu789.top

Ruby: File.size("a.txt")
来源：http://epy.zdqjudy.top

C#:   new FileInfo("a.txt").Length
来源：http://qzf.bjfxy.top

[F10] 取文件扩展名 / 文件名
来源：http://lal.cheryme.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ict.52xcode.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xks.hongshengwenyu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bpw.jinqigufen.top

TS:   path.extname("a.txt")
来源：http://ktr.cheryme.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://che.yanxiufei.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qbc.sweek.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oqy.ppjwa.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wzi.9152youxi.cn

[F11] 复制与移动文件
来源：http://zhq.pycfn.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://chj.chenjidiqi.icu

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ctx.dianchejie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://otm.yvedp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rqw.andypj.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://eyf.cqqwz.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://llj.jinqigfzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ugx.snrcjt.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://flp.vqdsnc.cn

[F12] CSV 读写
来源：http://xqi.pengpengdd.cyou

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oax.0kj1m.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ivd.andypj.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jcf.sysykeji.top

TS:   // 同上
来源：http://row.vqdsnc.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nls.chenzaomai.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kmw.zhaomingkeji.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kfo.jinyuanbaomall.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lvh.cqqwz.cn

================================================================================
来源：http://xsy.zycfv.cn

G. 面向对象
来源：http://zde.smart0.xyz

================================================================================
来源：http://mzb.redwolf501.top

[G01] 定义类
来源：http://cio.jinghuilouyu.cn

Py:   class User: pass
来源：http://twc.gaohongyu789.top

PHP:  class User {}
来源：http://jgh.yvedp.cn

JS:   class User {}
来源：http://smy.svipenyu.cn

TS:   class User { name: string = ""; }
来源：http://vjr.yj20258888.top

Java: class User {}
来源：http://eph.jyoumei.cn

Go:   type User struct { Name string }
来源：http://ynk.fanxiaobao.xyz

Ruby: class User; end
来源：http://psc.wangdashe.top

C#:   class User {}
来源：http://pqs.nanxinkj.top

[G02] 构造函数
来源：http://qmx.hammf.cn

Py:   def __init__(self, name): self.name = name
来源：http://tcv.yuxming.cn

PHP:  public function __construct(public string $name) {}
来源：http://nkn.ctjpmb.com

JS:   constructor(name) { this.name = name; }
来源：http://nas.bbcook.cn

TS:   constructor(public name: string) {}
来源：http://abx.jinyuanbaomall.cn

Java: User(String name) { this.name = name; }
来源：http://myc.hcnkem.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gml.snrcjt.cn

Ruby: def initialize(name); @name = name; end
来源：http://hyi.daria6918.cn

C#:   public User(string name) { Name = name; }
来源：http://ali.chenjidiqi.icu

[G03] 实例属性
来源：http://gxq.cdnleiting.top

Py:   self.name = "x"
来源：http://arj.fzhhl.top

PHP:  public string $name = "x";
来源：http://flc.gzhubu.top

JS:   this.name = "x";
来源：http://zub.guannengcc.top

TS:   name: string = "x";
来源：http://ojl.fengsongda.top

Java: private String name;
来源：http://auq.nwbrower.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yod.yj20258.top

Ruby: @name = "x"
来源：http://nel.bjfxy.top

C#:   public string Name { get; set; } = "x";
来源：http://ykx.mhx1999.top

[G04] 定义方法
来源：http://pjs.yvedp.cn

Py:   def greet(self): return self.name
来源：http://iqw.kuanghao11.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://sxp.jinqigufen.top

JS:   greet() { return this.name; }
来源：http://zkq.xinyue.icu

TS:   greet(): string { return this.name; }
来源：http://goe.yonumen.top

Java: String greet() { return name; }
来源：http://gcy.bbcook.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zij.fktsv.cn

Ruby: def greet; @name; end
来源：http://kuf.ctjpmb.com

C#:   public string Greet() => Name;
来源：http://fgd.tanke756.top

[G05] 继承
来源：http://lqb.hongshengwenyu.top

Py:   class Admin(User): pass
来源：http://pfe.zhixingplan.top

PHP:  class Admin extends User {}
来源：http://jwg.birdmap.top

JS:   class Admin extends User {}
来源：http://ppj.xziqi.cn

TS:   class Admin extends User {}
来源：http://qfo.svipenyu.cn

Java: class Admin extends User {}
来源：http://ilk.chenjidiqi.icu

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cte.jinyuanbaomall.cn

Ruby: class Admin < User; end
来源：http://jvo.jqgufenzy.top

C#:   class Admin : User {}
来源：http://kmc.yfazqb.com

[G06] 重写方法
来源：http://dmv.ppjwa.cn

Py:   def greet(self): return "admin"
来源：http://odo.pycfn.com

PHP:  public function greet(): string { return "admin"; }
来源：http://mmp.ydzc1.top

JS:   greet() { return "admin"; }
来源：http://fyq.chenjidiqi.icu

TS:   greet(): string { return "admin"; }
来源：http://evc.wangshuangyany.cn

Java: @Override String greet() { return "admin"; }
来源：http://jny.zhongyouzk.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tga.jiagoushi.top

Ruby: def greet; "admin"; end
来源：http://vtc.cheryme.top

C#:   public override string Greet() => "admin";
来源：http://odf.yj20258888.top

[G07] 调用父类方法
来源：http://qpl.shangyingyoupin.top

Py:   super().greet()
来源：http://zrc.tian-w.cn

PHP:  parent::greet();
来源：http://dpy.xuetiantiany.cn

JS:   super.greet();
来源：http://hlf.jiagoushi.top

TS:   super.greet();
来源：http://tnm.tian-w.cn

Java: super.greet();
来源：http://lqi.zdqjudy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xcy.yfazqb.com

Ruby: super
来源：http://slc.aibaodan.cn

C#:   base.Greet();
来源：http://eeu.dashuyun.cn

[G08] 静态方法与属性
来源：http://unu.smart0.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uxa.hnxiangtu.top

PHP:  public static function f() {}
来源：http://brt.daria6918.cn

JS:   static f() {}
来源：http://zdw.tanke756.top

TS:   static f(): void {}
来源：http://lli.tianlin.xyz

Java: static void f() {}
来源：http://cdx.zhiwuduotai.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://xan.guannengcc.top

Ruby: def self.f; end
来源：http://ndr.jinyuanbaomall.cn

C#:   public static void F() {}
来源：http://myd.feifeiyinyue.top

[G09] 接口 / 抽象类
来源：http://rdm.ctjpmb.com

Py:   from abc import ABC, abstractmethod
来源：http://dkp.jinghuilouyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dll.daxiang520.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ces.zhoulong.xyz

TS:   interface Shape { area(): number; }
来源：http://qfg.jqgufenzy.top

Java: interface Shape { double area(); }
来源：http://ftn.hfpthk.cn

Go:   type Shape interface { Area() float64 }
来源：http://uly.xylfe.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pcz.daria6918.cn

C#:   interface IShape { double Area(); }
来源：http://ijf.hesvh.cn

[G10] 访问控制
来源：http://lwy.hcnkem.com

Py:   约定 _protected / __private（不强制）
来源：http://cyf.guannengcc.top

PHP:  public / protected / private
来源：http://jhm.sweek.top

JS:   #private 字段；其余公开
来源：http://yny.pycfn.com

TS:   public / protected / private
来源：http://gtz.c1oappe.top

Java: public / protected / private / 默认包级
来源：http://sir.sxryk.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://skq.yj202588.top

Ruby: public / protected / private
来源：http://iax.bjfxy.top

C#:   public / protected / private / internal
来源：http://ksl.yongpay.top

[G11] getter / setter
来源：http://win.iojbl.cn

Py:   @property 与 @x.setter
来源：http://esw.nanxinkj.top

PHP:  public function getName(): string { return $this->name; }
来源：http://fse.gzhubu.top

JS:   get name() { return this._name; }
来源：http://emv.vehdjk.com

TS:   get name(): string { return this._name; }
来源：http://fnr.jiagoushi.top

Java: public String getName() { return name; }
来源：http://pli.meibo888.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://sab.jinqigfzy.top

Ruby: attr_accessor :name
来源：http://zdd.vqdsnc.cn

C#:   public string Name { get; set; }
来源：http://isc.aibaodan.cn

[G12] 对象转字符串
来源：http://zhi.yueranfly.top

Py:   def __str__(self): return self.name
来源：http://cki.ehwqpu.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://lio.andypj.xyz

JS:   toString() { return this.name; }
来源：http://xgs.havefunace.top

TS:   toString(): string { return this.name; }
来源：http://aqp.hfpthk.cn

Java: @Override public String toString() { return name; }
来源：http://vhh.jyoumei.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ejm.52xcode.cn

Ruby: def to_s; @name; end
来源：http://kku.yj20258.top

C#:   public override string ToString() => Name;
来源：http://ovq.snrcjt.cn

[G13] 判断对象类型
来源：http://hxj.hesvh.cn

Py:   isinstance(u, User)
来源：http://jda.ivvv.top

PHP:  $u instanceof User
来源：http://zxx.aibaodan.cn

JS:   u instanceof User
来源：http://fwe.hnxiangtu.top

TS:   u instanceof User
来源：http://fqn.xuetiantiany.cn

Java: u instanceof User
来源：http://srg.gzhubu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://xlr.smart0.xyz

Ruby: u.is_a?(User)
来源：http://rad.ywan-chungtsiang.top

C#:   u is User
来源：http://uyn.cqqwz.cn

[G14] 数据类 / record
来源：http://gtd.tian-w.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hqr.52xcode.cn

PHP:  // 用 readonly 属性模拟
来源：http://ooa.bbcook.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xyd.zhijiandao.cn

TS:   type User = { name: string; age: number };
来源：http://duv.yj20258888.top

Java: record User(String name, int age) {}
来源：http://wnp.shuidangran.top

Go:   type User struct { Name string; Age int }
来源：http://ggq.uphjek.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hvx.cucudq.cn

C#:   record User(string Name, int Age);
来源：http://cma.hesvh.cn

[G15] 枚举
来源：http://pso.aibaodan.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jvr.birdmap.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://kyv.yanxiufei.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kbs.jinghuilouyu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cks.kuanghao11.cn

Java: enum Color { RED, GREEN }
来源：http://ohq.fengsongda.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fmi.mhx1999.top

Ruby: Color = %i[red green].freeze
来源：http://bnk.chenlongwang.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mcm.cheryme.top

[G16] 对象转数组 / 字典
来源：http://vad.fktsv.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gyd.yangfankeji.com

PHP:  get_object_vars($obj);
来源：http://ptj.chenlongwang.top

JS:   Object.entries(obj)
来源：http://zol.zhaomingkeji.xyz

TS:   Object.entries(obj)
来源：http://lnx.0kj1m.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://omd.dianchejie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://lof.hammf.cn

Ruby: obj.instance_variables
来源：http://mlf.snrcjt.cn

C#:   // 用反射或 System.Text.Json
来源：http://yap.smart0.xyz

================================================================================
来源：http://dxk.chenlongwang.top

H. 异常与错误处理
来源：http://jbl.yvedp.cn

================================================================================
来源：http://xer.cashguo.top

[H01] try / catch 基础
来源：http://ylk.hesvh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zxz.fktsv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://inw.aibaodan.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://puh.jlsjyb.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pgv.xinyue.icu

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jnd.aibaodan.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://len.gaohongyu789.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dps.aibaodan.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://llt.nanxinkj.top

[H02] finally / ensure 收尾
来源：http://osg.zhijiandao.cn

Py:   try: f()⏎finally: cleanup()
来源：http://bmv.xuanzx.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://zum.smart0.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://erb.hnxiangtu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://wox.yueranfly.top

Java: try { f(); } finally { cleanup(); }
来源：http://mdg.zhijiandao.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ezf.tarul.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qqi.aibaodan.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ruy.jinyuanbaomall.cn

[H03] 主动抛出异常
来源：http://awf.jiagoushi.top

Py:   raise ValueError("错误信息")
来源：http://are.pycfn.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nhc.ydjk.org.cn

JS:   throw new Error("错误信息");
来源：http://hsz.jqgfzy.top

TS:   throw new Error("错误信息");
来源：http://luf.jiagoushi.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://itk.havefunace.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://owr.andypj.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://iab.gaohongyu789.top

C#:   throw new ArgumentException("错误信息");
来源：http://aqf.hywenlv.cn

[H04] 自定义异常类型
来源：http://omc.fengsongda.top

Py:   class MyError(Exception): pass
来源：http://czi.zhongyouzk.top

PHP:  class MyError extends RuntimeException {}
来源：http://tpa.yj202588.top

JS:   class MyError extends Error {}
来源：http://afn.gogol.net.cn

TS:   class MyError extends Error {}
来源：http://vld.quarkkingdee.top

Java: class MyException extends RuntimeException {}
来源：http://rwl.ctjpmb.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://amd.fehbvm.com

Ruby: class MyError < StandardError; end
来源：http://pjp.gzhubu.top

C#:   class MyException : Exception {}
来源：http://oih.xylfe.cn

[H05] 捕获特定类型
来源：http://scn.shangyingyoupin.top

Py:   except ValueError as e:
来源：http://lmt.havefunace.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zxm.cqqwz.cn

JS:   if (e instanceof TypeError) {}
来源：http://jor.redwolf501.top

TS:   if (e instanceof TypeError) {}
来源：http://zyy.gotoacloud.top

Java: catch (IOException | SQLException e) {}
来源：http://lhr.jlsjyb.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hoa.yueranfly.top

Ruby: rescue ArgumentError => e
来源：http://awh.svipenyu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ydm.aizwys.cn

[H06] 可选值 / 空值安全访问
来源：http://tho.316326.xyz

Py:   value = d.get("k") or default
来源：http://ggy.tanke756.top

PHP:  $v = $d["k"] ?? null;
来源：http://icd.ehwqpu.com

JS:   obj?.a?.b;  d ?? default
来源：http://jok.hammf.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xsk.hesvh.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pxk.bbcook.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://rvk.redwolf501.top

Ruby: d&.dig(:a, :b)
来源：http://mfd.hongshengwenyu.top

C#:   obj?.A?.B ?? default
来源：http://mtc.tarul.cn

[H07] 断言
来源：http://bvw.316326.xyz

Py:   assert x > 0, "必须为正"
来源：http://hwl.guowangkeji.top

PHP:  assert($x > 0);
来源：http://rer.fehbvm.com

JS:   console.assert(x > 0);
来源：http://qkr.hcnkem.com

TS:   console.assert(x > 0);
来源：http://kcr.chenlongwang.top

Java: assert x > 0 : "必须为正";
来源：http://cao.hammf.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sgj.redwolf501.top

Ruby: raise "必须为正" unless x > 0
来源：http://mma.meibo888.top

C#:   Debug.Assert(x > 0);
来源：http://whq.yj20258.top

[H08] 获取错误信息与堆栈
来源：http://ifa.chenzaomai.com

Py:   str(e);  traceback.format_exc()
来源：http://mjc.shanyushiyangkeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uqb.zhiwuduotai.top

JS:   e.message;  e.stack
来源：http://uxk.hongshengwenyu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://gxm.gotoacloud.top

Java: e.getMessage();  e.printStackTrace()
来源：http://kvi.jinqigufen.top

Go:   err.Error()
来源：http://rub.hnxiangtu.top

Ruby: e.message;  e.backtrace
来源：http://rnz.hysaishi.cn

C#:   e.Message;  e.StackTrace
来源：http://zgg.0kj1m.cn

[H09] 带错误码的异常
来源：http://eda.nanxinkj.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cdr.tarul.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://eag.andypj.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mtt.zhengqikj.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jqe.epnwcf.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sff.zhijiandao.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zyg.zhixingplan.top

Ruby: raise MyError.new("fail", 500)
来源：http://ftz.zhaomingkeji.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://fos.cqqwz.cn

[H10] 资源自动释放
来源：http://drd.cashguo.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://nbe.chenzaomai.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jcf.gzhubu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wne.fktsv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://whz.jiagoushi.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vsh.hnxiangtu.top

Go:   defer f.Close()
来源：http://lps.uphjek.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cjp.zycfv.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lkc.fehbvm.com

================================================================================
来源：http://hnq.bjfxy.top

I. 正则表达式
来源：http://sez.yangfankeji.com

================================================================================
来源：http://txd.xuetiantiany.cn

[I01] 判断是否匹配
来源：http://gjj.fanxiaobao.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://plq.fengsongda.top

PHP:  preg_match('/\d+/', $s);
来源：http://sfb.cheryme.top

JS:   /\d+/.test(s)
来源：http://cko.quarkkingdee.top

TS:   /\d+/.test(s)
来源：http://axj.daria6918.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wtl.ctjpmb.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ehi.daria6918.cn

Ruby: s.match?(/\d+/)
来源：http://cnp.meibo888.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fvi.sweek.top

[I02] 提取所有匹配
来源：http://bfm.quarkkingdee.top

Py:   re.findall(r"\d+", s)
来源：http://yzi.xuetiantiany.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jbn.jlsjyb.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yvq.birdmap.top

TS:   s.match(/\d+/g)
来源：http://zek.jiagoushi.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://aml.nwbrower.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ppn.ehwqpu.com

Ruby: s.scan(/\d+/)
来源：http://vms.gaohongyu789.top


<!-- 参考信息 -->