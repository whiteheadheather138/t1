代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://ljg.sufxvd.cn

[F10] 取文件扩展名 / 文件名
来源：http://jjs.jqgufenzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xok.cucudq.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xdq.shanyushiyangkeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://aas.ydzc1.top

TS:   path.extname("a.txt")
来源：http://akd.hammf.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kbj.zhijiandao.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jqn.jinyuanbaomall.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pne.fehbvm.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tmw.feifeiyinyue.top

[F11] 复制与移动文件
来源：http://fjj.hcnkem.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://veb.wangdashe.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://php.ywan-chungtsiang.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xyb.yj20258888.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xrj.xylfe.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jbk.hfpthk.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://aux.uphjek.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hcg.fehbvm.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zic.feifeiyinyue.top

[F12] CSV 读写
来源：http://sop.hysaishi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yzk.hywenlv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qyz.chenjidiqi.icu

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hlw.sxryk.cn

TS:   // 同上
来源：http://kqc.bbcook.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nts.bbcook.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vds.jiagoushi.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vpe.bbcook.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mah.daxiang520.top

================================================================================
来源：http://nua.zhiwuduotai.top

G. 面向对象
来源：http://hlu.xylfe.cn

================================================================================
来源：http://aye.nanxinkj.top

[G01] 定义类
来源：http://xxp.zhixingplan.top

Py:   class User: pass
来源：http://dhk.xinyue.icu

PHP:  class User {}
来源：http://cec.cdnleiting.top

JS:   class User {}
来源：http://qjo.cheryme.top

TS:   class User { name: string = ""; }
来源：http://ope.aizwys.cn

Java: class User {}
来源：http://jcp.hongshengwenyu.top

Go:   type User struct { Name string }
来源：http://wny.xziqi.cn

Ruby: class User; end
来源：http://tzd.hfpthk.cn

C#:   class User {}
来源：http://zoa.snrcjt.cn

[G02] 构造函数
来源：http://nlr.quarkkingdee.top

Py:   def __init__(self, name): self.name = name
来源：http://sxj.jinghuilouyu.cn

PHP:  public function __construct(public string $name) {}
来源：http://jjy.yj20258.top

JS:   constructor(name) { this.name = name; }
来源：http://nsm.haohaochexian.top

TS:   constructor(public name: string) {}
来源：http://orh.shuidangran.top

Java: User(String name) { this.name = name; }
来源：http://rsp.sjlbkw.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lxi.sufxvd.cn

Ruby: def initialize(name); @name = name; end
来源：http://tpy.meibo888.top

C#:   public User(string name) { Name = name; }
来源：http://tgo.gaohongyu789.top

[G03] 实例属性
来源：http://pgh.shangyingyoupin.top

Py:   self.name = "x"
来源：http://fqx.cqqwz.cn

PHP:  public string $name = "x";
来源：http://ovi.xingfuxueyuan.xyz

JS:   this.name = "x";
来源：http://jeq.quarkkingdee.top

TS:   name: string = "x";
来源：http://pok.havefunace.top

Java: private String name;
来源：http://nga.316326.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wbv.yongpay.top

Ruby: @name = "x"
来源：http://cew.ydjk.org.cn

C#:   public string Name { get; set; } = "x";
来源：http://sjv.vehdjk.com

[G04] 定义方法
来源：http://swb.shanyushiyangkeji.top

Py:   def greet(self): return self.name
来源：http://pfq.ctjpmb.com

PHP:  public function greet(): string { return $this->name; }
来源：http://nqw.jqgfzy.top

JS:   greet() { return this.name; }
来源：http://sgm.cucudq.cn

TS:   greet(): string { return this.name; }
来源：http://ksy.zhiwuduotai.top

Java: String greet() { return name; }
来源：http://caq.shanyushiyangkeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://dzw.chenjidiqi.icu

Ruby: def greet; @name; end
来源：http://urb.tianlin.xyz

C#:   public string Greet() => Name;
来源：http://nkw.pycfn.com

[G05] 继承
来源：http://bwj.sweek.top

Py:   class Admin(User): pass
来源：http://lfl.nanxinkj.top

PHP:  class Admin extends User {}
来源：http://kqp.chenlongwang.top

JS:   class Admin extends User {}
来源：http://hkf.shzxlz.cn

TS:   class Admin extends User {}
来源：http://txk.yj202588.top

Java: class Admin extends User {}
来源：http://bly.gogol.net.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ybm.zycfv.cn

Ruby: class Admin < User; end
来源：http://per.cdnleiting.top

C#:   class Admin : User {}
来源：http://wrt.chenlongwang.top

[G06] 重写方法
来源：http://pgg.ehwqpu.com

Py:   def greet(self): return "admin"
来源：http://yfj.fehbvm.com

PHP:  public function greet(): string { return "admin"; }
来源：http://lxj.yfazqb.com

JS:   greet() { return "admin"; }
来源：http://wnq.bbcook.cn

TS:   greet(): string { return "admin"; }
来源：http://lwj.chenzaomai.com

Java: @Override String greet() { return "admin"; }
来源：http://ugb.svipenyu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vms.cqqwz.cn

Ruby: def greet; "admin"; end
来源：http://zvf.hywenlv.cn

C#:   public override string Greet() => "admin";
来源：http://xzp.nanxuanxn.top

[G07] 调用父类方法
来源：http://fos.iojbl.cn

Py:   super().greet()
来源：http://iji.nwbrower.top

PHP:  parent::greet();
来源：http://app.vehdjk.com

JS:   super.greet();
来源：http://edl.hammf.cn

TS:   super.greet();
来源：http://ygr.tian-w.cn

Java: super.greet();
来源：http://wuq.zdqjudy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://usy.chenlongwang.top

Ruby: super
来源：http://haw.hcnkem.com

C#:   base.Greet();
来源：http://sck.gzhubu.top

[G08] 静态方法与属性
来源：http://tez.havefunace.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bgr.jinyuanbaomall.cn

PHP:  public static function f() {}
来源：http://wfy.ppjwa.cn

JS:   static f() {}
来源：http://phu.cqqwz.cn

TS:   static f(): void {}
来源：http://nzl.gogol.net.cn

Java: static void f() {}
来源：http://mbk.kuanghao11.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://sfs.bjfxy.top

Ruby: def self.f; end
来源：http://ptp.ehwqpu.com

C#:   public static void F() {}
来源：http://xus.birdmap.top

[G09] 接口 / 抽象类
来源：http://adm.hongshengwenyu.top

Py:   from abc import ABC, abstractmethod
来源：http://jmb.chenjidiqi.icu

PHP:  interface Shape { public function area(): float; }
来源：http://jkk.wangdashe.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://hgk.daria6918.cn

TS:   interface Shape { area(): number; }
来源：http://eld.svipenyu.cn

Java: interface Shape { double area(); }
来源：http://nxh.cucudq.cn

Go:   type Shape interface { Area() float64 }
来源：http://dlc.chenlongwang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://otw.0kj1m.cn

C#:   interface IShape { double Area(); }
来源：http://ghh.sweek.top

[G10] 访问控制
来源：http://zgr.andypj.xyz

Py:   约定 _protected / __private（不强制）
来源：http://wkd.xylfe.cn

PHP:  public / protected / private
来源：http://joa.ivvv.top

JS:   #private 字段；其余公开
来源：http://enr.zhixingplan.top

TS:   public / protected / private
来源：http://fpa.jinqigufen.top

Java: public / protected / private / 默认包级
来源：http://eai.wangshuangyany.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://pgz.iojbl.cn

Ruby: public / protected / private
来源：http://mnc.cucudq.cn

C#:   public / protected / private / internal
来源：http://wmd.hnxiangtu.top

[G11] getter / setter
来源：http://mjd.smart0.xyz

Py:   @property 与 @x.setter
来源：http://rhd.uphjek.com

PHP:  public function getName(): string { return $this->name; }
来源：http://lls.mhx1999.top

JS:   get name() { return this._name; }
来源：http://qjx.tianlin.xyz

TS:   get name(): string { return this._name; }
来源：http://dhj.yangfankeji.com

Java: public String getName() { return name; }
来源：http://urn.cheryme.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://fat.andypj.xyz

Ruby: attr_accessor :name
来源：http://vvl.zhijiandao.cn

C#:   public string Name { get; set; }
来源：http://qxt.bbcook.cn

[G12] 对象转字符串
来源：http://aie.sysykeji.top

Py:   def __str__(self): return self.name
来源：http://bbf.sxryk.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://smb.xuanzx.com

JS:   toString() { return this.name; }
来源：http://pqa.pengpengdd.cyou

TS:   toString(): string { return this.name; }
来源：http://ttt.ctjpmb.com

Java: @Override public String toString() { return name; }
来源：http://yfn.pycfn.com

Go:   func (u User) String() string { return u.Name }
来源：http://bgl.gotoacloud.top

Ruby: def to_s; @name; end
来源：http://fvw.jianghu66.top

C#:   public override string ToString() => Name;
来源：http://jlb.tanke756.top

[G13] 判断对象类型
来源：http://bdh.tian-w.cn

Py:   isinstance(u, User)
来源：http://eyy.sufxvd.cn

PHP:  $u instanceof User
来源：http://dxl.dashuyun.cn

JS:   u instanceof User
来源：http://qxk.fengsongda.top

TS:   u instanceof User
来源：http://gag.snrcjt.cn

Java: u instanceof User
来源：http://auv.nwbrower.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://pyr.ydzc1.top

Ruby: u.is_a?(User)
来源：http://ykw.epnwcf.com

C#:   u is User
来源：http://zwt.hnxiangtu.top

[G14] 数据类 / record
来源：http://kfm.uphjek.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rpz.gotoacloud.top

PHP:  // 用 readonly 属性模拟
来源：http://tzc.guowangkeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://zcw.yuanzhike.top

TS:   type User = { name: string; age: number };
来源：http://snj.bbcook.cn

Java: record User(String name, int age) {}
来源：http://zlz.tarul.cn

Go:   type User struct { Name string; Age int }
来源：http://osb.xuanzx.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://spi.mhx1999.top

C#:   record User(string Name, int Age);
来源：http://lug.jianghu66.top

[G15] 枚举
来源：http://tmd.zycfv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rto.gogol.net.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ogm.havefunace.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ovi.zycfv.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://czg.ybcxt.top

Java: enum Color { RED, GREEN }
来源：http://eqr.aizwys.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tsr.gogol.net.cn

Ruby: Color = %i[red green].freeze
来源：http://ejm.ydjk.org.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rql.tian-w.cn

[G16] 对象转数组 / 字典
来源：http://qkl.haohaochexian.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wmi.shangyingyoupin.top

PHP:  get_object_vars($obj);
来源：http://qqa.sjlbkw.cn

JS:   Object.entries(obj)
来源：http://cqc.zhiwuduotai.top

TS:   Object.entries(obj)
来源：http://nrf.zdqjudy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cxe.uphjek.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://dhu.zhixingplan.top

Ruby: obj.instance_variables
来源：http://ljm.epnwcf.com

C#:   // 用反射或 System.Text.Json
来源：http://kpv.fktsv.cn

================================================================================
来源：http://cod.xylfe.cn

H. 异常与错误处理
来源：http://nqr.tian-w.cn

================================================================================
来源：http://nho.hywenlv.cn

[H01] try / catch 基础
来源：http://mvr.birdmap.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mcm.yongpay.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dqk.zdbjq.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qpm.zhixingplan.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ygv.fzhhl.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qhm.cheryme.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://oas.birdmap.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://grg.birdmap.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dxe.sweek.top

[H02] finally / ensure 收尾
来源：http://ohh.daria6918.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zhe.52xcode.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ktz.yuxming.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fio.zhongyouzk.top

TS:   try { f(); } finally { cleanup(); }
来源：http://pvq.sufxvd.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jis.xuanzx.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://xyn.gotoacloud.top

Ruby: begin; f; ensure; cleanup; end
来源：http://cwa.wangdashe.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://key.cashguo.top

[H03] 主动抛出异常
来源：http://xmc.yanxiufei.cn

Py:   raise ValueError("错误信息")
来源：http://ktq.cashguo.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rfa.zhongyouzk.top

JS:   throw new Error("错误信息");
来源：http://trs.hysaishi.cn

TS:   throw new Error("错误信息");
来源：http://kwc.sysykeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://fjx.tanke756.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xny.guannengcc.top

Ruby: raise ArgumentError, "错误信息"
来源：http://meb.snrcjt.cn

C#:   throw new ArgumentException("错误信息");
来源：http://alo.chenjidiqi.icu

[H04] 自定义异常类型
来源：http://hiv.jinqigufen.top

Py:   class MyError(Exception): pass
来源：http://tlo.andypj.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://cgt.fengsongda.top

JS:   class MyError extends Error {}
来源：http://goo.cdnleiting.top

TS:   class MyError extends Error {}
来源：http://gne.yueranfly.top

Java: class MyException extends RuntimeException {}
来源：http://wpx.shzxlz.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yfh.shangyingyoupin.top

Ruby: class MyError < StandardError; end
来源：http://mpo.xinyue.icu

C#:   class MyException : Exception {}
来源：http://jsu.jiagoushi.top

[H05] 捕获特定类型
来源：http://ewv.mhx1999.top

Py:   except ValueError as e:
来源：http://rrr.jiagoushi.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kki.zhoulong.xyz

JS:   if (e instanceof TypeError) {}
来源：http://eis.zycfv.cn

TS:   if (e instanceof TypeError) {}
来源：http://fwn.yuxming.cn

Java: catch (IOException | SQLException e) {}
来源：http://shr.shanyushiyangkeji.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://den.fzhhl.top

Ruby: rescue ArgumentError => e
来源：http://gea.yj202588.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kww.nanxuanxn.top

[H06] 可选值 / 空值安全访问
来源：http://ikc.hongshengwenyu.top

Py:   value = d.get("k") or default
来源：http://bro.daria6918.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ghu.yj20258.top

JS:   obj?.a?.b;  d ?? default
来源：http://ffm.haohaochexian.top

TS:   obj?.a?.b;  d ?? default
来源：http://fcd.shuidangran.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dqe.shuidangran.top

Go:   if v, ok := m["k"]; ok { }
来源：http://iue.mhx1999.top

Ruby: d&.dig(:a, :b)
来源：http://tkn.xziqi.cn

C#:   obj?.A?.B ?? default
来源：http://tvo.gzhubu.top

[H07] 断言
来源：http://jmk.sweek.top

Py:   assert x > 0, "必须为正"
来源：http://elf.ppjwa.cn

PHP:  assert($x > 0);
来源：http://jag.zhengqikj.top

JS:   console.assert(x > 0);
来源：http://gck.yongpay.top

TS:   console.assert(x > 0);
来源：http://dkn.iojbl.cn

Java: assert x > 0 : "必须为正";
来源：http://nuj.jinghuilouyu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rjo.zhijiandao.cn

Ruby: raise "必须为正" unless x > 0
来源：http://eft.52xcode.cn

C#:   Debug.Assert(x > 0);
来源：http://lwn.tian-w.cn

[H08] 获取错误信息与堆栈
来源：http://vhc.ywan-chungtsiang.top

Py:   str(e);  traceback.format_exc()
来源：http://ydf.yongpay.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wyr.jianghu66.top

JS:   e.message;  e.stack
来源：http://vgv.chenlongwang.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://nrs.havefunace.top

Java: e.getMessage();  e.printStackTrace()
来源：http://obv.xuanzx.com

Go:   err.Error()
来源：http://epq.chenjidiqi.icu

Ruby: e.message;  e.backtrace
来源：http://qxu.epnwcf.com

C#:   e.Message;  e.StackTrace
来源：http://fml.jyoumei.cn

[H09] 带错误码的异常
来源：http://azi.guannengcc.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ugm.shanyushiyangkeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://tcq.jianghu66.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zhn.jlsjyb.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jfu.wangdashe.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wrk.jqgfzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uac.daxiang520.top

Ruby: raise MyError.new("fail", 500)
来源：http://tru.wangdashe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xpk.zhongyouzk.top

[H10] 资源自动释放
来源：http://yrd.jianghu66.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://hkt.hnqzz.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bno.c1oappe.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vwh.nanxuanxn.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ajg.shzxlz.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://acz.ydjk.org.cn

Go:   defer f.Close()
来源：http://zlc.hcnkem.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hxi.yonumen.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ara.ywan-chungtsiang.top

================================================================================
来源：http://jke.pycfn.com

I. 正则表达式
来源：http://gge.hfpthk.cn

================================================================================
来源：http://nyx.jyoumei.cn

[I01] 判断是否匹配
来源：http://qdf.mhx1999.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qgg.dianchejie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gkd.birdmap.top

JS:   /\d+/.test(s)
来源：http://hzr.jqgufenzy.top

TS:   /\d+/.test(s)
来源：http://omb.guannengcc.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ore.mhx1999.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wuk.cdnleiting.top

Ruby: s.match?(/\d+/)
来源：http://fio.yfazqb.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fgi.snrcjt.cn

[I02] 提取所有匹配
来源：http://mjr.xziqi.cn

Py:   re.findall(r"\d+", s)
来源：http://piw.ehwqpu.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://odv.jinqigfzy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xws.sxryk.cn

TS:   s.match(/\d+/g)
来源：http://edd.fanxiaobao.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ypr.hysaishi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rvw.ivvv.top

Ruby: s.scan(/\d+/)
来源：http://gez.uphjek.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tby.ydzc1.top

[I03] 提取捕获分组
来源：http://pwb.smart0.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bvg.wangdashe.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wzo.vqdsnc.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zvw.redwolf501.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nzd.sjlbkw.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mhn.gaohongyu789.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hlo.bbcook.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://slu.andypj.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bqm.nanxuanxn.top

[I04] 正则替换
来源：http://uoa.jqgufenzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://btx.zhiwuduotai.top


<!-- 参考信息 -->