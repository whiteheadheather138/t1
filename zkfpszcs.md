代发 wailian999

================================================================================
来源：http://whq.wangdashe.top

G. 面向对象
来源：http://qaw.ydzc1.top

================================================================================
来源：http://vif.redwolf501.top

[G01] 定义类
来源：http://qqs.c1oappe.top

Py:   class User: pass
来源：http://zwc.aizwys.cn

PHP:  class User {}
来源：http://szk.snrcjt.cn

JS:   class User {}
来源：http://vrf.cucudq.cn

TS:   class User { name: string = ""; }
来源：http://fnm.xingfuxueyuan.xyz

Java: class User {}
来源：http://xdn.jyoumei.cn

Go:   type User struct { Name string }
来源：http://rnl.pengpengdd.cyou

Ruby: class User; end
来源：http://vad.fanxiaobao.xyz

C#:   class User {}
来源：http://uwy.pycfn.com

[G02] 构造函数
来源：http://yhi.jqgufenzy.top

Py:   def __init__(self, name): self.name = name
来源：http://ogx.yj202588.top

PHP:  public function __construct(public string $name) {}
来源：http://lsk.yvedp.cn

JS:   constructor(name) { this.name = name; }
来源：http://llh.zdbjq.cn

TS:   constructor(public name: string) {}
来源：http://tyr.hammf.cn

Java: User(String name) { this.name = name; }
来源：http://bla.redwolf501.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gqc.jiagoushi.top

Ruby: def initialize(name); @name = name; end
来源：http://sdg.hnxiangtu.top

C#:   public User(string name) { Name = name; }
来源：http://wye.yueranfly.top

[G03] 实例属性
来源：http://dpk.gzhubu.top

Py:   self.name = "x"
来源：http://pid.bjfxy.top

PHP:  public string $name = "x";
来源：http://gjw.cashguo.top

JS:   this.name = "x";
来源：http://htb.guannengcc.top

TS:   name: string = "x";
来源：http://jwz.jinqigufen.top

Java: private String name;
来源：http://loi.zhiwuduotai.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pqu.jinghuilouyu.cn

Ruby: @name = "x"
来源：http://ypc.yueranfly.top

C#:   public string Name { get; set; } = "x";
来源：http://soa.tianlin.xyz

[G04] 定义方法
来源：http://ezj.pycfn.com

Py:   def greet(self): return self.name
来源：http://hac.shuidangran.top

PHP:  public function greet(): string { return $this->name; }
来源：http://tct.uphjek.com

JS:   greet() { return this.name; }
来源：http://wxq.xuanzx.com

TS:   greet(): string { return this.name; }
来源：http://kbs.tianlin.xyz

Java: String greet() { return name; }
来源：http://dhl.tanke756.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ltu.cdnleiting.top

Ruby: def greet; @name; end
来源：http://fhe.jianghu66.top

C#:   public string Greet() => Name;
来源：http://ehj.hongshengwenyu.top

[G05] 继承
来源：http://eig.tian-w.cn

Py:   class Admin(User): pass
来源：http://ucz.daria6918.cn

PHP:  class Admin extends User {}
来源：http://xjn.chenzaomai.com

JS:   class Admin extends User {}
来源：http://ljj.cheryme.top

TS:   class Admin extends User {}
来源：http://btl.cqqwz.cn

Java: class Admin extends User {}
来源：http://rrb.jinqigufen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://eqr.yuanzhike.top

Ruby: class Admin < User; end
来源：http://fyu.cashguo.top

C#:   class Admin : User {}
来源：http://bvt.cheryme.top

[G06] 重写方法
来源：http://kbo.sweek.top

Py:   def greet(self): return "admin"
来源：http://xvd.pengpengdd.cyou

PHP:  public function greet(): string { return "admin"; }
来源：http://kvo.cucudq.cn

JS:   greet() { return "admin"; }
来源：http://zvz.jinyuanbaomall.cn

TS:   greet(): string { return "admin"; }
来源：http://biq.9152youxi.cn

Java: @Override String greet() { return "admin"; }
来源：http://skx.sjlbkw.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rkd.pycfn.com

Ruby: def greet; "admin"; end
来源：http://yja.fzhhl.top

C#:   public override string Greet() => "admin";
来源：http://zoy.ppjwa.cn

[G07] 调用父类方法
来源：http://lyc.yueranfly.top

Py:   super().greet()
来源：http://nez.shanyushiyangtech.top

PHP:  parent::greet();
来源：http://ref.shzxlz.cn

JS:   super.greet();
来源：http://kab.cheryme.top

TS:   super.greet();
来源：http://zxa.yj20258888.top

Java: super.greet();
来源：http://cvj.jqgufenzy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jsa.yonumen.top

Ruby: super
来源：http://yyx.shanyushiyangkeji.top

C#:   base.Greet();
来源：http://ogo.chenzaomai.com

[G08] 静态方法与属性
来源：http://twi.cdnleiting.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wgs.gotoacloud.top

PHP:  public static function f() {}
来源：http://nxx.gogol.net.cn

JS:   static f() {}
来源：http://hdi.zhixingplan.top

TS:   static f(): void {}
来源：http://swn.tianlin.xyz

Java: static void f() {}
来源：http://vuk.ydjk.org.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ajh.jqgfzy.top

Ruby: def self.f; end
来源：http://cbe.pycfn.com

C#:   public static void F() {}
来源：http://xlp.hammf.cn

[G09] 接口 / 抽象类
来源：http://lws.zhoulong.xyz

Py:   from abc import ABC, abstractmethod
来源：http://alh.ydjk.org.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zkn.kuanghao11.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rpx.hysaishi.cn

TS:   interface Shape { area(): number; }
来源：http://lhw.guowangkeji.top

Java: interface Shape { double area(); }
来源：http://ame.vqdsnc.cn

Go:   type Shape interface { Area() float64 }
来源：http://pew.mhx1999.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qcf.yonumen.top

C#:   interface IShape { double Area(); }
来源：http://acz.iojbl.cn

[G10] 访问控制
来源：http://npf.zdqjudy.top

Py:   约定 _protected / __private（不强制）
来源：http://hut.ppjwa.cn

PHP:  public / protected / private
来源：http://veg.xuetiantiany.cn

JS:   #private 字段；其余公开
来源：http://izo.zhoulong.xyz

TS:   public / protected / private
来源：http://pfa.shuidangran.top

Java: public / protected / private / 默认包级
来源：http://gom.hcnkem.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://fxm.zdqjudy.top

Ruby: public / protected / private
来源：http://kvo.birdmap.top

C#:   public / protected / private / internal
来源：http://cjl.yangfankeji.com

[G11] getter / setter
来源：http://fmd.cashguo.top

Py:   @property 与 @x.setter
来源：http://tvq.yj20258888.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ido.birdmap.top

JS:   get name() { return this._name; }
来源：http://umz.ehwqpu.com

TS:   get name(): string { return this._name; }
来源：http://zej.cashguo.top

Java: public String getName() { return name; }
来源：http://zxk.sjlbkw.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ztr.smart0.xyz

Ruby: attr_accessor :name
来源：http://mqp.yuanzhike.top

C#:   public string Name { get; set; }
来源：http://gxu.xuetiantiany.cn

[G12] 对象转字符串
来源：http://ajg.tian-w.cn

Py:   def __str__(self): return self.name
来源：http://pel.fengsongda.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://mkf.yj20258.top

JS:   toString() { return this.name; }
来源：http://gzs.jiagoushi.top

TS:   toString(): string { return this.name; }
来源：http://kyc.gzhubu.top

Java: @Override public String toString() { return name; }
来源：http://yqt.fengsongda.top

Go:   func (u User) String() string { return u.Name }
来源：http://zcx.shuidangran.top

Ruby: def to_s; @name; end
来源：http://eme.gaohongyu789.top

C#:   public override string ToString() => Name;
来源：http://fup.zhaomingkeji.xyz

[G13] 判断对象类型
来源：http://lez.dianchejie.cn

Py:   isinstance(u, User)
来源：http://ncr.wangdashe.top

PHP:  $u instanceof User
来源：http://bri.9152youxi.cn

JS:   u instanceof User
来源：http://lan.feifeiyinyue.top

TS:   u instanceof User
来源：http://oii.xziqi.cn

Java: u instanceof User
来源：http://ozc.birdmap.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://oor.ehwqpu.com

Ruby: u.is_a?(User)
来源：http://xzn.tianlin.xyz

C#:   u is User
来源：http://pqa.zdbjq.cn

[G14] 数据类 / record
来源：http://gly.yueranfly.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uyc.sweek.top

PHP:  // 用 readonly 属性模拟
来源：http://sjg.tianlin.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://sox.jinqigufen.top

TS:   type User = { name: string; age: number };
来源：http://gho.hammf.cn

Java: record User(String name, int age) {}
来源：http://yvx.zdqjudy.top

Go:   type User struct { Name string; Age int }
来源：http://wsx.sufxvd.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cre.nanxuanxn.top

C#:   record User(string Name, int Age);
来源：http://mqb.epnwcf.com

[G15] 枚举
来源：http://dar.jinqigufen.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rjj.xingfuxueyuan.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://ett.xingfuxueyuan.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vnp.hywenlv.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wlj.sufxvd.cn

Java: enum Color { RED, GREEN }
来源：http://itf.jinyuanbaomall.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rfo.jyoumei.cn

Ruby: Color = %i[red green].freeze
来源：http://lfn.shzxlz.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mod.yanxiufei.cn

[G16] 对象转数组 / 字典
来源：http://mkw.bbcook.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fxj.epnwcf.com

PHP:  get_object_vars($obj);
来源：http://pcb.birdmap.top

JS:   Object.entries(obj)
来源：http://ryw.tianlin.xyz

TS:   Object.entries(obj)
来源：http://fid.hnqzz.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sxi.xziqi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bca.xingfuxueyuan.xyz

Ruby: obj.instance_variables
来源：http://mvk.quarkkingdee.top

C#:   // 用反射或 System.Text.Json
来源：http://gav.xuetiantiany.cn

================================================================================
来源：http://exl.tarul.cn

H. 异常与错误处理
来源：http://sgo.daxiang520.top

================================================================================
来源：http://nax.snrcjt.cn

[H01] try / catch 基础
来源：http://gqk.kuanghao11.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yjc.svipenyu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mbo.aibaodan.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zpa.316326.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bpm.hnxiangtu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mxt.daxiang520.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ger.epnwcf.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pfr.daria6918.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://btd.9152youxi.cn

[H02] finally / ensure 收尾
来源：http://csl.iojbl.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xfk.shanyushiyangtech.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vlo.fanxiaobao.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://nvi.jinqigfzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://qls.zhijiandao.cn

Java: try { f(); } finally { cleanup(); }
来源：http://eax.shzxlz.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://oce.pycfn.com

Ruby: begin; f; ensure; cleanup; end
来源：http://agj.fehbvm.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://mti.sysykeji.top

[H03] 主动抛出异常
来源：http://het.zhengqikj.top

Py:   raise ValueError("错误信息")
来源：http://zjd.dashuyun.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tgt.hnxiangtu.top

JS:   throw new Error("错误信息");
来源：http://zhd.daria6918.cn

TS:   throw new Error("错误信息");
来源：http://ysb.zdbjq.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://puc.gaohongyu789.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xrk.guannengcc.top

Ruby: raise ArgumentError, "错误信息"
来源：http://phm.cheryme.top

C#:   throw new ArgumentException("错误信息");
来源：http://qhu.hammf.cn

[H04] 自定义异常类型
来源：http://dnd.yj20258888.top

Py:   class MyError(Exception): pass
来源：http://has.gotoacloud.top

PHP:  class MyError extends RuntimeException {}
来源：http://pma.zhongyouzk.top

JS:   class MyError extends Error {}
来源：http://isu.quarkkingdee.top

TS:   class MyError extends Error {}
来源：http://rfu.jqgufenzy.top

Java: class MyException extends RuntimeException {}
来源：http://lrf.gogol.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://upc.shuidangran.top

Ruby: class MyError < StandardError; end
来源：http://ytf.tianlin.xyz

C#:   class MyException : Exception {}
来源：http://yxv.hammf.cn

[H05] 捕获特定类型
来源：http://hou.zhongyouzk.top

Py:   except ValueError as e:
来源：http://jbt.sweek.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mom.xziqi.cn

JS:   if (e instanceof TypeError) {}
来源：http://vat.dianchejie.cn

TS:   if (e instanceof TypeError) {}
来源：http://huu.sjlbkw.cn

Java: catch (IOException | SQLException e) {}
来源：http://guj.wangdashe.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tvw.ydzc1.top

Ruby: rescue ArgumentError => e
来源：http://bzl.316326.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qah.wangshuangyany.cn

[H06] 可选值 / 空值安全访问
来源：http://nkn.sxryk.cn

Py:   value = d.get("k") or default
来源：http://gzs.yonumen.top

PHP:  $v = $d["k"] ?? null;
来源：http://gnm.birdmap.top

JS:   obj?.a?.b;  d ?? default
来源：http://kwf.shangyingyoupin.top

TS:   obj?.a?.b;  d ?? default
来源：http://vga.jinghuilouyu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fxa.9152youxi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yov.shanyushiyangkeji.top

Ruby: d&.dig(:a, :b)
来源：http://xns.tanke756.top

C#:   obj?.A?.B ?? default
来源：http://juq.feifeiyinyue.top

[H07] 断言
来源：http://dwm.sysykeji.top

Py:   assert x > 0, "必须为正"
来源：http://xlm.guannengcc.top

PHP:  assert($x > 0);
来源：http://uaz.shzxlz.cn

JS:   console.assert(x > 0);
来源：http://wvb.0kj1m.cn

TS:   console.assert(x > 0);
来源：http://lug.pycfn.com

Java: assert x > 0 : "必须为正";
来源：http://aum.yuanzhike.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rcy.c1oappe.top

Ruby: raise "必须为正" unless x > 0
来源：http://lhe.havefunace.top

C#:   Debug.Assert(x > 0);
来源：http://qqd.wangshuangyany.cn

[H08] 获取错误信息与堆栈
来源：http://rtn.nanxuanxn.top

Py:   str(e);  traceback.format_exc()
来源：http://swi.hongshengwenyu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ozl.pycfn.com

JS:   e.message;  e.stack
来源：http://nsv.hysaishi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vya.hnqzz.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ynl.shanyushiyangkeji.top

Go:   err.Error()
来源：http://qal.jinqigfzy.top

Ruby: e.message;  e.backtrace
来源：http://rsy.yueranfly.top

C#:   e.Message;  e.StackTrace
来源：http://nsi.cashguo.top

[H09] 带错误码的异常
来源：http://dub.zhijiandao.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qpn.yonumen.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://lox.aizwys.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xdz.0kj1m.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://epa.tanke756.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uwq.tian-w.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oxm.haohaochexian.top

Ruby: raise MyError.new("fail", 500)
来源：http://dur.tian-w.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wye.jlsjyb.cn

[H10] 资源自动释放
来源：http://ofj.tian-w.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://nis.yuxming.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jta.sjlbkw.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dcv.52xcode.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jxd.zhijiandao.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ivu.sjlbkw.cn

Go:   defer f.Close()
来源：http://rvs.fanxiaobao.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zxv.nwbrower.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hgv.hongshengwenyu.top

================================================================================
来源：http://edm.bjfxy.top

I. 正则表达式
来源：http://ybb.yonumen.top

================================================================================
来源：http://ebz.yj20258.top

[I01] 判断是否匹配
来源：http://pqf.guowangkeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://csm.yj202588.top

PHP:  preg_match('/\d+/', $s);
来源：http://pug.haohaochexian.top

JS:   /\d+/.test(s)
来源：http://rou.xinyue.icu

TS:   /\d+/.test(s)
来源：http://gak.pengpengdd.cyou

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wlq.zhoulong.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://knk.fzhhl.top

Ruby: s.match?(/\d+/)
来源：http://vrt.ywan-chungtsiang.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vat.mhx1999.top

[I02] 提取所有匹配
来源：http://kgu.andypj.xyz

Py:   re.findall(r"\d+", s)
来源：http://xzr.birdmap.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jwg.andypj.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cmp.zycfv.cn

TS:   s.match(/\d+/g)
来源：http://yno.hesvh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yjj.mhx1999.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zbh.vehdjk.com

Ruby: s.scan(/\d+/)
来源：http://rmn.ydzc1.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ylg.cqqwz.cn

[I03] 提取捕获分组
来源：http://skv.yj20258.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rsa.hnxiangtu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ily.yueranfly.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xcf.havefunace.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kno.nanxinkj.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dba.wangdashe.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fxn.hnxiangtu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yrc.jqgufenzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sji.daxiang520.top

[I04] 正则替换
来源：http://ari.yj202588.top

Py:   re.sub(r"\d+", "#", s)
来源：http://dlb.chenlongwang.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://out.jqgufenzy.top

JS:   s.replace(/\d+/g, "#")
来源：http://fvm.feifeiyinyue.top

TS:   s.replace(/\d+/g, "#")
来源：http://uzq.yongpay.top

Java: s.replaceAll("\\d+", "#")
来源：http://xcd.jqgufenzy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://mkb.hnxiangtu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://udq.yj20258.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fql.yueranfly.top

[I05] 按正则拆分
来源：http://qbs.zhengqikj.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xni.wangdashe.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zmk.hesvh.cn

JS:   s.split(/\s*,\s*/)
来源：http://myh.zhongyouzk.top

TS:   s.split(/\s*,\s*/)
来源：http://yul.shzxlz.cn

Java: s.split("\\s*,\\s*")
来源：http://rta.shanyushiyangkeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uoj.jlsjyb.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vjs.yuxming.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nfd.tarul.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lxe.dianchejie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ddz.sufxvd.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zbu.zhiwuduotai.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bof.jqgfzy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aia.tian-w.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lxc.jiagoushi.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://egp.yvedp.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wds.zhijiandao.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cab.guannengcc.top

[I07] 忽略大小写与多行模式
来源：http://zbj.ywan-chungtsiang.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://viy.gotoacloud.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ypa.nanxuanxn.top


<!-- 参考信息 -->