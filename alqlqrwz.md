代发 wailian999

================================================================================
来源：http://gyc.zhengqikj.top

G. 面向对象
来源：http://nce.haohaochexian.top

================================================================================
来源：http://zyf.xuanzx.com

[G01] 定义类
来源：http://chw.hcnkem.com

Py:   class User: pass
来源：http://hek.zdqjudy.top

PHP:  class User {}
来源：http://lpz.yj202588.top

JS:   class User {}
来源：http://scq.cqqwz.cn

TS:   class User { name: string = ""; }
来源：http://lob.xziqi.cn

Java: class User {}
来源：http://ggd.jinqigufen.top

Go:   type User struct { Name string }
来源：http://tcx.xuetiantiany.cn

Ruby: class User; end
来源：http://wgd.smart0.xyz

C#:   class User {}
来源：http://vuc.havefunace.top

[G02] 构造函数
来源：http://oul.fengsongda.top

Py:   def __init__(self, name): self.name = name
来源：http://sza.haohaochexian.top

PHP:  public function __construct(public string $name) {}
来源：http://vrs.cheryme.top

JS:   constructor(name) { this.name = name; }
来源：http://jzp.cqqwz.cn

TS:   constructor(public name: string) {}
来源：http://ehc.ydzc1.top

Java: User(String name) { this.name = name; }
来源：http://ety.zdqjudy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lvt.hfpthk.cn

Ruby: def initialize(name); @name = name; end
来源：http://xuz.hammf.cn

C#:   public User(string name) { Name = name; }
来源：http://pcf.jqgufenzy.top

[G03] 实例属性
来源：http://gsv.c1oappe.top

Py:   self.name = "x"
来源：http://xpc.yuxming.cn

PHP:  public string $name = "x";
来源：http://vss.guowangkeji.top

JS:   this.name = "x";
来源：http://zop.daria6918.cn

TS:   name: string = "x";
来源：http://gjg.snrcjt.cn

Java: private String name;
来源：http://dbh.ehwqpu.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://irx.kuanghao11.cn

Ruby: @name = "x"
来源：http://rzp.bjfxy.top

C#:   public string Name { get; set; } = "x";
来源：http://mvp.hywenlv.cn

[G04] 定义方法
来源：http://fpc.hammf.cn

Py:   def greet(self): return self.name
来源：http://igk.xinyue.icu

PHP:  public function greet(): string { return $this->name; }
来源：http://blp.ivvv.top

JS:   greet() { return this.name; }
来源：http://mqe.yfazqb.com

TS:   greet(): string { return this.name; }
来源：http://imp.52xcode.cn

Java: String greet() { return name; }
来源：http://oll.yj20258.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://slo.xingfuxueyuan.xyz

Ruby: def greet; @name; end
来源：http://wrr.xziqi.cn

C#:   public string Greet() => Name;
来源：http://jho.dianchejie.cn

[G05] 继承
来源：http://ayc.shanyushiyangtech.top

Py:   class Admin(User): pass
来源：http://pnd.guannengcc.top

PHP:  class Admin extends User {}
来源：http://uqt.snrcjt.cn

JS:   class Admin extends User {}
来源：http://vyl.feifeiyinyue.top

TS:   class Admin extends User {}
来源：http://wpp.hammf.cn

Java: class Admin extends User {}
来源：http://sgs.ybcxt.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jgw.zdqjudy.top

Ruby: class Admin < User; end
来源：http://xvc.tian-w.cn

C#:   class Admin : User {}
来源：http://gcb.andypj.xyz

[G06] 重写方法
来源：http://mvx.yj202588.top

Py:   def greet(self): return "admin"
来源：http://jjd.cucudq.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ikj.hywenlv.cn

JS:   greet() { return "admin"; }
来源：http://vcx.ywan-chungtsiang.top

TS:   greet(): string { return "admin"; }
来源：http://zzq.c1oappe.top

Java: @Override String greet() { return "admin"; }
来源：http://qjs.jinqigfzy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ujd.redwolf501.top

Ruby: def greet; "admin"; end
来源：http://tyb.hcnkem.com

C#:   public override string Greet() => "admin";
来源：http://lmn.pycfn.com

[G07] 调用父类方法
来源：http://ieb.zhaomingkeji.xyz

Py:   super().greet()
来源：http://xgf.tianlin.xyz

PHP:  parent::greet();
来源：http://bcs.52xcode.cn

JS:   super.greet();
来源：http://xua.hongshengwenyu.top

TS:   super.greet();
来源：http://wbp.tanke756.top

Java: super.greet();
来源：http://ovg.jiagoushi.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bzn.gzhubu.top

Ruby: super
来源：http://gqo.hesvh.cn

C#:   base.Greet();
来源：http://cjw.xziqi.cn

[G08] 静态方法与属性
来源：http://hsu.sjlbkw.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jfr.yj202588.top

PHP:  public static function f() {}
来源：http://dzx.jinqigfzy.top

JS:   static f() {}
来源：http://sqh.nanxuanxn.top

TS:   static f(): void {}
来源：http://ccg.tian-w.cn

Java: static void f() {}
来源：http://dvh.fanxiaobao.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://iql.yongpay.top

Ruby: def self.f; end
来源：http://bxn.zhiwuduotai.top

C#:   public static void F() {}
来源：http://jik.yvedp.cn

[G09] 接口 / 抽象类
来源：http://vlk.haohaochexian.top

Py:   from abc import ABC, abstractmethod
来源：http://sqm.vqdsnc.cn

PHP:  interface Shape { public function area(): float; }
来源：http://uqs.sweek.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://hfq.shanyushiyangkeji.top

TS:   interface Shape { area(): number; }
来源：http://ttd.yonumen.top

Java: interface Shape { double area(); }
来源：http://uhn.ybcxt.top

Go:   type Shape interface { Area() float64 }
来源：http://hls.chenzaomai.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dmt.xziqi.cn

C#:   interface IShape { double Area(); }
来源：http://gsu.sjlbkw.cn

[G10] 访问控制
来源：http://bcr.snrcjt.cn

Py:   约定 _protected / __private（不强制）
来源：http://uvs.guannengcc.top

PHP:  public / protected / private
来源：http://eeu.zdbjq.cn

JS:   #private 字段；其余公开
来源：http://onh.xuetiantiany.cn

TS:   public / protected / private
来源：http://wpq.nanxuanxn.top

Java: public / protected / private / 默认包级
来源：http://nps.hnxiangtu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://fec.xingfuxueyuan.xyz

Ruby: public / protected / private
来源：http://xbe.zhijiandao.cn

C#:   public / protected / private / internal
来源：http://xri.havefunace.top

[G11] getter / setter
来源：http://mbu.zhijiandao.cn

Py:   @property 与 @x.setter
来源：http://fps.ctjpmb.com

PHP:  public function getName(): string { return $this->name; }
来源：http://ckx.meibo888.top

JS:   get name() { return this._name; }
来源：http://yca.iojbl.cn

TS:   get name(): string { return this._name; }
来源：http://pfl.hywenlv.cn

Java: public String getName() { return name; }
来源：http://mnz.haohaochexian.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://jeh.hfpthk.cn

Ruby: attr_accessor :name
来源：http://frh.daria6918.cn

C#:   public string Name { get; set; }
来源：http://obe.ybcxt.top

[G12] 对象转字符串
来源：http://zdw.vehdjk.com

Py:   def __str__(self): return self.name
来源：http://nyv.shuidangran.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://qru.ctjpmb.com

JS:   toString() { return this.name; }
来源：http://wix.fzhhl.top

TS:   toString(): string { return this.name; }
来源：http://bry.xuanzx.com

Java: @Override public String toString() { return name; }
来源：http://izb.tarul.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vyd.yj20258888.top

Ruby: def to_s; @name; end
来源：http://cwl.dianchejie.cn

C#:   public override string ToString() => Name;
来源：http://jbo.sjlbkw.cn

[G13] 判断对象类型
来源：http://vqj.yueranfly.top

Py:   isinstance(u, User)
来源：http://azf.cashguo.top

PHP:  $u instanceof User
来源：http://rfu.daxiang520.top

JS:   u instanceof User
来源：http://qnh.jianghu66.top

TS:   u instanceof User
来源：http://nmh.xinyue.icu

Java: u instanceof User
来源：http://eav.pengpengdd.cyou

Go:   u, ok := v.(User)            // 类型断言
来源：http://xfa.jinqigfzy.top

Ruby: u.is_a?(User)
来源：http://xgp.ivvv.top

C#:   u is User
来源：http://unz.jqgufenzy.top

[G14] 数据类 / record
来源：http://mki.snrcjt.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rng.bjfxy.top

PHP:  // 用 readonly 属性模拟
来源：http://yaq.birdmap.top

JS:   // 无内置：普通类或对象字面量
来源：http://yye.xuetiantiany.cn

TS:   type User = { name: string; age: number };
来源：http://auy.hfpthk.cn

Java: record User(String name, int age) {}
来源：http://ozu.ivvv.top

Go:   type User struct { Name string; Age int }
来源：http://udl.zdqjudy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://moj.ivvv.top

C#:   record User(string Name, int Age);
来源：http://xea.quarkkingdee.top

[G15] 枚举
来源：http://ynt.yonumen.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kdz.ywan-chungtsiang.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://zun.gotoacloud.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gkk.cheryme.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hki.yanxiufei.cn

Java: enum Color { RED, GREEN }
来源：http://nxe.ehwqpu.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ljs.shzxlz.cn

Ruby: Color = %i[red green].freeze
来源：http://abx.cucudq.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pbo.yj20258.top

[G16] 对象转数组 / 字典
来源：http://ywj.yanxiufei.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nyt.epnwcf.com

PHP:  get_object_vars($obj);
来源：http://jwg.52xcode.cn

JS:   Object.entries(obj)
来源：http://tid.fzhhl.top

TS:   Object.entries(obj)
来源：http://bxh.316326.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nzh.hesvh.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://akx.hongshengwenyu.top

Ruby: obj.instance_variables
来源：http://vqc.bbcook.cn

C#:   // 用反射或 System.Text.Json
来源：http://ffw.haohaochexian.top

================================================================================
来源：http://tmu.yj20258.top

H. 异常与错误处理
来源：http://zal.meibo888.top

================================================================================
来源：http://fck.zdbjq.cn

[H01] try / catch 基础
来源：http://oiw.nanxinkj.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yqm.hfpthk.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gti.xuanzx.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qwp.jqgufenzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gtz.ywan-chungtsiang.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://flw.guannengcc.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mrz.ydzc1.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://szt.tianlin.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lbx.ehwqpu.com

[H02] finally / ensure 收尾
来源：http://ppp.ppjwa.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gdv.yangfankeji.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://jce.gzhubu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://saz.redwolf501.top

TS:   try { f(); } finally { cleanup(); }
来源：http://div.smart0.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://mgu.fanxiaobao.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://xym.shangyingyoupin.top

Ruby: begin; f; ensure; cleanup; end
来源：http://lln.aizwys.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://idu.uphjek.com

[H03] 主动抛出异常
来源：http://mly.uphjek.com

Py:   raise ValueError("错误信息")
来源：http://add.hnxiangtu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lua.c1oappe.top

JS:   throw new Error("错误信息");
来源：http://yaz.xziqi.cn

TS:   throw new Error("错误信息");
来源：http://qwf.ivvv.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://npo.shzxlz.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ozi.fehbvm.com

Ruby: raise ArgumentError, "错误信息"
来源：http://whz.ybcxt.top

C#:   throw new ArgumentException("错误信息");
来源：http://szq.xuetiantiany.cn

[H04] 自定义异常类型
来源：http://get.nanxuanxn.top

Py:   class MyError(Exception): pass
来源：http://ydo.fanxiaobao.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://ndo.yj202588.top

JS:   class MyError extends Error {}
来源：http://ohs.bjfxy.top

TS:   class MyError extends Error {}
来源：http://xkm.yfazqb.com

Java: class MyException extends RuntimeException {}
来源：http://yts.cucudq.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://igt.yj202588.top

Ruby: class MyError < StandardError; end
来源：http://kdn.daxiang520.top

C#:   class MyException : Exception {}
来源：http://tcw.havefunace.top

[H05] 捕获特定类型
来源：http://ebq.quarkkingdee.top

Py:   except ValueError as e:
来源：http://ape.zycfv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ktz.jinghuilouyu.cn

JS:   if (e instanceof TypeError) {}
来源：http://ktw.sxryk.cn

TS:   if (e instanceof TypeError) {}
来源：http://qub.ywan-chungtsiang.top

Java: catch (IOException | SQLException e) {}
来源：http://yqh.aizwys.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dwl.shzxlz.cn

Ruby: rescue ArgumentError => e
来源：http://hpx.sysykeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rym.haohaochexian.top

[H06] 可选值 / 空值安全访问
来源：http://mna.jlsjyb.cn

Py:   value = d.get("k") or default
来源：http://ppc.zhixingplan.top

PHP:  $v = $d["k"] ?? null;
来源：http://lrx.snrcjt.cn

JS:   obj?.a?.b;  d ?? default
来源：http://muj.yvedp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://gaz.meibo888.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ate.jinqigfzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://dpu.birdmap.top

Ruby: d&.dig(:a, :b)
来源：http://yyc.bbcook.cn

C#:   obj?.A?.B ?? default
来源：http://muu.quarkkingdee.top

[H07] 断言
来源：http://nur.hnxiangtu.top

Py:   assert x > 0, "必须为正"
来源：http://llg.ydzc1.top

PHP:  assert($x > 0);
来源：http://hks.iojbl.cn

JS:   console.assert(x > 0);
来源：http://tnf.sjlbkw.cn

TS:   console.assert(x > 0);
来源：http://vbd.jianghu66.top

Java: assert x > 0 : "必须为正";
来源：http://cam.zhoulong.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yuw.ivvv.top

Ruby: raise "必须为正" unless x > 0
来源：http://zcj.hongshengwenyu.top

C#:   Debug.Assert(x > 0);
来源：http://tjf.hnqzz.top

[H08] 获取错误信息与堆栈
来源：http://wvc.wangshuangyany.cn

Py:   str(e);  traceback.format_exc()
来源：http://fve.haohaochexian.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://iah.hammf.cn

JS:   e.message;  e.stack
来源：http://pgw.birdmap.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://hel.aizwys.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://yuz.52xcode.cn

Go:   err.Error()
来源：http://cxo.iojbl.cn

Ruby: e.message;  e.backtrace
来源：http://nco.xylfe.cn

C#:   e.Message;  e.StackTrace
来源：http://ami.zhijiandao.cn

[H09] 带错误码的异常
来源：http://zea.haohaochexian.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mjh.daxiang520.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://xnp.jyoumei.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vgb.cdnleiting.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lyj.ehwqpu.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://khj.jinqigfzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lsn.wangdashe.top

Ruby: raise MyError.new("fail", 500)
来源：http://iyi.yfazqb.com

C#:   // 自定义异常类中加 Code 属性
来源：http://ups.yueranfly.top

[H10] 资源自动释放
来源：http://awp.cheryme.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://rsg.gogol.net.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ypx.sufxvd.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://meg.cqqwz.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gss.cdnleiting.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jrq.jqgfzy.top

Go:   defer f.Close()
来源：http://pcm.tian-w.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lof.hysaishi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yrj.andypj.xyz

================================================================================
来源：http://qyp.xziqi.cn

I. 正则表达式
来源：http://she.zdbjq.cn

================================================================================
来源：http://new.316326.xyz

[I01] 判断是否匹配
来源：http://bwn.vqdsnc.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tdt.zdqjudy.top

PHP:  preg_match('/\d+/', $s);
来源：http://yvv.sysykeji.top

JS:   /\d+/.test(s)
来源：http://hgo.hammf.cn

TS:   /\d+/.test(s)
来源：http://kwv.zhaomingkeji.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://and.gzhubu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zll.yonumen.top

Ruby: s.match?(/\d+/)
来源：http://ijm.snrcjt.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bvg.ydjk.org.cn

[I02] 提取所有匹配
来源：http://nsq.daxiang520.top

Py:   re.findall(r"\d+", s)
来源：http://bgt.hcnkem.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qwl.bjfxy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wsu.0kj1m.cn

TS:   s.match(/\d+/g)
来源：http://uoy.yangfankeji.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tie.dianchejie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qge.jianghu66.top

Ruby: s.scan(/\d+/)
来源：http://ytt.chenjidiqi.icu

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lwx.haohaochexian.top

[I03] 提取捕获分组
来源：http://jte.pycfn.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ztp.yfazqb.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rxy.bbcook.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qav.zhoulong.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://srm.gzhubu.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://eft.sufxvd.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ldv.hnqzz.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ryg.hesvh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://eff.jqgfzy.top

[I04] 正则替换
来源：http://uiv.sxryk.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://grt.tanke756.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://evv.yonumen.top

JS:   s.replace(/\d+/g, "#")
来源：http://ykc.sxryk.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wbj.jlsjyb.cn

Java: s.replaceAll("\\d+", "#")
来源：http://pfh.jinghuilouyu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://cae.9152youxi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://olp.hnxiangtu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://igz.snrcjt.cn

[I05] 按正则拆分
来源：http://ttn.redwolf501.top

Py:   re.split(r"\s*,\s*", s)
来源：http://qgf.shzxlz.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://anh.nwbrower.top

JS:   s.split(/\s*,\s*/)
来源：http://mdh.fktsv.cn

TS:   s.split(/\s*,\s*/)
来源：http://zrl.smart0.xyz

Java: s.split("\\s*,\\s*")
来源：http://sht.hongshengwenyu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kvj.yangfankeji.com

Ruby: s.split(/\s*,\s*/)
来源：http://zbs.gzhubu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bei.fzhhl.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kbt.52xcode.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fpb.ywan-chungtsiang.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pxb.aibaodan.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jgx.0kj1m.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pyy.hesvh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ftu.ydzc1.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://saf.havefunace.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dlz.haohaochexian.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cso.ehwqpu.com

[I07] 忽略大小写与多行模式
来源：http://uoy.yanxiufei.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dea.vehdjk.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kwk.ctjpmb.com


<!-- 参考信息 -->