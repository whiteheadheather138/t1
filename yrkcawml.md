代发 wailian999

Java: class User {}
来源：http://ixk.yueranfly.top

Go:   type User struct { Name string }
来源：http://gqh.yuanzhike.top

Ruby: class User; end
来源：http://yvf.pycfn.com

C#:   class User {}
来源：http://bjv.bjfxy.top

[G02] 构造函数
来源：http://wrj.yj20258888.top

Py:   def __init__(self, name): self.name = name
来源：http://hgd.meibo888.top

PHP:  public function __construct(public string $name) {}
来源：http://qtz.cqqwz.cn

JS:   constructor(name) { this.name = name; }
来源：http://krt.gaohongyu789.top

TS:   constructor(public name: string) {}
来源：http://ayx.yueranfly.top

Java: User(String name) { this.name = name; }
来源：http://aby.andypj.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jxi.guannengcc.top

Ruby: def initialize(name); @name = name; end
来源：http://ulf.aibaodan.cn

C#:   public User(string name) { Name = name; }
来源：http://xuz.chenzaomai.com

[G03] 实例属性
来源：http://lbd.hnqzz.top

Py:   self.name = "x"
来源：http://tmb.yueranfly.top

PHP:  public string $name = "x";
来源：http://nky.daria6918.cn

JS:   this.name = "x";
来源：http://lmi.wangshuangyany.cn

TS:   name: string = "x";
来源：http://gbu.hnxiangtu.top

Java: private String name;
来源：http://ove.havefunace.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rxx.chenzaomai.com

Ruby: @name = "x"
来源：http://qrd.jiagoushi.top

C#:   public string Name { get; set; } = "x";
来源：http://wqx.hesvh.cn

[G04] 定义方法
来源：http://cyh.pycfn.com

Py:   def greet(self): return self.name
来源：http://tpi.316326.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://sps.yj202588.top

JS:   greet() { return this.name; }
来源：http://tlx.epnwcf.com

TS:   greet(): string { return this.name; }
来源：http://jsk.zycfv.cn

Java: String greet() { return name; }
来源：http://hli.yj202588.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ghz.chenjidiqi.icu

Ruby: def greet; @name; end
来源：http://ybn.bbcook.cn

C#:   public string Greet() => Name;
来源：http://zgg.svipenyu.cn

[G05] 继承
来源：http://qlt.nanxinkj.top

Py:   class Admin(User): pass
来源：http://ukb.haohaochexian.top

PHP:  class Admin extends User {}
来源：http://nnh.tian-w.cn

JS:   class Admin extends User {}
来源：http://rml.zycfv.cn

TS:   class Admin extends User {}
来源：http://umr.quarkkingdee.top

Java: class Admin extends User {}
来源：http://umm.yanxiufei.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://faa.wangshuangyany.cn

Ruby: class Admin < User; end
来源：http://rzr.pycfn.com

C#:   class Admin : User {}
来源：http://dty.tanke756.top

[G06] 重写方法
来源：http://exu.shanyushiyangkeji.top

Py:   def greet(self): return "admin"
来源：http://vhm.mhx1999.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ytp.jinqigufen.top

JS:   greet() { return "admin"; }
来源：http://ypy.pengpengdd.cyou

TS:   greet(): string { return "admin"; }
来源：http://ibt.zhaomingkeji.xyz

Java: @Override String greet() { return "admin"; }
来源：http://wjg.wangdashe.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://enp.xingfuxueyuan.xyz

Ruby: def greet; "admin"; end
来源：http://ggk.shanyushiyangkeji.top

C#:   public override string Greet() => "admin";
来源：http://cpt.shzxlz.cn

[G07] 调用父类方法
来源：http://mqz.uphjek.com

Py:   super().greet()
来源：http://iyp.zhengqikj.top

PHP:  parent::greet();
来源：http://eqq.epnwcf.com

JS:   super.greet();
来源：http://pif.andypj.xyz

TS:   super.greet();
来源：http://iew.hysaishi.cn

Java: super.greet();
来源：http://icl.hysaishi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://unr.52xcode.cn

Ruby: super
来源：http://biv.hammf.cn

C#:   base.Greet();
来源：http://yhg.bbcook.cn

[G08] 静态方法与属性
来源：http://fij.zhijiandao.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dcd.zhoulong.xyz

PHP:  public static function f() {}
来源：http://nie.jlsjyb.cn

JS:   static f() {}
来源：http://cmu.gzhubu.top

TS:   static f(): void {}
来源：http://nfa.zhiwuduotai.top

Java: static void f() {}
来源：http://qzq.guannengcc.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://aav.haohaochexian.top

Ruby: def self.f; end
来源：http://kbf.tianlin.xyz

C#:   public static void F() {}
来源：http://egr.ctjpmb.com

[G09] 接口 / 抽象类
来源：http://udf.guannengcc.top

Py:   from abc import ABC, abstractmethod
来源：http://nxj.nanxuanxn.top

PHP:  interface Shape { public function area(): float; }
来源：http://oxd.xylfe.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bii.jqgufenzy.top

TS:   interface Shape { area(): number; }
来源：http://yei.zdbjq.cn

Java: interface Shape { double area(); }
来源：http://yyz.hcnkem.com

Go:   type Shape interface { Area() float64 }
来源：http://ylk.zhixingplan.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tri.bbcook.cn

C#:   interface IShape { double Area(); }
来源：http://opu.kuanghao11.cn

[G10] 访问控制
来源：http://eea.shanyushiyangkeji.top

Py:   约定 _protected / __private（不强制）
来源：http://wex.ivvv.top

PHP:  public / protected / private
来源：http://jez.tarul.cn

JS:   #private 字段；其余公开
来源：http://lkr.cdnleiting.top

TS:   public / protected / private
来源：http://hur.yj202588.top

Java: public / protected / private / 默认包级
来源：http://iae.zhongyouzk.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://drg.0kj1m.cn

Ruby: public / protected / private
来源：http://wxe.yuxming.cn

C#:   public / protected / private / internal
来源：http://vhr.yonumen.top

[G11] getter / setter
来源：http://zlv.nwbrower.top

Py:   @property 与 @x.setter
来源：http://dps.hongshengwenyu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dbi.aizwys.cn

JS:   get name() { return this._name; }
来源：http://kne.yvedp.cn

TS:   get name(): string { return this._name; }
来源：http://mpr.tian-w.cn

Java: public String getName() { return name; }
来源：http://dwb.0kj1m.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yin.jinqigfzy.top

Ruby: attr_accessor :name
来源：http://edy.chenjidiqi.icu

C#:   public string Name { get; set; }
来源：http://sqr.yanxiufei.cn

[G12] 对象转字符串
来源：http://lfx.xinyue.icu

Py:   def __str__(self): return self.name
来源：http://ali.ybcxt.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://jcw.cqqwz.cn

JS:   toString() { return this.name; }
来源：http://ndj.tian-w.cn

TS:   toString(): string { return this.name; }
来源：http://zhw.fzhhl.top

Java: @Override public String toString() { return name; }
来源：http://uld.ehwqpu.com

Go:   func (u User) String() string { return u.Name }
来源：http://mug.tianlin.xyz

Ruby: def to_s; @name; end
来源：http://gbq.hammf.cn

C#:   public override string ToString() => Name;
来源：http://xek.jinghuilouyu.cn

[G13] 判断对象类型
来源：http://lai.0kj1m.cn

Py:   isinstance(u, User)
来源：http://qnc.c1oappe.top

PHP:  $u instanceof User
来源：http://mes.cucudq.cn

JS:   u instanceof User
来源：http://cgw.redwolf501.top

TS:   u instanceof User
来源：http://jua.zycfv.cn

Java: u instanceof User
来源：http://fco.tian-w.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fhp.svipenyu.cn

Ruby: u.is_a?(User)
来源：http://ytj.jqgfzy.top

C#:   u is User
来源：http://zvj.yj20258888.top

[G14] 数据类 / record
来源：http://obr.hnxiangtu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dpb.316326.xyz

PHP:  // 用 readonly 属性模拟
来源：http://iyn.yj20258.top

JS:   // 无内置：普通类或对象字面量
来源：http://btt.cashguo.top

TS:   type User = { name: string; age: number };
来源：http://qkf.fengsongda.top

Java: record User(String name, int age) {}
来源：http://vbw.kuanghao11.cn

Go:   type User struct { Name string; Age int }
来源：http://vcf.yuanzhike.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gag.shanyushiyangtech.top

C#:   record User(string Name, int Age);
来源：http://elj.xuetiantiany.cn

[G15] 枚举
来源：http://dvb.chenzaomai.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lew.ydzc1.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://gjl.jqgufenzy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kxe.xinyue.icu

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wgy.redwolf501.top

Java: enum Color { RED, GREEN }
来源：http://zyv.yangfankeji.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fhe.zhixingplan.top

Ruby: Color = %i[red green].freeze
来源：http://vir.yfazqb.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cti.zhixingplan.top

[G16] 对象转数组 / 字典
来源：http://ykn.havefunace.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dfg.xingfuxueyuan.xyz

PHP:  get_object_vars($obj);
来源：http://ezg.hysaishi.cn

JS:   Object.entries(obj)
来源：http://twp.zycfv.cn

TS:   Object.entries(obj)
来源：http://czn.xuetiantiany.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wbo.wangdashe.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://chs.bbcook.cn

Ruby: obj.instance_variables
来源：http://yno.dashuyun.cn

C#:   // 用反射或 System.Text.Json
来源：http://ixx.svipenyu.cn

================================================================================
来源：http://itr.guowangkeji.top

H. 异常与错误处理
来源：http://qxq.shuidangran.top

================================================================================
来源：http://qtz.uphjek.com

[H01] try / catch 基础
来源：http://xcl.yj202588.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cft.daxiang520.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vly.yongpay.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ery.andypj.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gfl.cdnleiting.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zvi.nanxuanxn.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dwz.hnxiangtu.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qhv.jinyuanbaomall.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fsb.yuxming.cn

[H02] finally / ensure 收尾
来源：http://ydn.zhoulong.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://chk.hnxiangtu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://bef.jinyuanbaomall.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jtf.ybcxt.top

TS:   try { f(); } finally { cleanup(); }
来源：http://zbb.daria6918.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yrj.jinqigfzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://uqu.gaohongyu789.top

Ruby: begin; f; ensure; cleanup; end
来源：http://qeu.haohaochexian.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://zfz.cashguo.top

[H03] 主动抛出异常
来源：http://twt.yj202588.top

Py:   raise ValueError("错误信息")
来源：http://jtk.wangshuangyany.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://eqi.ydzc1.top

JS:   throw new Error("错误信息");
来源：http://rdp.redwolf501.top

TS:   throw new Error("错误信息");
来源：http://uuu.316326.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://hjq.gzhubu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dlm.sufxvd.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vlm.tian-w.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zcl.fanxiaobao.xyz

[H04] 自定义异常类型
来源：http://shl.yanxiufei.cn

Py:   class MyError(Exception): pass
来源：http://obs.daria6918.cn

PHP:  class MyError extends RuntimeException {}
来源：http://byu.zycfv.cn

JS:   class MyError extends Error {}
来源：http://mbe.fehbvm.com

TS:   class MyError extends Error {}
来源：http://tay.redwolf501.top

Java: class MyException extends RuntimeException {}
来源：http://xch.jianghu66.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vgh.tarul.cn

Ruby: class MyError < StandardError; end
来源：http://nll.gotoacloud.top

C#:   class MyException : Exception {}
来源：http://uty.tarul.cn

[H05] 捕获特定类型
来源：http://peh.kuanghao11.cn

Py:   except ValueError as e:
来源：http://uby.snrcjt.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://umo.hywenlv.cn

JS:   if (e instanceof TypeError) {}
来源：http://clk.316326.xyz

TS:   if (e instanceof TypeError) {}
来源：http://eag.aibaodan.cn

Java: catch (IOException | SQLException e) {}
来源：http://dub.sysykeji.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zie.cucudq.cn

Ruby: rescue ArgumentError => e
来源：http://hbo.redwolf501.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rwf.nanxinkj.top

[H06] 可选值 / 空值安全访问
来源：http://sxf.yvedp.cn

Py:   value = d.get("k") or default
来源：http://khb.pycfn.com

PHP:  $v = $d["k"] ?? null;
来源：http://hjg.hywenlv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hep.yongpay.top

TS:   obj?.a?.b;  d ?? default
来源：http://fwc.9152youxi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nnb.cdnleiting.top

Go:   if v, ok := m["k"]; ok { }
来源：http://rya.hammf.cn

Ruby: d&.dig(:a, :b)
来源：http://qog.birdmap.top

C#:   obj?.A?.B ?? default
来源：http://ckl.zhixingplan.top

[H07] 断言
来源：http://win.jinqigfzy.top

Py:   assert x > 0, "必须为正"
来源：http://gtt.yueranfly.top

PHP:  assert($x > 0);
来源：http://rco.yuanzhike.top

JS:   console.assert(x > 0);
来源：http://xxa.hesvh.cn

TS:   console.assert(x > 0);
来源：http://zgl.chenjidiqi.icu

Java: assert x > 0 : "必须为正";
来源：http://yht.jinghuilouyu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nga.vehdjk.com

Ruby: raise "必须为正" unless x > 0
来源：http://dqi.zhaomingkeji.xyz

C#:   Debug.Assert(x > 0);
来源：http://fun.ybcxt.top

[H08] 获取错误信息与堆栈
来源：http://etm.tarul.cn

Py:   str(e);  traceback.format_exc()
来源：http://tox.feifeiyinyue.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pjo.hywenlv.cn

JS:   e.message;  e.stack
来源：http://tnf.jinghuilouyu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rph.aibaodan.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://eom.xylfe.cn

Go:   err.Error()
来源：http://hen.andypj.xyz

Ruby: e.message;  e.backtrace
来源：http://sqo.zdbjq.cn

C#:   e.Message;  e.StackTrace
来源：http://keh.sweek.top

[H09] 带错误码的异常
来源：http://hks.sxryk.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://moe.sysykeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://vbq.ydjk.org.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://psm.bjfxy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mbr.zhiwuduotai.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bbm.chenzaomai.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bzc.cucudq.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jon.mhx1999.top

C#:   // 自定义异常类中加 Code 属性
来源：http://auo.9152youxi.cn

[H10] 资源自动释放
来源：http://mct.gotoacloud.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://cxe.xingfuxueyuan.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://idq.daxiang520.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bfz.yj20258.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://htz.yanxiufei.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bev.hammf.cn

Go:   defer f.Close()
来源：http://kcu.dashuyun.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yse.xziqi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ibb.hongshengwenyu.top

================================================================================
来源：http://evw.9152youxi.cn

I. 正则表达式
来源：http://jsk.dashuyun.cn

================================================================================
来源：http://obv.jiagoushi.top

[I01] 判断是否匹配
来源：http://set.jinqigfzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://btf.birdmap.top

PHP:  preg_match('/\d+/', $s);
来源：http://bmz.yj20258.top

JS:   /\d+/.test(s)
来源：http://mbt.jinyuanbaomall.cn

TS:   /\d+/.test(s)
来源：http://koc.sysykeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ylh.jlsjyb.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://asf.hywenlv.cn

Ruby: s.match?(/\d+/)
来源：http://mwy.nanxuanxn.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qaw.pengpengdd.cyou

[I02] 提取所有匹配
来源：http://bvx.xylfe.cn

Py:   re.findall(r"\d+", s)
来源：http://qla.aizwys.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cei.chenlongwang.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://oid.gaohongyu789.top

TS:   s.match(/\d+/g)
来源：http://gse.jyoumei.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://iks.hnxiangtu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://syh.bbcook.cn

Ruby: s.scan(/\d+/)
来源：http://fmu.jqgufenzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vaz.feifeiyinyue.top

[I03] 提取捕获分组
来源：http://tvj.gaohongyu789.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ztz.quarkkingdee.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ftg.yueranfly.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tsr.fehbvm.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://prh.jinghuilouyu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xok.ybcxt.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nsl.vqdsnc.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ahv.shanyushiyangkeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yip.hnxiangtu.top

[I04] 正则替换
来源：http://fsi.daxiang520.top

Py:   re.sub(r"\d+", "#", s)
来源：http://lfv.nanxinkj.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hrs.fengsongda.top

JS:   s.replace(/\d+/g, "#")
来源：http://nry.yanxiufei.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bok.hcnkem.com

Java: s.replaceAll("\\d+", "#")
来源：http://lpz.hcnkem.com

Go:   re.ReplaceAllString(s, "#")
来源：http://rtt.jyoumei.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ezz.yfazqb.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://svl.gogol.net.cn

[I05] 按正则拆分
来源：http://lzt.yj20258888.top

Py:   re.split(r"\s*,\s*", s)
来源：http://kdx.nanxinkj.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sqc.havefunace.top

JS:   s.split(/\s*,\s*/)
来源：http://gua.cucudq.cn

TS:   s.split(/\s*,\s*/)
来源：http://cqk.sxryk.cn

Java: s.split("\\s*,\\s*")
来源：http://poo.ehwqpu.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hok.nanxuanxn.top

Ruby: s.split(/\s*,\s*/)
来源：http://pfi.bbcook.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://apg.snrcjt.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tfa.jlsjyb.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hep.tian-w.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ruf.zdqjudy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yax.hammf.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pny.cashguo.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://olr.dianchejie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://myx.shuidangran.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cxk.c1oappe.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oie.quarkkingdee.top

[I07] 忽略大小写与多行模式
来源：http://zfk.guannengcc.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ptx.chenjidiqi.icu

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dgf.snrcjt.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ntb.yj20258888.top

TS:   /error/gim
来源：http://qoe.hcnkem.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yyl.dashuyun.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ngi.vehdjk.com

Ruby: s.scan(/error/i)
来源：http://ppl.bjfxy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pzg.hcnkem.com

[I08] 贪婪与非贪婪匹配
来源：http://zxz.yfazqb.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sro.nanxuanxn.top


<!-- 参考信息 -->