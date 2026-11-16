代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://heq.jiagoushi.top

[F10] 取文件扩展名 / 文件名
来源：http://hfc.nwbrower.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hwg.hysaishi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wfh.jqgufenzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hix.gogol.net.cn

TS:   path.extname("a.txt")
来源：http://rcc.nanxuanxn.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://asl.jinghuilouyu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kda.hnqzz.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lth.316326.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sxv.cqqwz.cn

[F11] 复制与移动文件
来源：http://qiu.sysykeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ivi.jinyuanbaomall.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ond.chenzaomai.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mcb.yonumen.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vrv.ehwqpu.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ejt.ctjpmb.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pht.yj20258888.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fzk.hongshengwenyu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yvj.zhijiandao.cn

[F12] CSV 读写
来源：http://coo.yvedp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pzd.hysaishi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wup.feifeiyinyue.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://suw.zhoulong.xyz

TS:   // 同上
来源：http://tne.zhaomingkeji.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://seu.hongshengwenyu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hhu.jlsjyb.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hwy.xziqi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qpt.smart0.xyz

================================================================================
来源：http://czp.svipenyu.cn

G. 面向对象
来源：http://ggw.jinqigufen.top

================================================================================
来源：http://yqj.nanxuanxn.top

[G01] 定义类
来源：http://for.ehwqpu.com

Py:   class User: pass
来源：http://hme.dianchejie.cn

PHP:  class User {}
来源：http://jxw.dashuyun.cn

JS:   class User {}
来源：http://diu.jqgfzy.top

TS:   class User { name: string = ""; }
来源：http://goo.jianghu66.top

Java: class User {}
来源：http://vyp.yj202588.top

Go:   type User struct { Name string }
来源：http://dqg.snrcjt.cn

Ruby: class User; end
来源：http://hlz.yj202588.top

C#:   class User {}
来源：http://icr.c1oappe.top

[G02] 构造函数
来源：http://wgv.tarul.cn

Py:   def __init__(self, name): self.name = name
来源：http://izw.tanke756.top

PHP:  public function __construct(public string $name) {}
来源：http://fcz.hammf.cn

JS:   constructor(name) { this.name = name; }
来源：http://zru.chenlongwang.top

TS:   constructor(public name: string) {}
来源：http://hej.hammf.cn

Java: User(String name) { this.name = name; }
来源：http://loo.jinghuilouyu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uwp.meibo888.top

Ruby: def initialize(name); @name = name; end
来源：http://abz.jqgfzy.top

C#:   public User(string name) { Name = name; }
来源：http://hgp.pengpengdd.cyou

[G03] 实例属性
来源：http://hlx.hammf.cn

Py:   self.name = "x"
来源：http://buh.jinyuanbaomall.cn

PHP:  public string $name = "x";
来源：http://osg.jyoumei.cn

JS:   this.name = "x";
来源：http://nwp.feifeiyinyue.top

TS:   name: string = "x";
来源：http://ibp.jlsjyb.cn

Java: private String name;
来源：http://xdb.sxryk.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kfg.yuanzhike.top

Ruby: @name = "x"
来源：http://rri.zhixingplan.top

C#:   public string Name { get; set; } = "x";
来源：http://ulz.ppjwa.cn

[G04] 定义方法
来源：http://aos.daxiang520.top

Py:   def greet(self): return self.name
来源：http://owk.yj202588.top

PHP:  public function greet(): string { return $this->name; }
来源：http://yfm.uphjek.com

JS:   greet() { return this.name; }
来源：http://sfe.tianlin.xyz

TS:   greet(): string { return this.name; }
来源：http://ckm.sjlbkw.cn

Java: String greet() { return name; }
来源：http://eke.daxiang520.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://jmy.jqgfzy.top

Ruby: def greet; @name; end
来源：http://jqx.0kj1m.cn

C#:   public string Greet() => Name;
来源：http://qdy.yongpay.top

[G05] 继承
来源：http://gsy.ppjwa.cn

Py:   class Admin(User): pass
来源：http://ekw.ehwqpu.com

PHP:  class Admin extends User {}
来源：http://bgd.hnxiangtu.top

JS:   class Admin extends User {}
来源：http://xdk.chenlongwang.top

TS:   class Admin extends User {}
来源：http://vjg.hywenlv.cn

Java: class Admin extends User {}
来源：http://tbr.nanxinkj.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://slx.sweek.top

Ruby: class Admin < User; end
来源：http://vfm.wangdashe.top

C#:   class Admin : User {}
来源：http://aqe.hywenlv.cn

[G06] 重写方法
来源：http://dhp.yuxming.cn

Py:   def greet(self): return "admin"
来源：http://tmr.fehbvm.com

PHP:  public function greet(): string { return "admin"; }
来源：http://xnz.shanyushiyangtech.top

JS:   greet() { return "admin"; }
来源：http://yvl.gotoacloud.top

TS:   greet(): string { return "admin"; }
来源：http://yyz.zycfv.cn

Java: @Override String greet() { return "admin"; }
来源：http://nve.jyoumei.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qvp.jinghuilouyu.cn

Ruby: def greet; "admin"; end
来源：http://oln.gaohongyu789.top

C#:   public override string Greet() => "admin";
来源：http://oua.haohaochexian.top

[G07] 调用父类方法
来源：http://whb.vqdsnc.cn

Py:   super().greet()
来源：http://ifs.zhongyouzk.top

PHP:  parent::greet();
来源：http://vuo.sweek.top

JS:   super.greet();
来源：http://pre.sufxvd.cn

TS:   super.greet();
来源：http://vjh.yj20258888.top

Java: super.greet();
来源：http://elj.fktsv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zap.ydjk.org.cn

Ruby: super
来源：http://yhc.zhixingplan.top

C#:   base.Greet();
来源：http://rnb.zhijiandao.cn

[G08] 静态方法与属性
来源：http://ply.mhx1999.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://awq.redwolf501.top

PHP:  public static function f() {}
来源：http://ksv.shangyingyoupin.top

JS:   static f() {}
来源：http://kev.zhijiandao.cn

TS:   static f(): void {}
来源：http://lmn.wangdashe.top

Java: static void f() {}
来源：http://rai.yj20258888.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://jme.zhixingplan.top

Ruby: def self.f; end
来源：http://msd.zhongyouzk.top

C#:   public static void F() {}
来源：http://ace.jinqigfzy.top

[G09] 接口 / 抽象类
来源：http://yvp.jinqigufen.top

Py:   from abc import ABC, abstractmethod
来源：http://fhk.kuanghao11.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jru.fengsongda.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://pej.hongshengwenyu.top

TS:   interface Shape { area(): number; }
来源：http://bwd.havefunace.top

Java: interface Shape { double area(); }
来源：http://mgm.jlsjyb.cn

Go:   type Shape interface { Area() float64 }
来源：http://czc.zhaomingkeji.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ilq.dianchejie.cn

C#:   interface IShape { double Area(); }
来源：http://xav.yj20258.top

[G10] 访问控制
来源：http://pcx.yj20258888.top

Py:   约定 _protected / __private（不强制）
来源：http://ekt.bjfxy.top

PHP:  public / protected / private
来源：http://tpw.xinyue.icu

JS:   #private 字段；其余公开
来源：http://mlo.bbcook.cn

TS:   public / protected / private
来源：http://bqv.aibaodan.cn

Java: public / protected / private / 默认包级
来源：http://wjg.bbcook.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://esp.yfazqb.com

Ruby: public / protected / private
来源：http://jra.gogol.net.cn

C#:   public / protected / private / internal
来源：http://brf.shanyushiyangtech.top

[G11] getter / setter
来源：http://bxw.shanyushiyangtech.top

Py:   @property 与 @x.setter
来源：http://njh.zhixingplan.top

PHP:  public function getName(): string { return $this->name; }
来源：http://otg.ivvv.top

JS:   get name() { return this._name; }
来源：http://swb.tian-w.cn

TS:   get name(): string { return this._name; }
来源：http://wje.hcnkem.com

Java: public String getName() { return name; }
来源：http://xhx.bbcook.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dif.yueranfly.top

Ruby: attr_accessor :name
来源：http://gho.cdnleiting.top

C#:   public string Name { get; set; }
来源：http://lmq.ydzc1.top

[G12] 对象转字符串
来源：http://npk.ppjwa.cn

Py:   def __str__(self): return self.name
来源：http://gos.hongshengwenyu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://xzs.ppjwa.cn

JS:   toString() { return this.name; }
来源：http://gei.wangdashe.top

TS:   toString(): string { return this.name; }
来源：http://sdp.jinyuanbaomall.cn

Java: @Override public String toString() { return name; }
来源：http://fyf.daria6918.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ole.mhx1999.top

Ruby: def to_s; @name; end
来源：http://jyi.guannengcc.top

C#:   public override string ToString() => Name;
来源：http://lpv.mhx1999.top

[G13] 判断对象类型
来源：http://tod.jiagoushi.top

Py:   isinstance(u, User)
来源：http://uwb.kuanghao11.cn

PHP:  $u instanceof User
来源：http://vbt.hywenlv.cn

JS:   u instanceof User
来源：http://jur.hysaishi.cn

TS:   u instanceof User
来源：http://pkz.hammf.cn

Java: u instanceof User
来源：http://yvv.fengsongda.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://itw.tarul.cn

Ruby: u.is_a?(User)
来源：http://bok.vqdsnc.cn

C#:   u is User
来源：http://yit.yueranfly.top

[G14] 数据类 / record
来源：http://qjr.dashuyun.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jhm.birdmap.top

PHP:  // 用 readonly 属性模拟
来源：http://wrt.gotoacloud.top

JS:   // 无内置：普通类或对象字面量
来源：http://kjy.hesvh.cn

TS:   type User = { name: string; age: number };
来源：http://erm.tanke756.top

Java: record User(String name, int age) {}
来源：http://dgl.jinqigfzy.top

Go:   type User struct { Name string; Age int }
来源：http://jln.yueranfly.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://eud.yj202588.top

C#:   record User(string Name, int Age);
来源：http://kyk.shangyingyoupin.top

[G15] 枚举
来源：http://qpg.xinyue.icu

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fdy.nanxinkj.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://vmj.wangdashe.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kan.sufxvd.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://luk.daria6918.cn

Java: enum Color { RED, GREEN }
来源：http://jiw.yanxiufei.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hsc.hysaishi.cn

Ruby: Color = %i[red green].freeze
来源：http://wyi.meibo888.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ass.hesvh.cn

[G16] 对象转数组 / 字典
来源：http://uvx.wangdashe.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ymu.hfpthk.cn

PHP:  get_object_vars($obj);
来源：http://arx.zhongyouzk.top

JS:   Object.entries(obj)
来源：http://lnp.dashuyun.cn

TS:   Object.entries(obj)
来源：http://qix.gzhubu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rww.jiagoushi.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://hga.meibo888.top

Ruby: obj.instance_variables
来源：http://ntg.jyoumei.cn

C#:   // 用反射或 System.Text.Json
来源：http://kbs.sweek.top

================================================================================
来源：http://ngz.hfpthk.cn

H. 异常与错误处理
来源：http://goj.gotoacloud.top

================================================================================
来源：http://brx.sysykeji.top

[H01] try / catch 基础
来源：http://egy.gaohongyu789.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://plq.wangshuangyany.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://djt.zdbjq.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cin.jlsjyb.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gin.yueranfly.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jzp.gzhubu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wqi.jiagoushi.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://toj.xingfuxueyuan.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bmv.pengpengdd.cyou

[H02] finally / ensure 收尾
来源：http://klu.zhixingplan.top

Py:   try: f()⏎finally: cleanup()
来源：http://aap.dashuyun.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tjq.ppjwa.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jor.andypj.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://zjh.fengsongda.top

Java: try { f(); } finally { cleanup(); }
来源：http://leu.wangdashe.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ecc.bjfxy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ygg.hnxiangtu.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ydv.mhx1999.top

[H03] 主动抛出异常
来源：http://gxb.feifeiyinyue.top

Py:   raise ValueError("错误信息")
来源：http://vyn.guowangkeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://alx.shanyushiyangkeji.top

JS:   throw new Error("错误信息");
来源：http://loj.fktsv.cn

TS:   throw new Error("错误信息");
来源：http://gxz.redwolf501.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://vve.ydjk.org.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wcf.guowangkeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://kqz.wangdashe.top

C#:   throw new ArgumentException("错误信息");
来源：http://raf.hongshengwenyu.top

[H04] 自定义异常类型
来源：http://arp.sjlbkw.cn

Py:   class MyError(Exception): pass
来源：http://zps.zhixingplan.top

PHP:  class MyError extends RuntimeException {}
来源：http://mhh.cheryme.top

JS:   class MyError extends Error {}
来源：http://hvk.fzhhl.top

TS:   class MyError extends Error {}
来源：http://gmy.zdbjq.cn

Java: class MyException extends RuntimeException {}
来源：http://esd.tianlin.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vgw.yj202588.top

Ruby: class MyError < StandardError; end
来源：http://wda.ydjk.org.cn

C#:   class MyException : Exception {}
来源：http://oen.zhengqikj.top

[H05] 捕获特定类型
来源：http://vjd.vehdjk.com

Py:   except ValueError as e:
来源：http://mdw.sysykeji.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qta.mhx1999.top

JS:   if (e instanceof TypeError) {}
来源：http://ibt.shangyingyoupin.top

TS:   if (e instanceof TypeError) {}
来源：http://kzr.c1oappe.top

Java: catch (IOException | SQLException e) {}
来源：http://xqg.sweek.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://iqm.sufxvd.cn

Ruby: rescue ArgumentError => e
来源：http://fiz.zhaomingkeji.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ank.bbcook.cn

[H06] 可选值 / 空值安全访问
来源：http://uoo.sxryk.cn

Py:   value = d.get("k") or default
来源：http://amh.chenlongwang.top

PHP:  $v = $d["k"] ?? null;
来源：http://ilz.birdmap.top

JS:   obj?.a?.b;  d ?? default
来源：http://nqr.yueranfly.top

TS:   obj?.a?.b;  d ?? default
来源：http://whb.hesvh.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xcf.yvedp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://par.guowangkeji.top

Ruby: d&.dig(:a, :b)
来源：http://bqm.jinqigfzy.top

C#:   obj?.A?.B ?? default
来源：http://zws.fehbvm.com

[H07] 断言
来源：http://nkx.jianghu66.top

Py:   assert x > 0, "必须为正"
来源：http://cdp.xziqi.cn

PHP:  assert($x > 0);
来源：http://ldt.0kj1m.cn

JS:   console.assert(x > 0);
来源：http://msd.daria6918.cn

TS:   console.assert(x > 0);
来源：http://iki.yuxming.cn

Java: assert x > 0 : "必须为正";
来源：http://bwt.havefunace.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ykq.yonumen.top

Ruby: raise "必须为正" unless x > 0
来源：http://fba.jiagoushi.top

C#:   Debug.Assert(x > 0);
来源：http://qbj.shanyushiyangkeji.top

[H08] 获取错误信息与堆栈
来源：http://for.aizwys.cn

Py:   str(e);  traceback.format_exc()
来源：http://dog.smart0.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kht.pycfn.com

JS:   e.message;  e.stack
来源：http://lwn.ivvv.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://akz.meibo888.top

Java: e.getMessage();  e.printStackTrace()
来源：http://lts.yuanzhike.top

Go:   err.Error()
来源：http://fct.shanyushiyangtech.top

Ruby: e.message;  e.backtrace
来源：http://zab.hammf.cn

C#:   e.Message;  e.StackTrace
来源：http://qix.tian-w.cn

[H09] 带错误码的异常
来源：http://omc.tianlin.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fvm.shzxlz.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wnt.redwolf501.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://irr.yuxming.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yud.epnwcf.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blb.yj20258888.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lcm.guannengcc.top

Ruby: raise MyError.new("fail", 500)
来源：http://fxw.tanke756.top

C#:   // 自定义异常类中加 Code 属性
来源：http://bhg.zdbjq.cn

[H10] 资源自动释放
来源：http://iuh.wangshuangyany.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vwc.kuanghao11.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fue.jinqigufen.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lsc.daxiang520.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://shn.hfpthk.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://phh.yvedp.cn

Go:   defer f.Close()
来源：http://yhf.nwbrower.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ypa.hcnkem.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sgu.feifeiyinyue.top

================================================================================
来源：http://xjf.fktsv.cn

I. 正则表达式
来源：http://msw.jianghu66.top

================================================================================
来源：http://eij.hfpthk.cn

[I01] 判断是否匹配
来源：http://yme.hnxiangtu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yne.quarkkingdee.top

PHP:  preg_match('/\d+/', $s);
来源：http://why.fzhhl.top

JS:   /\d+/.test(s)
来源：http://wbd.svipenyu.cn

TS:   /\d+/.test(s)
来源：http://qzp.yangfankeji.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://eob.chenlongwang.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xfl.ppjwa.cn

Ruby: s.match?(/\d+/)
来源：http://hsf.yuanzhike.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sur.ybcxt.top

[I02] 提取所有匹配
来源：http://mdo.hongshengwenyu.top

Py:   re.findall(r"\d+", s)
来源：http://yxb.shzxlz.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hmd.ydzc1.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yvb.yuanzhike.top

TS:   s.match(/\d+/g)
来源：http://lqo.zdqjudy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yfu.yj20258888.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://izm.gzhubu.top

Ruby: s.scan(/\d+/)
来源：http://ndl.yanxiufei.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cag.cucudq.cn

[I03] 提取捕获分组
来源：http://lef.yvedp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kjj.shangyingyoupin.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bcq.uphjek.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hug.svipenyu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fqk.yueranfly.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dqx.zhijiandao.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vbq.aibaodan.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rap.yfazqb.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://exb.ydzc1.top

[I04] 正则替换
来源：http://bam.shzxlz.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mwc.uphjek.com


<!-- 参考信息 -->