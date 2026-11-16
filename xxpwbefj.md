代发 wailian999

Py:   class User: pass
来源：http://jgu.sysykeji.top

PHP:  class User {}
来源：http://kqo.sxryk.cn

JS:   class User {}
来源：http://lia.xinyue.icu

TS:   class User { name: string = ""; }
来源：http://jtp.c1oappe.top

Java: class User {}
来源：http://iem.smart0.xyz

Go:   type User struct { Name string }
来源：http://snp.fehbvm.com

Ruby: class User; end
来源：http://avs.zhixingplan.top

C#:   class User {}
来源：http://clz.hysaishi.cn

[G02] 构造函数
来源：http://lnd.ivvv.top

Py:   def __init__(self, name): self.name = name
来源：http://nyh.ydzc1.top

PHP:  public function __construct(public string $name) {}
来源：http://gab.vqdsnc.cn

JS:   constructor(name) { this.name = name; }
来源：http://bvm.sweek.top

TS:   constructor(public name: string) {}
来源：http://ukp.zycfv.cn

Java: User(String name) { this.name = name; }
来源：http://jsl.zhongyouzk.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rfy.jyoumei.cn

Ruby: def initialize(name); @name = name; end
来源：http://joz.yj202588.top

C#:   public User(string name) { Name = name; }
来源：http://qmn.daria6918.cn

[G03] 实例属性
来源：http://jto.quarkkingdee.top

Py:   self.name = "x"
来源：http://mfk.wangdashe.top

PHP:  public string $name = "x";
来源：http://nyp.hysaishi.cn

JS:   this.name = "x";
来源：http://ysw.jinyuanbaomall.cn

TS:   name: string = "x";
来源：http://ljw.jiagoushi.top

Java: private String name;
来源：http://pnp.guowangkeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lek.jqgfzy.top

Ruby: @name = "x"
来源：http://fld.snrcjt.cn

C#:   public string Name { get; set; } = "x";
来源：http://fjc.ydjk.org.cn

[G04] 定义方法
来源：http://fae.jiagoushi.top

Py:   def greet(self): return self.name
来源：http://ijz.sjlbkw.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://arq.iojbl.cn

JS:   greet() { return this.name; }
来源：http://fdo.yongpay.top

TS:   greet(): string { return this.name; }
来源：http://pwj.andypj.xyz

Java: String greet() { return name; }
来源：http://lmw.smart0.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://jjj.smart0.xyz

Ruby: def greet; @name; end
来源：http://zoz.smart0.xyz

C#:   public string Greet() => Name;
来源：http://mxt.yongpay.top

[G05] 继承
来源：http://myv.nwbrower.top

Py:   class Admin(User): pass
来源：http://jzh.yj20258.top

PHP:  class Admin extends User {}
来源：http://mbb.haohaochexian.top

JS:   class Admin extends User {}
来源：http://yls.gotoacloud.top

TS:   class Admin extends User {}
来源：http://qkw.gzhubu.top

Java: class Admin extends User {}
来源：http://byr.yuanzhike.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rla.nanxuanxn.top

Ruby: class Admin < User; end
来源：http://yhf.meibo888.top

C#:   class Admin : User {}
来源：http://omx.hcnkem.com

[G06] 重写方法
来源：http://cou.jyoumei.cn

Py:   def greet(self): return "admin"
来源：http://ozp.52xcode.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://lbb.zhijiandao.cn

JS:   greet() { return "admin"; }
来源：http://esl.zhijiandao.cn

TS:   greet(): string { return "admin"; }
来源：http://nnp.jinqigfzy.top

Java: @Override String greet() { return "admin"; }
来源：http://zda.xuanzx.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://noh.xuanzx.com

Ruby: def greet; "admin"; end
来源：http://zte.aibaodan.cn

C#:   public override string Greet() => "admin";
来源：http://nkx.pycfn.com

[G07] 调用父类方法
来源：http://yci.yj20258888.top

Py:   super().greet()
来源：http://vkn.zhiwuduotai.top

PHP:  parent::greet();
来源：http://bhv.ivvv.top

JS:   super.greet();
来源：http://ukl.wangshuangyany.cn

TS:   super.greet();
来源：http://hlw.jianghu66.top

Java: super.greet();
来源：http://kwn.redwolf501.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://upx.gaohongyu789.top

Ruby: super
来源：http://lby.yangfankeji.com

C#:   base.Greet();
来源：http://mpe.hnqzz.top

[G08] 静态方法与属性
来源：http://kqf.tanke756.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mtc.sysykeji.top

PHP:  public static function f() {}
来源：http://kxn.xylfe.cn

JS:   static f() {}
来源：http://emq.aibaodan.cn

TS:   static f(): void {}
来源：http://rxw.xylfe.cn

Java: static void f() {}
来源：http://irw.bjfxy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://vqc.c1oappe.top

Ruby: def self.f; end
来源：http://cff.hysaishi.cn

C#:   public static void F() {}
来源：http://bea.zhaomingkeji.xyz

[G09] 接口 / 抽象类
来源：http://qzx.hongshengwenyu.top

Py:   from abc import ABC, abstractmethod
来源：http://hie.chenlongwang.top

PHP:  interface Shape { public function area(): float; }
来源：http://bdf.kuanghao11.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nvp.52xcode.cn

TS:   interface Shape { area(): number; }
来源：http://foz.aizwys.cn

Java: interface Shape { double area(); }
来源：http://djm.jqgufenzy.top

Go:   type Shape interface { Area() float64 }
来源：http://etr.guowangkeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://opv.hammf.cn

C#:   interface IShape { double Area(); }
来源：http://mfp.andypj.xyz

[G10] 访问控制
来源：http://frp.haohaochexian.top

Py:   约定 _protected / __private（不强制）
来源：http://lpk.52xcode.cn

PHP:  public / protected / private
来源：http://yds.zhijiandao.cn

JS:   #private 字段；其余公开
来源：http://daq.tianlin.xyz

TS:   public / protected / private
来源：http://wym.ydjk.org.cn

Java: public / protected / private / 默认包级
来源：http://pma.ydjk.org.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://llr.jinyuanbaomall.cn

Ruby: public / protected / private
来源：http://gxt.andypj.xyz

C#:   public / protected / private / internal
来源：http://jzp.sufxvd.cn

[G11] getter / setter
来源：http://jer.vqdsnc.cn

Py:   @property 与 @x.setter
来源：http://dli.jlsjyb.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://seq.cashguo.top

JS:   get name() { return this._name; }
来源：http://uui.316326.xyz

TS:   get name(): string { return this._name; }
来源：http://zxi.jlsjyb.cn

Java: public String getName() { return name; }
来源：http://imc.pycfn.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://fvh.ivvv.top

Ruby: attr_accessor :name
来源：http://asg.cucudq.cn

C#:   public string Name { get; set; }
来源：http://lpl.ywan-chungtsiang.top

[G12] 对象转字符串
来源：http://ahk.guannengcc.top

Py:   def __str__(self): return self.name
来源：http://ons.fanxiaobao.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://nor.sysykeji.top

JS:   toString() { return this.name; }
来源：http://oxi.gotoacloud.top

TS:   toString(): string { return this.name; }
来源：http://sgv.sxryk.cn

Java: @Override public String toString() { return name; }
来源：http://qvj.mhx1999.top

Go:   func (u User) String() string { return u.Name }
来源：http://mcv.fktsv.cn

Ruby: def to_s; @name; end
来源：http://uwk.cucudq.cn

C#:   public override string ToString() => Name;
来源：http://tgg.ctjpmb.com

[G13] 判断对象类型
来源：http://nni.hysaishi.cn

Py:   isinstance(u, User)
来源：http://jnt.yfazqb.com

PHP:  $u instanceof User
来源：http://gyl.pycfn.com

JS:   u instanceof User
来源：http://qjy.fehbvm.com

TS:   u instanceof User
来源：http://ipb.bbcook.cn

Java: u instanceof User
来源：http://cgl.tian-w.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://toi.guannengcc.top

Ruby: u.is_a?(User)
来源：http://slt.guannengcc.top

C#:   u is User
来源：http://yxs.ctjpmb.com

[G14] 数据类 / record
来源：http://hgi.sysykeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zav.hfpthk.cn

PHP:  // 用 readonly 属性模拟
来源：http://kjr.zdqjudy.top

JS:   // 无内置：普通类或对象字面量
来源：http://dyh.zdbjq.cn

TS:   type User = { name: string; age: number };
来源：http://ygq.xylfe.cn

Java: record User(String name, int age) {}
来源：http://oaj.yueranfly.top

Go:   type User struct { Name string; Age int }
来源：http://uhg.tianlin.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mlx.xuetiantiany.cn

C#:   record User(string Name, int Age);
来源：http://why.shzxlz.cn

[G15] 枚举
来源：http://iou.sufxvd.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://iwz.hywenlv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ujo.meibo888.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://icf.sufxvd.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gkv.cucudq.cn

Java: enum Color { RED, GREEN }
来源：http://zuv.vqdsnc.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xog.vehdjk.com

Ruby: Color = %i[red green].freeze
来源：http://vvq.yonumen.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yiv.yueranfly.top

[G16] 对象转数组 / 字典
来源：http://hkl.316326.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fqn.sysykeji.top

PHP:  get_object_vars($obj);
来源：http://dfi.zycfv.cn

JS:   Object.entries(obj)
来源：http://kwr.chenzaomai.com

TS:   Object.entries(obj)
来源：http://aox.aibaodan.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://upw.ybcxt.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://vlb.hnqzz.top

Ruby: obj.instance_variables
来源：http://nua.iojbl.cn

C#:   // 用反射或 System.Text.Json
来源：http://azz.tarul.cn

================================================================================
来源：http://oda.gogol.net.cn

H. 异常与错误处理
来源：http://hiv.ivvv.top

================================================================================
来源：http://vyr.wangshuangyany.cn

[H01] try / catch 基础
来源：http://kun.jqgfzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fch.aibaodan.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gct.fzhhl.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tvb.zdbjq.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sgk.yuxming.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ejh.quarkkingdee.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xka.chenjidiqi.icu

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rbu.hywenlv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ajl.xuanzx.com

[H02] finally / ensure 收尾
来源：http://yrt.cqqwz.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dwz.c1oappe.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://qrn.kuanghao11.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bmt.gotoacloud.top

TS:   try { f(); } finally { cleanup(); }
来源：http://faa.zhijiandao.cn

Java: try { f(); } finally { cleanup(); }
来源：http://oqn.yuxming.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://lrm.shzxlz.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://oet.feifeiyinyue.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://vto.ybcxt.top

[H03] 主动抛出异常
来源：http://eob.chenlongwang.top

Py:   raise ValueError("错误信息")
来源：http://bai.hysaishi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uan.tanke756.top

JS:   throw new Error("错误信息");
来源：http://ujp.jlsjyb.cn

TS:   throw new Error("错误信息");
来源：http://wri.birdmap.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://kiv.zdbjq.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kdc.shanyushiyangtech.top

Ruby: raise ArgumentError, "错误信息"
来源：http://khk.jianghu66.top

C#:   throw new ArgumentException("错误信息");
来源：http://nsn.jlsjyb.cn

[H04] 自定义异常类型
来源：http://wua.gzhubu.top

Py:   class MyError(Exception): pass
来源：http://jau.svipenyu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qia.yuxming.cn

JS:   class MyError extends Error {}
来源：http://xjp.yj20258888.top

TS:   class MyError extends Error {}
来源：http://dlr.cashguo.top

Java: class MyException extends RuntimeException {}
来源：http://rfm.yj20258.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rvi.svipenyu.cn

Ruby: class MyError < StandardError; end
来源：http://oub.chenjidiqi.icu

C#:   class MyException : Exception {}
来源：http://qfc.daxiang520.top

[H05] 捕获特定类型
来源：http://zci.hywenlv.cn

Py:   except ValueError as e:
来源：http://zop.cdnleiting.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fjo.vqdsnc.cn

JS:   if (e instanceof TypeError) {}
来源：http://can.sysykeji.top

TS:   if (e instanceof TypeError) {}
来源：http://cmm.fzhhl.top

Java: catch (IOException | SQLException e) {}
来源：http://fsh.tarul.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://slv.yanxiufei.cn

Ruby: rescue ArgumentError => e
来源：http://org.jinyuanbaomall.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://osj.jianghu66.top

[H06] 可选值 / 空值安全访问
来源：http://rxz.pengpengdd.cyou

Py:   value = d.get("k") or default
来源：http://uzq.hammf.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bmt.redwolf501.top

JS:   obj?.a?.b;  d ?? default
来源：http://xfx.kuanghao11.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cje.chenzaomai.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ptb.hammf.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bdz.hcnkem.com

Ruby: d&.dig(:a, :b)
来源：http://erg.shanyushiyangkeji.top

C#:   obj?.A?.B ?? default
来源：http://hml.gotoacloud.top

[H07] 断言
来源：http://evf.tian-w.cn

Py:   assert x > 0, "必须为正"
来源：http://ixg.zhoulong.xyz

PHP:  assert($x > 0);
来源：http://fgc.bbcook.cn

JS:   console.assert(x > 0);
来源：http://jgj.guannengcc.top

TS:   console.assert(x > 0);
来源：http://clf.yangfankeji.com

Java: assert x > 0 : "必须为正";
来源：http://rlk.dashuyun.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jea.ywan-chungtsiang.top

Ruby: raise "必须为正" unless x > 0
来源：http://lhd.vehdjk.com

C#:   Debug.Assert(x > 0);
来源：http://ofr.chenzaomai.com

[H08] 获取错误信息与堆栈
来源：http://hdk.tian-w.cn

Py:   str(e);  traceback.format_exc()
来源：http://jxd.svipenyu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qfk.meibo888.top

JS:   e.message;  e.stack
来源：http://eaq.fehbvm.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://ega.xinyue.icu

Java: e.getMessage();  e.printStackTrace()
来源：http://was.yongpay.top

Go:   err.Error()
来源：http://ppy.cucudq.cn

Ruby: e.message;  e.backtrace
来源：http://dfe.nanxinkj.top

C#:   e.Message;  e.StackTrace
来源：http://jod.aibaodan.cn

[H09] 带错误码的异常
来源：http://xtz.fzhhl.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bmb.andypj.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://kmx.hongshengwenyu.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nwo.yj20258.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vgk.meibo888.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jnl.jianghu66.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zkt.zhiwuduotai.top

Ruby: raise MyError.new("fail", 500)
来源：http://lse.yueranfly.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xrq.ppjwa.cn

[H10] 资源自动释放
来源：http://qrp.ydjk.org.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://apx.haohaochexian.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ent.redwolf501.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://raq.cheryme.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ote.ydjk.org.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://eue.tanke756.top

Go:   defer f.Close()
来源：http://bnd.jinyuanbaomall.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xll.fzhhl.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://iiy.sufxvd.cn

================================================================================
来源：http://dph.zhengqikj.top

I. 正则表达式
来源：http://mmq.sjlbkw.cn

================================================================================
来源：http://wxa.quarkkingdee.top

[I01] 判断是否匹配
来源：http://mxm.shanyushiyangtech.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ukr.yangfankeji.com

PHP:  preg_match('/\d+/', $s);
来源：http://pli.zhijiandao.cn

JS:   /\d+/.test(s)
来源：http://poi.52xcode.cn

TS:   /\d+/.test(s)
来源：http://jlr.iojbl.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kfq.sufxvd.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fal.yuxming.cn

Ruby: s.match?(/\d+/)
来源：http://gpi.xuetiantiany.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jeo.sweek.top

[I02] 提取所有匹配
来源：http://eme.316326.xyz

Py:   re.findall(r"\d+", s)
来源：http://odb.xuanzx.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ies.xuetiantiany.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rwi.hammf.cn

TS:   s.match(/\d+/g)
来源：http://kes.shuidangran.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ogl.hysaishi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rky.yj202588.top

Ruby: s.scan(/\d+/)
来源：http://pzh.zhongyouzk.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gge.jinqigufen.top

[I03] 提取捕获分组
来源：http://sap.yongpay.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pex.xylfe.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rjd.xinyue.icu

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dfo.daria6918.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kof.tianlin.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xex.zhiwuduotai.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://awh.hongshengwenyu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ryb.quarkkingdee.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yfk.ehwqpu.com

[I04] 正则替换
来源：http://jrt.yuxming.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hal.ybcxt.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dyr.hfpthk.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ozf.cashguo.top

TS:   s.replace(/\d+/g, "#")
来源：http://ekx.havefunace.top

Java: s.replaceAll("\\d+", "#")
来源：http://dhv.yonumen.top

Go:   re.ReplaceAllString(s, "#")
来源：http://uol.ehwqpu.com

Ruby: s.gsub(/\d+/, "#")
来源：http://mmn.kuanghao11.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vjh.yangfankeji.com

[I05] 按正则拆分
来源：http://vwl.chenlongwang.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wfg.yj20258.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nte.hnxiangtu.top

JS:   s.split(/\s*,\s*/)
来源：http://ile.yonumen.top

TS:   s.split(/\s*,\s*/)
来源：http://xuh.uphjek.com

Java: s.split("\\s*,\\s*")
来源：http://qnd.uphjek.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lvj.xziqi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://lex.fengsongda.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bgo.ppjwa.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dmg.shuidangran.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://src.kuanghao11.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zuy.andypj.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://muj.kuanghao11.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pgr.zhixingplan.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jfw.cucudq.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://esz.xinyue.icu

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://eum.ehwqpu.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qjj.0kj1m.cn

[I07] 忽略大小写与多行模式
来源：http://vjq.bjfxy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yrj.cdnleiting.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ywf.cashguo.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://puh.tarul.cn

TS:   /error/gim
来源：http://yxq.pengpengdd.cyou

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://psw.vehdjk.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hqh.ydjk.org.cn


<!-- 参考信息 -->