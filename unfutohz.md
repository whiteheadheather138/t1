代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xqo.hywenlv.cn

TS:   path.extname("a.txt")
来源：http://fqh.xziqi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rhs.daria6918.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mro.hnxiangtu.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ntd.52xcode.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fmz.sufxvd.cn

[F11] 复制与移动文件
来源：http://roi.pengpengdd.cyou

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://skj.yj20258888.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kal.sxryk.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://txj.xylfe.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kwc.bbcook.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xsv.dianchejie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://arm.ybcxt.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rnd.yongpay.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bdv.fanxiaobao.xyz

[F12] CSV 读写
来源：http://tib.xylfe.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://glz.chenzaomai.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mny.guannengcc.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wwh.cheryme.top

TS:   // 同上
来源：http://ncu.tianlin.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qvy.cheryme.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://era.nwbrower.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://akz.svipenyu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qcb.sufxvd.cn

================================================================================
来源：http://svk.ehwqpu.com

G. 面向对象
来源：http://zlb.tarul.cn

================================================================================
来源：http://hip.cucudq.cn

[G01] 定义类
来源：http://zuf.yj20258888.top

Py:   class User: pass
来源：http://awk.epnwcf.com

PHP:  class User {}
来源：http://nda.jinyuanbaomall.cn

JS:   class User {}
来源：http://fmw.gaohongyu789.top

TS:   class User { name: string = ""; }
来源：http://wlf.yuxming.cn

Java: class User {}
来源：http://lxq.shzxlz.cn

Go:   type User struct { Name string }
来源：http://xvb.cucudq.cn

Ruby: class User; end
来源：http://jwj.epnwcf.com

C#:   class User {}
来源：http://xpa.ppjwa.cn

[G02] 构造函数
来源：http://qot.andypj.xyz

Py:   def __init__(self, name): self.name = name
来源：http://cdy.yangfankeji.com

PHP:  public function __construct(public string $name) {}
来源：http://mzw.andypj.xyz

JS:   constructor(name) { this.name = name; }
来源：http://pgp.zhaomingkeji.xyz

TS:   constructor(public name: string) {}
来源：http://flf.jiagoushi.top

Java: User(String name) { this.name = name; }
来源：http://yys.pycfn.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://eoa.yuxming.cn

Ruby: def initialize(name); @name = name; end
来源：http://kyl.zhixingplan.top

C#:   public User(string name) { Name = name; }
来源：http://dcr.nwbrower.top

[G03] 实例属性
来源：http://vep.jianghu66.top

Py:   self.name = "x"
来源：http://kif.jiagoushi.top

PHP:  public string $name = "x";
来源：http://way.sjlbkw.cn

JS:   this.name = "x";
来源：http://ffe.yuxming.cn

TS:   name: string = "x";
来源：http://chr.feifeiyinyue.top

Java: private String name;
来源：http://ksb.hcnkem.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jsm.aizwys.cn

Ruby: @name = "x"
来源：http://ijc.52xcode.cn

C#:   public string Name { get; set; } = "x";
来源：http://kon.zhongyouzk.top

[G04] 定义方法
来源：http://nev.ydzc1.top

Py:   def greet(self): return self.name
来源：http://fwg.gzhubu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://nnu.wangshuangyany.cn

JS:   greet() { return this.name; }
来源：http://aio.yuxming.cn

TS:   greet(): string { return this.name; }
来源：http://cln.tanke756.top

Java: String greet() { return name; }
来源：http://lfe.zhengqikj.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://cyb.c1oappe.top

Ruby: def greet; @name; end
来源：http://lpx.iojbl.cn

C#:   public string Greet() => Name;
来源：http://mps.gotoacloud.top

[G05] 继承
来源：http://xkk.ybcxt.top

Py:   class Admin(User): pass
来源：http://xcm.zhijiandao.cn

PHP:  class Admin extends User {}
来源：http://xfo.yonumen.top

JS:   class Admin extends User {}
来源：http://tfl.hongshengwenyu.top

TS:   class Admin extends User {}
来源：http://rtg.fehbvm.com

Java: class Admin extends User {}
来源：http://ewh.9152youxi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bdx.pengpengdd.cyou

Ruby: class Admin < User; end
来源：http://nzw.svipenyu.cn

C#:   class Admin : User {}
来源：http://lrs.52xcode.cn

[G06] 重写方法
来源：http://gui.jinyuanbaomall.cn

Py:   def greet(self): return "admin"
来源：http://clj.yuxming.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bzr.chenlongwang.top

JS:   greet() { return "admin"; }
来源：http://byl.jiagoushi.top

TS:   greet(): string { return "admin"; }
来源：http://gqm.xinyue.icu

Java: @Override String greet() { return "admin"; }
来源：http://mra.iojbl.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://epx.xziqi.cn

Ruby: def greet; "admin"; end
来源：http://frj.jqgufenzy.top

C#:   public override string Greet() => "admin";
来源：http://yql.yj20258888.top

[G07] 调用父类方法
来源：http://tvg.yangfankeji.com

Py:   super().greet()
来源：http://ojz.nwbrower.top

PHP:  parent::greet();
来源：http://otx.zhiwuduotai.top

JS:   super.greet();
来源：http://buu.yfazqb.com

TS:   super.greet();
来源：http://qzm.ydzc1.top

Java: super.greet();
来源：http://hyy.fanxiaobao.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xhc.jinyuanbaomall.cn

Ruby: super
来源：http://zss.hysaishi.cn

C#:   base.Greet();
来源：http://xeb.tarul.cn

[G08] 静态方法与属性
来源：http://kdu.ivvv.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cbc.c1oappe.top

PHP:  public static function f() {}
来源：http://dzr.xziqi.cn

JS:   static f() {}
来源：http://mkx.wangdashe.top

TS:   static f(): void {}
来源：http://dsu.ivvv.top

Java: static void f() {}
来源：http://yrk.ywan-chungtsiang.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://pnt.zdbjq.cn

Ruby: def self.f; end
来源：http://ssn.nwbrower.top

C#:   public static void F() {}
来源：http://pai.vehdjk.com

[G09] 接口 / 抽象类
来源：http://itw.tian-w.cn

Py:   from abc import ABC, abstractmethod
来源：http://btn.cqqwz.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zqg.gogol.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hys.zhoulong.xyz

TS:   interface Shape { area(): number; }
来源：http://eby.0kj1m.cn

Java: interface Shape { double area(); }
来源：http://jbq.52xcode.cn

Go:   type Shape interface { Area() float64 }
来源：http://pax.cdnleiting.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://oli.ybcxt.top

C#:   interface IShape { double Area(); }
来源：http://mxy.shanyushiyangkeji.top

[G10] 访问控制
来源：http://non.yonumen.top

Py:   约定 _protected / __private（不强制）
来源：http://vml.kuanghao11.cn

PHP:  public / protected / private
来源：http://hpn.jiagoushi.top

JS:   #private 字段；其余公开
来源：http://faf.xuanzx.com

TS:   public / protected / private
来源：http://rvo.ydzc1.top

Java: public / protected / private / 默认包级
来源：http://soh.guowangkeji.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://laf.ehwqpu.com

Ruby: public / protected / private
来源：http://mvv.zhaomingkeji.xyz

C#:   public / protected / private / internal
来源：http://llc.cheryme.top

[G11] getter / setter
来源：http://nbm.jyoumei.cn

Py:   @property 与 @x.setter
来源：http://klh.xinyue.icu

PHP:  public function getName(): string { return $this->name; }
来源：http://ufu.xuanzx.com

JS:   get name() { return this._name; }
来源：http://fnw.sjlbkw.cn

TS:   get name(): string { return this._name; }
来源：http://pva.andypj.xyz

Java: public String getName() { return name; }
来源：http://igc.ywan-chungtsiang.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://jye.gzhubu.top

Ruby: attr_accessor :name
来源：http://qdg.zhengqikj.top

C#:   public string Name { get; set; }
来源：http://tjl.zhixingplan.top

[G12] 对象转字符串
来源：http://jbe.52xcode.cn

Py:   def __str__(self): return self.name
来源：http://abs.hcnkem.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://hju.dianchejie.cn

JS:   toString() { return this.name; }
来源：http://aal.hongshengwenyu.top

TS:   toString(): string { return this.name; }
来源：http://nhh.gotoacloud.top

Java: @Override public String toString() { return name; }
来源：http://fkb.ydzc1.top

Go:   func (u User) String() string { return u.Name }
来源：http://tap.bbcook.cn

Ruby: def to_s; @name; end
来源：http://hwx.chenzaomai.com

C#:   public override string ToString() => Name;
来源：http://dwk.pengpengdd.cyou

[G13] 判断对象类型
来源：http://zil.aibaodan.cn

Py:   isinstance(u, User)
来源：http://lic.jinyuanbaomall.cn

PHP:  $u instanceof User
来源：http://zmq.gzhubu.top

JS:   u instanceof User
来源：http://bvj.jyoumei.cn

TS:   u instanceof User
来源：http://mkq.hnxiangtu.top

Java: u instanceof User
来源：http://lkb.kuanghao11.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kfj.shangyingyoupin.top

Ruby: u.is_a?(User)
来源：http://ono.wangshuangyany.cn

C#:   u is User
来源：http://jmw.gotoacloud.top

[G14] 数据类 / record
来源：http://nwn.zhiwuduotai.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ikg.xuetiantiany.cn

PHP:  // 用 readonly 属性模拟
来源：http://roy.ehwqpu.com

JS:   // 无内置：普通类或对象字面量
来源：http://mcr.wangdashe.top

TS:   type User = { name: string; age: number };
来源：http://zkh.jiagoushi.top

Java: record User(String name, int age) {}
来源：http://yfj.jinghuilouyu.cn

Go:   type User struct { Name string; Age int }
来源：http://knn.vehdjk.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uno.meibo888.top

C#:   record User(string Name, int Age);
来源：http://afr.jqgfzy.top

[G15] 枚举
来源：http://npq.jinghuilouyu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fxl.gaohongyu789.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://hie.xingfuxueyuan.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kyn.mhx1999.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cjj.mhx1999.top

Java: enum Color { RED, GREEN }
来源：http://dkd.yueranfly.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://but.zhoulong.xyz

Ruby: Color = %i[red green].freeze
来源：http://lfg.yangfankeji.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vrb.hfpthk.cn

[G16] 对象转数组 / 字典
来源：http://cia.wangdashe.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lil.yfazqb.com

PHP:  get_object_vars($obj);
来源：http://dmk.fktsv.cn

JS:   Object.entries(obj)
来源：http://ryh.52xcode.cn

TS:   Object.entries(obj)
来源：http://gog.yj202588.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kum.fehbvm.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://yuj.zhixingplan.top

Ruby: obj.instance_variables
来源：http://zfd.cqqwz.cn

C#:   // 用反射或 System.Text.Json
来源：http://vyw.cashguo.top

================================================================================
来源：http://taq.hammf.cn

H. 异常与错误处理
来源：http://szo.epnwcf.com

================================================================================
来源：http://zmf.chenlongwang.top

[H01] try / catch 基础
来源：http://wfr.quarkkingdee.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zqm.xuanzx.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wip.cdnleiting.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fms.hammf.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fiu.jqgufenzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://upi.hammf.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rvq.gogol.net.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mqo.zhiwuduotai.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nvj.zhengqikj.top

[H02] finally / ensure 收尾
来源：http://qaj.xinyue.icu

Py:   try: f()⏎finally: cleanup()
来源：http://ogu.xuanzx.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://ahl.zhiwuduotai.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ckz.tarul.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zxx.zhaomingkeji.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://lps.havefunace.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://vvt.hnxiangtu.top

Ruby: begin; f; ensure; cleanup; end
来源：http://dlz.ctjpmb.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://uhe.hammf.cn

[H03] 主动抛出异常
来源：http://vcv.epnwcf.com

Py:   raise ValueError("错误信息")
来源：http://hhw.havefunace.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mwj.zdqjudy.top

JS:   throw new Error("错误信息");
来源：http://smf.ydzc1.top

TS:   throw new Error("错误信息");
来源：http://jfz.jqgufenzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://bsp.hongshengwenyu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uvy.nwbrower.top

Ruby: raise ArgumentError, "错误信息"
来源：http://hzy.jlsjyb.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hpk.yj20258.top

[H04] 自定义异常类型
来源：http://lzv.jiagoushi.top

Py:   class MyError(Exception): pass
来源：http://djv.jlsjyb.cn

PHP:  class MyError extends RuntimeException {}
来源：http://kex.nanxinkj.top

JS:   class MyError extends Error {}
来源：http://ens.mhx1999.top

TS:   class MyError extends Error {}
来源：http://tfy.fzhhl.top

Java: class MyException extends RuntimeException {}
来源：http://zdo.gaohongyu789.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ebm.daria6918.cn

Ruby: class MyError < StandardError; end
来源：http://dxg.yj20258.top

C#:   class MyException : Exception {}
来源：http://tkp.yongpay.top

[H05] 捕获特定类型
来源：http://abe.svipenyu.cn

Py:   except ValueError as e:
来源：http://rli.zhoulong.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vls.wangdashe.top

JS:   if (e instanceof TypeError) {}
来源：http://epk.hongshengwenyu.top

TS:   if (e instanceof TypeError) {}
来源：http://qnq.dashuyun.cn

Java: catch (IOException | SQLException e) {}
来源：http://vif.fengsongda.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wtg.feifeiyinyue.top

Ruby: rescue ArgumentError => e
来源：http://qme.tian-w.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dts.zdbjq.cn

[H06] 可选值 / 空值安全访问
来源：http://ksk.snrcjt.cn

Py:   value = d.get("k") or default
来源：http://wpk.zhongyouzk.top

PHP:  $v = $d["k"] ?? null;
来源：http://zjf.c1oappe.top

JS:   obj?.a?.b;  d ?? default
来源：http://puj.xinyue.icu

TS:   obj?.a?.b;  d ?? default
来源：http://wgy.chenzaomai.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rmp.hongshengwenyu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://qsi.bbcook.cn

Ruby: d&.dig(:a, :b)
来源：http://jiv.yonumen.top

C#:   obj?.A?.B ?? default
来源：http://vjq.shzxlz.cn

[H07] 断言
来源：http://bor.sxryk.cn

Py:   assert x > 0, "必须为正"
来源：http://fbk.haohaochexian.top

PHP:  assert($x > 0);
来源：http://mdd.jinqigfzy.top

JS:   console.assert(x > 0);
来源：http://epg.zhixingplan.top

TS:   console.assert(x > 0);
来源：http://dxh.mhx1999.top

Java: assert x > 0 : "必须为正";
来源：http://gab.yonumen.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lhr.xingfuxueyuan.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://mlf.gogol.net.cn

C#:   Debug.Assert(x > 0);
来源：http://ept.hywenlv.cn

[H08] 获取错误信息与堆栈
来源：http://jvx.jqgufenzy.top

Py:   str(e);  traceback.format_exc()
来源：http://ygj.sxryk.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zel.birdmap.top

JS:   e.message;  e.stack
来源：http://dvj.chenzaomai.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://rhb.cheryme.top

Java: e.getMessage();  e.printStackTrace()
来源：http://czr.fanxiaobao.xyz

Go:   err.Error()
来源：http://gvi.hnqzz.top

Ruby: e.message;  e.backtrace
来源：http://kyz.c1oappe.top

C#:   e.Message;  e.StackTrace
来源：http://knl.xylfe.cn

[H09] 带错误码的异常
来源：http://xbn.gzhubu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yym.tianlin.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://dkc.epnwcf.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hnd.gotoacloud.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bds.cdnleiting.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lly.hongshengwenyu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://btr.yuxming.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pcj.vehdjk.com

C#:   // 自定义异常类中加 Code 属性
来源：http://ytb.shangyingyoupin.top

[H10] 资源自动释放
来源：http://sfi.gaohongyu789.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://qts.sweek.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qrc.zhixingplan.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qkr.hammf.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nkq.xuetiantiany.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tfm.yuxming.cn

Go:   defer f.Close()
来源：http://rkn.hcnkem.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://poq.meibo888.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qjx.smart0.xyz

================================================================================
来源：http://pte.pycfn.com

I. 正则表达式
来源：http://fjm.fzhhl.top

================================================================================
来源：http://pxz.jlsjyb.cn

[I01] 判断是否匹配
来源：http://zvc.sufxvd.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mlx.sysykeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://pbl.wangdashe.top

JS:   /\d+/.test(s)
来源：http://ixa.cheryme.top

TS:   /\d+/.test(s)
来源：http://sxj.yj20258888.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xue.zhengqikj.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zmu.cheryme.top

Ruby: s.match?(/\d+/)
来源：http://isv.guannengcc.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wpr.aizwys.cn

[I02] 提取所有匹配
来源：http://mbg.zhiwuduotai.top

Py:   re.findall(r"\d+", s)
来源：http://xxl.zhaomingkeji.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vks.kuanghao11.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yue.chenjidiqi.icu

TS:   s.match(/\d+/g)
来源：http://odj.zycfv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://axd.zhoulong.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ojc.hywenlv.cn

Ruby: s.scan(/\d+/)
来源：http://ovp.epnwcf.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wow.ctjpmb.com

[I03] 提取捕获分组
来源：http://guv.fehbvm.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ytv.gzhubu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://orr.vqdsnc.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bha.hywenlv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qfv.sxryk.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dsu.xziqi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lyx.vqdsnc.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://iar.hywenlv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jox.xingfuxueyuan.xyz

[I04] 正则替换
来源：http://cmq.ehwqpu.com

Py:   re.sub(r"\d+", "#", s)
来源：http://jdc.hongshengwenyu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yho.fengsongda.top

JS:   s.replace(/\d+/g, "#")
来源：http://tzt.bbcook.cn

TS:   s.replace(/\d+/g, "#")
来源：http://uum.cashguo.top

Java: s.replaceAll("\\d+", "#")
来源：http://sgx.ppjwa.cn


<!-- 参考信息 -->