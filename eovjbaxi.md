代发 wailian999

================================================================================
来源：http://yrj.hnqzz.top

G. 面向对象
来源：http://tmk.hysaishi.cn

================================================================================
来源：http://pbc.ywan-chungtsiang.top

[G01] 定义类
来源：http://bfx.9152youxi.cn

Py:   class User: pass
来源：http://uxk.andypj.xyz

PHP:  class User {}
来源：http://mlp.fehbvm.com

JS:   class User {}
来源：http://vbe.havefunace.top

TS:   class User { name: string = ""; }
来源：http://zaa.snrcjt.cn

Java: class User {}
来源：http://ddr.dashuyun.cn

Go:   type User struct { Name string }
来源：http://whg.xuanzx.com

Ruby: class User; end
来源：http://ypr.52xcode.cn

C#:   class User {}
来源：http://byv.haohaochexian.top

[G02] 构造函数
来源：http://zue.fengsongda.top

Py:   def __init__(self, name): self.name = name
来源：http://bwi.jlsjyb.cn

PHP:  public function __construct(public string $name) {}
来源：http://bsj.sysykeji.top

JS:   constructor(name) { this.name = name; }
来源：http://orj.shanyushiyangtech.top

TS:   constructor(public name: string) {}
来源：http://oxe.yuanzhike.top

Java: User(String name) { this.name = name; }
来源：http://tnz.fengsongda.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ziw.jlsjyb.cn

Ruby: def initialize(name); @name = name; end
来源：http://rbn.tarul.cn

C#:   public User(string name) { Name = name; }
来源：http://jvp.jlsjyb.cn

[G03] 实例属性
来源：http://ovw.ydzc1.top

Py:   self.name = "x"
来源：http://qlj.wangshuangyany.cn

PHP:  public string $name = "x";
来源：http://oyi.jinyuanbaomall.cn

JS:   this.name = "x";
来源：http://quf.redwolf501.top

TS:   name: string = "x";
来源：http://jhv.jinghuilouyu.cn

Java: private String name;
来源：http://crf.aibaodan.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vpv.9152youxi.cn

Ruby: @name = "x"
来源：http://hmt.tarul.cn

C#:   public string Name { get; set; } = "x";
来源：http://rvm.ivvv.top

[G04] 定义方法
来源：http://zof.fzhhl.top

Py:   def greet(self): return self.name
来源：http://lhz.cashguo.top

PHP:  public function greet(): string { return $this->name; }
来源：http://wqd.hnxiangtu.top

JS:   greet() { return this.name; }
来源：http://nyu.sxryk.cn

TS:   greet(): string { return this.name; }
来源：http://cjw.epnwcf.com

Java: String greet() { return name; }
来源：http://kpg.cucudq.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mij.shzxlz.cn

Ruby: def greet; @name; end
来源：http://kaf.zdqjudy.top

C#:   public string Greet() => Name;
来源：http://dva.nwbrower.top

[G05] 继承
来源：http://xnz.yj20258888.top

Py:   class Admin(User): pass
来源：http://voi.cqqwz.cn

PHP:  class Admin extends User {}
来源：http://hsv.jinyuanbaomall.cn

JS:   class Admin extends User {}
来源：http://avt.zhongyouzk.top

TS:   class Admin extends User {}
来源：http://ags.mhx1999.top

Java: class Admin extends User {}
来源：http://zmv.yj202588.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gso.yj20258888.top

Ruby: class Admin < User; end
来源：http://qmr.svipenyu.cn

C#:   class Admin : User {}
来源：http://pld.xuanzx.com

[G06] 重写方法
来源：http://btc.fktsv.cn

Py:   def greet(self): return "admin"
来源：http://jhi.aizwys.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qhr.jianghu66.top

JS:   greet() { return "admin"; }
来源：http://boz.ppjwa.cn

TS:   greet(): string { return "admin"; }
来源：http://szf.tanke756.top

Java: @Override String greet() { return "admin"; }
来源：http://ekv.shanyushiyangtech.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mwc.pycfn.com

Ruby: def greet; "admin"; end
来源：http://cef.meibo888.top

C#:   public override string Greet() => "admin";
来源：http://fuq.nwbrower.top

[G07] 调用父类方法
来源：http://huc.epnwcf.com

Py:   super().greet()
来源：http://zmg.tianlin.xyz

PHP:  parent::greet();
来源：http://vpd.tanke756.top

JS:   super.greet();
来源：http://ryy.zdbjq.cn

TS:   super.greet();
来源：http://stx.sysykeji.top

Java: super.greet();
来源：http://uoa.hysaishi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bpn.yuxming.cn

Ruby: super
来源：http://ely.zdqjudy.top

C#:   base.Greet();
来源：http://lyw.shanyushiyangtech.top

[G08] 静态方法与属性
来源：http://iwk.wangshuangyany.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yvi.zhoulong.xyz

PHP:  public static function f() {}
来源：http://lhk.haohaochexian.top

JS:   static f() {}
来源：http://ans.zdqjudy.top

TS:   static f(): void {}
来源：http://rjv.shanyushiyangkeji.top

Java: static void f() {}
来源：http://fgw.zhoulong.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://rel.snrcjt.cn

Ruby: def self.f; end
来源：http://bxs.yfazqb.com

C#:   public static void F() {}
来源：http://egw.shuidangran.top

[G09] 接口 / 抽象类
来源：http://qlz.nwbrower.top

Py:   from abc import ABC, abstractmethod
来源：http://kxa.daxiang520.top

PHP:  interface Shape { public function area(): float; }
来源：http://lyf.cqqwz.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wfv.yfazqb.com

TS:   interface Shape { area(): number; }
来源：http://ibc.xuetiantiany.cn

Java: interface Shape { double area(); }
来源：http://ywy.aizwys.cn

Go:   type Shape interface { Area() float64 }
来源：http://hfd.snrcjt.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lqx.andypj.xyz

C#:   interface IShape { double Area(); }
来源：http://iku.shangyingyoupin.top

[G10] 访问控制
来源：http://qvp.jinyuanbaomall.cn

Py:   约定 _protected / __private（不强制）
来源：http://xsi.hesvh.cn

PHP:  public / protected / private
来源：http://iqf.kuanghao11.cn

JS:   #private 字段；其余公开
来源：http://avi.sxryk.cn

TS:   public / protected / private
来源：http://dbg.zhixingplan.top

Java: public / protected / private / 默认包级
来源：http://coa.chenjidiqi.icu

Go:   首字母大写可导出，小写仅包内可见
来源：http://taq.tarul.cn

Ruby: public / protected / private
来源：http://bxv.cdnleiting.top

C#:   public / protected / private / internal
来源：http://wgx.cucudq.cn

[G11] getter / setter
来源：http://lty.9152youxi.cn

Py:   @property 与 @x.setter
来源：http://yiv.yvedp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://elj.zhaomingkeji.xyz

JS:   get name() { return this._name; }
来源：http://loy.jianghu66.top

TS:   get name(): string { return this._name; }
来源：http://blw.wangdashe.top

Java: public String getName() { return name; }
来源：http://upo.ybcxt.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://bdw.9152youxi.cn

Ruby: attr_accessor :name
来源：http://qhf.tanke756.top

C#:   public string Name { get; set; }
来源：http://lhx.sufxvd.cn

[G12] 对象转字符串
来源：http://ssm.pengpengdd.cyou

Py:   def __str__(self): return self.name
来源：http://ozn.yueranfly.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://zsv.tanke756.top

JS:   toString() { return this.name; }
来源：http://jye.cheryme.top

TS:   toString(): string { return this.name; }
来源：http://iue.meibo888.top

Java: @Override public String toString() { return name; }
来源：http://ezv.bbcook.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kos.hnqzz.top

Ruby: def to_s; @name; end
来源：http://whg.aibaodan.cn

C#:   public override string ToString() => Name;
来源：http://yad.epnwcf.com

[G13] 判断对象类型
来源：http://hag.sxryk.cn

Py:   isinstance(u, User)
来源：http://wcj.jiagoushi.top

PHP:  $u instanceof User
来源：http://gxp.vehdjk.com

JS:   u instanceof User
来源：http://bzj.ydzc1.top

TS:   u instanceof User
来源：http://pzd.bjfxy.top

Java: u instanceof User
来源：http://eam.316326.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://fny.zdqjudy.top

Ruby: u.is_a?(User)
来源：http://yek.nanxuanxn.top

C#:   u is User
来源：http://urw.bjfxy.top

[G14] 数据类 / record
来源：http://mkg.yuanzhike.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://oyc.havefunace.top

PHP:  // 用 readonly 属性模拟
来源：http://zja.zhiwuduotai.top

JS:   // 无内置：普通类或对象字面量
来源：http://wwq.gotoacloud.top

TS:   type User = { name: string; age: number };
来源：http://mza.jinqigfzy.top

Java: record User(String name, int age) {}
来源：http://arz.cucudq.cn

Go:   type User struct { Name string; Age int }
来源：http://sfm.sweek.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fro.ppjwa.cn

C#:   record User(string Name, int Age);
来源：http://haq.xuetiantiany.cn

[G15] 枚举
来源：http://tfh.ywan-chungtsiang.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nve.chenlongwang.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://box.guannengcc.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://oah.jyoumei.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://otw.yongpay.top

Java: enum Color { RED, GREEN }
来源：http://jnr.xuanzx.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bji.sysykeji.top

Ruby: Color = %i[red green].freeze
来源：http://qqu.yanxiufei.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://aib.wangdashe.top

[G16] 对象转数组 / 字典
来源：http://ksp.kuanghao11.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ztm.yangfankeji.com

PHP:  get_object_vars($obj);
来源：http://ydt.xziqi.cn

JS:   Object.entries(obj)
来源：http://hvm.daxiang520.top

TS:   Object.entries(obj)
来源：http://pyb.9152youxi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hee.zhiwuduotai.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ndg.jinyuanbaomall.cn

Ruby: obj.instance_variables
来源：http://mfr.epnwcf.com

C#:   // 用反射或 System.Text.Json
来源：http://gvd.bbcook.cn

================================================================================
来源：http://huw.ywan-chungtsiang.top

H. 异常与错误处理
来源：http://wdj.sxryk.cn

================================================================================
来源：http://vqp.haohaochexian.top

[H01] try / catch 基础
来源：http://ajx.hfpthk.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yqb.fengsongda.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jqc.c1oappe.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wvu.daria6918.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tfy.hnqzz.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://npv.gaohongyu789.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qkj.snrcjt.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ynz.haohaochexian.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kne.daria6918.cn

[H02] finally / ensure 收尾
来源：http://dgp.ctjpmb.com

Py:   try: f()⏎finally: cleanup()
来源：http://xcv.shanyushiyangtech.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ijk.nanxinkj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://vkc.mhx1999.top

TS:   try { f(); } finally { cleanup(); }
来源：http://aju.andypj.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://wll.redwolf501.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://gpf.cheryme.top

Ruby: begin; f; ensure; cleanup; end
来源：http://cjm.zhaomingkeji.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://dxx.yongpay.top

[H03] 主动抛出异常
来源：http://rya.sysykeji.top

Py:   raise ValueError("错误信息")
来源：http://tgs.wangshuangyany.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ypx.hnxiangtu.top

JS:   throw new Error("错误信息");
来源：http://cvy.vqdsnc.cn

TS:   throw new Error("错误信息");
来源：http://cth.sjlbkw.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xfd.ivvv.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jpu.sufxvd.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ckq.hfpthk.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gpt.chenzaomai.com

[H04] 自定义异常类型
来源：http://ryi.quarkkingdee.top

Py:   class MyError(Exception): pass
来源：http://rod.ybcxt.top

PHP:  class MyError extends RuntimeException {}
来源：http://xfe.tian-w.cn

JS:   class MyError extends Error {}
来源：http://mci.shuidangran.top

TS:   class MyError extends Error {}
来源：http://bsb.snrcjt.cn

Java: class MyException extends RuntimeException {}
来源：http://mps.hfpthk.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dhs.yj20258.top

Ruby: class MyError < StandardError; end
来源：http://tmh.jianghu66.top

C#:   class MyException : Exception {}
来源：http://ntg.shangyingyoupin.top

[H05] 捕获特定类型
来源：http://nah.c1oappe.top

Py:   except ValueError as e:
来源：http://kex.feifeiyinyue.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://enq.yongpay.top

JS:   if (e instanceof TypeError) {}
来源：http://dyf.quarkkingdee.top

TS:   if (e instanceof TypeError) {}
来源：http://mpa.ivvv.top

Java: catch (IOException | SQLException e) {}
来源：http://jvy.pycfn.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://abj.c1oappe.top

Ruby: rescue ArgumentError => e
来源：http://fgm.tian-w.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xjk.0kj1m.cn

[H06] 可选值 / 空值安全访问
来源：http://ekw.daria6918.cn

Py:   value = d.get("k") or default
来源：http://cvv.jinqigufen.top

PHP:  $v = $d["k"] ?? null;
来源：http://nah.yongpay.top

JS:   obj?.a?.b;  d ?? default
来源：http://dja.gzhubu.top

TS:   obj?.a?.b;  d ?? default
来源：http://gex.yonumen.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dbq.fktsv.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ajb.pycfn.com

Ruby: d&.dig(:a, :b)
来源：http://irn.ivvv.top

C#:   obj?.A?.B ?? default
来源：http://slu.shuidangran.top

[H07] 断言
来源：http://tjv.jinyuanbaomall.cn

Py:   assert x > 0, "必须为正"
来源：http://yam.ydzc1.top

PHP:  assert($x > 0);
来源：http://qdc.jinyuanbaomall.cn

JS:   console.assert(x > 0);
来源：http://ksl.hfpthk.cn

TS:   console.assert(x > 0);
来源：http://cya.kuanghao11.cn

Java: assert x > 0 : "必须为正";
来源：http://vyi.shangyingyoupin.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zvr.zhongyouzk.top

Ruby: raise "必须为正" unless x > 0
来源：http://nhl.ywan-chungtsiang.top

C#:   Debug.Assert(x > 0);
来源：http://hzt.zhaomingkeji.xyz

[H08] 获取错误信息与堆栈
来源：http://nsm.gogol.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://xun.shzxlz.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sbe.0kj1m.cn

JS:   e.message;  e.stack
来源：http://wbb.yuxming.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jis.haohaochexian.top

Java: e.getMessage();  e.printStackTrace()
来源：http://mxf.zhijiandao.cn

Go:   err.Error()
来源：http://nsh.feifeiyinyue.top

Ruby: e.message;  e.backtrace
来源：http://kga.chenzaomai.com

C#:   e.Message;  e.StackTrace
来源：http://szn.sufxvd.cn

[H09] 带错误码的异常
来源：http://yew.vqdsnc.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://djh.tian-w.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gtm.yanxiufei.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vfr.yuxming.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mue.zhongyouzk.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fev.zycfv.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qha.cdnleiting.top

Ruby: raise MyError.new("fail", 500)
来源：http://fns.jinyuanbaomall.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cen.epnwcf.com

[H10] 资源自动释放
来源：http://brv.jinyuanbaomall.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://agn.xingfuxueyuan.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://slr.cqqwz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yqo.sxryk.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kxr.sjlbkw.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://eie.yj20258888.top

Go:   defer f.Close()
来源：http://tye.xinyue.icu

Ruby: File.open("a.txt") { |f| f.read }
来源：http://saq.yuxming.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hso.jqgufenzy.top

================================================================================
来源：http://jtw.dashuyun.cn

I. 正则表达式
来源：http://ono.pengpengdd.cyou

================================================================================
来源：http://xpf.yuxming.cn

[I01] 判断是否匹配
来源：http://foz.pycfn.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vtr.sweek.top

PHP:  preg_match('/\d+/', $s);
来源：http://nte.52xcode.cn

JS:   /\d+/.test(s)
来源：http://mmf.haohaochexian.top

TS:   /\d+/.test(s)
来源：http://qgu.ywan-chungtsiang.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zjr.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fvh.fzhhl.top

Ruby: s.match?(/\d+/)
来源：http://crs.zhoulong.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cto.ivvv.top

[I02] 提取所有匹配
来源：http://blk.zhijiandao.cn

Py:   re.findall(r"\d+", s)
来源：http://phs.gaohongyu789.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sto.ywan-chungtsiang.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ywc.gogol.net.cn

TS:   s.match(/\d+/g)
来源：http://xcu.andypj.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://azo.zdbjq.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://utf.hongshengwenyu.top

Ruby: s.scan(/\d+/)
来源：http://nhb.hywenlv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vpz.hywenlv.cn

[I03] 提取捕获分组
来源：http://fbp.fktsv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ika.mhx1999.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qtf.fehbvm.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nib.pycfn.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yrw.gzhubu.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://glp.hesvh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ccq.ehwqpu.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qqq.bbcook.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qrt.wangshuangyany.cn

[I04] 正则替换
来源：http://xkj.hesvh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://aqx.ivvv.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://axh.dianchejie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ytn.hysaishi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vge.jinqigfzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://nbp.xylfe.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qth.9152youxi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mjh.chenlongwang.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hlj.jiagoushi.top

[I05] 按正则拆分
来源：http://orx.chenlongwang.top

Py:   re.split(r"\s*,\s*", s)
来源：http://cxj.cdnleiting.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hns.sufxvd.cn

JS:   s.split(/\s*,\s*/)
来源：http://soi.cashguo.top

TS:   s.split(/\s*,\s*/)
来源：http://ysk.sxryk.cn

Java: s.split("\\s*,\\s*")
来源：http://oqc.9152youxi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pxm.jqgfzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://izf.jinyuanbaomall.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sdi.yongpay.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dlx.xuanzx.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ivi.xingfuxueyuan.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bwb.xuanzx.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://psn.vehdjk.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nxo.daria6918.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://npl.zhongyouzk.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gwi.pengpengdd.cyou

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://npt.xuetiantiany.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lpq.fzhhl.top

[I07] 忽略大小写与多行模式
来源：http://kdc.daxiang520.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bui.vehdjk.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://imw.bbcook.cn


<!-- 参考信息 -->