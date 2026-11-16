代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mgz.jqgufenzy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ehm.havefunace.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hqj.cqqwz.cn

TS:   // 同上
来源：http://lut.zhengqikj.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vsv.gzhubu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://txz.yvedp.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lsg.xingfuxueyuan.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://akp.epnwcf.com

================================================================================
来源：http://nvo.mhx1999.top

G. 面向对象
来源：http://yfo.fanxiaobao.xyz

================================================================================
来源：http://guj.yueranfly.top

[G01] 定义类
来源：http://mar.yfazqb.com

Py:   class User: pass
来源：http://aml.sjlbkw.cn

PHP:  class User {}
来源：http://cfi.xingfuxueyuan.xyz

JS:   class User {}
来源：http://wli.yueranfly.top

TS:   class User { name: string = ""; }
来源：http://ecm.xinyue.icu

Java: class User {}
来源：http://lni.cheryme.top

Go:   type User struct { Name string }
来源：http://srl.tarul.cn

Ruby: class User; end
来源：http://grd.zhijiandao.cn

C#:   class User {}
来源：http://wzn.0kj1m.cn

[G02] 构造函数
来源：http://ujk.tarul.cn

Py:   def __init__(self, name): self.name = name
来源：http://lfl.c1oappe.top

PHP:  public function __construct(public string $name) {}
来源：http://vho.jinghuilouyu.cn

JS:   constructor(name) { this.name = name; }
来源：http://cit.gogol.net.cn

TS:   constructor(public name: string) {}
来源：http://iae.tian-w.cn

Java: User(String name) { this.name = name; }
来源：http://pyk.9152youxi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://eka.jiagoushi.top

Ruby: def initialize(name); @name = name; end
来源：http://cof.gotoacloud.top

C#:   public User(string name) { Name = name; }
来源：http://bzg.shuidangran.top

[G03] 实例属性
来源：http://otm.nanxinkj.top

Py:   self.name = "x"
来源：http://cfz.tarul.cn

PHP:  public string $name = "x";
来源：http://xfz.guowangkeji.top

JS:   this.name = "x";
来源：http://wcm.yanxiufei.cn

TS:   name: string = "x";
来源：http://kls.jianghu66.top

Java: private String name;
来源：http://gvx.vqdsnc.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jug.9152youxi.cn

Ruby: @name = "x"
来源：http://fze.yuanzhike.top

C#:   public string Name { get; set; } = "x";
来源：http://fqb.zdbjq.cn

[G04] 定义方法
来源：http://ocn.quarkkingdee.top

Py:   def greet(self): return self.name
来源：http://ynj.pengpengdd.cyou

PHP:  public function greet(): string { return $this->name; }
来源：http://rni.nanxuanxn.top

JS:   greet() { return this.name; }
来源：http://uzu.hfpthk.cn

TS:   greet(): string { return this.name; }
来源：http://guh.fanxiaobao.xyz

Java: String greet() { return name; }
来源：http://ghv.yonumen.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://gtx.gaohongyu789.top

Ruby: def greet; @name; end
来源：http://zpn.andypj.xyz

C#:   public string Greet() => Name;
来源：http://kan.vqdsnc.cn

[G05] 继承
来源：http://hmq.c1oappe.top

Py:   class Admin(User): pass
来源：http://iir.yfazqb.com

PHP:  class Admin extends User {}
来源：http://vyz.zhijiandao.cn

JS:   class Admin extends User {}
来源：http://bbp.zhongyouzk.top

TS:   class Admin extends User {}
来源：http://oqu.9152youxi.cn

Java: class Admin extends User {}
来源：http://tlm.hongshengwenyu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cnp.gaohongyu789.top

Ruby: class Admin < User; end
来源：http://mlq.gogol.net.cn

C#:   class Admin : User {}
来源：http://ccf.sufxvd.cn

[G06] 重写方法
来源：http://xbp.shuidangran.top

Py:   def greet(self): return "admin"
来源：http://fkr.wangdashe.top

PHP:  public function greet(): string { return "admin"; }
来源：http://nnh.pycfn.com

JS:   greet() { return "admin"; }
来源：http://uiw.yj202588.top

TS:   greet(): string { return "admin"; }
来源：http://ovi.aibaodan.cn

Java: @Override String greet() { return "admin"; }
来源：http://qqh.ydzc1.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lju.hysaishi.cn

Ruby: def greet; "admin"; end
来源：http://cvc.tanke756.top

C#:   public override string Greet() => "admin";
来源：http://hdq.yuxming.cn

[G07] 调用父类方法
来源：http://vje.gaohongyu789.top

Py:   super().greet()
来源：http://aut.ydzc1.top

PHP:  parent::greet();
来源：http://nwq.jlsjyb.cn

JS:   super.greet();
来源：http://cgw.aizwys.cn

TS:   super.greet();
来源：http://ayq.nanxinkj.top

Java: super.greet();
来源：http://iwc.redwolf501.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ubz.9152youxi.cn

Ruby: super
来源：http://snu.c1oappe.top

C#:   base.Greet();
来源：http://fnu.nanxinkj.top

[G08] 静态方法与属性
来源：http://tmg.xingfuxueyuan.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vdw.gogol.net.cn

PHP:  public static function f() {}
来源：http://rnw.hcnkem.com

JS:   static f() {}
来源：http://clf.sysykeji.top

TS:   static f(): void {}
来源：http://rsd.zdbjq.cn

Java: static void f() {}
来源：http://tfr.316326.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://hbk.xinyue.icu

Ruby: def self.f; end
来源：http://olr.svipenyu.cn

C#:   public static void F() {}
来源：http://zwg.mhx1999.top

[G09] 接口 / 抽象类
来源：http://qhg.cqqwz.cn

Py:   from abc import ABC, abstractmethod
来源：http://qxd.ehwqpu.com

PHP:  interface Shape { public function area(): float; }
来源：http://xte.zdqjudy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://fwo.yfazqb.com

TS:   interface Shape { area(): number; }
来源：http://xlp.jqgufenzy.top

Java: interface Shape { double area(); }
来源：http://rgh.jinqigfzy.top

Go:   type Shape interface { Area() float64 }
来源：http://xco.xinyue.icu

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fvw.xingfuxueyuan.xyz

C#:   interface IShape { double Area(); }
来源：http://gyf.yvedp.cn

[G10] 访问控制
来源：http://txo.vehdjk.com

Py:   约定 _protected / __private（不强制）
来源：http://ghn.zhongyouzk.top

PHP:  public / protected / private
来源：http://wov.hfpthk.cn

JS:   #private 字段；其余公开
来源：http://wqz.cashguo.top

TS:   public / protected / private
来源：http://idr.hesvh.cn

Java: public / protected / private / 默认包级
来源：http://hyz.chenzaomai.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://xvk.fanxiaobao.xyz

Ruby: public / protected / private
来源：http://yxv.mhx1999.top

C#:   public / protected / private / internal
来源：http://xjs.zhengqikj.top

[G11] getter / setter
来源：http://hrj.gogol.net.cn

Py:   @property 与 @x.setter
来源：http://zus.iojbl.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ffi.tianlin.xyz

JS:   get name() { return this._name; }
来源：http://zzj.yuxming.cn

TS:   get name(): string { return this._name; }
来源：http://chd.316326.xyz

Java: public String getName() { return name; }
来源：http://efu.hcnkem.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://gwy.ydjk.org.cn

Ruby: attr_accessor :name
来源：http://zer.jqgfzy.top

C#:   public string Name { get; set; }
来源：http://kyr.zdqjudy.top

[G12] 对象转字符串
来源：http://hpt.chenzaomai.com

Py:   def __str__(self): return self.name
来源：http://wqg.yanxiufei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jkk.sufxvd.cn

JS:   toString() { return this.name; }
来源：http://wxl.havefunace.top

TS:   toString(): string { return this.name; }
来源：http://afp.zycfv.cn

Java: @Override public String toString() { return name; }
来源：http://ohh.zhixingplan.top

Go:   func (u User) String() string { return u.Name }
来源：http://mfi.yangfankeji.com

Ruby: def to_s; @name; end
来源：http://jwe.quarkkingdee.top

C#:   public override string ToString() => Name;
来源：http://ttk.xylfe.cn

[G13] 判断对象类型
来源：http://lzy.wangdashe.top

Py:   isinstance(u, User)
来源：http://ryb.daria6918.cn

PHP:  $u instanceof User
来源：http://bah.ybcxt.top

JS:   u instanceof User
来源：http://tpq.hysaishi.cn

TS:   u instanceof User
来源：http://nqk.sufxvd.cn

Java: u instanceof User
来源：http://nwj.shanyushiyangtech.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://toa.smart0.xyz

Ruby: u.is_a?(User)
来源：http://rgd.birdmap.top

C#:   u is User
来源：http://xfh.dashuyun.cn

[G14] 数据类 / record
来源：http://gre.ivvv.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nmd.pycfn.com

PHP:  // 用 readonly 属性模拟
来源：http://tkq.fengsongda.top

JS:   // 无内置：普通类或对象字面量
来源：http://qvu.fengsongda.top

TS:   type User = { name: string; age: number };
来源：http://xxd.ppjwa.cn

Java: record User(String name, int age) {}
来源：http://lgv.iojbl.cn

Go:   type User struct { Name string; Age int }
来源：http://sem.xuanzx.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ggt.wangshuangyany.cn

C#:   record User(string Name, int Age);
来源：http://cxm.zhoulong.xyz

[G15] 枚举
来源：http://cdi.fanxiaobao.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bmb.hnxiangtu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://fky.pengpengdd.cyou

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yox.iojbl.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vie.nwbrower.top

Java: enum Color { RED, GREEN }
来源：http://zog.sjlbkw.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://okw.xuetiantiany.cn

Ruby: Color = %i[red green].freeze
来源：http://krr.zhoulong.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qbv.yuxming.cn

[G16] 对象转数组 / 字典
来源：http://axe.pengpengdd.cyou

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fmd.shzxlz.cn

PHP:  get_object_vars($obj);
来源：http://xlq.shanyushiyangkeji.top

JS:   Object.entries(obj)
来源：http://tqp.yuanzhike.top

TS:   Object.entries(obj)
来源：http://eoo.chenjidiqi.icu

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://psa.hongshengwenyu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://zxi.0kj1m.cn

Ruby: obj.instance_variables
来源：http://rnv.bjfxy.top

C#:   // 用反射或 System.Text.Json
来源：http://ane.vqdsnc.cn

================================================================================
来源：http://bnw.xingfuxueyuan.xyz

H. 异常与错误处理
来源：http://wsu.zycfv.cn

================================================================================
来源：http://fok.fengsongda.top

[H01] try / catch 基础
来源：http://zqz.ehwqpu.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tsu.nanxuanxn.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://afj.sweek.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rpz.zhongyouzk.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qjw.tian-w.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fik.ctjpmb.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zft.meibo888.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://buc.ydzc1.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://iqb.hysaishi.cn

[H02] finally / ensure 收尾
来源：http://bew.andypj.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://pfq.yuanzhike.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://guy.tianlin.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://mlz.c1oappe.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ftl.yangfankeji.com

Java: try { f(); } finally { cleanup(); }
来源：http://spl.haohaochexian.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://wfp.shangyingyoupin.top

Ruby: begin; f; ensure; cleanup; end
来源：http://irh.jqgufenzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ylg.nwbrower.top

[H03] 主动抛出异常
来源：http://yjt.nwbrower.top

Py:   raise ValueError("错误信息")
来源：http://txp.chenjidiqi.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zlc.hnqzz.top

JS:   throw new Error("错误信息");
来源：http://xno.feifeiyinyue.top

TS:   throw new Error("错误信息");
来源：http://gxj.jinqigufen.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://dsn.fzhhl.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tge.aizwys.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xqx.aizwys.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fmn.sysykeji.top

[H04] 自定义异常类型
来源：http://jie.sweek.top

Py:   class MyError(Exception): pass
来源：http://ppy.shanyushiyangtech.top

PHP:  class MyError extends RuntimeException {}
来源：http://gjg.jqgfzy.top

JS:   class MyError extends Error {}
来源：http://pwf.ctjpmb.com

TS:   class MyError extends Error {}
来源：http://ckp.ydzc1.top

Java: class MyException extends RuntimeException {}
来源：http://xbo.iojbl.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tyr.bbcook.cn

Ruby: class MyError < StandardError; end
来源：http://fad.c1oappe.top

C#:   class MyException : Exception {}
来源：http://unh.feifeiyinyue.top

[H05] 捕获特定类型
来源：http://wzx.xziqi.cn

Py:   except ValueError as e:
来源：http://wtt.hesvh.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://trq.guowangkeji.top

JS:   if (e instanceof TypeError) {}
来源：http://esw.aibaodan.cn

TS:   if (e instanceof TypeError) {}
来源：http://mdc.gzhubu.top

Java: catch (IOException | SQLException e) {}
来源：http://wls.fktsv.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zgs.hcnkem.com

Ruby: rescue ArgumentError => e
来源：http://pcn.316326.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hum.svipenyu.cn

[H06] 可选值 / 空值安全访问
来源：http://uqm.nanxuanxn.top

Py:   value = d.get("k") or default
来源：http://sby.jqgfzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://hpz.jinqigufen.top

JS:   obj?.a?.b;  d ?? default
来源：http://wrs.tianlin.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://kjo.zhoulong.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tah.xuanzx.com

Go:   if v, ok := m["k"]; ok { }
来源：http://xbl.zhongyouzk.top

Ruby: d&.dig(:a, :b)
来源：http://rxm.xinyue.icu

C#:   obj?.A?.B ?? default
来源：http://itw.vehdjk.com

[H07] 断言
来源：http://vpn.ybcxt.top

Py:   assert x > 0, "必须为正"
来源：http://bqq.xuanzx.com

PHP:  assert($x > 0);
来源：http://vad.ctjpmb.com

JS:   console.assert(x > 0);
来源：http://mzz.ywan-chungtsiang.top

TS:   console.assert(x > 0);
来源：http://djb.havefunace.top

Java: assert x > 0 : "必须为正";
来源：http://wgt.yfazqb.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://syg.zhaomingkeji.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://jpo.sufxvd.cn

C#:   Debug.Assert(x > 0);
来源：http://bsm.ydzc1.top

[H08] 获取错误信息与堆栈
来源：http://bvk.hammf.cn

Py:   str(e);  traceback.format_exc()
来源：http://vsc.zhaomingkeji.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ubi.ydzc1.top

JS:   e.message;  e.stack
来源：http://smq.jqgufenzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://fpc.jyoumei.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ktx.cqqwz.cn

Go:   err.Error()
来源：http://adm.c1oappe.top

Ruby: e.message;  e.backtrace
来源：http://ilp.ydzc1.top

C#:   e.Message;  e.StackTrace
来源：http://wju.gaohongyu789.top

[H09] 带错误码的异常
来源：http://ite.zdqjudy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://swt.dianchejie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mml.jlsjyb.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xhb.fehbvm.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fpv.aibaodan.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lkk.hcnkem.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hsw.mhx1999.top

Ruby: raise MyError.new("fail", 500)
来源：http://fby.fehbvm.com

C#:   // 自定义异常类中加 Code 属性
来源：http://wle.shanyushiyangkeji.top

[H10] 资源自动释放
来源：http://pvl.hongshengwenyu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ypo.fengsongda.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uje.guannengcc.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jig.gzhubu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tag.jinqigfzy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://giy.jiagoushi.top

Go:   defer f.Close()
来源：http://stp.shanyushiyangkeji.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mnc.52xcode.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cql.tarul.cn

================================================================================
来源：http://lah.guowangkeji.top

I. 正则表达式
来源：http://cft.ivvv.top

================================================================================
来源：http://yit.zhijiandao.cn

[I01] 判断是否匹配
来源：http://wmk.shanyushiyangkeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fow.quarkkingdee.top

PHP:  preg_match('/\d+/', $s);
来源：http://ewm.zhijiandao.cn

JS:   /\d+/.test(s)
来源：http://bjx.yj202588.top

TS:   /\d+/.test(s)
来源：http://nsk.hnqzz.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bhp.bjfxy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nid.epnwcf.com

Ruby: s.match?(/\d+/)
来源：http://lpg.bbcook.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mxb.9152youxi.cn

[I02] 提取所有匹配
来源：http://inr.cdnleiting.top

Py:   re.findall(r"\d+", s)
来源：http://dpw.yanxiufei.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kxg.jlsjyb.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mjp.hnqzz.top

TS:   s.match(/\d+/g)
来源：http://rva.hnqzz.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pym.birdmap.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tcf.hnxiangtu.top

Ruby: s.scan(/\d+/)
来源：http://lzl.iojbl.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gnh.vqdsnc.cn

[I03] 提取捕获分组
来源：http://zsj.daria6918.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mfs.smart0.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ois.yueranfly.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fbl.aizwys.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://koo.yj20258888.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wug.quarkkingdee.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dzq.nanxuanxn.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gdd.hongshengwenyu.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://aqw.zhixingplan.top

[I04] 正则替换
来源：http://tlf.yanxiufei.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wwm.fehbvm.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uzm.tian-w.cn

JS:   s.replace(/\d+/g, "#")
来源：http://upy.jianghu66.top

TS:   s.replace(/\d+/g, "#")
来源：http://qto.sysykeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://ddv.yfazqb.com

Go:   re.ReplaceAllString(s, "#")
来源：http://iys.sxryk.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qeo.nwbrower.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uvl.sjlbkw.cn

[I05] 按正则拆分
来源：http://kxz.chenzaomai.com

Py:   re.split(r"\s*,\s*", s)
来源：http://vpr.vqdsnc.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nlc.gogol.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://acq.9152youxi.cn

TS:   s.split(/\s*,\s*/)
来源：http://wua.yonumen.top

Java: s.split("\\s*,\\s*")
来源：http://btb.gaohongyu789.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zez.ctjpmb.com

Ruby: s.split(/\s*,\s*/)
来源：http://uyt.yuanzhike.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://htf.gaohongyu789.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vcp.pengpengdd.cyou

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hxr.cashguo.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://znn.nanxuanxn.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mwp.hywenlv.cn


<!-- 参考信息 -->