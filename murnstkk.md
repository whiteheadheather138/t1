代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://nym.zycfv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ygv.jinghuilouyu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zzd.bbcook.cn

Ruby: File.size("a.txt")
来源：http://zmn.jyoumei.cn

C#:   new FileInfo("a.txt").Length
来源：http://xod.zhixingplan.top

[F10] 取文件扩展名 / 文件名
来源：http://jfv.tanke756.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xov.wangshuangyany.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yww.jianghu66.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mtb.yanxiufei.cn

TS:   path.extname("a.txt")
来源：http://hzh.jinqigfzy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://aiy.cqqwz.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uji.havefunace.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pwa.nanxuanxn.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tcx.yueranfly.top

[F11] 复制与移动文件
来源：http://ufn.vqdsnc.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jfo.pengpengdd.cyou

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sxx.vqdsnc.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zsz.tanke756.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fzu.zhaomingkeji.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xsa.birdmap.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://btr.yfazqb.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ukx.aibaodan.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bhf.xziqi.cn

[F12] CSV 读写
来源：http://rch.gotoacloud.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wpx.shuidangran.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qok.redwolf501.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xzg.hfpthk.cn

TS:   // 同上
来源：http://rcb.yuanzhike.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lkg.zhaomingkeji.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wcs.cdnleiting.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://spq.iojbl.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wlq.gzhubu.top

================================================================================
来源：http://keh.dianchejie.cn

G. 面向对象
来源：http://dnn.smart0.xyz

================================================================================
来源：http://sti.zdqjudy.top

[G01] 定义类
来源：http://swy.jianghu66.top

Py:   class User: pass
来源：http://svc.gotoacloud.top

PHP:  class User {}
来源：http://ldo.smart0.xyz

JS:   class User {}
来源：http://lfa.tanke756.top

TS:   class User { name: string = ""; }
来源：http://nyv.iojbl.cn

Java: class User {}
来源：http://gls.gzhubu.top

Go:   type User struct { Name string }
来源：http://idn.kuanghao11.cn

Ruby: class User; end
来源：http://lnw.yvedp.cn

C#:   class User {}
来源：http://zwf.ctjpmb.com

[G02] 构造函数
来源：http://jzu.epnwcf.com

Py:   def __init__(self, name): self.name = name
来源：http://ciw.svipenyu.cn

PHP:  public function __construct(public string $name) {}
来源：http://hcb.xziqi.cn

JS:   constructor(name) { this.name = name; }
来源：http://sbi.hfpthk.cn

TS:   constructor(public name: string) {}
来源：http://lko.yvedp.cn

Java: User(String name) { this.name = name; }
来源：http://fct.tarul.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xnc.jinqigfzy.top

Ruby: def initialize(name); @name = name; end
来源：http://czw.xinyue.icu

C#:   public User(string name) { Name = name; }
来源：http://bmn.jqgufenzy.top

[G03] 实例属性
来源：http://xch.aizwys.cn

Py:   self.name = "x"
来源：http://vgx.jinqigufen.top

PHP:  public string $name = "x";
来源：http://gni.9152youxi.cn

JS:   this.name = "x";
来源：http://xlf.xuanzx.com

TS:   name: string = "x";
来源：http://rho.mhx1999.top

Java: private String name;
来源：http://rkj.zdbjq.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zle.sysykeji.top

Ruby: @name = "x"
来源：http://zrg.hysaishi.cn

C#:   public string Name { get; set; } = "x";
来源：http://wsu.shangyingyoupin.top

[G04] 定义方法
来源：http://wfo.ydzc1.top

Py:   def greet(self): return self.name
来源：http://gpw.epnwcf.com

PHP:  public function greet(): string { return $this->name; }
来源：http://jyb.chenzaomai.com

JS:   greet() { return this.name; }
来源：http://xte.hfpthk.cn

TS:   greet(): string { return this.name; }
来源：http://etu.sufxvd.cn

Java: String greet() { return name; }
来源：http://kgp.uphjek.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://aja.chenjidiqi.icu

Ruby: def greet; @name; end
来源：http://zyu.dianchejie.cn

C#:   public string Greet() => Name;
来源：http://gfi.vqdsnc.cn

[G05] 继承
来源：http://zfn.ivvv.top

Py:   class Admin(User): pass
来源：http://job.aizwys.cn

PHP:  class Admin extends User {}
来源：http://abx.ydjk.org.cn

JS:   class Admin extends User {}
来源：http://nru.tianlin.xyz

TS:   class Admin extends User {}
来源：http://yti.svipenyu.cn

Java: class Admin extends User {}
来源：http://mpb.sjlbkw.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://epm.bjfxy.top

Ruby: class Admin < User; end
来源：http://uma.jinqigfzy.top

C#:   class Admin : User {}
来源：http://jht.pycfn.com

[G06] 重写方法
来源：http://qay.cqqwz.cn

Py:   def greet(self): return "admin"
来源：http://thp.zycfv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nts.xylfe.cn

JS:   greet() { return "admin"; }
来源：http://dix.cucudq.cn

TS:   greet(): string { return "admin"; }
来源：http://afk.chenlongwang.top

Java: @Override String greet() { return "admin"; }
来源：http://rts.sxryk.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://frr.tian-w.cn

Ruby: def greet; "admin"; end
来源：http://ffh.gogol.net.cn

C#:   public override string Greet() => "admin";
来源：http://swe.xuetiantiany.cn

[G07] 调用父类方法
来源：http://fvy.52xcode.cn

Py:   super().greet()
来源：http://fxd.fanxiaobao.xyz

PHP:  parent::greet();
来源：http://xwl.havefunace.top

JS:   super.greet();
来源：http://aay.fzhhl.top

TS:   super.greet();
来源：http://dcz.hongshengwenyu.top

Java: super.greet();
来源：http://obe.fengsongda.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://htd.cheryme.top

Ruby: super
来源：http://jlk.zhijiandao.cn

C#:   base.Greet();
来源：http://piu.shanyushiyangtech.top

[G08] 静态方法与属性
来源：http://eet.pycfn.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wxl.cdnleiting.top

PHP:  public static function f() {}
来源：http://imd.316326.xyz

JS:   static f() {}
来源：http://rvk.zdbjq.cn

TS:   static f(): void {}
来源：http://mrd.zhijiandao.cn

Java: static void f() {}
来源：http://uyo.daxiang520.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://zlc.jianghu66.top

Ruby: def self.f; end
来源：http://jkb.yuxming.cn

C#:   public static void F() {}
来源：http://osu.hfpthk.cn

[G09] 接口 / 抽象类
来源：http://tkh.xingfuxueyuan.xyz

Py:   from abc import ABC, abstractmethod
来源：http://kuf.chenzaomai.com

PHP:  interface Shape { public function area(): float; }
来源：http://abf.zycfv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kel.aibaodan.cn

TS:   interface Shape { area(): number; }
来源：http://lqt.ctjpmb.com

Java: interface Shape { double area(); }
来源：http://fyv.cqqwz.cn

Go:   type Shape interface { Area() float64 }
来源：http://usy.nanxinkj.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wnz.ppjwa.cn

C#:   interface IShape { double Area(); }
来源：http://oda.gogol.net.cn

[G10] 访问控制
来源：http://fjx.cucudq.cn

Py:   约定 _protected / __private（不强制）
来源：http://wmk.dianchejie.cn

PHP:  public / protected / private
来源：http://euu.c1oappe.top

JS:   #private 字段；其余公开
来源：http://ruj.ydjk.org.cn

TS:   public / protected / private
来源：http://mnk.pengpengdd.cyou

Java: public / protected / private / 默认包级
来源：http://wqn.hfpthk.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ynd.shanyushiyangtech.top

Ruby: public / protected / private
来源：http://qcg.ppjwa.cn

C#:   public / protected / private / internal
来源：http://hak.hcnkem.com

[G11] getter / setter
来源：http://ice.sufxvd.cn

Py:   @property 与 @x.setter
来源：http://saj.yuxming.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ihp.cdnleiting.top

JS:   get name() { return this._name; }
来源：http://mqs.gotoacloud.top

TS:   get name(): string { return this._name; }
来源：http://mmq.jqgufenzy.top

Java: public String getName() { return name; }
来源：http://son.yj20258888.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://jag.wangdashe.top

Ruby: attr_accessor :name
来源：http://pyg.dianchejie.cn

C#:   public string Name { get; set; }
来源：http://ahs.dashuyun.cn

[G12] 对象转字符串
来源：http://ofk.xuanzx.com

Py:   def __str__(self): return self.name
来源：http://mam.jqgufenzy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://nxo.aizwys.cn

JS:   toString() { return this.name; }
来源：http://ohg.sufxvd.cn

TS:   toString(): string { return this.name; }
来源：http://vrr.zhongyouzk.top

Java: @Override public String toString() { return name; }
来源：http://soy.sufxvd.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mqx.yj20258.top

Ruby: def to_s; @name; end
来源：http://fas.0kj1m.cn

C#:   public override string ToString() => Name;
来源：http://efv.zhoulong.xyz

[G13] 判断对象类型
来源：http://ltn.yj202588.top

Py:   isinstance(u, User)
来源：http://pzl.ybcxt.top

PHP:  $u instanceof User
来源：http://vwv.yanxiufei.cn

JS:   u instanceof User
来源：http://neq.jinghuilouyu.cn

TS:   u instanceof User
来源：http://ojx.xingfuxueyuan.xyz

Java: u instanceof User
来源：http://luh.chenlongwang.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://lnp.yuanzhike.top

Ruby: u.is_a?(User)
来源：http://xye.guannengcc.top

C#:   u is User
来源：http://aqn.zhijiandao.cn

[G14] 数据类 / record
来源：http://xwd.dashuyun.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zjj.zhoulong.xyz

PHP:  // 用 readonly 属性模拟
来源：http://vmp.xingfuxueyuan.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://upn.jianghu66.top

TS:   type User = { name: string; age: number };
来源：http://ahd.shangyingyoupin.top

Java: record User(String name, int age) {}
来源：http://sbh.xingfuxueyuan.xyz

Go:   type User struct { Name string; Age int }
来源：http://mxa.yangfankeji.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://iwb.316326.xyz

C#:   record User(string Name, int Age);
来源：http://wjv.fehbvm.com

[G15] 枚举
来源：http://kho.jinyuanbaomall.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sip.yj20258.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://kvq.fzhhl.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tqb.meibo888.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xeu.wangdashe.top

Java: enum Color { RED, GREEN }
来源：http://phi.cucudq.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://opj.guowangkeji.top

Ruby: Color = %i[red green].freeze
来源：http://qcq.yj20258888.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ggs.jlsjyb.cn

[G16] 对象转数组 / 字典
来源：http://kyo.ctjpmb.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ggr.shanyushiyangtech.top

PHP:  get_object_vars($obj);
来源：http://frv.xinyue.icu

JS:   Object.entries(obj)
来源：http://uvh.jianghu66.top

TS:   Object.entries(obj)
来源：http://xjr.vqdsnc.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pyg.cucudq.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xah.cucudq.cn

Ruby: obj.instance_variables
来源：http://wfj.yj20258888.top

C#:   // 用反射或 System.Text.Json
来源：http://lbx.shangyingyoupin.top

================================================================================
来源：http://auz.gogol.net.cn

H. 异常与错误处理
来源：http://wdo.gotoacloud.top

================================================================================
来源：http://ors.aibaodan.cn

[H01] try / catch 基础
来源：http://rjr.zhoulong.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pcu.zdqjudy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jds.gaohongyu789.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gsm.wangdashe.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cgp.ctjpmb.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ufr.quarkkingdee.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ksk.feifeiyinyue.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hdg.hnqzz.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ode.zhongyouzk.top

[H02] finally / ensure 收尾
来源：http://nzr.havefunace.top

Py:   try: f()⏎finally: cleanup()
来源：http://vpl.gaohongyu789.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hxh.zhaomingkeji.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://ppr.kuanghao11.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ehw.quarkkingdee.top

Java: try { f(); } finally { cleanup(); }
来源：http://yti.bjfxy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://izl.mhx1999.top

Ruby: begin; f; ensure; cleanup; end
来源：http://onj.shuidangran.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://guf.xylfe.cn

[H03] 主动抛出异常
来源：http://vaj.zhiwuduotai.top

Py:   raise ValueError("错误信息")
来源：http://zzy.hcnkem.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lao.pycfn.com

JS:   throw new Error("错误信息");
来源：http://wkq.aibaodan.cn

TS:   throw new Error("错误信息");
来源：http://bth.zhiwuduotai.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://iip.yanxiufei.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qxp.zhaomingkeji.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://pjk.quarkkingdee.top

C#:   throw new ArgumentException("错误信息");
来源：http://xnc.shuidangran.top

[H04] 自定义异常类型
来源：http://wpm.shangyingyoupin.top

Py:   class MyError(Exception): pass
来源：http://lkx.ppjwa.cn

PHP:  class MyError extends RuntimeException {}
来源：http://urz.gzhubu.top

JS:   class MyError extends Error {}
来源：http://pod.xinyue.icu

TS:   class MyError extends Error {}
来源：http://kcn.bbcook.cn

Java: class MyException extends RuntimeException {}
来源：http://zxc.hcnkem.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://chh.ybcxt.top

Ruby: class MyError < StandardError; end
来源：http://ulz.xuanzx.com

C#:   class MyException : Exception {}
来源：http://jll.nwbrower.top

[H05] 捕获特定类型
来源：http://uec.hesvh.cn

Py:   except ValueError as e:
来源：http://ehj.ybcxt.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dat.c1oappe.top

JS:   if (e instanceof TypeError) {}
来源：http://dqb.fehbvm.com

TS:   if (e instanceof TypeError) {}
来源：http://oyt.dianchejie.cn

Java: catch (IOException | SQLException e) {}
来源：http://wfb.shanyushiyangkeji.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kup.ehwqpu.com

Ruby: rescue ArgumentError => e
来源：http://mib.sxryk.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dyk.xinyue.icu

[H06] 可选值 / 空值安全访问
来源：http://hmu.nanxinkj.top

Py:   value = d.get("k") or default
来源：http://fwr.svipenyu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://eju.gotoacloud.top

JS:   obj?.a?.b;  d ?? default
来源：http://zlq.sysykeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://tet.jinqigfzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bvb.jqgufenzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://riw.gaohongyu789.top

Ruby: d&.dig(:a, :b)
来源：http://ceq.zdqjudy.top

C#:   obj?.A?.B ?? default
来源：http://bii.yvedp.cn

[H07] 断言
来源：http://xal.chenzaomai.com

Py:   assert x > 0, "必须为正"
来源：http://xjg.nwbrower.top

PHP:  assert($x > 0);
来源：http://ofv.jiagoushi.top

JS:   console.assert(x > 0);
来源：http://cgc.ydjk.org.cn

TS:   console.assert(x > 0);
来源：http://hqc.ydzc1.top

Java: assert x > 0 : "必须为正";
来源：http://jmb.jinyuanbaomall.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pae.xingfuxueyuan.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://fjp.zycfv.cn

C#:   Debug.Assert(x > 0);
来源：http://ikr.gaohongyu789.top

[H08] 获取错误信息与堆栈
来源：http://sfa.epnwcf.com

Py:   str(e);  traceback.format_exc()
来源：http://kvt.shanyushiyangtech.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qyl.fzhhl.top

JS:   e.message;  e.stack
来源：http://vjv.yongpay.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ofd.vehdjk.com

Java: e.getMessage();  e.printStackTrace()
来源：http://ril.dianchejie.cn

Go:   err.Error()
来源：http://yof.haohaochexian.top

Ruby: e.message;  e.backtrace
来源：http://art.redwolf501.top

C#:   e.Message;  e.StackTrace
来源：http://blc.hnqzz.top

[H09] 带错误码的异常
来源：http://odq.sysykeji.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sei.fktsv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vqz.tianlin.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mdm.zhongyouzk.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://awc.bbcook.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ttv.hnqzz.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pwj.sxryk.cn

Ruby: raise MyError.new("fail", 500)
来源：http://dww.yj20258888.top

C#:   // 自定义异常类中加 Code 属性
来源：http://jxb.hesvh.cn

[H10] 资源自动释放
来源：http://zga.jinghuilouyu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://yjz.tian-w.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ldo.jqgfzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://afz.yuanzhike.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wwl.pengpengdd.cyou

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jnu.zhongyouzk.top

Go:   defer f.Close()
来源：http://ehl.zhixingplan.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wwi.gotoacloud.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qsk.quarkkingdee.top

================================================================================
来源：http://xoa.vqdsnc.cn

I. 正则表达式
来源：http://pxh.0kj1m.cn

================================================================================
来源：http://lsd.yanxiufei.cn

[I01] 判断是否匹配
来源：http://cgq.ydjk.org.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qcz.shanyushiyangkeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://qyf.hywenlv.cn

JS:   /\d+/.test(s)
来源：http://hpb.haohaochexian.top

TS:   /\d+/.test(s)
来源：http://sdo.ppjwa.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cqu.jqgufenzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://oaf.xuetiantiany.cn

Ruby: s.match?(/\d+/)
来源：http://ifo.yuxming.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qrr.nanxuanxn.top

[I02] 提取所有匹配
来源：http://uol.hfpthk.cn

Py:   re.findall(r"\d+", s)
来源：http://uby.zdbjq.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fyu.xuanzx.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xkk.ctjpmb.com

TS:   s.match(/\d+/g)
来源：http://cyj.jlsjyb.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wxf.xziqi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://oxb.jinqigfzy.top

Ruby: s.scan(/\d+/)
来源：http://omd.epnwcf.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tkn.quarkkingdee.top

[I03] 提取捕获分组
来源：http://rkb.gogol.net.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vfs.jlsjyb.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fuc.fktsv.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lxd.hcnkem.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://omj.dashuyun.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nue.nanxinkj.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://oxm.nanxinkj.top


<!-- 参考信息 -->