代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kzx.yuxming.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mbx.chenjidiqi.icu

[F11] 复制与移动文件
来源：http://jga.hongshengwenyu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jcn.iojbl.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://scb.ehwqpu.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kyw.52xcode.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hbt.sysykeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rts.redwolf501.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fxk.sxryk.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zjx.gotoacloud.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ozr.zhongyouzk.top

[F12] CSV 读写
来源：http://bmd.zdbjq.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pku.sweek.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ewz.sysykeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vew.yueranfly.top

TS:   // 同上
来源：http://xbu.fzhhl.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qwc.redwolf501.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ton.hfpthk.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cyv.yj202588.top

C#:   // 无内置：用 CsvHelper 库
来源：http://qqg.yj20258.top

================================================================================
来源：http://dgr.aibaodan.cn

G. 面向对象
来源：http://lzs.pycfn.com

================================================================================
来源：http://ojy.zhiwuduotai.top

[G01] 定义类
来源：http://ntt.yj20258.top

Py:   class User: pass
来源：http://ztd.vqdsnc.cn

PHP:  class User {}
来源：http://auy.chenzaomai.com

JS:   class User {}
来源：http://qrz.yonumen.top

TS:   class User { name: string = ""; }
来源：http://rpa.ybcxt.top

Java: class User {}
来源：http://usf.xinyue.icu

Go:   type User struct { Name string }
来源：http://kvh.xziqi.cn

Ruby: class User; end
来源：http://nge.zhaomingkeji.xyz

C#:   class User {}
来源：http://vad.xingfuxueyuan.xyz

[G02] 构造函数
来源：http://ntw.chenjidiqi.icu

Py:   def __init__(self, name): self.name = name
来源：http://mek.yuanzhike.top

PHP:  public function __construct(public string $name) {}
来源：http://jdn.dianchejie.cn

JS:   constructor(name) { this.name = name; }
来源：http://fxp.kuanghao11.cn

TS:   constructor(public name: string) {}
来源：http://crv.shanyushiyangkeji.top

Java: User(String name) { this.name = name; }
来源：http://fmj.cashguo.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://whk.yanxiufei.cn

Ruby: def initialize(name); @name = name; end
来源：http://ybr.fktsv.cn

C#:   public User(string name) { Name = name; }
来源：http://vao.bjfxy.top

[G03] 实例属性
来源：http://lvn.daxiang520.top

Py:   self.name = "x"
来源：http://tqf.zdbjq.cn

PHP:  public string $name = "x";
来源：http://mvg.jiagoushi.top

JS:   this.name = "x";
来源：http://wgl.zhoulong.xyz

TS:   name: string = "x";
来源：http://hde.ydjk.org.cn

Java: private String name;
来源：http://qgj.dianchejie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rhv.wangshuangyany.cn

Ruby: @name = "x"
来源：http://hqw.quarkkingdee.top

C#:   public string Name { get; set; } = "x";
来源：http://cve.ppjwa.cn

[G04] 定义方法
来源：http://zvt.xuetiantiany.cn

Py:   def greet(self): return self.name
来源：http://lzf.52xcode.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://yhb.nanxinkj.top

JS:   greet() { return this.name; }
来源：http://czo.9152youxi.cn

TS:   greet(): string { return this.name; }
来源：http://eas.hfpthk.cn

Java: String greet() { return name; }
来源：http://utc.yonumen.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://dvs.bbcook.cn

Ruby: def greet; @name; end
来源：http://ssl.kuanghao11.cn

C#:   public string Greet() => Name;
来源：http://mpr.jlsjyb.cn

[G05] 继承
来源：http://ben.hfpthk.cn

Py:   class Admin(User): pass
来源：http://gvt.chenjidiqi.icu

PHP:  class Admin extends User {}
来源：http://joc.haohaochexian.top

JS:   class Admin extends User {}
来源：http://wss.guowangkeji.top

TS:   class Admin extends User {}
来源：http://tog.aizwys.cn

Java: class Admin extends User {}
来源：http://rvs.aibaodan.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mdr.birdmap.top

Ruby: class Admin < User; end
来源：http://fhz.xuanzx.com

C#:   class Admin : User {}
来源：http://xoq.fehbvm.com

[G06] 重写方法
来源：http://mmi.zhengqikj.top

Py:   def greet(self): return "admin"
来源：http://jus.smart0.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://mrk.xuetiantiany.cn

JS:   greet() { return "admin"; }
来源：http://zeq.ydjk.org.cn

TS:   greet(): string { return "admin"; }
来源：http://egh.tian-w.cn

Java: @Override String greet() { return "admin"; }
来源：http://wwn.zhoulong.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ylx.bbcook.cn

Ruby: def greet; "admin"; end
来源：http://uas.ppjwa.cn

C#:   public override string Greet() => "admin";
来源：http://xod.sufxvd.cn

[G07] 调用父类方法
来源：http://hjt.xuanzx.com

Py:   super().greet()
来源：http://ltv.xziqi.cn

PHP:  parent::greet();
来源：http://unh.snrcjt.cn

JS:   super.greet();
来源：http://vqw.jqgufenzy.top

TS:   super.greet();
来源：http://vvu.ydzc1.top

Java: super.greet();
来源：http://nnj.zhijiandao.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pef.yongpay.top

Ruby: super
来源：http://gsf.hesvh.cn

C#:   base.Greet();
来源：http://dry.52xcode.cn

[G08] 静态方法与属性
来源：http://dab.jinghuilouyu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cns.hongshengwenyu.top

PHP:  public static function f() {}
来源：http://lmv.ydjk.org.cn

JS:   static f() {}
来源：http://dbm.zycfv.cn

TS:   static f(): void {}
来源：http://quo.sjlbkw.cn

Java: static void f() {}
来源：http://lky.uphjek.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://hwc.sjlbkw.cn

Ruby: def self.f; end
来源：http://feh.ehwqpu.com

C#:   public static void F() {}
来源：http://weh.pengpengdd.cyou

[G09] 接口 / 抽象类
来源：http://nim.zhiwuduotai.top

Py:   from abc import ABC, abstractmethod
来源：http://grf.yongpay.top

PHP:  interface Shape { public function area(): float; }
来源：http://vlu.zhiwuduotai.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://krb.hcnkem.com

TS:   interface Shape { area(): number; }
来源：http://cyx.cheryme.top

Java: interface Shape { double area(); }
来源：http://bzs.zhiwuduotai.top

Go:   type Shape interface { Area() float64 }
来源：http://dgj.jiagoushi.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zud.shanyushiyangtech.top

C#:   interface IShape { double Area(); }
来源：http://hpr.ydjk.org.cn

[G10] 访问控制
来源：http://flp.tarul.cn

Py:   约定 _protected / __private（不强制）
来源：http://rcw.wangdashe.top

PHP:  public / protected / private
来源：http://yoj.fehbvm.com

JS:   #private 字段；其余公开
来源：http://hht.jqgufenzy.top

TS:   public / protected / private
来源：http://hhl.smart0.xyz

Java: public / protected / private / 默认包级
来源：http://via.ivvv.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://dxn.xingfuxueyuan.xyz

Ruby: public / protected / private
来源：http://xei.yanxiufei.cn

C#:   public / protected / private / internal
来源：http://ptx.pengpengdd.cyou

[G11] getter / setter
来源：http://zjk.dianchejie.cn

Py:   @property 与 @x.setter
来源：http://oys.sysykeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://nkv.gzhubu.top

JS:   get name() { return this._name; }
来源：http://huo.tian-w.cn

TS:   get name(): string { return this._name; }
来源：http://bqu.daria6918.cn

Java: public String getName() { return name; }
来源：http://psf.ctjpmb.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://qlu.zhoulong.xyz

Ruby: attr_accessor :name
来源：http://mhd.uphjek.com

C#:   public string Name { get; set; }
来源：http://hxf.jinqigufen.top

[G12] 对象转字符串
来源：http://pen.hcnkem.com

Py:   def __str__(self): return self.name
来源：http://xmn.xuanzx.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://coi.gotoacloud.top

JS:   toString() { return this.name; }
来源：http://mkt.zhixingplan.top

TS:   toString(): string { return this.name; }
来源：http://jdo.fehbvm.com

Java: @Override public String toString() { return name; }
来源：http://nlf.hnqzz.top

Go:   func (u User) String() string { return u.Name }
来源：http://jvp.birdmap.top

Ruby: def to_s; @name; end
来源：http://tmn.shanyushiyangkeji.top

C#:   public override string ToString() => Name;
来源：http://wrx.hnqzz.top

[G13] 判断对象类型
来源：http://qdi.chenjidiqi.icu

Py:   isinstance(u, User)
来源：http://him.andypj.xyz

PHP:  $u instanceof User
来源：http://znq.yuanzhike.top

JS:   u instanceof User
来源：http://reb.jqgfzy.top

TS:   u instanceof User
来源：http://izm.nanxuanxn.top

Java: u instanceof User
来源：http://unj.feifeiyinyue.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ybq.gzhubu.top

Ruby: u.is_a?(User)
来源：http://khb.yangfankeji.com

C#:   u is User
来源：http://rmn.shuidangran.top

[G14] 数据类 / record
来源：http://cla.xylfe.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lei.birdmap.top

PHP:  // 用 readonly 属性模拟
来源：http://jpq.316326.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://bzy.chenjidiqi.icu

TS:   type User = { name: string; age: number };
来源：http://xgp.yueranfly.top

Java: record User(String name, int age) {}
来源：http://din.mhx1999.top

Go:   type User struct { Name string; Age int }
来源：http://bfg.jinqigufen.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ram.pengpengdd.cyou

C#:   record User(string Name, int Age);
来源：http://qyw.hfpthk.cn

[G15] 枚举
来源：http://rzz.shangyingyoupin.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://aix.gogol.net.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fyr.zhengqikj.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fsz.hfpthk.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://enm.guannengcc.top

Java: enum Color { RED, GREEN }
来源：http://gnh.shangyingyoupin.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://irk.sufxvd.cn

Ruby: Color = %i[red green].freeze
来源：http://grv.quarkkingdee.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gdc.pengpengdd.cyou

[G16] 对象转数组 / 字典
来源：http://jtg.fehbvm.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://owy.zhijiandao.cn

PHP:  get_object_vars($obj);
来源：http://hoi.iojbl.cn

JS:   Object.entries(obj)
来源：http://qff.fzhhl.top

TS:   Object.entries(obj)
来源：http://ipj.jiagoushi.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ntv.quarkkingdee.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://wvs.redwolf501.top

Ruby: obj.instance_variables
来源：http://kbh.nwbrower.top

C#:   // 用反射或 System.Text.Json
来源：http://icf.smart0.xyz

================================================================================
来源：http://rwn.gotoacloud.top

H. 异常与错误处理
来源：http://ads.andypj.xyz

================================================================================
来源：http://gmv.snrcjt.cn

[H01] try / catch 基础
来源：http://mib.jqgufenzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xiq.cdnleiting.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://epu.ydjk.org.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://src.xingfuxueyuan.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wsb.wangshuangyany.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lue.zhengqikj.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hfr.daxiang520.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vzt.hammf.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hnf.hcnkem.com

[H02] finally / ensure 收尾
来源：http://gvv.gogol.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://bag.yj20258.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://jfh.zhiwuduotai.top

JS:   try { f(); } finally { cleanup(); }
来源：http://xqn.fengsongda.top

TS:   try { f(); } finally { cleanup(); }
来源：http://pkd.dianchejie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lyd.gotoacloud.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://odc.quarkkingdee.top

Ruby: begin; f; ensure; cleanup; end
来源：http://sxh.havefunace.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://cik.zycfv.cn

[H03] 主动抛出异常
来源：http://duv.epnwcf.com

Py:   raise ValueError("错误信息")
来源：http://neu.yuxming.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yrw.zhoulong.xyz

JS:   throw new Error("错误信息");
来源：http://dmq.zdbjq.cn

TS:   throw new Error("错误信息");
来源：http://nfd.zdbjq.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://cvb.yangfankeji.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ecm.gotoacloud.top

Ruby: raise ArgumentError, "错误信息"
来源：http://cqf.zhoulong.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://uzw.vqdsnc.cn

[H04] 自定义异常类型
来源：http://bhh.zdqjudy.top

Py:   class MyError(Exception): pass
来源：http://qpr.hongshengwenyu.top

PHP:  class MyError extends RuntimeException {}
来源：http://skf.cheryme.top

JS:   class MyError extends Error {}
来源：http://zfg.sysykeji.top

TS:   class MyError extends Error {}
来源：http://uja.haohaochexian.top

Java: class MyException extends RuntimeException {}
来源：http://vnq.hfpthk.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rtd.aizwys.cn

Ruby: class MyError < StandardError; end
来源：http://mts.jyoumei.cn

C#:   class MyException : Exception {}
来源：http://dln.zdbjq.cn

[H05] 捕获特定类型
来源：http://ovx.zhixingplan.top

Py:   except ValueError as e:
来源：http://obt.shanyushiyangkeji.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zaz.sweek.top

JS:   if (e instanceof TypeError) {}
来源：http://wst.feifeiyinyue.top

TS:   if (e instanceof TypeError) {}
来源：http://oep.yj20258888.top

Java: catch (IOException | SQLException e) {}
来源：http://jsg.jyoumei.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://adm.gzhubu.top

Ruby: rescue ArgumentError => e
来源：http://avw.shuidangran.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jqp.kuanghao11.cn

[H06] 可选值 / 空值安全访问
来源：http://nfh.jinyuanbaomall.cn

Py:   value = d.get("k") or default
来源：http://smc.cucudq.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kzz.hysaishi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mha.jinghuilouyu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://htj.redwolf501.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://knt.kuanghao11.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xvl.epnwcf.com

Ruby: d&.dig(:a, :b)
来源：http://bow.zhoulong.xyz

C#:   obj?.A?.B ?? default
来源：http://fyj.hnqzz.top

[H07] 断言
来源：http://dfx.zhiwuduotai.top

Py:   assert x > 0, "必须为正"
来源：http://vdz.ehwqpu.com

PHP:  assert($x > 0);
来源：http://xsf.zdqjudy.top

JS:   console.assert(x > 0);
来源：http://jcn.xylfe.cn

TS:   console.assert(x > 0);
来源：http://car.snrcjt.cn

Java: assert x > 0 : "必须为正";
来源：http://hgu.hywenlv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cfy.cucudq.cn

Ruby: raise "必须为正" unless x > 0
来源：http://nda.yanxiufei.cn

C#:   Debug.Assert(x > 0);
来源：http://bct.pengpengdd.cyou

[H08] 获取错误信息与堆栈
来源：http://kqs.fzhhl.top

Py:   str(e);  traceback.format_exc()
来源：http://hpw.mhx1999.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://eyi.hnqzz.top

JS:   e.message;  e.stack
来源：http://shr.jinyuanbaomall.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://put.kuanghao11.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zzv.zhijiandao.cn

Go:   err.Error()
来源：http://iea.ydzc1.top

Ruby: e.message;  e.backtrace
来源：http://jdl.zycfv.cn

C#:   e.Message;  e.StackTrace
来源：http://bcj.gzhubu.top

[H09] 带错误码的异常
来源：http://fwt.zhijiandao.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hnr.cucudq.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ynf.hongshengwenyu.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://leg.yuxming.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gob.xinyue.icu

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jwk.yfazqb.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ygr.hfpthk.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ahe.xuanzx.com

C#:   // 自定义异常类中加 Code 属性
来源：http://qeh.yj20258.top

[H10] 资源自动释放
来源：http://sfb.fanxiaobao.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://qzr.hongshengwenyu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fri.yj202588.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://asd.yonumen.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rgd.fktsv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kyk.hammf.cn

Go:   defer f.Close()
来源：http://kwa.gotoacloud.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://niv.xinyue.icu

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bru.sxryk.cn

================================================================================
来源：http://eel.ivvv.top

I. 正则表达式
来源：http://oto.iojbl.cn

================================================================================
来源：http://sqt.jiagoushi.top

[I01] 判断是否匹配
来源：http://rvz.hnqzz.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zoo.jinghuilouyu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://mkg.yuxming.cn

JS:   /\d+/.test(s)
来源：http://cni.9152youxi.cn

TS:   /\d+/.test(s)
来源：http://tao.yj20258888.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ukr.yueranfly.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bat.sweek.top

Ruby: s.match?(/\d+/)
来源：http://vub.redwolf501.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yzw.fehbvm.com

[I02] 提取所有匹配
来源：http://mzb.zhengqikj.top

Py:   re.findall(r"\d+", s)
来源：http://imj.wangdashe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zxu.zhongyouzk.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uap.ctjpmb.com

TS:   s.match(/\d+/g)
来源：http://qku.shuidangran.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://txi.cheryme.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kcc.dianchejie.cn

Ruby: s.scan(/\d+/)
来源：http://sym.zycfv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qdu.tianlin.xyz

[I03] 提取捕获分组
来源：http://ave.nanxuanxn.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bsh.jyoumei.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kwx.52xcode.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bax.yvedp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rlh.jqgufenzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://roi.chenlongwang.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hir.52xcode.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gbf.dashuyun.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://awa.quarkkingdee.top

[I04] 正则替换
来源：http://yad.hysaishi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qvg.pycfn.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://igm.hfpthk.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nhq.sweek.top

TS:   s.replace(/\d+/g, "#")
来源：http://lzr.havefunace.top

Java: s.replaceAll("\\d+", "#")
来源：http://dil.pengpengdd.cyou

Go:   re.ReplaceAllString(s, "#")
来源：http://hcb.gogol.net.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://akg.yj202588.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mnm.hnxiangtu.top

[I05] 按正则拆分
来源：http://loq.hammf.cn


<!-- 参考信息 -->