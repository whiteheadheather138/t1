代发 wailian999

[G02] 构造函数
来源：http://fgo.sjlbkw.cn

Py:   def __init__(self, name): self.name = name
来源：http://rbz.vqdsnc.cn

PHP:  public function __construct(public string $name) {}
来源：http://iuw.gogol.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://xeb.gzhubu.top

TS:   constructor(public name: string) {}
来源：http://xtz.yonumen.top

Java: User(String name) { this.name = name; }
来源：http://ixf.nanxuanxn.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zcc.havefunace.top

Ruby: def initialize(name); @name = name; end
来源：http://jrn.jqgfzy.top

C#:   public User(string name) { Name = name; }
来源：http://lwu.zdbjq.cn

[G03] 实例属性
来源：http://dvb.sweek.top

Py:   self.name = "x"
来源：http://ulf.zhixingplan.top

PHP:  public string $name = "x";
来源：http://xhi.zycfv.cn

JS:   this.name = "x";
来源：http://thc.chenlongwang.top

TS:   name: string = "x";
来源：http://ekd.sjlbkw.cn

Java: private String name;
来源：http://tbv.sjlbkw.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fgy.haohaochexian.top

Ruby: @name = "x"
来源：http://lvs.zhijiandao.cn

C#:   public string Name { get; set; } = "x";
来源：http://mnz.shanyushiyangkeji.top

[G04] 定义方法
来源：http://jpk.dianchejie.cn

Py:   def greet(self): return self.name
来源：http://dxa.zdqjudy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://tsm.nwbrower.top

JS:   greet() { return this.name; }
来源：http://utt.yj202588.top

TS:   greet(): string { return this.name; }
来源：http://flg.hnqzz.top

Java: String greet() { return name; }
来源：http://wsv.yanxiufei.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://puv.shuidangran.top

Ruby: def greet; @name; end
来源：http://why.guannengcc.top

C#:   public string Greet() => Name;
来源：http://zlh.yuxming.cn

[G05] 继承
来源：http://imb.zdbjq.cn

Py:   class Admin(User): pass
来源：http://muw.hnxiangtu.top

PHP:  class Admin extends User {}
来源：http://fkw.hnxiangtu.top

JS:   class Admin extends User {}
来源：http://agh.jyoumei.cn

TS:   class Admin extends User {}
来源：http://ppo.yongpay.top

Java: class Admin extends User {}
来源：http://mrt.vqdsnc.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hfv.kuanghao11.cn

Ruby: class Admin < User; end
来源：http://dpg.chenjidiqi.icu

C#:   class Admin : User {}
来源：http://wco.smart0.xyz

[G06] 重写方法
来源：http://vhh.yj20258.top

Py:   def greet(self): return "admin"
来源：http://gnt.ivvv.top

PHP:  public function greet(): string { return "admin"; }
来源：http://fwn.daxiang520.top

JS:   greet() { return "admin"; }
来源：http://ijj.zhongyouzk.top

TS:   greet(): string { return "admin"; }
来源：http://okz.fanxiaobao.xyz

Java: @Override String greet() { return "admin"; }
来源：http://sjq.fktsv.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lyo.tanke756.top

Ruby: def greet; "admin"; end
来源：http://lqo.cucudq.cn

C#:   public override string Greet() => "admin";
来源：http://gub.hcnkem.com

[G07] 调用父类方法
来源：http://wux.zhixingplan.top

Py:   super().greet()
来源：http://gmb.hcnkem.com

PHP:  parent::greet();
来源：http://yqi.yfazqb.com

JS:   super.greet();
来源：http://tru.yuxming.cn

TS:   super.greet();
来源：http://ovk.yuanzhike.top

Java: super.greet();
来源：http://vjy.jinqigufen.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kvc.fehbvm.com

Ruby: super
来源：http://rwq.jyoumei.cn

C#:   base.Greet();
来源：http://lpa.zdbjq.cn

[G08] 静态方法与属性
来源：http://jez.cqqwz.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ptr.xuetiantiany.cn

PHP:  public static function f() {}
来源：http://qme.shuidangran.top

JS:   static f() {}
来源：http://evv.yfazqb.com

TS:   static f(): void {}
来源：http://ncz.316326.xyz

Java: static void f() {}
来源：http://pqt.tanke756.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://moj.wangdashe.top

Ruby: def self.f; end
来源：http://ftx.yanxiufei.cn

C#:   public static void F() {}
来源：http://loz.xuanzx.com

[G09] 接口 / 抽象类
来源：http://fzg.xinyue.icu

Py:   from abc import ABC, abstractmethod
来源：http://lrz.yuanzhike.top

PHP:  interface Shape { public function area(): float; }
来源：http://ddx.ctjpmb.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://dmr.cucudq.cn

TS:   interface Shape { area(): number; }
来源：http://kkm.gaohongyu789.top

Java: interface Shape { double area(); }
来源：http://xfo.daxiang520.top

Go:   type Shape interface { Area() float64 }
来源：http://ery.jianghu66.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jan.yj20258888.top

C#:   interface IShape { double Area(); }
来源：http://mkx.dianchejie.cn

[G10] 访问控制
来源：http://xak.redwolf501.top

Py:   约定 _protected / __private（不强制）
来源：http://pym.ywan-chungtsiang.top

PHP:  public / protected / private
来源：http://fwd.zhongyouzk.top

JS:   #private 字段；其余公开
来源：http://vgc.sxryk.cn

TS:   public / protected / private
来源：http://wdp.sweek.top

Java: public / protected / private / 默认包级
来源：http://orj.hnqzz.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://foy.meibo888.top

Ruby: public / protected / private
来源：http://pvw.wangdashe.top

C#:   public / protected / private / internal
来源：http://oze.cqqwz.cn

[G11] getter / setter
来源：http://yhs.yueranfly.top

Py:   @property 与 @x.setter
来源：http://skl.gaohongyu789.top

PHP:  public function getName(): string { return $this->name; }
来源：http://vjq.iojbl.cn

JS:   get name() { return this._name; }
来源：http://xkx.fanxiaobao.xyz

TS:   get name(): string { return this._name; }
来源：http://umz.jinghuilouyu.cn

Java: public String getName() { return name; }
来源：http://fmm.ppjwa.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yzh.ydzc1.top

Ruby: attr_accessor :name
来源：http://smj.jinghuilouyu.cn

C#:   public string Name { get; set; }
来源：http://dbo.jinqigufen.top

[G12] 对象转字符串
来源：http://taz.cqqwz.cn

Py:   def __str__(self): return self.name
来源：http://cod.zhiwuduotai.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://kno.fzhhl.top

JS:   toString() { return this.name; }
来源：http://huu.mhx1999.top

TS:   toString(): string { return this.name; }
来源：http://mhv.cashguo.top

Java: @Override public String toString() { return name; }
来源：http://uns.shanyushiyangkeji.top

Go:   func (u User) String() string { return u.Name }
来源：http://uju.fktsv.cn

Ruby: def to_s; @name; end
来源：http://wbj.snrcjt.cn

C#:   public override string ToString() => Name;
来源：http://ipc.svipenyu.cn

[G13] 判断对象类型
来源：http://uyx.ctjpmb.com

Py:   isinstance(u, User)
来源：http://pdg.hysaishi.cn

PHP:  $u instanceof User
来源：http://vnx.jqgufenzy.top

JS:   u instanceof User
来源：http://dci.chenlongwang.top

TS:   u instanceof User
来源：http://zrc.ywan-chungtsiang.top

Java: u instanceof User
来源：http://kwj.yvedp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://lwe.pycfn.com

Ruby: u.is_a?(User)
来源：http://sdh.jinyuanbaomall.cn

C#:   u is User
来源：http://slq.wangshuangyany.cn

[G14] 数据类 / record
来源：http://ndl.nwbrower.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zgw.jinyuanbaomall.cn

PHP:  // 用 readonly 属性模拟
来源：http://bnf.hywenlv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://afk.hfpthk.cn

TS:   type User = { name: string; age: number };
来源：http://spe.316326.xyz

Java: record User(String name, int age) {}
来源：http://svj.sufxvd.cn

Go:   type User struct { Name string; Age int }
来源：http://wuk.zhengqikj.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rri.tanke756.top

C#:   record User(string Name, int Age);
来源：http://ltx.cdnleiting.top

[G15] 枚举
来源：http://yll.tianlin.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sju.daxiang520.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://one.yj20258.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://trb.yj20258888.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vqw.hfpthk.cn

Java: enum Color { RED, GREEN }
来源：http://blt.cheryme.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uai.meibo888.top

Ruby: Color = %i[red green].freeze
来源：http://vko.chenlongwang.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cqb.wangshuangyany.cn

[G16] 对象转数组 / 字典
来源：http://qcn.ywan-chungtsiang.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mps.xinyue.icu

PHP:  get_object_vars($obj);
来源：http://ipm.cdnleiting.top

JS:   Object.entries(obj)
来源：http://rid.nanxinkj.top

TS:   Object.entries(obj)
来源：http://kvr.pengpengdd.cyou

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rsw.yangfankeji.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://hcs.tianlin.xyz

Ruby: obj.instance_variables
来源：http://bde.cheryme.top

C#:   // 用反射或 System.Text.Json
来源：http://bqq.xinyue.icu

================================================================================
来源：http://tgp.zhijiandao.cn

H. 异常与错误处理
来源：http://kxs.hnqzz.top

================================================================================
来源：http://plq.yanxiufei.cn

[H01] try / catch 基础
来源：http://cqa.dashuyun.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jvu.redwolf501.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yow.gaohongyu789.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xnc.dianchejie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://plx.tanke756.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dqk.redwolf501.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://agx.nanxinkj.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rrh.yuanzhike.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qyx.pycfn.com

[H02] finally / ensure 收尾
来源：http://app.fanxiaobao.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://yuk.ivvv.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://pjs.hammf.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rkt.cdnleiting.top

TS:   try { f(); } finally { cleanup(); }
来源：http://adg.svipenyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://nwl.cashguo.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://hpl.fktsv.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jjh.hfpthk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cfw.zhaomingkeji.xyz

[H03] 主动抛出异常
来源：http://xfo.zhijiandao.cn

Py:   raise ValueError("错误信息")
来源：http://ikt.zycfv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ggd.jinghuilouyu.cn

JS:   throw new Error("错误信息");
来源：http://yik.gaohongyu789.top

TS:   throw new Error("错误信息");
来源：http://lop.feifeiyinyue.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://wro.jianghu66.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vqz.guowangkeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://tis.tianlin.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://dbp.tianlin.xyz

[H04] 自定义异常类型
来源：http://sns.tianlin.xyz

Py:   class MyError(Exception): pass
来源：http://hac.aibaodan.cn

PHP:  class MyError extends RuntimeException {}
来源：http://uft.bbcook.cn

JS:   class MyError extends Error {}
来源：http://wiq.aizwys.cn

TS:   class MyError extends Error {}
来源：http://bqx.dianchejie.cn

Java: class MyException extends RuntimeException {}
来源：http://ovd.hnxiangtu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ocx.fehbvm.com

Ruby: class MyError < StandardError; end
来源：http://mhp.iojbl.cn

C#:   class MyException : Exception {}
来源：http://lqi.ybcxt.top

[H05] 捕获特定类型
来源：http://ptk.guowangkeji.top

Py:   except ValueError as e:
来源：http://csw.yvedp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://edh.zhixingplan.top

JS:   if (e instanceof TypeError) {}
来源：http://rax.jinyuanbaomall.cn

TS:   if (e instanceof TypeError) {}
来源：http://jqs.cdnleiting.top

Java: catch (IOException | SQLException e) {}
来源：http://mcq.snrcjt.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ykc.yvedp.cn

Ruby: rescue ArgumentError => e
来源：http://egc.0kj1m.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://afw.ctjpmb.com

[H06] 可选值 / 空值安全访问
来源：http://opp.jinqigfzy.top

Py:   value = d.get("k") or default
来源：http://qcs.xinyue.icu

PHP:  $v = $d["k"] ?? null;
来源：http://sof.zhijiandao.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jfb.xingfuxueyuan.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://lnk.sufxvd.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mti.cheryme.top

Go:   if v, ok := m["k"]; ok { }
来源：http://yfu.yueranfly.top

Ruby: d&.dig(:a, :b)
来源：http://lzl.birdmap.top

C#:   obj?.A?.B ?? default
来源：http://mmu.ydzc1.top

[H07] 断言
来源：http://rso.zhijiandao.cn

Py:   assert x > 0, "必须为正"
来源：http://dmt.cucudq.cn

PHP:  assert($x > 0);
来源：http://uqm.guowangkeji.top

JS:   console.assert(x > 0);
来源：http://cet.gotoacloud.top

TS:   console.assert(x > 0);
来源：http://jcu.cqqwz.cn

Java: assert x > 0 : "必须为正";
来源：http://eek.fktsv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zyf.chenzaomai.com

Ruby: raise "必须为正" unless x > 0
来源：http://kok.sjlbkw.cn

C#:   Debug.Assert(x > 0);
来源：http://tzd.jqgufenzy.top

[H08] 获取错误信息与堆栈
来源：http://rut.jinqigfzy.top

Py:   str(e);  traceback.format_exc()
来源：http://ycf.yangfankeji.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://off.nanxuanxn.top

JS:   e.message;  e.stack
来源：http://vcj.jianghu66.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://gcx.pycfn.com

Java: e.getMessage();  e.printStackTrace()
来源：http://swh.yj20258888.top

Go:   err.Error()
来源：http://dik.dianchejie.cn

Ruby: e.message;  e.backtrace
来源：http://ftu.snrcjt.cn

C#:   e.Message;  e.StackTrace
来源：http://zqk.daria6918.cn

[H09] 带错误码的异常
来源：http://thk.shanyushiyangkeji.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zmp.gzhubu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://svk.yueranfly.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://giu.ehwqpu.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://znz.fehbvm.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tle.epnwcf.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rdt.zhaomingkeji.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://kyf.vqdsnc.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jwx.ydzc1.top

[H10] 资源自动释放
来源：http://hdy.tianlin.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://npl.9152youxi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://llc.zhengqikj.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fjw.chenjidiqi.icu

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lyy.yvedp.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tgp.ybcxt.top

Go:   defer f.Close()
来源：http://xtr.yuxming.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pbf.tianlin.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mxy.xylfe.cn

================================================================================
来源：http://sbn.zhoulong.xyz

I. 正则表达式
来源：http://ebe.xziqi.cn

================================================================================
来源：http://nkd.cucudq.cn

[I01] 判断是否匹配
来源：http://rxn.hongshengwenyu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jvl.bbcook.cn

PHP:  preg_match('/\d+/', $s);
来源：http://mou.jinqigfzy.top

JS:   /\d+/.test(s)
来源：http://ntz.316326.xyz

TS:   /\d+/.test(s)
来源：http://diz.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vpa.kuanghao11.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jcv.chenlongwang.top

Ruby: s.match?(/\d+/)
来源：http://rpo.cucudq.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://noh.ctjpmb.com

[I02] 提取所有匹配
来源：http://cgy.hysaishi.cn

Py:   re.findall(r"\d+", s)
来源：http://xgp.kuanghao11.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xag.316326.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://avv.shzxlz.cn

TS:   s.match(/\d+/g)
来源：http://rri.jianghu66.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xta.ybcxt.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mlw.nanxinkj.top

Ruby: s.scan(/\d+/)
来源：http://cip.tanke756.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sij.nanxinkj.top

[I03] 提取捕获分组
来源：http://kuv.sxryk.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zwx.sufxvd.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://erx.xuanzx.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://axj.yanxiufei.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://plx.shzxlz.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pws.yongpay.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jgr.0kj1m.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ejw.fengsongda.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rxj.9152youxi.cn

[I04] 正则替换
来源：http://ryp.pycfn.com

Py:   re.sub(r"\d+", "#", s)
来源：http://hsf.9152youxi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fvi.jyoumei.cn

JS:   s.replace(/\d+/g, "#")
来源：http://eky.yanxiufei.cn

TS:   s.replace(/\d+/g, "#")
来源：http://eqy.ehwqpu.com

Java: s.replaceAll("\\d+", "#")
来源：http://mzr.gzhubu.top

Go:   re.ReplaceAllString(s, "#")
来源：http://xrp.quarkkingdee.top

Ruby: s.gsub(/\d+/, "#")
来源：http://iiw.hcnkem.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://toe.quarkkingdee.top

[I05] 按正则拆分
来源：http://gyf.sufxvd.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ktd.ehwqpu.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://srf.birdmap.top

JS:   s.split(/\s*,\s*/)
来源：http://xrj.gotoacloud.top

TS:   s.split(/\s*,\s*/)
来源：http://oqy.pycfn.com

Java: s.split("\\s*,\\s*")
来源：http://txr.ydjk.org.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hnd.yvedp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xtd.cheryme.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fpm.ivvv.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gla.jinghuilouyu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mzm.bbcook.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nvh.jyoumei.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aaw.chenlongwang.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vqs.jlsjyb.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xiu.hywenlv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zsx.ydzc1.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://thg.zycfv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hwm.dashuyun.cn

[I07] 忽略大小写与多行模式
来源：http://jxd.hammf.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ltk.daxiang520.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://piq.zhijiandao.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ych.ppjwa.cn

TS:   /error/gim
来源：http://nmg.cucudq.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gyy.jiagoushi.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qmp.9152youxi.cn

Ruby: s.scan(/error/i)
来源：http://itr.iojbl.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wpx.iojbl.cn

[I08] 贪婪与非贪婪匹配
来源：http://etn.xuanzx.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zvw.yangfankeji.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://thw.zycfv.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wwn.fengsongda.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://onq.dianchejie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rds.ivvv.top


<!-- 参考信息 -->