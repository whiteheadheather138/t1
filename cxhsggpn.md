代发 wailian999

Py:   class User: pass
来源：http://ett.fengsongda.top

PHP:  class User {}
来源：http://jwi.xziqi.cn

JS:   class User {}
来源：http://xzw.sjlbkw.cn

TS:   class User { name: string = ""; }
来源：http://vtc.hcnkem.com

Java: class User {}
来源：http://clm.zhoulong.xyz

Go:   type User struct { Name string }
来源：http://zzg.haohaochexian.top

Ruby: class User; end
来源：http://fck.gotoacloud.top

C#:   class User {}
来源：http://nco.ehwqpu.com

[G02] 构造函数
来源：http://pip.sweek.top

Py:   def __init__(self, name): self.name = name
来源：http://ldi.hcnkem.com

PHP:  public function __construct(public string $name) {}
来源：http://ueq.hywenlv.cn

JS:   constructor(name) { this.name = name; }
来源：http://rhi.ppjwa.cn

TS:   constructor(public name: string) {}
来源：http://yyc.hywenlv.cn

Java: User(String name) { this.name = name; }
来源：http://rgh.jinqigufen.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://net.hesvh.cn

Ruby: def initialize(name); @name = name; end
来源：http://ppi.yonumen.top

C#:   public User(string name) { Name = name; }
来源：http://kio.yangfankeji.com

[G03] 实例属性
来源：http://ibl.tian-w.cn

Py:   self.name = "x"
来源：http://pbv.nanxuanxn.top

PHP:  public string $name = "x";
来源：http://bwu.zhengqikj.top

JS:   this.name = "x";
来源：http://yjf.zhiwuduotai.top

TS:   name: string = "x";
来源：http://tzn.svipenyu.cn

Java: private String name;
来源：http://avx.ydzc1.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zis.quarkkingdee.top

Ruby: @name = "x"
来源：http://vmf.sysykeji.top

C#:   public string Name { get; set; } = "x";
来源：http://lbm.tian-w.cn

[G04] 定义方法
来源：http://stm.shzxlz.cn

Py:   def greet(self): return self.name
来源：http://rwa.0kj1m.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://osz.zhoulong.xyz

JS:   greet() { return this.name; }
来源：http://oie.haohaochexian.top

TS:   greet(): string { return this.name; }
来源：http://dxe.birdmap.top

Java: String greet() { return name; }
来源：http://aqv.fehbvm.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://asq.zycfv.cn

Ruby: def greet; @name; end
来源：http://spc.ybcxt.top

C#:   public string Greet() => Name;
来源：http://hwm.vehdjk.com

[G05] 继承
来源：http://usp.dashuyun.cn

Py:   class Admin(User): pass
来源：http://ufu.yongpay.top

PHP:  class Admin extends User {}
来源：http://qpp.jiagoushi.top

JS:   class Admin extends User {}
来源：http://cxn.meibo888.top

TS:   class Admin extends User {}
来源：http://kll.xingfuxueyuan.xyz

Java: class Admin extends User {}
来源：http://gii.yj202588.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rwn.xylfe.cn

Ruby: class Admin < User; end
来源：http://xfs.zhijiandao.cn

C#:   class Admin : User {}
来源：http://zcu.jqgufenzy.top

[G06] 重写方法
来源：http://rwn.xinyue.icu

Py:   def greet(self): return "admin"
来源：http://smi.jiagoushi.top

PHP:  public function greet(): string { return "admin"; }
来源：http://egu.redwolf501.top

JS:   greet() { return "admin"; }
来源：http://odg.zhixingplan.top

TS:   greet(): string { return "admin"; }
来源：http://fpd.hnxiangtu.top

Java: @Override String greet() { return "admin"; }
来源：http://usm.jqgufenzy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ikl.xylfe.cn

Ruby: def greet; "admin"; end
来源：http://fkh.hongshengwenyu.top

C#:   public override string Greet() => "admin";
来源：http://fmq.tianlin.xyz

[G07] 调用父类方法
来源：http://yaq.xziqi.cn

Py:   super().greet()
来源：http://dsu.hesvh.cn

PHP:  parent::greet();
来源：http://jpy.0kj1m.cn

JS:   super.greet();
来源：http://wat.hongshengwenyu.top

TS:   super.greet();
来源：http://psp.daxiang520.top

Java: super.greet();
来源：http://wyq.hysaishi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zpe.iojbl.cn

Ruby: super
来源：http://maz.zhaomingkeji.xyz

C#:   base.Greet();
来源：http://qcw.ppjwa.cn

[G08] 静态方法与属性
来源：http://hze.epnwcf.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qzv.ywan-chungtsiang.top

PHP:  public static function f() {}
来源：http://rzu.aizwys.cn

JS:   static f() {}
来源：http://bgt.jiagoushi.top

TS:   static f(): void {}
来源：http://jzl.wangshuangyany.cn

Java: static void f() {}
来源：http://qoe.yj202588.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://sem.sufxvd.cn

Ruby: def self.f; end
来源：http://hnb.fzhhl.top

C#:   public static void F() {}
来源：http://vok.wangshuangyany.cn

[G09] 接口 / 抽象类
来源：http://eos.hnxiangtu.top

Py:   from abc import ABC, abstractmethod
来源：http://smr.zhijiandao.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lvp.ydzc1.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://qbl.cdnleiting.top

TS:   interface Shape { area(): number; }
来源：http://kcw.jinqigfzy.top

Java: interface Shape { double area(); }
来源：http://zfr.sysykeji.top

Go:   type Shape interface { Area() float64 }
来源：http://fhy.wangshuangyany.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lca.smart0.xyz

C#:   interface IShape { double Area(); }
来源：http://njl.zhongyouzk.top

[G10] 访问控制
来源：http://rxj.hnxiangtu.top

Py:   约定 _protected / __private（不强制）
来源：http://cmz.yonumen.top

PHP:  public / protected / private
来源：http://pev.yvedp.cn

JS:   #private 字段；其余公开
来源：http://eoo.fehbvm.com

TS:   public / protected / private
来源：http://bez.chenzaomai.com

Java: public / protected / private / 默认包级
来源：http://ptq.yj202588.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://xdk.xuanzx.com

Ruby: public / protected / private
来源：http://iyi.tarul.cn

C#:   public / protected / private / internal
来源：http://irz.jinyuanbaomall.cn

[G11] getter / setter
来源：http://fzd.aizwys.cn

Py:   @property 与 @x.setter
来源：http://hfr.xuetiantiany.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://plj.jianghu66.top

JS:   get name() { return this._name; }
来源：http://nek.epnwcf.com

TS:   get name(): string { return this._name; }
来源：http://myb.chenzaomai.com

Java: public String getName() { return name; }
来源：http://eka.chenjidiqi.icu

Go:   func (u User) GetName() string { return u.Name }
来源：http://upi.jqgufenzy.top

Ruby: attr_accessor :name
来源：http://ozj.zhaomingkeji.xyz

C#:   public string Name { get; set; }
来源：http://upz.feifeiyinyue.top

[G12] 对象转字符串
来源：http://lyv.hongshengwenyu.top

Py:   def __str__(self): return self.name
来源：http://fcu.zhengqikj.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://bov.ybcxt.top

JS:   toString() { return this.name; }
来源：http://kxs.ppjwa.cn

TS:   toString(): string { return this.name; }
来源：http://qwa.xingfuxueyuan.xyz

Java: @Override public String toString() { return name; }
来源：http://crz.yj20258.top

Go:   func (u User) String() string { return u.Name }
来源：http://qpi.hywenlv.cn

Ruby: def to_s; @name; end
来源：http://nzw.vehdjk.com

C#:   public override string ToString() => Name;
来源：http://rrb.dashuyun.cn

[G13] 判断对象类型
来源：http://bed.gzhubu.top

Py:   isinstance(u, User)
来源：http://hzl.ppjwa.cn

PHP:  $u instanceof User
来源：http://gxa.smart0.xyz

JS:   u instanceof User
来源：http://veo.cashguo.top

TS:   u instanceof User
来源：http://vii.cucudq.cn

Java: u instanceof User
来源：http://gnq.uphjek.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://wjr.shuidangran.top

Ruby: u.is_a?(User)
来源：http://che.birdmap.top

C#:   u is User
来源：http://pia.chenlongwang.top

[G14] 数据类 / record
来源：http://kuc.jinqigfzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://soe.fanxiaobao.xyz

PHP:  // 用 readonly 属性模拟
来源：http://gsf.pycfn.com

JS:   // 无内置：普通类或对象字面量
来源：http://oho.pycfn.com

TS:   type User = { name: string; age: number };
来源：http://oxc.andypj.xyz

Java: record User(String name, int age) {}
来源：http://dto.pycfn.com

Go:   type User struct { Name string; Age int }
来源：http://fcg.uphjek.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zab.fanxiaobao.xyz

C#:   record User(string Name, int Age);
来源：http://tqj.sufxvd.cn

[G15] 枚举
来源：http://vir.tianlin.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pcn.smart0.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://rxl.tian-w.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dko.cqqwz.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://iir.xziqi.cn

Java: enum Color { RED, GREEN }
来源：http://wnn.fzhhl.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yxi.xinyue.icu

Ruby: Color = %i[red green].freeze
来源：http://yxd.yj202588.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bhs.guowangkeji.top

[G16] 对象转数组 / 字典
来源：http://bsz.daxiang520.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ykb.jinyuanbaomall.cn

PHP:  get_object_vars($obj);
来源：http://wei.zhijiandao.cn

JS:   Object.entries(obj)
来源：http://llp.hfpthk.cn

TS:   Object.entries(obj)
来源：http://bbx.dianchejie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hvs.52xcode.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gew.xylfe.cn

Ruby: obj.instance_variables
来源：http://jpi.yueranfly.top

C#:   // 用反射或 System.Text.Json
来源：http://jxw.shanyushiyangkeji.top

================================================================================
来源：http://ozd.jqgufenzy.top

H. 异常与错误处理
来源：http://ubm.0kj1m.cn

================================================================================
来源：http://vsr.xuetiantiany.cn

[H01] try / catch 基础
来源：http://nkc.zhongyouzk.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://irk.sysykeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qby.yvedp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ejq.shangyingyoupin.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mka.sxryk.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rrz.9152youxi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xhh.hongshengwenyu.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dda.andypj.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oqp.smart0.xyz

[H02] finally / ensure 收尾
来源：http://smr.hongshengwenyu.top

Py:   try: f()⏎finally: cleanup()
来源：http://bbb.sufxvd.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://liv.nwbrower.top

JS:   try { f(); } finally { cleanup(); }
来源：http://xen.jinqigfzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://kic.gzhubu.top

Java: try { f(); } finally { cleanup(); }
来源：http://sti.yj20258888.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://sfp.vqdsnc.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kfv.jinqigfzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://qkt.yuxming.cn

[H03] 主动抛出异常
来源：http://agy.xuanzx.com

Py:   raise ValueError("错误信息")
来源：http://rxs.yanxiufei.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://huu.yuxming.cn

JS:   throw new Error("错误信息");
来源：http://xni.hcnkem.com

TS:   throw new Error("错误信息");
来源：http://tuy.yj202588.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://osf.nwbrower.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jsx.kuanghao11.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://odj.jyoumei.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lhm.shanyushiyangkeji.top

[H04] 自定义异常类型
来源：http://pkn.xuanzx.com

Py:   class MyError(Exception): pass
来源：http://ezj.feifeiyinyue.top

PHP:  class MyError extends RuntimeException {}
来源：http://cse.yvedp.cn

JS:   class MyError extends Error {}
来源：http://phm.yanxiufei.cn

TS:   class MyError extends Error {}
来源：http://vau.hysaishi.cn

Java: class MyException extends RuntimeException {}
来源：http://vms.meibo888.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://iqx.jqgfzy.top

Ruby: class MyError < StandardError; end
来源：http://xwk.zdqjudy.top

C#:   class MyException : Exception {}
来源：http://som.fktsv.cn

[H05] 捕获特定类型
来源：http://cyq.wangdashe.top

Py:   except ValueError as e:
来源：http://arf.yj202588.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zbr.hywenlv.cn

JS:   if (e instanceof TypeError) {}
来源：http://wfe.svipenyu.cn

TS:   if (e instanceof TypeError) {}
来源：http://nev.yangfankeji.com

Java: catch (IOException | SQLException e) {}
来源：http://nzq.fktsv.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cjp.ivvv.top

Ruby: rescue ArgumentError => e
来源：http://nau.chenlongwang.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uhu.pengpengdd.cyou

[H06] 可选值 / 空值安全访问
来源：http://hvg.yongpay.top

Py:   value = d.get("k") or default
来源：http://xae.hfpthk.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fap.ydzc1.top

JS:   obj?.a?.b;  d ?? default
来源：http://dlq.fengsongda.top

TS:   obj?.a?.b;  d ?? default
来源：http://vam.gogol.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lav.jiagoushi.top

Go:   if v, ok := m["k"]; ok { }
来源：http://zsw.yuxming.cn

Ruby: d&.dig(:a, :b)
来源：http://zeh.hnxiangtu.top

C#:   obj?.A?.B ?? default
来源：http://dbo.fktsv.cn

[H07] 断言
来源：http://tcv.xziqi.cn

Py:   assert x > 0, "必须为正"
来源：http://kgj.daria6918.cn

PHP:  assert($x > 0);
来源：http://fne.hcnkem.com

JS:   console.assert(x > 0);
来源：http://clj.jlsjyb.cn

TS:   console.assert(x > 0);
来源：http://izj.yj20258888.top

Java: assert x > 0 : "必须为正";
来源：http://fvq.yangfankeji.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://alb.yuxming.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gtl.wangdashe.top

C#:   Debug.Assert(x > 0);
来源：http://prb.yongpay.top

[H08] 获取错误信息与堆栈
来源：http://wgn.xylfe.cn

Py:   str(e);  traceback.format_exc()
来源：http://muh.jinyuanbaomall.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yjw.wangdashe.top

JS:   e.message;  e.stack
来源：http://vwp.yj202588.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://bdt.daria6918.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://rdh.hnxiangtu.top

Go:   err.Error()
来源：http://isf.sysykeji.top

Ruby: e.message;  e.backtrace
来源：http://rpm.jianghu66.top

C#:   e.Message;  e.StackTrace
来源：http://lhm.fanxiaobao.xyz

[H09] 带错误码的异常
来源：http://roo.yj20258.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kcm.jyoumei.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://oek.yuxming.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nvt.xuanzx.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qmw.hnqzz.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ndx.hongshengwenyu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tci.dianchejie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xdz.fanxiaobao.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://uwp.jyoumei.cn

[H10] 资源自动释放
来源：http://rrn.ydzc1.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://etr.xylfe.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://aib.wangdashe.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tuh.jiagoushi.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kfp.gzhubu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cag.sjlbkw.cn

Go:   defer f.Close()
来源：http://nhk.birdmap.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://trv.tian-w.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fra.shuidangran.top

================================================================================
来源：http://qbv.dianchejie.cn

I. 正则表达式
来源：http://ntf.redwolf501.top

================================================================================
来源：http://zxl.yfazqb.com

[I01] 判断是否匹配
来源：http://azb.gotoacloud.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jfd.epnwcf.com

PHP:  preg_match('/\d+/', $s);
来源：http://kgl.jqgufenzy.top

JS:   /\d+/.test(s)
来源：http://cia.bbcook.cn

TS:   /\d+/.test(s)
来源：http://pzz.zhaomingkeji.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tpu.cashguo.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jxe.hongshengwenyu.top

Ruby: s.match?(/\d+/)
来源：http://mje.hywenlv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jbr.tarul.cn

[I02] 提取所有匹配
来源：http://wen.quarkkingdee.top

Py:   re.findall(r"\d+", s)
来源：http://alv.zhaomingkeji.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fxb.ehwqpu.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kcn.shuidangran.top

TS:   s.match(/\d+/g)
来源：http://rjf.guannengcc.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jfa.svipenyu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gcv.zycfv.cn

Ruby: s.scan(/\d+/)
来源：http://ucr.shanyushiyangkeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://won.xinyue.icu

[I03] 提取捕获分组
来源：http://kgz.tianlin.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qxh.aibaodan.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jqj.ehwqpu.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cfl.yj202588.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://skp.xinyue.icu

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tsq.shanyushiyangtech.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tto.shangyingyoupin.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bmr.hnxiangtu.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://twe.quarkkingdee.top

[I04] 正则替换
来源：http://eda.ydjk.org.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zxj.zhijiandao.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fdn.xingfuxueyuan.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://wgk.snrcjt.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hcs.feifeiyinyue.top

Java: s.replaceAll("\\d+", "#")
来源：http://rbj.pycfn.com

Go:   re.ReplaceAllString(s, "#")
来源：http://zbm.yanxiufei.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://uyk.c1oappe.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lzs.shuidangran.top

[I05] 按正则拆分
来源：http://bje.gotoacloud.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ouo.quarkkingdee.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ffu.sysykeji.top

JS:   s.split(/\s*,\s*/)
来源：http://pyy.guowangkeji.top

TS:   s.split(/\s*,\s*/)
来源：http://xqf.haohaochexian.top

Java: s.split("\\s*,\\s*")
来源：http://yeb.bbcook.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bii.zhoulong.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://ubh.jqgfzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ute.jianghu66.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ued.jqgfzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xcm.jqgfzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://eve.fzhhl.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://saz.gzhubu.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://grm.yfazqb.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bkq.chenjidiqi.icu

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rds.dashuyun.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://acn.c1oappe.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zfs.jinghuilouyu.cn

[I07] 忽略大小写与多行模式
来源：http://ukm.shzxlz.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wdg.zdqjudy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mvo.aizwys.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kli.feifeiyinyue.top

TS:   /error/gim
来源：http://rkb.aizwys.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nmk.zhongyouzk.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lyw.redwolf501.top


<!-- 参考信息 -->