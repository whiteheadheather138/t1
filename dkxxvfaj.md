代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://tpv.yueranfly.top

Java: Files.size(Path.of("a.txt"))
来源：http://ciu.jqgfzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zla.sxryk.cn

Ruby: File.size("a.txt")
来源：http://khi.316326.xyz

C#:   new FileInfo("a.txt").Length
来源：http://zud.zhaomingkeji.xyz

[F10] 取文件扩展名 / 文件名
来源：http://xzp.tanke756.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://idg.wangshuangyany.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hjj.zhixingplan.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gwk.ybcxt.top

TS:   path.extname("a.txt")
来源：http://fga.svipenyu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fqs.yfazqb.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sgt.guowangkeji.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://klc.shanyushiyangkeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sbq.cheryme.top

[F11] 复制与移动文件
来源：http://cwp.wangdashe.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pow.tianlin.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wgb.epnwcf.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jzi.shuidangran.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lsm.tianlin.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nvk.tianlin.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pyq.shanyushiyangkeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qpc.ppjwa.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mfc.jianghu66.top

[F12] CSV 读写
来源：http://iiw.jinghuilouyu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dra.iojbl.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rdh.yonumen.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rmf.andypj.xyz

TS:   // 同上
来源：http://qsu.jinqigufen.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dgu.jlsjyb.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rcy.chenzaomai.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dbl.yj20258.top

C#:   // 无内置：用 CsvHelper 库
来源：http://xtx.iojbl.cn

================================================================================
来源：http://oox.ybcxt.top

G. 面向对象
来源：http://ppz.tarul.cn

================================================================================
来源：http://lgg.tanke756.top

[G01] 定义类
来源：http://ebl.cdnleiting.top

Py:   class User: pass
来源：http://nns.guannengcc.top

PHP:  class User {}
来源：http://lkr.gotoacloud.top

JS:   class User {}
来源：http://ktu.svipenyu.cn

TS:   class User { name: string = ""; }
来源：http://qbt.316326.xyz

Java: class User {}
来源：http://rnq.nwbrower.top

Go:   type User struct { Name string }
来源：http://orx.bjfxy.top

Ruby: class User; end
来源：http://qug.tanke756.top

C#:   class User {}
来源：http://ica.smart0.xyz

[G02] 构造函数
来源：http://vhh.iojbl.cn

Py:   def __init__(self, name): self.name = name
来源：http://uob.nanxuanxn.top

PHP:  public function __construct(public string $name) {}
来源：http://jil.xingfuxueyuan.xyz

JS:   constructor(name) { this.name = name; }
来源：http://srf.0kj1m.cn

TS:   constructor(public name: string) {}
来源：http://hsy.ybcxt.top

Java: User(String name) { this.name = name; }
来源：http://oyr.bjfxy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://trd.redwolf501.top

Ruby: def initialize(name); @name = name; end
来源：http://ngw.zycfv.cn

C#:   public User(string name) { Name = name; }
来源：http://txo.cqqwz.cn

[G03] 实例属性
来源：http://krq.cdnleiting.top

Py:   self.name = "x"
来源：http://ned.xziqi.cn

PHP:  public string $name = "x";
来源：http://zjd.wangshuangyany.cn

JS:   this.name = "x";
来源：http://jtt.daxiang520.top

TS:   name: string = "x";
来源：http://rso.jinqigfzy.top

Java: private String name;
来源：http://ktx.pycfn.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gid.havefunace.top

Ruby: @name = "x"
来源：http://hvo.yueranfly.top

C#:   public string Name { get; set; } = "x";
来源：http://ifu.yongpay.top

[G04] 定义方法
来源：http://rdn.jqgfzy.top

Py:   def greet(self): return self.name
来源：http://eyr.yj202588.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qik.hnxiangtu.top

JS:   greet() { return this.name; }
来源：http://hxt.tarul.cn

TS:   greet(): string { return this.name; }
来源：http://lns.yj20258888.top

Java: String greet() { return name; }
来源：http://iek.zycfv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qyx.fzhhl.top

Ruby: def greet; @name; end
来源：http://hgi.xuetiantiany.cn

C#:   public string Greet() => Name;
来源：http://cwt.fktsv.cn

[G05] 继承
来源：http://vzd.ydzc1.top

Py:   class Admin(User): pass
来源：http://ruf.0kj1m.cn

PHP:  class Admin extends User {}
来源：http://ckk.vqdsnc.cn

JS:   class Admin extends User {}
来源：http://luu.yonumen.top

TS:   class Admin extends User {}
来源：http://pyl.xingfuxueyuan.xyz

Java: class Admin extends User {}
来源：http://kdz.zhaomingkeji.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dzv.jlsjyb.cn

Ruby: class Admin < User; end
来源：http://vms.ydjk.org.cn

C#:   class Admin : User {}
来源：http://tlu.feifeiyinyue.top

[G06] 重写方法
来源：http://yob.andypj.xyz

Py:   def greet(self): return "admin"
来源：http://qph.9152youxi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hvs.316326.xyz

JS:   greet() { return "admin"; }
来源：http://zdx.bjfxy.top

TS:   greet(): string { return "admin"; }
来源：http://byd.bbcook.cn

Java: @Override String greet() { return "admin"; }
来源：http://pxu.shanyushiyangkeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kju.redwolf501.top

Ruby: def greet; "admin"; end
来源：http://xca.zhixingplan.top

C#:   public override string Greet() => "admin";
来源：http://efj.sweek.top

[G07] 调用父类方法
来源：http://evm.zdbjq.cn

Py:   super().greet()
来源：http://xlt.jinghuilouyu.cn

PHP:  parent::greet();
来源：http://pzo.haohaochexian.top

JS:   super.greet();
来源：http://rvp.hfpthk.cn

TS:   super.greet();
来源：http://jxt.hfpthk.cn

Java: super.greet();
来源：http://ljl.yfazqb.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tip.feifeiyinyue.top

Ruby: super
来源：http://zdq.xingfuxueyuan.xyz

C#:   base.Greet();
来源：http://xnm.ivvv.top

[G08] 静态方法与属性
来源：http://scv.cashguo.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bjb.chenlongwang.top

PHP:  public static function f() {}
来源：http://jou.andypj.xyz

JS:   static f() {}
来源：http://mkt.pycfn.com

TS:   static f(): void {}
来源：http://cko.zhoulong.xyz

Java: static void f() {}
来源：http://plo.fehbvm.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://hxp.aibaodan.cn

Ruby: def self.f; end
来源：http://cwy.hongshengwenyu.top

C#:   public static void F() {}
来源：http://yng.iojbl.cn

[G09] 接口 / 抽象类
来源：http://gam.316326.xyz

Py:   from abc import ABC, abstractmethod
来源：http://tlq.hywenlv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://shn.cdnleiting.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://oxt.cqqwz.cn

TS:   interface Shape { area(): number; }
来源：http://wlj.shanyushiyangtech.top

Java: interface Shape { double area(); }
来源：http://oke.zhengqikj.top

Go:   type Shape interface { Area() float64 }
来源：http://cbj.chenjidiqi.icu

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cjs.jinqigufen.top

C#:   interface IShape { double Area(); }
来源：http://jzq.zhoulong.xyz

[G10] 访问控制
来源：http://qsa.aibaodan.cn

Py:   约定 _protected / __private（不强制）
来源：http://jhz.zhaomingkeji.xyz

PHP:  public / protected / private
来源：http://pws.jinyuanbaomall.cn

JS:   #private 字段；其余公开
来源：http://nby.sufxvd.cn

TS:   public / protected / private
来源：http://xwh.aizwys.cn

Java: public / protected / private / 默认包级
来源：http://chc.fanxiaobao.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://mht.ctjpmb.com

Ruby: public / protected / private
来源：http://lqu.chenlongwang.top

C#:   public / protected / private / internal
来源：http://ybc.fktsv.cn

[G11] getter / setter
来源：http://epi.dashuyun.cn

Py:   @property 与 @x.setter
来源：http://rrg.zhongyouzk.top

PHP:  public function getName(): string { return $this->name; }
来源：http://orf.tarul.cn

JS:   get name() { return this._name; }
来源：http://xnl.jyoumei.cn

TS:   get name(): string { return this._name; }
来源：http://lnb.bjfxy.top

Java: public String getName() { return name; }
来源：http://jfz.ybcxt.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://rnh.epnwcf.com

Ruby: attr_accessor :name
来源：http://woj.guowangkeji.top

C#:   public string Name { get; set; }
来源：http://xmq.andypj.xyz

[G12] 对象转字符串
来源：http://kyq.cucudq.cn

Py:   def __str__(self): return self.name
来源：http://xiw.uphjek.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://lbr.ivvv.top

JS:   toString() { return this.name; }
来源：http://urg.ehwqpu.com

TS:   toString(): string { return this.name; }
来源：http://mpu.gotoacloud.top

Java: @Override public String toString() { return name; }
来源：http://twj.aibaodan.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xdd.zdqjudy.top

Ruby: def to_s; @name; end
来源：http://lcs.ehwqpu.com

C#:   public override string ToString() => Name;
来源：http://wco.zhixingplan.top

[G13] 判断对象类型
来源：http://obm.xuanzx.com

Py:   isinstance(u, User)
来源：http://srz.xylfe.cn

PHP:  $u instanceof User
来源：http://fez.ivvv.top

JS:   u instanceof User
来源：http://pdu.meibo888.top

TS:   u instanceof User
来源：http://hma.dianchejie.cn

Java: u instanceof User
来源：http://vxi.yj20258888.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ytt.cdnleiting.top

Ruby: u.is_a?(User)
来源：http://nvm.chenlongwang.top

C#:   u is User
来源：http://xjn.smart0.xyz

[G14] 数据类 / record
来源：http://hrt.shanyushiyangtech.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mfl.ybcxt.top

PHP:  // 用 readonly 属性模拟
来源：http://svg.zdqjudy.top

JS:   // 无内置：普通类或对象字面量
来源：http://ieu.uphjek.com

TS:   type User = { name: string; age: number };
来源：http://xuf.fzhhl.top

Java: record User(String name, int age) {}
来源：http://ang.birdmap.top

Go:   type User struct { Name string; Age int }
来源：http://gkg.shanyushiyangkeji.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dzp.c1oappe.top

C#:   record User(string Name, int Age);
来源：http://jce.uphjek.com

[G15] 枚举
来源：http://qva.nanxuanxn.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jxg.cheryme.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://heo.uphjek.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tnz.vehdjk.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://enc.vehdjk.com

Java: enum Color { RED, GREEN }
来源：http://dcu.feifeiyinyue.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kcp.hammf.cn

Ruby: Color = %i[red green].freeze
来源：http://wrv.yfazqb.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://chi.shanyushiyangkeji.top

[G16] 对象转数组 / 字典
来源：http://mae.bbcook.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://btr.havefunace.top

PHP:  get_object_vars($obj);
来源：http://sfp.daria6918.cn

JS:   Object.entries(obj)
来源：http://cpo.yonumen.top

TS:   Object.entries(obj)
来源：http://esr.wangdashe.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ibo.gaohongyu789.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://hbz.yongpay.top

Ruby: obj.instance_variables
来源：http://fpj.jiagoushi.top

C#:   // 用反射或 System.Text.Json
来源：http://ymh.yangfankeji.com

================================================================================
来源：http://rbv.tianlin.xyz

H. 异常与错误处理
来源：http://ldh.hnxiangtu.top

================================================================================
来源：http://lnw.xingfuxueyuan.xyz

[H01] try / catch 基础
来源：http://bux.vqdsnc.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ogl.yj20258888.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hor.jlsjyb.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mkd.nwbrower.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qfh.cucudq.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tcm.svipenyu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fpb.gogol.net.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ewh.aizwys.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rfl.nwbrower.top

[H02] finally / ensure 收尾
来源：http://ahl.0kj1m.cn

Py:   try: f()⏎finally: cleanup()
来源：http://hzh.ybcxt.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://osu.316326.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://xlt.guowangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://nsi.yvedp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pee.xylfe.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tek.wangshuangyany.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://weg.xinyue.icu

C#:   try { F(); } finally { Cleanup(); }
来源：http://aui.ydzc1.top

[H03] 主动抛出异常
来源：http://kmq.meibo888.top

Py:   raise ValueError("错误信息")
来源：http://tbs.ybcxt.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ipj.jinqigufen.top

JS:   throw new Error("错误信息");
来源：http://fsf.yonumen.top

TS:   throw new Error("错误信息");
来源：http://sso.cdnleiting.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://bxy.fanxiaobao.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dup.aizwys.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://nun.epnwcf.com

C#:   throw new ArgumentException("错误信息");
来源：http://tqe.ivvv.top

[H04] 自定义异常类型
来源：http://svz.ydzc1.top

Py:   class MyError(Exception): pass
来源：http://nlv.jianghu66.top

PHP:  class MyError extends RuntimeException {}
来源：http://zfz.yj20258.top

JS:   class MyError extends Error {}
来源：http://fsd.daxiang520.top

TS:   class MyError extends Error {}
来源：http://ojl.gogol.net.cn

Java: class MyException extends RuntimeException {}
来源：http://tjl.cucudq.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wiu.wangshuangyany.cn

Ruby: class MyError < StandardError; end
来源：http://fej.zhaomingkeji.xyz

C#:   class MyException : Exception {}
来源：http://tin.wangdashe.top

[H05] 捕获特定类型
来源：http://zad.sweek.top

Py:   except ValueError as e:
来源：http://hcs.ivvv.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://izb.tanke756.top

JS:   if (e instanceof TypeError) {}
来源：http://kpx.jlsjyb.cn

TS:   if (e instanceof TypeError) {}
来源：http://zti.sufxvd.cn

Java: catch (IOException | SQLException e) {}
来源：http://xis.xylfe.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cao.fanxiaobao.xyz

Ruby: rescue ArgumentError => e
来源：http://qiq.9152youxi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tmu.tian-w.cn

[H06] 可选值 / 空值安全访问
来源：http://ewl.zhaomingkeji.xyz

Py:   value = d.get("k") or default
来源：http://gku.tian-w.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rwn.nwbrower.top

JS:   obj?.a?.b;  d ?? default
来源：http://kax.gaohongyu789.top

TS:   obj?.a?.b;  d ?? default
来源：http://drs.dashuyun.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lfj.ydjk.org.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://eys.yanxiufei.cn

Ruby: d&.dig(:a, :b)
来源：http://hyl.ivvv.top

C#:   obj?.A?.B ?? default
来源：http://fhl.iojbl.cn

[H07] 断言
来源：http://voq.ehwqpu.com

Py:   assert x > 0, "必须为正"
来源：http://btu.chenzaomai.com

PHP:  assert($x > 0);
来源：http://rtd.316326.xyz

JS:   console.assert(x > 0);
来源：http://bhr.xingfuxueyuan.xyz

TS:   console.assert(x > 0);
来源：http://yjt.meibo888.top

Java: assert x > 0 : "必须为正";
来源：http://vbq.yangfankeji.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wxl.shzxlz.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rzh.jyoumei.cn

C#:   Debug.Assert(x > 0);
来源：http://pxx.jinghuilouyu.cn

[H08] 获取错误信息与堆栈
来源：http://qsg.dashuyun.cn

Py:   str(e);  traceback.format_exc()
来源：http://sto.jianghu66.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wtr.hongshengwenyu.top

JS:   e.message;  e.stack
来源：http://uvy.fzhhl.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://xmm.snrcjt.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://uqj.cdnleiting.top

Go:   err.Error()
来源：http://bta.chenzaomai.com

Ruby: e.message;  e.backtrace
来源：http://ago.zhoulong.xyz

C#:   e.Message;  e.StackTrace
来源：http://gba.nanxinkj.top

[H09] 带错误码的异常
来源：http://sdg.ydjk.org.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qxn.ctjpmb.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://adt.sufxvd.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vss.smart0.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://goj.iojbl.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ktw.guannengcc.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lld.cashguo.top

Ruby: raise MyError.new("fail", 500)
来源：http://gyb.yj202588.top

C#:   // 自定义异常类中加 Code 属性
来源：http://kcw.xingfuxueyuan.xyz

[H10] 资源自动释放
来源：http://fvf.0kj1m.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qrr.pengpengdd.cyou

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hmm.guowangkeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wgf.pengpengdd.cyou

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mww.xylfe.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rpy.hywenlv.cn

Go:   defer f.Close()
来源：http://meh.svipenyu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://utf.meibo888.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pvo.snrcjt.cn

================================================================================
来源：http://pnh.shangyingyoupin.top

I. 正则表达式
来源：http://qki.shzxlz.cn

================================================================================
来源：http://yqp.bjfxy.top

[I01] 判断是否匹配
来源：http://ise.0kj1m.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://llf.sjlbkw.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pua.tianlin.xyz

JS:   /\d+/.test(s)
来源：http://wxi.shanyushiyangtech.top

TS:   /\d+/.test(s)
来源：http://xxe.hesvh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wve.jiagoushi.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lbs.epnwcf.com

Ruby: s.match?(/\d+/)
来源：http://ter.fktsv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ndh.316326.xyz

[I02] 提取所有匹配
来源：http://qok.hammf.cn

Py:   re.findall(r"\d+", s)
来源：http://qqb.ydjk.org.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qno.hongshengwenyu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://caz.chenjidiqi.icu

TS:   s.match(/\d+/g)
来源：http://gga.xziqi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qym.zhoulong.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ezv.xingfuxueyuan.xyz

Ruby: s.scan(/\d+/)
来源：http://hwm.cashguo.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uce.vqdsnc.cn

[I03] 提取捕获分组
来源：http://fyz.gaohongyu789.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nhv.shangyingyoupin.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://idv.sysykeji.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wnk.tianlin.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tah.daxiang520.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gpx.yueranfly.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ahp.yongpay.top


<!-- 参考信息 -->