代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sto.kuanghao11.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nsa.zhongyouzk.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fdw.snrcjt.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://btg.epnwcf.com

================================================================================
来源：http://znm.xinyue.icu

G. 面向对象
来源：http://rpo.chenzaomai.com

================================================================================
来源：http://mqo.jqgfzy.top

[G01] 定义类
来源：http://pjx.9152youxi.cn

Py:   class User: pass
来源：http://clh.iojbl.cn

PHP:  class User {}
来源：http://szl.zhoulong.xyz

JS:   class User {}
来源：http://pjv.yj20258.top

TS:   class User { name: string = ""; }
来源：http://shw.xingfuxueyuan.xyz

Java: class User {}
来源：http://pjb.xingfuxueyuan.xyz

Go:   type User struct { Name string }
来源：http://rtb.yfazqb.com

Ruby: class User; end
来源：http://uri.fehbvm.com

C#:   class User {}
来源：http://mzi.jlsjyb.cn

[G02] 构造函数
来源：http://lfw.chenlongwang.top

Py:   def __init__(self, name): self.name = name
来源：http://prk.fanxiaobao.xyz

PHP:  public function __construct(public string $name) {}
来源：http://sst.ydjk.org.cn

JS:   constructor(name) { this.name = name; }
来源：http://uro.sufxvd.cn

TS:   constructor(public name: string) {}
来源：http://kmw.tarul.cn

Java: User(String name) { this.name = name; }
来源：http://csg.jiagoushi.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jtu.yueranfly.top

Ruby: def initialize(name); @name = name; end
来源：http://rfk.andypj.xyz

C#:   public User(string name) { Name = name; }
来源：http://upi.yangfankeji.com

[G03] 实例属性
来源：http://ysr.cheryme.top

Py:   self.name = "x"
来源：http://lkc.jyoumei.cn

PHP:  public string $name = "x";
来源：http://hss.xuetiantiany.cn

JS:   this.name = "x";
来源：http://jiz.jinqigufen.top

TS:   name: string = "x";
来源：http://vun.xuanzx.com

Java: private String name;
来源：http://iob.yonumen.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vmf.yvedp.cn

Ruby: @name = "x"
来源：http://sjh.hesvh.cn

C#:   public string Name { get; set; } = "x";
来源：http://eoz.gaohongyu789.top

[G04] 定义方法
来源：http://bzy.xingfuxueyuan.xyz

Py:   def greet(self): return self.name
来源：http://qnl.meibo888.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ajk.nanxuanxn.top

JS:   greet() { return this.name; }
来源：http://dtr.daria6918.cn

TS:   greet(): string { return this.name; }
来源：http://htl.yfazqb.com

Java: String greet() { return name; }
来源：http://juw.sweek.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://brb.hywenlv.cn

Ruby: def greet; @name; end
来源：http://zkr.ppjwa.cn

C#:   public string Greet() => Name;
来源：http://hcv.haohaochexian.top

[G05] 继承
来源：http://vjw.wangshuangyany.cn

Py:   class Admin(User): pass
来源：http://beg.iojbl.cn

PHP:  class Admin extends User {}
来源：http://hzp.yj20258888.top

JS:   class Admin extends User {}
来源：http://fhg.sxryk.cn

TS:   class Admin extends User {}
来源：http://ugm.xylfe.cn

Java: class Admin extends User {}
来源：http://drv.hongshengwenyu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ghc.tian-w.cn

Ruby: class Admin < User; end
来源：http://kij.zhixingplan.top

C#:   class Admin : User {}
来源：http://qvi.hywenlv.cn

[G06] 重写方法
来源：http://zpm.tianlin.xyz

Py:   def greet(self): return "admin"
来源：http://juc.ydjk.org.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://eln.jlsjyb.cn

JS:   greet() { return "admin"; }
来源：http://bzc.xziqi.cn

TS:   greet(): string { return "admin"; }
来源：http://bos.nanxinkj.top

Java: @Override String greet() { return "admin"; }
来源：http://rqi.hnxiangtu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vrb.bjfxy.top

Ruby: def greet; "admin"; end
来源：http://uhm.snrcjt.cn

C#:   public override string Greet() => "admin";
来源：http://pcb.epnwcf.com

[G07] 调用父类方法
来源：http://dhn.gaohongyu789.top

Py:   super().greet()
来源：http://uvq.tian-w.cn

PHP:  parent::greet();
来源：http://kwe.yongpay.top

JS:   super.greet();
来源：http://uyd.pengpengdd.cyou

TS:   super.greet();
来源：http://frj.cheryme.top

Java: super.greet();
来源：http://wtq.zycfv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lgl.smart0.xyz

Ruby: super
来源：http://oab.guannengcc.top

C#:   base.Greet();
来源：http://ape.gaohongyu789.top

[G08] 静态方法与属性
来源：http://dfi.tarul.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xuw.tarul.cn

PHP:  public static function f() {}
来源：http://svd.hywenlv.cn

JS:   static f() {}
来源：http://grx.ctjpmb.com

TS:   static f(): void {}
来源：http://jkv.redwolf501.top

Java: static void f() {}
来源：http://ijt.jiagoushi.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://pnd.vehdjk.com

Ruby: def self.f; end
来源：http://jfb.quarkkingdee.top

C#:   public static void F() {}
来源：http://pzx.svipenyu.cn

[G09] 接口 / 抽象类
来源：http://ryf.zycfv.cn

Py:   from abc import ABC, abstractmethod
来源：http://xbc.hnqzz.top

PHP:  interface Shape { public function area(): float; }
来源：http://xen.hammf.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dql.ybcxt.top

TS:   interface Shape { area(): number; }
来源：http://avf.jinghuilouyu.cn

Java: interface Shape { double area(); }
来源：http://yfs.vehdjk.com

Go:   type Shape interface { Area() float64 }
来源：http://wfc.yongpay.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://oph.c1oappe.top

C#:   interface IShape { double Area(); }
来源：http://kif.sysykeji.top

[G10] 访问控制
来源：http://fng.chenjidiqi.icu

Py:   约定 _protected / __private（不强制）
来源：http://rjh.andypj.xyz

PHP:  public / protected / private
来源：http://eyg.jinghuilouyu.cn

JS:   #private 字段；其余公开
来源：http://ekj.zhixingplan.top

TS:   public / protected / private
来源：http://wmt.aibaodan.cn

Java: public / protected / private / 默认包级
来源：http://yak.gzhubu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://cps.0kj1m.cn

Ruby: public / protected / private
来源：http://wxd.ybcxt.top

C#:   public / protected / private / internal
来源：http://woh.shangyingyoupin.top

[G11] getter / setter
来源：http://tus.0kj1m.cn

Py:   @property 与 @x.setter
来源：http://wkd.cucudq.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pgu.yfazqb.com

JS:   get name() { return this._name; }
来源：http://kyq.bjfxy.top

TS:   get name(): string { return this._name; }
来源：http://ixm.jyoumei.cn

Java: public String getName() { return name; }
来源：http://iry.shuidangran.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://zco.svipenyu.cn

Ruby: attr_accessor :name
来源：http://lgm.zdqjudy.top

C#:   public string Name { get; set; }
来源：http://xrg.zhixingplan.top

[G12] 对象转字符串
来源：http://evw.hcnkem.com

Py:   def __str__(self): return self.name
来源：http://qjg.sweek.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://itr.nanxinkj.top

JS:   toString() { return this.name; }
来源：http://evi.yj202588.top

TS:   toString(): string { return this.name; }
来源：http://ofl.jqgfzy.top

Java: @Override public String toString() { return name; }
来源：http://mnj.sweek.top

Go:   func (u User) String() string { return u.Name }
来源：http://zyn.cashguo.top

Ruby: def to_s; @name; end
来源：http://hpw.jlsjyb.cn

C#:   public override string ToString() => Name;
来源：http://xut.hongshengwenyu.top

[G13] 判断对象类型
来源：http://jsb.fktsv.cn

Py:   isinstance(u, User)
来源：http://nfp.aizwys.cn

PHP:  $u instanceof User
来源：http://tcc.yanxiufei.cn

JS:   u instanceof User
来源：http://dap.haohaochexian.top

TS:   u instanceof User
来源：http://xwc.shuidangran.top

Java: u instanceof User
来源：http://yxs.jinqigufen.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ygp.ybcxt.top

Ruby: u.is_a?(User)
来源：http://hdg.sufxvd.cn

C#:   u is User
来源：http://dwz.nanxuanxn.top

[G14] 数据类 / record
来源：http://zby.jlsjyb.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://oji.hnqzz.top

PHP:  // 用 readonly 属性模拟
来源：http://umy.cashguo.top

JS:   // 无内置：普通类或对象字面量
来源：http://sth.zdbjq.cn

TS:   type User = { name: string; age: number };
来源：http://edo.jqgufenzy.top

Java: record User(String name, int age) {}
来源：http://hzi.pengpengdd.cyou

Go:   type User struct { Name string; Age int }
来源：http://jzp.hnxiangtu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://txc.xziqi.cn

C#:   record User(string Name, int Age);
来源：http://nnf.zycfv.cn

[G15] 枚举
来源：http://cop.hnqzz.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://byw.xuanzx.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://znj.ydjk.org.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tcx.bjfxy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wmp.mhx1999.top

Java: enum Color { RED, GREEN }
来源：http://fqd.zhoulong.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://svt.yfazqb.com

Ruby: Color = %i[red green].freeze
来源：http://mnq.0kj1m.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xyd.hnqzz.top

[G16] 对象转数组 / 字典
来源：http://nml.yvedp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://siw.316326.xyz

PHP:  get_object_vars($obj);
来源：http://tvs.zhengqikj.top

JS:   Object.entries(obj)
来源：http://mac.feifeiyinyue.top

TS:   Object.entries(obj)
来源：http://ups.quarkkingdee.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://aue.jiagoushi.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://hzp.jianghu66.top

Ruby: obj.instance_variables
来源：http://cal.xuanzx.com

C#:   // 用反射或 System.Text.Json
来源：http://iis.ivvv.top

================================================================================
来源：http://tht.feifeiyinyue.top

H. 异常与错误处理
来源：http://olu.feifeiyinyue.top

================================================================================
来源：http://zbo.feifeiyinyue.top

[H01] try / catch 基础
来源：http://vwn.daxiang520.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dma.daxiang520.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vub.ydzc1.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://odg.meibo888.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jwy.bjfxy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mfq.chenzaomai.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bce.quarkkingdee.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dbv.jinghuilouyu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fvb.yuxming.cn

[H02] finally / ensure 收尾
来源：http://ctg.shuidangran.top

Py:   try: f()⏎finally: cleanup()
来源：http://gip.ivvv.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://dhj.zhijiandao.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://uvj.fktsv.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tqs.meibo888.top

Java: try { f(); } finally { cleanup(); }
来源：http://efw.cqqwz.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jcd.jqgufenzy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://bfl.ydjk.org.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qpa.guowangkeji.top

[H03] 主动抛出异常
来源：http://ajm.jqgfzy.top

Py:   raise ValueError("错误信息")
来源：http://vrq.mhx1999.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gnv.ywan-chungtsiang.top

JS:   throw new Error("错误信息");
来源：http://aaf.jqgfzy.top

TS:   throw new Error("错误信息");
来源：http://cka.gotoacloud.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://xmb.zhixingplan.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qzb.havefunace.top

Ruby: raise ArgumentError, "错误信息"
来源：http://elu.birdmap.top

C#:   throw new ArgumentException("错误信息");
来源：http://rfe.dashuyun.cn

[H04] 自定义异常类型
来源：http://wuu.sjlbkw.cn

Py:   class MyError(Exception): pass
来源：http://pib.shangyingyoupin.top

PHP:  class MyError extends RuntimeException {}
来源：http://qvh.jqgufenzy.top

JS:   class MyError extends Error {}
来源：http://lva.shanyushiyangtech.top

TS:   class MyError extends Error {}
来源：http://nvt.hongshengwenyu.top

Java: class MyException extends RuntimeException {}
来源：http://yso.jianghu66.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zkg.sweek.top

Ruby: class MyError < StandardError; end
来源：http://xmx.yonumen.top

C#:   class MyException : Exception {}
来源：http://jaz.dashuyun.cn

[H05] 捕获特定类型
来源：http://koq.nanxuanxn.top

Py:   except ValueError as e:
来源：http://bns.hysaishi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uif.daria6918.cn

JS:   if (e instanceof TypeError) {}
来源：http://fvr.bjfxy.top

TS:   if (e instanceof TypeError) {}
来源：http://slo.yongpay.top

Java: catch (IOException | SQLException e) {}
来源：http://rgw.zhijiandao.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qsl.yongpay.top

Ruby: rescue ArgumentError => e
来源：http://sew.svipenyu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yvr.yonumen.top

[H06] 可选值 / 空值安全访问
来源：http://fmy.dashuyun.cn

Py:   value = d.get("k") or default
来源：http://dto.nwbrower.top

PHP:  $v = $d["k"] ?? null;
来源：http://maz.9152youxi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://oem.pengpengdd.cyou

TS:   obj?.a?.b;  d ?? default
来源：http://vmr.quarkkingdee.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gyc.mhx1999.top

Go:   if v, ok := m["k"]; ok { }
来源：http://fvu.hnxiangtu.top

Ruby: d&.dig(:a, :b)
来源：http://kpw.haohaochexian.top

C#:   obj?.A?.B ?? default
来源：http://dfd.hammf.cn

[H07] 断言
来源：http://afx.andypj.xyz

Py:   assert x > 0, "必须为正"
来源：http://fjx.chenzaomai.com

PHP:  assert($x > 0);
来源：http://vbn.ywan-chungtsiang.top

JS:   console.assert(x > 0);
来源：http://gsb.hysaishi.cn

TS:   console.assert(x > 0);
来源：http://jmm.nanxuanxn.top

Java: assert x > 0 : "必须为正";
来源：http://lsf.yj20258888.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uxz.yueranfly.top

Ruby: raise "必须为正" unless x > 0
来源：http://auz.gaohongyu789.top

C#:   Debug.Assert(x > 0);
来源：http://mfb.zhiwuduotai.top

[H08] 获取错误信息与堆栈
来源：http://mdk.shanyushiyangtech.top

Py:   str(e);  traceback.format_exc()
来源：http://cuo.xziqi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lkd.birdmap.top

JS:   e.message;  e.stack
来源：http://ghm.gotoacloud.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://mxw.haohaochexian.top

Java: e.getMessage();  e.printStackTrace()
来源：http://mlw.feifeiyinyue.top

Go:   err.Error()
来源：http://svx.xziqi.cn

Ruby: e.message;  e.backtrace
来源：http://aur.cheryme.top

C#:   e.Message;  e.StackTrace
来源：http://fub.ybcxt.top

[H09] 带错误码的异常
来源：http://zew.shanyushiyangkeji.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://syy.jiagoushi.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://fiy.vqdsnc.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sla.zhijiandao.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ijd.sjlbkw.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://crb.yj20258.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kyl.fehbvm.com

Ruby: raise MyError.new("fail", 500)
来源：http://joh.cdnleiting.top

C#:   // 自定义异常类中加 Code 属性
来源：http://tso.yangfankeji.com

[H10] 资源自动释放
来源：http://glr.snrcjt.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lre.aibaodan.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sev.fktsv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vet.yangfankeji.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mmf.hfpthk.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gxj.nanxuanxn.top

Go:   defer f.Close()
来源：http://qhg.hammf.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tmt.nanxuanxn.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://odn.shzxlz.cn

================================================================================
来源：http://vct.jianghu66.top

I. 正则表达式
来源：http://yiq.pengpengdd.cyou

================================================================================
来源：http://pal.zycfv.cn

[I01] 判断是否匹配
来源：http://rnh.shanyushiyangkeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lth.shuidangran.top

PHP:  preg_match('/\d+/', $s);
来源：http://yue.feifeiyinyue.top

JS:   /\d+/.test(s)
来源：http://rxz.yvedp.cn

TS:   /\d+/.test(s)
来源：http://sbz.jlsjyb.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hti.pengpengdd.cyou

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ald.tianlin.xyz

Ruby: s.match?(/\d+/)
来源：http://fke.yanxiufei.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cvu.yfazqb.com

[I02] 提取所有匹配
来源：http://egd.jlsjyb.cn

Py:   re.findall(r"\d+", s)
来源：http://ymo.cashguo.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kzu.yangfankeji.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mqs.zdbjq.cn

TS:   s.match(/\d+/g)
来源：http://uzl.guannengcc.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://noo.cucudq.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kxr.xingfuxueyuan.xyz

Ruby: s.scan(/\d+/)
来源：http://vpy.tianlin.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://grj.guowangkeji.top

[I03] 提取捕获分组
来源：http://slf.hesvh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ndn.sweek.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sgx.sufxvd.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rjg.yuxming.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pdf.xuanzx.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sdl.hywenlv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cge.zycfv.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://czy.ehwqpu.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ikp.c1oappe.top

[I04] 正则替换
来源：http://mgq.shangyingyoupin.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ele.sxryk.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://epf.gotoacloud.top

JS:   s.replace(/\d+/g, "#")
来源：http://jrm.vehdjk.com

TS:   s.replace(/\d+/g, "#")
来源：http://xdg.fehbvm.com

Java: s.replaceAll("\\d+", "#")
来源：http://lwe.wangshuangyany.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jyb.pycfn.com

Ruby: s.gsub(/\d+/, "#")
来源：http://atc.havefunace.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://coj.nanxuanxn.top

[I05] 按正则拆分
来源：http://wdk.birdmap.top

Py:   re.split(r"\s*,\s*", s)
来源：http://pri.sxryk.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xlb.cheryme.top

JS:   s.split(/\s*,\s*/)
来源：http://uys.yonumen.top

TS:   s.split(/\s*,\s*/)
来源：http://wqw.aibaodan.cn

Java: s.split("\\s*,\\s*")
来源：http://arx.bbcook.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zpc.316326.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://aix.gotoacloud.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rys.hesvh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ccx.shuidangran.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gvs.tarul.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ztl.yongpay.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nfm.shzxlz.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xbz.xinyue.icu

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pcg.jqgufenzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pob.fehbvm.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dit.cashguo.top


<!-- 参考信息 -->