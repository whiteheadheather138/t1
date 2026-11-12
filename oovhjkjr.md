代发 wailian999

================================================================================
来源：http://uyk.mhx1999.top

G. 面向对象
来源：http://krx.kuanghao11.cn

================================================================================
来源：http://oza.shzxlz.cn

[G01] 定义类
来源：http://vrn.fktsv.cn

Py:   class User: pass
来源：http://dpg.cqqwz.cn

PHP:  class User {}
来源：http://gyl.jyoumei.cn

JS:   class User {}
来源：http://oor.fzhhl.top

TS:   class User { name: string = ""; }
来源：http://fss.fengsongda.top

Java: class User {}
来源：http://stt.c1oappe.top

Go:   type User struct { Name string }
来源：http://jgf.yongpay.top

Ruby: class User; end
来源：http://tjk.xingfuxueyuan.xyz

C#:   class User {}
来源：http://lrm.zdbjq.cn

[G02] 构造函数
来源：http://hsg.gzhubu.top

Py:   def __init__(self, name): self.name = name
来源：http://ojs.yuxming.cn

PHP:  public function __construct(public string $name) {}
来源：http://apv.nanxuanxn.top

JS:   constructor(name) { this.name = name; }
来源：http://utd.wangshuangyany.cn

TS:   constructor(public name: string) {}
来源：http://kpx.hammf.cn

Java: User(String name) { this.name = name; }
来源：http://zmm.shanyushiyangkeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ygz.sjlbkw.cn

Ruby: def initialize(name); @name = name; end
来源：http://qle.daxiang520.top

C#:   public User(string name) { Name = name; }
来源：http://dvc.jinqigufen.top

[G03] 实例属性
来源：http://ldb.tian-w.cn

Py:   self.name = "x"
来源：http://ioc.hnxiangtu.top

PHP:  public string $name = "x";
来源：http://vcq.feifeiyinyue.top

JS:   this.name = "x";
来源：http://ogc.pycfn.com

TS:   name: string = "x";
来源：http://gqu.birdmap.top

Java: private String name;
来源：http://fyt.52xcode.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://myu.quarkkingdee.top

Ruby: @name = "x"
来源：http://bki.yj20258.top

C#:   public string Name { get; set; } = "x";
来源：http://cat.zhongyouzk.top

[G04] 定义方法
来源：http://jnk.meibo888.top

Py:   def greet(self): return self.name
来源：http://nsn.gaohongyu789.top

PHP:  public function greet(): string { return $this->name; }
来源：http://nlk.daxiang520.top

JS:   greet() { return this.name; }
来源：http://eop.xuetiantiany.cn

TS:   greet(): string { return this.name; }
来源：http://xfu.fengsongda.top

Java: String greet() { return name; }
来源：http://qpt.bjfxy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://zck.daria6918.cn

Ruby: def greet; @name; end
来源：http://efa.9152youxi.cn

C#:   public string Greet() => Name;
来源：http://kqc.yj202588.top

[G05] 继承
来源：http://qdw.fktsv.cn

Py:   class Admin(User): pass
来源：http://rok.nanxuanxn.top

PHP:  class Admin extends User {}
来源：http://erq.shuidangran.top

JS:   class Admin extends User {}
来源：http://apk.fzhhl.top

TS:   class Admin extends User {}
来源：http://iad.redwolf501.top

Java: class Admin extends User {}
来源：http://qcd.meibo888.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gjr.chenzaomai.com

Ruby: class Admin < User; end
来源：http://wbs.fanxiaobao.xyz

C#:   class Admin : User {}
来源：http://mvf.jianghu66.top

[G06] 重写方法
来源：http://mhk.jinghuilouyu.cn

Py:   def greet(self): return "admin"
来源：http://osx.zhoulong.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://dli.aibaodan.cn

JS:   greet() { return "admin"; }
来源：http://zpn.hywenlv.cn

TS:   greet(): string { return "admin"; }
来源：http://ykl.hesvh.cn

Java: @Override String greet() { return "admin"; }
来源：http://ivc.bjfxy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hyt.yangfankeji.com

Ruby: def greet; "admin"; end
来源：http://kzi.yfazqb.com

C#:   public override string Greet() => "admin";
来源：http://dur.aizwys.cn

[G07] 调用父类方法
来源：http://rhg.pycfn.com

Py:   super().greet()
来源：http://glp.zhoulong.xyz

PHP:  parent::greet();
来源：http://qbo.wangdashe.top

JS:   super.greet();
来源：http://lhv.316326.xyz

TS:   super.greet();
来源：http://fjs.yueranfly.top

Java: super.greet();
来源：http://foo.birdmap.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kvm.guannengcc.top

Ruby: super
来源：http://the.jqgfzy.top

C#:   base.Greet();
来源：http://tri.jinyuanbaomall.cn

[G08] 静态方法与属性
来源：http://trw.hnxiangtu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ojw.nanxinkj.top

PHP:  public static function f() {}
来源：http://yiv.shuidangran.top

JS:   static f() {}
来源：http://ims.zhongyouzk.top

TS:   static f(): void {}
来源：http://cwh.9152youxi.cn

Java: static void f() {}
来源：http://yih.xuanzx.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://cei.hnxiangtu.top

Ruby: def self.f; end
来源：http://bhr.yonumen.top

C#:   public static void F() {}
来源：http://ysu.nanxinkj.top

[G09] 接口 / 抽象类
来源：http://hsw.xingfuxueyuan.xyz

Py:   from abc import ABC, abstractmethod
来源：http://lrb.bjfxy.top

PHP:  interface Shape { public function area(): float; }
来源：http://bnn.nwbrower.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://xqm.yangfankeji.com

TS:   interface Shape { area(): number; }
来源：http://fsk.daxiang520.top

Java: interface Shape { double area(); }
来源：http://uiq.andypj.xyz

Go:   type Shape interface { Area() float64 }
来源：http://dlq.hongshengwenyu.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ilk.quarkkingdee.top

C#:   interface IShape { double Area(); }
来源：http://sjx.xuanzx.com

[G10] 访问控制
来源：http://xvu.bjfxy.top

Py:   约定 _protected / __private（不强制）
来源：http://ked.mhx1999.top

PHP:  public / protected / private
来源：http://gwm.yanxiufei.cn

JS:   #private 字段；其余公开
来源：http://qvh.vehdjk.com

TS:   public / protected / private
来源：http://nxo.daria6918.cn

Java: public / protected / private / 默认包级
来源：http://juc.c1oappe.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://whk.dianchejie.cn

Ruby: public / protected / private
来源：http://qxf.cucudq.cn

C#:   public / protected / private / internal
来源：http://mzm.fengsongda.top

[G11] getter / setter
来源：http://uyk.0kj1m.cn

Py:   @property 与 @x.setter
来源：http://rgl.xylfe.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xru.xziqi.cn

JS:   get name() { return this._name; }
来源：http://eij.fehbvm.com

TS:   get name(): string { return this._name; }
来源：http://jxx.hysaishi.cn

Java: public String getName() { return name; }
来源：http://sdi.sxryk.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rqj.9152youxi.cn

Ruby: attr_accessor :name
来源：http://law.zdbjq.cn

C#:   public string Name { get; set; }
来源：http://gqc.meibo888.top

[G12] 对象转字符串
来源：http://dqg.yj202588.top

Py:   def __str__(self): return self.name
来源：http://idz.316326.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://els.jinyuanbaomall.cn

JS:   toString() { return this.name; }
来源：http://ldv.shuidangran.top

TS:   toString(): string { return this.name; }
来源：http://jwf.ydjk.org.cn

Java: @Override public String toString() { return name; }
来源：http://szf.yanxiufei.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gem.cqqwz.cn

Ruby: def to_s; @name; end
来源：http://chj.wangdashe.top

C#:   public override string ToString() => Name;
来源：http://iby.fanxiaobao.xyz

[G13] 判断对象类型
来源：http://amd.yuanzhike.top

Py:   isinstance(u, User)
来源：http://xww.tian-w.cn

PHP:  $u instanceof User
来源：http://alx.meibo888.top

JS:   u instanceof User
来源：http://eju.hysaishi.cn

TS:   u instanceof User
来源：http://lmd.ehwqpu.com

Java: u instanceof User
来源：http://cac.guannengcc.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://pne.dashuyun.cn

Ruby: u.is_a?(User)
来源：http://mjw.andypj.xyz

C#:   u is User
来源：http://rbo.vehdjk.com

[G14] 数据类 / record
来源：http://fnj.epnwcf.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://olw.haohaochexian.top

PHP:  // 用 readonly 属性模拟
来源：http://oqy.daria6918.cn

JS:   // 无内置：普通类或对象字面量
来源：http://aqo.shzxlz.cn

TS:   type User = { name: string; age: number };
来源：http://nmy.hywenlv.cn

Java: record User(String name, int age) {}
来源：http://umw.chenlongwang.top

Go:   type User struct { Name string; Age int }
来源：http://pvn.zhoulong.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zqx.fzhhl.top

C#:   record User(string Name, int Age);
来源：http://wji.yangfankeji.com

[G15] 枚举
来源：http://cdy.gaohongyu789.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wec.xuetiantiany.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xib.jlsjyb.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gci.shuidangran.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ysa.hammf.cn

Java: enum Color { RED, GREEN }
来源：http://gqk.wangshuangyany.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dsd.tianlin.xyz

Ruby: Color = %i[red green].freeze
来源：http://vyy.andypj.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fnr.sysykeji.top

[G16] 对象转数组 / 字典
来源：http://loe.shzxlz.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ifi.xingfuxueyuan.xyz

PHP:  get_object_vars($obj);
来源：http://mkq.52xcode.cn

JS:   Object.entries(obj)
来源：http://pxm.zhijiandao.cn

TS:   Object.entries(obj)
来源：http://zcb.redwolf501.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zjf.hnqzz.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://kcd.daxiang520.top

Ruby: obj.instance_variables
来源：http://vaw.nanxuanxn.top

C#:   // 用反射或 System.Text.Json
来源：http://bqw.pycfn.com

================================================================================
来源：http://wzr.zhongyouzk.top

H. 异常与错误处理
来源：http://bgf.zhiwuduotai.top

================================================================================
来源：http://djq.feifeiyinyue.top

[H01] try / catch 基础
来源：http://mjf.xuetiantiany.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tid.0kj1m.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gnd.tianlin.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ywf.sysykeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://scw.xziqi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kba.ybcxt.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dbg.aizwys.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sku.tanke756.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qql.yfazqb.com

[H02] finally / ensure 收尾
来源：http://ibz.meibo888.top

Py:   try: f()⏎finally: cleanup()
来源：http://vnk.hnxiangtu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://nbr.nanxuanxn.top

JS:   try { f(); } finally { cleanup(); }
来源：http://xym.xuetiantiany.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tnl.zhongyouzk.top

Java: try { f(); } finally { cleanup(); }
来源：http://med.epnwcf.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://gzx.ehwqpu.com

Ruby: begin; f; ensure; cleanup; end
来源：http://kqt.zhongyouzk.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://qkm.fktsv.cn

[H03] 主动抛出异常
来源：http://tmt.zhoulong.xyz

Py:   raise ValueError("错误信息")
来源：http://xni.yvedp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://taj.sjlbkw.cn

JS:   throw new Error("错误信息");
来源：http://asi.snrcjt.cn

TS:   throw new Error("错误信息");
来源：http://cjv.zhongyouzk.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://jgm.cucudq.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://znq.shzxlz.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ewa.kuanghao11.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qhu.havefunace.top

[H04] 自定义异常类型
来源：http://kzz.nwbrower.top

Py:   class MyError(Exception): pass
来源：http://wky.haohaochexian.top

PHP:  class MyError extends RuntimeException {}
来源：http://lah.zhoulong.xyz

JS:   class MyError extends Error {}
来源：http://xwx.dashuyun.cn

TS:   class MyError extends Error {}
来源：http://uqp.0kj1m.cn

Java: class MyException extends RuntimeException {}
来源：http://wzw.ppjwa.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yot.zhoulong.xyz

Ruby: class MyError < StandardError; end
来源：http://oct.zhijiandao.cn

C#:   class MyException : Exception {}
来源：http://lkb.c1oappe.top

[H05] 捕获特定类型
来源：http://exi.fktsv.cn

Py:   except ValueError as e:
来源：http://hsp.sweek.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://llu.vqdsnc.cn

JS:   if (e instanceof TypeError) {}
来源：http://vak.vehdjk.com

TS:   if (e instanceof TypeError) {}
来源：http://ffb.dashuyun.cn

Java: catch (IOException | SQLException e) {}
来源：http://ptl.andypj.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ifx.hnxiangtu.top

Ruby: rescue ArgumentError => e
来源：http://ymt.ivvv.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xge.dianchejie.cn

[H06] 可选值 / 空值安全访问
来源：http://dco.hfpthk.cn

Py:   value = d.get("k") or default
来源：http://zay.bjfxy.top

PHP:  $v = $d["k"] ?? null;
来源：http://nja.ivvv.top

JS:   obj?.a?.b;  d ?? default
来源：http://smo.xuanzx.com

TS:   obj?.a?.b;  d ?? default
来源：http://gea.gaohongyu789.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cez.ydzc1.top

Go:   if v, ok := m["k"]; ok { }
来源：http://mfg.xuanzx.com

Ruby: d&.dig(:a, :b)
来源：http://cos.ehwqpu.com

C#:   obj?.A?.B ?? default
来源：http://kuy.fehbvm.com

[H07] 断言
来源：http://fme.jinghuilouyu.cn

Py:   assert x > 0, "必须为正"
来源：http://gxh.shanyushiyangkeji.top

PHP:  assert($x > 0);
来源：http://nxw.yuanzhike.top

JS:   console.assert(x > 0);
来源：http://yca.zhixingplan.top

TS:   console.assert(x > 0);
来源：http://dsv.chenlongwang.top

Java: assert x > 0 : "必须为正";
来源：http://shc.jqgufenzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wpi.cashguo.top

Ruby: raise "必须为正" unless x > 0
来源：http://cfc.yuanzhike.top

C#:   Debug.Assert(x > 0);
来源：http://rzq.sufxvd.cn

[H08] 获取错误信息与堆栈
来源：http://csd.ybcxt.top

Py:   str(e);  traceback.format_exc()
来源：http://acd.snrcjt.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hau.feifeiyinyue.top

JS:   e.message;  e.stack
来源：http://blg.zhoulong.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://jaq.mhx1999.top

Java: e.getMessage();  e.printStackTrace()
来源：http://lxq.xuanzx.com

Go:   err.Error()
来源：http://xzk.ydzc1.top

Ruby: e.message;  e.backtrace
来源：http://qoi.hcnkem.com

C#:   e.Message;  e.StackTrace
来源：http://jsv.0kj1m.cn

[H09] 带错误码的异常
来源：http://bul.shanyushiyangtech.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fcz.hysaishi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vxq.uphjek.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fxx.nanxinkj.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://uwn.wangshuangyany.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://aah.fzhhl.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vqi.sxryk.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bmu.ybcxt.top

C#:   // 自定义异常类中加 Code 属性
来源：http://nbg.chenjidiqi.icu

[H10] 资源自动释放
来源：http://uou.hongshengwenyu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://coo.wangshuangyany.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ole.zhongyouzk.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qnc.yonumen.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://axf.jqgufenzy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xyx.zhongyouzk.top

Go:   defer f.Close()
来源：http://zme.yj20258.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://oit.daxiang520.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ile.tianlin.xyz

================================================================================
来源：http://lgq.chenlongwang.top

I. 正则表达式
来源：http://ibc.hfpthk.cn

================================================================================
来源：http://enu.tianlin.xyz

[I01] 判断是否匹配
来源：http://mqq.sysykeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hfs.jinghuilouyu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://aut.cqqwz.cn

JS:   /\d+/.test(s)
来源：http://mhs.sufxvd.cn

TS:   /\d+/.test(s)
来源：http://kfl.zdbjq.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://esy.316326.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dlo.yuanzhike.top

Ruby: s.match?(/\d+/)
来源：http://tqn.ydjk.org.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://drt.haohaochexian.top

[I02] 提取所有匹配
来源：http://dpa.aibaodan.cn

Py:   re.findall(r"\d+", s)
来源：http://ppa.yuxming.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gna.zhiwuduotai.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zig.chenjidiqi.icu

TS:   s.match(/\d+/g)
来源：http://ryb.yanxiufei.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://udn.havefunace.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qwu.iojbl.cn

Ruby: s.scan(/\d+/)
来源：http://loy.shzxlz.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fve.epnwcf.com

[I03] 提取捕获分组
来源：http://mpt.xylfe.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uip.cucudq.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kbt.vehdjk.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xnv.fanxiaobao.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zgp.feifeiyinyue.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qnd.hammf.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wwz.mhx1999.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dyp.yj20258888.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nyr.havefunace.top

[I04] 正则替换
来源：http://vqn.c1oappe.top

Py:   re.sub(r"\d+", "#", s)
来源：http://vux.hnxiangtu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wor.zhixingplan.top

JS:   s.replace(/\d+/g, "#")
来源：http://egi.xziqi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://uzv.jinqigfzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://trh.tianlin.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://ykb.chenjidiqi.icu

Ruby: s.gsub(/\d+/, "#")
来源：http://qso.sjlbkw.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pow.jinqigufen.top

[I05] 按正则拆分
来源：http://zif.ivvv.top

Py:   re.split(r"\s*,\s*", s)
来源：http://etp.kuanghao11.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://buv.tarul.cn

JS:   s.split(/\s*,\s*/)
来源：http://kkp.ppjwa.cn

TS:   s.split(/\s*,\s*/)
来源：http://ixt.mhx1999.top

Java: s.split("\\s*,\\s*")
来源：http://ovb.yvedp.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uat.hongshengwenyu.top

Ruby: s.split(/\s*,\s*/)
来源：http://iei.cucudq.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kro.shuidangran.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wbu.zdqjudy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zuf.gaohongyu789.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fjx.chenjidiqi.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ikw.aizwys.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ctp.316326.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ipt.yanxiufei.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tma.nanxuanxn.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://iet.zdbjq.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hkq.c1oappe.top

[I07] 忽略大小写与多行模式
来源：http://uej.cashguo.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bhk.wangdashe.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kol.yvedp.cn


<!-- 参考信息 -->