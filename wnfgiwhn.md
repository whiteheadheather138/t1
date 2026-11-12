代发 wailian999

================================================================================
来源：http://aoj.gzhubu.top

G. 面向对象
来源：http://tms.hnqzz.top

================================================================================
来源：http://chd.yj20258.top

[G01] 定义类
来源：http://bbd.c1oappe.top

Py:   class User: pass
来源：http://kwp.tanke756.top

PHP:  class User {}
来源：http://mdf.jinqigfzy.top

JS:   class User {}
来源：http://hoq.hfpthk.cn

TS:   class User { name: string = ""; }
来源：http://izv.bbcook.cn

Java: class User {}
来源：http://rkd.xuetiantiany.cn

Go:   type User struct { Name string }
来源：http://lms.0kj1m.cn

Ruby: class User; end
来源：http://ekl.yueranfly.top

C#:   class User {}
来源：http://amh.fanxiaobao.xyz

[G02] 构造函数
来源：http://hca.chenlongwang.top

Py:   def __init__(self, name): self.name = name
来源：http://zbu.gotoacloud.top

PHP:  public function __construct(public string $name) {}
来源：http://pmz.zdqjudy.top

JS:   constructor(name) { this.name = name; }
来源：http://vqj.hfpthk.cn

TS:   constructor(public name: string) {}
来源：http://lqs.xziqi.cn

Java: User(String name) { this.name = name; }
来源：http://fca.cashguo.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wcr.smart0.xyz

Ruby: def initialize(name); @name = name; end
来源：http://vuy.wangdashe.top

C#:   public User(string name) { Name = name; }
来源：http://mwu.xziqi.cn

[G03] 实例属性
来源：http://vpn.yanxiufei.cn

Py:   self.name = "x"
来源：http://dmf.mhx1999.top

PHP:  public string $name = "x";
来源：http://hgc.redwolf501.top

JS:   this.name = "x";
来源：http://chb.hongshengwenyu.top

TS:   name: string = "x";
来源：http://ftf.chenzaomai.com

Java: private String name;
来源：http://xfj.mhx1999.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hlu.haohaochexian.top

Ruby: @name = "x"
来源：http://pdm.haohaochexian.top

C#:   public string Name { get; set; } = "x";
来源：http://moy.hnqzz.top

[G04] 定义方法
来源：http://ptj.andypj.xyz

Py:   def greet(self): return self.name
来源：http://jza.fanxiaobao.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://dez.shuidangran.top

JS:   greet() { return this.name; }
来源：http://ckz.andypj.xyz

TS:   greet(): string { return this.name; }
来源：http://qrq.meibo888.top

Java: String greet() { return name; }
来源：http://fhj.chenjidiqi.icu

Go:   func (u User) Greet() string { return u.Name }
来源：http://nku.tianlin.xyz

Ruby: def greet; @name; end
来源：http://tot.xuanzx.com

C#:   public string Greet() => Name;
来源：http://dva.tarul.cn

[G05] 继承
来源：http://yin.zhixingplan.top

Py:   class Admin(User): pass
来源：http://rzb.jinghuilouyu.cn

PHP:  class Admin extends User {}
来源：http://vez.wangshuangyany.cn

JS:   class Admin extends User {}
来源：http://jer.hammf.cn

TS:   class Admin extends User {}
来源：http://upq.kuanghao11.cn

Java: class Admin extends User {}
来源：http://xra.hysaishi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nhp.yanxiufei.cn

Ruby: class Admin < User; end
来源：http://xdz.ctjpmb.com

C#:   class Admin : User {}
来源：http://rgl.ybcxt.top

[G06] 重写方法
来源：http://xwl.316326.xyz

Py:   def greet(self): return "admin"
来源：http://lpw.jqgufenzy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://srp.wangdashe.top

JS:   greet() { return "admin"; }
来源：http://wuw.gaohongyu789.top

TS:   greet(): string { return "admin"; }
来源：http://ifb.52xcode.cn

Java: @Override String greet() { return "admin"; }
来源：http://mmo.gogol.net.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rux.ywan-chungtsiang.top

Ruby: def greet; "admin"; end
来源：http://xmq.hongshengwenyu.top

C#:   public override string Greet() => "admin";
来源：http://pwo.bjfxy.top

[G07] 调用父类方法
来源：http://yvb.tian-w.cn

Py:   super().greet()
来源：http://hmp.yangfankeji.com

PHP:  parent::greet();
来源：http://xnc.zhijiandao.cn

JS:   super.greet();
来源：http://ywy.havefunace.top

TS:   super.greet();
来源：http://nxl.dashuyun.cn

Java: super.greet();
来源：http://svm.nwbrower.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wga.jinqigufen.top

Ruby: super
来源：http://yhi.pycfn.com

C#:   base.Greet();
来源：http://yrg.shanyushiyangtech.top

[G08] 静态方法与属性
来源：http://kay.zhoulong.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bzk.zdqjudy.top

PHP:  public static function f() {}
来源：http://eer.kuanghao11.cn

JS:   static f() {}
来源：http://ruv.yangfankeji.com

TS:   static f(): void {}
来源：http://gds.jinyuanbaomall.cn

Java: static void f() {}
来源：http://fmj.zhoulong.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://jrv.xziqi.cn

Ruby: def self.f; end
来源：http://jkv.vqdsnc.cn

C#:   public static void F() {}
来源：http://qpa.xinyue.icu

[G09] 接口 / 抽象类
来源：http://uch.xuetiantiany.cn

Py:   from abc import ABC, abstractmethod
来源：http://ndc.jianghu66.top

PHP:  interface Shape { public function area(): float; }
来源：http://qfh.yj20258.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://tyg.uphjek.com

TS:   interface Shape { area(): number; }
来源：http://hde.316326.xyz

Java: interface Shape { double area(); }
来源：http://lub.daria6918.cn

Go:   type Shape interface { Area() float64 }
来源：http://pwv.hesvh.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://acm.yanxiufei.cn

C#:   interface IShape { double Area(); }
来源：http://onf.mhx1999.top

[G10] 访问控制
来源：http://oyt.snrcjt.cn

Py:   约定 _protected / __private（不强制）
来源：http://vry.yuxming.cn

PHP:  public / protected / private
来源：http://lfl.svipenyu.cn

JS:   #private 字段；其余公开
来源：http://hze.chenzaomai.com

TS:   public / protected / private
来源：http://rbf.yuanzhike.top

Java: public / protected / private / 默认包级
来源：http://rix.xylfe.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nde.sufxvd.cn

Ruby: public / protected / private
来源：http://hcf.jinghuilouyu.cn

C#:   public / protected / private / internal
来源：http://mak.jyoumei.cn

[G11] getter / setter
来源：http://xmi.zhengqikj.top

Py:   @property 与 @x.setter
来源：http://alx.ctjpmb.com

PHP:  public function getName(): string { return $this->name; }
来源：http://caj.hfpthk.cn

JS:   get name() { return this._name; }
来源：http://fwn.birdmap.top

TS:   get name(): string { return this._name; }
来源：http://szl.hysaishi.cn

Java: public String getName() { return name; }
来源：http://yip.yj20258888.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://kwz.daxiang520.top

Ruby: attr_accessor :name
来源：http://kqx.sufxvd.cn

C#:   public string Name { get; set; }
来源：http://qeu.fzhhl.top

[G12] 对象转字符串
来源：http://eop.zhixingplan.top

Py:   def __str__(self): return self.name
来源：http://qey.bbcook.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qbx.iojbl.cn

JS:   toString() { return this.name; }
来源：http://frh.yj20258.top

TS:   toString(): string { return this.name; }
来源：http://wvd.fanxiaobao.xyz

Java: @Override public String toString() { return name; }
来源：http://hwz.zdqjudy.top

Go:   func (u User) String() string { return u.Name }
来源：http://emf.xinyue.icu

Ruby: def to_s; @name; end
来源：http://gmu.hnqzz.top

C#:   public override string ToString() => Name;
来源：http://ken.xingfuxueyuan.xyz

[G13] 判断对象类型
来源：http://jzq.cucudq.cn

Py:   isinstance(u, User)
来源：http://mmi.xuetiantiany.cn

PHP:  $u instanceof User
来源：http://ayb.sxryk.cn

JS:   u instanceof User
来源：http://gzn.yuxming.cn

TS:   u instanceof User
来源：http://qwd.ywan-chungtsiang.top

Java: u instanceof User
来源：http://wwl.vqdsnc.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kju.guannengcc.top

Ruby: u.is_a?(User)
来源：http://ucl.havefunace.top

C#:   u is User
来源：http://hmz.aibaodan.cn

[G14] 数据类 / record
来源：http://qbj.zhoulong.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cef.jqgfzy.top

PHP:  // 用 readonly 属性模拟
来源：http://jqj.zhaomingkeji.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://lhx.fanxiaobao.xyz

TS:   type User = { name: string; age: number };
来源：http://tpl.cqqwz.cn

Java: record User(String name, int age) {}
来源：http://qae.wangshuangyany.cn

Go:   type User struct { Name string; Age int }
来源：http://lua.sxryk.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ajv.dashuyun.cn

C#:   record User(string Name, int Age);
来源：http://hvx.jyoumei.cn

[G15] 枚举
来源：http://klt.yueranfly.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dqz.hnqzz.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://etm.quarkkingdee.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://plc.tianlin.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bsv.dashuyun.cn

Java: enum Color { RED, GREEN }
来源：http://kfo.zdbjq.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bep.hnqzz.top

Ruby: Color = %i[red green].freeze
来源：http://qye.zycfv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ypj.guowangkeji.top

[G16] 对象转数组 / 字典
来源：http://ivk.zhiwuduotai.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wss.yonumen.top

PHP:  get_object_vars($obj);
来源：http://prb.svipenyu.cn

JS:   Object.entries(obj)
来源：http://jwl.hcnkem.com

TS:   Object.entries(obj)
来源：http://mob.gogol.net.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://swu.fengsongda.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://fkn.yuanzhike.top

Ruby: obj.instance_variables
来源：http://jbn.havefunace.top

C#:   // 用反射或 System.Text.Json
来源：http://rer.jinghuilouyu.cn

================================================================================
来源：http://jtm.fehbvm.com

H. 异常与错误处理
来源：http://fbn.hfpthk.cn

================================================================================
来源：http://jro.snrcjt.cn

[H01] try / catch 基础
来源：http://vco.aizwys.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kyi.fengsongda.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://opr.fengsongda.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rbk.yfazqb.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qef.zhaomingkeji.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fym.52xcode.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nbq.yj20258.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sdi.zhijiandao.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ams.jlsjyb.cn

[H02] finally / ensure 收尾
来源：http://bcn.yj20258.top

Py:   try: f()⏎finally: cleanup()
来源：http://ygq.yj20258.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://kdu.shanyushiyangkeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://qfs.yongpay.top

TS:   try { f(); } finally { cleanup(); }
来源：http://bvy.hesvh.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qca.andypj.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://vfs.0kj1m.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://xcq.hywenlv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tcj.jinqigufen.top

[H03] 主动抛出异常
来源：http://mlk.nwbrower.top

Py:   raise ValueError("错误信息")
来源：http://lzc.zdbjq.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bnd.jqgfzy.top

JS:   throw new Error("错误信息");
来源：http://obn.nanxuanxn.top

TS:   throw new Error("错误信息");
来源：http://zci.chenzaomai.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://msd.fanxiaobao.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://aje.316326.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://dks.feifeiyinyue.top

C#:   throw new ArgumentException("错误信息");
来源：http://jhl.andypj.xyz

[H04] 自定义异常类型
来源：http://gtc.fktsv.cn

Py:   class MyError(Exception): pass
来源：http://stl.shuidangran.top

PHP:  class MyError extends RuntimeException {}
来源：http://jvf.shanyushiyangtech.top

JS:   class MyError extends Error {}
来源：http://ubn.zhijiandao.cn

TS:   class MyError extends Error {}
来源：http://slc.yongpay.top

Java: class MyException extends RuntimeException {}
来源：http://vjx.ehwqpu.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vot.nwbrower.top

Ruby: class MyError < StandardError; end
来源：http://iih.jqgfzy.top

C#:   class MyException : Exception {}
来源：http://tuk.dashuyun.cn

[H05] 捕获特定类型
来源：http://ffx.fanxiaobao.xyz

Py:   except ValueError as e:
来源：http://mpu.xinyue.icu

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cav.daria6918.cn

JS:   if (e instanceof TypeError) {}
来源：http://yqv.shanyushiyangtech.top

TS:   if (e instanceof TypeError) {}
来源：http://gvn.0kj1m.cn

Java: catch (IOException | SQLException e) {}
来源：http://uwk.zhiwuduotai.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://btc.bbcook.cn

Ruby: rescue ArgumentError => e
来源：http://gdz.xuetiantiany.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://aue.tanke756.top

[H06] 可选值 / 空值安全访问
来源：http://fch.svipenyu.cn

Py:   value = d.get("k") or default
来源：http://abx.yanxiufei.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mrq.hesvh.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xtb.yongpay.top

TS:   obj?.a?.b;  d ?? default
来源：http://sso.chenzaomai.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wvp.ivvv.top

Go:   if v, ok := m["k"]; ok { }
来源：http://uuy.yuanzhike.top

Ruby: d&.dig(:a, :b)
来源：http://rup.jqgfzy.top

C#:   obj?.A?.B ?? default
来源：http://sej.hywenlv.cn

[H07] 断言
来源：http://bvh.jinghuilouyu.cn

Py:   assert x > 0, "必须为正"
来源：http://wnb.sjlbkw.cn

PHP:  assert($x > 0);
来源：http://ksy.hcnkem.com

JS:   console.assert(x > 0);
来源：http://skr.pengpengdd.cyou

TS:   console.assert(x > 0);
来源：http://rjq.hcnkem.com

Java: assert x > 0 : "必须为正";
来源：http://nbh.zhixingplan.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hpv.shuidangran.top

Ruby: raise "必须为正" unless x > 0
来源：http://ojx.nwbrower.top

C#:   Debug.Assert(x > 0);
来源：http://lqb.tianlin.xyz

[H08] 获取错误信息与堆栈
来源：http://ggu.xziqi.cn

Py:   str(e);  traceback.format_exc()
来源：http://asp.chenlongwang.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://plj.sjlbkw.cn

JS:   e.message;  e.stack
来源：http://abt.xuanzx.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://tdz.316326.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://iny.dianchejie.cn

Go:   err.Error()
来源：http://kks.cqqwz.cn

Ruby: e.message;  e.backtrace
来源：http://ets.9152youxi.cn

C#:   e.Message;  e.StackTrace
来源：http://bkz.birdmap.top

[H09] 带错误码的异常
来源：http://ovm.nwbrower.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ybb.hongshengwenyu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://tpx.chenlongwang.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://eco.jqgfzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pie.yuanzhike.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://krc.svipenyu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://opk.tanke756.top

Ruby: raise MyError.new("fail", 500)
来源：http://xyv.hfpthk.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ido.fzhhl.top

[H10] 资源自动释放
来源：http://atd.jinqigfzy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://scz.hammf.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rmy.daria6918.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hvc.cheryme.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cmx.yuxming.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hoc.316326.xyz

Go:   defer f.Close()
来源：http://jze.jlsjyb.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://obc.ehwqpu.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fml.jlsjyb.cn

================================================================================
来源：http://kuu.zhongyouzk.top

I. 正则表达式
来源：http://uwm.bbcook.cn

================================================================================
来源：http://kvj.chenzaomai.com

[I01] 判断是否匹配
来源：http://qne.xziqi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://exn.cqqwz.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vyb.hfpthk.cn

JS:   /\d+/.test(s)
来源：http://csf.hfpthk.cn

TS:   /\d+/.test(s)
来源：http://vde.pycfn.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://scu.cashguo.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lcz.zhongyouzk.top

Ruby: s.match?(/\d+/)
来源：http://ckf.bbcook.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lli.316326.xyz

[I02] 提取所有匹配
来源：http://cig.52xcode.cn

Py:   re.findall(r"\d+", s)
来源：http://igs.daxiang520.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rkj.jianghu66.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hua.zhiwuduotai.top

TS:   s.match(/\d+/g)
来源：http://hbr.uphjek.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qfs.jlsjyb.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rpp.ivvv.top

Ruby: s.scan(/\d+/)
来源：http://jhm.guannengcc.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tdb.feifeiyinyue.top

[I03] 提取捕获分组
来源：http://yqj.pengpengdd.cyou

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://msc.fzhhl.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gof.dashuyun.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cck.jqgufenzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fiu.chenjidiqi.icu

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://von.jqgufenzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rxl.cheryme.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jmg.uphjek.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gyc.jyoumei.cn

[I04] 正则替换
来源：http://yqi.sweek.top

Py:   re.sub(r"\d+", "#", s)
来源：http://cqo.xingfuxueyuan.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://olr.uphjek.com

JS:   s.replace(/\d+/g, "#")
来源：http://qqr.jiagoushi.top

TS:   s.replace(/\d+/g, "#")
来源：http://nwd.uphjek.com

Java: s.replaceAll("\\d+", "#")
来源：http://npe.chenzaomai.com

Go:   re.ReplaceAllString(s, "#")
来源：http://bny.zdqjudy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://rrl.fktsv.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jqc.c1oappe.top

[I05] 按正则拆分
来源：http://kxn.hysaishi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qoy.shanyushiyangtech.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://skx.tanke756.top

JS:   s.split(/\s*,\s*/)
来源：http://vsp.jiagoushi.top

TS:   s.split(/\s*,\s*/)
来源：http://pof.vqdsnc.cn

Java: s.split("\\s*,\\s*")
来源：http://ctf.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nak.gogol.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vac.sweek.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mdh.yvedp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qud.mhx1999.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tvw.daxiang520.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vnz.tian-w.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ddk.redwolf501.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://afb.shanyushiyangtech.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wyg.fengsongda.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wwn.aizwys.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nyq.jinqigfzy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zsm.tarul.cn

[I07] 忽略大小写与多行模式
来源：http://fiw.sjlbkw.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dyh.svipenyu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://awv.nanxuanxn.top


<!-- 参考信息 -->