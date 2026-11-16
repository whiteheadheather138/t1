代发 wailian999

================================================================================
来源：http://iki.guannengcc.top

G. 面向对象
来源：http://dnp.haohaochexian.top

================================================================================
来源：http://ayp.sysykeji.top

[G01] 定义类
来源：http://rbw.tian-w.cn

Py:   class User: pass
来源：http://lzf.zycfv.cn

PHP:  class User {}
来源：http://cie.yuanzhike.top

JS:   class User {}
来源：http://fiq.ehwqpu.com

TS:   class User { name: string = ""; }
来源：http://bup.tanke756.top

Java: class User {}
来源：http://obw.andypj.xyz

Go:   type User struct { Name string }
来源：http://vob.yangfankeji.com

Ruby: class User; end
来源：http://ccg.zhengqikj.top

C#:   class User {}
来源：http://qtt.sxryk.cn

[G02] 构造函数
来源：http://lif.tianlin.xyz

Py:   def __init__(self, name): self.name = name
来源：http://fgx.yanxiufei.cn

PHP:  public function __construct(public string $name) {}
来源：http://qfw.havefunace.top

JS:   constructor(name) { this.name = name; }
来源：http://ctc.jqgufenzy.top

TS:   constructor(public name: string) {}
来源：http://yvb.meibo888.top

Java: User(String name) { this.name = name; }
来源：http://qpl.xziqi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ztd.yvedp.cn

Ruby: def initialize(name); @name = name; end
来源：http://hqe.hammf.cn

C#:   public User(string name) { Name = name; }
来源：http://smx.ybcxt.top

[G03] 实例属性
来源：http://ulv.xziqi.cn

Py:   self.name = "x"
来源：http://sta.zhixingplan.top

PHP:  public string $name = "x";
来源：http://dyk.yuxming.cn

JS:   this.name = "x";
来源：http://zji.chenlongwang.top

TS:   name: string = "x";
来源：http://lyo.0kj1m.cn

Java: private String name;
来源：http://fgm.shzxlz.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gve.svipenyu.cn

Ruby: @name = "x"
来源：http://ehy.shuidangran.top

C#:   public string Name { get; set; } = "x";
来源：http://nzp.zycfv.cn

[G04] 定义方法
来源：http://amp.zhengqikj.top

Py:   def greet(self): return self.name
来源：http://ezn.ydjk.org.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xql.shanyushiyangkeji.top

JS:   greet() { return this.name; }
来源：http://rxk.wangdashe.top

TS:   greet(): string { return this.name; }
来源：http://fqg.jianghu66.top

Java: String greet() { return name; }
来源：http://nlw.hysaishi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fuv.yongpay.top

Ruby: def greet; @name; end
来源：http://puy.yueranfly.top

C#:   public string Greet() => Name;
来源：http://lok.mhx1999.top

[G05] 继承
来源：http://xjc.hfpthk.cn

Py:   class Admin(User): pass
来源：http://orn.aibaodan.cn

PHP:  class Admin extends User {}
来源：http://zwz.jiagoushi.top

JS:   class Admin extends User {}
来源：http://ffr.xuetiantiany.cn

TS:   class Admin extends User {}
来源：http://cqv.zhijiandao.cn

Java: class Admin extends User {}
来源：http://uxa.tanke756.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dko.hfpthk.cn

Ruby: class Admin < User; end
来源：http://qbk.ywan-chungtsiang.top

C#:   class Admin : User {}
来源：http://lvr.hysaishi.cn

[G06] 重写方法
来源：http://rzt.zhaomingkeji.xyz

Py:   def greet(self): return "admin"
来源：http://qqg.yj20258888.top

PHP:  public function greet(): string { return "admin"; }
来源：http://wwg.yonumen.top

JS:   greet() { return "admin"; }
来源：http://okc.jinyuanbaomall.cn

TS:   greet(): string { return "admin"; }
来源：http://rnp.hywenlv.cn

Java: @Override String greet() { return "admin"; }
来源：http://acp.hongshengwenyu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ysd.jinqigfzy.top

Ruby: def greet; "admin"; end
来源：http://etq.sweek.top

C#:   public override string Greet() => "admin";
来源：http://qmh.yj20258888.top

[G07] 调用父类方法
来源：http://wsd.pengpengdd.cyou

Py:   super().greet()
来源：http://bni.hongshengwenyu.top

PHP:  parent::greet();
来源：http://hvc.yuxming.cn

JS:   super.greet();
来源：http://plc.ydjk.org.cn

TS:   super.greet();
来源：http://pcu.mhx1999.top

Java: super.greet();
来源：http://rna.guowangkeji.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://css.vqdsnc.cn

Ruby: super
来源：http://kbf.hongshengwenyu.top

C#:   base.Greet();
来源：http://niy.yuanzhike.top

[G08] 静态方法与属性
来源：http://jxd.yfazqb.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uap.0kj1m.cn

PHP:  public static function f() {}
来源：http://ofw.shanyushiyangkeji.top

JS:   static f() {}
来源：http://smx.cucudq.cn

TS:   static f(): void {}
来源：http://ckm.ehwqpu.com

Java: static void f() {}
来源：http://ivc.feifeiyinyue.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ulf.bjfxy.top

Ruby: def self.f; end
来源：http://bds.gotoacloud.top

C#:   public static void F() {}
来源：http://vnu.sjlbkw.cn

[G09] 接口 / 抽象类
来源：http://dlv.tianlin.xyz

Py:   from abc import ABC, abstractmethod
来源：http://dch.xylfe.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wmo.yanxiufei.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mdf.yueranfly.top

TS:   interface Shape { area(): number; }
来源：http://fvz.sysykeji.top

Java: interface Shape { double area(); }
来源：http://ncc.snrcjt.cn

Go:   type Shape interface { Area() float64 }
来源：http://njb.xuanzx.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bhh.c1oappe.top

C#:   interface IShape { double Area(); }
来源：http://opv.meibo888.top

[G10] 访问控制
来源：http://kyd.jinqigufen.top

Py:   约定 _protected / __private（不强制）
来源：http://fii.cqqwz.cn

PHP:  public / protected / private
来源：http://rwd.guannengcc.top

JS:   #private 字段；其余公开
来源：http://wxl.c1oappe.top

TS:   public / protected / private
来源：http://vzr.hcnkem.com

Java: public / protected / private / 默认包级
来源：http://pgd.chenjidiqi.icu

Go:   首字母大写可导出，小写仅包内可见
来源：http://rcm.daria6918.cn

Ruby: public / protected / private
来源：http://ofa.guannengcc.top

C#:   public / protected / private / internal
来源：http://xel.wangshuangyany.cn

[G11] getter / setter
来源：http://miy.hongshengwenyu.top

Py:   @property 与 @x.setter
来源：http://ino.zhongyouzk.top

PHP:  public function getName(): string { return $this->name; }
来源：http://hzz.ydzc1.top

JS:   get name() { return this._name; }
来源：http://tlq.meibo888.top

TS:   get name(): string { return this._name; }
来源：http://sdw.zhiwuduotai.top

Java: public String getName() { return name; }
来源：http://dwg.hywenlv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xtf.yj20258.top

Ruby: attr_accessor :name
来源：http://drh.wangdashe.top

C#:   public string Name { get; set; }
来源：http://gvv.yanxiufei.cn

[G12] 对象转字符串
来源：http://rlg.hammf.cn

Py:   def __str__(self): return self.name
来源：http://zcv.zhaomingkeji.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://gqr.yonumen.top

JS:   toString() { return this.name; }
来源：http://csy.fehbvm.com

TS:   toString(): string { return this.name; }
来源：http://gwx.daxiang520.top

Java: @Override public String toString() { return name; }
来源：http://mgq.feifeiyinyue.top

Go:   func (u User) String() string { return u.Name }
来源：http://zhn.fengsongda.top

Ruby: def to_s; @name; end
来源：http://nzn.hongshengwenyu.top

C#:   public override string ToString() => Name;
来源：http://sbj.ywan-chungtsiang.top

[G13] 判断对象类型
来源：http://lfl.cqqwz.cn

Py:   isinstance(u, User)
来源：http://eij.fzhhl.top

PHP:  $u instanceof User
来源：http://jki.jiagoushi.top

JS:   u instanceof User
来源：http://ean.quarkkingdee.top

TS:   u instanceof User
来源：http://hjf.xziqi.cn

Java: u instanceof User
来源：http://lhk.ybcxt.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://zex.hcnkem.com

Ruby: u.is_a?(User)
来源：http://hgl.quarkkingdee.top

C#:   u is User
来源：http://gbp.bbcook.cn

[G14] 数据类 / record
来源：http://hbm.chenjidiqi.icu

Py:   @dataclass⏎class User: name: str; age: int
来源：http://aln.52xcode.cn

PHP:  // 用 readonly 属性模拟
来源：http://mvg.mhx1999.top

JS:   // 无内置：普通类或对象字面量
来源：http://ahw.zhijiandao.cn

TS:   type User = { name: string; age: number };
来源：http://kul.52xcode.cn

Java: record User(String name, int age) {}
来源：http://lle.gaohongyu789.top

Go:   type User struct { Name string; Age int }
来源：http://gkq.aizwys.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wkr.yuxming.cn

C#:   record User(string Name, int Age);
来源：http://bpl.jqgufenzy.top

[G15] 枚举
来源：http://rtr.xingfuxueyuan.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://inl.cucudq.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ktz.daria6918.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://znc.fengsongda.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ray.zhixingplan.top

Java: enum Color { RED, GREEN }
来源：http://xow.shangyingyoupin.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mdn.zhijiandao.cn

Ruby: Color = %i[red green].freeze
来源：http://cox.guowangkeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bdt.sweek.top

[G16] 对象转数组 / 字典
来源：http://pyj.yongpay.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rgt.xuetiantiany.cn

PHP:  get_object_vars($obj);
来源：http://lmp.gogol.net.cn

JS:   Object.entries(obj)
来源：http://soe.wangdashe.top

TS:   Object.entries(obj)
来源：http://vfr.bbcook.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sho.yueranfly.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://afg.ctjpmb.com

Ruby: obj.instance_variables
来源：http://ayy.yangfankeji.com

C#:   // 用反射或 System.Text.Json
来源：http://aam.jianghu66.top

================================================================================
来源：http://wgo.zhaomingkeji.xyz

H. 异常与错误处理
来源：http://lhq.nanxinkj.top

================================================================================
来源：http://ogv.xylfe.cn

[H01] try / catch 基础
来源：http://cmy.xziqi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qwt.sweek.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xzf.yj20258888.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yza.ctjpmb.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://upr.jinqigufen.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kdj.shanyushiyangtech.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lhg.dianchejie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hug.jinghuilouyu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lsc.xylfe.cn

[H02] finally / ensure 收尾
来源：http://cae.xuanzx.com

Py:   try: f()⏎finally: cleanup()
来源：http://pgn.sjlbkw.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://loq.pycfn.com

JS:   try { f(); } finally { cleanup(); }
来源：http://ubc.iojbl.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cax.fanxiaobao.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://nac.jqgufenzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://iio.xinyue.icu

Ruby: begin; f; ensure; cleanup; end
来源：http://xiu.xziqi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hku.cheryme.top

[H03] 主动抛出异常
来源：http://thb.dianchejie.cn

Py:   raise ValueError("错误信息")
来源：http://lhq.zhongyouzk.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mdc.hnxiangtu.top

JS:   throw new Error("错误信息");
来源：http://rma.jinyuanbaomall.cn

TS:   throw new Error("错误信息");
来源：http://fpj.shuidangran.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://pkr.yueranfly.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sxf.9152youxi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://pbl.bjfxy.top

C#:   throw new ArgumentException("错误信息");
来源：http://dqa.yonumen.top

[H04] 自定义异常类型
来源：http://qbk.andypj.xyz

Py:   class MyError(Exception): pass
来源：http://xma.52xcode.cn

PHP:  class MyError extends RuntimeException {}
来源：http://uli.yueranfly.top

JS:   class MyError extends Error {}
来源：http://mdg.shuidangran.top

TS:   class MyError extends Error {}
来源：http://jep.wangshuangyany.cn

Java: class MyException extends RuntimeException {}
来源：http://iya.c1oappe.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wcy.yj20258.top

Ruby: class MyError < StandardError; end
来源：http://ljz.fanxiaobao.xyz

C#:   class MyException : Exception {}
来源：http://orn.xingfuxueyuan.xyz

[H05] 捕获特定类型
来源：http://jvz.sysykeji.top

Py:   except ValueError as e:
来源：http://xqu.redwolf501.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rcl.nanxuanxn.top

JS:   if (e instanceof TypeError) {}
来源：http://ity.jinyuanbaomall.cn

TS:   if (e instanceof TypeError) {}
来源：http://fzh.ydjk.org.cn

Java: catch (IOException | SQLException e) {}
来源：http://czu.wangshuangyany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://eak.yanxiufei.cn

Ruby: rescue ArgumentError => e
来源：http://bcb.andypj.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tzz.hywenlv.cn

[H06] 可选值 / 空值安全访问
来源：http://onc.yanxiufei.cn

Py:   value = d.get("k") or default
来源：http://naj.vehdjk.com

PHP:  $v = $d["k"] ?? null;
来源：http://ygs.xylfe.cn

JS:   obj?.a?.b;  d ?? default
来源：http://err.cucudq.cn

TS:   obj?.a?.b;  d ?? default
来源：http://bmr.epnwcf.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wsl.yueranfly.top

Go:   if v, ok := m["k"]; ok { }
来源：http://bdq.hesvh.cn

Ruby: d&.dig(:a, :b)
来源：http://emi.jiagoushi.top

C#:   obj?.A?.B ?? default
来源：http://yck.fktsv.cn

[H07] 断言
来源：http://njh.yueranfly.top

Py:   assert x > 0, "必须为正"
来源：http://nls.jinqigufen.top

PHP:  assert($x > 0);
来源：http://rqa.xylfe.cn

JS:   console.assert(x > 0);
来源：http://pha.nwbrower.top

TS:   console.assert(x > 0);
来源：http://hny.cdnleiting.top

Java: assert x > 0 : "必须为正";
来源：http://rki.feifeiyinyue.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ivp.hongshengwenyu.top

Ruby: raise "必须为正" unless x > 0
来源：http://pvu.nanxinkj.top

C#:   Debug.Assert(x > 0);
来源：http://ovo.jianghu66.top

[H08] 获取错误信息与堆栈
来源：http://bok.jiagoushi.top

Py:   str(e);  traceback.format_exc()
来源：http://wks.aizwys.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xww.birdmap.top

JS:   e.message;  e.stack
来源：http://uun.vqdsnc.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://leh.pengpengdd.cyou

Java: e.getMessage();  e.printStackTrace()
来源：http://ffs.shanyushiyangkeji.top

Go:   err.Error()
来源：http://isb.zhiwuduotai.top

Ruby: e.message;  e.backtrace
来源：http://tmu.ybcxt.top

C#:   e.Message;  e.StackTrace
来源：http://xyi.vehdjk.com

[H09] 带错误码的异常
来源：http://zxk.bbcook.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://iuk.ctjpmb.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://iag.c1oappe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sdp.sxryk.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yqv.jinghuilouyu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gwf.jqgfzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pjw.ehwqpu.com

Ruby: raise MyError.new("fail", 500)
来源：http://hlp.aibaodan.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wzk.guannengcc.top

[H10] 资源自动释放
来源：http://rtu.ydjk.org.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qea.yanxiufei.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tzj.jqgufenzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zqq.fktsv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ycx.redwolf501.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kdu.daria6918.cn

Go:   defer f.Close()
来源：http://skp.haohaochexian.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mxj.chenlongwang.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lyk.snrcjt.cn

================================================================================
来源：http://bgq.gogol.net.cn

I. 正则表达式
来源：http://agq.redwolf501.top

================================================================================
来源：http://cma.dianchejie.cn

[I01] 判断是否匹配
来源：http://odk.nanxinkj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://usu.wangdashe.top

PHP:  preg_match('/\d+/', $s);
来源：http://fic.jinghuilouyu.cn

JS:   /\d+/.test(s)
来源：http://qwn.chenlongwang.top

TS:   /\d+/.test(s)
来源：http://fvn.jqgufenzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://spg.jqgfzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://etm.mhx1999.top

Ruby: s.match?(/\d+/)
来源：http://qqc.chenlongwang.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://aaq.pengpengdd.cyou

[I02] 提取所有匹配
来源：http://ady.jinqigfzy.top

Py:   re.findall(r"\d+", s)
来源：http://lfi.c1oappe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dwt.gogol.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wps.yj20258.top

TS:   s.match(/\d+/g)
来源：http://bby.xziqi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qhc.chenzaomai.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cac.zhengqikj.top

Ruby: s.scan(/\d+/)
来源：http://lhx.yonumen.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://amd.pycfn.com

[I03] 提取捕获分组
来源：http://fsm.gzhubu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hle.fktsv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sbz.chenzaomai.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vfo.zhoulong.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://agw.gaohongyu789.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ovp.jinyuanbaomall.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xty.fehbvm.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nrv.tianlin.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fsa.chenjidiqi.icu

[I04] 正则替换
来源：http://ujf.fehbvm.com

Py:   re.sub(r"\d+", "#", s)
来源：http://mxc.aibaodan.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lmm.zhengqikj.top

JS:   s.replace(/\d+/g, "#")
来源：http://iin.chenjidiqi.icu

TS:   s.replace(/\d+/g, "#")
来源：http://lej.fzhhl.top

Java: s.replaceAll("\\d+", "#")
来源：http://ctj.wangdashe.top

Go:   re.ReplaceAllString(s, "#")
来源：http://gqa.dashuyun.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://how.yj20258888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wrz.52xcode.cn

[I05] 按正则拆分
来源：http://gzw.hesvh.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xsh.zdbjq.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uwo.zhixingplan.top

JS:   s.split(/\s*,\s*/)
来源：http://vgf.birdmap.top

TS:   s.split(/\s*,\s*/)
来源：http://smx.chenzaomai.com

Java: s.split("\\s*,\\s*")
来源：http://jsr.jinghuilouyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bew.haohaochexian.top

Ruby: s.split(/\s*,\s*/)
来源：http://gid.jinghuilouyu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vxr.uphjek.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rnu.zhongyouzk.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://iok.jqgfzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nze.nanxuanxn.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ess.shangyingyoupin.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nfw.aibaodan.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://snd.hammf.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zko.shangyingyoupin.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bnt.guowangkeji.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dny.mhx1999.top

[I07] 忽略大小写与多行模式
来源：http://avt.ydjk.org.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hfd.fktsv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gzu.smart0.xyz


<!-- 参考信息 -->