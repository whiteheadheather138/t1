代发 wailian999

[G02] 构造函数
来源：http://tbj.yj202588.top

Py:   def __init__(self, name): self.name = name
来源：http://qlp.andypj.xyz

PHP:  public function __construct(public string $name) {}
来源：http://bdc.fktsv.cn

JS:   constructor(name) { this.name = name; }
来源：http://ezj.gaohongyu789.top

TS:   constructor(public name: string) {}
来源：http://yxg.vehdjk.com

Java: User(String name) { this.name = name; }
来源：http://iww.aibaodan.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ywh.hcnkem.com

Ruby: def initialize(name); @name = name; end
来源：http://kab.aizwys.cn

C#:   public User(string name) { Name = name; }
来源：http://aqn.sjlbkw.cn

[G03] 实例属性
来源：http://tyw.jianghu66.top

Py:   self.name = "x"
来源：http://hlj.bjfxy.top

PHP:  public string $name = "x";
来源：http://wmo.sufxvd.cn

JS:   this.name = "x";
来源：http://wxd.zdqjudy.top

TS:   name: string = "x";
来源：http://zxz.zhijiandao.cn

Java: private String name;
来源：http://olm.ctjpmb.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kml.daria6918.cn

Ruby: @name = "x"
来源：http://noy.tian-w.cn

C#:   public string Name { get; set; } = "x";
来源：http://vfm.pycfn.com

[G04] 定义方法
来源：http://kqu.xylfe.cn

Py:   def greet(self): return self.name
来源：http://rmb.aibaodan.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lkg.yongpay.top

JS:   greet() { return this.name; }
来源：http://way.sjlbkw.cn

TS:   greet(): string { return this.name; }
来源：http://tjn.nwbrower.top

Java: String greet() { return name; }
来源：http://ytk.zhongyouzk.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://qpr.zhaomingkeji.xyz

Ruby: def greet; @name; end
来源：http://vdd.havefunace.top

C#:   public string Greet() => Name;
来源：http://tbr.shanyushiyangkeji.top

[G05] 继承
来源：http://blo.xingfuxueyuan.xyz

Py:   class Admin(User): pass
来源：http://xis.bjfxy.top

PHP:  class Admin extends User {}
来源：http://lah.tanke756.top

JS:   class Admin extends User {}
来源：http://ffr.tianlin.xyz

TS:   class Admin extends User {}
来源：http://uxt.yvedp.cn

Java: class Admin extends User {}
来源：http://qpm.daxiang520.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ikr.yonumen.top

Ruby: class Admin < User; end
来源：http://vis.gaohongyu789.top

C#:   class Admin : User {}
来源：http://pos.fanxiaobao.xyz

[G06] 重写方法
来源：http://zum.cdnleiting.top

Py:   def greet(self): return "admin"
来源：http://aat.gaohongyu789.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ugs.yfazqb.com

JS:   greet() { return "admin"; }
来源：http://xds.shanyushiyangkeji.top

TS:   greet(): string { return "admin"; }
来源：http://lyb.feifeiyinyue.top

Java: @Override String greet() { return "admin"; }
来源：http://eli.ydjk.org.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qxu.zycfv.cn

Ruby: def greet; "admin"; end
来源：http://rhy.c1oappe.top

C#:   public override string Greet() => "admin";
来源：http://mwn.cheryme.top

[G07] 调用父类方法
来源：http://png.c1oappe.top

Py:   super().greet()
来源：http://znq.xziqi.cn

PHP:  parent::greet();
来源：http://iqt.yj202588.top

JS:   super.greet();
来源：http://ucd.jinqigufen.top

TS:   super.greet();
来源：http://eao.zhijiandao.cn

Java: super.greet();
来源：http://ybt.ehwqpu.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ezz.ctjpmb.com

Ruby: super
来源：http://wnw.xziqi.cn

C#:   base.Greet();
来源：http://pvp.fanxiaobao.xyz

[G08] 静态方法与属性
来源：http://hmx.mhx1999.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gyq.vehdjk.com

PHP:  public static function f() {}
来源：http://xjn.nanxinkj.top

JS:   static f() {}
来源：http://tkx.yj202588.top

TS:   static f(): void {}
来源：http://gnw.yj20258.top

Java: static void f() {}
来源：http://ixs.sysykeji.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://oes.c1oappe.top

Ruby: def self.f; end
来源：http://xba.jyoumei.cn

C#:   public static void F() {}
来源：http://lee.c1oappe.top

[G09] 接口 / 抽象类
来源：http://zns.jqgufenzy.top

Py:   from abc import ABC, abstractmethod
来源：http://euy.hnxiangtu.top

PHP:  interface Shape { public function area(): float; }
来源：http://ljn.bbcook.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wqv.tianlin.xyz

TS:   interface Shape { area(): number; }
来源：http://fqp.52xcode.cn

Java: interface Shape { double area(); }
来源：http://oci.hongshengwenyu.top

Go:   type Shape interface { Area() float64 }
来源：http://rwz.sjlbkw.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vzq.316326.xyz

C#:   interface IShape { double Area(); }
来源：http://twu.gaohongyu789.top

[G10] 访问控制
来源：http://rxt.ctjpmb.com

Py:   约定 _protected / __private（不强制）
来源：http://xef.0kj1m.cn

PHP:  public / protected / private
来源：http://oeo.quarkkingdee.top

JS:   #private 字段；其余公开
来源：http://mcw.feifeiyinyue.top

TS:   public / protected / private
来源：http://nxj.yj20258.top

Java: public / protected / private / 默认包级
来源：http://foi.zhixingplan.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ato.yj20258888.top

Ruby: public / protected / private
来源：http://oas.sysykeji.top

C#:   public / protected / private / internal
来源：http://frw.hesvh.cn

[G11] getter / setter
来源：http://nxf.zhaomingkeji.xyz

Py:   @property 与 @x.setter
来源：http://hvj.snrcjt.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://acv.hammf.cn

JS:   get name() { return this._name; }
来源：http://jie.zdbjq.cn

TS:   get name(): string { return this._name; }
来源：http://cxk.tian-w.cn

Java: public String getName() { return name; }
来源：http://fcq.jianghu66.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://deq.bbcook.cn

Ruby: attr_accessor :name
来源：http://uha.ctjpmb.com

C#:   public string Name { get; set; }
来源：http://ive.nanxuanxn.top

[G12] 对象转字符串
来源：http://fir.hongshengwenyu.top

Py:   def __str__(self): return self.name
来源：http://pql.ivvv.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://apt.hywenlv.cn

JS:   toString() { return this.name; }
来源：http://ztl.sufxvd.cn

TS:   toString(): string { return this.name; }
来源：http://bdg.yvedp.cn

Java: @Override public String toString() { return name; }
来源：http://hyl.cqqwz.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gkc.snrcjt.cn

Ruby: def to_s; @name; end
来源：http://rgm.yuxming.cn

C#:   public override string ToString() => Name;
来源：http://bri.fanxiaobao.xyz

[G13] 判断对象类型
来源：http://nun.ybcxt.top

Py:   isinstance(u, User)
来源：http://wgq.zhaomingkeji.xyz

PHP:  $u instanceof User
来源：http://zrd.c1oappe.top

JS:   u instanceof User
来源：http://zto.ybcxt.top

TS:   u instanceof User
来源：http://hyi.gaohongyu789.top

Java: u instanceof User
来源：http://xai.xuetiantiany.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jid.hywenlv.cn

Ruby: u.is_a?(User)
来源：http://vqf.chenjidiqi.icu

C#:   u is User
来源：http://dkr.aizwys.cn

[G14] 数据类 / record
来源：http://zwq.52xcode.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qlx.cucudq.cn

PHP:  // 用 readonly 属性模拟
来源：http://cxy.shanyushiyangtech.top

JS:   // 无内置：普通类或对象字面量
来源：http://wwa.yuxming.cn

TS:   type User = { name: string; age: number };
来源：http://osi.sxryk.cn

Java: record User(String name, int age) {}
来源：http://zgh.shzxlz.cn

Go:   type User struct { Name string; Age int }
来源：http://mgt.guannengcc.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zti.shzxlz.cn

C#:   record User(string Name, int Age);
来源：http://pjg.xuetiantiany.cn

[G15] 枚举
来源：http://rzm.feifeiyinyue.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lgq.cheryme.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://mpk.dianchejie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://civ.kuanghao11.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fao.hywenlv.cn

Java: enum Color { RED, GREEN }
来源：http://luu.xylfe.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mft.xylfe.cn

Ruby: Color = %i[red green].freeze
来源：http://yas.snrcjt.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kbm.yj202588.top

[G16] 对象转数组 / 字典
来源：http://sdp.guannengcc.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://owz.aibaodan.cn

PHP:  get_object_vars($obj);
来源：http://fsq.zdbjq.cn

JS:   Object.entries(obj)
来源：http://lqs.aibaodan.cn

TS:   Object.entries(obj)
来源：http://uxz.haohaochexian.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://trq.jlsjyb.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hud.hnxiangtu.top

Ruby: obj.instance_variables
来源：http://clk.xuanzx.com

C#:   // 用反射或 System.Text.Json
来源：http://ako.zhengqikj.top

================================================================================
来源：http://elc.hammf.cn

H. 异常与错误处理
来源：http://ect.yfazqb.com

================================================================================
来源：http://ucf.snrcjt.cn

[H01] try / catch 基础
来源：http://qiv.jinqigfzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dsq.yongpay.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tmt.yongpay.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vrc.jianghu66.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wcs.hongshengwenyu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pqd.xinyue.icu

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wos.nwbrower.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vnn.cheryme.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://njz.pycfn.com

[H02] finally / ensure 收尾
来源：http://ztk.dashuyun.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pcs.daxiang520.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hbx.pycfn.com

JS:   try { f(); } finally { cleanup(); }
来源：http://jkg.hesvh.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lcv.fzhhl.top

Java: try { f(); } finally { cleanup(); }
来源：http://cbu.bbcook.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vvz.gogol.net.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wbb.yj20258.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://dtf.ybcxt.top

[H03] 主动抛出异常
来源：http://eza.jyoumei.cn

Py:   raise ValueError("错误信息")
来源：http://ogq.ppjwa.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zzo.haohaochexian.top

JS:   throw new Error("错误信息");
来源：http://pwn.xuanzx.com

TS:   throw new Error("错误信息");
来源：http://gzx.gaohongyu789.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://veh.shangyingyoupin.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ndx.nwbrower.top

Ruby: raise ArgumentError, "错误信息"
来源：http://jum.xuetiantiany.cn

C#:   throw new ArgumentException("错误信息");
来源：http://trf.yj202588.top

[H04] 自定义异常类型
来源：http://kyg.yanxiufei.cn

Py:   class MyError(Exception): pass
来源：http://pmm.tanke756.top

PHP:  class MyError extends RuntimeException {}
来源：http://hip.aizwys.cn

JS:   class MyError extends Error {}
来源：http://kuw.chenzaomai.com

TS:   class MyError extends Error {}
来源：http://zqj.nanxinkj.top

Java: class MyException extends RuntimeException {}
来源：http://irs.vqdsnc.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jqe.haohaochexian.top

Ruby: class MyError < StandardError; end
来源：http://nfy.bjfxy.top

C#:   class MyException : Exception {}
来源：http://orj.0kj1m.cn

[H05] 捕获特定类型
来源：http://dny.316326.xyz

Py:   except ValueError as e:
来源：http://ufi.fengsongda.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uoz.shzxlz.cn

JS:   if (e instanceof TypeError) {}
来源：http://lhr.chenzaomai.com

TS:   if (e instanceof TypeError) {}
来源：http://gmw.sxryk.cn

Java: catch (IOException | SQLException e) {}
来源：http://kyq.ydzc1.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sts.nwbrower.top

Ruby: rescue ArgumentError => e
来源：http://ppl.ydzc1.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uqe.snrcjt.cn

[H06] 可选值 / 空值安全访问
来源：http://gku.jinghuilouyu.cn

Py:   value = d.get("k") or default
来源：http://dxn.redwolf501.top

PHP:  $v = $d["k"] ?? null;
来源：http://kpw.yj20258888.top

JS:   obj?.a?.b;  d ?? default
来源：http://qzp.hcnkem.com

TS:   obj?.a?.b;  d ?? default
来源：http://vdj.cqqwz.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://guw.feifeiyinyue.top

Go:   if v, ok := m["k"]; ok { }
来源：http://vxb.xingfuxueyuan.xyz

Ruby: d&.dig(:a, :b)
来源：http://ktd.chenjidiqi.icu

C#:   obj?.A?.B ?? default
来源：http://igb.jlsjyb.cn

[H07] 断言
来源：http://jes.hysaishi.cn

Py:   assert x > 0, "必须为正"
来源：http://lpp.wangshuangyany.cn

PHP:  assert($x > 0);
来源：http://ajn.pycfn.com

JS:   console.assert(x > 0);
来源：http://wft.jlsjyb.cn

TS:   console.assert(x > 0);
来源：http://ssi.shangyingyoupin.top

Java: assert x > 0 : "必须为正";
来源：http://gdj.nwbrower.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hne.hysaishi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rsz.52xcode.cn

C#:   Debug.Assert(x > 0);
来源：http://qjb.guannengcc.top

[H08] 获取错误信息与堆栈
来源：http://xip.ywan-chungtsiang.top

Py:   str(e);  traceback.format_exc()
来源：http://cry.zhongyouzk.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xne.vehdjk.com

JS:   e.message;  e.stack
来源：http://dxs.jqgufenzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ygc.dashuyun.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xmf.xuanzx.com

Go:   err.Error()
来源：http://ijx.andypj.xyz

Ruby: e.message;  e.backtrace
来源：http://zst.zdqjudy.top

C#:   e.Message;  e.StackTrace
来源：http://vcu.hammf.cn

[H09] 带错误码的异常
来源：http://lag.fktsv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jak.ydjk.org.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nxa.tian-w.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uxk.ywan-chungtsiang.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pns.xuanzx.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hyh.fanxiaobao.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hxf.hammf.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jyu.xingfuxueyuan.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://fyl.pengpengdd.cyou

[H10] 资源自动释放
来源：http://sye.shanyushiyangkeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://jfx.nwbrower.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ybk.tianlin.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bkz.pengpengdd.cyou

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mpl.quarkkingdee.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hcu.ydjk.org.cn

Go:   defer f.Close()
来源：http://eit.shuidangran.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mrt.ctjpmb.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wup.xinyue.icu

================================================================================
来源：http://wwf.jinghuilouyu.cn

I. 正则表达式
来源：http://ser.zhengqikj.top

================================================================================
来源：http://kpr.gogol.net.cn

[I01] 判断是否匹配
来源：http://tay.shangyingyoupin.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://msb.mhx1999.top

PHP:  preg_match('/\d+/', $s);
来源：http://uyd.yj20258888.top

JS:   /\d+/.test(s)
来源：http://yib.zhijiandao.cn

TS:   /\d+/.test(s)
来源：http://myy.hesvh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zkw.jlsjyb.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://efg.kuanghao11.cn

Ruby: s.match?(/\d+/)
来源：http://hji.bbcook.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gwu.daria6918.cn

[I02] 提取所有匹配
来源：http://nrd.nanxuanxn.top

Py:   re.findall(r"\d+", s)
来源：http://qdb.cdnleiting.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sxh.jinyuanbaomall.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://khe.cheryme.top

TS:   s.match(/\d+/g)
来源：http://hwo.ywan-chungtsiang.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lgk.guowangkeji.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bxf.xuanzx.com

Ruby: s.scan(/\d+/)
来源：http://fie.bjfxy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yua.cdnleiting.top

[I03] 提取捕获分组
来源：http://hqr.epnwcf.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zbx.52xcode.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hfp.xinyue.icu

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://edk.zhengqikj.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nfe.guannengcc.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xqh.chenlongwang.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ohc.hammf.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ipn.guannengcc.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://aqm.fengsongda.top

[I04] 正则替换
来源：http://fhd.52xcode.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qrw.xziqi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://aac.guowangkeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://vua.zhaomingkeji.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://rwf.cdnleiting.top

Java: s.replaceAll("\\d+", "#")
来源：http://ebg.yfazqb.com

Go:   re.ReplaceAllString(s, "#")
来源：http://fjj.gaohongyu789.top

Ruby: s.gsub(/\d+/, "#")
来源：http://itd.nwbrower.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://owk.yfazqb.com

[I05] 按正则拆分
来源：http://yjs.feifeiyinyue.top

Py:   re.split(r"\s*,\s*", s)
来源：http://vcr.nwbrower.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fgh.jinqigfzy.top

JS:   s.split(/\s*,\s*/)
来源：http://ouy.hnqzz.top

TS:   s.split(/\s*,\s*/)
来源：http://vbm.epnwcf.com

Java: s.split("\\s*,\\s*")
来源：http://wqg.guannengcc.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rea.ydjk.org.cn

Ruby: s.split(/\s*,\s*/)
来源：http://lhy.sjlbkw.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://por.gogol.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rdr.cashguo.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://haq.guowangkeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wwm.xziqi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bgj.shuidangran.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uoj.yuxming.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zho.svipenyu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://irv.ybcxt.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xym.nanxuanxn.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://whg.fengsongda.top

[I07] 忽略大小写与多行模式
来源：http://njn.mhx1999.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://aly.yj20258888.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sur.yj20258888.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rwp.haohaochexian.top

TS:   /error/gim
来源：http://kxh.9152youxi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://exw.cucudq.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ijr.vqdsnc.cn

Ruby: s.scan(/error/i)
来源：http://xmt.52xcode.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vbn.nanxinkj.top

[I08] 贪婪与非贪婪匹配
来源：http://grt.jyoumei.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dbs.yvedp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://avs.xylfe.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tay.zhoulong.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://glr.birdmap.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://com.jqgufenzy.top


<!-- 参考信息 -->