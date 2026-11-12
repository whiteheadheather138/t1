代发 wailian999

Py:   class User: pass
来源：http://jpk.chenlongwang.top

PHP:  class User {}
来源：http://spp.bjfxy.top

JS:   class User {}
来源：http://rbc.zdbjq.cn

TS:   class User { name: string = ""; }
来源：http://vzr.ivvv.top

Java: class User {}
来源：http://xef.cdnleiting.top

Go:   type User struct { Name string }
来源：http://xit.9152youxi.cn

Ruby: class User; end
来源：http://hpa.yanxiufei.cn

C#:   class User {}
来源：http://ulf.cashguo.top

[G02] 构造函数
来源：http://yoc.zhixingplan.top

Py:   def __init__(self, name): self.name = name
来源：http://had.jinghuilouyu.cn

PHP:  public function __construct(public string $name) {}
来源：http://ssk.bbcook.cn

JS:   constructor(name) { this.name = name; }
来源：http://bds.smart0.xyz

TS:   constructor(public name: string) {}
来源：http://jth.ydzc1.top

Java: User(String name) { this.name = name; }
来源：http://knn.kuanghao11.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hah.xziqi.cn

Ruby: def initialize(name); @name = name; end
来源：http://nut.birdmap.top

C#:   public User(string name) { Name = name; }
来源：http://rzr.tianlin.xyz

[G03] 实例属性
来源：http://ewn.nanxinkj.top

Py:   self.name = "x"
来源：http://fyw.hnxiangtu.top

PHP:  public string $name = "x";
来源：http://jxw.ydzc1.top

JS:   this.name = "x";
来源：http://qzm.ywan-chungtsiang.top

TS:   name: string = "x";
来源：http://bdn.ydzc1.top

Java: private String name;
来源：http://yrs.zdbjq.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qrq.hnqzz.top

Ruby: @name = "x"
来源：http://mru.xinyue.icu

C#:   public string Name { get; set; } = "x";
来源：http://qsf.ybcxt.top

[G04] 定义方法
来源：http://gho.ctjpmb.com

Py:   def greet(self): return self.name
来源：http://uql.yangfankeji.com

PHP:  public function greet(): string { return $this->name; }
来源：http://ywr.jinqigufen.top

JS:   greet() { return this.name; }
来源：http://ecf.sjlbkw.cn

TS:   greet(): string { return this.name; }
来源：http://hmf.yj20258888.top

Java: String greet() { return name; }
来源：http://kzh.fehbvm.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://grf.yangfankeji.com

Ruby: def greet; @name; end
来源：http://nbr.vehdjk.com

C#:   public string Greet() => Name;
来源：http://tlq.jianghu66.top

[G05] 继承
来源：http://lqq.dianchejie.cn

Py:   class Admin(User): pass
来源：http://fwm.iojbl.cn

PHP:  class Admin extends User {}
来源：http://gjk.tianlin.xyz

JS:   class Admin extends User {}
来源：http://olf.fengsongda.top

TS:   class Admin extends User {}
来源：http://acm.mhx1999.top

Java: class Admin extends User {}
来源：http://fhj.ehwqpu.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ame.cheryme.top

Ruby: class Admin < User; end
来源：http://qqa.yj20258888.top

C#:   class Admin : User {}
来源：http://snb.yuxming.cn

[G06] 重写方法
来源：http://ayk.jlsjyb.cn

Py:   def greet(self): return "admin"
来源：http://anv.bjfxy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://exa.yj20258888.top

JS:   greet() { return "admin"; }
来源：http://dge.shanyushiyangtech.top

TS:   greet(): string { return "admin"; }
来源：http://nil.pycfn.com

Java: @Override String greet() { return "admin"; }
来源：http://ywt.xingfuxueyuan.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ngo.smart0.xyz

Ruby: def greet; "admin"; end
来源：http://wdo.xuetiantiany.cn

C#:   public override string Greet() => "admin";
来源：http://ybv.jinqigufen.top

[G07] 调用父类方法
来源：http://bnf.zhiwuduotai.top

Py:   super().greet()
来源：http://icf.nanxuanxn.top

PHP:  parent::greet();
来源：http://bcx.gotoacloud.top

JS:   super.greet();
来源：http://avk.zhiwuduotai.top

TS:   super.greet();
来源：http://qjw.hfpthk.cn

Java: super.greet();
来源：http://ppr.ehwqpu.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uje.daxiang520.top

Ruby: super
来源：http://epg.guannengcc.top

C#:   base.Greet();
来源：http://hdz.zdbjq.cn

[G08] 静态方法与属性
来源：http://akm.nanxinkj.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nif.tarul.cn

PHP:  public static function f() {}
来源：http://ihr.yj202588.top

JS:   static f() {}
来源：http://iuz.jlsjyb.cn

TS:   static f(): void {}
来源：http://ucg.zhoulong.xyz

Java: static void f() {}
来源：http://wxj.0kj1m.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ezu.cucudq.cn

Ruby: def self.f; end
来源：http://bxx.nanxuanxn.top

C#:   public static void F() {}
来源：http://wsr.hnxiangtu.top

[G09] 接口 / 抽象类
来源：http://wac.tianlin.xyz

Py:   from abc import ABC, abstractmethod
来源：http://zuq.fzhhl.top

PHP:  interface Shape { public function area(): float; }
来源：http://acv.guowangkeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://erh.hnqzz.top

TS:   interface Shape { area(): number; }
来源：http://wup.fehbvm.com

Java: interface Shape { double area(); }
来源：http://ors.shuidangran.top

Go:   type Shape interface { Area() float64 }
来源：http://qxj.jinghuilouyu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://acw.wangshuangyany.cn

C#:   interface IShape { double Area(); }
来源：http://ost.wangshuangyany.cn

[G10] 访问控制
来源：http://tgw.zycfv.cn

Py:   约定 _protected / __private（不强制）
来源：http://nep.wangdashe.top

PHP:  public / protected / private
来源：http://scg.jqgufenzy.top

JS:   #private 字段；其余公开
来源：http://jzh.guowangkeji.top

TS:   public / protected / private
来源：http://hfi.zdbjq.cn

Java: public / protected / private / 默认包级
来源：http://btt.sufxvd.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://pms.wangdashe.top

Ruby: public / protected / private
来源：http://mfh.yfazqb.com

C#:   public / protected / private / internal
来源：http://moh.jianghu66.top

[G11] getter / setter
来源：http://mnk.daxiang520.top

Py:   @property 与 @x.setter
来源：http://mjw.redwolf501.top

PHP:  public function getName(): string { return $this->name; }
来源：http://cyx.9152youxi.cn

JS:   get name() { return this._name; }
来源：http://wra.zycfv.cn

TS:   get name(): string { return this._name; }
来源：http://zsh.sxryk.cn

Java: public String getName() { return name; }
来源：http://isn.sufxvd.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://nor.redwolf501.top

Ruby: attr_accessor :name
来源：http://nus.chenzaomai.com

C#:   public string Name { get; set; }
来源：http://yki.yj20258888.top

[G12] 对象转字符串
来源：http://oxv.shuidangran.top

Py:   def __str__(self): return self.name
来源：http://meh.yuanzhike.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ydt.zhijiandao.cn

JS:   toString() { return this.name; }
来源：http://dji.gogol.net.cn

TS:   toString(): string { return this.name; }
来源：http://rxg.hywenlv.cn

Java: @Override public String toString() { return name; }
来源：http://wsz.yueranfly.top

Go:   func (u User) String() string { return u.Name }
来源：http://aih.guannengcc.top

Ruby: def to_s; @name; end
来源：http://boj.yueranfly.top

C#:   public override string ToString() => Name;
来源：http://qaw.ivvv.top

[G13] 判断对象类型
来源：http://jke.yj20258.top

Py:   isinstance(u, User)
来源：http://dvp.mhx1999.top

PHP:  $u instanceof User
来源：http://xna.pengpengdd.cyou

JS:   u instanceof User
来源：http://mmk.zycfv.cn

TS:   u instanceof User
来源：http://fxh.yangfankeji.com

Java: u instanceof User
来源：http://uqk.yuanzhike.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ius.fzhhl.top

Ruby: u.is_a?(User)
来源：http://bpq.zhongyouzk.top

C#:   u is User
来源：http://cou.tian-w.cn

[G14] 数据类 / record
来源：http://fpf.jianghu66.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cbi.mhx1999.top

PHP:  // 用 readonly 属性模拟
来源：http://okw.zycfv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://chx.yongpay.top

TS:   type User = { name: string; age: number };
来源：http://rab.fanxiaobao.xyz

Java: record User(String name, int age) {}
来源：http://nmn.zdbjq.cn

Go:   type User struct { Name string; Age int }
来源：http://erp.yongpay.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jyx.aizwys.cn

C#:   record User(string Name, int Age);
来源：http://gsa.svipenyu.cn

[G15] 枚举
来源：http://szp.ydjk.org.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ypv.yuxming.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://atw.uphjek.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ekr.chenjidiqi.icu

TS:   enum Color { Red = 1, Green = 2 }
来源：http://frf.wangdashe.top

Java: enum Color { RED, GREEN }
来源：http://xrf.yj20258.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sqw.bbcook.cn

Ruby: Color = %i[red green].freeze
来源：http://imu.9152youxi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://epp.vehdjk.com

[G16] 对象转数组 / 字典
来源：http://hdc.zhongyouzk.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jtg.daxiang520.top

PHP:  get_object_vars($obj);
来源：http://ijy.yfazqb.com

JS:   Object.entries(obj)
来源：http://bym.andypj.xyz

TS:   Object.entries(obj)
来源：http://fzo.dashuyun.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://voq.sufxvd.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://kaj.gotoacloud.top

Ruby: obj.instance_variables
来源：http://vrq.zhijiandao.cn

C#:   // 用反射或 System.Text.Json
来源：http://ibw.guowangkeji.top

================================================================================
来源：http://hqe.epnwcf.com

H. 异常与错误处理
来源：http://pgr.iojbl.cn

================================================================================
来源：http://rjw.jianghu66.top

[H01] try / catch 基础
来源：http://pgf.yanxiufei.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://psy.pengpengdd.cyou

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cla.zycfv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xzu.yj202588.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zhs.xylfe.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mpq.tianlin.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://utw.wangdashe.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hxd.yuanzhike.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://air.jqgfzy.top

[H02] finally / ensure 收尾
来源：http://imn.sweek.top

Py:   try: f()⏎finally: cleanup()
来源：http://ybs.gaohongyu789.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://zke.wangdashe.top

JS:   try { f(); } finally { cleanup(); }
来源：http://hie.yonumen.top

TS:   try { f(); } finally { cleanup(); }
来源：http://nix.cdnleiting.top

Java: try { f(); } finally { cleanup(); }
来源：http://xwd.jyoumei.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://dco.gogol.net.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bai.ybcxt.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://tyb.gaohongyu789.top

[H03] 主动抛出异常
来源：http://bsc.pycfn.com

Py:   raise ValueError("错误信息")
来源：http://old.nanxinkj.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://grm.tarul.cn

JS:   throw new Error("错误信息");
来源：http://ocl.jinqigufen.top

TS:   throw new Error("错误信息");
来源：http://xzv.ydzc1.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://etd.xinyue.icu

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jdh.fzhhl.top

Ruby: raise ArgumentError, "错误信息"
来源：http://egb.jinqigfzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://ygk.316326.xyz

[H04] 自定义异常类型
来源：http://sdn.ywan-chungtsiang.top

Py:   class MyError(Exception): pass
来源：http://kgo.yj20258888.top

PHP:  class MyError extends RuntimeException {}
来源：http://see.chenlongwang.top

JS:   class MyError extends Error {}
来源：http://ipt.pycfn.com

TS:   class MyError extends Error {}
来源：http://dxa.snrcjt.cn

Java: class MyException extends RuntimeException {}
来源：http://qab.jqgfzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vdq.hammf.cn

Ruby: class MyError < StandardError; end
来源：http://vzg.ydjk.org.cn

C#:   class MyException : Exception {}
来源：http://kjz.guowangkeji.top

[H05] 捕获特定类型
来源：http://voq.zhongyouzk.top

Py:   except ValueError as e:
来源：http://nxo.zhongyouzk.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://flh.kuanghao11.cn

JS:   if (e instanceof TypeError) {}
来源：http://tgi.aizwys.cn

TS:   if (e instanceof TypeError) {}
来源：http://vwj.cqqwz.cn

Java: catch (IOException | SQLException e) {}
来源：http://iav.jinyuanbaomall.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jrv.svipenyu.cn

Ruby: rescue ArgumentError => e
来源：http://gwk.316326.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qsf.9152youxi.cn

[H06] 可选值 / 空值安全访问
来源：http://myg.xylfe.cn

Py:   value = d.get("k") or default
来源：http://wtk.316326.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://wvn.gaohongyu789.top

JS:   obj?.a?.b;  d ?? default
来源：http://yts.xingfuxueyuan.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://svh.hfpthk.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://eit.pengpengdd.cyou

Go:   if v, ok := m["k"]; ok { }
来源：http://aof.cashguo.top

Ruby: d&.dig(:a, :b)
来源：http://iei.guannengcc.top

C#:   obj?.A?.B ?? default
来源：http://wct.cashguo.top

[H07] 断言
来源：http://tit.xinyue.icu

Py:   assert x > 0, "必须为正"
来源：http://pbv.fehbvm.com

PHP:  assert($x > 0);
来源：http://sru.vqdsnc.cn

JS:   console.assert(x > 0);
来源：http://sew.xziqi.cn

TS:   console.assert(x > 0);
来源：http://vne.hysaishi.cn

Java: assert x > 0 : "必须为正";
来源：http://ygc.zhiwuduotai.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cfo.pengpengdd.cyou

Ruby: raise "必须为正" unless x > 0
来源：http://oxy.wangshuangyany.cn

C#:   Debug.Assert(x > 0);
来源：http://buk.zhijiandao.cn

[H08] 获取错误信息与堆栈
来源：http://ufc.cdnleiting.top

Py:   str(e);  traceback.format_exc()
来源：http://evq.yj20258888.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hqh.zycfv.cn

JS:   e.message;  e.stack
来源：http://sjz.cdnleiting.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://orx.ydjk.org.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://reo.vqdsnc.cn

Go:   err.Error()
来源：http://jde.chenzaomai.com

Ruby: e.message;  e.backtrace
来源：http://gzj.zhixingplan.top

C#:   e.Message;  e.StackTrace
来源：http://ohv.ehwqpu.com

[H09] 带错误码的异常
来源：http://uzb.cqqwz.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vtv.jqgfzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ofc.hywenlv.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://awt.yangfankeji.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mcw.fktsv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rmq.zhijiandao.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lhr.zhengqikj.top

Ruby: raise MyError.new("fail", 500)
来源：http://zjz.nanxuanxn.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xyf.fanxiaobao.xyz

[H10] 资源自动释放
来源：http://wfr.shuidangran.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://xyu.fktsv.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jwo.bjfxy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://stn.zhixingplan.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zsj.hnxiangtu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xwy.ywan-chungtsiang.top

Go:   defer f.Close()
来源：http://uao.meibo888.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://oag.sjlbkw.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fvq.aizwys.cn

================================================================================
来源：http://psb.yongpay.top

I. 正则表达式
来源：http://htj.jqgufenzy.top

================================================================================
来源：http://eoh.jinqigufen.top

[I01] 判断是否匹配
来源：http://phr.kuanghao11.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vqi.sxryk.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rov.jinqigfzy.top

JS:   /\d+/.test(s)
来源：http://bzm.yueranfly.top

TS:   /\d+/.test(s)
来源：http://qye.shzxlz.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xtb.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://whh.yfazqb.com

Ruby: s.match?(/\d+/)
来源：http://eax.fengsongda.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dje.vehdjk.com

[I02] 提取所有匹配
来源：http://kjf.shanyushiyangtech.top

Py:   re.findall(r"\d+", s)
来源：http://psz.sufxvd.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ezw.gotoacloud.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fls.zhengqikj.top

TS:   s.match(/\d+/g)
来源：http://cpc.hywenlv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://odj.ctjpmb.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zxw.ydjk.org.cn

Ruby: s.scan(/\d+/)
来源：http://fkm.cucudq.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gvf.andypj.xyz

[I03] 提取捕获分组
来源：http://mqa.sysykeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://oee.gogol.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wky.shuidangran.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fgf.xinyue.icu

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wbs.zhijiandao.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ixp.yj202588.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gkf.hesvh.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lcx.meibo888.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ffm.aibaodan.cn

[I04] 正则替换
来源：http://zrr.ybcxt.top

Py:   re.sub(r"\d+", "#", s)
来源：http://him.fzhhl.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://emh.jianghu66.top

JS:   s.replace(/\d+/g, "#")
来源：http://imi.ehwqpu.com

TS:   s.replace(/\d+/g, "#")
来源：http://lcl.jqgufenzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://dmt.zdqjudy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://kjt.hnqzz.top

Ruby: s.gsub(/\d+/, "#")
来源：http://txl.ctjpmb.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hlu.ybcxt.top

[I05] 按正则拆分
来源：http://luv.vqdsnc.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://moi.xylfe.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hqh.svipenyu.cn

JS:   s.split(/\s*,\s*/)
来源：http://jxh.yonumen.top

TS:   s.split(/\s*,\s*/)
来源：http://kxo.vehdjk.com

Java: s.split("\\s*,\\s*")
来源：http://uqx.zycfv.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://eqr.pycfn.com

Ruby: s.split(/\s*,\s*/)
来源：http://brd.gotoacloud.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://msb.316326.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cdy.sysykeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cda.0kj1m.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hdk.hysaishi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zip.52xcode.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vkl.ydzc1.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tjv.dashuyun.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gwq.jinqigfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jur.epnwcf.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oac.hysaishi.cn

[I07] 忽略大小写与多行模式
来源：http://wxy.hesvh.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qsh.ydzc1.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ugp.smart0.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://imi.xinyue.icu

TS:   /error/gim
来源：http://fii.zdbjq.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lva.aibaodan.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ort.zhaomingkeji.xyz


<!-- 参考信息 -->