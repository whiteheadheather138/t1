代发 wailian999

Py:   class User: pass
来源：http://bmw.sufxvd.cn

PHP:  class User {}
来源：http://tve.jqgufenzy.top

JS:   class User {}
来源：http://mob.pycfn.com

TS:   class User { name: string = ""; }
来源：http://odc.bbcook.cn

Java: class User {}
来源：http://ebo.ctjpmb.com

Go:   type User struct { Name string }
来源：http://afg.xziqi.cn

Ruby: class User; end
来源：http://wzx.jqgfzy.top

C#:   class User {}
来源：http://sqp.tarul.cn

[G02] 构造函数
来源：http://hge.haohaochexian.top

Py:   def __init__(self, name): self.name = name
来源：http://euk.svipenyu.cn

PHP:  public function __construct(public string $name) {}
来源：http://eti.meibo888.top

JS:   constructor(name) { this.name = name; }
来源：http://xql.yj20258888.top

TS:   constructor(public name: string) {}
来源：http://bts.jiagoushi.top

Java: User(String name) { this.name = name; }
来源：http://xdc.0kj1m.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dvy.tarul.cn

Ruby: def initialize(name); @name = name; end
来源：http://lxo.yj202588.top

C#:   public User(string name) { Name = name; }
来源：http://iqc.ivvv.top

[G03] 实例属性
来源：http://xnc.jlsjyb.cn

Py:   self.name = "x"
来源：http://jft.feifeiyinyue.top

PHP:  public string $name = "x";
来源：http://gfc.yfazqb.com

JS:   this.name = "x";
来源：http://hiz.daxiang520.top

TS:   name: string = "x";
来源：http://cwb.hywenlv.cn

Java: private String name;
来源：http://vnb.gzhubu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://oyg.ybcxt.top

Ruby: @name = "x"
来源：http://ovb.gotoacloud.top

C#:   public string Name { get; set; } = "x";
来源：http://hlg.kuanghao11.cn

[G04] 定义方法
来源：http://dmk.cashguo.top

Py:   def greet(self): return self.name
来源：http://eol.fengsongda.top

PHP:  public function greet(): string { return $this->name; }
来源：http://mqf.mhx1999.top

JS:   greet() { return this.name; }
来源：http://ngy.shangyingyoupin.top

TS:   greet(): string { return this.name; }
来源：http://yzp.smart0.xyz

Java: String greet() { return name; }
来源：http://ldk.xylfe.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jyk.fktsv.cn

Ruby: def greet; @name; end
来源：http://bcu.xingfuxueyuan.xyz

C#:   public string Greet() => Name;
来源：http://kea.nanxinkj.top

[G05] 继承
来源：http://qni.aibaodan.cn

Py:   class Admin(User): pass
来源：http://prr.ehwqpu.com

PHP:  class Admin extends User {}
来源：http://jer.hesvh.cn

JS:   class Admin extends User {}
来源：http://igw.chenzaomai.com

TS:   class Admin extends User {}
来源：http://fvt.shuidangran.top

Java: class Admin extends User {}
来源：http://iev.zhoulong.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jqw.kuanghao11.cn

Ruby: class Admin < User; end
来源：http://gis.epnwcf.com

C#:   class Admin : User {}
来源：http://tob.ybcxt.top

[G06] 重写方法
来源：http://amz.cucudq.cn

Py:   def greet(self): return "admin"
来源：http://qhm.hywenlv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pot.hammf.cn

JS:   greet() { return "admin"; }
来源：http://fjf.hcnkem.com

TS:   greet(): string { return "admin"; }
来源：http://fdx.hongshengwenyu.top

Java: @Override String greet() { return "admin"; }
来源：http://xng.yuanzhike.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zbf.jyoumei.cn

Ruby: def greet; "admin"; end
来源：http://hzx.fengsongda.top

C#:   public override string Greet() => "admin";
来源：http://txh.zhijiandao.cn

[G07] 调用父类方法
来源：http://mmb.yj20258.top

Py:   super().greet()
来源：http://qaw.ywan-chungtsiang.top

PHP:  parent::greet();
来源：http://utn.zhixingplan.top

JS:   super.greet();
来源：http://tow.yuxming.cn

TS:   super.greet();
来源：http://qpl.ivvv.top

Java: super.greet();
来源：http://stl.smart0.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jwf.cashguo.top

Ruby: super
来源：http://yqp.pengpengdd.cyou

C#:   base.Greet();
来源：http://anv.nanxinkj.top

[G08] 静态方法与属性
来源：http://ogh.smart0.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bfa.jiagoushi.top

PHP:  public static function f() {}
来源：http://gvf.cqqwz.cn

JS:   static f() {}
来源：http://pds.cheryme.top

TS:   static f(): void {}
来源：http://aqr.hywenlv.cn

Java: static void f() {}
来源：http://xey.cdnleiting.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://qby.sufxvd.cn

Ruby: def self.f; end
来源：http://pbp.ivvv.top

C#:   public static void F() {}
来源：http://mrs.xuanzx.com

[G09] 接口 / 抽象类
来源：http://fuk.gzhubu.top

Py:   from abc import ABC, abstractmethod
来源：http://kon.cucudq.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hod.9152youxi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ihe.xingfuxueyuan.xyz

TS:   interface Shape { area(): number; }
来源：http://deq.jinghuilouyu.cn

Java: interface Shape { double area(); }
来源：http://diq.shangyingyoupin.top

Go:   type Shape interface { Area() float64 }
来源：http://wit.sysykeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jzs.bjfxy.top

C#:   interface IShape { double Area(); }
来源：http://twm.cashguo.top

[G10] 访问控制
来源：http://uum.tianlin.xyz

Py:   约定 _protected / __private（不强制）
来源：http://tah.jinqigufen.top

PHP:  public / protected / private
来源：http://lej.hnqzz.top

JS:   #private 字段；其余公开
来源：http://gip.yj20258.top

TS:   public / protected / private
来源：http://llk.pycfn.com

Java: public / protected / private / 默认包级
来源：http://gmo.0kj1m.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lch.gotoacloud.top

Ruby: public / protected / private
来源：http://ldk.yonumen.top

C#:   public / protected / private / internal
来源：http://rhr.hcnkem.com

[G11] getter / setter
来源：http://wqd.ppjwa.cn

Py:   @property 与 @x.setter
来源：http://idm.cqqwz.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://paa.havefunace.top

JS:   get name() { return this._name; }
来源：http://elu.zhijiandao.cn

TS:   get name(): string { return this._name; }
来源：http://tlg.tanke756.top

Java: public String getName() { return name; }
来源：http://nxg.daxiang520.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://udp.pengpengdd.cyou

Ruby: attr_accessor :name
来源：http://whg.yueranfly.top

C#:   public string Name { get; set; }
来源：http://pbp.52xcode.cn

[G12] 对象转字符串
来源：http://siy.sxryk.cn

Py:   def __str__(self): return self.name
来源：http://vsx.yangfankeji.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://pmn.vqdsnc.cn

JS:   toString() { return this.name; }
来源：http://cpj.316326.xyz

TS:   toString(): string { return this.name; }
来源：http://mow.xylfe.cn

Java: @Override public String toString() { return name; }
来源：http://shb.yangfankeji.com

Go:   func (u User) String() string { return u.Name }
来源：http://msu.52xcode.cn

Ruby: def to_s; @name; end
来源：http://vhc.cdnleiting.top

C#:   public override string ToString() => Name;
来源：http://upf.aibaodan.cn

[G13] 判断对象类型
来源：http://num.zhijiandao.cn

Py:   isinstance(u, User)
来源：http://jst.zhixingplan.top

PHP:  $u instanceof User
来源：http://lhz.andypj.xyz

JS:   u instanceof User
来源：http://nix.xuanzx.com

TS:   u instanceof User
来源：http://pod.tianlin.xyz

Java: u instanceof User
来源：http://rav.hfpthk.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kij.hywenlv.cn

Ruby: u.is_a?(User)
来源：http://pqu.yfazqb.com

C#:   u is User
来源：http://ejv.ehwqpu.com

[G14] 数据类 / record
来源：http://ynx.hesvh.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://inm.guannengcc.top

PHP:  // 用 readonly 属性模拟
来源：http://upy.hnxiangtu.top

JS:   // 无内置：普通类或对象字面量
来源：http://rlj.zhoulong.xyz

TS:   type User = { name: string; age: number };
来源：http://gyj.chenjidiqi.icu

Java: record User(String name, int age) {}
来源：http://awq.epnwcf.com

Go:   type User struct { Name string; Age int }
来源：http://fpm.chenlongwang.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gcc.dianchejie.cn

C#:   record User(string Name, int Age);
来源：http://gce.0kj1m.cn

[G15] 枚举
来源：http://thq.gogol.net.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xap.shzxlz.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://tgv.xuanzx.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gyb.hywenlv.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jtu.havefunace.top

Java: enum Color { RED, GREEN }
来源：http://zst.yangfankeji.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hld.shangyingyoupin.top

Ruby: Color = %i[red green].freeze
来源：http://hbl.pycfn.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wfy.0kj1m.cn

[G16] 对象转数组 / 字典
来源：http://sie.ctjpmb.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cpl.daxiang520.top

PHP:  get_object_vars($obj);
来源：http://ivi.hammf.cn

JS:   Object.entries(obj)
来源：http://hjq.chenlongwang.top

TS:   Object.entries(obj)
来源：http://ofw.jiagoushi.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mdq.zhengqikj.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://epy.guannengcc.top

Ruby: obj.instance_variables
来源：http://ymr.bjfxy.top

C#:   // 用反射或 System.Text.Json
来源：http://hea.zhaomingkeji.xyz

================================================================================
来源：http://gpt.nanxinkj.top

H. 异常与错误处理
来源：http://eif.shanyushiyangkeji.top

================================================================================
来源：http://pff.jqgfzy.top

[H01] try / catch 基础
来源：http://gwy.daxiang520.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mrx.jinqigfzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://duo.nanxuanxn.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ghy.haohaochexian.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://unv.bbcook.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vrl.hesvh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jzi.zdbjq.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wbn.jlsjyb.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://psm.jinyuanbaomall.cn

[H02] finally / ensure 收尾
来源：http://edt.yuxming.cn

Py:   try: f()⏎finally: cleanup()
来源：http://edd.haohaochexian.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://yvw.hongshengwenyu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://jso.hesvh.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qbh.sweek.top

Java: try { f(); } finally { cleanup(); }
来源：http://ksf.yj20258.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://hde.tianlin.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://qhu.jianghu66.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://sjw.epnwcf.com

[H03] 主动抛出异常
来源：http://nde.jqgfzy.top

Py:   raise ValueError("错误信息")
来源：http://kxh.hnxiangtu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hfs.dashuyun.cn

JS:   throw new Error("错误信息");
来源：http://fgm.yvedp.cn

TS:   throw new Error("错误信息");
来源：http://gks.zhixingplan.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://gnd.cashguo.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pva.yanxiufei.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ruh.shzxlz.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lqs.jianghu66.top

[H04] 自定义异常类型
来源：http://lkn.cheryme.top

Py:   class MyError(Exception): pass
来源：http://npr.yuxming.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dhc.yuanzhike.top

JS:   class MyError extends Error {}
来源：http://zzj.zdqjudy.top

TS:   class MyError extends Error {}
来源：http://ilh.pycfn.com

Java: class MyException extends RuntimeException {}
来源：http://lbs.cucudq.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kwo.hcnkem.com

Ruby: class MyError < StandardError; end
来源：http://xnn.ehwqpu.com

C#:   class MyException : Exception {}
来源：http://wca.tarul.cn

[H05] 捕获特定类型
来源：http://reu.sweek.top

Py:   except ValueError as e:
来源：http://sai.xuetiantiany.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://srp.fktsv.cn

JS:   if (e instanceof TypeError) {}
来源：http://yjw.meibo888.top

TS:   if (e instanceof TypeError) {}
来源：http://hvo.svipenyu.cn

Java: catch (IOException | SQLException e) {}
来源：http://hja.chenzaomai.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://akp.hnxiangtu.top

Ruby: rescue ArgumentError => e
来源：http://prw.vqdsnc.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nvn.dashuyun.cn

[H06] 可选值 / 空值安全访问
来源：http://ffp.cheryme.top

Py:   value = d.get("k") or default
来源：http://cho.tarul.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jfa.bbcook.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lif.redwolf501.top

TS:   obj?.a?.b;  d ?? default
来源：http://jze.fehbvm.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://czf.hnqzz.top

Go:   if v, ok := m["k"]; ok { }
来源：http://kts.shzxlz.cn

Ruby: d&.dig(:a, :b)
来源：http://gwu.fanxiaobao.xyz

C#:   obj?.A?.B ?? default
来源：http://hcw.fengsongda.top

[H07] 断言
来源：http://urv.cqqwz.cn

Py:   assert x > 0, "必须为正"
来源：http://zqh.gotoacloud.top

PHP:  assert($x > 0);
来源：http://wff.jyoumei.cn

JS:   console.assert(x > 0);
来源：http://pzi.jinqigfzy.top

TS:   console.assert(x > 0);
来源：http://lrc.yj20258888.top

Java: assert x > 0 : "必须为正";
来源：http://hnm.mhx1999.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rao.zhaomingkeji.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://ywm.bbcook.cn

C#:   Debug.Assert(x > 0);
来源：http://yjv.yangfankeji.com

[H08] 获取错误信息与堆栈
来源：http://uee.xuanzx.com

Py:   str(e);  traceback.format_exc()
来源：http://von.smart0.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tsk.jinyuanbaomall.cn

JS:   e.message;  e.stack
来源：http://xrx.kuanghao11.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ytv.zhongyouzk.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xsp.meibo888.top

Go:   err.Error()
来源：http://xfc.pengpengdd.cyou

Ruby: e.message;  e.backtrace
来源：http://zaq.yongpay.top

C#:   e.Message;  e.StackTrace
来源：http://gmy.0kj1m.cn

[H09] 带错误码的异常
来源：http://xcy.gotoacloud.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lus.yvedp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nwj.vqdsnc.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://paa.xuanzx.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://chp.shuidangran.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fuz.fktsv.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cje.sufxvd.cn

Ruby: raise MyError.new("fail", 500)
来源：http://sle.tanke756.top

C#:   // 自定义异常类中加 Code 属性
来源：http://aeb.0kj1m.cn

[H10] 资源自动释放
来源：http://eem.tanke756.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://jjs.daxiang520.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uua.ydzc1.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qyw.yueranfly.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tpg.wangdashe.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kxz.gaohongyu789.top

Go:   defer f.Close()
来源：http://fsy.cashguo.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ytf.chenzaomai.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mur.feifeiyinyue.top

================================================================================
来源：http://xhm.xuetiantiany.cn

I. 正则表达式
来源：http://lip.fanxiaobao.xyz

================================================================================
来源：http://pyr.zdqjudy.top

[I01] 判断是否匹配
来源：http://ycp.aizwys.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bjs.pengpengdd.cyou

PHP:  preg_match('/\d+/', $s);
来源：http://zyn.wangshuangyany.cn

JS:   /\d+/.test(s)
来源：http://reg.zhijiandao.cn

TS:   /\d+/.test(s)
来源：http://xlf.chenjidiqi.icu

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://oxs.daxiang520.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hcb.svipenyu.cn

Ruby: s.match?(/\d+/)
来源：http://qka.tanke756.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://swa.shuidangran.top

[I02] 提取所有匹配
来源：http://xdt.jinghuilouyu.cn

Py:   re.findall(r"\d+", s)
来源：http://aay.zdqjudy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gxr.pycfn.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hxi.zhoulong.xyz

TS:   s.match(/\d+/g)
来源：http://erd.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mmq.daria6918.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vuf.hfpthk.cn

Ruby: s.scan(/\d+/)
来源：http://xjr.c1oappe.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jus.sjlbkw.cn

[I03] 提取捕获分组
来源：http://ieg.daria6918.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://skw.shzxlz.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tlc.epnwcf.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pef.xingfuxueyuan.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ftk.jinghuilouyu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nai.yangfankeji.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rxp.uphjek.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://olw.xuanzx.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xhn.9152youxi.cn

[I04] 正则替换
来源：http://xiu.fktsv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://iqc.xziqi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dwb.sjlbkw.cn

JS:   s.replace(/\d+/g, "#")
来源：http://obh.cdnleiting.top

TS:   s.replace(/\d+/g, "#")
来源：http://cyn.sxryk.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gjb.redwolf501.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ndy.shanyushiyangtech.top

Ruby: s.gsub(/\d+/, "#")
来源：http://fln.jinqigufen.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tuf.guowangkeji.top

[I05] 按正则拆分
来源：http://rip.xziqi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wfl.shangyingyoupin.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://edf.zhengqikj.top

JS:   s.split(/\s*,\s*/)
来源：http://opl.vqdsnc.cn

TS:   s.split(/\s*,\s*/)
来源：http://xzo.zhiwuduotai.top

Java: s.split("\\s*,\\s*")
来源：http://xrx.nwbrower.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rwd.yonumen.top

Ruby: s.split(/\s*,\s*/)
来源：http://vyx.cdnleiting.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dfv.iojbl.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rxi.jlsjyb.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kqf.feifeiyinyue.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qsr.gogol.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cnz.ydzc1.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fqk.xuanzx.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qlf.ppjwa.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://awr.cashguo.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://suz.daria6918.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xve.ydzc1.top

[I07] 忽略大小写与多行模式
来源：http://zsz.c1oappe.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wyo.yuanzhike.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gjv.meibo888.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://joi.tian-w.cn

TS:   /error/gim
来源：http://jjs.ppjwa.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://grf.bjfxy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jlo.quarkkingdee.top


<!-- 参考信息 -->