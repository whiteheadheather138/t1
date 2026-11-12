代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://xjg.jianghu66.top

[F10] 取文件扩展名 / 文件名
来源：http://wht.haohaochexian.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bak.gogol.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wpx.zhoulong.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lmr.jinyuanbaomall.cn

TS:   path.extname("a.txt")
来源：http://xvv.c1oappe.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yvf.daria6918.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mko.hcnkem.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://agn.yanxiufei.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://eaz.bbcook.cn

[F11] 复制与移动文件
来源：http://xpt.snrcjt.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://irj.epnwcf.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sej.meibo888.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kun.kuanghao11.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cdk.zhengqikj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ugu.yuanzhike.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sla.epnwcf.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nlo.cqqwz.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ckn.ehwqpu.com

[F12] CSV 读写
来源：http://yyg.shanyushiyangkeji.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zch.yueranfly.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ogb.zhixingplan.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zpb.fktsv.cn

TS:   // 同上
来源：http://mui.dashuyun.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nsl.jinyuanbaomall.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kzo.dashuyun.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qzn.jinqigfzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://rfr.jinghuilouyu.cn

================================================================================
来源：http://oxz.svipenyu.cn

G. 面向对象
来源：http://lsy.yangfankeji.com

================================================================================
来源：http://pon.jinghuilouyu.cn

[G01] 定义类
来源：http://dnv.nanxinkj.top

Py:   class User: pass
来源：http://yji.zycfv.cn

PHP:  class User {}
来源：http://epc.andypj.xyz

JS:   class User {}
来源：http://imi.jinyuanbaomall.cn

TS:   class User { name: string = ""; }
来源：http://rnh.fanxiaobao.xyz

Java: class User {}
来源：http://dwf.zhoulong.xyz

Go:   type User struct { Name string }
来源：http://zzc.sysykeji.top

Ruby: class User; end
来源：http://weg.sxryk.cn

C#:   class User {}
来源：http://iol.jiagoushi.top

[G02] 构造函数
来源：http://nhk.epnwcf.com

Py:   def __init__(self, name): self.name = name
来源：http://wtg.ehwqpu.com

PHP:  public function __construct(public string $name) {}
来源：http://oal.hcnkem.com

JS:   constructor(name) { this.name = name; }
来源：http://mur.gogol.net.cn

TS:   constructor(public name: string) {}
来源：http://bap.yangfankeji.com

Java: User(String name) { this.name = name; }
来源：http://ytk.nanxinkj.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xpg.dianchejie.cn

Ruby: def initialize(name); @name = name; end
来源：http://ojv.jlsjyb.cn

C#:   public User(string name) { Name = name; }
来源：http://ckm.redwolf501.top

[G03] 实例属性
来源：http://ikm.shanyushiyangtech.top

Py:   self.name = "x"
来源：http://eiy.guowangkeji.top

PHP:  public string $name = "x";
来源：http://mas.hfpthk.cn

JS:   this.name = "x";
来源：http://dtx.sufxvd.cn

TS:   name: string = "x";
来源：http://kus.fzhhl.top

Java: private String name;
来源：http://hcp.yfazqb.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://igx.birdmap.top

Ruby: @name = "x"
来源：http://kvb.smart0.xyz

C#:   public string Name { get; set; } = "x";
来源：http://hau.vqdsnc.cn

[G04] 定义方法
来源：http://fvp.gotoacloud.top

Py:   def greet(self): return self.name
来源：http://xuy.jyoumei.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://cnh.jqgufenzy.top

JS:   greet() { return this.name; }
来源：http://ebb.hammf.cn

TS:   greet(): string { return this.name; }
来源：http://izp.sjlbkw.cn

Java: String greet() { return name; }
来源：http://evq.aibaodan.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lvy.birdmap.top

Ruby: def greet; @name; end
来源：http://bfd.fehbvm.com

C#:   public string Greet() => Name;
来源：http://sgi.zhiwuduotai.top

[G05] 继承
来源：http://dya.hcnkem.com

Py:   class Admin(User): pass
来源：http://kfw.hysaishi.cn

PHP:  class Admin extends User {}
来源：http://ahb.zhongyouzk.top

JS:   class Admin extends User {}
来源：http://ivr.hnxiangtu.top

TS:   class Admin extends User {}
来源：http://twg.zdbjq.cn

Java: class Admin extends User {}
来源：http://hun.cqqwz.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pmd.tianlin.xyz

Ruby: class Admin < User; end
来源：http://ybj.vehdjk.com

C#:   class Admin : User {}
来源：http://fkl.xuanzx.com

[G06] 重写方法
来源：http://koo.zhaomingkeji.xyz

Py:   def greet(self): return "admin"
来源：http://sug.ivvv.top

PHP:  public function greet(): string { return "admin"; }
来源：http://szq.jinqigfzy.top

JS:   greet() { return "admin"; }
来源：http://xjj.dianchejie.cn

TS:   greet(): string { return "admin"; }
来源：http://lny.dianchejie.cn

Java: @Override String greet() { return "admin"; }
来源：http://jrl.pengpengdd.cyou

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sjg.shanyushiyangtech.top

Ruby: def greet; "admin"; end
来源：http://hnm.gaohongyu789.top

C#:   public override string Greet() => "admin";
来源：http://fmw.hongshengwenyu.top

[G07] 调用父类方法
来源：http://hxu.shuidangran.top

Py:   super().greet()
来源：http://vxm.hcnkem.com

PHP:  parent::greet();
来源：http://aey.zhiwuduotai.top

JS:   super.greet();
来源：http://cmg.chenjidiqi.icu

TS:   super.greet();
来源：http://uuw.nanxinkj.top

Java: super.greet();
来源：http://yhm.shzxlz.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bny.quarkkingdee.top

Ruby: super
来源：http://aag.fengsongda.top

C#:   base.Greet();
来源：http://zjd.shanyushiyangtech.top

[G08] 静态方法与属性
来源：http://vtv.feifeiyinyue.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jbs.ivvv.top

PHP:  public static function f() {}
来源：http://udu.shuidangran.top

JS:   static f() {}
来源：http://jpw.yj20258.top

TS:   static f(): void {}
来源：http://dtt.aizwys.cn

Java: static void f() {}
来源：http://ekt.ydzc1.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://jhz.gaohongyu789.top

Ruby: def self.f; end
来源：http://ivf.xuetiantiany.cn

C#:   public static void F() {}
来源：http://cqc.nanxuanxn.top

[G09] 接口 / 抽象类
来源：http://jmn.dashuyun.cn

Py:   from abc import ABC, abstractmethod
来源：http://vsn.yuanzhike.top

PHP:  interface Shape { public function area(): float; }
来源：http://jnb.andypj.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://giz.dashuyun.cn

TS:   interface Shape { area(): number; }
来源：http://upv.zhaomingkeji.xyz

Java: interface Shape { double area(); }
来源：http://xbs.daria6918.cn

Go:   type Shape interface { Area() float64 }
来源：http://zyf.xinyue.icu

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tqx.uphjek.com

C#:   interface IShape { double Area(); }
来源：http://wsm.zhongyouzk.top

[G10] 访问控制
来源：http://fjt.hywenlv.cn

Py:   约定 _protected / __private（不强制）
来源：http://cjm.zhiwuduotai.top

PHP:  public / protected / private
来源：http://cwp.chenlongwang.top

JS:   #private 字段；其余公开
来源：http://pnr.redwolf501.top

TS:   public / protected / private
来源：http://qcm.xylfe.cn

Java: public / protected / private / 默认包级
来源：http://chm.ydzc1.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://cma.xuetiantiany.cn

Ruby: public / protected / private
来源：http://ehy.bjfxy.top

C#:   public / protected / private / internal
来源：http://yot.gogol.net.cn

[G11] getter / setter
来源：http://pjb.dianchejie.cn

Py:   @property 与 @x.setter
来源：http://muy.zhixingplan.top

PHP:  public function getName(): string { return $this->name; }
来源：http://yvi.c1oappe.top

JS:   get name() { return this._name; }
来源：http://okm.zhijiandao.cn

TS:   get name(): string { return this._name; }
来源：http://jnb.shanyushiyangtech.top

Java: public String getName() { return name; }
来源：http://lig.ehwqpu.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://csx.nwbrower.top

Ruby: attr_accessor :name
来源：http://exq.sysykeji.top

C#:   public string Name { get; set; }
来源：http://aqf.zycfv.cn

[G12] 对象转字符串
来源：http://qjc.xingfuxueyuan.xyz

Py:   def __str__(self): return self.name
来源：http://uof.uphjek.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://nex.aibaodan.cn

JS:   toString() { return this.name; }
来源：http://hpl.yongpay.top

TS:   toString(): string { return this.name; }
来源：http://xst.svipenyu.cn

Java: @Override public String toString() { return name; }
来源：http://ddm.svipenyu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xwv.xinyue.icu

Ruby: def to_s; @name; end
来源：http://ejp.tarul.cn

C#:   public override string ToString() => Name;
来源：http://ssm.jlsjyb.cn

[G13] 判断对象类型
来源：http://tis.nwbrower.top

Py:   isinstance(u, User)
来源：http://ebl.wangdashe.top

PHP:  $u instanceof User
来源：http://mak.zhijiandao.cn

JS:   u instanceof User
来源：http://cqy.yuanzhike.top

TS:   u instanceof User
来源：http://dgl.wangdashe.top

Java: u instanceof User
来源：http://mml.yuanzhike.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ycu.feifeiyinyue.top

Ruby: u.is_a?(User)
来源：http://pnp.dashuyun.cn

C#:   u is User
来源：http://exb.tanke756.top

[G14] 数据类 / record
来源：http://woe.epnwcf.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://iuk.chenlongwang.top

PHP:  // 用 readonly 属性模拟
来源：http://spd.c1oappe.top

JS:   // 无内置：普通类或对象字面量
来源：http://gof.aizwys.cn

TS:   type User = { name: string; age: number };
来源：http://nnk.yongpay.top

Java: record User(String name, int age) {}
来源：http://oro.316326.xyz

Go:   type User struct { Name string; Age int }
来源：http://aho.dashuyun.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tzq.svipenyu.cn

C#:   record User(string Name, int Age);
来源：http://mgg.vehdjk.com

[G15] 枚举
来源：http://xfn.0kj1m.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qbt.tarul.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dqg.yongpay.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rjj.smart0.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vtq.jyoumei.cn

Java: enum Color { RED, GREEN }
来源：http://nfe.zdbjq.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ose.yj20258.top

Ruby: Color = %i[red green].freeze
来源：http://ivw.0kj1m.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lmo.xingfuxueyuan.xyz

[G16] 对象转数组 / 字典
来源：http://fov.fktsv.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yxg.ybcxt.top

PHP:  get_object_vars($obj);
来源：http://rvn.aizwys.cn

JS:   Object.entries(obj)
来源：http://iia.shuidangran.top

TS:   Object.entries(obj)
来源：http://flo.shuidangran.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gbq.jinyuanbaomall.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://nyw.chenlongwang.top

Ruby: obj.instance_variables
来源：http://ypk.ywan-chungtsiang.top

C#:   // 用反射或 System.Text.Json
来源：http://mdl.bbcook.cn

================================================================================
来源：http://yhd.tanke756.top

H. 异常与错误处理
来源：http://srh.316326.xyz

================================================================================
来源：http://vxn.andypj.xyz

[H01] try / catch 基础
来源：http://qxr.hfpthk.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vxv.smart0.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dem.ydzc1.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dkq.ppjwa.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xes.sjlbkw.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jbc.gzhubu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sta.feifeiyinyue.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ygd.zhongyouzk.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kvl.kuanghao11.cn

[H02] finally / ensure 收尾
来源：http://kif.sjlbkw.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dcd.chenjidiqi.icu

PHP:  try { f(); } finally { cleanup(); }
来源：http://iih.nwbrower.top

JS:   try { f(); } finally { cleanup(); }
来源：http://qji.sysykeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://tub.ivvv.top

Java: try { f(); } finally { cleanup(); }
来源：http://ont.jinqigfzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://zzk.yj20258888.top

Ruby: begin; f; ensure; cleanup; end
来源：http://bhm.shangyingyoupin.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://sod.xingfuxueyuan.xyz

[H03] 主动抛出异常
来源：http://nah.meibo888.top

Py:   raise ValueError("错误信息")
来源：http://tjw.chenjidiqi.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ots.yanxiufei.cn

JS:   throw new Error("错误信息");
来源：http://lah.jianghu66.top

TS:   throw new Error("错误信息");
来源：http://zxo.yongpay.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hpg.cucudq.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wpz.wangdashe.top

Ruby: raise ArgumentError, "错误信息"
来源：http://kgc.hfpthk.cn

C#:   throw new ArgumentException("错误信息");
来源：http://seb.yvedp.cn

[H04] 自定义异常类型
来源：http://mnl.yj202588.top

Py:   class MyError(Exception): pass
来源：http://ksp.wangdashe.top

PHP:  class MyError extends RuntimeException {}
来源：http://jnf.zhengqikj.top

JS:   class MyError extends Error {}
来源：http://ubr.yongpay.top

TS:   class MyError extends Error {}
来源：http://cgg.jinyuanbaomall.cn

Java: class MyException extends RuntimeException {}
来源：http://cfc.dashuyun.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fos.ppjwa.cn

Ruby: class MyError < StandardError; end
来源：http://jtl.ydjk.org.cn

C#:   class MyException : Exception {}
来源：http://rtr.c1oappe.top

[H05] 捕获特定类型
来源：http://guw.shanyushiyangkeji.top

Py:   except ValueError as e:
来源：http://vih.ctjpmb.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ugl.gotoacloud.top

JS:   if (e instanceof TypeError) {}
来源：http://jnu.sweek.top

TS:   if (e instanceof TypeError) {}
来源：http://xzl.birdmap.top

Java: catch (IOException | SQLException e) {}
来源：http://fst.xuetiantiany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://khm.sufxvd.cn

Ruby: rescue ArgumentError => e
来源：http://xlq.shangyingyoupin.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lmc.dashuyun.cn

[H06] 可选值 / 空值安全访问
来源：http://gel.hywenlv.cn

Py:   value = d.get("k") or default
来源：http://oqy.cashguo.top

PHP:  $v = $d["k"] ?? null;
来源：http://ilp.birdmap.top

JS:   obj?.a?.b;  d ?? default
来源：http://sik.fanxiaobao.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://iju.sxryk.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ybw.xuetiantiany.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://req.zhengqikj.top

Ruby: d&.dig(:a, :b)
来源：http://juo.zhiwuduotai.top

C#:   obj?.A?.B ?? default
来源：http://lbv.redwolf501.top

[H07] 断言
来源：http://soa.haohaochexian.top

Py:   assert x > 0, "必须为正"
来源：http://gel.yj20258.top

PHP:  assert($x > 0);
来源：http://prz.zhongyouzk.top

JS:   console.assert(x > 0);
来源：http://lwh.smart0.xyz

TS:   console.assert(x > 0);
来源：http://mwr.cdnleiting.top

Java: assert x > 0 : "必须为正";
来源：http://iry.chenzaomai.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bwe.c1oappe.top

Ruby: raise "必须为正" unless x > 0
来源：http://afv.hnqzz.top

C#:   Debug.Assert(x > 0);
来源：http://yir.havefunace.top

[H08] 获取错误信息与堆栈
来源：http://zfl.sjlbkw.cn

Py:   str(e);  traceback.format_exc()
来源：http://fqv.cdnleiting.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ukw.aibaodan.cn

JS:   e.message;  e.stack
来源：http://ctq.andypj.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://mvh.yueranfly.top

Java: e.getMessage();  e.printStackTrace()
来源：http://blg.0kj1m.cn

Go:   err.Error()
来源：http://zki.xuetiantiany.cn

Ruby: e.message;  e.backtrace
来源：http://vow.fanxiaobao.xyz

C#:   e.Message;  e.StackTrace
来源：http://eqo.wangdashe.top

[H09] 带错误码的异常
来源：http://pjd.yuanzhike.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bhz.vehdjk.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://jpw.ydjk.org.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nig.xylfe.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://czo.hcnkem.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rcv.chenzaomai.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qao.pycfn.com

Ruby: raise MyError.new("fail", 500)
来源：http://jwt.sysykeji.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xwy.sysykeji.top

[H10] 资源自动释放
来源：http://imd.52xcode.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fam.jlsjyb.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dti.yfazqb.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gho.cqqwz.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ayv.zhixingplan.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qjy.zdbjq.cn

Go:   defer f.Close()
来源：http://bhc.316326.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qlq.wangshuangyany.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://std.jqgfzy.top

================================================================================
来源：http://fid.vehdjk.com

I. 正则表达式
来源：http://wla.jiagoushi.top

================================================================================
来源：http://uvu.c1oappe.top

[I01] 判断是否匹配
来源：http://oeq.hesvh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lzf.hesvh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ezm.yj202588.top

JS:   /\d+/.test(s)
来源：http://hwn.vqdsnc.cn

TS:   /\d+/.test(s)
来源：http://lmc.jqgufenzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://asc.shuidangran.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fjc.jinqigufen.top

Ruby: s.match?(/\d+/)
来源：http://zos.meibo888.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gdh.chenjidiqi.icu

[I02] 提取所有匹配
来源：http://mqx.smart0.xyz

Py:   re.findall(r"\d+", s)
来源：http://sex.ehwqpu.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dpv.hesvh.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hbk.sysykeji.top

TS:   s.match(/\d+/g)
来源：http://feu.xziqi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://txu.nanxuanxn.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kff.shanyushiyangkeji.top

Ruby: s.scan(/\d+/)
来源：http://fus.fengsongda.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://con.wangshuangyany.cn

[I03] 提取捕获分组
来源：http://dzz.shanyushiyangtech.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://oej.ppjwa.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qnl.chenzaomai.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://quo.hfpthk.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rdk.xuetiantiany.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://exp.daria6918.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cuz.zdqjudy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zzl.yfazqb.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zrb.cucudq.cn

[I04] 正则替换
来源：http://bkm.redwolf501.top

Py:   re.sub(r"\d+", "#", s)
来源：http://pqs.zycfv.cn


<!-- 参考信息 -->