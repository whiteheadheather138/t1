代发 wailian999

Java: class User {}
来源：http://unt.zhaomingkeji.xyz

Go:   type User struct { Name string }
来源：http://mjn.hnqzz.top

Ruby: class User; end
来源：http://zlc.yvedp.cn

C#:   class User {}
来源：http://hdv.cucudq.cn

[G02] 构造函数
来源：http://rek.sysykeji.top

Py:   def __init__(self, name): self.name = name
来源：http://uso.hcnkem.com

PHP:  public function __construct(public string $name) {}
来源：http://wyy.jinyuanbaomall.cn

JS:   constructor(name) { this.name = name; }
来源：http://aqt.yanxiufei.cn

TS:   constructor(public name: string) {}
来源：http://ksm.uphjek.com

Java: User(String name) { this.name = name; }
来源：http://pfi.wangdashe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://spf.havefunace.top

Ruby: def initialize(name); @name = name; end
来源：http://kdm.sufxvd.cn

C#:   public User(string name) { Name = name; }
来源：http://qii.vqdsnc.cn

[G03] 实例属性
来源：http://evm.aizwys.cn

Py:   self.name = "x"
来源：http://fks.0kj1m.cn

PHP:  public string $name = "x";
来源：http://jja.ppjwa.cn

JS:   this.name = "x";
来源：http://zti.shanyushiyangkeji.top

TS:   name: string = "x";
来源：http://wzd.kuanghao11.cn

Java: private String name;
来源：http://hzv.hnqzz.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uyg.yj20258.top

Ruby: @name = "x"
来源：http://mtt.hysaishi.cn

C#:   public string Name { get; set; } = "x";
来源：http://sum.hnxiangtu.top

[G04] 定义方法
来源：http://kak.xuanzx.com

Py:   def greet(self): return self.name
来源：http://gll.sxryk.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ztm.fengsongda.top

JS:   greet() { return this.name; }
来源：http://hbl.dianchejie.cn

TS:   greet(): string { return this.name; }
来源：http://wom.hammf.cn

Java: String greet() { return name; }
来源：http://qgz.shanyushiyangtech.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://dot.kuanghao11.cn

Ruby: def greet; @name; end
来源：http://nju.52xcode.cn

C#:   public string Greet() => Name;
来源：http://qxm.yj20258888.top

[G05] 继承
来源：http://fei.sweek.top

Py:   class Admin(User): pass
来源：http://qzc.hammf.cn

PHP:  class Admin extends User {}
来源：http://rca.ehwqpu.com

JS:   class Admin extends User {}
来源：http://fqz.chenzaomai.com

TS:   class Admin extends User {}
来源：http://hqt.0kj1m.cn

Java: class Admin extends User {}
来源：http://rmm.chenzaomai.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uuq.jqgufenzy.top

Ruby: class Admin < User; end
来源：http://qss.kuanghao11.cn

C#:   class Admin : User {}
来源：http://rac.jqgufenzy.top

[G06] 重写方法
来源：http://ofy.tian-w.cn

Py:   def greet(self): return "admin"
来源：http://ttn.smart0.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://qfe.xziqi.cn

JS:   greet() { return "admin"; }
来源：http://wwv.shangyingyoupin.top

TS:   greet(): string { return "admin"; }
来源：http://zvp.bjfxy.top

Java: @Override String greet() { return "admin"; }
来源：http://gam.fehbvm.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ati.svipenyu.cn

Ruby: def greet; "admin"; end
来源：http://qqv.0kj1m.cn

C#:   public override string Greet() => "admin";
来源：http://uqj.yueranfly.top

[G07] 调用父类方法
来源：http://ztb.hywenlv.cn

Py:   super().greet()
来源：http://nts.aizwys.cn

PHP:  parent::greet();
来源：http://tnv.yueranfly.top

JS:   super.greet();
来源：http://sab.fanxiaobao.xyz

TS:   super.greet();
来源：http://dhn.cucudq.cn

Java: super.greet();
来源：http://qzq.hywenlv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nkt.yangfankeji.com

Ruby: super
来源：http://npu.yangfankeji.com

C#:   base.Greet();
来源：http://css.xinyue.icu

[G08] 静态方法与属性
来源：http://ylg.cucudq.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jnj.hcnkem.com

PHP:  public static function f() {}
来源：http://roi.tian-w.cn

JS:   static f() {}
来源：http://uza.yueranfly.top

TS:   static f(): void {}
来源：http://qwu.iojbl.cn

Java: static void f() {}
来源：http://ymh.xinyue.icu

Go:   // 无 static：用包级函数，按包名调用
来源：http://xqx.xuetiantiany.cn

Ruby: def self.f; end
来源：http://hka.xuanzx.com

C#:   public static void F() {}
来源：http://erk.fktsv.cn

[G09] 接口 / 抽象类
来源：http://pvn.dianchejie.cn

Py:   from abc import ABC, abstractmethod
来源：http://dfg.nanxuanxn.top

PHP:  interface Shape { public function area(): float; }
来源：http://qeq.chenlongwang.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://vrn.daxiang520.top

TS:   interface Shape { area(): number; }
来源：http://jsw.haohaochexian.top

Java: interface Shape { double area(); }
来源：http://apx.zdqjudy.top

Go:   type Shape interface { Area() float64 }
来源：http://eyq.redwolf501.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sim.hfpthk.cn

C#:   interface IShape { double Area(); }
来源：http://ahf.fktsv.cn

[G10] 访问控制
来源：http://ifa.fzhhl.top

Py:   约定 _protected / __private（不强制）
来源：http://sqk.tianlin.xyz

PHP:  public / protected / private
来源：http://kkt.zhengqikj.top

JS:   #private 字段；其余公开
来源：http://aty.fengsongda.top

TS:   public / protected / private
来源：http://oux.havefunace.top

Java: public / protected / private / 默认包级
来源：http://wdc.xuanzx.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://ukf.jianghu66.top

Ruby: public / protected / private
来源：http://tvg.hnqzz.top

C#:   public / protected / private / internal
来源：http://qqm.jinghuilouyu.cn

[G11] getter / setter
来源：http://clt.tianlin.xyz

Py:   @property 与 @x.setter
来源：http://jus.hammf.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://rff.jlsjyb.cn

JS:   get name() { return this._name; }
来源：http://xmh.tian-w.cn

TS:   get name(): string { return this._name; }
来源：http://qfr.pycfn.com

Java: public String getName() { return name; }
来源：http://jaq.gzhubu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://vhn.tianlin.xyz

Ruby: attr_accessor :name
来源：http://wnk.xziqi.cn

C#:   public string Name { get; set; }
来源：http://ype.shanyushiyangtech.top

[G12] 对象转字符串
来源：http://shq.yanxiufei.cn

Py:   def __str__(self): return self.name
来源：http://naj.ydzc1.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://hwc.zhongyouzk.top

JS:   toString() { return this.name; }
来源：http://mwu.9152youxi.cn

TS:   toString(): string { return this.name; }
来源：http://ixm.cashguo.top

Java: @Override public String toString() { return name; }
来源：http://ywt.daxiang520.top

Go:   func (u User) String() string { return u.Name }
来源：http://usw.chenlongwang.top

Ruby: def to_s; @name; end
来源：http://ptr.kuanghao11.cn

C#:   public override string ToString() => Name;
来源：http://won.pycfn.com

[G13] 判断对象类型
来源：http://epr.chenlongwang.top

Py:   isinstance(u, User)
来源：http://vvn.zhongyouzk.top

PHP:  $u instanceof User
来源：http://rjy.aibaodan.cn

JS:   u instanceof User
来源：http://mie.shuidangran.top

TS:   u instanceof User
来源：http://eyl.zhaomingkeji.xyz

Java: u instanceof User
来源：http://oqu.ctjpmb.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://pju.tianlin.xyz

Ruby: u.is_a?(User)
来源：http://kkc.yfazqb.com

C#:   u is User
来源：http://gxv.jinqigufen.top

[G14] 数据类 / record
来源：http://ovb.xingfuxueyuan.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bye.nanxinkj.top

PHP:  // 用 readonly 属性模拟
来源：http://wjx.aibaodan.cn

JS:   // 无内置：普通类或对象字面量
来源：http://clo.shuidangran.top

TS:   type User = { name: string; age: number };
来源：http://gcr.tanke756.top

Java: record User(String name, int age) {}
来源：http://aak.birdmap.top

Go:   type User struct { Name string; Age int }
来源：http://jxz.52xcode.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rjq.nanxuanxn.top

C#:   record User(string Name, int Age);
来源：http://eod.bbcook.cn

[G15] 枚举
来源：http://krk.gotoacloud.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vhf.yfazqb.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://crk.mhx1999.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nbl.hfpthk.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vgy.guannengcc.top

Java: enum Color { RED, GREEN }
来源：http://fvq.ppjwa.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jpg.cucudq.cn

Ruby: Color = %i[red green].freeze
来源：http://egm.shangyingyoupin.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ioa.vehdjk.com

[G16] 对象转数组 / 字典
来源：http://wnf.jyoumei.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://skb.hongshengwenyu.top

PHP:  get_object_vars($obj);
来源：http://ijl.fzhhl.top

JS:   Object.entries(obj)
来源：http://igj.chenjidiqi.icu

TS:   Object.entries(obj)
来源：http://mhj.havefunace.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xxj.guowangkeji.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://mya.fehbvm.com

Ruby: obj.instance_variables
来源：http://dwf.shzxlz.cn

C#:   // 用反射或 System.Text.Json
来源：http://rhs.ybcxt.top

================================================================================
来源：http://ztz.hcnkem.com

H. 异常与错误处理
来源：http://sqk.bjfxy.top

================================================================================
来源：http://ekk.zdqjudy.top

[H01] try / catch 基础
来源：http://nfe.cheryme.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hsy.vehdjk.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vmk.zhijiandao.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://iyd.zycfv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xcm.dashuyun.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xsp.ydzc1.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://prd.zdqjudy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wio.bbcook.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ywq.havefunace.top

[H02] finally / ensure 收尾
来源：http://scc.meibo888.top

Py:   try: f()⏎finally: cleanup()
来源：http://olm.ehwqpu.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://kyv.yfazqb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://iss.c1oappe.top

TS:   try { f(); } finally { cleanup(); }
来源：http://oob.yueranfly.top

Java: try { f(); } finally { cleanup(); }
来源：http://coq.haohaochexian.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://dcy.ehwqpu.com

Ruby: begin; f; ensure; cleanup; end
来源：http://qfr.yueranfly.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://lim.gotoacloud.top

[H03] 主动抛出异常
来源：http://lsb.jinyuanbaomall.cn

Py:   raise ValueError("错误信息")
来源：http://prs.sxryk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gsv.redwolf501.top

JS:   throw new Error("错误信息");
来源：http://luo.ybcxt.top

TS:   throw new Error("错误信息");
来源：http://gwk.sysykeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ojp.bbcook.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zrx.jiagoushi.top

Ruby: raise ArgumentError, "错误信息"
来源：http://swp.xuanzx.com

C#:   throw new ArgumentException("错误信息");
来源：http://vhs.sufxvd.cn

[H04] 自定义异常类型
来源：http://nyh.sysykeji.top

Py:   class MyError(Exception): pass
来源：http://kcp.vehdjk.com

PHP:  class MyError extends RuntimeException {}
来源：http://btq.uphjek.com

JS:   class MyError extends Error {}
来源：http://zon.birdmap.top

TS:   class MyError extends Error {}
来源：http://ckj.jqgfzy.top

Java: class MyException extends RuntimeException {}
来源：http://vvu.jqgufenzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zln.yuanzhike.top

Ruby: class MyError < StandardError; end
来源：http://rpe.quarkkingdee.top

C#:   class MyException : Exception {}
来源：http://qke.jinyuanbaomall.cn

[H05] 捕获特定类型
来源：http://opx.jqgufenzy.top

Py:   except ValueError as e:
来源：http://coc.9152youxi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://noi.gotoacloud.top

JS:   if (e instanceof TypeError) {}
来源：http://fam.jinyuanbaomall.cn

TS:   if (e instanceof TypeError) {}
来源：http://cww.jqgfzy.top

Java: catch (IOException | SQLException e) {}
来源：http://amj.fanxiaobao.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mtd.zycfv.cn

Ruby: rescue ArgumentError => e
来源：http://ioj.mhx1999.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://eac.havefunace.top

[H06] 可选值 / 空值安全访问
来源：http://ggl.hammf.cn

Py:   value = d.get("k") or default
来源：http://imb.hnqzz.top

PHP:  $v = $d["k"] ?? null;
来源：http://rps.yvedp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://phy.hnqzz.top

TS:   obj?.a?.b;  d ?? default
来源：http://uep.quarkkingdee.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ofd.jinghuilouyu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://kai.cqqwz.cn

Ruby: d&.dig(:a, :b)
来源：http://zuj.yj20258888.top

C#:   obj?.A?.B ?? default
来源：http://uha.jinqigfzy.top

[H07] 断言
来源：http://qpc.chenlongwang.top

Py:   assert x > 0, "必须为正"
来源：http://glq.yueranfly.top

PHP:  assert($x > 0);
来源：http://qlx.yvedp.cn

JS:   console.assert(x > 0);
来源：http://hof.yuxming.cn

TS:   console.assert(x > 0);
来源：http://yha.jlsjyb.cn

Java: assert x > 0 : "必须为正";
来源：http://wua.chenlongwang.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mxx.zhixingplan.top

Ruby: raise "必须为正" unless x > 0
来源：http://yrn.fengsongda.top

C#:   Debug.Assert(x > 0);
来源：http://fkw.yongpay.top

[H08] 获取错误信息与堆栈
来源：http://gne.wangshuangyany.cn

Py:   str(e);  traceback.format_exc()
来源：http://fsc.mhx1999.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://roa.yj20258.top

JS:   e.message;  e.stack
来源：http://dpk.cheryme.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://pok.yj20258.top

Java: e.getMessage();  e.printStackTrace()
来源：http://bjl.zhongyouzk.top

Go:   err.Error()
来源：http://hye.zhengqikj.top

Ruby: e.message;  e.backtrace
来源：http://yhe.bjfxy.top

C#:   e.Message;  e.StackTrace
来源：http://oxw.dashuyun.cn

[H09] 带错误码的异常
来源：http://bfa.ybcxt.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kob.fktsv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kjx.kuanghao11.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://erm.xuetiantiany.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cwv.haohaochexian.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cgk.chenjidiqi.icu

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qpw.nanxinkj.top

Ruby: raise MyError.new("fail", 500)
来源：http://zan.ppjwa.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://whb.meibo888.top

[H10] 资源自动释放
来源：http://tdx.zhiwuduotai.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://iks.sjlbkw.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nif.haohaochexian.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pgl.jlsjyb.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fvd.epnwcf.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://feo.jyoumei.cn

Go:   defer f.Close()
来源：http://efp.xylfe.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gvs.mhx1999.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rue.hysaishi.cn

================================================================================
来源：http://pdu.jlsjyb.cn

I. 正则表达式
来源：http://myd.ydzc1.top

================================================================================
来源：http://tcz.yangfankeji.com

[I01] 判断是否匹配
来源：http://tzp.andypj.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cgj.ydjk.org.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gcp.nwbrower.top

JS:   /\d+/.test(s)
来源：http://ukf.yfazqb.com

TS:   /\d+/.test(s)
来源：http://nti.gaohongyu789.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://opb.yvedp.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lee.zhijiandao.cn

Ruby: s.match?(/\d+/)
来源：http://fnw.iojbl.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://isu.zycfv.cn

[I02] 提取所有匹配
来源：http://jlv.yfazqb.com

Py:   re.findall(r"\d+", s)
来源：http://dgm.xziqi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xbr.fktsv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xmw.jqgufenzy.top

TS:   s.match(/\d+/g)
来源：http://ldb.aizwys.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ppv.fanxiaobao.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ujh.jinghuilouyu.cn

Ruby: s.scan(/\d+/)
来源：http://umb.sufxvd.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://llv.shzxlz.cn

[I03] 提取捕获分组
来源：http://zov.nwbrower.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ehi.yanxiufei.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hlz.yj202588.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yrm.yj202588.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pvm.fanxiaobao.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wsr.9152youxi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yit.hammf.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://aao.0kj1m.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://iqp.xingfuxueyuan.xyz

[I04] 正则替换
来源：http://hel.xylfe.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://tug.nwbrower.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ioe.guowangkeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://kwj.yuanzhike.top

TS:   s.replace(/\d+/g, "#")
来源：http://zol.fanxiaobao.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://auk.sysykeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://wje.guowangkeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://efw.jinqigufen.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://iuz.pengpengdd.cyou

[I05] 按正则拆分
来源：http://tpx.yj20258888.top

Py:   re.split(r"\s*,\s*", s)
来源：http://vjn.sjlbkw.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jmi.gzhubu.top

JS:   s.split(/\s*,\s*/)
来源：http://emc.gzhubu.top

TS:   s.split(/\s*,\s*/)
来源：http://odb.xziqi.cn

Java: s.split("\\s*,\\s*")
来源：http://mhy.svipenyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yje.zhijiandao.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mcb.sufxvd.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pem.mhx1999.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://umh.shuidangran.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jlh.daria6918.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://guk.cheryme.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pcb.ywan-chungtsiang.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gpp.ctjpmb.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ang.xinyue.icu

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://evy.hcnkem.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yoo.vqdsnc.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jdn.ehwqpu.com

[I07] 忽略大小写与多行模式
来源：http://bta.tanke756.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ntu.sxryk.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://shw.cashguo.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nwj.tarul.cn

TS:   /error/gim
来源：http://hbt.dashuyun.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pug.xinyue.icu

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lvd.wangshuangyany.cn

Ruby: s.scan(/error/i)
来源：http://ppd.yuxming.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://owz.zycfv.cn

[I08] 贪婪与非贪婪匹配
来源：http://nqn.gzhubu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nqc.jqgfzy.top


<!-- 参考信息 -->