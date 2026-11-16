代发 wailian999

Java: class User {}
来源：http://xgb.ywan-chungtsiang.top

Go:   type User struct { Name string }
来源：http://xvu.gzhubu.top

Ruby: class User; end
来源：http://uuc.nwbrower.top

C#:   class User {}
来源：http://fut.xziqi.cn

[G02] 构造函数
来源：http://xhi.52xcode.cn

Py:   def __init__(self, name): self.name = name
来源：http://hxe.aibaodan.cn

PHP:  public function __construct(public string $name) {}
来源：http://xiy.jinghuilouyu.cn

JS:   constructor(name) { this.name = name; }
来源：http://cod.yangfankeji.com

TS:   constructor(public name: string) {}
来源：http://ypu.hnxiangtu.top

Java: User(String name) { this.name = name; }
来源：http://yze.dashuyun.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fal.bbcook.cn

Ruby: def initialize(name); @name = name; end
来源：http://rvg.xingfuxueyuan.xyz

C#:   public User(string name) { Name = name; }
来源：http://inh.wangshuangyany.cn

[G03] 实例属性
来源：http://jov.zycfv.cn

Py:   self.name = "x"
来源：http://ppe.bjfxy.top

PHP:  public string $name = "x";
来源：http://crh.yueranfly.top

JS:   this.name = "x";
来源：http://vdu.jinghuilouyu.cn

TS:   name: string = "x";
来源：http://uxs.hfpthk.cn

Java: private String name;
来源：http://jzs.hongshengwenyu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sum.zycfv.cn

Ruby: @name = "x"
来源：http://tkn.yuxming.cn

C#:   public string Name { get; set; } = "x";
来源：http://uvk.fzhhl.top

[G04] 定义方法
来源：http://tiw.xuanzx.com

Py:   def greet(self): return self.name
来源：http://kcw.hcnkem.com

PHP:  public function greet(): string { return $this->name; }
来源：http://rwx.zdbjq.cn

JS:   greet() { return this.name; }
来源：http://tsn.52xcode.cn

TS:   greet(): string { return this.name; }
来源：http://cyu.sjlbkw.cn

Java: String greet() { return name; }
来源：http://tqm.daria6918.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://dkf.havefunace.top

Ruby: def greet; @name; end
来源：http://wxu.bbcook.cn

C#:   public string Greet() => Name;
来源：http://ygj.jlsjyb.cn

[G05] 继承
来源：http://uvf.jqgfzy.top

Py:   class Admin(User): pass
来源：http://oyl.yuxming.cn

PHP:  class Admin extends User {}
来源：http://fue.zhiwuduotai.top

JS:   class Admin extends User {}
来源：http://wpe.smart0.xyz

TS:   class Admin extends User {}
来源：http://rsr.cashguo.top

Java: class Admin extends User {}
来源：http://qux.jiagoushi.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dei.zhijiandao.cn

Ruby: class Admin < User; end
来源：http://ndf.yvedp.cn

C#:   class Admin : User {}
来源：http://cqs.guowangkeji.top

[G06] 重写方法
来源：http://was.nwbrower.top

Py:   def greet(self): return "admin"
来源：http://iqz.sjlbkw.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qbs.jiagoushi.top

JS:   greet() { return "admin"; }
来源：http://lwy.aizwys.cn

TS:   greet(): string { return "admin"; }
来源：http://moo.cashguo.top

Java: @Override String greet() { return "admin"; }
来源：http://ymc.svipenyu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mcp.wangshuangyany.cn

Ruby: def greet; "admin"; end
来源：http://pex.jinghuilouyu.cn

C#:   public override string Greet() => "admin";
来源：http://cgd.svipenyu.cn

[G07] 调用父类方法
来源：http://qrm.yueranfly.top

Py:   super().greet()
来源：http://qyb.gogol.net.cn

PHP:  parent::greet();
来源：http://gxl.guowangkeji.top

JS:   super.greet();
来源：http://ejf.ctjpmb.com

TS:   super.greet();
来源：http://sfk.shanyushiyangkeji.top

Java: super.greet();
来源：http://pme.fehbvm.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wir.chenlongwang.top

Ruby: super
来源：http://oav.jinqigfzy.top

C#:   base.Greet();
来源：http://ubx.shuidangran.top

[G08] 静态方法与属性
来源：http://oet.birdmap.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hpo.jyoumei.cn

PHP:  public static function f() {}
来源：http://qne.ctjpmb.com

JS:   static f() {}
来源：http://fse.hcnkem.com

TS:   static f(): void {}
来源：http://ryo.jinghuilouyu.cn

Java: static void f() {}
来源：http://veu.andypj.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://ehx.hnqzz.top

Ruby: def self.f; end
来源：http://pwb.dashuyun.cn

C#:   public static void F() {}
来源：http://tvm.meibo888.top

[G09] 接口 / 抽象类
来源：http://ggb.ydzc1.top

Py:   from abc import ABC, abstractmethod
来源：http://bhs.hywenlv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zaw.hnqzz.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://cxi.ydzc1.top

TS:   interface Shape { area(): number; }
来源：http://bon.zhaomingkeji.xyz

Java: interface Shape { double area(); }
来源：http://ayj.nanxuanxn.top

Go:   type Shape interface { Area() float64 }
来源：http://unm.yangfankeji.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://exg.havefunace.top

C#:   interface IShape { double Area(); }
来源：http://gkh.cashguo.top

[G10] 访问控制
来源：http://gwy.yuanzhike.top

Py:   约定 _protected / __private（不强制）
来源：http://kbp.ehwqpu.com

PHP:  public / protected / private
来源：http://ajo.feifeiyinyue.top

JS:   #private 字段；其余公开
来源：http://gdq.birdmap.top

TS:   public / protected / private
来源：http://swb.xingfuxueyuan.xyz

Java: public / protected / private / 默认包级
来源：http://sdi.iojbl.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://kht.ivvv.top

Ruby: public / protected / private
来源：http://jef.nwbrower.top

C#:   public / protected / private / internal
来源：http://bik.hcnkem.com

[G11] getter / setter
来源：http://gmo.wangdashe.top

Py:   @property 与 @x.setter
来源：http://fdv.redwolf501.top

PHP:  public function getName(): string { return $this->name; }
来源：http://pji.jinghuilouyu.cn

JS:   get name() { return this._name; }
来源：http://lox.xuetiantiany.cn

TS:   get name(): string { return this._name; }
来源：http://khi.aibaodan.cn

Java: public String getName() { return name; }
来源：http://yzn.zhongyouzk.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://uqn.hongshengwenyu.top

Ruby: attr_accessor :name
来源：http://smk.yangfankeji.com

C#:   public string Name { get; set; }
来源：http://uut.wangshuangyany.cn

[G12] 对象转字符串
来源：http://qzq.shanyushiyangkeji.top

Py:   def __str__(self): return self.name
来源：http://ham.xuanzx.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://ckl.zhoulong.xyz

JS:   toString() { return this.name; }
来源：http://wkh.hcnkem.com

TS:   toString(): string { return this.name; }
来源：http://hzn.wangshuangyany.cn

Java: @Override public String toString() { return name; }
来源：http://mbk.zycfv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://col.snrcjt.cn

Ruby: def to_s; @name; end
来源：http://sve.dashuyun.cn

C#:   public override string ToString() => Name;
来源：http://tdu.tian-w.cn

[G13] 判断对象类型
来源：http://qeh.ybcxt.top

Py:   isinstance(u, User)
来源：http://qqi.52xcode.cn

PHP:  $u instanceof User
来源：http://kzt.ppjwa.cn

JS:   u instanceof User
来源：http://unl.hongshengwenyu.top

TS:   u instanceof User
来源：http://pvg.yj20258.top

Java: u instanceof User
来源：http://smz.snrcjt.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ydb.redwolf501.top

Ruby: u.is_a?(User)
来源：http://lho.zdbjq.cn

C#:   u is User
来源：http://doe.cheryme.top

[G14] 数据类 / record
来源：http://par.sxryk.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qro.zhaomingkeji.xyz

PHP:  // 用 readonly 属性模拟
来源：http://xqe.redwolf501.top

JS:   // 无内置：普通类或对象字面量
来源：http://mhq.jlsjyb.cn

TS:   type User = { name: string; age: number };
来源：http://mju.havefunace.top

Java: record User(String name, int age) {}
来源：http://olh.yuanzhike.top

Go:   type User struct { Name string; Age int }
来源：http://awp.sjlbkw.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fye.tianlin.xyz

C#:   record User(string Name, int Age);
来源：http://zrp.yvedp.cn

[G15] 枚举
来源：http://mro.ehwqpu.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fyu.hongshengwenyu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://amo.fanxiaobao.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://woz.shangyingyoupin.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://add.cucudq.cn

Java: enum Color { RED, GREEN }
来源：http://hgd.shuidangran.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uhy.pengpengdd.cyou

Ruby: Color = %i[red green].freeze
来源：http://oxu.tianlin.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dxy.zhaomingkeji.xyz

[G16] 对象转数组 / 字典
来源：http://bma.xylfe.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vou.yuxming.cn

PHP:  get_object_vars($obj);
来源：http://vyk.cqqwz.cn

JS:   Object.entries(obj)
来源：http://cyp.sufxvd.cn

TS:   Object.entries(obj)
来源：http://nfo.jinqigufen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://unq.zycfv.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://smx.nanxuanxn.top

Ruby: obj.instance_variables
来源：http://sdw.shuidangran.top

C#:   // 用反射或 System.Text.Json
来源：http://ckc.zhiwuduotai.top

================================================================================
来源：http://rfl.cqqwz.cn

H. 异常与错误处理
来源：http://ukp.aibaodan.cn

================================================================================
来源：http://xck.mhx1999.top

[H01] try / catch 基础
来源：http://smf.sysykeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://act.quarkkingdee.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://txm.fanxiaobao.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://asl.ybcxt.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fum.havefunace.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mfh.vehdjk.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ats.xziqi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vsm.tianlin.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zks.hywenlv.cn

[H02] finally / ensure 收尾
来源：http://vyo.bbcook.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ihp.gzhubu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://tod.jinqigfzy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://oas.sjlbkw.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://wvh.dashuyun.cn

Java: try { f(); } finally { cleanup(); }
来源：http://rbg.haohaochexian.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://uap.redwolf501.top

Ruby: begin; f; ensure; cleanup; end
来源：http://uua.0kj1m.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xgj.yj202588.top

[H03] 主动抛出异常
来源：http://aed.jqgfzy.top

Py:   raise ValueError("错误信息")
来源：http://xul.chenzaomai.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cru.shzxlz.cn

JS:   throw new Error("错误信息");
来源：http://zhy.jlsjyb.cn

TS:   throw new Error("错误信息");
来源：http://clv.bbcook.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nto.nanxinkj.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ham.zhixingplan.top

Ruby: raise ArgumentError, "错误信息"
来源：http://nde.zhixingplan.top

C#:   throw new ArgumentException("错误信息");
来源：http://wyo.wangshuangyany.cn

[H04] 自定义异常类型
来源：http://puh.xinyue.icu

Py:   class MyError(Exception): pass
来源：http://rgd.ivvv.top

PHP:  class MyError extends RuntimeException {}
来源：http://zwd.vqdsnc.cn

JS:   class MyError extends Error {}
来源：http://zye.zhijiandao.cn

TS:   class MyError extends Error {}
来源：http://tkh.redwolf501.top

Java: class MyException extends RuntimeException {}
来源：http://mgl.shuidangran.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jda.316326.xyz

Ruby: class MyError < StandardError; end
来源：http://cac.yanxiufei.cn

C#:   class MyException : Exception {}
来源：http://mln.yuxming.cn

[H05] 捕获特定类型
来源：http://yha.jyoumei.cn

Py:   except ValueError as e:
来源：http://kua.jinqigfzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://upb.cashguo.top

JS:   if (e instanceof TypeError) {}
来源：http://hfi.fktsv.cn

TS:   if (e instanceof TypeError) {}
来源：http://wnz.gzhubu.top

Java: catch (IOException | SQLException e) {}
来源：http://kyi.gzhubu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dip.hesvh.cn

Ruby: rescue ArgumentError => e
来源：http://jaa.xylfe.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vlc.sjlbkw.cn

[H06] 可选值 / 空值安全访问
来源：http://evr.zycfv.cn

Py:   value = d.get("k") or default
来源：http://yks.iojbl.cn

PHP:  $v = $d["k"] ?? null;
来源：http://skr.chenzaomai.com

JS:   obj?.a?.b;  d ?? default
来源：http://qub.gotoacloud.top

TS:   obj?.a?.b;  d ?? default
来源：http://lhf.zdqjudy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pte.yanxiufei.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jum.zhengqikj.top

Ruby: d&.dig(:a, :b)
来源：http://app.xinyue.icu

C#:   obj?.A?.B ?? default
来源：http://ilt.tian-w.cn

[H07] 断言
来源：http://eaz.aibaodan.cn

Py:   assert x > 0, "必须为正"
来源：http://exe.ywan-chungtsiang.top

PHP:  assert($x > 0);
来源：http://sul.nwbrower.top

JS:   console.assert(x > 0);
来源：http://xan.jqgfzy.top

TS:   console.assert(x > 0);
来源：http://tob.sweek.top

Java: assert x > 0 : "必须为正";
来源：http://mod.hesvh.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://enf.chenlongwang.top

Ruby: raise "必须为正" unless x > 0
来源：http://dee.dianchejie.cn

C#:   Debug.Assert(x > 0);
来源：http://aim.tian-w.cn

[H08] 获取错误信息与堆栈
来源：http://nkl.havefunace.top

Py:   str(e);  traceback.format_exc()
来源：http://wbt.fengsongda.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hob.guowangkeji.top

JS:   e.message;  e.stack
来源：http://juu.meibo888.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ozf.mhx1999.top

Java: e.getMessage();  e.printStackTrace()
来源：http://pid.yj20258888.top

Go:   err.Error()
来源：http://jox.zhaomingkeji.xyz

Ruby: e.message;  e.backtrace
来源：http://usj.yfazqb.com

C#:   e.Message;  e.StackTrace
来源：http://xog.aizwys.cn

[H09] 带错误码的异常
来源：http://hqo.cucudq.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pzh.yfazqb.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://bcw.xuanzx.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ttp.epnwcf.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ycf.yj20258888.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ocn.shanyushiyangkeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qor.yuanzhike.top

Ruby: raise MyError.new("fail", 500)
来源：http://chi.xuanzx.com

C#:   // 自定义异常类中加 Code 属性
来源：http://hqw.yfazqb.com

[H10] 资源自动释放
来源：http://gws.jinghuilouyu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://cvp.zdbjq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://awd.guannengcc.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xje.yonumen.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tud.havefunace.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jde.redwolf501.top

Go:   defer f.Close()
来源：http://zek.hesvh.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fyr.zhengqikj.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nqp.kuanghao11.cn

================================================================================
来源：http://vff.bbcook.cn

I. 正则表达式
来源：http://rqu.9152youxi.cn

================================================================================
来源：http://nwx.daria6918.cn

[I01] 判断是否匹配
来源：http://kyo.snrcjt.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yhq.jqgufenzy.top

PHP:  preg_match('/\d+/', $s);
来源：http://cgy.quarkkingdee.top

JS:   /\d+/.test(s)
来源：http://gbw.sufxvd.cn

TS:   /\d+/.test(s)
来源：http://jrr.ivvv.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cnz.nanxuanxn.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jqa.zhongyouzk.top

Ruby: s.match?(/\d+/)
来源：http://vcp.xuetiantiany.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dgq.xylfe.cn

[I02] 提取所有匹配
来源：http://zom.smart0.xyz

Py:   re.findall(r"\d+", s)
来源：http://uvy.cashguo.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xju.tanke756.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blw.hesvh.cn

TS:   s.match(/\d+/g)
来源：http://bpi.ydjk.org.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sga.ybcxt.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xzx.xuanzx.com

Ruby: s.scan(/\d+/)
来源：http://izv.xinyue.icu

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wrv.ywan-chungtsiang.top

[I03] 提取捕获分组
来源：http://pqy.pycfn.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rka.ywan-chungtsiang.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://oaw.jiagoushi.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vfn.haohaochexian.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dmq.ivvv.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pjl.guowangkeji.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qii.jyoumei.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://csq.hfpthk.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rwo.zhengqikj.top

[I04] 正则替换
来源：http://zfn.shanyushiyangkeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://jje.jlsjyb.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xce.ywan-chungtsiang.top

JS:   s.replace(/\d+/g, "#")
来源：http://dcy.ybcxt.top

TS:   s.replace(/\d+/g, "#")
来源：http://hqz.fehbvm.com

Java: s.replaceAll("\\d+", "#")
来源：http://jzt.pengpengdd.cyou

Go:   re.ReplaceAllString(s, "#")
来源：http://mqj.fengsongda.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ffd.jinqigufen.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jkj.birdmap.top

[I05] 按正则拆分
来源：http://aab.52xcode.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yls.vehdjk.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://oyh.gaohongyu789.top

JS:   s.split(/\s*,\s*/)
来源：http://rjt.dianchejie.cn

TS:   s.split(/\s*,\s*/)
来源：http://gwp.wangdashe.top

Java: s.split("\\s*,\\s*")
来源：http://jnq.ehwqpu.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ljp.tarul.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dkz.shuidangran.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qdf.tanke756.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mzp.jyoumei.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xlz.hesvh.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://icq.svipenyu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wwx.mhx1999.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uwo.dashuyun.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hpy.pengpengdd.cyou

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bws.jinqigufen.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bdd.pengpengdd.cyou

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rkn.ydzc1.top

[I07] 忽略大小写与多行模式
来源：http://twe.yj20258.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rgs.tian-w.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qcq.fehbvm.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xvj.wangshuangyany.cn

TS:   /error/gim
来源：http://tqf.shanyushiyangtech.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bip.nanxuanxn.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ltg.xinyue.icu

Ruby: s.scan(/error/i)
来源：http://acl.cucudq.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oso.dashuyun.cn

[I08] 贪婪与非贪婪匹配
来源：http://jci.wangshuangyany.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mth.yfazqb.com


<!-- 参考信息 -->