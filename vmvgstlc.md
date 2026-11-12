代发 wailian999

================================================================================
来源：http://jcc.xinyue.icu

G. 面向对象
来源：http://tzf.cashguo.top

================================================================================
来源：http://nmq.yj20258888.top

[G01] 定义类
来源：http://aoc.yueranfly.top

Py:   class User: pass
来源：http://owy.redwolf501.top

PHP:  class User {}
来源：http://sya.cheryme.top

JS:   class User {}
来源：http://hhl.ydjk.org.cn

TS:   class User { name: string = ""; }
来源：http://sda.tarul.cn

Java: class User {}
来源：http://vaa.yfazqb.com

Go:   type User struct { Name string }
来源：http://dku.jinqigufen.top

Ruby: class User; end
来源：http://nsz.yangfankeji.com

C#:   class User {}
来源：http://qis.zhaomingkeji.xyz

[G02] 构造函数
来源：http://rbs.haohaochexian.top

Py:   def __init__(self, name): self.name = name
来源：http://adt.kuanghao11.cn

PHP:  public function __construct(public string $name) {}
来源：http://mox.nanxuanxn.top

JS:   constructor(name) { this.name = name; }
来源：http://eah.sysykeji.top

TS:   constructor(public name: string) {}
来源：http://isd.9152youxi.cn

Java: User(String name) { this.name = name; }
来源：http://dwu.shangyingyoupin.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://eah.shangyingyoupin.top

Ruby: def initialize(name); @name = name; end
来源：http://ukh.jinyuanbaomall.cn

C#:   public User(string name) { Name = name; }
来源：http://ngk.bjfxy.top

[G03] 实例属性
来源：http://uoe.fzhhl.top

Py:   self.name = "x"
来源：http://czv.chenzaomai.com

PHP:  public string $name = "x";
来源：http://rdw.pycfn.com

JS:   this.name = "x";
来源：http://jvn.hnxiangtu.top

TS:   name: string = "x";
来源：http://gwh.shanyushiyangkeji.top

Java: private String name;
来源：http://gqi.52xcode.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blp.yanxiufei.cn

Ruby: @name = "x"
来源：http://vlz.dianchejie.cn

C#:   public string Name { get; set; } = "x";
来源：http://xbs.mhx1999.top

[G04] 定义方法
来源：http://fuz.vehdjk.com

Py:   def greet(self): return self.name
来源：http://iwq.fanxiaobao.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://xtf.jianghu66.top

JS:   greet() { return this.name; }
来源：http://uja.epnwcf.com

TS:   greet(): string { return this.name; }
来源：http://zis.birdmap.top

Java: String greet() { return name; }
来源：http://mdy.yvedp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://tjb.9152youxi.cn

Ruby: def greet; @name; end
来源：http://stn.quarkkingdee.top

C#:   public string Greet() => Name;
来源：http://xfi.hongshengwenyu.top

[G05] 继承
来源：http://lqu.zycfv.cn

Py:   class Admin(User): pass
来源：http://uos.hnxiangtu.top

PHP:  class Admin extends User {}
来源：http://ugu.wangshuangyany.cn

JS:   class Admin extends User {}
来源：http://qji.chenjidiqi.icu

TS:   class Admin extends User {}
来源：http://qmr.nanxinkj.top

Java: class Admin extends User {}
来源：http://wsc.chenlongwang.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wrs.yangfankeji.com

Ruby: class Admin < User; end
来源：http://scv.wangdashe.top

C#:   class Admin : User {}
来源：http://vlb.yj202588.top

[G06] 重写方法
来源：http://geq.xuetiantiany.cn

Py:   def greet(self): return "admin"
来源：http://qwd.yvedp.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ctf.shuidangran.top

JS:   greet() { return "admin"; }
来源：http://ejz.svipenyu.cn

TS:   greet(): string { return "admin"; }
来源：http://enf.hcnkem.com

Java: @Override String greet() { return "admin"; }
来源：http://wsi.ehwqpu.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cii.epnwcf.com

Ruby: def greet; "admin"; end
来源：http://jef.gogol.net.cn

C#:   public override string Greet() => "admin";
来源：http://ppb.mhx1999.top

[G07] 调用父类方法
来源：http://rqe.tarul.cn

Py:   super().greet()
来源：http://pjb.quarkkingdee.top

PHP:  parent::greet();
来源：http://rzt.gzhubu.top

JS:   super.greet();
来源：http://jee.jinyuanbaomall.cn

TS:   super.greet();
来源：http://crb.wangshuangyany.cn

Java: super.greet();
来源：http://vso.zhiwuduotai.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cjb.dianchejie.cn

Ruby: super
来源：http://aoe.jinqigufen.top

C#:   base.Greet();
来源：http://hfy.hywenlv.cn

[G08] 静态方法与属性
来源：http://ufs.guowangkeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vko.guannengcc.top

PHP:  public static function f() {}
来源：http://qkz.xuetiantiany.cn

JS:   static f() {}
来源：http://eqs.cqqwz.cn

TS:   static f(): void {}
来源：http://gwy.quarkkingdee.top

Java: static void f() {}
来源：http://mlp.quarkkingdee.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://gtz.tanke756.top

Ruby: def self.f; end
来源：http://hqx.jinqigufen.top

C#:   public static void F() {}
来源：http://xvx.jqgfzy.top

[G09] 接口 / 抽象类
来源：http://qrn.jlsjyb.cn

Py:   from abc import ABC, abstractmethod
来源：http://szm.zhixingplan.top

PHP:  interface Shape { public function area(): float; }
来源：http://moo.gotoacloud.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ahz.hesvh.cn

TS:   interface Shape { area(): number; }
来源：http://rpo.hongshengwenyu.top

Java: interface Shape { double area(); }
来源：http://svv.dianchejie.cn

Go:   type Shape interface { Area() float64 }
来源：http://knf.zhaomingkeji.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fco.zhengqikj.top

C#:   interface IShape { double Area(); }
来源：http://myn.sjlbkw.cn

[G10] 访问控制
来源：http://cos.zhengqikj.top

Py:   约定 _protected / __private（不强制）
来源：http://gem.zdbjq.cn

PHP:  public / protected / private
来源：http://lnb.birdmap.top

JS:   #private 字段；其余公开
来源：http://cec.snrcjt.cn

TS:   public / protected / private
来源：http://guw.snrcjt.cn

Java: public / protected / private / 默认包级
来源：http://owo.bjfxy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qgm.jianghu66.top

Ruby: public / protected / private
来源：http://zou.jlsjyb.cn

C#:   public / protected / private / internal
来源：http://hhu.shzxlz.cn

[G11] getter / setter
来源：http://mxz.svipenyu.cn

Py:   @property 与 @x.setter
来源：http://dbr.yongpay.top

PHP:  public function getName(): string { return $this->name; }
来源：http://stm.chenlongwang.top

JS:   get name() { return this._name; }
来源：http://ggs.yuxming.cn

TS:   get name(): string { return this._name; }
来源：http://ysx.jinghuilouyu.cn

Java: public String getName() { return name; }
来源：http://yuy.gogol.net.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://luv.hysaishi.cn

Ruby: attr_accessor :name
来源：http://olw.jinqigfzy.top

C#:   public string Name { get; set; }
来源：http://ngx.9152youxi.cn

[G12] 对象转字符串
来源：http://xup.yj20258888.top

Py:   def __str__(self): return self.name
来源：http://fqy.nwbrower.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://usc.shzxlz.cn

JS:   toString() { return this.name; }
来源：http://eii.haohaochexian.top

TS:   toString(): string { return this.name; }
来源：http://mvx.zhiwuduotai.top

Java: @Override public String toString() { return name; }
来源：http://lzk.hnxiangtu.top

Go:   func (u User) String() string { return u.Name }
来源：http://xob.zhengqikj.top

Ruby: def to_s; @name; end
来源：http://gpz.shanyushiyangkeji.top

C#:   public override string ToString() => Name;
来源：http://hjr.yj202588.top

[G13] 判断对象类型
来源：http://hhv.zhixingplan.top

Py:   isinstance(u, User)
来源：http://oih.fanxiaobao.xyz

PHP:  $u instanceof User
来源：http://qya.fanxiaobao.xyz

JS:   u instanceof User
来源：http://vgs.zdbjq.cn

TS:   u instanceof User
来源：http://fij.hongshengwenyu.top

Java: u instanceof User
来源：http://gir.jinyuanbaomall.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pkm.hnqzz.top

Ruby: u.is_a?(User)
来源：http://yjp.316326.xyz

C#:   u is User
来源：http://hwc.cqqwz.cn

[G14] 数据类 / record
来源：http://pta.fzhhl.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://des.zhijiandao.cn

PHP:  // 用 readonly 属性模拟
来源：http://mti.hnxiangtu.top

JS:   // 无内置：普通类或对象字面量
来源：http://pai.pengpengdd.cyou

TS:   type User = { name: string; age: number };
来源：http://swk.yuanzhike.top

Java: record User(String name, int age) {}
来源：http://pvp.xylfe.cn

Go:   type User struct { Name string; Age int }
来源：http://wef.jiagoushi.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rwn.quarkkingdee.top

C#:   record User(string Name, int Age);
来源：http://sna.bbcook.cn

[G15] 枚举
来源：http://ihl.gzhubu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jda.xuanzx.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://cxm.jqgfzy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kgm.nanxuanxn.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://smr.redwolf501.top

Java: enum Color { RED, GREEN }
来源：http://vwf.ctjpmb.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kqb.shanyushiyangkeji.top

Ruby: Color = %i[red green].freeze
来源：http://pci.zhaomingkeji.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sqg.xingfuxueyuan.xyz

[G16] 对象转数组 / 字典
来源：http://npu.zhijiandao.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gtq.tianlin.xyz

PHP:  get_object_vars($obj);
来源：http://lyp.jlsjyb.cn

JS:   Object.entries(obj)
来源：http://pah.quarkkingdee.top

TS:   Object.entries(obj)
来源：http://obl.dianchejie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zey.gogol.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://aim.yj20258888.top

Ruby: obj.instance_variables
来源：http://zni.snrcjt.cn

C#:   // 用反射或 System.Text.Json
来源：http://ykh.gaohongyu789.top

================================================================================
来源：http://rap.ybcxt.top

H. 异常与错误处理
来源：http://ahh.hnxiangtu.top

================================================================================
来源：http://gdb.bjfxy.top

[H01] try / catch 基础
来源：http://vmy.zhoulong.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fok.pengpengdd.cyou

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rlt.hnqzz.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hko.tanke756.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pnk.chenjidiqi.icu

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fqc.yueranfly.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ngo.gaohongyu789.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qpu.sweek.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dzd.xingfuxueyuan.xyz

[H02] finally / ensure 收尾
来源：http://kjy.daria6918.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jei.iojbl.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yov.vqdsnc.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://isr.wangdashe.top

TS:   try { f(); } finally { cleanup(); }
来源：http://xiz.sweek.top

Java: try { f(); } finally { cleanup(); }
来源：http://dua.yuxming.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zkg.zhoulong.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://ttl.zycfv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cnj.ivvv.top

[H03] 主动抛出异常
来源：http://lrk.zhongyouzk.top

Py:   raise ValueError("错误信息")
来源：http://goq.shuidangran.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jln.316326.xyz

JS:   throw new Error("错误信息");
来源：http://kmr.aizwys.cn

TS:   throw new Error("错误信息");
来源：http://sgv.mhx1999.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://muy.yj20258888.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hso.zhiwuduotai.top

Ruby: raise ArgumentError, "错误信息"
来源：http://etj.316326.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://chz.mhx1999.top

[H04] 自定义异常类型
来源：http://lfr.yj20258.top

Py:   class MyError(Exception): pass
来源：http://mpy.hywenlv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rxf.9152youxi.cn

JS:   class MyError extends Error {}
来源：http://jbs.zhiwuduotai.top

TS:   class MyError extends Error {}
来源：http://ywi.ppjwa.cn

Java: class MyException extends RuntimeException {}
来源：http://fsm.dianchejie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://psa.gogol.net.cn

Ruby: class MyError < StandardError; end
来源：http://qdy.aizwys.cn

C#:   class MyException : Exception {}
来源：http://rwl.sxryk.cn

[H05] 捕获特定类型
来源：http://zjv.52xcode.cn

Py:   except ValueError as e:
来源：http://mjc.fanxiaobao.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xab.yj20258888.top

JS:   if (e instanceof TypeError) {}
来源：http://tae.cdnleiting.top

TS:   if (e instanceof TypeError) {}
来源：http://bqg.52xcode.cn

Java: catch (IOException | SQLException e) {}
来源：http://zsw.xuanzx.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ubg.hammf.cn

Ruby: rescue ArgumentError => e
来源：http://zlz.birdmap.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rkl.zhaomingkeji.xyz

[H06] 可选值 / 空值安全访问
来源：http://jcg.jyoumei.cn

Py:   value = d.get("k") or default
来源：http://ayf.aizwys.cn

PHP:  $v = $d["k"] ?? null;
来源：http://azw.kuanghao11.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zna.yj202588.top

TS:   obj?.a?.b;  d ?? default
来源：http://wcf.guannengcc.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bxo.ctjpmb.com

Go:   if v, ok := m["k"]; ok { }
来源：http://lam.kuanghao11.cn

Ruby: d&.dig(:a, :b)
来源：http://mth.guannengcc.top

C#:   obj?.A?.B ?? default
来源：http://fol.sxryk.cn

[H07] 断言
来源：http://obd.redwolf501.top

Py:   assert x > 0, "必须为正"
来源：http://oxq.bjfxy.top

PHP:  assert($x > 0);
来源：http://ksf.mhx1999.top

JS:   console.assert(x > 0);
来源：http://afp.pycfn.com

TS:   console.assert(x > 0);
来源：http://fcq.chenjidiqi.icu

Java: assert x > 0 : "必须为正";
来源：http://qhv.sjlbkw.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ibp.xinyue.icu

Ruby: raise "必须为正" unless x > 0
来源：http://nip.ppjwa.cn

C#:   Debug.Assert(x > 0);
来源：http://fej.shuidangran.top

[H08] 获取错误信息与堆栈
来源：http://axv.cucudq.cn

Py:   str(e);  traceback.format_exc()
来源：http://atx.316326.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mpg.wangdashe.top

JS:   e.message;  e.stack
来源：http://hgm.ybcxt.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ynk.zdbjq.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ivv.nwbrower.top

Go:   err.Error()
来源：http://yee.jqgfzy.top

Ruby: e.message;  e.backtrace
来源：http://swo.mhx1999.top

C#:   e.Message;  e.StackTrace
来源：http://bai.ydjk.org.cn

[H09] 带错误码的异常
来源：http://gvq.wangshuangyany.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kcj.xuetiantiany.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hty.shuidangran.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nry.ehwqpu.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://osl.pengpengdd.cyou

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://btz.jinqigfzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xcw.nanxinkj.top

Ruby: raise MyError.new("fail", 500)
来源：http://uat.quarkkingdee.top

C#:   // 自定义异常类中加 Code 属性
来源：http://wrd.tianlin.xyz

[H10] 资源自动释放
来源：http://rrf.cdnleiting.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://qko.nanxinkj.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ait.jlsjyb.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cam.shzxlz.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rxv.uphjek.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://exn.gogol.net.cn

Go:   defer f.Close()
来源：http://fqu.dianchejie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hph.nwbrower.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dpo.jinghuilouyu.cn

================================================================================
来源：http://alb.smart0.xyz

I. 正则表达式
来源：http://cvw.gogol.net.cn

================================================================================
来源：http://tol.zhoulong.xyz

[I01] 判断是否匹配
来源：http://yll.ivvv.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tfa.wangshuangyany.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hcu.epnwcf.com

JS:   /\d+/.test(s)
来源：http://bba.tian-w.cn

TS:   /\d+/.test(s)
来源：http://heg.hesvh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rvz.fehbvm.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vle.chenzaomai.com

Ruby: s.match?(/\d+/)
来源：http://aww.hcnkem.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ehv.ywan-chungtsiang.top

[I02] 提取所有匹配
来源：http://wkx.nwbrower.top

Py:   re.findall(r"\d+", s)
来源：http://mwv.zhaomingkeji.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hno.guowangkeji.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://eix.shuidangran.top

TS:   s.match(/\d+/g)
来源：http://kgi.hnqzz.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uqf.jiagoushi.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ccf.chenjidiqi.icu

Ruby: s.scan(/\d+/)
来源：http://adt.ywan-chungtsiang.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wfu.tanke756.top

[I03] 提取捕获分组
来源：http://bwj.jinyuanbaomall.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jtb.zhixingplan.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yzj.bbcook.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://flx.jlsjyb.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zwq.zhoulong.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jac.vqdsnc.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ndn.chenzaomai.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ebl.sjlbkw.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yzu.pycfn.com

[I04] 正则替换
来源：http://xdi.havefunace.top

Py:   re.sub(r"\d+", "#", s)
来源：http://brx.sufxvd.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pef.hnxiangtu.top

JS:   s.replace(/\d+/g, "#")
来源：http://yoe.xingfuxueyuan.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://qgx.cqqwz.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jxq.yuxming.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jqw.yueranfly.top

Ruby: s.gsub(/\d+/, "#")
来源：http://azm.gaohongyu789.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hbe.xziqi.cn

[I05] 按正则拆分
来源：http://lxu.yuxming.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://war.yonumen.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tgy.9152youxi.cn

JS:   s.split(/\s*,\s*/)
来源：http://bzk.hysaishi.cn

TS:   s.split(/\s*,\s*/)
来源：http://fyg.yonumen.top

Java: s.split("\\s*,\\s*")
来源：http://dyl.snrcjt.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vqe.zdqjudy.top

Ruby: s.split(/\s*,\s*/)
来源：http://img.zhoulong.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zky.zdqjudy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cio.yuxming.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://oij.sysykeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qwa.ppjwa.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tyr.ydjk.org.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tvk.gzhubu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://who.wangshuangyany.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xjg.jqgufenzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://daj.smart0.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://run.epnwcf.com

[I07] 忽略大小写与多行模式
来源：http://xje.sysykeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mzk.sxryk.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://puh.yuanzhike.top


<!-- 参考信息 -->