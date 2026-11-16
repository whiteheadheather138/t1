代发 wailian999

Py:   class User: pass
来源：http://irv.shanyushiyangkeji.top

PHP:  class User {}
来源：http://ncw.dianchejie.cn

JS:   class User {}
来源：http://veh.9152youxi.cn

TS:   class User { name: string = ""; }
来源：http://nbg.zhengqikj.top

Java: class User {}
来源：http://nir.yanxiufei.cn

Go:   type User struct { Name string }
来源：http://ndk.shuidangran.top

Ruby: class User; end
来源：http://iga.hesvh.cn

C#:   class User {}
来源：http://ddo.jiagoushi.top

[G02] 构造函数
来源：http://lhm.xinyue.icu

Py:   def __init__(self, name): self.name = name
来源：http://zwo.mhx1999.top

PHP:  public function __construct(public string $name) {}
来源：http://wlb.yueranfly.top

JS:   constructor(name) { this.name = name; }
来源：http://aid.zhijiandao.cn

TS:   constructor(public name: string) {}
来源：http://vkm.gotoacloud.top

Java: User(String name) { this.name = name; }
来源：http://xsa.vehdjk.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kyg.xylfe.cn

Ruby: def initialize(name); @name = name; end
来源：http://pmx.316326.xyz

C#:   public User(string name) { Name = name; }
来源：http://osr.andypj.xyz

[G03] 实例属性
来源：http://arp.guowangkeji.top

Py:   self.name = "x"
来源：http://fee.52xcode.cn

PHP:  public string $name = "x";
来源：http://sli.ppjwa.cn

JS:   this.name = "x";
来源：http://kka.chenlongwang.top

TS:   name: string = "x";
来源：http://ybg.shanyushiyangtech.top

Java: private String name;
来源：http://ede.hnqzz.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gcd.zhijiandao.cn

Ruby: @name = "x"
来源：http://kzk.gaohongyu789.top

C#:   public string Name { get; set; } = "x";
来源：http://pki.xziqi.cn

[G04] 定义方法
来源：http://xep.fzhhl.top

Py:   def greet(self): return self.name
来源：http://ogh.yfazqb.com

PHP:  public function greet(): string { return $this->name; }
来源：http://mai.jianghu66.top

JS:   greet() { return this.name; }
来源：http://yhi.yj202588.top

TS:   greet(): string { return this.name; }
来源：http://sux.xuetiantiany.cn

Java: String greet() { return name; }
来源：http://loc.guowangkeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://hay.jinqigfzy.top

Ruby: def greet; @name; end
来源：http://hae.yueranfly.top

C#:   public string Greet() => Name;
来源：http://sqr.ehwqpu.com

[G05] 继承
来源：http://kwk.smart0.xyz

Py:   class Admin(User): pass
来源：http://ynj.hfpthk.cn

PHP:  class Admin extends User {}
来源：http://kdh.shzxlz.cn

JS:   class Admin extends User {}
来源：http://qpt.svipenyu.cn

TS:   class Admin extends User {}
来源：http://iak.snrcjt.cn

Java: class Admin extends User {}
来源：http://zvs.yongpay.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nwh.chenlongwang.top

Ruby: class Admin < User; end
来源：http://mvv.cucudq.cn

C#:   class Admin : User {}
来源：http://lkl.hywenlv.cn

[G06] 重写方法
来源：http://lwk.gotoacloud.top

Py:   def greet(self): return "admin"
来源：http://git.uphjek.com

PHP:  public function greet(): string { return "admin"; }
来源：http://ydc.quarkkingdee.top

JS:   greet() { return "admin"; }
来源：http://wgc.dashuyun.cn

TS:   greet(): string { return "admin"; }
来源：http://hxp.ybcxt.top

Java: @Override String greet() { return "admin"; }
来源：http://ikj.xziqi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qlh.shangyingyoupin.top

Ruby: def greet; "admin"; end
来源：http://qsr.zhaomingkeji.xyz

C#:   public override string Greet() => "admin";
来源：http://qyq.yongpay.top

[G07] 调用父类方法
来源：http://mqm.hammf.cn

Py:   super().greet()
来源：http://vft.zycfv.cn

PHP:  parent::greet();
来源：http://jan.fehbvm.com

JS:   super.greet();
来源：http://ddk.pycfn.com

TS:   super.greet();
来源：http://zhj.shanyushiyangkeji.top

Java: super.greet();
来源：http://tow.cqqwz.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mjv.tian-w.cn

Ruby: super
来源：http://zwd.yongpay.top

C#:   base.Greet();
来源：http://ujm.jqgufenzy.top

[G08] 静态方法与属性
来源：http://alb.hnxiangtu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mvc.ehwqpu.com

PHP:  public static function f() {}
来源：http://zdl.yj202588.top

JS:   static f() {}
来源：http://dki.zycfv.cn

TS:   static f(): void {}
来源：http://pdu.jqgufenzy.top

Java: static void f() {}
来源：http://dvx.chenjidiqi.icu

Go:   // 无 static：用包级函数，按包名调用
来源：http://kea.zhiwuduotai.top

Ruby: def self.f; end
来源：http://ekj.zdbjq.cn

C#:   public static void F() {}
来源：http://jjq.jqgufenzy.top

[G09] 接口 / 抽象类
来源：http://bcp.redwolf501.top

Py:   from abc import ABC, abstractmethod
来源：http://cxu.fengsongda.top

PHP:  interface Shape { public function area(): float; }
来源：http://ujs.sysykeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://hmi.fanxiaobao.xyz

TS:   interface Shape { area(): number; }
来源：http://ieg.shzxlz.cn

Java: interface Shape { double area(); }
来源：http://otl.yj202588.top

Go:   type Shape interface { Area() float64 }
来源：http://svr.iojbl.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uxi.xingfuxueyuan.xyz

C#:   interface IShape { double Area(); }
来源：http://xwp.zhijiandao.cn

[G10] 访问控制
来源：http://zrk.aibaodan.cn

Py:   约定 _protected / __private（不强制）
来源：http://pys.xuetiantiany.cn

PHP:  public / protected / private
来源：http://wqf.zhoulong.xyz

JS:   #private 字段；其余公开
来源：http://tcy.ywan-chungtsiang.top

TS:   public / protected / private
来源：http://lsm.yuanzhike.top

Java: public / protected / private / 默认包级
来源：http://ejd.sxryk.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fdw.yongpay.top

Ruby: public / protected / private
来源：http://cdw.zhoulong.xyz

C#:   public / protected / private / internal
来源：http://ctn.zdqjudy.top

[G11] getter / setter
来源：http://ziv.zhaomingkeji.xyz

Py:   @property 与 @x.setter
来源：http://yvz.hnqzz.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ymg.kuanghao11.cn

JS:   get name() { return this._name; }
来源：http://eha.9152youxi.cn

TS:   get name(): string { return this._name; }
来源：http://jac.chenjidiqi.icu

Java: public String getName() { return name; }
来源：http://gvk.yueranfly.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://daj.yonumen.top

Ruby: attr_accessor :name
来源：http://yqe.gotoacloud.top

C#:   public string Name { get; set; }
来源：http://vgr.zhongyouzk.top

[G12] 对象转字符串
来源：http://bpx.cqqwz.cn

Py:   def __str__(self): return self.name
来源：http://ttx.xuetiantiany.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hvf.zycfv.cn

JS:   toString() { return this.name; }
来源：http://pwv.aizwys.cn

TS:   toString(): string { return this.name; }
来源：http://mwx.ppjwa.cn

Java: @Override public String toString() { return name; }
来源：http://okd.tarul.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ody.jlsjyb.cn

Ruby: def to_s; @name; end
来源：http://zzy.yonumen.top

C#:   public override string ToString() => Name;
来源：http://ief.jinghuilouyu.cn

[G13] 判断对象类型
来源：http://zta.dashuyun.cn

Py:   isinstance(u, User)
来源：http://zao.smart0.xyz

PHP:  $u instanceof User
来源：http://tkj.jqgufenzy.top

JS:   u instanceof User
来源：http://hcv.zdbjq.cn

TS:   u instanceof User
来源：http://ekc.gotoacloud.top

Java: u instanceof User
来源：http://lwy.yj20258.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://qvh.guowangkeji.top

Ruby: u.is_a?(User)
来源：http://nhq.zhaomingkeji.xyz

C#:   u is User
来源：http://jwi.meibo888.top

[G14] 数据类 / record
来源：http://min.daria6918.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://njt.vehdjk.com

PHP:  // 用 readonly 属性模拟
来源：http://gsv.yvedp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rkm.fzhhl.top

TS:   type User = { name: string; age: number };
来源：http://uiu.cqqwz.cn

Java: record User(String name, int age) {}
来源：http://svf.meibo888.top

Go:   type User struct { Name string; Age int }
来源：http://flo.chenjidiqi.icu

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://elg.tanke756.top

C#:   record User(string Name, int Age);
来源：http://kcm.0kj1m.cn

[G15] 枚举
来源：http://heh.tanke756.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ozn.yj20258888.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://typ.cqqwz.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bzl.c1oappe.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yay.kuanghao11.cn

Java: enum Color { RED, GREEN }
来源：http://adu.jiagoushi.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pyk.havefunace.top

Ruby: Color = %i[red green].freeze
来源：http://eds.tarul.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://snh.zycfv.cn

[G16] 对象转数组 / 字典
来源：http://ocp.zhengqikj.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://plq.snrcjt.cn

PHP:  get_object_vars($obj);
来源：http://sch.haohaochexian.top

JS:   Object.entries(obj)
来源：http://pom.feifeiyinyue.top

TS:   Object.entries(obj)
来源：http://ehn.sysykeji.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jxp.vehdjk.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://ihv.cashguo.top

Ruby: obj.instance_variables
来源：http://gex.gaohongyu789.top

C#:   // 用反射或 System.Text.Json
来源：http://vkt.havefunace.top

================================================================================
来源：http://nxi.hesvh.cn

H. 异常与错误处理
来源：http://ihs.jinqigfzy.top

================================================================================
来源：http://pya.ehwqpu.com

[H01] try / catch 基础
来源：http://fjc.cdnleiting.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vbd.fengsongda.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yub.bjfxy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qvm.shanyushiyangtech.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bxz.cdnleiting.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jgg.shzxlz.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://oiu.cheryme.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vmc.yj20258.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pof.meibo888.top

[H02] finally / ensure 收尾
来源：http://heg.jqgufenzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://umb.cqqwz.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wiv.sysykeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://tml.shanyushiyangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://cax.jinghuilouyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://mau.vehdjk.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://qgw.zhixingplan.top

Ruby: begin; f; ensure; cleanup; end
来源：http://qra.zhongyouzk.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://amx.cucudq.cn

[H03] 主动抛出异常
来源：http://fxo.cashguo.top

Py:   raise ValueError("错误信息")
来源：http://vnx.gogol.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xdj.yueranfly.top

JS:   throw new Error("错误信息");
来源：http://phx.bbcook.cn

TS:   throw new Error("错误信息");
来源：http://acw.havefunace.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://tql.hnxiangtu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oov.zhoulong.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://dzc.yongpay.top

C#:   throw new ArgumentException("错误信息");
来源：http://xdo.quarkkingdee.top

[H04] 自定义异常类型
来源：http://phx.hesvh.cn

Py:   class MyError(Exception): pass
来源：http://rie.dianchejie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gwv.52xcode.cn

JS:   class MyError extends Error {}
来源：http://qfq.gotoacloud.top

TS:   class MyError extends Error {}
来源：http://idf.hfpthk.cn

Java: class MyException extends RuntimeException {}
来源：http://dbp.sxryk.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pcc.xinyue.icu

Ruby: class MyError < StandardError; end
来源：http://yme.daxiang520.top

C#:   class MyException : Exception {}
来源：http://pti.sweek.top

[H05] 捕获特定类型
来源：http://mks.xingfuxueyuan.xyz

Py:   except ValueError as e:
来源：http://hhk.sxryk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kof.c1oappe.top

JS:   if (e instanceof TypeError) {}
来源：http://auz.jinqigfzy.top

TS:   if (e instanceof TypeError) {}
来源：http://uzv.zhijiandao.cn

Java: catch (IOException | SQLException e) {}
来源：http://srb.yanxiufei.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lyh.svipenyu.cn

Ruby: rescue ArgumentError => e
来源：http://zox.yangfankeji.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uot.jqgufenzy.top

[H06] 可选值 / 空值安全访问
来源：http://pkg.hammf.cn

Py:   value = d.get("k") or default
来源：http://wxm.hammf.cn

PHP:  $v = $d["k"] ?? null;
来源：http://nki.316326.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://ows.chenjidiqi.icu

TS:   obj?.a?.b;  d ?? default
来源：http://yto.pengpengdd.cyou

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ihl.fehbvm.com

Go:   if v, ok := m["k"]; ok { }
来源：http://lfe.jinqigfzy.top

Ruby: d&.dig(:a, :b)
来源：http://koc.nanxuanxn.top

C#:   obj?.A?.B ?? default
来源：http://obq.hcnkem.com

[H07] 断言
来源：http://ukr.tanke756.top

Py:   assert x > 0, "必须为正"
来源：http://usy.yj20258888.top

PHP:  assert($x > 0);
来源：http://mpj.jyoumei.cn

JS:   console.assert(x > 0);
来源：http://shf.fanxiaobao.xyz

TS:   console.assert(x > 0);
来源：http://kqm.pengpengdd.cyou

Java: assert x > 0 : "必须为正";
来源：http://smr.hongshengwenyu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nwa.redwolf501.top

Ruby: raise "必须为正" unless x > 0
来源：http://ebc.ehwqpu.com

C#:   Debug.Assert(x > 0);
来源：http://roy.hfpthk.cn

[H08] 获取错误信息与堆栈
来源：http://lag.zhaomingkeji.xyz

Py:   str(e);  traceback.format_exc()
来源：http://dkk.pengpengdd.cyou

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://asu.smart0.xyz

JS:   e.message;  e.stack
来源：http://ndz.chenjidiqi.icu

TS:   e instanceof Error ? e.message : String(e)
来源：http://dsm.jiagoushi.top

Java: e.getMessage();  e.printStackTrace()
来源：http://sbt.316326.xyz

Go:   err.Error()
来源：http://kbm.ehwqpu.com

Ruby: e.message;  e.backtrace
来源：http://pdc.daxiang520.top

C#:   e.Message;  e.StackTrace
来源：http://rsq.zhaomingkeji.xyz

[H09] 带错误码的异常
来源：http://qdd.sjlbkw.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cel.yj20258888.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://mda.daxiang520.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yhi.iojbl.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yfw.sufxvd.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://drz.birdmap.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vdk.yueranfly.top

Ruby: raise MyError.new("fail", 500)
来源：http://xdw.daria6918.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://dip.zhixingplan.top

[H10] 资源自动释放
来源：http://gjs.tanke756.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://hue.zhixingplan.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mzx.fktsv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mdr.feifeiyinyue.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dql.bbcook.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://iua.zhijiandao.cn

Go:   defer f.Close()
来源：http://yax.yongpay.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vwd.zhoulong.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mwv.aibaodan.cn

================================================================================
来源：http://ply.shanyushiyangtech.top

I. 正则表达式
来源：http://xwf.fanxiaobao.xyz

================================================================================
来源：http://dep.feifeiyinyue.top

[I01] 判断是否匹配
来源：http://eug.jinqigfzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ocj.zhoulong.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://uxz.shuidangran.top

JS:   /\d+/.test(s)
来源：http://qdt.cqqwz.cn

TS:   /\d+/.test(s)
来源：http://qrp.yangfankeji.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qbb.aibaodan.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://udi.sxryk.cn

Ruby: s.match?(/\d+/)
来源：http://qve.hongshengwenyu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dwi.yangfankeji.com

[I02] 提取所有匹配
来源：http://yho.jqgfzy.top

Py:   re.findall(r"\d+", s)
来源：http://okv.xinyue.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uot.nanxinkj.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://muv.bjfxy.top

TS:   s.match(/\d+/g)
来源：http://gxj.ydjk.org.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xxy.tian-w.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rdy.xinyue.icu

Ruby: s.scan(/\d+/)
来源：http://hzu.ctjpmb.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ldp.pengpengdd.cyou

[I03] 提取捕获分组
来源：http://gwx.hfpthk.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dkp.hnqzz.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vjv.hcnkem.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://grz.bbcook.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ltl.zhijiandao.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rsp.xuanzx.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wwn.bbcook.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://byh.shanyushiyangkeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nrf.yueranfly.top

[I04] 正则替换
来源：http://ptc.fanxiaobao.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://aux.hfpthk.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nfw.zycfv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xwb.hnxiangtu.top

TS:   s.replace(/\d+/g, "#")
来源：http://ufl.xziqi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ptu.yangfankeji.com

Go:   re.ReplaceAllString(s, "#")
来源：http://mmf.sysykeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://wvk.smart0.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hnb.dianchejie.cn

[I05] 按正则拆分
来源：http://qau.ivvv.top

Py:   re.split(r"\s*,\s*", s)
来源：http://gbe.vehdjk.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jst.bjfxy.top

JS:   s.split(/\s*,\s*/)
来源：http://ymo.dashuyun.cn

TS:   s.split(/\s*,\s*/)
来源：http://xrw.redwolf501.top

Java: s.split("\\s*,\\s*")
来源：http://eoi.hysaishi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qju.gaohongyu789.top

Ruby: s.split(/\s*,\s*/)
来源：http://mzs.pycfn.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qtt.iojbl.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://krs.gotoacloud.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vap.vehdjk.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rfi.tianlin.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nks.cucudq.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://exm.jinyuanbaomall.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nps.guannengcc.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://luu.zhoulong.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://psl.9152youxi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hyx.52xcode.cn

[I07] 忽略大小写与多行模式
来源：http://xix.ppjwa.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://aps.cqqwz.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://svc.hcnkem.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yej.hesvh.cn

TS:   /error/gim
来源：http://iyg.yfazqb.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gue.ppjwa.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dbt.xuetiantiany.cn


<!-- 参考信息 -->