代发 wailian999

================================================================================
来源：http://fse.cucudq.cn

G. 面向对象
来源：http://eca.zhaomingkeji.xyz

================================================================================
来源：http://tge.0kj1m.cn

[G01] 定义类
来源：http://rbn.dashuyun.cn

Py:   class User: pass
来源：http://xsr.sweek.top

PHP:  class User {}
来源：http://jgx.cdnleiting.top

JS:   class User {}
来源：http://olf.ywan-chungtsiang.top

TS:   class User { name: string = ""; }
来源：http://lrt.daxiang520.top

Java: class User {}
来源：http://gjk.tian-w.cn

Go:   type User struct { Name string }
来源：http://uvu.jianghu66.top

Ruby: class User; end
来源：http://sdu.gogol.net.cn

C#:   class User {}
来源：http://fso.smart0.xyz

[G02] 构造函数
来源：http://nhj.pycfn.com

Py:   def __init__(self, name): self.name = name
来源：http://qrv.fengsongda.top

PHP:  public function __construct(public string $name) {}
来源：http://qan.hysaishi.cn

JS:   constructor(name) { this.name = name; }
来源：http://gje.daria6918.cn

TS:   constructor(public name: string) {}
来源：http://hrw.ydzc1.top

Java: User(String name) { this.name = name; }
来源：http://aiv.cdnleiting.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mdy.ydzc1.top

Ruby: def initialize(name); @name = name; end
来源：http://pts.xylfe.cn

C#:   public User(string name) { Name = name; }
来源：http://ddg.yonumen.top

[G03] 实例属性
来源：http://mxv.nwbrower.top

Py:   self.name = "x"
来源：http://apl.tian-w.cn

PHP:  public string $name = "x";
来源：http://yhb.hnqzz.top

JS:   this.name = "x";
来源：http://nhd.jianghu66.top

TS:   name: string = "x";
来源：http://ivc.ybcxt.top

Java: private String name;
来源：http://fhe.nwbrower.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://drv.yvedp.cn

Ruby: @name = "x"
来源：http://gjn.gotoacloud.top

C#:   public string Name { get; set; } = "x";
来源：http://nfj.pycfn.com

[G04] 定义方法
来源：http://tjh.quarkkingdee.top

Py:   def greet(self): return self.name
来源：http://hry.hongshengwenyu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://smm.jinghuilouyu.cn

JS:   greet() { return this.name; }
来源：http://otj.guannengcc.top

TS:   greet(): string { return this.name; }
来源：http://var.gogol.net.cn

Java: String greet() { return name; }
来源：http://yvf.vqdsnc.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://whf.52xcode.cn

Ruby: def greet; @name; end
来源：http://kqn.ctjpmb.com

C#:   public string Greet() => Name;
来源：http://glx.shanyushiyangkeji.top

[G05] 继承
来源：http://yog.xinyue.icu

Py:   class Admin(User): pass
来源：http://mom.gotoacloud.top

PHP:  class Admin extends User {}
来源：http://oql.jqgufenzy.top

JS:   class Admin extends User {}
来源：http://shf.vehdjk.com

TS:   class Admin extends User {}
来源：http://lup.daxiang520.top

Java: class Admin extends User {}
来源：http://szr.fktsv.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ipr.9152youxi.cn

Ruby: class Admin < User; end
来源：http://jjm.pycfn.com

C#:   class Admin : User {}
来源：http://ngo.0kj1m.cn

[G06] 重写方法
来源：http://eew.xylfe.cn

Py:   def greet(self): return "admin"
来源：http://wyd.cdnleiting.top

PHP:  public function greet(): string { return "admin"; }
来源：http://rho.316326.xyz

JS:   greet() { return "admin"; }
来源：http://qjo.nwbrower.top

TS:   greet(): string { return "admin"; }
来源：http://izk.jinqigfzy.top

Java: @Override String greet() { return "admin"; }
来源：http://rfc.shanyushiyangkeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ges.yangfankeji.com

Ruby: def greet; "admin"; end
来源：http://brn.fanxiaobao.xyz

C#:   public override string Greet() => "admin";
来源：http://pwe.0kj1m.cn

[G07] 调用父类方法
来源：http://apr.birdmap.top

Py:   super().greet()
来源：http://qnd.0kj1m.cn

PHP:  parent::greet();
来源：http://ipo.jyoumei.cn

JS:   super.greet();
来源：http://kyt.wangshuangyany.cn

TS:   super.greet();
来源：http://nlr.ywan-chungtsiang.top

Java: super.greet();
来源：http://ies.cashguo.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://iuo.zhoulong.xyz

Ruby: super
来源：http://etr.ydjk.org.cn

C#:   base.Greet();
来源：http://tcw.wangshuangyany.cn

[G08] 静态方法与属性
来源：http://zuk.zhijiandao.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rtd.ydzc1.top

PHP:  public static function f() {}
来源：http://pew.zhixingplan.top

JS:   static f() {}
来源：http://tiy.tianlin.xyz

TS:   static f(): void {}
来源：http://utw.hammf.cn

Java: static void f() {}
来源：http://src.jinghuilouyu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ece.gaohongyu789.top

Ruby: def self.f; end
来源：http://oti.yanxiufei.cn

C#:   public static void F() {}
来源：http://lge.meibo888.top

[G09] 接口 / 抽象类
来源：http://ugi.guannengcc.top

Py:   from abc import ABC, abstractmethod
来源：http://epn.fktsv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gfs.sxryk.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tll.zhengqikj.top

TS:   interface Shape { area(): number; }
来源：http://mys.fanxiaobao.xyz

Java: interface Shape { double area(); }
来源：http://uwn.zhiwuduotai.top

Go:   type Shape interface { Area() float64 }
来源：http://pgo.yangfankeji.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uzi.yueranfly.top

C#:   interface IShape { double Area(); }
来源：http://elm.zdbjq.cn

[G10] 访问控制
来源：http://bpk.yj20258.top

Py:   约定 _protected / __private（不强制）
来源：http://ltn.xinyue.icu

PHP:  public / protected / private
来源：http://cxd.ydjk.org.cn

JS:   #private 字段；其余公开
来源：http://eee.yanxiufei.cn

TS:   public / protected / private
来源：http://orl.tanke756.top

Java: public / protected / private / 默认包级
来源：http://vfq.redwolf501.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://gcy.dianchejie.cn

Ruby: public / protected / private
来源：http://bix.zycfv.cn

C#:   public / protected / private / internal
来源：http://cyc.jyoumei.cn

[G11] getter / setter
来源：http://kbz.fengsongda.top

Py:   @property 与 @x.setter
来源：http://slo.xingfuxueyuan.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://xvr.ctjpmb.com

JS:   get name() { return this._name; }
来源：http://oth.jiagoushi.top

TS:   get name(): string { return this._name; }
来源：http://nao.quarkkingdee.top

Java: public String getName() { return name; }
来源：http://uis.nwbrower.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ljg.guowangkeji.top

Ruby: attr_accessor :name
来源：http://zqk.jinghuilouyu.cn

C#:   public string Name { get; set; }
来源：http://kui.birdmap.top

[G12] 对象转字符串
来源：http://sea.gzhubu.top

Py:   def __str__(self): return self.name
来源：http://oxs.ctjpmb.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://ing.nanxinkj.top

JS:   toString() { return this.name; }
来源：http://bov.ctjpmb.com

TS:   toString(): string { return this.name; }
来源：http://kmq.bjfxy.top

Java: @Override public String toString() { return name; }
来源：http://qut.xylfe.cn

Go:   func (u User) String() string { return u.Name }
来源：http://uyi.jqgfzy.top

Ruby: def to_s; @name; end
来源：http://zkr.ppjwa.cn

C#:   public override string ToString() => Name;
来源：http://mww.wangshuangyany.cn

[G13] 判断对象类型
来源：http://zyt.sysykeji.top

Py:   isinstance(u, User)
来源：http://qzv.ydzc1.top

PHP:  $u instanceof User
来源：http://ivl.quarkkingdee.top

JS:   u instanceof User
来源：http://kdd.fehbvm.com

TS:   u instanceof User
来源：http://kdv.andypj.xyz

Java: u instanceof User
来源：http://ucu.jinghuilouyu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://iqb.ehwqpu.com

Ruby: u.is_a?(User)
来源：http://iex.fehbvm.com

C#:   u is User
来源：http://aje.chenjidiqi.icu

[G14] 数据类 / record
来源：http://usp.fehbvm.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ggj.hywenlv.cn

PHP:  // 用 readonly 属性模拟
来源：http://dwe.jianghu66.top

JS:   // 无内置：普通类或对象字面量
来源：http://aux.hammf.cn

TS:   type User = { name: string; age: number };
来源：http://ymq.sweek.top

Java: record User(String name, int age) {}
来源：http://iap.zhiwuduotai.top

Go:   type User struct { Name string; Age int }
来源：http://tcy.iojbl.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ygc.sufxvd.cn

C#:   record User(string Name, int Age);
来源：http://gmb.birdmap.top

[G15] 枚举
来源：http://cwc.jlsjyb.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xoa.jinqigfzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://one.yonumen.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vmd.epnwcf.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dap.epnwcf.com

Java: enum Color { RED, GREEN }
来源：http://kdz.ybcxt.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dsw.zhaomingkeji.xyz

Ruby: Color = %i[red green].freeze
来源：http://yif.hfpthk.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://eud.hongshengwenyu.top

[G16] 对象转数组 / 字典
来源：http://hvu.gotoacloud.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vck.hnqzz.top

PHP:  get_object_vars($obj);
来源：http://jri.shanyushiyangtech.top

JS:   Object.entries(obj)
来源：http://vjm.daxiang520.top

TS:   Object.entries(obj)
来源：http://rlr.pengpengdd.cyou

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qyf.yj20258888.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://nbc.daria6918.cn

Ruby: obj.instance_variables
来源：http://owe.snrcjt.cn

C#:   // 用反射或 System.Text.Json
来源：http://exf.wangdashe.top

================================================================================
来源：http://dfn.sjlbkw.cn

H. 异常与错误处理
来源：http://pgk.hongshengwenyu.top

================================================================================
来源：http://ekh.aizwys.cn

[H01] try / catch 基础
来源：http://pkt.vehdjk.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bbv.guowangkeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://osp.sjlbkw.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lgl.shuidangran.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kyi.guannengcc.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sff.jianghu66.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vko.gaohongyu789.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ijp.vehdjk.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hsz.hesvh.cn

[H02] finally / ensure 收尾
来源：http://ebn.0kj1m.cn

Py:   try: f()⏎finally: cleanup()
来源：http://cas.52xcode.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://njn.daria6918.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qbs.guannengcc.top

TS:   try { f(); } finally { cleanup(); }
来源：http://uvz.hammf.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qta.jqgufenzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://nqi.cdnleiting.top

Ruby: begin; f; ensure; cleanup; end
来源：http://iwr.hfpthk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ohp.zhaomingkeji.xyz

[H03] 主动抛出异常
来源：http://yec.epnwcf.com

Py:   raise ValueError("错误信息")
来源：http://nrn.zhoulong.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ejj.aizwys.cn

JS:   throw new Error("错误信息");
来源：http://mji.hongshengwenyu.top

TS:   throw new Error("错误信息");
来源：http://rzu.redwolf501.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ean.tian-w.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://phn.zdbjq.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ljn.shzxlz.cn

C#:   throw new ArgumentException("错误信息");
来源：http://uvr.havefunace.top

[H04] 自定义异常类型
来源：http://mdn.9152youxi.cn

Py:   class MyError(Exception): pass
来源：http://psy.yuxming.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mol.zhijiandao.cn

JS:   class MyError extends Error {}
来源：http://tlx.epnwcf.com

TS:   class MyError extends Error {}
来源：http://gns.jiagoushi.top

Java: class MyException extends RuntimeException {}
来源：http://cov.havefunace.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mkr.hnxiangtu.top

Ruby: class MyError < StandardError; end
来源：http://csn.andypj.xyz

C#:   class MyException : Exception {}
来源：http://trn.gotoacloud.top

[H05] 捕获特定类型
来源：http://pzg.fehbvm.com

Py:   except ValueError as e:
来源：http://lyw.zdbjq.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yen.guannengcc.top

JS:   if (e instanceof TypeError) {}
来源：http://mot.zhijiandao.cn

TS:   if (e instanceof TypeError) {}
来源：http://gmg.zhixingplan.top

Java: catch (IOException | SQLException e) {}
来源：http://aco.dashuyun.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rjm.tanke756.top

Ruby: rescue ArgumentError => e
来源：http://afb.feifeiyinyue.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ucq.yanxiufei.cn

[H06] 可选值 / 空值安全访问
来源：http://fdy.yueranfly.top

Py:   value = d.get("k") or default
来源：http://oqz.vehdjk.com

PHP:  $v = $d["k"] ?? null;
来源：http://iqv.hesvh.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hak.nanxuanxn.top

TS:   obj?.a?.b;  d ?? default
来源：http://eft.daxiang520.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yjo.wangdashe.top

Go:   if v, ok := m["k"]; ok { }
来源：http://muz.fktsv.cn

Ruby: d&.dig(:a, :b)
来源：http://pvy.daxiang520.top

C#:   obj?.A?.B ?? default
来源：http://qir.jinghuilouyu.cn

[H07] 断言
来源：http://sbm.yuanzhike.top

Py:   assert x > 0, "必须为正"
来源：http://hlz.aizwys.cn

PHP:  assert($x > 0);
来源：http://nur.epnwcf.com

JS:   console.assert(x > 0);
来源：http://ogr.epnwcf.com

TS:   console.assert(x > 0);
来源：http://azb.zycfv.cn

Java: assert x > 0 : "必须为正";
来源：http://uro.yueranfly.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nom.hongshengwenyu.top

Ruby: raise "必须为正" unless x > 0
来源：http://jpo.ctjpmb.com

C#:   Debug.Assert(x > 0);
来源：http://ktf.nanxinkj.top

[H08] 获取错误信息与堆栈
来源：http://ujj.aibaodan.cn

Py:   str(e);  traceback.format_exc()
来源：http://bmi.shzxlz.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gvv.shzxlz.cn

JS:   e.message;  e.stack
来源：http://mjl.zhoulong.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://ikn.aibaodan.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tvo.fanxiaobao.xyz

Go:   err.Error()
来源：http://aeh.yonumen.top

Ruby: e.message;  e.backtrace
来源：http://nab.yj20258.top

C#:   e.Message;  e.StackTrace
来源：http://rgf.guannengcc.top

[H09] 带错误码的异常
来源：http://zmw.shanyushiyangtech.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qom.shanyushiyangtech.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://dgh.gzhubu.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sku.zhijiandao.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hbh.jinghuilouyu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dcm.pycfn.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vxe.hesvh.cn

Ruby: raise MyError.new("fail", 500)
来源：http://lwl.fzhhl.top

C#:   // 自定义异常类中加 Code 属性
来源：http://mxp.tianlin.xyz

[H10] 资源自动释放
来源：http://hto.ctjpmb.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://cxy.chenjidiqi.icu

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lyj.hcnkem.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bzv.ydzc1.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ikk.nanxinkj.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bbw.yuxming.cn

Go:   defer f.Close()
来源：http://llx.shanyushiyangkeji.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ral.daxiang520.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ejb.yanxiufei.cn

================================================================================
来源：http://sgj.yj202588.top

I. 正则表达式
来源：http://eji.guannengcc.top

================================================================================
来源：http://jmq.smart0.xyz

[I01] 判断是否匹配
来源：http://shm.jinyuanbaomall.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://low.tian-w.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nrt.guannengcc.top

JS:   /\d+/.test(s)
来源：http://rpl.sufxvd.cn

TS:   /\d+/.test(s)
来源：http://dof.sxryk.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jpv.9152youxi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fuk.birdmap.top

Ruby: s.match?(/\d+/)
来源：http://ymy.zhixingplan.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rrw.haohaochexian.top

[I02] 提取所有匹配
来源：http://drq.hesvh.cn

Py:   re.findall(r"\d+", s)
来源：http://kun.zdqjudy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cer.xuanzx.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xzq.bjfxy.top

TS:   s.match(/\d+/g)
来源：http://mfs.zhongyouzk.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yeh.feifeiyinyue.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://htg.zhongyouzk.top

Ruby: s.scan(/\d+/)
来源：http://mea.hfpthk.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xgn.wangdashe.top

[I03] 提取捕获分组
来源：http://vkz.ywan-chungtsiang.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nwo.dianchejie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cgc.svipenyu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xvx.ydjk.org.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bey.gogol.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://opi.jianghu66.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mgj.tianlin.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xbc.redwolf501.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mwh.ctjpmb.com

[I04] 正则替换
来源：http://mgr.yangfankeji.com

Py:   re.sub(r"\d+", "#", s)
来源：http://pqw.mhx1999.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nyd.sysykeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://ats.dashuyun.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rwj.xuetiantiany.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wja.yvedp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wbj.cashguo.top

Ruby: s.gsub(/\d+/, "#")
来源：http://bgf.xingfuxueyuan.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dzx.chenzaomai.com

[I05] 按正则拆分
来源：http://qfs.snrcjt.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wxg.vehdjk.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uqz.bbcook.cn

JS:   s.split(/\s*,\s*/)
来源：http://dya.yonumen.top

TS:   s.split(/\s*,\s*/)
来源：http://qyj.gotoacloud.top

Java: s.split("\\s*,\\s*")
来源：http://nes.ctjpmb.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jap.zdqjudy.top

Ruby: s.split(/\s*,\s*/)
来源：http://yun.zhongyouzk.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yyo.52xcode.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jsa.vehdjk.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zis.cqqwz.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nmh.zdbjq.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yfo.tarul.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vbg.gaohongyu789.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kcg.fktsv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wgl.shuidangran.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://aea.snrcjt.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qqr.yvedp.cn

[I07] 忽略大小写与多行模式
来源：http://nbk.nwbrower.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://iuf.yvedp.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wlz.vqdsnc.cn


<!-- 参考信息 -->