代发 wailian999

Java: class User {}
来源：http://dkc.52xcode.cn

Go:   type User struct { Name string }
来源：http://nmd.cqqwz.cn

Ruby: class User; end
来源：http://dle.daria6918.cn

C#:   class User {}
来源：http://hrr.yj202588.top

[G02] 构造函数
来源：http://wgl.cdnleiting.top

Py:   def __init__(self, name): self.name = name
来源：http://dnp.shanyushiyangtech.top

PHP:  public function __construct(public string $name) {}
来源：http://yet.zhaomingkeji.xyz

JS:   constructor(name) { this.name = name; }
来源：http://abj.tarul.cn

TS:   constructor(public name: string) {}
来源：http://bnt.zhixingplan.top

Java: User(String name) { this.name = name; }
来源：http://ntm.xinyue.icu

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fsa.yangfankeji.com

Ruby: def initialize(name); @name = name; end
来源：http://uht.hysaishi.cn

C#:   public User(string name) { Name = name; }
来源：http://qxs.fehbvm.com

[G03] 实例属性
来源：http://mnz.xuanzx.com

Py:   self.name = "x"
来源：http://bfy.pycfn.com

PHP:  public string $name = "x";
来源：http://zzh.52xcode.cn

JS:   this.name = "x";
来源：http://fke.zhongyouzk.top

TS:   name: string = "x";
来源：http://zfj.hywenlv.cn

Java: private String name;
来源：http://esp.jlsjyb.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sia.ydjk.org.cn

Ruby: @name = "x"
来源：http://dww.jinyuanbaomall.cn

C#:   public string Name { get; set; } = "x";
来源：http://yqj.yongpay.top

[G04] 定义方法
来源：http://tjq.xinyue.icu

Py:   def greet(self): return self.name
来源：http://xyw.redwolf501.top

PHP:  public function greet(): string { return $this->name; }
来源：http://mpc.fzhhl.top

JS:   greet() { return this.name; }
来源：http://del.fktsv.cn

TS:   greet(): string { return this.name; }
来源：http://itw.jinghuilouyu.cn

Java: String greet() { return name; }
来源：http://szd.yfazqb.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://pxa.zhongyouzk.top

Ruby: def greet; @name; end
来源：http://idm.fktsv.cn

C#:   public string Greet() => Name;
来源：http://pcp.bbcook.cn

[G05] 继承
来源：http://fed.jinyuanbaomall.cn

Py:   class Admin(User): pass
来源：http://mxm.sweek.top

PHP:  class Admin extends User {}
来源：http://wxa.chenzaomai.com

JS:   class Admin extends User {}
来源：http://bej.sxryk.cn

TS:   class Admin extends User {}
来源：http://zzs.jyoumei.cn

Java: class Admin extends User {}
来源：http://qlk.birdmap.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bds.jqgfzy.top

Ruby: class Admin < User; end
来源：http://fpb.havefunace.top

C#:   class Admin : User {}
来源：http://ekn.jqgufenzy.top

[G06] 重写方法
来源：http://izu.jlsjyb.cn

Py:   def greet(self): return "admin"
来源：http://uxc.cheryme.top

PHP:  public function greet(): string { return "admin"; }
来源：http://obb.zhaomingkeji.xyz

JS:   greet() { return "admin"; }
来源：http://oed.jlsjyb.cn

TS:   greet(): string { return "admin"; }
来源：http://rjp.epnwcf.com

Java: @Override String greet() { return "admin"; }
来源：http://fbf.yongpay.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sfj.yuanzhike.top

Ruby: def greet; "admin"; end
来源：http://ahb.pycfn.com

C#:   public override string Greet() => "admin";
来源：http://rle.yvedp.cn

[G07] 调用父类方法
来源：http://zjz.nanxuanxn.top

Py:   super().greet()
来源：http://iry.ydzc1.top

PHP:  parent::greet();
来源：http://yla.gogol.net.cn

JS:   super.greet();
来源：http://fcb.c1oappe.top

TS:   super.greet();
来源：http://pbb.c1oappe.top

Java: super.greet();
来源：http://ryr.hesvh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pfx.jiagoushi.top

Ruby: super
来源：http://qjx.vqdsnc.cn

C#:   base.Greet();
来源：http://xtl.316326.xyz

[G08] 静态方法与属性
来源：http://xsm.jqgfzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bfj.ctjpmb.com

PHP:  public static function f() {}
来源：http://txg.tarul.cn

JS:   static f() {}
来源：http://edc.chenzaomai.com

TS:   static f(): void {}
来源：http://vel.cashguo.top

Java: static void f() {}
来源：http://mfj.wangshuangyany.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ldg.xingfuxueyuan.xyz

Ruby: def self.f; end
来源：http://klz.cheryme.top

C#:   public static void F() {}
来源：http://zhs.gotoacloud.top

[G09] 接口 / 抽象类
来源：http://xwf.mhx1999.top

Py:   from abc import ABC, abstractmethod
来源：http://dbn.gzhubu.top

PHP:  interface Shape { public function area(): float; }
来源：http://ibv.jinqigfzy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://gil.hesvh.cn

TS:   interface Shape { area(): number; }
来源：http://dmt.svipenyu.cn

Java: interface Shape { double area(); }
来源：http://mkr.quarkkingdee.top

Go:   type Shape interface { Area() float64 }
来源：http://uwp.shzxlz.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rvc.epnwcf.com

C#:   interface IShape { double Area(); }
来源：http://glc.ivvv.top

[G10] 访问控制
来源：http://nay.jqgfzy.top

Py:   约定 _protected / __private（不强制）
来源：http://yvh.ivvv.top

PHP:  public / protected / private
来源：http://lbb.shuidangran.top

JS:   #private 字段；其余公开
来源：http://xtm.bjfxy.top

TS:   public / protected / private
来源：http://ndl.zhiwuduotai.top

Java: public / protected / private / 默认包级
来源：http://tah.chenzaomai.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://owk.xziqi.cn

Ruby: public / protected / private
来源：http://fig.dianchejie.cn

C#:   public / protected / private / internal
来源：http://eer.9152youxi.cn

[G11] getter / setter
来源：http://xbz.xuanzx.com

Py:   @property 与 @x.setter
来源：http://dnt.vehdjk.com

PHP:  public function getName(): string { return $this->name; }
来源：http://yke.ctjpmb.com

JS:   get name() { return this._name; }
来源：http://rpa.redwolf501.top

TS:   get name(): string { return this._name; }
来源：http://wma.meibo888.top

Java: public String getName() { return name; }
来源：http://kri.tian-w.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://pcw.sufxvd.cn

Ruby: attr_accessor :name
来源：http://ohc.wangdashe.top

C#:   public string Name { get; set; }
来源：http://gcm.ydzc1.top

[G12] 对象转字符串
来源：http://atq.birdmap.top

Py:   def __str__(self): return self.name
来源：http://uba.jianghu66.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ttc.hongshengwenyu.top

JS:   toString() { return this.name; }
来源：http://plt.yj20258888.top

TS:   toString(): string { return this.name; }
来源：http://pjx.pengpengdd.cyou

Java: @Override public String toString() { return name; }
来源：http://vrm.ydzc1.top

Go:   func (u User) String() string { return u.Name }
来源：http://duw.gotoacloud.top

Ruby: def to_s; @name; end
来源：http://fsq.jqgfzy.top

C#:   public override string ToString() => Name;
来源：http://zvz.xylfe.cn

[G13] 判断对象类型
来源：http://lzn.guowangkeji.top

Py:   isinstance(u, User)
来源：http://vnm.hysaishi.cn

PHP:  $u instanceof User
来源：http://cxu.nanxinkj.top

JS:   u instanceof User
来源：http://tvf.ppjwa.cn

TS:   u instanceof User
来源：http://suw.316326.xyz

Java: u instanceof User
来源：http://zfu.sxryk.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kwv.yangfankeji.com

Ruby: u.is_a?(User)
来源：http://qkv.hysaishi.cn

C#:   u is User
来源：http://pyo.dianchejie.cn

[G14] 数据类 / record
来源：http://ary.c1oappe.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pdu.guowangkeji.top

PHP:  // 用 readonly 属性模拟
来源：http://bar.fktsv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lym.hcnkem.com

TS:   type User = { name: string; age: number };
来源：http://col.gotoacloud.top

Java: record User(String name, int age) {}
来源：http://hgn.fanxiaobao.xyz

Go:   type User struct { Name string; Age int }
来源：http://fxo.havefunace.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hky.dianchejie.cn

C#:   record User(string Name, int Age);
来源：http://shs.ivvv.top

[G15] 枚举
来源：http://keu.yj202588.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jmd.ydzc1.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://zrk.nwbrower.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vmb.nwbrower.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bdy.birdmap.top

Java: enum Color { RED, GREEN }
来源：http://jij.ydzc1.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nao.dashuyun.cn

Ruby: Color = %i[red green].freeze
来源：http://kde.hammf.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lmv.yvedp.cn

[G16] 对象转数组 / 字典
来源：http://sbe.tianlin.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uqn.jiagoushi.top

PHP:  get_object_vars($obj);
来源：http://mga.yfazqb.com

JS:   Object.entries(obj)
来源：http://sqd.haohaochexian.top

TS:   Object.entries(obj)
来源：http://mqa.yuanzhike.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vpw.fehbvm.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://mne.kuanghao11.cn

Ruby: obj.instance_variables
来源：http://ayj.sweek.top

C#:   // 用反射或 System.Text.Json
来源：http://jzj.hywenlv.cn

================================================================================
来源：http://hth.guowangkeji.top

H. 异常与错误处理
来源：http://gbo.dashuyun.cn

================================================================================
来源：http://aly.xuetiantiany.cn

[H01] try / catch 基础
来源：http://cma.ydjk.org.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yqs.fengsongda.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qre.hysaishi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nck.aizwys.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vqf.jlsjyb.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jre.jqgfzy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://asb.bbcook.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rzh.aizwys.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jyj.9152youxi.cn

[H02] finally / ensure 收尾
来源：http://yla.sweek.top

Py:   try: f()⏎finally: cleanup()
来源：http://vjg.aibaodan.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hpw.bbcook.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ltx.redwolf501.top

TS:   try { f(); } finally { cleanup(); }
来源：http://fye.tarul.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bdz.yuanzhike.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://fbx.ydjk.org.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sat.yueranfly.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://aml.gogol.net.cn

[H03] 主动抛出异常
来源：http://rou.9152youxi.cn

Py:   raise ValueError("错误信息")
来源：http://gbq.zhiwuduotai.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rnd.aibaodan.cn

JS:   throw new Error("错误信息");
来源：http://xtb.316326.xyz

TS:   throw new Error("错误信息");
来源：http://aex.jlsjyb.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xcu.pengpengdd.cyou

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wsz.yonumen.top

Ruby: raise ArgumentError, "错误信息"
来源：http://jfj.xuanzx.com

C#:   throw new ArgumentException("错误信息");
来源：http://ejc.jlsjyb.cn

[H04] 自定义异常类型
来源：http://cgb.tanke756.top

Py:   class MyError(Exception): pass
来源：http://ljz.cucudq.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ojx.yonumen.top

JS:   class MyError extends Error {}
来源：http://zny.fktsv.cn

TS:   class MyError extends Error {}
来源：http://pjv.yfazqb.com

Java: class MyException extends RuntimeException {}
来源：http://ira.pengpengdd.cyou

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gkx.gotoacloud.top

Ruby: class MyError < StandardError; end
来源：http://lxz.shanyushiyangkeji.top

C#:   class MyException : Exception {}
来源：http://xkf.yfazqb.com

[H05] 捕获特定类型
来源：http://pam.zhoulong.xyz

Py:   except ValueError as e:
来源：http://cyi.jiagoushi.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://iqm.andypj.xyz

JS:   if (e instanceof TypeError) {}
来源：http://clh.ydjk.org.cn

TS:   if (e instanceof TypeError) {}
来源：http://hwt.c1oappe.top

Java: catch (IOException | SQLException e) {}
来源：http://yyq.aizwys.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://aam.ybcxt.top

Ruby: rescue ArgumentError => e
来源：http://mrn.svipenyu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hyn.dashuyun.cn

[H06] 可选值 / 空值安全访问
来源：http://qik.ywan-chungtsiang.top

Py:   value = d.get("k") or default
来源：http://izj.smart0.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://eou.0kj1m.cn

JS:   obj?.a?.b;  d ?? default
来源：http://tce.yj20258888.top

TS:   obj?.a?.b;  d ?? default
来源：http://veg.xziqi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://spi.ydjk.org.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mjj.xuetiantiany.cn

Ruby: d&.dig(:a, :b)
来源：http://eoi.zhongyouzk.top

C#:   obj?.A?.B ?? default
来源：http://rcj.316326.xyz

[H07] 断言
来源：http://pox.quarkkingdee.top

Py:   assert x > 0, "必须为正"
来源：http://hhy.xuanzx.com

PHP:  assert($x > 0);
来源：http://ojk.ehwqpu.com

JS:   console.assert(x > 0);
来源：http://jwn.vqdsnc.cn

TS:   console.assert(x > 0);
来源：http://dxv.quarkkingdee.top

Java: assert x > 0 : "必须为正";
来源：http://kwe.aizwys.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pua.cheryme.top

Ruby: raise "必须为正" unless x > 0
来源：http://tqg.ydjk.org.cn

C#:   Debug.Assert(x > 0);
来源：http://iqx.fanxiaobao.xyz

[H08] 获取错误信息与堆栈
来源：http://uiw.9152youxi.cn

Py:   str(e);  traceback.format_exc()
来源：http://cgy.jianghu66.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xaz.yueranfly.top

JS:   e.message;  e.stack
来源：http://sgl.vqdsnc.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yqq.bbcook.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://khi.sjlbkw.cn

Go:   err.Error()
来源：http://pkd.hammf.cn

Ruby: e.message;  e.backtrace
来源：http://nvf.guannengcc.top

C#:   e.Message;  e.StackTrace
来源：http://uff.cashguo.top

[H09] 带错误码的异常
来源：http://nlv.jinghuilouyu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gus.feifeiyinyue.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://udg.nanxuanxn.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qur.jqgufenzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pkj.gaohongyu789.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sch.zhengqikj.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ybt.316326.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://znw.yonumen.top

C#:   // 自定义异常类中加 Code 属性
来源：http://rmd.yongpay.top

[H10] 资源自动释放
来源：http://fzr.zdqjudy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://anr.dianchejie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sbv.chenzaomai.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pow.zhixingplan.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gpi.ehwqpu.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vwv.jinqigfzy.top

Go:   defer f.Close()
来源：http://xke.ppjwa.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gdy.sjlbkw.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ekp.sxryk.cn

================================================================================
来源：http://cgw.9152youxi.cn

I. 正则表达式
来源：http://ozl.tianlin.xyz

================================================================================
来源：http://cni.yuanzhike.top

[I01] 判断是否匹配
来源：http://doj.sufxvd.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ejs.xinyue.icu

PHP:  preg_match('/\d+/', $s);
来源：http://sil.yonumen.top

JS:   /\d+/.test(s)
来源：http://nwc.hywenlv.cn

TS:   /\d+/.test(s)
来源：http://haf.shanyushiyangtech.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rpb.jqgufenzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://swt.jinqigfzy.top

Ruby: s.match?(/\d+/)
来源：http://ztz.pengpengdd.cyou

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bnb.feifeiyinyue.top

[I02] 提取所有匹配
来源：http://mbb.hammf.cn

Py:   re.findall(r"\d+", s)
来源：http://rnm.jinyuanbaomall.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wwb.zhiwuduotai.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zfe.sxryk.cn

TS:   s.match(/\d+/g)
来源：http://wdv.ivvv.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hid.ehwqpu.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kry.zdqjudy.top

Ruby: s.scan(/\d+/)
来源：http://lyq.tanke756.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://krw.zhengqikj.top

[I03] 提取捕获分组
来源：http://dag.yonumen.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kuq.yj20258.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vhn.feifeiyinyue.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oif.hammf.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nlr.svipenyu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jtu.hesvh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zsm.yonumen.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qmo.birdmap.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kgc.zycfv.cn

[I04] 正则替换
来源：http://ixq.zhaomingkeji.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://thu.chenlongwang.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lkm.gogol.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kwl.andypj.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://xca.zycfv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wxb.aizwys.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://uft.0kj1m.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hhl.wangshuangyany.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wfd.zhongyouzk.top

[I05] 按正则拆分
来源：http://yng.iojbl.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ati.jinghuilouyu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://axt.nanxinkj.top

JS:   s.split(/\s*,\s*/)
来源：http://toz.uphjek.com

TS:   s.split(/\s*,\s*/)
来源：http://kkd.pycfn.com

Java: s.split("\\s*,\\s*")
来源：http://tsx.tian-w.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hoq.xuanzx.com

Ruby: s.split(/\s*,\s*/)
来源：http://ger.zhongyouzk.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mfq.ydzc1.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xqg.nanxuanxn.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fth.yfazqb.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://moq.yuxming.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rhb.sysykeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://enh.uphjek.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://swz.nwbrower.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ylr.cheryme.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gde.shzxlz.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lgo.mhx1999.top

[I07] 忽略大小写与多行模式
来源：http://uzb.xuanzx.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bsl.jianghu66.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kpy.chenjidiqi.icu

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ann.316326.xyz

TS:   /error/gim
来源：http://agy.yj20258.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pzm.c1oappe.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mvm.dianchejie.cn

Ruby: s.scan(/error/i)
来源：http://rxe.dashuyun.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lqg.quarkkingdee.top

[I08] 贪婪与非贪婪匹配
来源：http://plr.wangshuangyany.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://smi.nanxuanxn.top


<!-- 参考信息 -->