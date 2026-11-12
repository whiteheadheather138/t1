代发 wailian999

Java: class User {}
来源：http://alf.cucudq.cn

Go:   type User struct { Name string }
来源：http://dly.kuanghao11.cn

Ruby: class User; end
来源：http://lqd.fehbvm.com

C#:   class User {}
来源：http://hkz.yonumen.top

[G02] 构造函数
来源：http://whn.hesvh.cn

Py:   def __init__(self, name): self.name = name
来源：http://qom.316326.xyz

PHP:  public function __construct(public string $name) {}
来源：http://bqw.tian-w.cn

JS:   constructor(name) { this.name = name; }
来源：http://dbb.bjfxy.top

TS:   constructor(public name: string) {}
来源：http://pvn.meibo888.top

Java: User(String name) { this.name = name; }
来源：http://jjy.cashguo.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://roa.bjfxy.top

Ruby: def initialize(name); @name = name; end
来源：http://pxc.pycfn.com

C#:   public User(string name) { Name = name; }
来源：http://apb.aibaodan.cn

[G03] 实例属性
来源：http://hfg.wangshuangyany.cn

Py:   self.name = "x"
来源：http://pba.xingfuxueyuan.xyz

PHP:  public string $name = "x";
来源：http://fjb.gzhubu.top

JS:   this.name = "x";
来源：http://xbr.fehbvm.com

TS:   name: string = "x";
来源：http://gka.chenjidiqi.icu

Java: private String name;
来源：http://mvp.pengpengdd.cyou

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nof.shangyingyoupin.top

Ruby: @name = "x"
来源：http://wtv.tanke756.top

C#:   public string Name { get; set; } = "x";
来源：http://nex.meibo888.top

[G04] 定义方法
来源：http://hqi.feifeiyinyue.top

Py:   def greet(self): return self.name
来源：http://pra.shzxlz.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ksq.tian-w.cn

JS:   greet() { return this.name; }
来源：http://fxl.chenjidiqi.icu

TS:   greet(): string { return this.name; }
来源：http://eac.yvedp.cn

Java: String greet() { return name; }
来源：http://hly.jinqigufen.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://qpi.nwbrower.top

Ruby: def greet; @name; end
来源：http://qvt.jqgufenzy.top

C#:   public string Greet() => Name;
来源：http://ujd.fzhhl.top

[G05] 继承
来源：http://dpa.jyoumei.cn

Py:   class Admin(User): pass
来源：http://pfv.sysykeji.top

PHP:  class Admin extends User {}
来源：http://eot.bjfxy.top

JS:   class Admin extends User {}
来源：http://xvj.haohaochexian.top

TS:   class Admin extends User {}
来源：http://imo.jinyuanbaomall.cn

Java: class Admin extends User {}
来源：http://aos.hammf.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xzz.wangdashe.top

Ruby: class Admin < User; end
来源：http://cjg.ybcxt.top

C#:   class Admin : User {}
来源：http://dow.ywan-chungtsiang.top

[G06] 重写方法
来源：http://xzb.ehwqpu.com

Py:   def greet(self): return "admin"
来源：http://afv.hcnkem.com

PHP:  public function greet(): string { return "admin"; }
来源：http://wzu.jyoumei.cn

JS:   greet() { return "admin"; }
来源：http://lse.ywan-chungtsiang.top

TS:   greet(): string { return "admin"; }
来源：http://abk.tianlin.xyz

Java: @Override String greet() { return "admin"; }
来源：http://wur.shanyushiyangkeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://plh.zhijiandao.cn

Ruby: def greet; "admin"; end
来源：http://hqu.jiagoushi.top

C#:   public override string Greet() => "admin";
来源：http://kqt.sufxvd.cn

[G07] 调用父类方法
来源：http://oqd.jyoumei.cn

Py:   super().greet()
来源：http://iby.jqgufenzy.top

PHP:  parent::greet();
来源：http://mnf.ydzc1.top

JS:   super.greet();
来源：http://bck.xziqi.cn

TS:   super.greet();
来源：http://xvc.hysaishi.cn

Java: super.greet();
来源：http://qqt.mhx1999.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yof.iojbl.cn

Ruby: super
来源：http://jxa.zhongyouzk.top

C#:   base.Greet();
来源：http://kjk.cashguo.top

[G08] 静态方法与属性
来源：http://sue.sjlbkw.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yjp.shanyushiyangtech.top

PHP:  public static function f() {}
来源：http://ovm.yonumen.top

JS:   static f() {}
来源：http://ygv.xuetiantiany.cn

TS:   static f(): void {}
来源：http://jbn.hongshengwenyu.top

Java: static void f() {}
来源：http://wre.yfazqb.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://vwm.gogol.net.cn

Ruby: def self.f; end
来源：http://srr.tian-w.cn

C#:   public static void F() {}
来源：http://epm.tanke756.top

[G09] 接口 / 抽象类
来源：http://ooe.yongpay.top

Py:   from abc import ABC, abstractmethod
来源：http://lay.zdqjudy.top

PHP:  interface Shape { public function area(): float; }
来源：http://pjq.sxryk.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://gsq.jyoumei.cn

TS:   interface Shape { area(): number; }
来源：http://puc.uphjek.com

Java: interface Shape { double area(); }
来源：http://jjq.jinyuanbaomall.cn

Go:   type Shape interface { Area() float64 }
来源：http://kob.zdbjq.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://huo.hnxiangtu.top

C#:   interface IShape { double Area(); }
来源：http://wpn.daxiang520.top

[G10] 访问控制
来源：http://wda.316326.xyz

Py:   约定 _protected / __private（不强制）
来源：http://dey.dianchejie.cn

PHP:  public / protected / private
来源：http://bwq.yanxiufei.cn

JS:   #private 字段；其余公开
来源：http://mqh.sysykeji.top

TS:   public / protected / private
来源：http://oka.xuanzx.com

Java: public / protected / private / 默认包级
来源：http://gki.guowangkeji.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://dce.316326.xyz

Ruby: public / protected / private
来源：http://wcy.haohaochexian.top

C#:   public / protected / private / internal
来源：http://drv.quarkkingdee.top

[G11] getter / setter
来源：http://vqi.ivvv.top

Py:   @property 与 @x.setter
来源：http://wpd.cashguo.top

PHP:  public function getName(): string { return $this->name; }
来源：http://abb.zhiwuduotai.top

JS:   get name() { return this._name; }
来源：http://hec.cashguo.top

TS:   get name(): string { return this._name; }
来源：http://zgk.shzxlz.cn

Java: public String getName() { return name; }
来源：http://lnw.zhiwuduotai.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://uyg.hnqzz.top

Ruby: attr_accessor :name
来源：http://vez.nanxinkj.top

C#:   public string Name { get; set; }
来源：http://aop.ywan-chungtsiang.top

[G12] 对象转字符串
来源：http://mkv.shangyingyoupin.top

Py:   def __str__(self): return self.name
来源：http://lqc.52xcode.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://tbb.jinyuanbaomall.cn

JS:   toString() { return this.name; }
来源：http://hjr.zhengqikj.top

TS:   toString(): string { return this.name; }
来源：http://gec.yuanzhike.top

Java: @Override public String toString() { return name; }
来源：http://qmt.zhongyouzk.top

Go:   func (u User) String() string { return u.Name }
来源：http://rta.tanke756.top

Ruby: def to_s; @name; end
来源：http://iza.wangshuangyany.cn

C#:   public override string ToString() => Name;
来源：http://psa.gogol.net.cn

[G13] 判断对象类型
来源：http://ylm.jinyuanbaomall.cn

Py:   isinstance(u, User)
来源：http://lmq.mhx1999.top

PHP:  $u instanceof User
来源：http://pbj.0kj1m.cn

JS:   u instanceof User
来源：http://ugt.havefunace.top

TS:   u instanceof User
来源：http://rjj.gotoacloud.top

Java: u instanceof User
来源：http://vol.xinyue.icu

Go:   u, ok := v.(User)            // 类型断言
来源：http://gyw.zhoulong.xyz

Ruby: u.is_a?(User)
来源：http://ujm.uphjek.com

C#:   u is User
来源：http://clq.fehbvm.com

[G14] 数据类 / record
来源：http://fxx.wangdashe.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nya.shanyushiyangkeji.top

PHP:  // 用 readonly 属性模拟
来源：http://nlk.shanyushiyangtech.top

JS:   // 无内置：普通类或对象字面量
来源：http://dqs.chenjidiqi.icu

TS:   type User = { name: string; age: number };
来源：http://ezq.zhengqikj.top

Java: record User(String name, int age) {}
来源：http://ptr.yuxming.cn

Go:   type User struct { Name string; Age int }
来源：http://goe.havefunace.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gjq.ywan-chungtsiang.top

C#:   record User(string Name, int Age);
来源：http://foh.ywan-chungtsiang.top

[G15] 枚举
来源：http://uxa.wangdashe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fof.ybcxt.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://usq.hesvh.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://prm.hnxiangtu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://boz.shuidangran.top

Java: enum Color { RED, GREEN }
来源：http://vek.xinyue.icu

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jwx.jinghuilouyu.cn

Ruby: Color = %i[red green].freeze
来源：http://fvt.fktsv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://byl.316326.xyz

[G16] 对象转数组 / 字典
来源：http://kai.9152youxi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hmu.sysykeji.top

PHP:  get_object_vars($obj);
来源：http://ptl.xziqi.cn

JS:   Object.entries(obj)
来源：http://dkf.guannengcc.top

TS:   Object.entries(obj)
来源：http://ulf.yuxming.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://oyi.guowangkeji.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ijh.fktsv.cn

Ruby: obj.instance_variables
来源：http://hra.hammf.cn

C#:   // 用反射或 System.Text.Json
来源：http://gpg.hongshengwenyu.top

================================================================================
来源：http://nrl.zhengqikj.top

H. 异常与错误处理
来源：http://bbs.uphjek.com

================================================================================
来源：http://slt.iojbl.cn

[H01] try / catch 基础
来源：http://gkn.quarkkingdee.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xbv.zdqjudy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xcy.ctjpmb.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jmv.ctjpmb.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bwp.cqqwz.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kps.chenjidiqi.icu

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hlx.dianchejie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mdk.yj20258.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://glx.havefunace.top

[H02] finally / ensure 收尾
来源：http://ikq.fktsv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vee.ivvv.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://uzl.hywenlv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ecz.yanxiufei.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://odj.cucudq.cn

Java: try { f(); } finally { cleanup(); }
来源：http://sxi.jianghu66.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://vyi.fehbvm.com

Ruby: begin; f; ensure; cleanup; end
来源：http://kik.bjfxy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://cwl.yuxming.cn

[H03] 主动抛出异常
来源：http://npt.wangshuangyany.cn

Py:   raise ValueError("错误信息")
来源：http://bbm.xuetiantiany.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://djd.chenzaomai.com

JS:   throw new Error("错误信息");
来源：http://frz.316326.xyz

TS:   throw new Error("错误信息");
来源：http://oep.ctjpmb.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://flj.gzhubu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xjp.hnqzz.top

Ruby: raise ArgumentError, "错误信息"
来源：http://rjy.birdmap.top

C#:   throw new ArgumentException("错误信息");
来源：http://pjk.chenzaomai.com

[H04] 自定义异常类型
来源：http://vgu.jianghu66.top

Py:   class MyError(Exception): pass
来源：http://nuu.tarul.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pbl.jqgufenzy.top

JS:   class MyError extends Error {}
来源：http://rgx.nanxuanxn.top

TS:   class MyError extends Error {}
来源：http://klm.chenzaomai.com

Java: class MyException extends RuntimeException {}
来源：http://tas.fengsongda.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://aqh.tian-w.cn

Ruby: class MyError < StandardError; end
来源：http://bge.kuanghao11.cn

C#:   class MyException : Exception {}
来源：http://upi.vqdsnc.cn

[H05] 捕获特定类型
来源：http://www.bbcook.cn

Py:   except ValueError as e:
来源：http://zje.shanyushiyangtech.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://voa.shangyingyoupin.top

JS:   if (e instanceof TypeError) {}
来源：http://kvx.chenlongwang.top

TS:   if (e instanceof TypeError) {}
来源：http://gah.cheryme.top

Java: catch (IOException | SQLException e) {}
来源：http://jsp.hysaishi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xyk.yueranfly.top

Ruby: rescue ArgumentError => e
来源：http://eaw.sysykeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ytj.zhengqikj.top

[H06] 可选值 / 空值安全访问
来源：http://ikn.yonumen.top

Py:   value = d.get("k") or default
来源：http://yyf.yj20258.top

PHP:  $v = $d["k"] ?? null;
来源：http://plk.ydzc1.top

JS:   obj?.a?.b;  d ?? default
来源：http://nbe.fanxiaobao.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://ahe.zdqjudy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vhx.tanke756.top

Go:   if v, ok := m["k"]; ok { }
来源：http://jse.cashguo.top

Ruby: d&.dig(:a, :b)
来源：http://pzu.fengsongda.top

C#:   obj?.A?.B ?? default
来源：http://dmq.yfazqb.com

[H07] 断言
来源：http://jwm.zhijiandao.cn

Py:   assert x > 0, "必须为正"
来源：http://gio.snrcjt.cn

PHP:  assert($x > 0);
来源：http://zoy.jqgufenzy.top

JS:   console.assert(x > 0);
来源：http://kyr.cqqwz.cn

TS:   console.assert(x > 0);
来源：http://hbj.tanke756.top

Java: assert x > 0 : "必须为正";
来源：http://woj.9152youxi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uwt.pycfn.com

Ruby: raise "必须为正" unless x > 0
来源：http://ydp.316326.xyz

C#:   Debug.Assert(x > 0);
来源：http://kcp.daxiang520.top

[H08] 获取错误信息与堆栈
来源：http://oau.daxiang520.top

Py:   str(e);  traceback.format_exc()
来源：http://xfe.hfpthk.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://alo.jinqigfzy.top

JS:   e.message;  e.stack
来源：http://wkn.ybcxt.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ksm.hywenlv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://yap.sysykeji.top

Go:   err.Error()
来源：http://ojo.gogol.net.cn

Ruby: e.message;  e.backtrace
来源：http://aqb.aizwys.cn

C#:   e.Message;  e.StackTrace
来源：http://gwh.gaohongyu789.top

[H09] 带错误码的异常
来源：http://soo.meibo888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jgw.yonumen.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://pub.shangyingyoupin.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wjh.gaohongyu789.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ydz.smart0.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xxv.gaohongyu789.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kqb.hammf.cn

Ruby: raise MyError.new("fail", 500)
来源：http://cvk.xziqi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://kpa.kuanghao11.cn

[H10] 资源自动释放
来源：http://dee.snrcjt.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://dqg.jyoumei.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bmc.cucudq.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xbo.zhijiandao.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qca.hesvh.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kra.chenjidiqi.icu

Go:   defer f.Close()
来源：http://ivh.hesvh.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mnk.xylfe.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://idh.birdmap.top

================================================================================
来源：http://yph.daxiang520.top

I. 正则表达式
来源：http://brr.52xcode.cn

================================================================================
来源：http://adr.shanyushiyangkeji.top

[I01] 判断是否匹配
来源：http://vgh.ehwqpu.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hwp.316326.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://zdc.shangyingyoupin.top

JS:   /\d+/.test(s)
来源：http://mrh.sweek.top

TS:   /\d+/.test(s)
来源：http://luc.yj20258.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kaq.xinyue.icu

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jed.tanke756.top

Ruby: s.match?(/\d+/)
来源：http://eva.yuxming.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hhe.zhengqikj.top

[I02] 提取所有匹配
来源：http://lme.sjlbkw.cn

Py:   re.findall(r"\d+", s)
来源：http://akj.316326.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bhu.zhongyouzk.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ozy.jiagoushi.top

TS:   s.match(/\d+/g)
来源：http://ega.ehwqpu.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rpl.tarul.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://equ.c1oappe.top

Ruby: s.scan(/\d+/)
来源：http://pdu.svipenyu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://has.52xcode.cn

[I03] 提取捕获分组
来源：http://uex.0kj1m.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bkg.redwolf501.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cef.fengsongda.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://iic.gzhubu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uwo.zhixingplan.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lqj.yj20258888.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nsm.ivvv.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zbv.dianchejie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oia.sysykeji.top

[I04] 正则替换
来源：http://nhh.yueranfly.top

Py:   re.sub(r"\d+", "#", s)
来源：http://fuk.yj20258888.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://brq.shzxlz.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dfb.guowangkeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://kru.quarkkingdee.top

Java: s.replaceAll("\\d+", "#")
来源：http://ugl.epnwcf.com

Go:   re.ReplaceAllString(s, "#")
来源：http://gdr.sweek.top

Ruby: s.gsub(/\d+/, "#")
来源：http://sjj.cashguo.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ejb.hongshengwenyu.top

[I05] 按正则拆分
来源：http://wgj.zdbjq.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://lfp.xylfe.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://adl.ydzc1.top

JS:   s.split(/\s*,\s*/)
来源：http://vpw.0kj1m.cn

TS:   s.split(/\s*,\s*/)
来源：http://yar.tanke756.top

Java: s.split("\\s*,\\s*")
来源：http://ejc.chenlongwang.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://meu.fzhhl.top

Ruby: s.split(/\s*,\s*/)
来源：http://gli.nanxinkj.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mjq.yj20258888.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zjc.wangshuangyany.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wzd.gotoacloud.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ten.epnwcf.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zun.havefunace.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://snt.yonumen.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hmm.chenzaomai.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://huz.sysykeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bmh.gotoacloud.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lhm.jinghuilouyu.cn

[I07] 忽略大小写与多行模式
来源：http://bzb.xziqi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nbj.feifeiyinyue.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dxa.shzxlz.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nio.nanxuanxn.top

TS:   /error/gim
来源：http://hmk.xinyue.icu

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dby.sufxvd.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rkm.jqgufenzy.top

Ruby: s.scan(/error/i)
来源：http://ket.jinqigfzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://frq.sweek.top

[I08] 贪婪与非贪婪匹配
来源：http://qbq.fehbvm.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nbn.yj202588.top


<!-- 参考信息 -->