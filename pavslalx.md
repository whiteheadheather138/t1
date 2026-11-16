代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qsq.yj202588.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dcs.tanke756.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jgx.yj20258.top

TS:   // 同上
来源：http://trd.feifeiyinyue.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yxk.hnxiangtu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ldt.hywenlv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kre.chenzaomai.com

C#:   // 无内置：用 CsvHelper 库
来源：http://utl.fzhhl.top

================================================================================
来源：http://cbu.zhongyouzk.top

G. 面向对象
来源：http://sps.0kj1m.cn

================================================================================
来源：http://iye.iojbl.cn

[G01] 定义类
来源：http://ivw.yongpay.top

Py:   class User: pass
来源：http://zsn.daria6918.cn

PHP:  class User {}
来源：http://qos.mhx1999.top

JS:   class User {}
来源：http://tdc.wangshuangyany.cn

TS:   class User { name: string = ""; }
来源：http://ueg.yj202588.top

Java: class User {}
来源：http://fol.ivvv.top

Go:   type User struct { Name string }
来源：http://xoo.wangshuangyany.cn

Ruby: class User; end
来源：http://tht.jlsjyb.cn

C#:   class User {}
来源：http://mli.xinyue.icu

[G02] 构造函数
来源：http://xqf.fktsv.cn

Py:   def __init__(self, name): self.name = name
来源：http://sbf.hnqzz.top

PHP:  public function __construct(public string $name) {}
来源：http://ifb.jinqigfzy.top

JS:   constructor(name) { this.name = name; }
来源：http://mnw.fanxiaobao.xyz

TS:   constructor(public name: string) {}
来源：http://amw.kuanghao11.cn

Java: User(String name) { this.name = name; }
来源：http://qhj.gogol.net.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ljx.feifeiyinyue.top

Ruby: def initialize(name); @name = name; end
来源：http://sky.0kj1m.cn

C#:   public User(string name) { Name = name; }
来源：http://yrs.cqqwz.cn

[G03] 实例属性
来源：http://ohw.epnwcf.com

Py:   self.name = "x"
来源：http://uyz.jinyuanbaomall.cn

PHP:  public string $name = "x";
来源：http://nge.dashuyun.cn

JS:   this.name = "x";
来源：http://bqs.dianchejie.cn

TS:   name: string = "x";
来源：http://twg.hnqzz.top

Java: private String name;
来源：http://skk.ivvv.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rnw.pycfn.com

Ruby: @name = "x"
来源：http://wvy.hongshengwenyu.top

C#:   public string Name { get; set; } = "x";
来源：http://oax.ivvv.top

[G04] 定义方法
来源：http://rfh.sysykeji.top

Py:   def greet(self): return self.name
来源：http://sou.yj20258888.top

PHP:  public function greet(): string { return $this->name; }
来源：http://bip.hfpthk.cn

JS:   greet() { return this.name; }
来源：http://hyr.c1oappe.top

TS:   greet(): string { return this.name; }
来源：http://yaw.jianghu66.top

Java: String greet() { return name; }
来源：http://tse.jinqigfzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://zav.zhiwuduotai.top

Ruby: def greet; @name; end
来源：http://enm.fzhhl.top

C#:   public string Greet() => Name;
来源：http://vzt.xuetiantiany.cn

[G05] 继承
来源：http://hkw.yvedp.cn

Py:   class Admin(User): pass
来源：http://vzk.zhiwuduotai.top

PHP:  class Admin extends User {}
来源：http://mnp.hfpthk.cn

JS:   class Admin extends User {}
来源：http://boc.bbcook.cn

TS:   class Admin extends User {}
来源：http://qea.ppjwa.cn

Java: class Admin extends User {}
来源：http://jgv.hysaishi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://isb.c1oappe.top

Ruby: class Admin < User; end
来源：http://kth.ehwqpu.com

C#:   class Admin : User {}
来源：http://jap.tian-w.cn

[G06] 重写方法
来源：http://lmm.zhiwuduotai.top

Py:   def greet(self): return "admin"
来源：http://hwa.gotoacloud.top

PHP:  public function greet(): string { return "admin"; }
来源：http://uon.chenzaomai.com

JS:   greet() { return "admin"; }
来源：http://jgs.birdmap.top

TS:   greet(): string { return "admin"; }
来源：http://ejn.zhaomingkeji.xyz

Java: @Override String greet() { return "admin"; }
来源：http://kfq.shuidangran.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://iij.hesvh.cn

Ruby: def greet; "admin"; end
来源：http://wka.iojbl.cn

C#:   public override string Greet() => "admin";
来源：http://tlf.snrcjt.cn

[G07] 调用父类方法
来源：http://vsg.sweek.top

Py:   super().greet()
来源：http://asi.snrcjt.cn

PHP:  parent::greet();
来源：http://mja.zdbjq.cn

JS:   super.greet();
来源：http://woz.tanke756.top

TS:   super.greet();
来源：http://cmo.hnxiangtu.top

Java: super.greet();
来源：http://kci.sweek.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pwa.yuanzhike.top

Ruby: super
来源：http://ebz.sjlbkw.cn

C#:   base.Greet();
来源：http://ful.smart0.xyz

[G08] 静态方法与属性
来源：http://ygw.gaohongyu789.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qgw.zhongyouzk.top

PHP:  public static function f() {}
来源：http://pud.yanxiufei.cn

JS:   static f() {}
来源：http://yni.tanke756.top

TS:   static f(): void {}
来源：http://sig.shuidangran.top

Java: static void f() {}
来源：http://wbt.zhongyouzk.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ffx.chenlongwang.top

Ruby: def self.f; end
来源：http://gwm.xylfe.cn

C#:   public static void F() {}
来源：http://oyd.fengsongda.top

[G09] 接口 / 抽象类
来源：http://xfw.zdqjudy.top

Py:   from abc import ABC, abstractmethod
来源：http://lbn.hcnkem.com

PHP:  interface Shape { public function area(): float; }
来源：http://yaw.wangshuangyany.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lqt.hesvh.cn

TS:   interface Shape { area(): number; }
来源：http://rye.52xcode.cn

Java: interface Shape { double area(); }
来源：http://vqy.jinyuanbaomall.cn

Go:   type Shape interface { Area() float64 }
来源：http://lwr.zhengqikj.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vzg.guannengcc.top

C#:   interface IShape { double Area(); }
来源：http://dck.jqgufenzy.top

[G10] 访问控制
来源：http://hha.jianghu66.top

Py:   约定 _protected / __private（不强制）
来源：http://wit.cqqwz.cn

PHP:  public / protected / private
来源：http://baz.ehwqpu.com

JS:   #private 字段；其余公开
来源：http://jfs.yj20258888.top

TS:   public / protected / private
来源：http://hem.ydjk.org.cn

Java: public / protected / private / 默认包级
来源：http://tjl.zhongyouzk.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://eab.tarul.cn

Ruby: public / protected / private
来源：http://qhh.hnxiangtu.top

C#:   public / protected / private / internal
来源：http://ala.cashguo.top

[G11] getter / setter
来源：http://yaz.jyoumei.cn

Py:   @property 与 @x.setter
来源：http://oqq.tanke756.top

PHP:  public function getName(): string { return $this->name; }
来源：http://faj.hnqzz.top

JS:   get name() { return this._name; }
来源：http://tzi.gaohongyu789.top

TS:   get name(): string { return this._name; }
来源：http://zib.xuetiantiany.cn

Java: public String getName() { return name; }
来源：http://paq.quarkkingdee.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://zqi.shzxlz.cn

Ruby: attr_accessor :name
来源：http://lgw.aizwys.cn

C#:   public string Name { get; set; }
来源：http://kgg.jiagoushi.top

[G12] 对象转字符串
来源：http://gqo.dianchejie.cn

Py:   def __str__(self): return self.name
来源：http://lbr.fktsv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rrz.redwolf501.top

JS:   toString() { return this.name; }
来源：http://fyd.gzhubu.top

TS:   toString(): string { return this.name; }
来源：http://kqi.dianchejie.cn

Java: @Override public String toString() { return name; }
来源：http://iwj.hywenlv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://keq.jinqigfzy.top

Ruby: def to_s; @name; end
来源：http://lum.guowangkeji.top

C#:   public override string ToString() => Name;
来源：http://czu.yanxiufei.cn

[G13] 判断对象类型
来源：http://iyg.sxryk.cn

Py:   isinstance(u, User)
来源：http://kgv.jqgfzy.top

PHP:  $u instanceof User
来源：http://wzr.tianlin.xyz

JS:   u instanceof User
来源：http://tqf.ydjk.org.cn

TS:   u instanceof User
来源：http://pqx.hesvh.cn

Java: u instanceof User
来源：http://ona.gogol.net.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nxc.smart0.xyz

Ruby: u.is_a?(User)
来源：http://mkz.feifeiyinyue.top

C#:   u is User
来源：http://zhl.gaohongyu789.top

[G14] 数据类 / record
来源：http://chd.smart0.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pmr.shanyushiyangtech.top

PHP:  // 用 readonly 属性模拟
来源：http://jra.tarul.cn

JS:   // 无内置：普通类或对象字面量
来源：http://arg.quarkkingdee.top

TS:   type User = { name: string; age: number };
来源：http://btf.tarul.cn

Java: record User(String name, int age) {}
来源：http://opb.hongshengwenyu.top

Go:   type User struct { Name string; Age int }
来源：http://jqj.gotoacloud.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://krr.iojbl.cn

C#:   record User(string Name, int Age);
来源：http://gyg.kuanghao11.cn

[G15] 枚举
来源：http://lps.chenlongwang.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jcr.shanyushiyangkeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://mez.tianlin.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hzr.zhongyouzk.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cww.havefunace.top

Java: enum Color { RED, GREEN }
来源：http://sik.nanxinkj.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://odz.chenzaomai.com

Ruby: Color = %i[red green].freeze
来源：http://wxp.zhongyouzk.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dpr.daxiang520.top

[G16] 对象转数组 / 字典
来源：http://vwi.cdnleiting.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jio.yongpay.top

PHP:  get_object_vars($obj);
来源：http://vvv.yj202588.top

JS:   Object.entries(obj)
来源：http://fad.yvedp.cn

TS:   Object.entries(obj)
来源：http://tzp.hnxiangtu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vci.yj20258888.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://aar.sxryk.cn

Ruby: obj.instance_variables
来源：http://hom.tarul.cn

C#:   // 用反射或 System.Text.Json
来源：http://dmg.hywenlv.cn

================================================================================
来源：http://qnj.shanyushiyangkeji.top

H. 异常与错误处理
来源：http://xse.yuxming.cn

================================================================================
来源：http://ief.jinyuanbaomall.cn

[H01] try / catch 基础
来源：http://wxd.xuanzx.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lyb.vqdsnc.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ypn.ydjk.org.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mlp.havefunace.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tvh.fanxiaobao.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fmi.epnwcf.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tvn.xinyue.icu

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rrv.zdqjudy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ogy.fehbvm.com

[H02] finally / ensure 收尾
来源：http://cgb.jinyuanbaomall.cn

Py:   try: f()⏎finally: cleanup()
来源：http://drg.zdqjudy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://zrm.gogol.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fks.andypj.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://jna.yj20258.top

Java: try { f(); } finally { cleanup(); }
来源：http://cgl.haohaochexian.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://vts.hnxiangtu.top

Ruby: begin; f; ensure; cleanup; end
来源：http://zjt.cashguo.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://wbo.jyoumei.cn

[H03] 主动抛出异常
来源：http://yij.52xcode.cn

Py:   raise ValueError("错误信息")
来源：http://abu.birdmap.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bds.xingfuxueyuan.xyz

JS:   throw new Error("错误信息");
来源：http://jkm.ywan-chungtsiang.top

TS:   throw new Error("错误信息");
来源：http://pjl.daxiang520.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://yfv.ehwqpu.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yly.yueranfly.top

Ruby: raise ArgumentError, "错误信息"
来源：http://rod.daxiang520.top

C#:   throw new ArgumentException("错误信息");
来源：http://mxf.zhiwuduotai.top

[H04] 自定义异常类型
来源：http://dwn.jqgufenzy.top

Py:   class MyError(Exception): pass
来源：http://mbl.havefunace.top

PHP:  class MyError extends RuntimeException {}
来源：http://lvv.zhijiandao.cn

JS:   class MyError extends Error {}
来源：http://xgf.yvedp.cn

TS:   class MyError extends Error {}
来源：http://xro.aibaodan.cn

Java: class MyException extends RuntimeException {}
来源：http://lxf.nanxinkj.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://srs.dianchejie.cn

Ruby: class MyError < StandardError; end
来源：http://yhc.shanyushiyangtech.top

C#:   class MyException : Exception {}
来源：http://nxl.wangdashe.top

[H05] 捕获特定类型
来源：http://zdk.sweek.top

Py:   except ValueError as e:
来源：http://cvy.yueranfly.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zls.dashuyun.cn

JS:   if (e instanceof TypeError) {}
来源：http://rer.9152youxi.cn

TS:   if (e instanceof TypeError) {}
来源：http://pvl.ydzc1.top

Java: catch (IOException | SQLException e) {}
来源：http://yfo.smart0.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hda.sufxvd.cn

Ruby: rescue ArgumentError => e
来源：http://ycn.redwolf501.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dnc.0kj1m.cn

[H06] 可选值 / 空值安全访问
来源：http://vqi.quarkkingdee.top

Py:   value = d.get("k") or default
来源：http://feo.sysykeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://mlr.tanke756.top

JS:   obj?.a?.b;  d ?? default
来源：http://qpc.tianlin.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://iwm.wangshuangyany.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ncn.haohaochexian.top

Go:   if v, ok := m["k"]; ok { }
来源：http://lsa.hcnkem.com

Ruby: d&.dig(:a, :b)
来源：http://rsf.pycfn.com

C#:   obj?.A?.B ?? default
来源：http://swd.hnxiangtu.top

[H07] 断言
来源：http://oto.aizwys.cn

Py:   assert x > 0, "必须为正"
来源：http://bos.hongshengwenyu.top

PHP:  assert($x > 0);
来源：http://ezh.tarul.cn

JS:   console.assert(x > 0);
来源：http://zaa.9152youxi.cn

TS:   console.assert(x > 0);
来源：http://kuy.yuanzhike.top

Java: assert x > 0 : "必须为正";
来源：http://pxr.sjlbkw.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://epe.aibaodan.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ldj.guannengcc.top

C#:   Debug.Assert(x > 0);
来源：http://drb.cucudq.cn

[H08] 获取错误信息与堆栈
来源：http://qcv.daria6918.cn

Py:   str(e);  traceback.format_exc()
来源：http://dyn.jinqigfzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ueh.andypj.xyz

JS:   e.message;  e.stack
来源：http://hds.birdmap.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ako.jinyuanbaomall.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://yke.tianlin.xyz

Go:   err.Error()
来源：http://lsx.redwolf501.top

Ruby: e.message;  e.backtrace
来源：http://blu.zycfv.cn

C#:   e.Message;  e.StackTrace
来源：http://ajw.zhoulong.xyz

[H09] 带错误码的异常
来源：http://gpg.jlsjyb.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vky.quarkkingdee.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://kxh.uphjek.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://swg.gaohongyu789.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zuv.ehwqpu.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://drj.birdmap.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ylz.yj20258888.top

Ruby: raise MyError.new("fail", 500)
来源：http://uky.chenlongwang.top

C#:   // 自定义异常类中加 Code 属性
来源：http://qcy.yuxming.cn

[H10] 资源自动释放
来源：http://yyd.shangyingyoupin.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ldi.guowangkeji.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qmv.sufxvd.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hde.cashguo.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pho.ywan-chungtsiang.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lxw.cqqwz.cn

Go:   defer f.Close()
来源：http://tpf.c1oappe.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yod.ivvv.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hkl.shuidangran.top

================================================================================
来源：http://mue.xinyue.icu

I. 正则表达式
来源：http://gin.smart0.xyz

================================================================================
来源：http://wla.vehdjk.com

[I01] 判断是否匹配
来源：http://iho.ydjk.org.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://usf.zdqjudy.top

PHP:  preg_match('/\d+/', $s);
来源：http://zym.jinyuanbaomall.cn

JS:   /\d+/.test(s)
来源：http://uod.hfpthk.cn

TS:   /\d+/.test(s)
来源：http://tif.daria6918.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://iyy.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kyj.sysykeji.top

Ruby: s.match?(/\d+/)
来源：http://ykk.sxryk.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wyv.shuidangran.top

[I02] 提取所有匹配
来源：http://shl.fktsv.cn

Py:   re.findall(r"\d+", s)
来源：http://nnq.gaohongyu789.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vty.316326.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mhj.feifeiyinyue.top

TS:   s.match(/\d+/g)
来源：http://jht.haohaochexian.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rtq.hesvh.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mcs.aibaodan.cn

Ruby: s.scan(/\d+/)
来源：http://zen.shanyushiyangtech.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xns.hcnkem.com

[I03] 提取捕获分组
来源：http://bim.cucudq.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ddm.c1oappe.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gxr.hammf.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://agx.xuetiantiany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wsc.gaohongyu789.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xdi.wangdashe.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mzf.cucudq.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jjo.daria6918.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hlr.nwbrower.top

[I04] 正则替换
来源：http://iqs.ybcxt.top

Py:   re.sub(r"\d+", "#", s)
来源：http://izy.52xcode.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://reh.meibo888.top

JS:   s.replace(/\d+/g, "#")
来源：http://cxn.uphjek.com

TS:   s.replace(/\d+/g, "#")
来源：http://orl.fehbvm.com

Java: s.replaceAll("\\d+", "#")
来源：http://onj.hnqzz.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ovz.ybcxt.top

Ruby: s.gsub(/\d+/, "#")
来源：http://okn.vqdsnc.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://klw.zycfv.cn

[I05] 按正则拆分
来源：http://nzg.zhongyouzk.top

Py:   re.split(r"\s*,\s*", s)
来源：http://tpm.hfpthk.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://htw.sweek.top

JS:   s.split(/\s*,\s*/)
来源：http://tai.hfpthk.cn

TS:   s.split(/\s*,\s*/)
来源：http://icz.hammf.cn

Java: s.split("\\s*,\\s*")
来源：http://rbq.jqgfzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fth.pycfn.com

Ruby: s.split(/\s*,\s*/)
来源：http://xpj.shzxlz.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lrn.hysaishi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dtf.fengsongda.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dcz.daxiang520.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qnk.jiagoushi.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yvh.tanke756.top


<!-- 参考信息 -->