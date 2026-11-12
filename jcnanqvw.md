代发 wailian999

================================================================================
来源：http://jix.yvedp.cn

G. 面向对象
来源：http://jvn.iojbl.cn

================================================================================
来源：http://mdo.cqqwz.cn

[G01] 定义类
来源：http://hnm.jlsjyb.cn

Py:   class User: pass
来源：http://ufa.tian-w.cn

PHP:  class User {}
来源：http://ith.vqdsnc.cn

JS:   class User {}
来源：http://ngt.jinyuanbaomall.cn

TS:   class User { name: string = ""; }
来源：http://bif.xziqi.cn

Java: class User {}
来源：http://rte.yj20258888.top

Go:   type User struct { Name string }
来源：http://ufg.jiagoushi.top

Ruby: class User; end
来源：http://yia.fengsongda.top

C#:   class User {}
来源：http://arm.zdbjq.cn

[G02] 构造函数
来源：http://vqs.feifeiyinyue.top

Py:   def __init__(self, name): self.name = name
来源：http://cox.quarkkingdee.top

PHP:  public function __construct(public string $name) {}
来源：http://sda.tianlin.xyz

JS:   constructor(name) { this.name = name; }
来源：http://lnc.wangdashe.top

TS:   constructor(public name: string) {}
来源：http://kwo.chenlongwang.top

Java: User(String name) { this.name = name; }
来源：http://lqj.daria6918.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oyx.xuetiantiany.cn

Ruby: def initialize(name); @name = name; end
来源：http://zey.vqdsnc.cn

C#:   public User(string name) { Name = name; }
来源：http://cld.bjfxy.top

[G03] 实例属性
来源：http://zre.tian-w.cn

Py:   self.name = "x"
来源：http://zyi.tianlin.xyz

PHP:  public string $name = "x";
来源：http://khj.0kj1m.cn

JS:   this.name = "x";
来源：http://dat.meibo888.top

TS:   name: string = "x";
来源：http://zdh.chenlongwang.top

Java: private String name;
来源：http://nmr.tanke756.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lqa.fanxiaobao.xyz

Ruby: @name = "x"
来源：http://izg.guannengcc.top

C#:   public string Name { get; set; } = "x";
来源：http://hzh.gaohongyu789.top

[G04] 定义方法
来源：http://vsr.cdnleiting.top

Py:   def greet(self): return self.name
来源：http://toe.andypj.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://cgg.xuetiantiany.cn

JS:   greet() { return this.name; }
来源：http://iks.tanke756.top

TS:   greet(): string { return this.name; }
来源：http://jlf.uphjek.com

Java: String greet() { return name; }
来源：http://wtj.yj20258888.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://bxq.fzhhl.top

Ruby: def greet; @name; end
来源：http://nhf.ydzc1.top

C#:   public string Greet() => Name;
来源：http://qcn.gzhubu.top

[G05] 继承
来源：http://hma.zhongyouzk.top

Py:   class Admin(User): pass
来源：http://gxy.9152youxi.cn

PHP:  class Admin extends User {}
来源：http://wsu.fktsv.cn

JS:   class Admin extends User {}
来源：http://pmf.chenlongwang.top

TS:   class Admin extends User {}
来源：http://dav.ywan-chungtsiang.top

Java: class Admin extends User {}
来源：http://goh.bjfxy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://exy.hongshengwenyu.top

Ruby: class Admin < User; end
来源：http://poi.zycfv.cn

C#:   class Admin : User {}
来源：http://okg.dashuyun.cn

[G06] 重写方法
来源：http://zmy.smart0.xyz

Py:   def greet(self): return "admin"
来源：http://ngh.hammf.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://uml.hysaishi.cn

JS:   greet() { return "admin"; }
来源：http://vdx.meibo888.top

TS:   greet(): string { return "admin"; }
来源：http://qlc.fanxiaobao.xyz

Java: @Override String greet() { return "admin"; }
来源：http://fna.zdqjudy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cli.jqgufenzy.top

Ruby: def greet; "admin"; end
来源：http://xgo.birdmap.top

C#:   public override string Greet() => "admin";
来源：http://kpl.hfpthk.cn

[G07] 调用父类方法
来源：http://umn.ybcxt.top

Py:   super().greet()
来源：http://mww.yfazqb.com

PHP:  parent::greet();
来源：http://ggi.hywenlv.cn

JS:   super.greet();
来源：http://lrb.hammf.cn

TS:   super.greet();
来源：http://orc.zhaomingkeji.xyz

Java: super.greet();
来源：http://auy.jinqigufen.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jwy.tanke756.top

Ruby: super
来源：http://usv.hcnkem.com

C#:   base.Greet();
来源：http://gwv.hfpthk.cn

[G08] 静态方法与属性
来源：http://hqp.aizwys.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://eil.cheryme.top

PHP:  public static function f() {}
来源：http://udr.bbcook.cn

JS:   static f() {}
来源：http://hfu.jinyuanbaomall.cn

TS:   static f(): void {}
来源：http://yfg.shanyushiyangtech.top

Java: static void f() {}
来源：http://tob.xingfuxueyuan.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://evf.jinqigufen.top

Ruby: def self.f; end
来源：http://ebr.zhongyouzk.top

C#:   public static void F() {}
来源：http://wyh.dianchejie.cn

[G09] 接口 / 抽象类
来源：http://cag.zhaomingkeji.xyz

Py:   from abc import ABC, abstractmethod
来源：http://iio.cashguo.top

PHP:  interface Shape { public function area(): float; }
来源：http://gyp.xuetiantiany.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ypd.feifeiyinyue.top

TS:   interface Shape { area(): number; }
来源：http://yxi.sysykeji.top

Java: interface Shape { double area(); }
来源：http://jhq.meibo888.top

Go:   type Shape interface { Area() float64 }
来源：http://rrn.hesvh.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uma.hnqzz.top

C#:   interface IShape { double Area(); }
来源：http://mrb.yfazqb.com

[G10] 访问控制
来源：http://uzr.fktsv.cn

Py:   约定 _protected / __private（不强制）
来源：http://kvs.daxiang520.top

PHP:  public / protected / private
来源：http://qdj.fktsv.cn

JS:   #private 字段；其余公开
来源：http://jzq.zhixingplan.top

TS:   public / protected / private
来源：http://ymr.epnwcf.com

Java: public / protected / private / 默认包级
来源：http://bqw.9152youxi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://cfj.zhiwuduotai.top

Ruby: public / protected / private
来源：http://ryf.316326.xyz

C#:   public / protected / private / internal
来源：http://jtl.zhaomingkeji.xyz

[G11] getter / setter
来源：http://hoh.guowangkeji.top

Py:   @property 与 @x.setter
来源：http://are.yueranfly.top

PHP:  public function getName(): string { return $this->name; }
来源：http://wpn.pengpengdd.cyou

JS:   get name() { return this._name; }
来源：http://xsy.shanyushiyangkeji.top

TS:   get name(): string { return this._name; }
来源：http://agg.xylfe.cn

Java: public String getName() { return name; }
来源：http://kca.shuidangran.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://rtt.fktsv.cn

Ruby: attr_accessor :name
来源：http://lua.haohaochexian.top

C#:   public string Name { get; set; }
来源：http://ric.9152youxi.cn

[G12] 对象转字符串
来源：http://atc.daria6918.cn

Py:   def __str__(self): return self.name
来源：http://hny.zdqjudy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://eyw.yfazqb.com

JS:   toString() { return this.name; }
来源：http://bps.hcnkem.com

TS:   toString(): string { return this.name; }
来源：http://fpt.sxryk.cn

Java: @Override public String toString() { return name; }
来源：http://oay.ivvv.top

Go:   func (u User) String() string { return u.Name }
来源：http://ecy.andypj.xyz

Ruby: def to_s; @name; end
来源：http://skj.svipenyu.cn

C#:   public override string ToString() => Name;
来源：http://ynd.epnwcf.com

[G13] 判断对象类型
来源：http://dwf.zhengqikj.top

Py:   isinstance(u, User)
来源：http://wdf.jqgufenzy.top

PHP:  $u instanceof User
来源：http://ify.ybcxt.top

JS:   u instanceof User
来源：http://uyk.jqgfzy.top

TS:   u instanceof User
来源：http://wse.daxiang520.top

Java: u instanceof User
来源：http://bob.hongshengwenyu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://dij.ppjwa.cn

Ruby: u.is_a?(User)
来源：http://syf.chenlongwang.top

C#:   u is User
来源：http://bkt.shangyingyoupin.top

[G14] 数据类 / record
来源：http://eej.hnxiangtu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yzx.feifeiyinyue.top

PHP:  // 用 readonly 属性模拟
来源：http://tcy.yueranfly.top

JS:   // 无内置：普通类或对象字面量
来源：http://zif.yuanzhike.top

TS:   type User = { name: string; age: number };
来源：http://cqc.hywenlv.cn

Java: record User(String name, int age) {}
来源：http://pkw.hcnkem.com

Go:   type User struct { Name string; Age int }
来源：http://fnj.ydjk.org.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ywv.zhaomingkeji.xyz

C#:   record User(string Name, int Age);
来源：http://zis.zhaomingkeji.xyz

[G15] 枚举
来源：http://ooe.jianghu66.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ljo.xylfe.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://nvu.yangfankeji.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yxd.zhongyouzk.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mac.hnqzz.top

Java: enum Color { RED, GREEN }
来源：http://txc.svipenyu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zlp.zhongyouzk.top

Ruby: Color = %i[red green].freeze
来源：http://tkm.jlsjyb.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yya.ydzc1.top

[G16] 对象转数组 / 字典
来源：http://jcd.guannengcc.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://equ.yj20258.top

PHP:  get_object_vars($obj);
来源：http://pdh.jqgufenzy.top

JS:   Object.entries(obj)
来源：http://wtt.shanyushiyangkeji.top

TS:   Object.entries(obj)
来源：http://zzs.tian-w.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yvq.yuanzhike.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://avs.havefunace.top

Ruby: obj.instance_variables
来源：http://pcm.gogol.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://rfh.pycfn.com

================================================================================
来源：http://ixu.fengsongda.top

H. 异常与错误处理
来源：http://tvb.c1oappe.top

================================================================================
来源：http://xkk.shanyushiyangkeji.top

[H01] try / catch 基础
来源：http://kvo.zhijiandao.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xzo.gaohongyu789.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cxl.bbcook.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vhn.ydzc1.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qfd.c1oappe.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kts.xziqi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://epc.hywenlv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sxz.yuxming.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qcb.xinyue.icu

[H02] finally / ensure 收尾
来源：http://nfg.daxiang520.top

Py:   try: f()⏎finally: cleanup()
来源：http://cfx.yanxiufei.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yla.cqqwz.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hdq.yj20258888.top

TS:   try { f(); } finally { cleanup(); }
来源：http://jaj.yueranfly.top

Java: try { f(); } finally { cleanup(); }
来源：http://wzk.ctjpmb.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://ktb.bbcook.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vvr.vehdjk.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://irn.yonumen.top

[H03] 主动抛出异常
来源：http://fhc.gotoacloud.top

Py:   raise ValueError("错误信息")
来源：http://vpe.daxiang520.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xms.tian-w.cn

JS:   throw new Error("错误信息");
来源：http://glk.jlsjyb.cn

TS:   throw new Error("错误信息");
来源：http://aix.jinqigfzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://vqa.zhongyouzk.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qip.sysykeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://lhs.0kj1m.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wqg.ybcxt.top

[H04] 自定义异常类型
来源：http://xas.sufxvd.cn

Py:   class MyError(Exception): pass
来源：http://pki.feifeiyinyue.top

PHP:  class MyError extends RuntimeException {}
来源：http://xkv.fengsongda.top

JS:   class MyError extends Error {}
来源：http://iqz.fehbvm.com

TS:   class MyError extends Error {}
来源：http://wji.hammf.cn

Java: class MyException extends RuntimeException {}
来源：http://agi.mhx1999.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ffs.hnqzz.top

Ruby: class MyError < StandardError; end
来源：http://xkb.yuanzhike.top

C#:   class MyException : Exception {}
来源：http://rbr.bbcook.cn

[H05] 捕获特定类型
来源：http://vhx.fzhhl.top

Py:   except ValueError as e:
来源：http://hsz.smart0.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://atz.cdnleiting.top

JS:   if (e instanceof TypeError) {}
来源：http://byl.fengsongda.top

TS:   if (e instanceof TypeError) {}
来源：http://jpe.sweek.top

Java: catch (IOException | SQLException e) {}
来源：http://lic.yanxiufei.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qwm.ivvv.top

Ruby: rescue ArgumentError => e
来源：http://ubx.cashguo.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://scg.gzhubu.top

[H06] 可选值 / 空值安全访问
来源：http://kcl.cucudq.cn

Py:   value = d.get("k") or default
来源：http://uwa.sjlbkw.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jah.nanxuanxn.top

JS:   obj?.a?.b;  d ?? default
来源：http://rrd.gaohongyu789.top

TS:   obj?.a?.b;  d ?? default
来源：http://ugd.zhaomingkeji.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hsj.sweek.top

Go:   if v, ok := m["k"]; ok { }
来源：http://szm.aizwys.cn

Ruby: d&.dig(:a, :b)
来源：http://ulb.hysaishi.cn

C#:   obj?.A?.B ?? default
来源：http://gml.zhoulong.xyz

[H07] 断言
来源：http://axc.hesvh.cn

Py:   assert x > 0, "必须为正"
来源：http://hvp.shangyingyoupin.top

PHP:  assert($x > 0);
来源：http://rfh.ctjpmb.com

JS:   console.assert(x > 0);
来源：http://fgz.jiagoushi.top

TS:   console.assert(x > 0);
来源：http://bfc.havefunace.top

Java: assert x > 0 : "必须为正";
来源：http://ush.meibo888.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nqd.tanke756.top

Ruby: raise "必须为正" unless x > 0
来源：http://mwm.ctjpmb.com

C#:   Debug.Assert(x > 0);
来源：http://atn.yuanzhike.top

[H08] 获取错误信息与堆栈
来源：http://psf.zdqjudy.top

Py:   str(e);  traceback.format_exc()
来源：http://vdi.shanyushiyangkeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bbk.9152youxi.cn

JS:   e.message;  e.stack
来源：http://ntq.hnxiangtu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://kfq.shanyushiyangtech.top

Java: e.getMessage();  e.printStackTrace()
来源：http://awp.andypj.xyz

Go:   err.Error()
来源：http://isx.jinqigufen.top

Ruby: e.message;  e.backtrace
来源：http://yax.zhengqikj.top

C#:   e.Message;  e.StackTrace
来源：http://hhj.bjfxy.top

[H09] 带错误码的异常
来源：http://gdf.andypj.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hdz.yongpay.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://fnl.guowangkeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://oop.yfazqb.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fdb.jinqigfzy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wxr.xinyue.icu

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qpa.nanxuanxn.top

Ruby: raise MyError.new("fail", 500)
来源：http://rpb.shzxlz.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ovi.chenlongwang.top

[H10] 资源自动释放
来源：http://vlz.jyoumei.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ueu.zhixingplan.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vtu.hfpthk.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://etz.chenjidiqi.icu

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hfj.jinqigufen.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pqd.sysykeji.top

Go:   defer f.Close()
来源：http://xaa.nwbrower.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jbc.yj20258.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cme.zhiwuduotai.top

================================================================================
来源：http://zto.jqgfzy.top

I. 正则表达式
来源：http://rck.vehdjk.com

================================================================================
来源：http://lnc.ywan-chungtsiang.top

[I01] 判断是否匹配
来源：http://rht.ydjk.org.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hjt.xylfe.cn

PHP:  preg_match('/\d+/', $s);
来源：http://anf.nwbrower.top

JS:   /\d+/.test(s)
来源：http://glk.bbcook.cn

TS:   /\d+/.test(s)
来源：http://dgb.hongshengwenyu.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kyu.yueranfly.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ios.aizwys.cn

Ruby: s.match?(/\d+/)
来源：http://ztp.nanxinkj.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qfo.sxryk.cn

[I02] 提取所有匹配
来源：http://gey.yj20258.top

Py:   re.findall(r"\d+", s)
来源：http://wzc.zhongyouzk.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tsq.zhiwuduotai.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gjl.yonumen.top

TS:   s.match(/\d+/g)
来源：http://hij.birdmap.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://aln.guannengcc.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rdy.sufxvd.cn

Ruby: s.scan(/\d+/)
来源：http://mza.nanxinkj.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://deg.cucudq.cn

[I03] 提取捕获分组
来源：http://flt.chenlongwang.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kgr.cheryme.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qrf.yongpay.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rea.cdnleiting.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wkh.zhoulong.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bnk.gotoacloud.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bfh.guowangkeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mkd.yonumen.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hul.hcnkem.com

[I04] 正则替换
来源：http://kzs.vqdsnc.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hmc.jianghu66.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://eti.haohaochexian.top

JS:   s.replace(/\d+/g, "#")
来源：http://ery.sjlbkw.cn

TS:   s.replace(/\d+/g, "#")
来源：http://tfk.xuetiantiany.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wjr.zycfv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xlp.pycfn.com

Ruby: s.gsub(/\d+/, "#")
来源：http://yzk.pengpengdd.cyou

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kep.uphjek.com

[I05] 按正则拆分
来源：http://njg.fehbvm.com

Py:   re.split(r"\s*,\s*", s)
来源：http://ame.cqqwz.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uqj.pycfn.com

JS:   s.split(/\s*,\s*/)
来源：http://qeo.cdnleiting.top

TS:   s.split(/\s*,\s*/)
来源：http://ulm.cqqwz.cn

Java: s.split("\\s*,\\s*")
来源：http://dga.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xcx.shzxlz.cn

Ruby: s.split(/\s*,\s*/)
来源：http://aao.ydjk.org.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dvx.jinqigufen.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vyj.ywan-chungtsiang.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gxr.fehbvm.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dre.fktsv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://szp.fanxiaobao.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yob.shanyushiyangtech.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zsu.tianlin.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tdy.hesvh.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hgx.hywenlv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ddr.hammf.cn

[I07] 忽略大小写与多行模式
来源：http://fzb.xziqi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hrq.ehwqpu.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ozv.sjlbkw.cn


<!-- 参考信息 -->