代发 wailian999

Py:   class User: pass
来源：http://znm.guannengcc.top

PHP:  class User {}
来源：http://erc.cqqwz.cn

JS:   class User {}
来源：http://mxl.yanxiufei.cn

TS:   class User { name: string = ""; }
来源：http://igs.ybcxt.top

Java: class User {}
来源：http://oro.snrcjt.cn

Go:   type User struct { Name string }
来源：http://koj.cqqwz.cn

Ruby: class User; end
来源：http://wso.316326.xyz

C#:   class User {}
来源：http://nqv.bjfxy.top

[G02] 构造函数
来源：http://oev.sysykeji.top

Py:   def __init__(self, name): self.name = name
来源：http://xza.tanke756.top

PHP:  public function __construct(public string $name) {}
来源：http://hri.zhongyouzk.top

JS:   constructor(name) { this.name = name; }
来源：http://lhx.jinghuilouyu.cn

TS:   constructor(public name: string) {}
来源：http://sgp.yuxming.cn

Java: User(String name) { this.name = name; }
来源：http://tzw.c1oappe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ndd.ctjpmb.com

Ruby: def initialize(name); @name = name; end
来源：http://czv.andypj.xyz

C#:   public User(string name) { Name = name; }
来源：http://woq.ppjwa.cn

[G03] 实例属性
来源：http://xmi.fzhhl.top

Py:   self.name = "x"
来源：http://xci.daxiang520.top

PHP:  public string $name = "x";
来源：http://clg.pycfn.com

JS:   this.name = "x";
来源：http://yrm.yvedp.cn

TS:   name: string = "x";
来源：http://kdd.cashguo.top

Java: private String name;
来源：http://weu.zhongyouzk.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mrj.gotoacloud.top

Ruby: @name = "x"
来源：http://vpx.xinyue.icu

C#:   public string Name { get; set; } = "x";
来源：http://tcf.haohaochexian.top

[G04] 定义方法
来源：http://ata.sufxvd.cn

Py:   def greet(self): return self.name
来源：http://urr.yuanzhike.top

PHP:  public function greet(): string { return $this->name; }
来源：http://wyx.9152youxi.cn

JS:   greet() { return this.name; }
来源：http://gei.shanyushiyangtech.top

TS:   greet(): string { return this.name; }
来源：http://jdv.9152youxi.cn

Java: String greet() { return name; }
来源：http://hrw.ivvv.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://dgr.yonumen.top

Ruby: def greet; @name; end
来源：http://egl.sufxvd.cn

C#:   public string Greet() => Name;
来源：http://dne.hysaishi.cn

[G05] 继承
来源：http://gqx.dianchejie.cn

Py:   class Admin(User): pass
来源：http://syi.hcnkem.com

PHP:  class Admin extends User {}
来源：http://ifv.xziqi.cn

JS:   class Admin extends User {}
来源：http://qrm.wangshuangyany.cn

TS:   class Admin extends User {}
来源：http://pfx.yonumen.top

Java: class Admin extends User {}
来源：http://xqg.ywan-chungtsiang.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lak.yj20258.top

Ruby: class Admin < User; end
来源：http://fda.xingfuxueyuan.xyz

C#:   class Admin : User {}
来源：http://ajv.yonumen.top

[G06] 重写方法
来源：http://piu.daxiang520.top

Py:   def greet(self): return "admin"
来源：http://azs.smart0.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://vcu.cashguo.top

JS:   greet() { return "admin"; }
来源：http://nwc.xuanzx.com

TS:   greet(): string { return "admin"; }
来源：http://cbo.hysaishi.cn

Java: @Override String greet() { return "admin"; }
来源：http://xow.nanxuanxn.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zfz.jiagoushi.top

Ruby: def greet; "admin"; end
来源：http://lpg.chenzaomai.com

C#:   public override string Greet() => "admin";
来源：http://yvc.guannengcc.top

[G07] 调用父类方法
来源：http://erp.mhx1999.top

Py:   super().greet()
来源：http://qfc.zhengqikj.top

PHP:  parent::greet();
来源：http://hqp.zhijiandao.cn

JS:   super.greet();
来源：http://loa.havefunace.top

TS:   super.greet();
来源：http://oov.hcnkem.com

Java: super.greet();
来源：http://pvk.yj202588.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pow.andypj.xyz

Ruby: super
来源：http://wzr.jianghu66.top

C#:   base.Greet();
来源：http://qhv.ybcxt.top

[G08] 静态方法与属性
来源：http://sdm.sufxvd.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vwq.yj20258.top

PHP:  public static function f() {}
来源：http://ndm.jyoumei.cn

JS:   static f() {}
来源：http://wec.bbcook.cn

TS:   static f(): void {}
来源：http://uor.dianchejie.cn

Java: static void f() {}
来源：http://tpd.ywan-chungtsiang.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://amt.cdnleiting.top

Ruby: def self.f; end
来源：http://ybo.zhixingplan.top

C#:   public static void F() {}
来源：http://fby.yonumen.top

[G09] 接口 / 抽象类
来源：http://paf.haohaochexian.top

Py:   from abc import ABC, abstractmethod
来源：http://hyx.vehdjk.com

PHP:  interface Shape { public function area(): float; }
来源：http://mwz.yanxiufei.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://snn.cdnleiting.top

TS:   interface Shape { area(): number; }
来源：http://kro.jyoumei.cn

Java: interface Shape { double area(); }
来源：http://tcb.tanke756.top

Go:   type Shape interface { Area() float64 }
来源：http://oiq.yfazqb.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yev.zhixingplan.top

C#:   interface IShape { double Area(); }
来源：http://nbi.52xcode.cn

[G10] 访问控制
来源：http://gsu.zdbjq.cn

Py:   约定 _protected / __private（不强制）
来源：http://xzz.shangyingyoupin.top

PHP:  public / protected / private
来源：http://sio.ctjpmb.com

JS:   #private 字段；其余公开
来源：http://reh.shanyushiyangkeji.top

TS:   public / protected / private
来源：http://xdk.tanke756.top

Java: public / protected / private / 默认包级
来源：http://lli.nanxuanxn.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://dzu.shanyushiyangkeji.top

Ruby: public / protected / private
来源：http://brh.hysaishi.cn

C#:   public / protected / private / internal
来源：http://uar.hcnkem.com

[G11] getter / setter
来源：http://iny.tianlin.xyz

Py:   @property 与 @x.setter
来源：http://dqt.9152youxi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://uwr.yuxming.cn

JS:   get name() { return this._name; }
来源：http://wfj.52xcode.cn

TS:   get name(): string { return this._name; }
来源：http://owm.jinqigfzy.top

Java: public String getName() { return name; }
来源：http://emm.guowangkeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://qwr.yj20258.top

Ruby: attr_accessor :name
来源：http://heu.ybcxt.top

C#:   public string Name { get; set; }
来源：http://iuj.yj20258888.top

[G12] 对象转字符串
来源：http://wld.yonumen.top

Py:   def __str__(self): return self.name
来源：http://yhl.shuidangran.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://cgq.ybcxt.top

JS:   toString() { return this.name; }
来源：http://gji.ydzc1.top

TS:   toString(): string { return this.name; }
来源：http://cpp.shangyingyoupin.top

Java: @Override public String toString() { return name; }
来源：http://vyg.yongpay.top

Go:   func (u User) String() string { return u.Name }
来源：http://rht.ppjwa.cn

Ruby: def to_s; @name; end
来源：http://wmi.jyoumei.cn

C#:   public override string ToString() => Name;
来源：http://rba.dashuyun.cn

[G13] 判断对象类型
来源：http://jcy.zdbjq.cn

Py:   isinstance(u, User)
来源：http://seb.jyoumei.cn

PHP:  $u instanceof User
来源：http://fql.shangyingyoupin.top

JS:   u instanceof User
来源：http://drr.fzhhl.top

TS:   u instanceof User
来源：http://dfu.cashguo.top

Java: u instanceof User
来源：http://eio.zhaomingkeji.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://khw.yangfankeji.com

Ruby: u.is_a?(User)
来源：http://zwm.daria6918.cn

C#:   u is User
来源：http://sxv.zhiwuduotai.top

[G14] 数据类 / record
来源：http://bem.yuxming.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xlw.ehwqpu.com

PHP:  // 用 readonly 属性模拟
来源：http://mkq.yfazqb.com

JS:   // 无内置：普通类或对象字面量
来源：http://gln.sjlbkw.cn

TS:   type User = { name: string; age: number };
来源：http://fxs.yvedp.cn

Java: record User(String name, int age) {}
来源：http://qfm.yuxming.cn

Go:   type User struct { Name string; Age int }
来源：http://qor.havefunace.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://smi.ctjpmb.com

C#:   record User(string Name, int Age);
来源：http://ytg.aizwys.cn

[G15] 枚举
来源：http://afz.shuidangran.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://crr.guowangkeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ogn.zhengqikj.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://prz.jianghu66.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://owy.xylfe.cn

Java: enum Color { RED, GREEN }
来源：http://kjh.daria6918.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rhn.sufxvd.cn

Ruby: Color = %i[red green].freeze
来源：http://bjr.xziqi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mxg.hfpthk.cn

[G16] 对象转数组 / 字典
来源：http://wme.ydzc1.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tyn.jqgufenzy.top

PHP:  get_object_vars($obj);
来源：http://mpn.wangdashe.top

JS:   Object.entries(obj)
来源：http://oak.yuanzhike.top

TS:   Object.entries(obj)
来源：http://ary.aizwys.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tzk.ppjwa.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hrh.haohaochexian.top

Ruby: obj.instance_variables
来源：http://hin.hammf.cn

C#:   // 用反射或 System.Text.Json
来源：http://wge.sysykeji.top

================================================================================
来源：http://qnb.zhengqikj.top

H. 异常与错误处理
来源：http://vas.9152youxi.cn

================================================================================
来源：http://gjo.smart0.xyz

[H01] try / catch 基础
来源：http://ddr.nanxinkj.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qhb.hongshengwenyu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lph.jinqigufen.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gbl.dashuyun.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://obc.zhaomingkeji.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lxe.zhoulong.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yen.nanxinkj.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://upg.kuanghao11.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mad.xinyue.icu

[H02] finally / ensure 收尾
来源：http://pmf.yonumen.top

Py:   try: f()⏎finally: cleanup()
来源：http://tcb.bjfxy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://qaz.zdqjudy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://dbf.gzhubu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://mdh.pengpengdd.cyou

Java: try { f(); } finally { cleanup(); }
来源：http://wfq.yonumen.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://prt.yongpay.top

Ruby: begin; f; ensure; cleanup; end
来源：http://qca.daria6918.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hxo.fehbvm.com

[H03] 主动抛出异常
来源：http://lpv.fanxiaobao.xyz

Py:   raise ValueError("错误信息")
来源：http://czo.cashguo.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nul.epnwcf.com

JS:   throw new Error("错误信息");
来源：http://pyy.aizwys.cn

TS:   throw new Error("错误信息");
来源：http://yjv.guannengcc.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://bkb.yvedp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dsh.daria6918.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://kqy.hesvh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://guy.fehbvm.com

[H04] 自定义异常类型
来源：http://pmc.ctjpmb.com

Py:   class MyError(Exception): pass
来源：http://wyk.zhengqikj.top

PHP:  class MyError extends RuntimeException {}
来源：http://adn.kuanghao11.cn

JS:   class MyError extends Error {}
来源：http://uwx.bjfxy.top

TS:   class MyError extends Error {}
来源：http://nob.meibo888.top

Java: class MyException extends RuntimeException {}
来源：http://nld.fengsongda.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ajc.hesvh.cn

Ruby: class MyError < StandardError; end
来源：http://urf.yfazqb.com

C#:   class MyException : Exception {}
来源：http://qsq.smart0.xyz

[H05] 捕获特定类型
来源：http://vco.sweek.top

Py:   except ValueError as e:
来源：http://skc.uphjek.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wyf.316326.xyz

JS:   if (e instanceof TypeError) {}
来源：http://dnc.jlsjyb.cn

TS:   if (e instanceof TypeError) {}
来源：http://mts.wangdashe.top

Java: catch (IOException | SQLException e) {}
来源：http://arg.jyoumei.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sir.redwolf501.top

Ruby: rescue ArgumentError => e
来源：http://muw.cqqwz.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://olq.snrcjt.cn

[H06] 可选值 / 空值安全访问
来源：http://ymt.yuanzhike.top

Py:   value = d.get("k") or default
来源：http://qwf.hywenlv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kvd.chenjidiqi.icu

JS:   obj?.a?.b;  d ?? default
来源：http://qnt.316326.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://qcp.dashuyun.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dey.feifeiyinyue.top

Go:   if v, ok := m["k"]; ok { }
来源：http://plo.gotoacloud.top

Ruby: d&.dig(:a, :b)
来源：http://wqd.guannengcc.top

C#:   obj?.A?.B ?? default
来源：http://rkb.mhx1999.top

[H07] 断言
来源：http://kgo.svipenyu.cn

Py:   assert x > 0, "必须为正"
来源：http://lex.jqgufenzy.top

PHP:  assert($x > 0);
来源：http://lbf.jinyuanbaomall.cn

JS:   console.assert(x > 0);
来源：http://qeg.ywan-chungtsiang.top

TS:   console.assert(x > 0);
来源：http://lty.xziqi.cn

Java: assert x > 0 : "必须为正";
来源：http://bkp.zdbjq.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kkw.yvedp.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wng.jinyuanbaomall.cn

C#:   Debug.Assert(x > 0);
来源：http://csz.fehbvm.com

[H08] 获取错误信息与堆栈
来源：http://bth.cqqwz.cn

Py:   str(e);  traceback.format_exc()
来源：http://rpt.yongpay.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wws.jiagoushi.top

JS:   e.message;  e.stack
来源：http://xgb.jinyuanbaomall.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zjd.jyoumei.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://chq.hywenlv.cn

Go:   err.Error()
来源：http://bjf.jianghu66.top

Ruby: e.message;  e.backtrace
来源：http://xbg.ctjpmb.com

C#:   e.Message;  e.StackTrace
来源：http://iwo.pycfn.com

[H09] 带错误码的异常
来源：http://awh.meibo888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cou.dashuyun.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wny.chenlongwang.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://npj.cashguo.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cqc.jiagoushi.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://iwv.gzhubu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://eqy.feifeiyinyue.top

Ruby: raise MyError.new("fail", 500)
来源：http://kwq.hfpthk.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qxi.daria6918.cn

[H10] 资源自动释放
来源：http://yrl.jiagoushi.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://isr.zdqjudy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ggc.guowangkeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://frt.hysaishi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bqi.vqdsnc.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ujx.nanxinkj.top

Go:   defer f.Close()
来源：http://can.redwolf501.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yke.hfpthk.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dzw.hywenlv.cn

================================================================================
来源：http://cwd.xuanzx.com

I. 正则表达式
来源：http://mer.dashuyun.cn

================================================================================
来源：http://lto.epnwcf.com

[I01] 判断是否匹配
来源：http://fsk.chenzaomai.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zig.zhixingplan.top

PHP:  preg_match('/\d+/', $s);
来源：http://djg.aibaodan.cn

JS:   /\d+/.test(s)
来源：http://vcf.dashuyun.cn

TS:   /\d+/.test(s)
来源：http://oep.haohaochexian.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rcq.sxryk.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://aht.hesvh.cn

Ruby: s.match?(/\d+/)
来源：http://ouz.haohaochexian.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dev.bjfxy.top

[I02] 提取所有匹配
来源：http://awm.shanyushiyangkeji.top

Py:   re.findall(r"\d+", s)
来源：http://zba.jinqigufen.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dsv.xziqi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xeq.hfpthk.cn

TS:   s.match(/\d+/g)
来源：http://qtq.zhiwuduotai.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://irp.iojbl.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rjw.nanxinkj.top

Ruby: s.scan(/\d+/)
来源：http://ozv.bbcook.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yxt.dashuyun.cn

[I03] 提取捕获分组
来源：http://avu.yj20258.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dzk.redwolf501.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lyo.nanxinkj.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://koh.xingfuxueyuan.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jpw.pycfn.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vru.yangfankeji.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jae.chenjidiqi.icu

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://era.dashuyun.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://muk.hfpthk.cn

[I04] 正则替换
来源：http://shz.cucudq.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rmh.ywan-chungtsiang.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zsj.gaohongyu789.top

JS:   s.replace(/\d+/g, "#")
来源：http://tqr.gotoacloud.top

TS:   s.replace(/\d+/g, "#")
来源：http://pqi.tian-w.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fmy.guannengcc.top

Go:   re.ReplaceAllString(s, "#")
来源：http://gkm.gogol.net.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wvd.aibaodan.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nct.jiagoushi.top

[I05] 按正则拆分
来源：http://nst.jinyuanbaomall.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://krg.ivvv.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cry.yvedp.cn

JS:   s.split(/\s*,\s*/)
来源：http://ymq.jyoumei.cn

TS:   s.split(/\s*,\s*/)
来源：http://kxx.zhijiandao.cn

Java: s.split("\\s*,\\s*")
来源：http://dkq.shangyingyoupin.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://snf.tianlin.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://ula.hcnkem.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cab.sufxvd.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zbo.ctjpmb.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://drq.xuetiantiany.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://shh.yonumen.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://idh.chenlongwang.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bex.gogol.net.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bwp.tianlin.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://llb.ppjwa.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fva.zdqjudy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vys.jqgfzy.top

[I07] 忽略大小写与多行模式
来源：http://fxo.zhijiandao.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kpk.fanxiaobao.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mxm.zhixingplan.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bit.jinyuanbaomall.cn

TS:   /error/gim
来源：http://egs.jqgfzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pqs.xylfe.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bau.haohaochexian.top


<!-- 参考信息 -->