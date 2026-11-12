代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://kvc.gzhubu.top

[F10] 取文件扩展名 / 文件名
来源：http://tne.bbcook.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://spe.yonumen.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vmr.feifeiyinyue.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xdd.xuanzx.com

TS:   path.extname("a.txt")
来源：http://whu.redwolf501.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://aru.jiagoushi.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qwu.jinghuilouyu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ewm.jinqigufen.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://igi.jqgufenzy.top

[F11] 复制与移动文件
来源：http://joe.sufxvd.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zym.andypj.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ebo.ydzc1.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vsg.gogol.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tvf.cqqwz.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vms.meibo888.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://maw.iojbl.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wxs.shzxlz.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ahx.yj202588.top

[F12] CSV 读写
来源：http://ttf.jinghuilouyu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gwt.zhiwuduotai.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rzp.chenzaomai.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://udz.gaohongyu789.top

TS:   // 同上
来源：http://uey.hywenlv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uhd.meibo888.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cht.haohaochexian.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://maj.gogol.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zfx.hfpthk.cn

================================================================================
来源：http://gbr.andypj.xyz

G. 面向对象
来源：http://rqw.yj20258888.top

================================================================================
来源：http://yes.xuanzx.com

[G01] 定义类
来源：http://gxg.jyoumei.cn

Py:   class User: pass
来源：http://bef.dianchejie.cn

PHP:  class User {}
来源：http://dyx.gogol.net.cn

JS:   class User {}
来源：http://tlk.vehdjk.com

TS:   class User { name: string = ""; }
来源：http://xiw.guowangkeji.top

Java: class User {}
来源：http://kob.fehbvm.com

Go:   type User struct { Name string }
来源：http://yqw.quarkkingdee.top

Ruby: class User; end
来源：http://dhh.c1oappe.top

C#:   class User {}
来源：http://iiv.hfpthk.cn

[G02] 构造函数
来源：http://afv.jlsjyb.cn

Py:   def __init__(self, name): self.name = name
来源：http://mky.birdmap.top

PHP:  public function __construct(public string $name) {}
来源：http://uef.jqgfzy.top

JS:   constructor(name) { this.name = name; }
来源：http://guc.xinyue.icu

TS:   constructor(public name: string) {}
来源：http://ubb.redwolf501.top

Java: User(String name) { this.name = name; }
来源：http://sll.smart0.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cgf.tianlin.xyz

Ruby: def initialize(name); @name = name; end
来源：http://rhg.andypj.xyz

C#:   public User(string name) { Name = name; }
来源：http://hsb.vehdjk.com

[G03] 实例属性
来源：http://baq.ydzc1.top

Py:   self.name = "x"
来源：http://bda.fengsongda.top

PHP:  public string $name = "x";
来源：http://wdz.birdmap.top

JS:   this.name = "x";
来源：http://uoa.quarkkingdee.top

TS:   name: string = "x";
来源：http://evk.cheryme.top

Java: private String name;
来源：http://jce.guowangkeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mhj.sweek.top

Ruby: @name = "x"
来源：http://vwm.wangdashe.top

C#:   public string Name { get; set; } = "x";
来源：http://pre.fehbvm.com

[G04] 定义方法
来源：http://vfn.ybcxt.top

Py:   def greet(self): return self.name
来源：http://luo.shanyushiyangkeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://uyo.snrcjt.cn

JS:   greet() { return this.name; }
来源：http://jmu.zhiwuduotai.top

TS:   greet(): string { return this.name; }
来源：http://lle.jiagoushi.top

Java: String greet() { return name; }
来源：http://roe.jinghuilouyu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xvt.cucudq.cn

Ruby: def greet; @name; end
来源：http://ndd.ybcxt.top

C#:   public string Greet() => Name;
来源：http://sbt.ivvv.top

[G05] 继承
来源：http://npz.xylfe.cn

Py:   class Admin(User): pass
来源：http://kqg.52xcode.cn

PHP:  class Admin extends User {}
来源：http://lao.kuanghao11.cn

JS:   class Admin extends User {}
来源：http://kba.smart0.xyz

TS:   class Admin extends User {}
来源：http://ysj.iojbl.cn

Java: class Admin extends User {}
来源：http://ybi.hfpthk.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zog.guowangkeji.top

Ruby: class Admin < User; end
来源：http://yij.9152youxi.cn

C#:   class Admin : User {}
来源：http://rnx.jqgufenzy.top

[G06] 重写方法
来源：http://azl.vqdsnc.cn

Py:   def greet(self): return "admin"
来源：http://axw.wangdashe.top

PHP:  public function greet(): string { return "admin"; }
来源：http://nhk.zhiwuduotai.top

JS:   greet() { return "admin"; }
来源：http://yvd.feifeiyinyue.top

TS:   greet(): string { return "admin"; }
来源：http://xdh.fehbvm.com

Java: @Override String greet() { return "admin"; }
来源：http://eva.haohaochexian.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://upy.fengsongda.top

Ruby: def greet; "admin"; end
来源：http://ymb.svipenyu.cn

C#:   public override string Greet() => "admin";
来源：http://nqd.yueranfly.top

[G07] 调用父类方法
来源：http://oxg.yuxming.cn

Py:   super().greet()
来源：http://tie.yangfankeji.com

PHP:  parent::greet();
来源：http://snb.feifeiyinyue.top

JS:   super.greet();
来源：http://quv.fanxiaobao.xyz

TS:   super.greet();
来源：http://bwb.yanxiufei.cn

Java: super.greet();
来源：http://zty.jianghu66.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://thx.aizwys.cn

Ruby: super
来源：http://pyy.smart0.xyz

C#:   base.Greet();
来源：http://baq.gzhubu.top

[G08] 静态方法与属性
来源：http://tvr.haohaochexian.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://spu.cucudq.cn

PHP:  public static function f() {}
来源：http://dwt.zhijiandao.cn

JS:   static f() {}
来源：http://vmi.havefunace.top

TS:   static f(): void {}
来源：http://ady.yongpay.top

Java: static void f() {}
来源：http://jmg.haohaochexian.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://gks.zdqjudy.top

Ruby: def self.f; end
来源：http://dsr.yongpay.top

C#:   public static void F() {}
来源：http://ejf.quarkkingdee.top

[G09] 接口 / 抽象类
来源：http://iwy.yj20258.top

Py:   from abc import ABC, abstractmethod
来源：http://was.birdmap.top

PHP:  interface Shape { public function area(): float; }
来源：http://cxw.haohaochexian.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://bqn.shuidangran.top

TS:   interface Shape { area(): number; }
来源：http://yjj.yonumen.top

Java: interface Shape { double area(); }
来源：http://jxd.shanyushiyangkeji.top

Go:   type Shape interface { Area() float64 }
来源：http://zet.fehbvm.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dja.yanxiufei.cn

C#:   interface IShape { double Area(); }
来源：http://dty.pycfn.com

[G10] 访问控制
来源：http://rdf.zhijiandao.cn

Py:   约定 _protected / __private（不强制）
来源：http://jfl.yongpay.top

PHP:  public / protected / private
来源：http://pxg.aizwys.cn

JS:   #private 字段；其余公开
来源：http://olw.guannengcc.top

TS:   public / protected / private
来源：http://wzl.haohaochexian.top

Java: public / protected / private / 默认包级
来源：http://atc.fengsongda.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://bha.tarul.cn

Ruby: public / protected / private
来源：http://emo.guannengcc.top

C#:   public / protected / private / internal
来源：http://nhe.yuanzhike.top

[G11] getter / setter
来源：http://myx.hnxiangtu.top

Py:   @property 与 @x.setter
来源：http://ajx.jinqigfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://upz.gogol.net.cn

JS:   get name() { return this._name; }
来源：http://lhd.yj202588.top

TS:   get name(): string { return this._name; }
来源：http://jnn.epnwcf.com

Java: public String getName() { return name; }
来源：http://vqn.jinqigfzy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://xmc.aibaodan.cn

Ruby: attr_accessor :name
来源：http://axq.yangfankeji.com

C#:   public string Name { get; set; }
来源：http://uvu.hcnkem.com

[G12] 对象转字符串
来源：http://kez.yangfankeji.com

Py:   def __str__(self): return self.name
来源：http://use.sweek.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ttj.vqdsnc.cn

JS:   toString() { return this.name; }
来源：http://lbh.chenzaomai.com

TS:   toString(): string { return this.name; }
来源：http://tgu.jinyuanbaomall.cn

Java: @Override public String toString() { return name; }
来源：http://oel.gotoacloud.top

Go:   func (u User) String() string { return u.Name }
来源：http://fzh.xingfuxueyuan.xyz

Ruby: def to_s; @name; end
来源：http://yxz.meibo888.top

C#:   public override string ToString() => Name;
来源：http://mhz.xinyue.icu

[G13] 判断对象类型
来源：http://hni.andypj.xyz

Py:   isinstance(u, User)
来源：http://qgz.snrcjt.cn

PHP:  $u instanceof User
来源：http://ywj.cqqwz.cn

JS:   u instanceof User
来源：http://tlb.cashguo.top

TS:   u instanceof User
来源：http://xhm.xingfuxueyuan.xyz

Java: u instanceof User
来源：http://sne.epnwcf.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://wsy.shanyushiyangkeji.top

Ruby: u.is_a?(User)
来源：http://ujc.gotoacloud.top

C#:   u is User
来源：http://jrg.zhoulong.xyz

[G14] 数据类 / record
来源：http://osd.jqgufenzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cxj.cdnleiting.top

PHP:  // 用 readonly 属性模拟
来源：http://vri.bbcook.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ytm.ppjwa.cn

TS:   type User = { name: string; age: number };
来源：http://uaz.gaohongyu789.top

Java: record User(String name, int age) {}
来源：http://zfj.shanyushiyangtech.top

Go:   type User struct { Name string; Age int }
来源：http://kpq.nwbrower.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ayb.yj202588.top

C#:   record User(string Name, int Age);
来源：http://ohu.epnwcf.com

[G15] 枚举
来源：http://zhf.yuanzhike.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://urk.snrcjt.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://veg.jinyuanbaomall.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bcf.52xcode.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bsn.haohaochexian.top

Java: enum Color { RED, GREEN }
来源：http://psu.xuanzx.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dpo.xziqi.cn

Ruby: Color = %i[red green].freeze
来源：http://cfr.yongpay.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tyf.guannengcc.top

[G16] 对象转数组 / 字典
来源：http://srd.yj20258.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fbd.nanxinkj.top

PHP:  get_object_vars($obj);
来源：http://ggv.gotoacloud.top

JS:   Object.entries(obj)
来源：http://pmo.andypj.xyz

TS:   Object.entries(obj)
来源：http://bip.fktsv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://usa.andypj.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://gnj.316326.xyz

Ruby: obj.instance_variables
来源：http://ldz.vqdsnc.cn

C#:   // 用反射或 System.Text.Json
来源：http://fli.quarkkingdee.top

================================================================================
来源：http://coe.shanyushiyangkeji.top

H. 异常与错误处理
来源：http://xzk.ydzc1.top

================================================================================
来源：http://kyr.ivvv.top

[H01] try / catch 基础
来源：http://nci.cheryme.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hbm.tarul.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kzi.zhengqikj.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pjv.andypj.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yld.yfazqb.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vdy.tianlin.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qoy.quarkkingdee.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sdc.chenzaomai.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://akb.jinyuanbaomall.cn

[H02] finally / ensure 收尾
来源：http://kqf.jqgfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://xpa.aizwys.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://atz.hcnkem.com

JS:   try { f(); } finally { cleanup(); }
来源：http://czj.ivvv.top

TS:   try { f(); } finally { cleanup(); }
来源：http://otb.fzhhl.top

Java: try { f(); } finally { cleanup(); }
来源：http://dne.guannengcc.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://tnn.fzhhl.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ojj.jianghu66.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://oxt.xuetiantiany.cn

[H03] 主动抛出异常
来源：http://pvq.bbcook.cn

Py:   raise ValueError("错误信息")
来源：http://ega.wangdashe.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bxz.hesvh.cn

JS:   throw new Error("错误信息");
来源：http://nyn.yongpay.top

TS:   throw new Error("错误信息");
来源：http://etn.jianghu66.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ich.ywan-chungtsiang.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ctb.birdmap.top

Ruby: raise ArgumentError, "错误信息"
来源：http://fly.cqqwz.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qep.ppjwa.cn

[H04] 自定义异常类型
来源：http://pnu.ctjpmb.com

Py:   class MyError(Exception): pass
来源：http://hnd.shanyushiyangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://vwj.zdbjq.cn

JS:   class MyError extends Error {}
来源：http://sep.chenjidiqi.icu

TS:   class MyError extends Error {}
来源：http://gdw.sxryk.cn

Java: class MyException extends RuntimeException {}
来源：http://xoy.fengsongda.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qha.ybcxt.top

Ruby: class MyError < StandardError; end
来源：http://qtn.yonumen.top

C#:   class MyException : Exception {}
来源：http://nqp.zhaomingkeji.xyz

[H05] 捕获特定类型
来源：http://bjk.zhengqikj.top

Py:   except ValueError as e:
来源：http://wkn.ivvv.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://iaq.fzhhl.top

JS:   if (e instanceof TypeError) {}
来源：http://sar.hammf.cn

TS:   if (e instanceof TypeError) {}
来源：http://vqm.haohaochexian.top

Java: catch (IOException | SQLException e) {}
来源：http://ged.smart0.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vyk.gzhubu.top

Ruby: rescue ArgumentError => e
来源：http://dls.52xcode.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nwx.316326.xyz

[H06] 可选值 / 空值安全访问
来源：http://sbr.sysykeji.top

Py:   value = d.get("k") or default
来源：http://zii.aizwys.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xra.aizwys.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mym.ydjk.org.cn

TS:   obj?.a?.b;  d ?? default
来源：http://epm.bjfxy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fbh.fktsv.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ntb.jinyuanbaomall.cn

Ruby: d&.dig(:a, :b)
来源：http://glw.9152youxi.cn

C#:   obj?.A?.B ?? default
来源：http://wqj.yfazqb.com

[H07] 断言
来源：http://ldk.jinghuilouyu.cn

Py:   assert x > 0, "必须为正"
来源：http://ufw.jqgfzy.top

PHP:  assert($x > 0);
来源：http://lzc.hammf.cn

JS:   console.assert(x > 0);
来源：http://qrm.wangshuangyany.cn

TS:   console.assert(x > 0);
来源：http://epk.snrcjt.cn

Java: assert x > 0 : "必须为正";
来源：http://gjb.zhengqikj.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ivh.guowangkeji.top

Ruby: raise "必须为正" unless x > 0
来源：http://gdo.sxryk.cn

C#:   Debug.Assert(x > 0);
来源：http://ssh.jyoumei.cn

[H08] 获取错误信息与堆栈
来源：http://akd.hywenlv.cn

Py:   str(e);  traceback.format_exc()
来源：http://egi.316326.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zhp.cqqwz.cn

JS:   e.message;  e.stack
来源：http://zvz.xuetiantiany.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://alo.yonumen.top

Java: e.getMessage();  e.printStackTrace()
来源：http://pgg.pengpengdd.cyou

Go:   err.Error()
来源：http://dkn.jinqigfzy.top

Ruby: e.message;  e.backtrace
来源：http://uuo.sweek.top

C#:   e.Message;  e.StackTrace
来源：http://ryf.ydjk.org.cn

[H09] 带错误码的异常
来源：http://lua.zhoulong.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dyg.ywan-chungtsiang.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://qkj.fehbvm.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://juw.ywan-chungtsiang.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kmr.feifeiyinyue.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://prd.feifeiyinyue.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jvp.sjlbkw.cn

Ruby: raise MyError.new("fail", 500)
来源：http://emw.jqgfzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://snw.sxryk.cn

[H10] 资源自动释放
来源：http://npz.jianghu66.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://pth.jlsjyb.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kpk.yj20258.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ddq.mhx1999.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://efc.ywan-chungtsiang.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cse.ehwqpu.com

Go:   defer f.Close()
来源：http://cyl.316326.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://eqi.xuetiantiany.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rst.shanyushiyangkeji.top

================================================================================
来源：http://ckd.zhijiandao.cn

I. 正则表达式
来源：http://wrp.316326.xyz

================================================================================
来源：http://uwz.zhongyouzk.top

[I01] 判断是否匹配
来源：http://cgx.gzhubu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qnz.yuxming.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jea.9152youxi.cn

JS:   /\d+/.test(s)
来源：http://rmn.daria6918.cn

TS:   /\d+/.test(s)
来源：http://vrm.nanxinkj.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vuz.0kj1m.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hay.daxiang520.top

Ruby: s.match?(/\d+/)
来源：http://zpw.jinghuilouyu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zsi.sysykeji.top

[I02] 提取所有匹配
来源：http://pud.ppjwa.cn

Py:   re.findall(r"\d+", s)
来源：http://emk.chenjidiqi.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jfz.guowangkeji.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qwp.shangyingyoupin.top

TS:   s.match(/\d+/g)
来源：http://lqh.yj202588.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ibd.jianghu66.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wdq.daxiang520.top

Ruby: s.scan(/\d+/)
来源：http://mfm.mhx1999.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://njs.sufxvd.cn

[I03] 提取捕获分组
来源：http://ewh.wangdashe.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wbw.jinyuanbaomall.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ips.jyoumei.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ftl.tarul.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dnn.vqdsnc.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rbt.vehdjk.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wmv.haohaochexian.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ddn.shuidangran.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fmf.zdqjudy.top

[I04] 正则替换
来源：http://fjk.chenjidiqi.icu

Py:   re.sub(r"\d+", "#", s)
来源：http://mpe.zhijiandao.cn


<!-- 参考信息 -->