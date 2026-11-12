代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ohq.shuidangran.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kdi.yfazqb.com

[F11] 复制与移动文件
来源：http://ylt.kuanghao11.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hii.hfpthk.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rcj.xinyue.icu

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://awk.bbcook.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zjy.ywan-chungtsiang.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nbq.xuanzx.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jsx.mhx1999.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rwl.vehdjk.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ako.dianchejie.cn

[F12] CSV 读写
来源：http://kqn.vehdjk.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://csi.zhijiandao.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qcq.chenjidiqi.icu

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vlj.jyoumei.cn

TS:   // 同上
来源：http://xvj.cdnleiting.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ppk.mhx1999.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vqz.316326.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ewe.shzxlz.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://apm.nanxinkj.top

================================================================================
来源：http://wzb.sweek.top

G. 面向对象
来源：http://pvh.zdbjq.cn

================================================================================
来源：http://hby.gotoacloud.top

[G01] 定义类
来源：http://xxf.yonumen.top

Py:   class User: pass
来源：http://uww.0kj1m.cn

PHP:  class User {}
来源：http://qod.hysaishi.cn

JS:   class User {}
来源：http://ree.cqqwz.cn

TS:   class User { name: string = ""; }
来源：http://vkx.zhaomingkeji.xyz

Java: class User {}
来源：http://cqa.hysaishi.cn

Go:   type User struct { Name string }
来源：http://dzm.jiagoushi.top

Ruby: class User; end
来源：http://lbw.quarkkingdee.top

C#:   class User {}
来源：http://vuq.yj20258888.top

[G02] 构造函数
来源：http://qtr.zdbjq.cn

Py:   def __init__(self, name): self.name = name
来源：http://hhf.zhiwuduotai.top

PHP:  public function __construct(public string $name) {}
来源：http://dsg.hcnkem.com

JS:   constructor(name) { this.name = name; }
来源：http://tad.jianghu66.top

TS:   constructor(public name: string) {}
来源：http://jzz.zhaomingkeji.xyz

Java: User(String name) { this.name = name; }
来源：http://jnb.dashuyun.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ewc.yanxiufei.cn

Ruby: def initialize(name); @name = name; end
来源：http://wdu.pengpengdd.cyou

C#:   public User(string name) { Name = name; }
来源：http://hmn.yuanzhike.top

[G03] 实例属性
来源：http://phi.zycfv.cn

Py:   self.name = "x"
来源：http://zep.yvedp.cn

PHP:  public string $name = "x";
来源：http://xhw.xuetiantiany.cn

JS:   this.name = "x";
来源：http://iqa.jlsjyb.cn

TS:   name: string = "x";
来源：http://dcm.0kj1m.cn

Java: private String name;
来源：http://zos.tarul.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://waa.gzhubu.top

Ruby: @name = "x"
来源：http://znx.jqgfzy.top

C#:   public string Name { get; set; } = "x";
来源：http://naf.shanyushiyangkeji.top

[G04] 定义方法
来源：http://hnj.xziqi.cn

Py:   def greet(self): return self.name
来源：http://ynw.smart0.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://oly.yj20258.top

JS:   greet() { return this.name; }
来源：http://lty.xuetiantiany.cn

TS:   greet(): string { return this.name; }
来源：http://lcw.sjlbkw.cn

Java: String greet() { return name; }
来源：http://ojc.mhx1999.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://weq.zhoulong.xyz

Ruby: def greet; @name; end
来源：http://ylo.zhaomingkeji.xyz

C#:   public string Greet() => Name;
来源：http://zcs.tian-w.cn

[G05] 继承
来源：http://hgn.hnxiangtu.top

Py:   class Admin(User): pass
来源：http://grw.uphjek.com

PHP:  class Admin extends User {}
来源：http://nvr.cdnleiting.top

JS:   class Admin extends User {}
来源：http://xmm.ppjwa.cn

TS:   class Admin extends User {}
来源：http://hml.ehwqpu.com

Java: class Admin extends User {}
来源：http://bre.daria6918.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xnq.zycfv.cn

Ruby: class Admin < User; end
来源：http://dia.ehwqpu.com

C#:   class Admin : User {}
来源：http://lma.nanxinkj.top

[G06] 重写方法
来源：http://sac.hcnkem.com

Py:   def greet(self): return "admin"
来源：http://rhr.0kj1m.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tkr.gogol.net.cn

JS:   greet() { return "admin"; }
来源：http://ubb.xziqi.cn

TS:   greet(): string { return "admin"; }
来源：http://gmx.xinyue.icu

Java: @Override String greet() { return "admin"; }
来源：http://zfd.wangdashe.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://eze.9152youxi.cn

Ruby: def greet; "admin"; end
来源：http://atg.yanxiufei.cn

C#:   public override string Greet() => "admin";
来源：http://rzh.dashuyun.cn

[G07] 调用父类方法
来源：http://bkq.tarul.cn

Py:   super().greet()
来源：http://qcq.ydzc1.top

PHP:  parent::greet();
来源：http://atj.hnqzz.top

JS:   super.greet();
来源：http://lqj.wangshuangyany.cn

TS:   super.greet();
来源：http://kwe.gzhubu.top

Java: super.greet();
来源：http://lcy.c1oappe.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xni.ehwqpu.com

Ruby: super
来源：http://bos.snrcjt.cn

C#:   base.Greet();
来源：http://zdp.gaohongyu789.top

[G08] 静态方法与属性
来源：http://oez.shangyingyoupin.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ybj.bbcook.cn

PHP:  public static function f() {}
来源：http://dqb.shanyushiyangkeji.top

JS:   static f() {}
来源：http://gxv.uphjek.com

TS:   static f(): void {}
来源：http://itm.vehdjk.com

Java: static void f() {}
来源：http://naq.mhx1999.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ipy.pengpengdd.cyou

Ruby: def self.f; end
来源：http://pvl.yj202588.top

C#:   public static void F() {}
来源：http://iwf.cdnleiting.top

[G09] 接口 / 抽象类
来源：http://qaq.fehbvm.com

Py:   from abc import ABC, abstractmethod
来源：http://nvn.iojbl.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jgv.jlsjyb.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nfc.yuanzhike.top

TS:   interface Shape { area(): number; }
来源：http://hsx.hongshengwenyu.top

Java: interface Shape { double area(); }
来源：http://cwy.zhijiandao.cn

Go:   type Shape interface { Area() float64 }
来源：http://rzf.gogol.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mah.kuanghao11.cn

C#:   interface IShape { double Area(); }
来源：http://ifq.fzhhl.top

[G10] 访问控制
来源：http://bui.meibo888.top

Py:   约定 _protected / __private（不强制）
来源：http://tez.cashguo.top

PHP:  public / protected / private
来源：http://tkx.gogol.net.cn

JS:   #private 字段；其余公开
来源：http://nst.jinyuanbaomall.cn

TS:   public / protected / private
来源：http://dmm.pycfn.com

Java: public / protected / private / 默认包级
来源：http://woz.c1oappe.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ptw.zhongyouzk.top

Ruby: public / protected / private
来源：http://wbt.birdmap.top

C#:   public / protected / private / internal
来源：http://gyv.zhiwuduotai.top

[G11] getter / setter
来源：http://fri.hammf.cn

Py:   @property 与 @x.setter
来源：http://qyq.zhengqikj.top

PHP:  public function getName(): string { return $this->name; }
来源：http://fnq.cqqwz.cn

JS:   get name() { return this._name; }
来源：http://dwv.yuanzhike.top

TS:   get name(): string { return this._name; }
来源：http://kce.sweek.top

Java: public String getName() { return name; }
来源：http://rjx.hcnkem.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://hrx.jlsjyb.cn

Ruby: attr_accessor :name
来源：http://wbf.0kj1m.cn

C#:   public string Name { get; set; }
来源：http://uqj.yj20258888.top

[G12] 对象转字符串
来源：http://dbr.fktsv.cn

Py:   def __str__(self): return self.name
来源：http://kol.smart0.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://ady.xingfuxueyuan.xyz

JS:   toString() { return this.name; }
来源：http://cwr.xinyue.icu

TS:   toString(): string { return this.name; }
来源：http://yvk.jlsjyb.cn

Java: @Override public String toString() { return name; }
来源：http://rmb.jqgfzy.top

Go:   func (u User) String() string { return u.Name }
来源：http://ryc.daxiang520.top

Ruby: def to_s; @name; end
来源：http://hzq.316326.xyz

C#:   public override string ToString() => Name;
来源：http://vuq.fehbvm.com

[G13] 判断对象类型
来源：http://zdo.jlsjyb.cn

Py:   isinstance(u, User)
来源：http://reo.zhaomingkeji.xyz

PHP:  $u instanceof User
来源：http://tij.ydjk.org.cn

JS:   u instanceof User
来源：http://yyr.zhaomingkeji.xyz

TS:   u instanceof User
来源：http://jpu.yj202588.top

Java: u instanceof User
来源：http://bla.zdqjudy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://per.ctjpmb.com

Ruby: u.is_a?(User)
来源：http://voa.hnqzz.top

C#:   u is User
来源：http://hcm.fktsv.cn

[G14] 数据类 / record
来源：http://anv.andypj.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ubi.hnqzz.top

PHP:  // 用 readonly 属性模拟
来源：http://ugp.yvedp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://cno.haohaochexian.top

TS:   type User = { name: string; age: number };
来源：http://coo.cdnleiting.top

Java: record User(String name, int age) {}
来源：http://fvg.yfazqb.com

Go:   type User struct { Name string; Age int }
来源：http://wre.fengsongda.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://btr.jinqigfzy.top

C#:   record User(string Name, int Age);
来源：http://jql.hongshengwenyu.top

[G15] 枚举
来源：http://dnm.hnqzz.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ihf.hnxiangtu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://prs.meibo888.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fmu.hongshengwenyu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nfq.sweek.top

Java: enum Color { RED, GREEN }
来源：http://tme.hfpthk.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hlj.sxryk.cn

Ruby: Color = %i[red green].freeze
来源：http://vgv.epnwcf.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dgy.ydzc1.top

[G16] 对象转数组 / 字典
来源：http://xen.hfpthk.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://oie.nanxuanxn.top

PHP:  get_object_vars($obj);
来源：http://wcn.shzxlz.cn

JS:   Object.entries(obj)
来源：http://rrg.sweek.top

TS:   Object.entries(obj)
来源：http://hdd.zycfv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jjq.shanyushiyangkeji.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://alj.xuanzx.com

Ruby: obj.instance_variables
来源：http://lct.redwolf501.top

C#:   // 用反射或 System.Text.Json
来源：http://xej.xinyue.icu

================================================================================
来源：http://frl.shanyushiyangkeji.top

H. 异常与错误处理
来源：http://iky.ppjwa.cn

================================================================================
来源：http://xag.wangshuangyany.cn

[H01] try / catch 基础
来源：http://ebh.yuxming.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gks.iojbl.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vpf.uphjek.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://maz.yj202588.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rbn.quarkkingdee.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tus.kuanghao11.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mez.pycfn.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qpz.bbcook.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://edr.shzxlz.cn

[H02] finally / ensure 收尾
来源：http://gls.9152youxi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://avo.shanyushiyangtech.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://mrz.iojbl.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qmo.jinqigfzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://pbx.shuidangran.top

Java: try { f(); } finally { cleanup(); }
来源：http://hdx.nanxuanxn.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ezl.jianghu66.top

Ruby: begin; f; ensure; cleanup; end
来源：http://yxn.cucudq.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gkd.gzhubu.top

[H03] 主动抛出异常
来源：http://bch.jinqigufen.top

Py:   raise ValueError("错误信息")
来源：http://wgs.shangyingyoupin.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://enc.sufxvd.cn

JS:   throw new Error("错误信息");
来源：http://hia.hywenlv.cn

TS:   throw new Error("错误信息");
来源：http://cvp.fengsongda.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://dnq.zhoulong.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ynl.c1oappe.top

Ruby: raise ArgumentError, "错误信息"
来源：http://zpm.zhoulong.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://tcz.cashguo.top

[H04] 自定义异常类型
来源：http://bwa.gzhubu.top

Py:   class MyError(Exception): pass
来源：http://rlu.9152youxi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://kjt.cashguo.top

JS:   class MyError extends Error {}
来源：http://xie.chenzaomai.com

TS:   class MyError extends Error {}
来源：http://mee.cheryme.top

Java: class MyException extends RuntimeException {}
来源：http://oyu.daxiang520.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xqh.uphjek.com

Ruby: class MyError < StandardError; end
来源：http://gjv.yanxiufei.cn

C#:   class MyException : Exception {}
来源：http://bwh.pycfn.com

[H05] 捕获特定类型
来源：http://ubr.ehwqpu.com

Py:   except ValueError as e:
来源：http://nrx.zycfv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://boe.gogol.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://sap.yongpay.top

TS:   if (e instanceof TypeError) {}
来源：http://ikp.tarul.cn

Java: catch (IOException | SQLException e) {}
来源：http://tee.sufxvd.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jhk.nanxinkj.top

Ruby: rescue ArgumentError => e
来源：http://muw.pycfn.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tjh.guannengcc.top

[H06] 可选值 / 空值安全访问
来源：http://hec.jinyuanbaomall.cn

Py:   value = d.get("k") or default
来源：http://pkz.hfpthk.cn

PHP:  $v = $d["k"] ?? null;
来源：http://glw.haohaochexian.top

JS:   obj?.a?.b;  d ?? default
来源：http://qjc.aibaodan.cn

TS:   obj?.a?.b;  d ?? default
来源：http://sqa.jiagoushi.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uac.52xcode.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://cuj.c1oappe.top

Ruby: d&.dig(:a, :b)
来源：http://rsr.chenzaomai.com

C#:   obj?.A?.B ?? default
来源：http://yuc.gotoacloud.top

[H07] 断言
来源：http://mri.xuetiantiany.cn

Py:   assert x > 0, "必须为正"
来源：http://nqp.dashuyun.cn

PHP:  assert($x > 0);
来源：http://myf.shzxlz.cn

JS:   console.assert(x > 0);
来源：http://drx.bbcook.cn

TS:   console.assert(x > 0);
来源：http://yxl.ctjpmb.com

Java: assert x > 0 : "必须为正";
来源：http://ksm.bbcook.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://leo.fanxiaobao.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://ego.52xcode.cn

C#:   Debug.Assert(x > 0);
来源：http://opy.ppjwa.cn

[H08] 获取错误信息与堆栈
来源：http://jdn.nwbrower.top

Py:   str(e);  traceback.format_exc()
来源：http://wen.yueranfly.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ihz.tianlin.xyz

JS:   e.message;  e.stack
来源：http://qho.zhaomingkeji.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://ock.dashuyun.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kzt.yuanzhike.top

Go:   err.Error()
来源：http://ivw.pengpengdd.cyou

Ruby: e.message;  e.backtrace
来源：http://ill.fengsongda.top

C#:   e.Message;  e.StackTrace
来源：http://bql.hammf.cn

[H09] 带错误码的异常
来源：http://wve.yongpay.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zxl.ydjk.org.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://tiq.cashguo.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tlk.wangshuangyany.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zvk.gaohongyu789.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pyz.snrcjt.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mor.fehbvm.com

Ruby: raise MyError.new("fail", 500)
来源：http://nwv.jyoumei.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yfn.wangdashe.top

[H10] 资源自动释放
来源：http://vyz.yfazqb.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://dcr.shanyushiyangtech.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zng.ctjpmb.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zbx.vehdjk.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sqf.pycfn.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ktm.guannengcc.top

Go:   defer f.Close()
来源：http://hpa.jinghuilouyu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wvm.zdbjq.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sic.guannengcc.top

================================================================================
来源：http://yeo.fanxiaobao.xyz

I. 正则表达式
来源：http://raq.andypj.xyz

================================================================================
来源：http://koq.pycfn.com

[I01] 判断是否匹配
来源：http://hys.cheryme.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cxs.jiagoushi.top

PHP:  preg_match('/\d+/', $s);
来源：http://sfl.jiagoushi.top

JS:   /\d+/.test(s)
来源：http://dtc.yueranfly.top

TS:   /\d+/.test(s)
来源：http://jcz.nanxinkj.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://srm.fktsv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://oqt.ctjpmb.com

Ruby: s.match?(/\d+/)
来源：http://xpy.tian-w.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bnh.wangshuangyany.cn

[I02] 提取所有匹配
来源：http://pso.c1oappe.top

Py:   re.findall(r"\d+", s)
来源：http://mgv.birdmap.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xva.dashuyun.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ivx.kuanghao11.cn

TS:   s.match(/\d+/g)
来源：http://mqv.uphjek.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dfr.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uca.sjlbkw.cn

Ruby: s.scan(/\d+/)
来源：http://bnr.yangfankeji.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ydy.zycfv.cn

[I03] 提取捕获分组
来源：http://xpy.hcnkem.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bjo.tianlin.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://aun.xuanzx.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xmh.52xcode.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zck.mhx1999.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zuf.ybcxt.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zbh.hongshengwenyu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hyk.vehdjk.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tar.pycfn.com

[I04] 正则替换
来源：http://rin.fengsongda.top

Py:   re.sub(r"\d+", "#", s)
来源：http://sry.vehdjk.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vzv.uphjek.com

JS:   s.replace(/\d+/g, "#")
来源：http://rut.sufxvd.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vze.zhiwuduotai.top

Java: s.replaceAll("\\d+", "#")
来源：http://zpf.dashuyun.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kqj.9152youxi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cbn.fengsongda.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ahe.nanxuanxn.top

[I05] 按正则拆分
来源：http://zym.shanyushiyangtech.top


<!-- 参考信息 -->