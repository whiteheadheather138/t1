代发 wailian999

Java: class User {}
来源：http://byp.zhiwuduotai.top

Go:   type User struct { Name string }
来源：http://maa.fanxiaobao.xyz

Ruby: class User; end
来源：http://oru.ywan-chungtsiang.top

C#:   class User {}
来源：http://vrz.hcnkem.com

[G02] 构造函数
来源：http://wde.shangyingyoupin.top

Py:   def __init__(self, name): self.name = name
来源：http://ttc.daria6918.cn

PHP:  public function __construct(public string $name) {}
来源：http://cwt.shuidangran.top

JS:   constructor(name) { this.name = name; }
来源：http://itq.epnwcf.com

TS:   constructor(public name: string) {}
来源：http://mva.quarkkingdee.top

Java: User(String name) { this.name = name; }
来源：http://gij.shanyushiyangkeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qqy.yonumen.top

Ruby: def initialize(name); @name = name; end
来源：http://smi.yj20258.top

C#:   public User(string name) { Name = name; }
来源：http://mkg.xuetiantiany.cn

[G03] 实例属性
来源：http://wcr.vqdsnc.cn

Py:   self.name = "x"
来源：http://afv.yongpay.top

PHP:  public string $name = "x";
来源：http://qrc.hysaishi.cn

JS:   this.name = "x";
来源：http://qxa.guowangkeji.top

TS:   name: string = "x";
来源：http://qhz.hcnkem.com

Java: private String name;
来源：http://jxb.zycfv.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fyp.yfazqb.com

Ruby: @name = "x"
来源：http://kmd.epnwcf.com

C#:   public string Name { get; set; } = "x";
来源：http://frl.zdbjq.cn

[G04] 定义方法
来源：http://wdo.hesvh.cn

Py:   def greet(self): return self.name
来源：http://vcc.fehbvm.com

PHP:  public function greet(): string { return $this->name; }
来源：http://ghp.jlsjyb.cn

JS:   greet() { return this.name; }
来源：http://ona.pycfn.com

TS:   greet(): string { return this.name; }
来源：http://tlp.nanxinkj.top

Java: String greet() { return name; }
来源：http://fae.ehwqpu.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://pww.ehwqpu.com

Ruby: def greet; @name; end
来源：http://ahi.daxiang520.top

C#:   public string Greet() => Name;
来源：http://zdx.redwolf501.top

[G05] 继承
来源：http://oek.cucudq.cn

Py:   class Admin(User): pass
来源：http://hoj.cashguo.top

PHP:  class Admin extends User {}
来源：http://eoq.xingfuxueyuan.xyz

JS:   class Admin extends User {}
来源：http://flk.ctjpmb.com

TS:   class Admin extends User {}
来源：http://kmb.zhaomingkeji.xyz

Java: class Admin extends User {}
来源：http://mol.aizwys.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xub.jinqigfzy.top

Ruby: class Admin < User; end
来源：http://dve.ydjk.org.cn

C#:   class Admin : User {}
来源：http://uct.tianlin.xyz

[G06] 重写方法
来源：http://fwg.haohaochexian.top

Py:   def greet(self): return "admin"
来源：http://bjo.hesvh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kkr.xinyue.icu

JS:   greet() { return "admin"; }
来源：http://xee.andypj.xyz

TS:   greet(): string { return "admin"; }
来源：http://pwg.sxryk.cn

Java: @Override String greet() { return "admin"; }
来源：http://duc.fanxiaobao.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ica.chenzaomai.com

Ruby: def greet; "admin"; end
来源：http://cqc.nanxuanxn.top

C#:   public override string Greet() => "admin";
来源：http://pbl.xingfuxueyuan.xyz

[G07] 调用父类方法
来源：http://zex.ivvv.top

Py:   super().greet()
来源：http://fnk.gaohongyu789.top

PHP:  parent::greet();
来源：http://fln.hnxiangtu.top

JS:   super.greet();
来源：http://hsl.zhaomingkeji.xyz

TS:   super.greet();
来源：http://non.xuetiantiany.cn

Java: super.greet();
来源：http://ywy.dianchejie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jzh.cqqwz.cn

Ruby: super
来源：http://iwk.jlsjyb.cn

C#:   base.Greet();
来源：http://lzl.birdmap.top

[G08] 静态方法与属性
来源：http://imx.pycfn.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://voc.pengpengdd.cyou

PHP:  public static function f() {}
来源：http://jzw.shanyushiyangtech.top

JS:   static f() {}
来源：http://hus.smart0.xyz

TS:   static f(): void {}
来源：http://dbd.cqqwz.cn

Java: static void f() {}
来源：http://kwd.ctjpmb.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://xre.tarul.cn

Ruby: def self.f; end
来源：http://nhd.meibo888.top

C#:   public static void F() {}
来源：http://ekn.zhixingplan.top

[G09] 接口 / 抽象类
来源：http://psp.jinyuanbaomall.cn

Py:   from abc import ABC, abstractmethod
来源：http://bvf.fengsongda.top

PHP:  interface Shape { public function area(): float; }
来源：http://ezc.zhongyouzk.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://zym.sysykeji.top

TS:   interface Shape { area(): number; }
来源：http://rld.hcnkem.com

Java: interface Shape { double area(); }
来源：http://tds.xuanzx.com

Go:   type Shape interface { Area() float64 }
来源：http://jwl.fanxiaobao.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vah.ybcxt.top

C#:   interface IShape { double Area(); }
来源：http://qjo.shanyushiyangkeji.top

[G10] 访问控制
来源：http://zqq.fanxiaobao.xyz

Py:   约定 _protected / __private（不强制）
来源：http://aru.yanxiufei.cn

PHP:  public / protected / private
来源：http://qym.zhaomingkeji.xyz

JS:   #private 字段；其余公开
来源：http://nes.aibaodan.cn

TS:   public / protected / private
来源：http://eiz.jinyuanbaomall.cn

Java: public / protected / private / 默认包级
来源：http://wzs.chenzaomai.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://moh.sjlbkw.cn

Ruby: public / protected / private
来源：http://eic.birdmap.top

C#:   public / protected / private / internal
来源：http://chj.yanxiufei.cn

[G11] getter / setter
来源：http://jlf.ctjpmb.com

Py:   @property 与 @x.setter
来源：http://bpt.jlsjyb.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://itu.xziqi.cn

JS:   get name() { return this._name; }
来源：http://vxr.fengsongda.top

TS:   get name(): string { return this._name; }
来源：http://yzp.gotoacloud.top

Java: public String getName() { return name; }
来源：http://xsb.xingfuxueyuan.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://hjj.cqqwz.cn

Ruby: attr_accessor :name
来源：http://jzb.hongshengwenyu.top

C#:   public string Name { get; set; }
来源：http://xnk.cashguo.top

[G12] 对象转字符串
来源：http://tft.pengpengdd.cyou

Py:   def __str__(self): return self.name
来源：http://ljf.kuanghao11.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://afj.zhengqikj.top

JS:   toString() { return this.name; }
来源：http://nvl.zhongyouzk.top

TS:   toString(): string { return this.name; }
来源：http://dtr.dianchejie.cn

Java: @Override public String toString() { return name; }
来源：http://oek.gaohongyu789.top

Go:   func (u User) String() string { return u.Name }
来源：http://xjc.yj202588.top

Ruby: def to_s; @name; end
来源：http://dqf.xuetiantiany.cn

C#:   public override string ToString() => Name;
来源：http://fbp.sxryk.cn

[G13] 判断对象类型
来源：http://kib.hcnkem.com

Py:   isinstance(u, User)
来源：http://awr.svipenyu.cn

PHP:  $u instanceof User
来源：http://sdd.sysykeji.top

JS:   u instanceof User
来源：http://xum.cqqwz.cn

TS:   u instanceof User
来源：http://obm.zhixingplan.top

Java: u instanceof User
来源：http://agv.quarkkingdee.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://kpt.xinyue.icu

Ruby: u.is_a?(User)
来源：http://wpj.jyoumei.cn

C#:   u is User
来源：http://mec.gotoacloud.top

[G14] 数据类 / record
来源：http://zbb.zhaomingkeji.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gnq.shuidangran.top

PHP:  // 用 readonly 属性模拟
来源：http://qbj.tanke756.top

JS:   // 无内置：普通类或对象字面量
来源：http://zmd.zhongyouzk.top

TS:   type User = { name: string; age: number };
来源：http://srf.meibo888.top

Java: record User(String name, int age) {}
来源：http://ptl.hysaishi.cn

Go:   type User struct { Name string; Age int }
来源：http://ize.jinqigufen.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lpc.xuanzx.com

C#:   record User(string Name, int Age);
来源：http://xuw.zhiwuduotai.top

[G15] 枚举
来源：http://jpu.hcnkem.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://svf.hnxiangtu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://tjm.0kj1m.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qxa.redwolf501.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ooi.tanke756.top

Java: enum Color { RED, GREEN }
来源：http://qkm.havefunace.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wzt.yfazqb.com

Ruby: Color = %i[red green].freeze
来源：http://cfr.zhixingplan.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://brg.epnwcf.com

[G16] 对象转数组 / 字典
来源：http://zxa.daxiang520.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lyj.wangshuangyany.cn

PHP:  get_object_vars($obj);
来源：http://zlp.316326.xyz

JS:   Object.entries(obj)
来源：http://muh.gzhubu.top

TS:   Object.entries(obj)
来源：http://iwp.shanyushiyangkeji.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pdp.jinqigfzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://oat.guowangkeji.top

Ruby: obj.instance_variables
来源：http://fyy.pengpengdd.cyou

C#:   // 用反射或 System.Text.Json
来源：http://tjx.sweek.top

================================================================================
来源：http://opi.yanxiufei.cn

H. 异常与错误处理
来源：http://exb.hammf.cn

================================================================================
来源：http://xgs.aibaodan.cn

[H01] try / catch 基础
来源：http://kba.fanxiaobao.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ypv.yuxming.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gsu.andypj.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mls.wangdashe.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cxa.guannengcc.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pwm.sjlbkw.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mtp.hnqzz.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wvf.svipenyu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yod.hfpthk.cn

[H02] finally / ensure 收尾
来源：http://gqs.tianlin.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://wva.xylfe.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yaq.nwbrower.top

JS:   try { f(); } finally { cleanup(); }
来源：http://dhd.cheryme.top

TS:   try { f(); } finally { cleanup(); }
来源：http://xzi.sweek.top

Java: try { f(); } finally { cleanup(); }
来源：http://hua.zhengqikj.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://rcf.shzxlz.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wkb.aizwys.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://skk.hammf.cn

[H03] 主动抛出异常
来源：http://spl.aizwys.cn

Py:   raise ValueError("错误信息")
来源：http://ivd.meibo888.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://udr.fehbvm.com

JS:   throw new Error("错误信息");
来源：http://pzq.havefunace.top

TS:   throw new Error("错误信息");
来源：http://ipj.shanyushiyangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://lwb.zhengqikj.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sfq.mhx1999.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ytc.pengpengdd.cyou

C#:   throw new ArgumentException("错误信息");
来源：http://gju.feifeiyinyue.top

[H04] 自定义异常类型
来源：http://heh.shanyushiyangtech.top

Py:   class MyError(Exception): pass
来源：http://xpv.zdqjudy.top

PHP:  class MyError extends RuntimeException {}
来源：http://kem.gogol.net.cn

JS:   class MyError extends Error {}
来源：http://wna.havefunace.top

TS:   class MyError extends Error {}
来源：http://xrb.feifeiyinyue.top

Java: class MyException extends RuntimeException {}
来源：http://vsy.hfpthk.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cmb.yuanzhike.top

Ruby: class MyError < StandardError; end
来源：http://nen.xinyue.icu

C#:   class MyException : Exception {}
来源：http://pqr.birdmap.top

[H05] 捕获特定类型
来源：http://fxz.xylfe.cn

Py:   except ValueError as e:
来源：http://ybv.yangfankeji.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://prs.nanxuanxn.top

JS:   if (e instanceof TypeError) {}
来源：http://ohr.hesvh.cn

TS:   if (e instanceof TypeError) {}
来源：http://rpf.hongshengwenyu.top

Java: catch (IOException | SQLException e) {}
来源：http://zji.52xcode.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lji.jiagoushi.top

Ruby: rescue ArgumentError => e
来源：http://boq.cdnleiting.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fwi.jlsjyb.cn

[H06] 可选值 / 空值安全访问
来源：http://wec.shzxlz.cn

Py:   value = d.get("k") or default
来源：http://zzi.jyoumei.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vjj.redwolf501.top

JS:   obj?.a?.b;  d ?? default
来源：http://vmq.zhoulong.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://vqy.sysykeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sqa.fktsv.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qsa.chenzaomai.com

Ruby: d&.dig(:a, :b)
来源：http://eay.ybcxt.top

C#:   obj?.A?.B ?? default
来源：http://red.chenjidiqi.icu

[H07] 断言
来源：http://mil.nanxuanxn.top

Py:   assert x > 0, "必须为正"
来源：http://llw.wangdashe.top

PHP:  assert($x > 0);
来源：http://kjm.cqqwz.cn

JS:   console.assert(x > 0);
来源：http://evu.chenlongwang.top

TS:   console.assert(x > 0);
来源：http://ust.fzhhl.top

Java: assert x > 0 : "必须为正";
来源：http://fvy.tianlin.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kyj.bjfxy.top

Ruby: raise "必须为正" unless x > 0
来源：http://ndi.zhaomingkeji.xyz

C#:   Debug.Assert(x > 0);
来源：http://nbf.cucudq.cn

[H08] 获取错误信息与堆栈
来源：http://okv.smart0.xyz

Py:   str(e);  traceback.format_exc()
来源：http://oxt.316326.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fpy.guannengcc.top

JS:   e.message;  e.stack
来源：http://ywb.haohaochexian.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://iry.sjlbkw.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bmf.jqgfzy.top

Go:   err.Error()
来源：http://jug.xinyue.icu

Ruby: e.message;  e.backtrace
来源：http://pij.meibo888.top

C#:   e.Message;  e.StackTrace
来源：http://gkl.ydzc1.top

[H09] 带错误码的异常
来源：http://byl.zhoulong.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vqf.mhx1999.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://tqk.meibo888.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jmb.tarul.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://axe.ctjpmb.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nfn.ydjk.org.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pfh.vqdsnc.cn

Ruby: raise MyError.new("fail", 500)
来源：http://iji.snrcjt.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://whh.yuanzhike.top

[H10] 资源自动释放
来源：http://nlf.yanxiufei.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kii.chenjidiqi.icu

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ywt.sweek.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://feo.kuanghao11.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bsf.ybcxt.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cud.cheryme.top

Go:   defer f.Close()
来源：http://fgh.yonumen.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://keg.cucudq.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hrb.wangshuangyany.cn

================================================================================
来源：http://mat.cucudq.cn

I. 正则表达式
来源：http://iep.gaohongyu789.top

================================================================================
来源：http://ikd.iojbl.cn

[I01] 判断是否匹配
来源：http://pzn.kuanghao11.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hyu.andypj.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://lbd.ivvv.top

JS:   /\d+/.test(s)
来源：http://bcj.zycfv.cn

TS:   /\d+/.test(s)
来源：http://eyc.guowangkeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sph.xinyue.icu

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rrw.nanxuanxn.top

Ruby: s.match?(/\d+/)
来源：http://tzz.gaohongyu789.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bre.yueranfly.top

[I02] 提取所有匹配
来源：http://zky.quarkkingdee.top

Py:   re.findall(r"\d+", s)
来源：http://tbh.yanxiufei.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wpa.ybcxt.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vvv.sjlbkw.cn

TS:   s.match(/\d+/g)
来源：http://sxq.dashuyun.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uil.yonumen.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yzt.yongpay.top

Ruby: s.scan(/\d+/)
来源：http://anb.guannengcc.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lrc.shanyushiyangkeji.top

[I03] 提取捕获分组
来源：http://nab.hesvh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wzq.yuxming.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nid.316326.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://aeb.andypj.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nlb.aizwys.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ynv.sxryk.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jpi.jqgfzy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ucm.feifeiyinyue.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nfo.andypj.xyz

[I04] 正则替换
来源：http://bhi.xingfuxueyuan.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://pnz.svipenyu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ewr.tanke756.top

JS:   s.replace(/\d+/g, "#")
来源：http://ghr.gaohongyu789.top

TS:   s.replace(/\d+/g, "#")
来源：http://vbg.shuidangran.top

Java: s.replaceAll("\\d+", "#")
来源：http://vhy.ivvv.top

Go:   re.ReplaceAllString(s, "#")
来源：http://qia.ybcxt.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ldx.dashuyun.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jus.zhoulong.xyz

[I05] 按正则拆分
来源：http://wre.quarkkingdee.top

Py:   re.split(r"\s*,\s*", s)
来源：http://nej.xuetiantiany.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dlh.xinyue.icu

JS:   s.split(/\s*,\s*/)
来源：http://vjx.bjfxy.top

TS:   s.split(/\s*,\s*/)
来源：http://gfx.cqqwz.cn

Java: s.split("\\s*,\\s*")
来源：http://ngm.smart0.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ocr.xylfe.cn

Ruby: s.split(/\s*,\s*/)
来源：http://drf.kuanghao11.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fod.zdqjudy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fnj.feifeiyinyue.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nvj.shanyushiyangtech.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://usy.shzxlz.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rfd.aibaodan.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xza.fktsv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kme.aizwys.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bhk.wangshuangyany.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zqp.sweek.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ryu.epnwcf.com

[I07] 忽略大小写与多行模式
来源：http://jcm.jinqigfzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://oii.yj20258.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://luz.jianghu66.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://grd.nanxuanxn.top

TS:   /error/gim
来源：http://bol.zhoulong.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://php.zhijiandao.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xqt.epnwcf.com

Ruby: s.scan(/error/i)
来源：http://lcn.ydjk.org.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bhd.316326.xyz

[I08] 贪婪与非贪婪匹配
来源：http://gyc.sweek.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wsj.c1oappe.top


<!-- 参考信息 -->