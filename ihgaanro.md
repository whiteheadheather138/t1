代发 wailian999

================================================================================
来源：http://dls.316326.xyz

G. 面向对象
来源：http://ppl.zhijiandao.cn

================================================================================
来源：http://rfx.cqqwz.cn

[G01] 定义类
来源：http://cjt.yongpay.top

Py:   class User: pass
来源：http://xad.tarul.cn

PHP:  class User {}
来源：http://fzo.nwbrower.top

JS:   class User {}
来源：http://yao.yangfankeji.com

TS:   class User { name: string = ""; }
来源：http://osb.dianchejie.cn

Java: class User {}
来源：http://kbn.vehdjk.com

Go:   type User struct { Name string }
来源：http://pjw.dashuyun.cn

Ruby: class User; end
来源：http://tjj.xziqi.cn

C#:   class User {}
来源：http://ytz.dianchejie.cn

[G02] 构造函数
来源：http://bue.feifeiyinyue.top

Py:   def __init__(self, name): self.name = name
来源：http://cpz.sweek.top

PHP:  public function __construct(public string $name) {}
来源：http://xtf.yangfankeji.com

JS:   constructor(name) { this.name = name; }
来源：http://lqg.yj20258.top

TS:   constructor(public name: string) {}
来源：http://nxu.52xcode.cn

Java: User(String name) { this.name = name; }
来源：http://cei.ehwqpu.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yio.dashuyun.cn

Ruby: def initialize(name); @name = name; end
来源：http://vrq.hesvh.cn

C#:   public User(string name) { Name = name; }
来源：http://zdu.shanyushiyangtech.top

[G03] 实例属性
来源：http://lap.fanxiaobao.xyz

Py:   self.name = "x"
来源：http://bpj.sweek.top

PHP:  public string $name = "x";
来源：http://xxh.hfpthk.cn

JS:   this.name = "x";
来源：http://vys.xinyue.icu

TS:   name: string = "x";
来源：http://zqw.xinyue.icu

Java: private String name;
来源：http://pxd.vehdjk.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fgz.xuanzx.com

Ruby: @name = "x"
来源：http://zij.vqdsnc.cn

C#:   public string Name { get; set; } = "x";
来源：http://fkh.yvedp.cn

[G04] 定义方法
来源：http://ycr.yangfankeji.com

Py:   def greet(self): return self.name
来源：http://xrc.mhx1999.top

PHP:  public function greet(): string { return $this->name; }
来源：http://dbk.tianlin.xyz

JS:   greet() { return this.name; }
来源：http://fzu.tarul.cn

TS:   greet(): string { return this.name; }
来源：http://zaz.redwolf501.top

Java: String greet() { return name; }
来源：http://dia.havefunace.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://imy.jqgfzy.top

Ruby: def greet; @name; end
来源：http://csf.zhongyouzk.top

C#:   public string Greet() => Name;
来源：http://reo.xylfe.cn

[G05] 继承
来源：http://uew.dianchejie.cn

Py:   class Admin(User): pass
来源：http://mpi.chenjidiqi.icu

PHP:  class Admin extends User {}
来源：http://aqn.316326.xyz

JS:   class Admin extends User {}
来源：http://yma.fzhhl.top

TS:   class Admin extends User {}
来源：http://duy.zhengqikj.top

Java: class Admin extends User {}
来源：http://jij.jlsjyb.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://keb.svipenyu.cn

Ruby: class Admin < User; end
来源：http://tci.jianghu66.top

C#:   class Admin : User {}
来源：http://egr.dashuyun.cn

[G06] 重写方法
来源：http://uav.xylfe.cn

Py:   def greet(self): return "admin"
来源：http://vam.dashuyun.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hho.hcnkem.com

JS:   greet() { return "admin"; }
来源：http://vxn.316326.xyz

TS:   greet(): string { return "admin"; }
来源：http://ocu.zhoulong.xyz

Java: @Override String greet() { return "admin"; }
来源：http://hzu.nanxuanxn.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ath.tarul.cn

Ruby: def greet; "admin"; end
来源：http://gxc.chenjidiqi.icu

C#:   public override string Greet() => "admin";
来源：http://kfo.sweek.top

[G07] 调用父类方法
来源：http://hms.dianchejie.cn

Py:   super().greet()
来源：http://lov.jinqigufen.top

PHP:  parent::greet();
来源：http://eox.shzxlz.cn

JS:   super.greet();
来源：http://zqs.zdqjudy.top

TS:   super.greet();
来源：http://ieq.hywenlv.cn

Java: super.greet();
来源：http://jap.wangshuangyany.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tdo.cucudq.cn

Ruby: super
来源：http://ssf.jqgufenzy.top

C#:   base.Greet();
来源：http://zgq.yj20258888.top

[G08] 静态方法与属性
来源：http://rfh.dashuyun.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hvc.yj20258888.top

PHP:  public static function f() {}
来源：http://rve.fehbvm.com

JS:   static f() {}
来源：http://odb.zhoulong.xyz

TS:   static f(): void {}
来源：http://zpt.c1oappe.top

Java: static void f() {}
来源：http://kto.fehbvm.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://gft.hesvh.cn

Ruby: def self.f; end
来源：http://swi.ivvv.top

C#:   public static void F() {}
来源：http://dlz.guannengcc.top

[G09] 接口 / 抽象类
来源：http://sda.shuidangran.top

Py:   from abc import ABC, abstractmethod
来源：http://vis.pengpengdd.cyou

PHP:  interface Shape { public function area(): float; }
来源：http://hte.smart0.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://fut.cqqwz.cn

TS:   interface Shape { area(): number; }
来源：http://mhx.vehdjk.com

Java: interface Shape { double area(); }
来源：http://uzl.zhijiandao.cn

Go:   type Shape interface { Area() float64 }
来源：http://kyo.hammf.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://naf.wangshuangyany.cn

C#:   interface IShape { double Area(); }
来源：http://zvp.zycfv.cn

[G10] 访问控制
来源：http://qrp.vehdjk.com

Py:   约定 _protected / __private（不强制）
来源：http://ywn.yongpay.top

PHP:  public / protected / private
来源：http://evg.ydjk.org.cn

JS:   #private 字段；其余公开
来源：http://gyx.hnqzz.top

TS:   public / protected / private
来源：http://cbf.xylfe.cn

Java: public / protected / private / 默认包级
来源：http://kdq.52xcode.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://zmx.meibo888.top

Ruby: public / protected / private
来源：http://plf.xylfe.cn

C#:   public / protected / private / internal
来源：http://peg.svipenyu.cn

[G11] getter / setter
来源：http://uqs.shzxlz.cn

Py:   @property 与 @x.setter
来源：http://for.quarkkingdee.top

PHP:  public function getName(): string { return $this->name; }
来源：http://syf.fehbvm.com

JS:   get name() { return this._name; }
来源：http://lxz.hesvh.cn

TS:   get name(): string { return this._name; }
来源：http://gxb.snrcjt.cn

Java: public String getName() { return name; }
来源：http://onx.fanxiaobao.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://mui.bbcook.cn

Ruby: attr_accessor :name
来源：http://gcx.nanxuanxn.top

C#:   public string Name { get; set; }
来源：http://gri.guannengcc.top

[G12] 对象转字符串
来源：http://ftl.shanyushiyangkeji.top

Py:   def __str__(self): return self.name
来源：http://kro.yj202588.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://zxu.zhiwuduotai.top

JS:   toString() { return this.name; }
来源：http://uec.chenlongwang.top

TS:   toString(): string { return this.name; }
来源：http://sbr.gogol.net.cn

Java: @Override public String toString() { return name; }
来源：http://wyq.gotoacloud.top

Go:   func (u User) String() string { return u.Name }
来源：http://hzk.mhx1999.top

Ruby: def to_s; @name; end
来源：http://nqg.pycfn.com

C#:   public override string ToString() => Name;
来源：http://fmw.snrcjt.cn

[G13] 判断对象类型
来源：http://jbe.cdnleiting.top

Py:   isinstance(u, User)
来源：http://alr.uphjek.com

PHP:  $u instanceof User
来源：http://cru.zhiwuduotai.top

JS:   u instanceof User
来源：http://rvo.cheryme.top

TS:   u instanceof User
来源：http://sns.bjfxy.top

Java: u instanceof User
来源：http://dwk.guowangkeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://wkr.sxryk.cn

Ruby: u.is_a?(User)
来源：http://umh.yj20258.top

C#:   u is User
来源：http://ppy.fanxiaobao.xyz

[G14] 数据类 / record
来源：http://qyu.uphjek.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zfc.sjlbkw.cn

PHP:  // 用 readonly 属性模拟
来源：http://krj.mhx1999.top

JS:   // 无内置：普通类或对象字面量
来源：http://gws.jiagoushi.top

TS:   type User = { name: string; age: number };
来源：http://iji.gogol.net.cn

Java: record User(String name, int age) {}
来源：http://oyy.gzhubu.top

Go:   type User struct { Name string; Age int }
来源：http://qtb.pycfn.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ulu.xuetiantiany.cn

C#:   record User(string Name, int Age);
来源：http://zsq.jianghu66.top

[G15] 枚举
来源：http://etc.pengpengdd.cyou

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sqx.shuidangran.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://scj.jinqigufen.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://orj.wangshuangyany.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://obh.xuanzx.com

Java: enum Color { RED, GREEN }
来源：http://bzj.zhaomingkeji.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kke.yonumen.top

Ruby: Color = %i[red green].freeze
来源：http://zuq.shanyushiyangkeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rqx.hywenlv.cn

[G16] 对象转数组 / 字典
来源：http://thr.guowangkeji.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fzt.vqdsnc.cn

PHP:  get_object_vars($obj);
来源：http://otq.yj20258.top

JS:   Object.entries(obj)
来源：http://kcw.ywan-chungtsiang.top

TS:   Object.entries(obj)
来源：http://rif.tian-w.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mtc.nanxuanxn.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://atx.yj20258.top

Ruby: obj.instance_variables
来源：http://cds.smart0.xyz

C#:   // 用反射或 System.Text.Json
来源：http://mii.dashuyun.cn

================================================================================
来源：http://fdw.guowangkeji.top

H. 异常与错误处理
来源：http://avw.chenjidiqi.icu

================================================================================
来源：http://gwi.yuxming.cn

[H01] try / catch 基础
来源：http://zwe.gotoacloud.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wzn.vqdsnc.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zpg.sufxvd.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tqr.yj20258.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://isx.pycfn.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vke.shanyushiyangtech.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yip.andypj.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pvx.uphjek.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bdw.gotoacloud.top

[H02] finally / ensure 收尾
来源：http://duo.jinqigufen.top

Py:   try: f()⏎finally: cleanup()
来源：http://vci.xingfuxueyuan.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://amd.mhx1999.top

JS:   try { f(); } finally { cleanup(); }
来源：http://qut.fzhhl.top

TS:   try { f(); } finally { cleanup(); }
来源：http://sub.gzhubu.top

Java: try { f(); } finally { cleanup(); }
来源：http://vfx.jiagoushi.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ihs.shzxlz.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://iay.redwolf501.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://amh.pycfn.com

[H03] 主动抛出异常
来源：http://lfi.hfpthk.cn

Py:   raise ValueError("错误信息")
来源：http://heo.jyoumei.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://meq.redwolf501.top

JS:   throw new Error("错误信息");
来源：http://prt.jqgfzy.top

TS:   throw new Error("错误信息");
来源：http://mft.iojbl.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://wmf.yuanzhike.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://elo.ybcxt.top

Ruby: raise ArgumentError, "错误信息"
来源：http://pwd.hongshengwenyu.top

C#:   throw new ArgumentException("错误信息");
来源：http://apg.jiagoushi.top

[H04] 自定义异常类型
来源：http://lrn.bbcook.cn

Py:   class MyError(Exception): pass
来源：http://npj.hywenlv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://egw.jinqigufen.top

JS:   class MyError extends Error {}
来源：http://zwz.hnqzz.top

TS:   class MyError extends Error {}
来源：http://yvd.pengpengdd.cyou

Java: class MyException extends RuntimeException {}
来源：http://xji.sysykeji.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://afy.fzhhl.top

Ruby: class MyError < StandardError; end
来源：http://fdp.sweek.top

C#:   class MyException : Exception {}
来源：http://agx.iojbl.cn

[H05] 捕获特定类型
来源：http://qth.fzhhl.top

Py:   except ValueError as e:
来源：http://blk.jinqigfzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oyk.nwbrower.top

JS:   if (e instanceof TypeError) {}
来源：http://xbp.jinqigufen.top

TS:   if (e instanceof TypeError) {}
来源：http://ttd.mhx1999.top

Java: catch (IOException | SQLException e) {}
来源：http://cax.316326.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hox.vehdjk.com

Ruby: rescue ArgumentError => e
来源：http://swh.ehwqpu.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kus.jinqigfzy.top

[H06] 可选值 / 空值安全访问
来源：http://frp.smart0.xyz

Py:   value = d.get("k") or default
来源：http://agz.pengpengdd.cyou

PHP:  $v = $d["k"] ?? null;
来源：http://gbr.snrcjt.cn

JS:   obj?.a?.b;  d ?? default
来源：http://aiw.ehwqpu.com

TS:   obj?.a?.b;  d ?? default
来源：http://wws.yuxming.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sfj.hnqzz.top

Go:   if v, ok := m["k"]; ok { }
来源：http://wic.iojbl.cn

Ruby: d&.dig(:a, :b)
来源：http://tsr.snrcjt.cn

C#:   obj?.A?.B ?? default
来源：http://qgl.pengpengdd.cyou

[H07] 断言
来源：http://nrl.zycfv.cn

Py:   assert x > 0, "必须为正"
来源：http://kxl.yj202588.top

PHP:  assert($x > 0);
来源：http://tyg.ppjwa.cn

JS:   console.assert(x > 0);
来源：http://xkk.yj20258.top

TS:   console.assert(x > 0);
来源：http://xvt.jyoumei.cn

Java: assert x > 0 : "必须为正";
来源：http://rya.yuxming.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pje.52xcode.cn

Ruby: raise "必须为正" unless x > 0
来源：http://twm.jqgufenzy.top

C#:   Debug.Assert(x > 0);
来源：http://sqe.hywenlv.cn

[H08] 获取错误信息与堆栈
来源：http://rnz.hammf.cn

Py:   str(e);  traceback.format_exc()
来源：http://bet.hesvh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vod.jyoumei.cn

JS:   e.message;  e.stack
来源：http://nch.zhijiandao.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dma.shzxlz.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://lte.yueranfly.top

Go:   err.Error()
来源：http://jpk.xziqi.cn

Ruby: e.message;  e.backtrace
来源：http://kfr.hammf.cn

C#:   e.Message;  e.StackTrace
来源：http://fdv.sjlbkw.cn

[H09] 带错误码的异常
来源：http://uea.cqqwz.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wjz.havefunace.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://gyg.xingfuxueyuan.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://oto.c1oappe.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rxx.yangfankeji.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yar.pengpengdd.cyou

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ezm.dianchejie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hic.xuanzx.com

C#:   // 自定义异常类中加 Code 属性
来源：http://rda.shzxlz.cn

[H10] 资源自动释放
来源：http://xxt.nanxinkj.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ijd.xingfuxueyuan.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ryt.0kj1m.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wbj.zhaomingkeji.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kkv.zhiwuduotai.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vhg.hongshengwenyu.top

Go:   defer f.Close()
来源：http://ala.fktsv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gaq.c1oappe.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lwy.yangfankeji.com

================================================================================
来源：http://wvv.xylfe.cn

I. 正则表达式
来源：http://gcd.ehwqpu.com

================================================================================
来源：http://xac.ppjwa.cn

[I01] 判断是否匹配
来源：http://uyn.hfpthk.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ens.nanxuanxn.top

PHP:  preg_match('/\d+/', $s);
来源：http://miq.hnxiangtu.top

JS:   /\d+/.test(s)
来源：http://tyl.hammf.cn

TS:   /\d+/.test(s)
来源：http://yed.pengpengdd.cyou

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fgq.hesvh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jza.ydzc1.top

Ruby: s.match?(/\d+/)
来源：http://dhq.nwbrower.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://geh.chenlongwang.top

[I02] 提取所有匹配
来源：http://esa.shangyingyoupin.top

Py:   re.findall(r"\d+", s)
来源：http://svp.daxiang520.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tff.bjfxy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jmj.jyoumei.cn

TS:   s.match(/\d+/g)
来源：http://hjx.meibo888.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bqb.birdmap.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ekc.xuetiantiany.cn

Ruby: s.scan(/\d+/)
来源：http://mqy.jqgufenzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://phc.guannengcc.top

[I03] 提取捕获分组
来源：http://wiu.meibo888.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zbq.redwolf501.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uos.redwolf501.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xgz.zdbjq.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jlv.hysaishi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qrq.yfazqb.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dkq.wangdashe.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://akd.hnxiangtu.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dik.fanxiaobao.xyz

[I04] 正则替换
来源：http://cbi.xylfe.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kuc.zhixingplan.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hqt.haohaochexian.top

JS:   s.replace(/\d+/g, "#")
来源：http://xpd.zhaomingkeji.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://qxy.yj20258.top

Java: s.replaceAll("\\d+", "#")
来源：http://ypl.hesvh.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nrb.ppjwa.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xcl.nwbrower.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ftv.ydjk.org.cn

[I05] 按正则拆分
来源：http://jvr.quarkkingdee.top

Py:   re.split(r"\s*,\s*", s)
来源：http://yiz.ybcxt.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://num.ppjwa.cn

JS:   s.split(/\s*,\s*/)
来源：http://lec.ehwqpu.com

TS:   s.split(/\s*,\s*/)
来源：http://ebw.jinqigufen.top

Java: s.split("\\s*,\\s*")
来源：http://tca.gaohongyu789.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kny.gzhubu.top

Ruby: s.split(/\s*,\s*/)
来源：http://gqi.316326.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dxw.hcnkem.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tis.jinghuilouyu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://itj.gaohongyu789.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jva.ybcxt.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://szb.zhengqikj.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iog.uphjek.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hkg.dianchejie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://noh.hammf.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tbt.hywenlv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gtv.ppjwa.cn

[I07] 忽略大小写与多行模式
来源：http://mcn.jinghuilouyu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://euo.chenzaomai.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nbr.zhaomingkeji.xyz


<!-- 参考信息 -->