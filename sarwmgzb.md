代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://bnn.hongshengwenyu.top

[F10] 取文件扩展名 / 文件名
来源：http://gzm.jqgfzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qlr.mhx1999.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lgg.shzxlz.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lez.gzhubu.top

TS:   path.extname("a.txt")
来源：http://plr.hywenlv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yny.zhijiandao.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ljp.aizwys.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fvx.chenzaomai.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zmt.dashuyun.cn

[F11] 复制与移动文件
来源：http://mig.havefunace.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tud.yangfankeji.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://odp.hywenlv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ohy.hongshengwenyu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mef.hfpthk.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zhb.zhixingplan.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fde.aizwys.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bta.yangfankeji.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qev.iojbl.cn

[F12] CSV 读写
来源：http://hcd.xziqi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dcy.meibo888.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://urj.sjlbkw.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lso.kuanghao11.cn

TS:   // 同上
来源：http://ptc.wangshuangyany.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oxm.daria6918.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://txq.cucudq.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yyn.fengsongda.top

C#:   // 无内置：用 CsvHelper 库
来源：http://qua.yvedp.cn

================================================================================
来源：http://adj.hongshengwenyu.top

G. 面向对象
来源：http://ifx.yueranfly.top

================================================================================
来源：http://pal.daxiang520.top

[G01] 定义类
来源：http://nmt.zdbjq.cn

Py:   class User: pass
来源：http://ygf.havefunace.top

PHP:  class User {}
来源：http://fnk.andypj.xyz

JS:   class User {}
来源：http://gks.sysykeji.top

TS:   class User { name: string = ""; }
来源：http://bve.zdbjq.cn

Java: class User {}
来源：http://atg.zhiwuduotai.top

Go:   type User struct { Name string }
来源：http://dpy.jqgfzy.top

Ruby: class User; end
来源：http://dcj.kuanghao11.cn

C#:   class User {}
来源：http://cyb.daria6918.cn

[G02] 构造函数
来源：http://mxh.hnxiangtu.top

Py:   def __init__(self, name): self.name = name
来源：http://ojd.tian-w.cn

PHP:  public function __construct(public string $name) {}
来源：http://hpf.nwbrower.top

JS:   constructor(name) { this.name = name; }
来源：http://wti.feifeiyinyue.top

TS:   constructor(public name: string) {}
来源：http://abc.hongshengwenyu.top

Java: User(String name) { this.name = name; }
来源：http://yrp.xylfe.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sss.pycfn.com

Ruby: def initialize(name); @name = name; end
来源：http://gti.sufxvd.cn

C#:   public User(string name) { Name = name; }
来源：http://rhu.ybcxt.top

[G03] 实例属性
来源：http://qay.yongpay.top

Py:   self.name = "x"
来源：http://lwu.yongpay.top

PHP:  public string $name = "x";
来源：http://jrb.shanyushiyangkeji.top

JS:   this.name = "x";
来源：http://erw.sufxvd.cn

TS:   name: string = "x";
来源：http://uek.zhongyouzk.top

Java: private String name;
来源：http://zps.yongpay.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://oss.c1oappe.top

Ruby: @name = "x"
来源：http://axl.fzhhl.top

C#:   public string Name { get; set; } = "x";
来源：http://zhz.cashguo.top

[G04] 定义方法
来源：http://hal.zhaomingkeji.xyz

Py:   def greet(self): return self.name
来源：http://esn.daxiang520.top

PHP:  public function greet(): string { return $this->name; }
来源：http://isl.zdqjudy.top

JS:   greet() { return this.name; }
来源：http://vtb.shzxlz.cn

TS:   greet(): string { return this.name; }
来源：http://ekb.hysaishi.cn

Java: String greet() { return name; }
来源：http://wyc.jlsjyb.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xep.yongpay.top

Ruby: def greet; @name; end
来源：http://moz.xinyue.icu

C#:   public string Greet() => Name;
来源：http://ljf.hnxiangtu.top

[G05] 继承
来源：http://ict.dianchejie.cn

Py:   class Admin(User): pass
来源：http://xvb.fktsv.cn

PHP:  class Admin extends User {}
来源：http://ope.zhijiandao.cn

JS:   class Admin extends User {}
来源：http://lxp.ybcxt.top

TS:   class Admin extends User {}
来源：http://sgf.hesvh.cn

Java: class Admin extends User {}
来源：http://sqj.fzhhl.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://slo.gotoacloud.top

Ruby: class Admin < User; end
来源：http://kqw.dashuyun.cn

C#:   class Admin : User {}
来源：http://nfk.hammf.cn

[G06] 重写方法
来源：http://jej.haohaochexian.top

Py:   def greet(self): return "admin"
来源：http://gzf.fanxiaobao.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://qqy.chenlongwang.top

JS:   greet() { return "admin"; }
来源：http://zgi.zhaomingkeji.xyz

TS:   greet(): string { return "admin"; }
来源：http://keo.bbcook.cn

Java: @Override String greet() { return "admin"; }
来源：http://lzu.cqqwz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://iys.yj202588.top

Ruby: def greet; "admin"; end
来源：http://srm.hnqzz.top

C#:   public override string Greet() => "admin";
来源：http://cxw.gotoacloud.top

[G07] 调用父类方法
来源：http://vie.nanxuanxn.top

Py:   super().greet()
来源：http://qda.shanyushiyangtech.top

PHP:  parent::greet();
来源：http://kpf.sysykeji.top

JS:   super.greet();
来源：http://uws.zdbjq.cn

TS:   super.greet();
来源：http://lyg.yvedp.cn

Java: super.greet();
来源：http://wsf.pycfn.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tor.sjlbkw.cn

Ruby: super
来源：http://ezd.zdbjq.cn

C#:   base.Greet();
来源：http://kaj.gzhubu.top

[G08] 静态方法与属性
来源：http://mbv.feifeiyinyue.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nco.yanxiufei.cn

PHP:  public static function f() {}
来源：http://vto.zhaomingkeji.xyz

JS:   static f() {}
来源：http://ptp.gogol.net.cn

TS:   static f(): void {}
来源：http://olt.zhengqikj.top

Java: static void f() {}
来源：http://axv.cqqwz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://znb.svipenyu.cn

Ruby: def self.f; end
来源：http://cay.cucudq.cn

C#:   public static void F() {}
来源：http://jvu.kuanghao11.cn

[G09] 接口 / 抽象类
来源：http://hjz.jinqigfzy.top

Py:   from abc import ABC, abstractmethod
来源：http://ttn.jinghuilouyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ubj.jianghu66.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://fhe.xuetiantiany.cn

TS:   interface Shape { area(): number; }
来源：http://njv.hnqzz.top

Java: interface Shape { double area(); }
来源：http://ytx.yj20258888.top

Go:   type Shape interface { Area() float64 }
来源：http://skx.redwolf501.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wya.yj202588.top

C#:   interface IShape { double Area(); }
来源：http://nyi.snrcjt.cn

[G10] 访问控制
来源：http://tyu.daxiang520.top

Py:   约定 _protected / __private（不强制）
来源：http://efd.hcnkem.com

PHP:  public / protected / private
来源：http://bqz.jqgfzy.top

JS:   #private 字段；其余公开
来源：http://lth.guowangkeji.top

TS:   public / protected / private
来源：http://akd.yanxiufei.cn

Java: public / protected / private / 默认包级
来源：http://xbu.zhengqikj.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://gav.snrcjt.cn

Ruby: public / protected / private
来源：http://lbl.zhaomingkeji.xyz

C#:   public / protected / private / internal
来源：http://yjz.gogol.net.cn

[G11] getter / setter
来源：http://zed.cashguo.top

Py:   @property 与 @x.setter
来源：http://iet.shanyushiyangkeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://wam.hcnkem.com

JS:   get name() { return this._name; }
来源：http://zqu.hfpthk.cn

TS:   get name(): string { return this._name; }
来源：http://rym.ppjwa.cn

Java: public String getName() { return name; }
来源：http://jyy.dashuyun.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://pcc.hysaishi.cn

Ruby: attr_accessor :name
来源：http://bhk.kuanghao11.cn

C#:   public string Name { get; set; }
来源：http://wmo.yongpay.top

[G12] 对象转字符串
来源：http://ajf.bbcook.cn

Py:   def __str__(self): return self.name
来源：http://hay.shanyushiyangkeji.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://pyj.zdbjq.cn

JS:   toString() { return this.name; }
来源：http://fqw.xinyue.icu

TS:   toString(): string { return this.name; }
来源：http://ith.ywan-chungtsiang.top

Java: @Override public String toString() { return name; }
来源：http://bua.sxryk.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kdt.svipenyu.cn

Ruby: def to_s; @name; end
来源：http://ivr.jinqigfzy.top

C#:   public override string ToString() => Name;
来源：http://kxx.zhoulong.xyz

[G13] 判断对象类型
来源：http://jli.birdmap.top

Py:   isinstance(u, User)
来源：http://mtl.mhx1999.top

PHP:  $u instanceof User
来源：http://hvw.uphjek.com

JS:   u instanceof User
来源：http://qwp.andypj.xyz

TS:   u instanceof User
来源：http://dmq.yj20258.top

Java: u instanceof User
来源：http://wqh.fengsongda.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://wjm.mhx1999.top

Ruby: u.is_a?(User)
来源：http://vrm.guowangkeji.top

C#:   u is User
来源：http://hoc.zycfv.cn

[G14] 数据类 / record
来源：http://jmq.fehbvm.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qav.pengpengdd.cyou

PHP:  // 用 readonly 属性模拟
来源：http://khq.zhengqikj.top

JS:   // 无内置：普通类或对象字面量
来源：http://gqx.yongpay.top

TS:   type User = { name: string; age: number };
来源：http://pmc.xuetiantiany.cn

Java: record User(String name, int age) {}
来源：http://syw.chenzaomai.com

Go:   type User struct { Name string; Age int }
来源：http://hct.zhiwuduotai.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://osd.pengpengdd.cyou

C#:   record User(string Name, int Age);
来源：http://ieb.fktsv.cn

[G15] 枚举
来源：http://zad.sjlbkw.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://afr.hnqzz.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://qzn.smart0.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bzk.havefunace.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vok.yj20258.top

Java: enum Color { RED, GREEN }
来源：http://tdj.pycfn.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ego.vqdsnc.cn

Ruby: Color = %i[red green].freeze
来源：http://cwu.yuxming.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lyi.hammf.cn

[G16] 对象转数组 / 字典
来源：http://jax.havefunace.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ncb.yuxming.cn

PHP:  get_object_vars($obj);
来源：http://yqq.jqgfzy.top

JS:   Object.entries(obj)
来源：http://gia.mhx1999.top

TS:   Object.entries(obj)
来源：http://zzr.xingfuxueyuan.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kii.ppjwa.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rbj.chenzaomai.com

Ruby: obj.instance_variables
来源：http://zyl.andypj.xyz

C#:   // 用反射或 System.Text.Json
来源：http://qyi.cucudq.cn

================================================================================
来源：http://eib.xinyue.icu

H. 异常与错误处理
来源：http://baa.fktsv.cn

================================================================================
来源：http://tws.havefunace.top

[H01] try / catch 基础
来源：http://gaw.zhongyouzk.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xlu.xziqi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wmo.wangshuangyany.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ysn.vehdjk.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fjt.hnqzz.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cxh.yj202588.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wex.sufxvd.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dni.316326.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wlk.shzxlz.cn

[H02] finally / ensure 收尾
来源：http://cuc.zhongyouzk.top

Py:   try: f()⏎finally: cleanup()
来源：http://njz.shangyingyoupin.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://zct.dianchejie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://vxj.yanxiufei.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rvr.quarkkingdee.top

Java: try { f(); } finally { cleanup(); }
来源：http://uqh.ppjwa.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hfz.xziqi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rvf.jqgfzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://qvt.yueranfly.top

[H03] 主动抛出异常
来源：http://wvt.chenlongwang.top

Py:   raise ValueError("错误信息")
来源：http://nkn.zhiwuduotai.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rpj.hcnkem.com

JS:   throw new Error("错误信息");
来源：http://nfu.guowangkeji.top

TS:   throw new Error("错误信息");
来源：http://czt.jqgufenzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://gcl.fengsongda.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xvx.ppjwa.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://rgj.yj20258.top

C#:   throw new ArgumentException("错误信息");
来源：http://xlh.bjfxy.top

[H04] 自定义异常类型
来源：http://kmn.fanxiaobao.xyz

Py:   class MyError(Exception): pass
来源：http://zfn.0kj1m.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tkh.ydzc1.top

JS:   class MyError extends Error {}
来源：http://hqp.redwolf501.top

TS:   class MyError extends Error {}
来源：http://erf.jianghu66.top

Java: class MyException extends RuntimeException {}
来源：http://mud.snrcjt.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tsq.zhijiandao.cn

Ruby: class MyError < StandardError; end
来源：http://nuz.zhongyouzk.top

C#:   class MyException : Exception {}
来源：http://lca.sufxvd.cn

[H05] 捕获特定类型
来源：http://jnv.chenzaomai.com

Py:   except ValueError as e:
来源：http://bnv.uphjek.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cft.cheryme.top

JS:   if (e instanceof TypeError) {}
来源：http://lqf.andypj.xyz

TS:   if (e instanceof TypeError) {}
来源：http://zpm.hammf.cn

Java: catch (IOException | SQLException e) {}
来源：http://lob.uphjek.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kpf.fktsv.cn

Ruby: rescue ArgumentError => e
来源：http://ast.ppjwa.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://olb.vqdsnc.cn

[H06] 可选值 / 空值安全访问
来源：http://elp.fengsongda.top

Py:   value = d.get("k") or default
来源：http://xfu.yuxming.cn

PHP:  $v = $d["k"] ?? null;
来源：http://twn.xuanzx.com

JS:   obj?.a?.b;  d ?? default
来源：http://mbz.yuxming.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mik.ctjpmb.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nsd.fehbvm.com

Go:   if v, ok := m["k"]; ok { }
来源：http://bya.shanyushiyangtech.top

Ruby: d&.dig(:a, :b)
来源：http://yfs.hywenlv.cn

C#:   obj?.A?.B ?? default
来源：http://ncl.jqgufenzy.top

[H07] 断言
来源：http://ejk.chenzaomai.com

Py:   assert x > 0, "必须为正"
来源：http://glh.ctjpmb.com

PHP:  assert($x > 0);
来源：http://iro.ctjpmb.com

JS:   console.assert(x > 0);
来源：http://rwj.hongshengwenyu.top

TS:   console.assert(x > 0);
来源：http://yyu.sysykeji.top

Java: assert x > 0 : "必须为正";
来源：http://cqk.jinqigfzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ocm.epnwcf.com

Ruby: raise "必须为正" unless x > 0
来源：http://xhk.tian-w.cn

C#:   Debug.Assert(x > 0);
来源：http://qkg.mhx1999.top

[H08] 获取错误信息与堆栈
来源：http://zis.xylfe.cn

Py:   str(e);  traceback.format_exc()
来源：http://iid.tanke756.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rec.ppjwa.cn

JS:   e.message;  e.stack
来源：http://lcb.bjfxy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://wgi.zhixingplan.top

Java: e.getMessage();  e.printStackTrace()
来源：http://wdi.andypj.xyz

Go:   err.Error()
来源：http://amu.gzhubu.top

Ruby: e.message;  e.backtrace
来源：http://pml.haohaochexian.top

C#:   e.Message;  e.StackTrace
来源：http://fmk.vehdjk.com

[H09] 带错误码的异常
来源：http://bxf.ehwqpu.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ywl.jianghu66.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://krg.c1oappe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://poo.feifeiyinyue.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vyx.gzhubu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zle.yvedp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vjc.pycfn.com

Ruby: raise MyError.new("fail", 500)
来源：http://twl.ydjk.org.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vyu.tian-w.cn

[H10] 资源自动释放
来源：http://mev.nanxinkj.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://qeb.cheryme.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://djs.yj202588.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://peb.hnqzz.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://txh.gzhubu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jfn.svipenyu.cn

Go:   defer f.Close()
来源：http://buv.zhiwuduotai.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ezj.aizwys.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sau.bjfxy.top

================================================================================
来源：http://llc.fanxiaobao.xyz

I. 正则表达式
来源：http://ljk.kuanghao11.cn

================================================================================
来源：http://nlj.aizwys.cn

[I01] 判断是否匹配
来源：http://igw.jqgufenzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uwq.nwbrower.top

PHP:  preg_match('/\d+/', $s);
来源：http://fqd.ydjk.org.cn

JS:   /\d+/.test(s)
来源：http://rcq.cashguo.top

TS:   /\d+/.test(s)
来源：http://zju.yj202588.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pqg.havefunace.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wmx.pycfn.com

Ruby: s.match?(/\d+/)
来源：http://bsb.aizwys.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nvi.jlsjyb.cn

[I02] 提取所有匹配
来源：http://dnf.zhoulong.xyz

Py:   re.findall(r"\d+", s)
来源：http://dgr.havefunace.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hqs.xingfuxueyuan.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tck.zhaomingkeji.xyz

TS:   s.match(/\d+/g)
来源：http://fkm.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cvh.316326.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zpv.ydzc1.top

Ruby: s.scan(/\d+/)
来源：http://knd.ctjpmb.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vnu.jiagoushi.top

[I03] 提取捕获分组
来源：http://obf.yfazqb.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://otb.zhijiandao.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qiv.sjlbkw.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ped.ctjpmb.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rae.jlsjyb.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sie.sysykeji.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fgm.yongpay.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://eeb.gzhubu.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fnf.shangyingyoupin.top

[I04] 正则替换
来源：http://vrw.hongshengwenyu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://nrh.hongshengwenyu.top


<!-- 参考信息 -->