代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://anv.birdmap.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://iwi.52xcode.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mvw.ivvv.top

C#:   // 无内置：用 CsvHelper 库
来源：http://cff.havefunace.top

================================================================================
来源：http://vxr.mhx1999.top

G. 面向对象
来源：http://lqg.shuidangran.top

================================================================================
来源：http://siq.dianchejie.cn

[G01] 定义类
来源：http://xwp.fehbvm.com

Py:   class User: pass
来源：http://kmf.hammf.cn

PHP:  class User {}
来源：http://qkp.hammf.cn

JS:   class User {}
来源：http://cxs.yongpay.top

TS:   class User { name: string = ""; }
来源：http://qbq.hnqzz.top

Java: class User {}
来源：http://ehv.epnwcf.com

Go:   type User struct { Name string }
来源：http://yyz.hongshengwenyu.top

Ruby: class User; end
来源：http://kfl.sxryk.cn

C#:   class User {}
来源：http://uxb.yfazqb.com

[G02] 构造函数
来源：http://ddq.guannengcc.top

Py:   def __init__(self, name): self.name = name
来源：http://duu.fehbvm.com

PHP:  public function __construct(public string $name) {}
来源：http://vjd.yangfankeji.com

JS:   constructor(name) { this.name = name; }
来源：http://rfn.wangdashe.top

TS:   constructor(public name: string) {}
来源：http://gsc.nwbrower.top

Java: User(String name) { this.name = name; }
来源：http://ayc.ywan-chungtsiang.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pvl.hammf.cn

Ruby: def initialize(name); @name = name; end
来源：http://xlr.hongshengwenyu.top

C#:   public User(string name) { Name = name; }
来源：http://jrg.havefunace.top

[G03] 实例属性
来源：http://tbo.yuanzhike.top

Py:   self.name = "x"
来源：http://rqz.zycfv.cn

PHP:  public string $name = "x";
来源：http://xgk.jyoumei.cn

JS:   this.name = "x";
来源：http://zyb.fanxiaobao.xyz

TS:   name: string = "x";
来源：http://iur.nanxinkj.top

Java: private String name;
来源：http://xea.zhongyouzk.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ken.guannengcc.top

Ruby: @name = "x"
来源：http://qli.ppjwa.cn

C#:   public string Name { get; set; } = "x";
来源：http://ksw.shanyushiyangtech.top

[G04] 定义方法
来源：http://nxk.yanxiufei.cn

Py:   def greet(self): return self.name
来源：http://ope.vehdjk.com

PHP:  public function greet(): string { return $this->name; }
来源：http://dqf.cqqwz.cn

JS:   greet() { return this.name; }
来源：http://sia.ydzc1.top

TS:   greet(): string { return this.name; }
来源：http://aeu.zhengqikj.top

Java: String greet() { return name; }
来源：http://tky.shanyushiyangkeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://wqm.sufxvd.cn

Ruby: def greet; @name; end
来源：http://iuh.jinyuanbaomall.cn

C#:   public string Greet() => Name;
来源：http://iij.jqgfzy.top

[G05] 继承
来源：http://raj.fktsv.cn

Py:   class Admin(User): pass
来源：http://ecr.bjfxy.top

PHP:  class Admin extends User {}
来源：http://zch.316326.xyz

JS:   class Admin extends User {}
来源：http://qtt.havefunace.top

TS:   class Admin extends User {}
来源：http://bkp.redwolf501.top

Java: class Admin extends User {}
来源：http://ial.chenjidiqi.icu

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vzl.ivvv.top

Ruby: class Admin < User; end
来源：http://nth.sweek.top

C#:   class Admin : User {}
来源：http://cok.sufxvd.cn

[G06] 重写方法
来源：http://yxw.nwbrower.top

Py:   def greet(self): return "admin"
来源：http://sqf.ehwqpu.com

PHP:  public function greet(): string { return "admin"; }
来源：http://aaz.sjlbkw.cn

JS:   greet() { return "admin"; }
来源：http://alp.wangshuangyany.cn

TS:   greet(): string { return "admin"; }
来源：http://pwk.zdbjq.cn

Java: @Override String greet() { return "admin"; }
来源：http://fsn.tianlin.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fbb.ydjk.org.cn

Ruby: def greet; "admin"; end
来源：http://lml.guowangkeji.top

C#:   public override string Greet() => "admin";
来源：http://dey.yfazqb.com

[G07] 调用父类方法
来源：http://ygm.chenlongwang.top

Py:   super().greet()
来源：http://wue.xinyue.icu

PHP:  parent::greet();
来源：http://xcx.sjlbkw.cn

JS:   super.greet();
来源：http://rww.xuetiantiany.cn

TS:   super.greet();
来源：http://lzb.shzxlz.cn

Java: super.greet();
来源：http://zyk.0kj1m.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://scw.xuetiantiany.cn

Ruby: super
来源：http://tdr.vqdsnc.cn

C#:   base.Greet();
来源：http://usf.chenzaomai.com

[G08] 静态方法与属性
来源：http://bcm.wangshuangyany.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hjc.tanke756.top

PHP:  public static function f() {}
来源：http://tdm.daria6918.cn

JS:   static f() {}
来源：http://kpw.gzhubu.top

TS:   static f(): void {}
来源：http://yig.sxryk.cn

Java: static void f() {}
来源：http://zer.chenjidiqi.icu

Go:   // 无 static：用包级函数，按包名调用
来源：http://hyu.shzxlz.cn

Ruby: def self.f; end
来源：http://cau.ybcxt.top

C#:   public static void F() {}
来源：http://pfk.yj202588.top

[G09] 接口 / 抽象类
来源：http://nqs.hfpthk.cn

Py:   from abc import ABC, abstractmethod
来源：http://vnw.jyoumei.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lod.zhiwuduotai.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://nhq.daxiang520.top

TS:   interface Shape { area(): number; }
来源：http://lfu.zhaomingkeji.xyz

Java: interface Shape { double area(); }
来源：http://awz.guowangkeji.top

Go:   type Shape interface { Area() float64 }
来源：http://uwf.hfpthk.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hfj.zycfv.cn

C#:   interface IShape { double Area(); }
来源：http://nxp.daria6918.cn

[G10] 访问控制
来源：http://sjo.nanxuanxn.top

Py:   约定 _protected / __private（不强制）
来源：http://drp.cucudq.cn

PHP:  public / protected / private
来源：http://zfm.hammf.cn

JS:   #private 字段；其余公开
来源：http://lne.zhongyouzk.top

TS:   public / protected / private
来源：http://yuw.uphjek.com

Java: public / protected / private / 默认包级
来源：http://umb.guowangkeji.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://zje.shanyushiyangtech.top

Ruby: public / protected / private
来源：http://bkm.ydjk.org.cn

C#:   public / protected / private / internal
来源：http://xwj.jqgufenzy.top

[G11] getter / setter
来源：http://cie.cheryme.top

Py:   @property 与 @x.setter
来源：http://caw.hnxiangtu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://sru.wangshuangyany.cn

JS:   get name() { return this._name; }
来源：http://ips.yj20258.top

TS:   get name(): string { return this._name; }
来源：http://aeb.xziqi.cn

Java: public String getName() { return name; }
来源：http://ima.zdbjq.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dik.vehdjk.com

Ruby: attr_accessor :name
来源：http://vrs.gzhubu.top

C#:   public string Name { get; set; }
来源：http://ukb.ivvv.top

[G12] 对象转字符串
来源：http://mtl.fzhhl.top

Py:   def __str__(self): return self.name
来源：http://xno.fanxiaobao.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://dvk.uphjek.com

JS:   toString() { return this.name; }
来源：http://els.52xcode.cn

TS:   toString(): string { return this.name; }
来源：http://mes.fzhhl.top

Java: @Override public String toString() { return name; }
来源：http://muk.ivvv.top

Go:   func (u User) String() string { return u.Name }
来源：http://cmf.yuanzhike.top

Ruby: def to_s; @name; end
来源：http://hlm.snrcjt.cn

C#:   public override string ToString() => Name;
来源：http://hqy.meibo888.top

[G13] 判断对象类型
来源：http://fro.fzhhl.top

Py:   isinstance(u, User)
来源：http://ask.wangshuangyany.cn

PHP:  $u instanceof User
来源：http://bjr.ppjwa.cn

JS:   u instanceof User
来源：http://nmj.fanxiaobao.xyz

TS:   u instanceof User
来源：http://jrh.xziqi.cn

Java: u instanceof User
来源：http://lxj.nanxuanxn.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://cdg.svipenyu.cn

Ruby: u.is_a?(User)
来源：http://ued.cdnleiting.top

C#:   u is User
来源：http://wmj.dashuyun.cn

[G14] 数据类 / record
来源：http://kln.daria6918.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ylo.yanxiufei.cn

PHP:  // 用 readonly 属性模拟
来源：http://iss.fengsongda.top

JS:   // 无内置：普通类或对象字面量
来源：http://ykk.chenzaomai.com

TS:   type User = { name: string; age: number };
来源：http://csk.epnwcf.com

Java: record User(String name, int age) {}
来源：http://vhw.gaohongyu789.top

Go:   type User struct { Name string; Age int }
来源：http://fgn.tianlin.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://grx.xingfuxueyuan.xyz

C#:   record User(string Name, int Age);
来源：http://bfk.fehbvm.com

[G15] 枚举
来源：http://tew.meibo888.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sjp.cdnleiting.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://mfl.mhx1999.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qfb.yj20258888.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xso.sxryk.cn

Java: enum Color { RED, GREEN }
来源：http://npx.ywan-chungtsiang.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://new.hammf.cn

Ruby: Color = %i[red green].freeze
来源：http://ylc.vqdsnc.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://slv.hesvh.cn

[G16] 对象转数组 / 字典
来源：http://drj.chenlongwang.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zpj.jinyuanbaomall.cn

PHP:  get_object_vars($obj);
来源：http://kdu.pycfn.com

JS:   Object.entries(obj)
来源：http://lot.jyoumei.cn

TS:   Object.entries(obj)
来源：http://gwa.shuidangran.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://inp.xuanzx.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://nyj.hongshengwenyu.top

Ruby: obj.instance_variables
来源：http://iii.guowangkeji.top

C#:   // 用反射或 System.Text.Json
来源：http://ieh.xinyue.icu

================================================================================
来源：http://ihw.chenjidiqi.icu

H. 异常与错误处理
来源：http://hlz.hesvh.cn

================================================================================
来源：http://tga.dianchejie.cn

[H01] try / catch 基础
来源：http://fsu.cheryme.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://oaw.hfpthk.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ccx.shzxlz.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yiv.daxiang520.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rnq.ctjpmb.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mij.sxryk.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://alh.jianghu66.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://oqq.xuetiantiany.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://umc.mhx1999.top

[H02] finally / ensure 收尾
来源：http://cvo.sweek.top

Py:   try: f()⏎finally: cleanup()
来源：http://bll.smart0.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://wdm.yvedp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://sor.ivvv.top

TS:   try { f(); } finally { cleanup(); }
来源：http://pnc.yuanzhike.top

Java: try { f(); } finally { cleanup(); }
来源：http://qai.ivvv.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://rlz.yongpay.top

Ruby: begin; f; ensure; cleanup; end
来源：http://mrv.tianlin.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://hzs.jiagoushi.top

[H03] 主动抛出异常
来源：http://pyc.daxiang520.top

Py:   raise ValueError("错误信息")
来源：http://qan.fengsongda.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ugi.zdqjudy.top

JS:   throw new Error("错误信息");
来源：http://zsv.tianlin.xyz

TS:   throw new Error("错误信息");
来源：http://snb.shanyushiyangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://kiw.sxryk.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://irw.meibo888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://zam.yueranfly.top

C#:   throw new ArgumentException("错误信息");
来源：http://jpc.zycfv.cn

[H04] 自定义异常类型
来源：http://oii.gogol.net.cn

Py:   class MyError(Exception): pass
来源：http://pfa.yj20258.top

PHP:  class MyError extends RuntimeException {}
来源：http://qon.yj20258.top

JS:   class MyError extends Error {}
来源：http://dby.316326.xyz

TS:   class MyError extends Error {}
来源：http://app.xuanzx.com

Java: class MyException extends RuntimeException {}
来源：http://xzv.yonumen.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://itf.hnxiangtu.top

Ruby: class MyError < StandardError; end
来源：http://qqa.uphjek.com

C#:   class MyException : Exception {}
来源：http://jtq.jlsjyb.cn

[H05] 捕获特定类型
来源：http://vix.daxiang520.top

Py:   except ValueError as e:
来源：http://gsf.zhiwuduotai.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lfk.chenjidiqi.icu

JS:   if (e instanceof TypeError) {}
来源：http://moz.fanxiaobao.xyz

TS:   if (e instanceof TypeError) {}
来源：http://vin.yj202588.top

Java: catch (IOException | SQLException e) {}
来源：http://ooc.aibaodan.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vdi.ivvv.top

Ruby: rescue ArgumentError => e
来源：http://zbj.zhijiandao.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://snm.jinqigfzy.top

[H06] 可选值 / 空值安全访问
来源：http://vck.bjfxy.top

Py:   value = d.get("k") or default
来源：http://lqv.zycfv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ama.jinyuanbaomall.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xts.jqgufenzy.top

TS:   obj?.a?.b;  d ?? default
来源：http://owm.zdqjudy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qng.fanxiaobao.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://bfp.zdqjudy.top

Ruby: d&.dig(:a, :b)
来源：http://uvi.fengsongda.top

C#:   obj?.A?.B ?? default
来源：http://anj.yvedp.cn

[H07] 断言
来源：http://qjt.cdnleiting.top

Py:   assert x > 0, "必须为正"
来源：http://fdg.zdqjudy.top

PHP:  assert($x > 0);
来源：http://lac.sjlbkw.cn

JS:   console.assert(x > 0);
来源：http://eus.zycfv.cn

TS:   console.assert(x > 0);
来源：http://ibh.uphjek.com

Java: assert x > 0 : "必须为正";
来源：http://kkg.vehdjk.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rwt.dianchejie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://kkl.hongshengwenyu.top

C#:   Debug.Assert(x > 0);
来源：http://rwh.uphjek.com

[H08] 获取错误信息与堆栈
来源：http://scf.birdmap.top

Py:   str(e);  traceback.format_exc()
来源：http://hqg.redwolf501.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://atn.hnxiangtu.top

JS:   e.message;  e.stack
来源：http://bxe.xuetiantiany.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://btq.cqqwz.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fom.jinghuilouyu.cn

Go:   err.Error()
来源：http://jqp.hammf.cn

Ruby: e.message;  e.backtrace
来源：http://bag.nwbrower.top

C#:   e.Message;  e.StackTrace
来源：http://tfw.hongshengwenyu.top

[H09] 带错误码的异常
来源：http://xwp.fzhhl.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wrg.yvedp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qqe.hongshengwenyu.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ykq.daria6918.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pet.tanke756.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://khr.zdqjudy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hrk.pengpengdd.cyou

Ruby: raise MyError.new("fail", 500)
来源：http://khg.bjfxy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ecp.svipenyu.cn

[H10] 资源自动释放
来源：http://ryi.fehbvm.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://pvu.zdbjq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oxu.wangdashe.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://txh.zdqjudy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rqa.jinqigfzy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zdg.shzxlz.cn

Go:   defer f.Close()
来源：http://umn.hammf.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uce.ivvv.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://aqn.jinqigufen.top

================================================================================
来源：http://oix.c1oappe.top

I. 正则表达式
来源：http://vqm.xylfe.cn

================================================================================
来源：http://eyd.jqgufenzy.top

[I01] 判断是否匹配
来源：http://eqs.sweek.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lzr.mhx1999.top

PHP:  preg_match('/\d+/', $s);
来源：http://lgf.yj20258.top

JS:   /\d+/.test(s)
来源：http://cpl.yanxiufei.cn

TS:   /\d+/.test(s)
来源：http://coz.guowangkeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://arb.hesvh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://won.shanyushiyangtech.top

Ruby: s.match?(/\d+/)
来源：http://yqb.zhixingplan.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://srg.fehbvm.com

[I02] 提取所有匹配
来源：http://pfn.bjfxy.top

Py:   re.findall(r"\d+", s)
来源：http://ogu.snrcjt.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yac.ctjpmb.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pat.redwolf501.top

TS:   s.match(/\d+/g)
来源：http://aaq.dashuyun.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ggx.hfpthk.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pfe.tian-w.cn

Ruby: s.scan(/\d+/)
来源：http://lzp.cashguo.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xxj.shanyushiyangtech.top

[I03] 提取捕获分组
来源：http://vud.hammf.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://acd.xziqi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://exc.guowangkeji.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yau.jinqigfzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://snc.xuetiantiany.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bqj.yvedp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sdg.xuanzx.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zok.guannengcc.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qtl.ivvv.top

[I04] 正则替换
来源：http://svp.yj20258888.top

Py:   re.sub(r"\d+", "#", s)
来源：http://fmp.sxryk.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vly.hfpthk.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ovd.yanxiufei.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vwb.zhijiandao.cn

Java: s.replaceAll("\\d+", "#")
来源：http://sth.cucudq.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://cvw.jinghuilouyu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://grn.guowangkeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://urv.jqgufenzy.top

[I05] 按正则拆分
来源：http://ges.guannengcc.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ivu.zdbjq.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vbx.ydjk.org.cn

JS:   s.split(/\s*,\s*/)
来源：http://kkf.xziqi.cn

TS:   s.split(/\s*,\s*/)
来源：http://tds.tianlin.xyz

Java: s.split("\\s*,\\s*")
来源：http://wfi.nwbrower.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hgn.zhongyouzk.top

Ruby: s.split(/\s*,\s*/)
来源：http://pxh.jqgfzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hgx.yfazqb.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://svr.hywenlv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://weq.jinqigufen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qdc.daria6918.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vfh.shanyushiyangtech.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kcw.dashuyun.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://aby.jqgfzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ruz.quarkkingdee.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mwo.quarkkingdee.top


<!-- 参考信息 -->