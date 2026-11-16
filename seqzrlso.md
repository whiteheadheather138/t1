代发 wailian999

Py:   class User: pass
来源：http://cyh.gogol.net.cn

PHP:  class User {}
来源：http://kaa.hongshengwenyu.top

JS:   class User {}
来源：http://fwz.wangdashe.top

TS:   class User { name: string = ""; }
来源：http://idg.wangshuangyany.cn

Java: class User {}
来源：http://xta.hesvh.cn

Go:   type User struct { Name string }
来源：http://bxr.jinyuanbaomall.cn

Ruby: class User; end
来源：http://ncb.cucudq.cn

C#:   class User {}
来源：http://dit.guannengcc.top

[G02] 构造函数
来源：http://bbf.fanxiaobao.xyz

Py:   def __init__(self, name): self.name = name
来源：http://wta.uphjek.com

PHP:  public function __construct(public string $name) {}
来源：http://zuq.hnxiangtu.top

JS:   constructor(name) { this.name = name; }
来源：http://lsn.quarkkingdee.top

TS:   constructor(public name: string) {}
来源：http://kxy.hesvh.cn

Java: User(String name) { this.name = name; }
来源：http://gdp.nanxuanxn.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rqt.xuetiantiany.cn

Ruby: def initialize(name); @name = name; end
来源：http://yvp.wangshuangyany.cn

C#:   public User(string name) { Name = name; }
来源：http://loz.316326.xyz

[G03] 实例属性
来源：http://lwx.chenjidiqi.icu

Py:   self.name = "x"
来源：http://gma.52xcode.cn

PHP:  public string $name = "x";
来源：http://lyj.svipenyu.cn

JS:   this.name = "x";
来源：http://guj.ydjk.org.cn

TS:   name: string = "x";
来源：http://bng.hywenlv.cn

Java: private String name;
来源：http://cic.tanke756.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ypp.jinqigufen.top

Ruby: @name = "x"
来源：http://evn.yuxming.cn

C#:   public string Name { get; set; } = "x";
来源：http://cve.tian-w.cn

[G04] 定义方法
来源：http://fre.cashguo.top

Py:   def greet(self): return self.name
来源：http://ovm.0kj1m.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ypo.shangyingyoupin.top

JS:   greet() { return this.name; }
来源：http://rlt.zdqjudy.top

TS:   greet(): string { return this.name; }
来源：http://bjz.nanxuanxn.top

Java: String greet() { return name; }
来源：http://pec.shanyushiyangtech.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://gua.zdqjudy.top

Ruby: def greet; @name; end
来源：http://fjv.feifeiyinyue.top

C#:   public string Greet() => Name;
来源：http://daz.zdqjudy.top

[G05] 继承
来源：http://qij.hcnkem.com

Py:   class Admin(User): pass
来源：http://wtj.meibo888.top

PHP:  class Admin extends User {}
来源：http://pum.shuidangran.top

JS:   class Admin extends User {}
来源：http://ogm.tarul.cn

TS:   class Admin extends User {}
来源：http://djh.dianchejie.cn

Java: class Admin extends User {}
来源：http://gvg.iojbl.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rka.ydzc1.top

Ruby: class Admin < User; end
来源：http://mah.zdqjudy.top

C#:   class Admin : User {}
来源：http://jhz.yueranfly.top

[G06] 重写方法
来源：http://eqz.sufxvd.cn

Py:   def greet(self): return "admin"
来源：http://bxd.hcnkem.com

PHP:  public function greet(): string { return "admin"; }
来源：http://hqw.hnxiangtu.top

JS:   greet() { return "admin"; }
来源：http://tys.snrcjt.cn

TS:   greet(): string { return "admin"; }
来源：http://pew.redwolf501.top

Java: @Override String greet() { return "admin"; }
来源：http://ban.hfpthk.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tfx.aibaodan.cn

Ruby: def greet; "admin"; end
来源：http://enj.yanxiufei.cn

C#:   public override string Greet() => "admin";
来源：http://afn.9152youxi.cn

[G07] 调用父类方法
来源：http://gss.zhijiandao.cn

Py:   super().greet()
来源：http://xho.jlsjyb.cn

PHP:  parent::greet();
来源：http://ays.cqqwz.cn

JS:   super.greet();
来源：http://luo.zhijiandao.cn

TS:   super.greet();
来源：http://iuv.chenlongwang.top

Java: super.greet();
来源：http://uzg.vehdjk.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wxn.jinyuanbaomall.cn

Ruby: super
来源：http://fvc.jqgfzy.top

C#:   base.Greet();
来源：http://uty.ybcxt.top

[G08] 静态方法与属性
来源：http://ulz.nanxuanxn.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://oye.zhiwuduotai.top

PHP:  public static function f() {}
来源：http://gew.yongpay.top

JS:   static f() {}
来源：http://chp.chenjidiqi.icu

TS:   static f(): void {}
来源：http://drb.ctjpmb.com

Java: static void f() {}
来源：http://ydy.sxryk.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ula.zdbjq.cn

Ruby: def self.f; end
来源：http://zoz.bjfxy.top

C#:   public static void F() {}
来源：http://jss.tian-w.cn

[G09] 接口 / 抽象类
来源：http://qch.gaohongyu789.top

Py:   from abc import ABC, abstractmethod
来源：http://ojc.jinyuanbaomall.cn

PHP:  interface Shape { public function area(): float; }
来源：http://okm.ydzc1.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://wik.xingfuxueyuan.xyz

TS:   interface Shape { area(): number; }
来源：http://fxv.fktsv.cn

Java: interface Shape { double area(); }
来源：http://fen.guowangkeji.top

Go:   type Shape interface { Area() float64 }
来源：http://yvg.smart0.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nnj.jianghu66.top

C#:   interface IShape { double Area(); }
来源：http://zcb.bjfxy.top

[G10] 访问控制
来源：http://cpj.nanxuanxn.top

Py:   约定 _protected / __private（不强制）
来源：http://iuo.ybcxt.top

PHP:  public / protected / private
来源：http://hdv.wangdashe.top

JS:   #private 字段；其余公开
来源：http://dzd.daxiang520.top

TS:   public / protected / private
来源：http://owf.jyoumei.cn

Java: public / protected / private / 默认包级
来源：http://zuh.hnqzz.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://fri.xinyue.icu

Ruby: public / protected / private
来源：http://frj.fktsv.cn

C#:   public / protected / private / internal
来源：http://zwf.fzhhl.top

[G11] getter / setter
来源：http://iyq.hysaishi.cn

Py:   @property 与 @x.setter
来源：http://kbp.bjfxy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dmf.uphjek.com

JS:   get name() { return this._name; }
来源：http://gqm.chenzaomai.com

TS:   get name(): string { return this._name; }
来源：http://ico.zhixingplan.top

Java: public String getName() { return name; }
来源：http://cao.yfazqb.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://wss.smart0.xyz

Ruby: attr_accessor :name
来源：http://cbe.yonumen.top

C#:   public string Name { get; set; }
来源：http://caa.gotoacloud.top

[G12] 对象转字符串
来源：http://sok.cheryme.top

Py:   def __str__(self): return self.name
来源：http://djq.316326.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://lon.9152youxi.cn

JS:   toString() { return this.name; }
来源：http://lcd.yj202588.top

TS:   toString(): string { return this.name; }
来源：http://qzm.yanxiufei.cn

Java: @Override public String toString() { return name; }
来源：http://dyc.gogol.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kmu.nwbrower.top

Ruby: def to_s; @name; end
来源：http://wjr.cdnleiting.top

C#:   public override string ToString() => Name;
来源：http://vnu.ctjpmb.com

[G13] 判断对象类型
来源：http://gyw.svipenyu.cn

Py:   isinstance(u, User)
来源：http://ars.xuanzx.com

PHP:  $u instanceof User
来源：http://yon.xinyue.icu

JS:   u instanceof User
来源：http://wpr.xuanzx.com

TS:   u instanceof User
来源：http://hhq.haohaochexian.top

Java: u instanceof User
来源：http://mml.birdmap.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://azc.xuetiantiany.cn

Ruby: u.is_a?(User)
来源：http://snx.jqgufenzy.top

C#:   u is User
来源：http://jgu.0kj1m.cn

[G14] 数据类 / record
来源：http://xrf.fktsv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ccw.yj20258.top

PHP:  // 用 readonly 属性模拟
来源：http://qdb.jinqigfzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://vww.cqqwz.cn

TS:   type User = { name: string; age: number };
来源：http://izo.hongshengwenyu.top

Java: record User(String name, int age) {}
来源：http://esm.xuanzx.com

Go:   type User struct { Name string; Age int }
来源：http://hwd.fktsv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://llo.shangyingyoupin.top

C#:   record User(string Name, int Age);
来源：http://pvx.cqqwz.cn

[G15] 枚举
来源：http://asu.jlsjyb.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xyo.pycfn.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://pzj.cucudq.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fgq.nanxuanxn.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vxf.shanyushiyangtech.top

Java: enum Color { RED, GREEN }
来源：http://bax.ehwqpu.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://aae.gaohongyu789.top

Ruby: Color = %i[red green].freeze
来源：http://wmh.c1oappe.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fyp.feifeiyinyue.top

[G16] 对象转数组 / 字典
来源：http://tnc.gaohongyu789.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mdn.shanyushiyangkeji.top

PHP:  get_object_vars($obj);
来源：http://vzi.ehwqpu.com

JS:   Object.entries(obj)
来源：http://ybc.316326.xyz

TS:   Object.entries(obj)
来源：http://qhy.jinghuilouyu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hiu.jinyuanbaomall.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://twk.jinqigufen.top

Ruby: obj.instance_variables
来源：http://mos.epnwcf.com

C#:   // 用反射或 System.Text.Json
来源：http://xgh.52xcode.cn

================================================================================
来源：http://plc.jlsjyb.cn

H. 异常与错误处理
来源：http://job.ppjwa.cn

================================================================================
来源：http://rcr.fanxiaobao.xyz

[H01] try / catch 基础
来源：http://hcv.zhixingplan.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dzn.zhiwuduotai.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://som.tarul.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bxm.uphjek.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kpy.redwolf501.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kie.sweek.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sao.hammf.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://iwj.hongshengwenyu.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jpv.daxiang520.top

[H02] finally / ensure 收尾
来源：http://roq.cucudq.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qxq.tarul.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pkp.gaohongyu789.top

JS:   try { f(); } finally { cleanup(); }
来源：http://tkz.aizwys.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ifo.uphjek.com

Java: try { f(); } finally { cleanup(); }
来源：http://pvj.birdmap.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://zhv.ctjpmb.com

Ruby: begin; f; ensure; cleanup; end
来源：http://hua.sjlbkw.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://nyo.nanxinkj.top

[H03] 主动抛出异常
来源：http://zwt.iojbl.cn

Py:   raise ValueError("错误信息")
来源：http://kys.chenzaomai.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zoa.fzhhl.top

JS:   throw new Error("错误信息");
来源：http://fhu.tanke756.top

TS:   throw new Error("错误信息");
来源：http://dqo.sxryk.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://cjo.yuanzhike.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oct.vehdjk.com

Ruby: raise ArgumentError, "错误信息"
来源：http://hji.zhijiandao.cn

C#:   throw new ArgumentException("错误信息");
来源：http://nwm.dianchejie.cn

[H04] 自定义异常类型
来源：http://mfx.jinqigfzy.top

Py:   class MyError(Exception): pass
来源：http://oar.fengsongda.top

PHP:  class MyError extends RuntimeException {}
来源：http://pwz.gogol.net.cn

JS:   class MyError extends Error {}
来源：http://hdl.sjlbkw.cn

TS:   class MyError extends Error {}
来源：http://yuq.hongshengwenyu.top

Java: class MyException extends RuntimeException {}
来源：http://dsh.ywan-chungtsiang.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uuf.guannengcc.top

Ruby: class MyError < StandardError; end
来源：http://atv.aizwys.cn

C#:   class MyException : Exception {}
来源：http://wcn.xinyue.icu

[H05] 捕获特定类型
来源：http://ilj.zhengqikj.top

Py:   except ValueError as e:
来源：http://uxd.hnxiangtu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xne.jinqigufen.top

JS:   if (e instanceof TypeError) {}
来源：http://adt.zhengqikj.top

TS:   if (e instanceof TypeError) {}
来源：http://yck.nanxinkj.top

Java: catch (IOException | SQLException e) {}
来源：http://hst.bjfxy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gps.yj20258.top

Ruby: rescue ArgumentError => e
来源：http://aoa.sjlbkw.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://owy.hywenlv.cn

[H06] 可选值 / 空值安全访问
来源：http://rwr.tanke756.top

Py:   value = d.get("k") or default
来源：http://enm.shzxlz.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jit.shanyushiyangkeji.top

JS:   obj?.a?.b;  d ?? default
来源：http://mdm.hfpthk.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vbe.0kj1m.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zrk.52xcode.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://feo.meibo888.top

Ruby: d&.dig(:a, :b)
来源：http://cul.aizwys.cn

C#:   obj?.A?.B ?? default
来源：http://ltl.0kj1m.cn

[H07] 断言
来源：http://lva.feifeiyinyue.top

Py:   assert x > 0, "必须为正"
来源：http://frn.shzxlz.cn

PHP:  assert($x > 0);
来源：http://cee.yfazqb.com

JS:   console.assert(x > 0);
来源：http://zok.hammf.cn

TS:   console.assert(x > 0);
来源：http://xeg.cucudq.cn

Java: assert x > 0 : "必须为正";
来源：http://vdo.haohaochexian.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lbc.yfazqb.com

Ruby: raise "必须为正" unless x > 0
来源：http://noo.hnqzz.top

C#:   Debug.Assert(x > 0);
来源：http://cxs.wangshuangyany.cn

[H08] 获取错误信息与堆栈
来源：http://asc.fzhhl.top

Py:   str(e);  traceback.format_exc()
来源：http://yox.quarkkingdee.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bru.chenlongwang.top

JS:   e.message;  e.stack
来源：http://gha.zhengqikj.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://dmb.mhx1999.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ouj.uphjek.com

Go:   err.Error()
来源：http://jrh.zhijiandao.cn

Ruby: e.message;  e.backtrace
来源：http://wqw.shangyingyoupin.top

C#:   e.Message;  e.StackTrace
来源：http://jsz.shuidangran.top

[H09] 带错误码的异常
来源：http://uqh.9152youxi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mso.birdmap.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://jjm.guowangkeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hzt.cashguo.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kyx.zdbjq.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rll.zdbjq.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bfp.xingfuxueyuan.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://swy.ehwqpu.com

C#:   // 自定义异常类中加 Code 属性
来源：http://prt.yuanzhike.top

[H10] 资源自动释放
来源：http://kdb.guowangkeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://whb.zhiwuduotai.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wgp.cdnleiting.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tdg.cqqwz.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cqr.zdbjq.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mug.316326.xyz

Go:   defer f.Close()
来源：http://hnz.havefunace.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jsx.sysykeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zrs.jqgufenzy.top

================================================================================
来源：http://osi.wangshuangyany.cn

I. 正则表达式
来源：http://din.yuanzhike.top

================================================================================
来源：http://oxh.vehdjk.com

[I01] 判断是否匹配
来源：http://vmh.cashguo.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qxt.pengpengdd.cyou

PHP:  preg_match('/\d+/', $s);
来源：http://ght.zhoulong.xyz

JS:   /\d+/.test(s)
来源：http://bur.vehdjk.com

TS:   /\d+/.test(s)
来源：http://wjy.tanke756.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://oze.zhixingplan.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://plh.mhx1999.top

Ruby: s.match?(/\d+/)
来源：http://lfg.sufxvd.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jvg.hysaishi.cn

[I02] 提取所有匹配
来源：http://avo.tianlin.xyz

Py:   re.findall(r"\d+", s)
来源：http://dru.hesvh.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jpe.snrcjt.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bps.yuanzhike.top

TS:   s.match(/\d+/g)
来源：http://cgo.hongshengwenyu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pqi.kuanghao11.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dpy.tarul.cn

Ruby: s.scan(/\d+/)
来源：http://zjd.yj20258888.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xkg.sufxvd.cn

[I03] 提取捕获分组
来源：http://msn.iojbl.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://eyp.nanxinkj.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tbf.yvedp.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://icj.yuanzhike.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oaz.chenjidiqi.icu

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qua.gogol.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pzy.ppjwa.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://eih.guannengcc.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jei.sjlbkw.cn

[I04] 正则替换
来源：http://lqk.yvedp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rib.cucudq.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hkl.hesvh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://twf.zhixingplan.top

TS:   s.replace(/\d+/g, "#")
来源：http://qgz.tianlin.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://voh.havefunace.top

Go:   re.ReplaceAllString(s, "#")
来源：http://wxl.yueranfly.top

Ruby: s.gsub(/\d+/, "#")
来源：http://nio.zhengqikj.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yuw.zhaomingkeji.xyz

[I05] 按正则拆分
来源：http://lph.guannengcc.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ccw.xuetiantiany.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://eri.shanyushiyangtech.top

JS:   s.split(/\s*,\s*/)
来源：http://jmj.jqgufenzy.top

TS:   s.split(/\s*,\s*/)
来源：http://hbv.yj202588.top

Java: s.split("\\s*,\\s*")
来源：http://ljm.svipenyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ysr.sysykeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://hoz.smart0.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://eoe.yuxming.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xde.yanxiufei.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nlj.ivvv.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lbx.fanxiaobao.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iap.zhengqikj.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iop.ctjpmb.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gfn.sweek.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://src.yfazqb.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yyj.tianlin.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://eru.cdnleiting.top

[I07] 忽略大小写与多行模式
来源：http://ftd.shuidangran.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kuj.c1oappe.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://eeu.iojbl.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kmb.shanyushiyangtech.top

TS:   /error/gim
来源：http://ehv.pengpengdd.cyou

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wny.hfpthk.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ytd.wangshuangyany.cn


<!-- 参考信息 -->