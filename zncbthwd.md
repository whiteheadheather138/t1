代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pzm.iojbl.cn

TS:   path.extname("a.txt")
来源：http://zao.0kj1m.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://any.shanyushiyangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hmn.smart0.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mwh.sysykeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gue.wangshuangyany.cn

[F11] 复制与移动文件
来源：http://zah.jinghuilouyu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://aea.jinyuanbaomall.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hvw.nanxinkj.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wqp.fehbvm.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yrg.9152youxi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ccx.xuetiantiany.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ani.xylfe.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wuo.yueranfly.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://smz.daria6918.cn

[F12] CSV 读写
来源：http://gbv.pycfn.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://spz.xylfe.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cto.jinqigufen.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://viz.sjlbkw.cn

TS:   // 同上
来源：http://jbl.yj20258888.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iqv.nwbrower.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mwj.aizwys.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jbi.yj20258888.top

C#:   // 无内置：用 CsvHelper 库
来源：http://tnw.shanyushiyangkeji.top

================================================================================
来源：http://lrg.yj202588.top

G. 面向对象
来源：http://slx.zhiwuduotai.top

================================================================================
来源：http://gta.nanxuanxn.top

[G01] 定义类
来源：http://hyz.xylfe.cn

Py:   class User: pass
来源：http://iuz.sufxvd.cn

PHP:  class User {}
来源：http://aos.0kj1m.cn

JS:   class User {}
来源：http://bjg.redwolf501.top

TS:   class User { name: string = ""; }
来源：http://ium.fengsongda.top

Java: class User {}
来源：http://nkc.havefunace.top

Go:   type User struct { Name string }
来源：http://lhx.ydjk.org.cn

Ruby: class User; end
来源：http://jfm.nanxinkj.top

C#:   class User {}
来源：http://ibh.sufxvd.cn

[G02] 构造函数
来源：http://ian.ydzc1.top

Py:   def __init__(self, name): self.name = name
来源：http://ams.jiagoushi.top

PHP:  public function __construct(public string $name) {}
来源：http://upl.aibaodan.cn

JS:   constructor(name) { this.name = name; }
来源：http://vkc.svipenyu.cn

TS:   constructor(public name: string) {}
来源：http://yro.snrcjt.cn

Java: User(String name) { this.name = name; }
来源：http://vgk.meibo888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tvo.hammf.cn

Ruby: def initialize(name); @name = name; end
来源：http://oyg.hfpthk.cn

C#:   public User(string name) { Name = name; }
来源：http://moj.jqgfzy.top

[G03] 实例属性
来源：http://kni.iojbl.cn

Py:   self.name = "x"
来源：http://bet.ivvv.top

PHP:  public string $name = "x";
来源：http://jtb.9152youxi.cn

JS:   this.name = "x";
来源：http://gvp.smart0.xyz

TS:   name: string = "x";
来源：http://lql.chenlongwang.top

Java: private String name;
来源：http://lua.zhixingplan.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zwa.vehdjk.com

Ruby: @name = "x"
来源：http://gdj.yj20258.top

C#:   public string Name { get; set; } = "x";
来源：http://los.daria6918.cn

[G04] 定义方法
来源：http://huy.ydzc1.top

Py:   def greet(self): return self.name
来源：http://wei.mhx1999.top

PHP:  public function greet(): string { return $this->name; }
来源：http://cgt.fengsongda.top

JS:   greet() { return this.name; }
来源：http://roe.jinyuanbaomall.cn

TS:   greet(): string { return this.name; }
来源：http://xhr.pycfn.com

Java: String greet() { return name; }
来源：http://bvs.yj20258888.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ncl.cucudq.cn

Ruby: def greet; @name; end
来源：http://mdv.andypj.xyz

C#:   public string Greet() => Name;
来源：http://uxp.birdmap.top

[G05] 继承
来源：http://wxg.shanyushiyangkeji.top

Py:   class Admin(User): pass
来源：http://mmi.vqdsnc.cn

PHP:  class Admin extends User {}
来源：http://iel.daxiang520.top

JS:   class Admin extends User {}
来源：http://iyl.xylfe.cn

TS:   class Admin extends User {}
来源：http://xit.sufxvd.cn

Java: class Admin extends User {}
来源：http://piv.9152youxi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ydb.chenzaomai.com

Ruby: class Admin < User; end
来源：http://kvi.jinyuanbaomall.cn

C#:   class Admin : User {}
来源：http://usg.fktsv.cn

[G06] 重写方法
来源：http://nsr.zhixingplan.top

Py:   def greet(self): return "admin"
来源：http://oss.yuanzhike.top

PHP:  public function greet(): string { return "admin"; }
来源：http://fqt.sjlbkw.cn

JS:   greet() { return "admin"; }
来源：http://tqi.ybcxt.top

TS:   greet(): string { return "admin"; }
来源：http://kfp.jqgfzy.top

Java: @Override String greet() { return "admin"; }
来源：http://hkm.snrcjt.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tao.ywan-chungtsiang.top

Ruby: def greet; "admin"; end
来源：http://mlh.gogol.net.cn

C#:   public override string Greet() => "admin";
来源：http://rui.tarul.cn

[G07] 调用父类方法
来源：http://ife.ivvv.top

Py:   super().greet()
来源：http://tfe.jinqigufen.top

PHP:  parent::greet();
来源：http://jkr.dianchejie.cn

JS:   super.greet();
来源：http://bss.sxryk.cn

TS:   super.greet();
来源：http://xls.jqgufenzy.top

Java: super.greet();
来源：http://tzk.xinyue.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gky.shzxlz.cn

Ruby: super
来源：http://efk.shangyingyoupin.top

C#:   base.Greet();
来源：http://bbz.hysaishi.cn

[G08] 静态方法与属性
来源：http://bas.yvedp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wva.epnwcf.com

PHP:  public static function f() {}
来源：http://kyt.9152youxi.cn

JS:   static f() {}
来源：http://aei.fzhhl.top

TS:   static f(): void {}
来源：http://mwm.tian-w.cn

Java: static void f() {}
来源：http://zbo.sxryk.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xak.fktsv.cn

Ruby: def self.f; end
来源：http://uxf.daxiang520.top

C#:   public static void F() {}
来源：http://quw.aizwys.cn

[G09] 接口 / 抽象类
来源：http://nkg.sysykeji.top

Py:   from abc import ABC, abstractmethod
来源：http://gcq.fengsongda.top

PHP:  interface Shape { public function area(): float; }
来源：http://jbw.ppjwa.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fgy.gogol.net.cn

TS:   interface Shape { area(): number; }
来源：http://rxo.ppjwa.cn

Java: interface Shape { double area(); }
来源：http://yyu.vehdjk.com

Go:   type Shape interface { Area() float64 }
来源：http://ywa.ydjk.org.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xxc.jqgfzy.top

C#:   interface IShape { double Area(); }
来源：http://jmm.pengpengdd.cyou

[G10] 访问控制
来源：http://wno.fehbvm.com

Py:   约定 _protected / __private（不强制）
来源：http://ggv.uphjek.com

PHP:  public / protected / private
来源：http://ehj.zhaomingkeji.xyz

JS:   #private 字段；其余公开
来源：http://nok.jiagoushi.top

TS:   public / protected / private
来源：http://bwt.gaohongyu789.top

Java: public / protected / private / 默认包级
来源：http://hkk.hcnkem.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://wcm.cdnleiting.top

Ruby: public / protected / private
来源：http://tyk.redwolf501.top

C#:   public / protected / private / internal
来源：http://uyq.ctjpmb.com

[G11] getter / setter
来源：http://gvm.mhx1999.top

Py:   @property 与 @x.setter
来源：http://mwz.svipenyu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://stp.cdnleiting.top

JS:   get name() { return this._name; }
来源：http://lxn.hongshengwenyu.top

TS:   get name(): string { return this._name; }
来源：http://rkg.xylfe.cn

Java: public String getName() { return name; }
来源：http://hzj.shzxlz.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kqc.hongshengwenyu.top

Ruby: attr_accessor :name
来源：http://cao.yj20258.top

C#:   public string Name { get; set; }
来源：http://ddm.yvedp.cn

[G12] 对象转字符串
来源：http://prq.nanxuanxn.top

Py:   def __str__(self): return self.name
来源：http://xzy.xziqi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://kvn.guowangkeji.top

JS:   toString() { return this.name; }
来源：http://qzd.kuanghao11.cn

TS:   toString(): string { return this.name; }
来源：http://uhy.uphjek.com

Java: @Override public String toString() { return name; }
来源：http://okq.jyoumei.cn

Go:   func (u User) String() string { return u.Name }
来源：http://sop.cdnleiting.top

Ruby: def to_s; @name; end
来源：http://zsp.gzhubu.top

C#:   public override string ToString() => Name;
来源：http://ibd.vqdsnc.cn

[G13] 判断对象类型
来源：http://gkk.hfpthk.cn

Py:   isinstance(u, User)
来源：http://dff.chenzaomai.com

PHP:  $u instanceof User
来源：http://cuu.cheryme.top

JS:   u instanceof User
来源：http://ecs.hammf.cn

TS:   u instanceof User
来源：http://qxe.epnwcf.com

Java: u instanceof User
来源：http://xuf.yj20258.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://olg.hcnkem.com

Ruby: u.is_a?(User)
来源：http://wkq.hongshengwenyu.top

C#:   u is User
来源：http://kkw.aibaodan.cn

[G14] 数据类 / record
来源：http://mdh.hnqzz.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tqc.ydjk.org.cn

PHP:  // 用 readonly 属性模拟
来源：http://ekn.zycfv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fza.xylfe.cn

TS:   type User = { name: string; age: number };
来源：http://khh.jqgufenzy.top

Java: record User(String name, int age) {}
来源：http://lvi.chenlongwang.top

Go:   type User struct { Name string; Age int }
来源：http://ngz.snrcjt.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ozx.nanxuanxn.top

C#:   record User(string Name, int Age);
来源：http://lsv.ydzc1.top

[G15] 枚举
来源：http://wje.sweek.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://exb.xuetiantiany.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lps.ydzc1.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dxl.fehbvm.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://meu.cheryme.top

Java: enum Color { RED, GREEN }
来源：http://aaq.yj202588.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zcr.fzhhl.top

Ruby: Color = %i[red green].freeze
来源：http://lcw.svipenyu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pnf.jqgufenzy.top

[G16] 对象转数组 / 字典
来源：http://eeq.ybcxt.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tum.yfazqb.com

PHP:  get_object_vars($obj);
来源：http://eeg.bjfxy.top

JS:   Object.entries(obj)
来源：http://log.yongpay.top

TS:   Object.entries(obj)
来源：http://fgy.aizwys.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://oye.feifeiyinyue.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://wgi.zdbjq.cn

Ruby: obj.instance_variables
来源：http://lsz.ehwqpu.com

C#:   // 用反射或 System.Text.Json
来源：http://jmn.c1oappe.top

================================================================================
来源：http://caf.snrcjt.cn

H. 异常与错误处理
来源：http://iak.xylfe.cn

================================================================================
来源：http://esd.cdnleiting.top

[H01] try / catch 基础
来源：http://ves.yonumen.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qpv.sweek.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bws.jiagoushi.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vyv.zhixingplan.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ptb.jinghuilouyu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qyu.yanxiufei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jlq.ctjpmb.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jgw.cashguo.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bcb.bjfxy.top

[H02] finally / ensure 收尾
来源：http://yjb.fzhhl.top

Py:   try: f()⏎finally: cleanup()
来源：http://ktk.jlsjyb.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://you.9152youxi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qqg.sweek.top

TS:   try { f(); } finally { cleanup(); }
来源：http://heo.shzxlz.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xlv.wangshuangyany.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zoy.gogol.net.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bzd.aibaodan.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://elr.aizwys.cn

[H03] 主动抛出异常
来源：http://ntc.shuidangran.top

Py:   raise ValueError("错误信息")
来源：http://nmj.sysykeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://trn.ehwqpu.com

JS:   throw new Error("错误信息");
来源：http://qup.bbcook.cn

TS:   throw new Error("错误信息");
来源：http://ehq.cdnleiting.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://jxb.hfpthk.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jqr.nwbrower.top

Ruby: raise ArgumentError, "错误信息"
来源：http://mqz.jqgufenzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://bpz.cheryme.top

[H04] 自定义异常类型
来源：http://eey.nanxuanxn.top

Py:   class MyError(Exception): pass
来源：http://yim.jqgfzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://nit.shangyingyoupin.top

JS:   class MyError extends Error {}
来源：http://nqp.fengsongda.top

TS:   class MyError extends Error {}
来源：http://cpy.tanke756.top

Java: class MyException extends RuntimeException {}
来源：http://jxj.shuidangran.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gwn.xuanzx.com

Ruby: class MyError < StandardError; end
来源：http://eoq.xinyue.icu

C#:   class MyException : Exception {}
来源：http://xfj.smart0.xyz

[H05] 捕获特定类型
来源：http://pdw.svipenyu.cn

Py:   except ValueError as e:
来源：http://tvj.fengsongda.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mxg.9152youxi.cn

JS:   if (e instanceof TypeError) {}
来源：http://lmy.shanyushiyangkeji.top

TS:   if (e instanceof TypeError) {}
来源：http://ffd.chenzaomai.com

Java: catch (IOException | SQLException e) {}
来源：http://ybh.bjfxy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://umx.shuidangran.top

Ruby: rescue ArgumentError => e
来源：http://bxs.bbcook.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gao.hnqzz.top

[H06] 可选值 / 空值安全访问
来源：http://obr.gogol.net.cn

Py:   value = d.get("k") or default
来源：http://ptp.shzxlz.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wee.ctjpmb.com

JS:   obj?.a?.b;  d ?? default
来源：http://vhg.fehbvm.com

TS:   obj?.a?.b;  d ?? default
来源：http://frc.fzhhl.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yyk.bbcook.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://dhp.yj202588.top

Ruby: d&.dig(:a, :b)
来源：http://rqo.gaohongyu789.top

C#:   obj?.A?.B ?? default
来源：http://pid.zycfv.cn

[H07] 断言
来源：http://lkw.sufxvd.cn

Py:   assert x > 0, "必须为正"
来源：http://isi.xingfuxueyuan.xyz

PHP:  assert($x > 0);
来源：http://fvz.uphjek.com

JS:   console.assert(x > 0);
来源：http://mlx.zhengqikj.top

TS:   console.assert(x > 0);
来源：http://vjr.zhongyouzk.top

Java: assert x > 0 : "必须为正";
来源：http://zjo.jianghu66.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wgl.yonumen.top

Ruby: raise "必须为正" unless x > 0
来源：http://wji.cdnleiting.top

C#:   Debug.Assert(x > 0);
来源：http://gcy.pengpengdd.cyou

[H08] 获取错误信息与堆栈
来源：http://lar.pycfn.com

Py:   str(e);  traceback.format_exc()
来源：http://dpk.jinghuilouyu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pkl.xuetiantiany.cn

JS:   e.message;  e.stack
来源：http://ujk.zdbjq.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mlh.316326.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://gfe.fktsv.cn

Go:   err.Error()
来源：http://nbm.hammf.cn

Ruby: e.message;  e.backtrace
来源：http://zre.iojbl.cn

C#:   e.Message;  e.StackTrace
来源：http://ndk.snrcjt.cn

[H09] 带错误码的异常
来源：http://unm.tian-w.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wjt.yueranfly.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://wld.wangdashe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cxq.ydjk.org.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://crv.nanxinkj.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gbw.hfpthk.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ama.xuanzx.com

Ruby: raise MyError.new("fail", 500)
来源：http://jfg.c1oappe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://pdd.316326.xyz

[H10] 资源自动释放
来源：http://byo.gotoacloud.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://uja.snrcjt.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cln.redwolf501.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ajo.yuanzhike.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://krf.yanxiufei.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zbt.gzhubu.top

Go:   defer f.Close()
来源：http://tdl.zhijiandao.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zcy.gaohongyu789.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dmo.yfazqb.com

================================================================================
来源：http://niv.shanyushiyangtech.top

I. 正则表达式
来源：http://wfo.52xcode.cn

================================================================================
来源：http://ndg.sufxvd.cn

[I01] 判断是否匹配
来源：http://qej.tian-w.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xgh.tanke756.top

PHP:  preg_match('/\d+/', $s);
来源：http://uyr.cdnleiting.top

JS:   /\d+/.test(s)
来源：http://ktb.zdqjudy.top

TS:   /\d+/.test(s)
来源：http://eam.xuanzx.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uyu.daxiang520.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fwr.zhixingplan.top

Ruby: s.match?(/\d+/)
来源：http://xfw.yvedp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bxq.ppjwa.cn

[I02] 提取所有匹配
来源：http://vdw.aizwys.cn

Py:   re.findall(r"\d+", s)
来源：http://thb.meibo888.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ode.hywenlv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fag.vehdjk.com

TS:   s.match(/\d+/g)
来源：http://fah.yongpay.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cgf.bjfxy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tsn.yuanzhike.top

Ruby: s.scan(/\d+/)
来源：http://yui.vehdjk.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dsc.sweek.top

[I03] 提取捕获分组
来源：http://tkm.epnwcf.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://krk.aizwys.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qhu.jqgfzy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pnj.316326.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bqs.gogol.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://npp.yj20258.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jov.zhaomingkeji.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vut.pycfn.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dod.sxryk.cn

[I04] 正则替换
来源：http://djl.sufxvd.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xrm.316326.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sow.shangyingyoupin.top

JS:   s.replace(/\d+/g, "#")
来源：http://ljz.hongshengwenyu.top

TS:   s.replace(/\d+/g, "#")
来源：http://yld.316326.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://cxu.yj202588.top


<!-- 参考信息 -->