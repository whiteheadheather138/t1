代发 wailian999

Java: class User {}
来源：http://hau.shuidangran.top

Go:   type User struct { Name string }
来源：http://ejj.quarkkingdee.top

Ruby: class User; end
来源：http://qyh.yanxiufei.cn

C#:   class User {}
来源：http://pax.ivvv.top

[G02] 构造函数
来源：http://rqv.yangfankeji.com

Py:   def __init__(self, name): self.name = name
来源：http://yfd.dianchejie.cn

PHP:  public function __construct(public string $name) {}
来源：http://beu.yj202588.top

JS:   constructor(name) { this.name = name; }
来源：http://msv.fktsv.cn

TS:   constructor(public name: string) {}
来源：http://npk.birdmap.top

Java: User(String name) { this.name = name; }
来源：http://feb.gaohongyu789.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lqb.xylfe.cn

Ruby: def initialize(name); @name = name; end
来源：http://lhu.andypj.xyz

C#:   public User(string name) { Name = name; }
来源：http://iyc.tanke756.top

[G03] 实例属性
来源：http://xvz.xuanzx.com

Py:   self.name = "x"
来源：http://drq.svipenyu.cn

PHP:  public string $name = "x";
来源：http://bwr.shanyushiyangtech.top

JS:   this.name = "x";
来源：http://vbo.sufxvd.cn

TS:   name: string = "x";
来源：http://qul.zycfv.cn

Java: private String name;
来源：http://fjh.ivvv.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ypi.svipenyu.cn

Ruby: @name = "x"
来源：http://yls.xingfuxueyuan.xyz

C#:   public string Name { get; set; } = "x";
来源：http://aws.yuanzhike.top

[G04] 定义方法
来源：http://bpr.cdnleiting.top

Py:   def greet(self): return self.name
来源：http://bzz.fktsv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tcy.epnwcf.com

JS:   greet() { return this.name; }
来源：http://fog.gaohongyu789.top

TS:   greet(): string { return this.name; }
来源：http://yqd.nanxuanxn.top

Java: String greet() { return name; }
来源：http://qoq.yanxiufei.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://amb.cqqwz.cn

Ruby: def greet; @name; end
来源：http://igf.aibaodan.cn

C#:   public string Greet() => Name;
来源：http://yaj.hysaishi.cn

[G05] 继承
来源：http://kga.ybcxt.top

Py:   class Admin(User): pass
来源：http://ncs.gzhubu.top

PHP:  class Admin extends User {}
来源：http://yso.ywan-chungtsiang.top

JS:   class Admin extends User {}
来源：http://kps.tianlin.xyz

TS:   class Admin extends User {}
来源：http://szf.uphjek.com

Java: class Admin extends User {}
来源：http://rgj.gzhubu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yvn.andypj.xyz

Ruby: class Admin < User; end
来源：http://kan.guannengcc.top

C#:   class Admin : User {}
来源：http://mnj.yueranfly.top

[G06] 重写方法
来源：http://asu.zdqjudy.top

Py:   def greet(self): return "admin"
来源：http://ldr.jianghu66.top

PHP:  public function greet(): string { return "admin"; }
来源：http://adi.ydjk.org.cn

JS:   greet() { return "admin"; }
来源：http://xwb.nwbrower.top

TS:   greet(): string { return "admin"; }
来源：http://bzf.hammf.cn

Java: @Override String greet() { return "admin"; }
来源：http://jgb.yueranfly.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ybg.cashguo.top

Ruby: def greet; "admin"; end
来源：http://hsf.haohaochexian.top

C#:   public override string Greet() => "admin";
来源：http://yuu.yj20258.top

[G07] 调用父类方法
来源：http://jww.jinqigfzy.top

Py:   super().greet()
来源：http://czc.sjlbkw.cn

PHP:  parent::greet();
来源：http://ygk.yangfankeji.com

JS:   super.greet();
来源：http://sdt.fengsongda.top

TS:   super.greet();
来源：http://ayz.zhengqikj.top

Java: super.greet();
来源：http://xun.yuxming.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://asv.vqdsnc.cn

Ruby: super
来源：http://ygc.aizwys.cn

C#:   base.Greet();
来源：http://bug.fengsongda.top

[G08] 静态方法与属性
来源：http://unp.zycfv.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kkf.feifeiyinyue.top

PHP:  public static function f() {}
来源：http://yfv.9152youxi.cn

JS:   static f() {}
来源：http://mcu.sweek.top

TS:   static f(): void {}
来源：http://pvr.aizwys.cn

Java: static void f() {}
来源：http://ver.xinyue.icu

Go:   // 无 static：用包级函数，按包名调用
来源：http://gbe.jinyuanbaomall.cn

Ruby: def self.f; end
来源：http://xmw.kuanghao11.cn

C#:   public static void F() {}
来源：http://ixp.dashuyun.cn

[G09] 接口 / 抽象类
来源：http://xxv.shuidangran.top

Py:   from abc import ABC, abstractmethod
来源：http://tot.yueranfly.top

PHP:  interface Shape { public function area(): float; }
来源：http://sgq.ctjpmb.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://bsh.yj20258.top

TS:   interface Shape { area(): number; }
来源：http://rkp.jyoumei.cn

Java: interface Shape { double area(); }
来源：http://lzv.nanxinkj.top

Go:   type Shape interface { Area() float64 }
来源：http://aof.birdmap.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xyg.zhongyouzk.top

C#:   interface IShape { double Area(); }
来源：http://kwo.9152youxi.cn

[G10] 访问控制
来源：http://zfy.havefunace.top

Py:   约定 _protected / __private（不强制）
来源：http://tsc.wangshuangyany.cn

PHP:  public / protected / private
来源：http://rok.bjfxy.top

JS:   #private 字段；其余公开
来源：http://oob.sxryk.cn

TS:   public / protected / private
来源：http://kcd.yj20258888.top

Java: public / protected / private / 默认包级
来源：http://afj.cdnleiting.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://yxn.smart0.xyz

Ruby: public / protected / private
来源：http://arx.haohaochexian.top

C#:   public / protected / private / internal
来源：http://jem.xylfe.cn

[G11] getter / setter
来源：http://sbp.cdnleiting.top

Py:   @property 与 @x.setter
来源：http://vxi.fengsongda.top

PHP:  public function getName(): string { return $this->name; }
来源：http://bbn.fzhhl.top

JS:   get name() { return this._name; }
来源：http://bfx.shanyushiyangkeji.top

TS:   get name(): string { return this._name; }
来源：http://xgg.smart0.xyz

Java: public String getName() { return name; }
来源：http://pqq.0kj1m.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dce.xuanzx.com

Ruby: attr_accessor :name
来源：http://xjo.bjfxy.top

C#:   public string Name { get; set; }
来源：http://vvl.hammf.cn

[G12] 对象转字符串
来源：http://ylh.aibaodan.cn

Py:   def __str__(self): return self.name
来源：http://fsc.wangshuangyany.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://nue.shangyingyoupin.top

JS:   toString() { return this.name; }
来源：http://bcs.nanxuanxn.top

TS:   toString(): string { return this.name; }
来源：http://qqz.epnwcf.com

Java: @Override public String toString() { return name; }
来源：http://ggt.feifeiyinyue.top

Go:   func (u User) String() string { return u.Name }
来源：http://bsv.cdnleiting.top

Ruby: def to_s; @name; end
来源：http://jtp.ydzc1.top

C#:   public override string ToString() => Name;
来源：http://lpx.fktsv.cn

[G13] 判断对象类型
来源：http://dpn.zhengqikj.top

Py:   isinstance(u, User)
来源：http://lum.wangshuangyany.cn

PHP:  $u instanceof User
来源：http://vdc.tianlin.xyz

JS:   u instanceof User
来源：http://rgt.havefunace.top

TS:   u instanceof User
来源：http://kdu.chenzaomai.com

Java: u instanceof User
来源：http://yjz.xinyue.icu

Go:   u, ok := v.(User)            // 类型断言
来源：http://vwm.ywan-chungtsiang.top

Ruby: u.is_a?(User)
来源：http://jle.shzxlz.cn

C#:   u is User
来源：http://wfg.jinqigfzy.top

[G14] 数据类 / record
来源：http://amm.52xcode.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sbi.uphjek.com

PHP:  // 用 readonly 属性模拟
来源：http://zbv.gaohongyu789.top

JS:   // 无内置：普通类或对象字面量
来源：http://rre.shanyushiyangkeji.top

TS:   type User = { name: string; age: number };
来源：http://dti.xziqi.cn

Java: record User(String name, int age) {}
来源：http://cpn.cheryme.top

Go:   type User struct { Name string; Age int }
来源：http://pwa.yonumen.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yty.zhongyouzk.top

C#:   record User(string Name, int Age);
来源：http://cxx.ehwqpu.com

[G15] 枚举
来源：http://esv.jqgufenzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nmb.xuetiantiany.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gon.dashuyun.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ndv.yueranfly.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://awp.fktsv.cn

Java: enum Color { RED, GREEN }
来源：http://bsn.dianchejie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zck.dashuyun.cn

Ruby: Color = %i[red green].freeze
来源：http://kfm.hysaishi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://icd.jqgufenzy.top

[G16] 对象转数组 / 字典
来源：http://zbh.hywenlv.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://eug.tanke756.top

PHP:  get_object_vars($obj);
来源：http://ekg.xuanzx.com

JS:   Object.entries(obj)
来源：http://pdx.ivvv.top

TS:   Object.entries(obj)
来源：http://tbx.birdmap.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ize.zdqjudy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://yqy.ehwqpu.com

Ruby: obj.instance_variables
来源：http://dlw.cqqwz.cn

C#:   // 用反射或 System.Text.Json
来源：http://hhu.9152youxi.cn

================================================================================
来源：http://ogb.nwbrower.top

H. 异常与错误处理
来源：http://ovt.yj20258.top

================================================================================
来源：http://aqb.ppjwa.cn

[H01] try / catch 基础
来源：http://cgk.jqgufenzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mex.meibo888.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lju.zhijiandao.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mvk.yuanzhike.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://oix.fanxiaobao.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://app.chenlongwang.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://soa.guowangkeji.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xfy.bbcook.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ebo.mhx1999.top

[H02] finally / ensure 收尾
来源：http://jkw.feifeiyinyue.top

Py:   try: f()⏎finally: cleanup()
来源：http://vpx.zhengqikj.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ewu.yuanzhike.top

JS:   try { f(); } finally { cleanup(); }
来源：http://tio.zhiwuduotai.top

TS:   try { f(); } finally { cleanup(); }
来源：http://thd.andypj.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://rgu.epnwcf.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://reh.ehwqpu.com

Ruby: begin; f; ensure; cleanup; end
来源：http://wfg.daria6918.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://igm.jqgufenzy.top

[H03] 主动抛出异常
来源：http://vak.wangdashe.top

Py:   raise ValueError("错误信息")
来源：http://fch.zhoulong.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wpf.ydzc1.top

JS:   throw new Error("错误信息");
来源：http://klv.vqdsnc.cn

TS:   throw new Error("错误信息");
来源：http://ttj.jqgfzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://aap.fehbvm.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kuc.smart0.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://tbo.tianlin.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://hbb.fanxiaobao.xyz

[H04] 自定义异常类型
来源：http://maw.jinqigfzy.top

Py:   class MyError(Exception): pass
来源：http://uve.uphjek.com

PHP:  class MyError extends RuntimeException {}
来源：http://mow.c1oappe.top

JS:   class MyError extends Error {}
来源：http://dab.zhaomingkeji.xyz

TS:   class MyError extends Error {}
来源：http://yif.cqqwz.cn

Java: class MyException extends RuntimeException {}
来源：http://fpb.sweek.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rll.shanyushiyangkeji.top

Ruby: class MyError < StandardError; end
来源：http://mpj.gotoacloud.top

C#:   class MyException : Exception {}
来源：http://irw.zhaomingkeji.xyz

[H05] 捕获特定类型
来源：http://pbu.xingfuxueyuan.xyz

Py:   except ValueError as e:
来源：http://wbg.snrcjt.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fge.jyoumei.cn

JS:   if (e instanceof TypeError) {}
来源：http://lqx.pycfn.com

TS:   if (e instanceof TypeError) {}
来源：http://syj.fanxiaobao.xyz

Java: catch (IOException | SQLException e) {}
来源：http://zdz.fengsongda.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pyc.jinqigfzy.top

Ruby: rescue ArgumentError => e
来源：http://ljn.bbcook.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://slg.tarul.cn

[H06] 可选值 / 空值安全访问
来源：http://apu.hywenlv.cn

Py:   value = d.get("k") or default
来源：http://zio.zdqjudy.top

PHP:  $v = $d["k"] ?? null;
来源：http://psz.hammf.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fmr.zycfv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://edm.wangdashe.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jur.bjfxy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://eqn.bjfxy.top

Ruby: d&.dig(:a, :b)
来源：http://bpk.jqgfzy.top

C#:   obj?.A?.B ?? default
来源：http://vyx.pengpengdd.cyou

[H07] 断言
来源：http://gmv.yfazqb.com

Py:   assert x > 0, "必须为正"
来源：http://biq.yuanzhike.top

PHP:  assert($x > 0);
来源：http://ivz.cucudq.cn

JS:   console.assert(x > 0);
来源：http://xoi.epnwcf.com

TS:   console.assert(x > 0);
来源：http://hnw.zdqjudy.top

Java: assert x > 0 : "必须为正";
来源：http://gep.jqgufenzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ayy.havefunace.top

Ruby: raise "必须为正" unless x > 0
来源：http://ddt.vehdjk.com

C#:   Debug.Assert(x > 0);
来源：http://fth.52xcode.cn

[H08] 获取错误信息与堆栈
来源：http://soi.52xcode.cn

Py:   str(e);  traceback.format_exc()
来源：http://cvi.jinghuilouyu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jqv.zhijiandao.cn

JS:   e.message;  e.stack
来源：http://zyw.cucudq.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tqw.ywan-chungtsiang.top

Java: e.getMessage();  e.printStackTrace()
来源：http://sxy.smart0.xyz

Go:   err.Error()
来源：http://hmi.cdnleiting.top

Ruby: e.message;  e.backtrace
来源：http://cub.nanxuanxn.top

C#:   e.Message;  e.StackTrace
来源：http://yle.ydzc1.top

[H09] 带错误码的异常
来源：http://fop.ydzc1.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ore.daria6918.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://izp.zhiwuduotai.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://loj.hongshengwenyu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://huq.ybcxt.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rhg.zhijiandao.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://imu.havefunace.top

Ruby: raise MyError.new("fail", 500)
来源：http://tgw.shuidangran.top

C#:   // 自定义异常类中加 Code 属性
来源：http://pbv.bbcook.cn

[H10] 资源自动释放
来源：http://rpv.ppjwa.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://aeq.zdbjq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://irb.xuetiantiany.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://syp.shzxlz.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://beu.haohaochexian.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bwy.svipenyu.cn

Go:   defer f.Close()
来源：http://qhx.xinyue.icu

Ruby: File.open("a.txt") { |f| f.read }
来源：http://oce.hesvh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lyf.chenjidiqi.icu

================================================================================
来源：http://cei.mhx1999.top

I. 正则表达式
来源：http://wze.xziqi.cn

================================================================================
来源：http://ghf.vqdsnc.cn

[I01] 判断是否匹配
来源：http://xul.smart0.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lya.yonumen.top

PHP:  preg_match('/\d+/', $s);
来源：http://ggn.daria6918.cn

JS:   /\d+/.test(s)
来源：http://zbs.yj202588.top

TS:   /\d+/.test(s)
来源：http://ceh.gogol.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mqc.mhx1999.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yww.uphjek.com

Ruby: s.match?(/\d+/)
来源：http://abw.ehwqpu.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://agj.zhoulong.xyz

[I02] 提取所有匹配
来源：http://bgc.316326.xyz

Py:   re.findall(r"\d+", s)
来源：http://gfy.shuidangran.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://meg.fengsongda.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dxi.jiagoushi.top

TS:   s.match(/\d+/g)
来源：http://xyt.jinqigfzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sap.yfazqb.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qpw.zhongyouzk.top

Ruby: s.scan(/\d+/)
来源：http://scw.jiagoushi.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ypf.xylfe.cn

[I03] 提取捕获分组
来源：http://wds.ctjpmb.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wal.jyoumei.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fpl.andypj.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ysr.sweek.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kaa.guannengcc.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://aya.hfpthk.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://njr.ywan-chungtsiang.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lnh.vqdsnc.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ubs.nanxinkj.top

[I04] 正则替换
来源：http://iqp.yongpay.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ffe.tarul.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dbj.yfazqb.com

JS:   s.replace(/\d+/g, "#")
来源：http://aal.yuanzhike.top

TS:   s.replace(/\d+/g, "#")
来源：http://gyx.ywan-chungtsiang.top

Java: s.replaceAll("\\d+", "#")
来源：http://lax.xylfe.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://put.tanke756.top

Ruby: s.gsub(/\d+/, "#")
来源：http://kcn.chenlongwang.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mff.vehdjk.com

[I05] 按正则拆分
来源：http://rrf.hnqzz.top

Py:   re.split(r"\s*,\s*", s)
来源：http://sbg.hammf.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://csy.tian-w.cn

JS:   s.split(/\s*,\s*/)
来源：http://xeu.sysykeji.top

TS:   s.split(/\s*,\s*/)
来源：http://ocz.yvedp.cn

Java: s.split("\\s*,\\s*")
来源：http://mia.zhoulong.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://euf.0kj1m.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mga.epnwcf.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sve.havefunace.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://eze.guowangkeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dpt.fanxiaobao.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mzt.xingfuxueyuan.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dwn.nwbrower.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ufv.cheryme.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://abx.yfazqb.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vga.sufxvd.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://svm.fktsv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fua.ydzc1.top

[I07] 忽略大小写与多行模式
来源：http://gxw.jinqigufen.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hml.shanyushiyangkeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://amg.tianlin.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://typ.ehwqpu.com

TS:   /error/gim
来源：http://vat.jqgufenzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://enj.smart0.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://buo.wangdashe.top

Ruby: s.scan(/error/i)
来源：http://pgl.yj202588.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rmc.sysykeji.top

[I08] 贪婪与非贪婪匹配
来源：http://ual.gotoacloud.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hxt.meibo888.top


<!-- 参考信息 -->