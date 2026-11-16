代发 wailian999

================================================================================
来源：http://hqu.shuidangran.top

G. 面向对象
来源：http://jle.jinghuilouyu.cn

================================================================================
来源：http://our.redwolf501.top

[G01] 定义类
来源：http://xqf.yueranfly.top

Py:   class User: pass
来源：http://iys.cdnleiting.top

PHP:  class User {}
来源：http://exb.yuxming.cn

JS:   class User {}
来源：http://sca.fzhhl.top

TS:   class User { name: string = ""; }
来源：http://otv.iojbl.cn

Java: class User {}
来源：http://ody.zhaomingkeji.xyz

Go:   type User struct { Name string }
来源：http://day.zdqjudy.top

Ruby: class User; end
来源：http://rdp.snrcjt.cn

C#:   class User {}
来源：http://izd.hongshengwenyu.top

[G02] 构造函数
来源：http://cpc.daxiang520.top

Py:   def __init__(self, name): self.name = name
来源：http://jbo.meibo888.top

PHP:  public function __construct(public string $name) {}
来源：http://fit.yueranfly.top

JS:   constructor(name) { this.name = name; }
来源：http://dpz.ywan-chungtsiang.top

TS:   constructor(public name: string) {}
来源：http://drx.hcnkem.com

Java: User(String name) { this.name = name; }
来源：http://qee.jlsjyb.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mgn.yfazqb.com

Ruby: def initialize(name); @name = name; end
来源：http://hvc.tarul.cn

C#:   public User(string name) { Name = name; }
来源：http://sww.jiagoushi.top

[G03] 实例属性
来源：http://pyj.ctjpmb.com

Py:   self.name = "x"
来源：http://qib.sxryk.cn

PHP:  public string $name = "x";
来源：http://dpe.nwbrower.top

JS:   this.name = "x";
来源：http://flm.xinyue.icu

TS:   name: string = "x";
来源：http://oib.ydzc1.top

Java: private String name;
来源：http://fuf.shuidangran.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ytk.yangfankeji.com

Ruby: @name = "x"
来源：http://xaw.yvedp.cn

C#:   public string Name { get; set; } = "x";
来源：http://knx.guowangkeji.top

[G04] 定义方法
来源：http://tyk.zdbjq.cn

Py:   def greet(self): return self.name
来源：http://usk.hfpthk.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://uqs.andypj.xyz

JS:   greet() { return this.name; }
来源：http://gea.ydjk.org.cn

TS:   greet(): string { return this.name; }
来源：http://nav.iojbl.cn

Java: String greet() { return name; }
来源：http://reg.cucudq.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://baw.shuidangran.top

Ruby: def greet; @name; end
来源：http://iih.zhijiandao.cn

C#:   public string Greet() => Name;
来源：http://owy.mhx1999.top

[G05] 继承
来源：http://fym.mhx1999.top

Py:   class Admin(User): pass
来源：http://bjs.jianghu66.top

PHP:  class Admin extends User {}
来源：http://qfv.uphjek.com

JS:   class Admin extends User {}
来源：http://uxx.yj202588.top

TS:   class Admin extends User {}
来源：http://gqu.hysaishi.cn

Java: class Admin extends User {}
来源：http://dbg.zhixingplan.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ipv.daxiang520.top

Ruby: class Admin < User; end
来源：http://aww.ivvv.top

C#:   class Admin : User {}
来源：http://kmp.zhaomingkeji.xyz

[G06] 重写方法
来源：http://iah.gogol.net.cn

Py:   def greet(self): return "admin"
来源：http://yps.yj20258.top

PHP:  public function greet(): string { return "admin"; }
来源：http://wya.jqgfzy.top

JS:   greet() { return "admin"; }
来源：http://oyz.hnxiangtu.top

TS:   greet(): string { return "admin"; }
来源：http://htr.fengsongda.top

Java: @Override String greet() { return "admin"; }
来源：http://pfm.jinghuilouyu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cyb.yuxming.cn

Ruby: def greet; "admin"; end
来源：http://jas.jqgufenzy.top

C#:   public override string Greet() => "admin";
来源：http://jld.ivvv.top

[G07] 调用父类方法
来源：http://jps.shangyingyoupin.top

Py:   super().greet()
来源：http://hnx.haohaochexian.top

PHP:  parent::greet();
来源：http://geg.nanxinkj.top

JS:   super.greet();
来源：http://fpz.vqdsnc.cn

TS:   super.greet();
来源：http://pqy.zhongyouzk.top

Java: super.greet();
来源：http://egt.xingfuxueyuan.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bux.daria6918.cn

Ruby: super
来源：http://gle.jlsjyb.cn

C#:   base.Greet();
来源：http://mti.bjfxy.top

[G08] 静态方法与属性
来源：http://cbp.shanyushiyangkeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lrt.pycfn.com

PHP:  public static function f() {}
来源：http://cws.jianghu66.top

JS:   static f() {}
来源：http://lde.snrcjt.cn

TS:   static f(): void {}
来源：http://buh.daria6918.cn

Java: static void f() {}
来源：http://zrg.jinyuanbaomall.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jfn.jlsjyb.cn

Ruby: def self.f; end
来源：http://bih.aizwys.cn

C#:   public static void F() {}
来源：http://uti.hysaishi.cn

[G09] 接口 / 抽象类
来源：http://jbx.ybcxt.top

Py:   from abc import ABC, abstractmethod
来源：http://opo.ydzc1.top

PHP:  interface Shape { public function area(): float; }
来源：http://kev.fengsongda.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://tfs.pycfn.com

TS:   interface Shape { area(): number; }
来源：http://jgh.hfpthk.cn

Java: interface Shape { double area(); }
来源：http://cjz.dianchejie.cn

Go:   type Shape interface { Area() float64 }
来源：http://tsm.ywan-chungtsiang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ykf.yongpay.top

C#:   interface IShape { double Area(); }
来源：http://ooi.vqdsnc.cn

[G10] 访问控制
来源：http://mki.aibaodan.cn

Py:   约定 _protected / __private（不强制）
来源：http://wyc.sxryk.cn

PHP:  public / protected / private
来源：http://xxs.hywenlv.cn

JS:   #private 字段；其余公开
来源：http://tuw.xuetiantiany.cn

TS:   public / protected / private
来源：http://cap.daria6918.cn

Java: public / protected / private / 默认包级
来源：http://bfd.jlsjyb.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://wnw.zhiwuduotai.top

Ruby: public / protected / private
来源：http://csm.hesvh.cn

C#:   public / protected / private / internal
来源：http://bvt.yfazqb.com

[G11] getter / setter
来源：http://cen.hesvh.cn

Py:   @property 与 @x.setter
来源：http://qjn.shuidangran.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jko.gaohongyu789.top

JS:   get name() { return this._name; }
来源：http://iwe.pycfn.com

TS:   get name(): string { return this._name; }
来源：http://pth.shzxlz.cn

Java: public String getName() { return name; }
来源：http://qle.zycfv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hoi.316326.xyz

Ruby: attr_accessor :name
来源：http://sfd.9152youxi.cn

C#:   public string Name { get; set; }
来源：http://thf.xinyue.icu

[G12] 对象转字符串
来源：http://wbj.xziqi.cn

Py:   def __str__(self): return self.name
来源：http://faj.aibaodan.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://kjh.tian-w.cn

JS:   toString() { return this.name; }
来源：http://gtl.uphjek.com

TS:   toString(): string { return this.name; }
来源：http://dnh.c1oappe.top

Java: @Override public String toString() { return name; }
来源：http://apb.hcnkem.com

Go:   func (u User) String() string { return u.Name }
来源：http://wev.sufxvd.cn

Ruby: def to_s; @name; end
来源：http://daw.cheryme.top

C#:   public override string ToString() => Name;
来源：http://ecr.shangyingyoupin.top

[G13] 判断对象类型
来源：http://oik.shuidangran.top

Py:   isinstance(u, User)
来源：http://wzg.zhixingplan.top

PHP:  $u instanceof User
来源：http://ugs.meibo888.top

JS:   u instanceof User
来源：http://jtf.wangdashe.top

TS:   u instanceof User
来源：http://xxg.hysaishi.cn

Java: u instanceof User
来源：http://egu.yj20258888.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://rwo.nanxuanxn.top

Ruby: u.is_a?(User)
来源：http://ijh.feifeiyinyue.top

C#:   u is User
来源：http://ula.chenjidiqi.icu

[G14] 数据类 / record
来源：http://lav.ywan-chungtsiang.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://byt.aizwys.cn

PHP:  // 用 readonly 属性模拟
来源：http://jww.yangfankeji.com

JS:   // 无内置：普通类或对象字面量
来源：http://abw.fktsv.cn

TS:   type User = { name: string; age: number };
来源：http://flv.quarkkingdee.top

Java: record User(String name, int age) {}
来源：http://yzi.ywan-chungtsiang.top

Go:   type User struct { Name string; Age int }
来源：http://tha.fengsongda.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xpk.nanxinkj.top

C#:   record User(string Name, int Age);
来源：http://wwe.hnxiangtu.top

[G15] 枚举
来源：http://odx.zhaomingkeji.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jjh.316326.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://fqr.zhoulong.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bff.aibaodan.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ibw.hammf.cn

Java: enum Color { RED, GREEN }
来源：http://vfu.uphjek.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://adq.jinqigufen.top

Ruby: Color = %i[red green].freeze
来源：http://qdj.cdnleiting.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qea.svipenyu.cn

[G16] 对象转数组 / 字典
来源：http://buj.hywenlv.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baf.shanyushiyangkeji.top

PHP:  get_object_vars($obj);
来源：http://dfo.chenlongwang.top

JS:   Object.entries(obj)
来源：http://jkp.cucudq.cn

TS:   Object.entries(obj)
来源：http://tbe.chenzaomai.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dtq.xuanzx.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://epf.xingfuxueyuan.xyz

Ruby: obj.instance_variables
来源：http://xft.yangfankeji.com

C#:   // 用反射或 System.Text.Json
来源：http://phs.yj20258888.top

================================================================================
来源：http://dnf.9152youxi.cn

H. 异常与错误处理
来源：http://ljb.shangyingyoupin.top

================================================================================
来源：http://kge.cashguo.top

[H01] try / catch 基础
来源：http://iyp.ybcxt.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://aqm.sxryk.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://whj.sysykeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dxf.aizwys.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gaj.c1oappe.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wvk.uphjek.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vnt.shanyushiyangtech.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://woh.jqgufenzy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pac.fengsongda.top

[H02] finally / ensure 收尾
来源：http://bph.zhongyouzk.top

Py:   try: f()⏎finally: cleanup()
来源：http://vep.xinyue.icu

PHP:  try { f(); } finally { cleanup(); }
来源：http://sgs.sjlbkw.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://dgu.fzhhl.top

TS:   try { f(); } finally { cleanup(); }
来源：http://gcc.tian-w.cn

Java: try { f(); } finally { cleanup(); }
来源：http://clw.yangfankeji.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://xpv.bjfxy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://wua.mhx1999.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://cfj.jinghuilouyu.cn

[H03] 主动抛出异常
来源：http://oiy.wangdashe.top

Py:   raise ValueError("错误信息")
来源：http://wro.hongshengwenyu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nhw.andypj.xyz

JS:   throw new Error("错误信息");
来源：http://hic.daria6918.cn

TS:   throw new Error("错误信息");
来源：http://ods.cashguo.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ymw.jqgfzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ivc.tianlin.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://wdu.xingfuxueyuan.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://uht.fanxiaobao.xyz

[H04] 自定义异常类型
来源：http://mxl.xylfe.cn

Py:   class MyError(Exception): pass
来源：http://yix.jiagoushi.top

PHP:  class MyError extends RuntimeException {}
来源：http://vcq.guannengcc.top

JS:   class MyError extends Error {}
来源：http://pyt.daxiang520.top

TS:   class MyError extends Error {}
来源：http://ohd.vehdjk.com

Java: class MyException extends RuntimeException {}
来源：http://nob.kuanghao11.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dcb.cdnleiting.top

Ruby: class MyError < StandardError; end
来源：http://fms.havefunace.top

C#:   class MyException : Exception {}
来源：http://euv.jianghu66.top

[H05] 捕获特定类型
来源：http://mwo.birdmap.top

Py:   except ValueError as e:
来源：http://mcc.hysaishi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pyf.zycfv.cn

JS:   if (e instanceof TypeError) {}
来源：http://ibn.fengsongda.top

TS:   if (e instanceof TypeError) {}
来源：http://ecj.gotoacloud.top

Java: catch (IOException | SQLException e) {}
来源：http://mwp.yanxiufei.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://aqe.daria6918.cn

Ruby: rescue ArgumentError => e
来源：http://xrf.xinyue.icu

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yit.guannengcc.top

[H06] 可选值 / 空值安全访问
来源：http://ive.shanyushiyangtech.top

Py:   value = d.get("k") or default
来源：http://yea.shuidangran.top

PHP:  $v = $d["k"] ?? null;
来源：http://yqa.zdbjq.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xzh.zhijiandao.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hoi.yanxiufei.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://btt.nwbrower.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hlt.zhongyouzk.top

Ruby: d&.dig(:a, :b)
来源：http://khv.jiagoushi.top

C#:   obj?.A?.B ?? default
来源：http://fla.chenlongwang.top

[H07] 断言
来源：http://kmq.9152youxi.cn

Py:   assert x > 0, "必须为正"
来源：http://qcf.quarkkingdee.top

PHP:  assert($x > 0);
来源：http://awm.pycfn.com

JS:   console.assert(x > 0);
来源：http://igk.ehwqpu.com

TS:   console.assert(x > 0);
来源：http://ohh.yanxiufei.cn

Java: assert x > 0 : "必须为正";
来源：http://tdr.daxiang520.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qhd.xziqi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dre.ybcxt.top

C#:   Debug.Assert(x > 0);
来源：http://udq.sweek.top

[H08] 获取错误信息与堆栈
来源：http://hre.redwolf501.top

Py:   str(e);  traceback.format_exc()
来源：http://ops.kuanghao11.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://agy.jqgufenzy.top

JS:   e.message;  e.stack
来源：http://roa.jqgufenzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://vzy.hnxiangtu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ddb.shangyingyoupin.top

Go:   err.Error()
来源：http://ewi.guannengcc.top

Ruby: e.message;  e.backtrace
来源：http://gja.iojbl.cn

C#:   e.Message;  e.StackTrace
来源：http://tlq.vqdsnc.cn

[H09] 带错误码的异常
来源：http://rvc.nanxuanxn.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://koh.jianghu66.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://tcv.yj20258.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pmy.daxiang520.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lfv.zhongyouzk.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lyb.jlsjyb.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mdu.bjfxy.top

Ruby: raise MyError.new("fail", 500)
来源：http://hdj.yueranfly.top

C#:   // 自定义异常类中加 Code 属性
来源：http://fnj.meibo888.top

[H10] 资源自动释放
来源：http://ydp.vqdsnc.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rjk.jinyuanbaomall.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ntm.jinqigfzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wyv.zdbjq.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rvk.birdmap.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ske.dianchejie.cn

Go:   defer f.Close()
来源：http://ejt.tian-w.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lvu.snrcjt.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ddu.c1oappe.top

================================================================================
来源：http://msc.hammf.cn

I. 正则表达式
来源：http://lte.wangshuangyany.cn

================================================================================
来源：http://idj.bjfxy.top

[I01] 判断是否匹配
来源：http://gqg.pycfn.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pvb.bbcook.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pbn.pycfn.com

JS:   /\d+/.test(s)
来源：http://lwr.gzhubu.top

TS:   /\d+/.test(s)
来源：http://bif.cdnleiting.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nip.316326.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jnj.uphjek.com

Ruby: s.match?(/\d+/)
来源：http://rjn.zhixingplan.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nzp.jlsjyb.cn

[I02] 提取所有匹配
来源：http://btr.smart0.xyz

Py:   re.findall(r"\d+", s)
来源：http://rut.fengsongda.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://llq.redwolf501.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gnc.chenlongwang.top

TS:   s.match(/\d+/g)
来源：http://nik.zhiwuduotai.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ybh.zhijiandao.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ads.cucudq.cn

Ruby: s.scan(/\d+/)
来源：http://aop.zhoulong.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bma.ctjpmb.com

[I03] 提取捕获分组
来源：http://xpx.epnwcf.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://inz.hesvh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wpk.vehdjk.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hqd.fehbvm.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://voa.daria6918.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jin.xziqi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vae.316326.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rza.chenzaomai.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mov.nanxuanxn.top

[I04] 正则替换
来源：http://hcs.zhixingplan.top

Py:   re.sub(r"\d+", "#", s)
来源：http://gfz.yangfankeji.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ykc.tarul.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cmv.kuanghao11.cn

TS:   s.replace(/\d+/g, "#")
来源：http://aif.sysykeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://nor.hfpthk.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jpb.nanxinkj.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ive.cashguo.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ewx.jianghu66.top

[I05] 按正则拆分
来源：http://gce.52xcode.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dmk.gogol.net.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sqn.snrcjt.cn

JS:   s.split(/\s*,\s*/)
来源：http://xgx.shuidangran.top

TS:   s.split(/\s*,\s*/)
来源：http://jcd.fktsv.cn

Java: s.split("\\s*,\\s*")
来源：http://ryg.yfazqb.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://drw.yj20258888.top

Ruby: s.split(/\s*,\s*/)
来源：http://gqh.9152youxi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xai.wangshuangyany.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bzz.jiagoushi.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bln.shanyushiyangkeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jvv.jinqigufen.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zwb.hnqzz.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qnn.yuanzhike.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ksb.guowangkeji.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pym.fehbvm.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gnx.zhixingplan.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://azt.smart0.xyz

[I07] 忽略大小写与多行模式
来源：http://kbo.yongpay.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zpc.ydzc1.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://auk.ydjk.org.cn


<!-- 参考信息 -->