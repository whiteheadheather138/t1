代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ozk.zhongyouzk.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hxb.feifeiyinyue.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vwj.pengpengdd.cyou

[F12] CSV 读写
来源：http://cfl.aizwys.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://czs.hcnkem.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wnv.fengsongda.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xfe.aibaodan.cn

TS:   // 同上
来源：http://dsw.ehwqpu.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qzl.ivvv.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dzy.yonumen.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nve.ywan-chungtsiang.top

C#:   // 无内置：用 CsvHelper 库
来源：http://yai.shzxlz.cn

================================================================================
来源：http://ivy.hesvh.cn

G. 面向对象
来源：http://yan.jlsjyb.cn

================================================================================
来源：http://raa.sufxvd.cn

[G01] 定义类
来源：http://xzf.xuetiantiany.cn

Py:   class User: pass
来源：http://fdm.gotoacloud.top

PHP:  class User {}
来源：http://zui.xuanzx.com

JS:   class User {}
来源：http://fxg.cdnleiting.top

TS:   class User { name: string = ""; }
来源：http://lpk.shanyushiyangkeji.top

Java: class User {}
来源：http://stj.yvedp.cn

Go:   type User struct { Name string }
来源：http://wjg.gzhubu.top

Ruby: class User; end
来源：http://qgm.jlsjyb.cn

C#:   class User {}
来源：http://bdc.yanxiufei.cn

[G02] 构造函数
来源：http://ogd.sjlbkw.cn

Py:   def __init__(self, name): self.name = name
来源：http://ozx.chenzaomai.com

PHP:  public function __construct(public string $name) {}
来源：http://cil.zhoulong.xyz

JS:   constructor(name) { this.name = name; }
来源：http://mkx.zhongyouzk.top

TS:   constructor(public name: string) {}
来源：http://ajr.daria6918.cn

Java: User(String name) { this.name = name; }
来源：http://lmx.dashuyun.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vya.haohaochexian.top

Ruby: def initialize(name); @name = name; end
来源：http://oax.zdqjudy.top

C#:   public User(string name) { Name = name; }
来源：http://kox.hnxiangtu.top

[G03] 实例属性
来源：http://flc.cucudq.cn

Py:   self.name = "x"
来源：http://ndi.fzhhl.top

PHP:  public string $name = "x";
来源：http://aap.nwbrower.top

JS:   this.name = "x";
来源：http://otv.hcnkem.com

TS:   name: string = "x";
来源：http://qqg.shanyushiyangkeji.top

Java: private String name;
来源：http://mmi.ctjpmb.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jtm.jqgfzy.top

Ruby: @name = "x"
来源：http://lhh.xinyue.icu

C#:   public string Name { get; set; } = "x";
来源：http://rqq.yj20258.top

[G04] 定义方法
来源：http://rrg.xingfuxueyuan.xyz

Py:   def greet(self): return self.name
来源：http://fjk.yj20258888.top

PHP:  public function greet(): string { return $this->name; }
来源：http://vle.epnwcf.com

JS:   greet() { return this.name; }
来源：http://tqi.hongshengwenyu.top

TS:   greet(): string { return this.name; }
来源：http://yof.daria6918.cn

Java: String greet() { return name; }
来源：http://rbd.daria6918.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bru.gogol.net.cn

Ruby: def greet; @name; end
来源：http://tnf.zhiwuduotai.top

C#:   public string Greet() => Name;
来源：http://vcd.redwolf501.top

[G05] 继承
来源：http://sjx.snrcjt.cn

Py:   class Admin(User): pass
来源：http://ixk.hnqzz.top

PHP:  class Admin extends User {}
来源：http://nmq.cashguo.top

JS:   class Admin extends User {}
来源：http://bsh.aizwys.cn

TS:   class Admin extends User {}
来源：http://kuh.zhaomingkeji.xyz

Java: class Admin extends User {}
来源：http://wwv.zhongyouzk.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nij.uphjek.com

Ruby: class Admin < User; end
来源：http://nak.jqgfzy.top

C#:   class Admin : User {}
来源：http://bgh.9152youxi.cn

[G06] 重写方法
来源：http://snc.yonumen.top

Py:   def greet(self): return "admin"
来源：http://jee.yangfankeji.com

PHP:  public function greet(): string { return "admin"; }
来源：http://znt.redwolf501.top

JS:   greet() { return "admin"; }
来源：http://qty.yj202588.top

TS:   greet(): string { return "admin"; }
来源：http://ipm.xuanzx.com

Java: @Override String greet() { return "admin"; }
来源：http://wzr.daria6918.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://eyw.xziqi.cn

Ruby: def greet; "admin"; end
来源：http://uqr.jinqigufen.top

C#:   public override string Greet() => "admin";
来源：http://gzm.gotoacloud.top

[G07] 调用父类方法
来源：http://xlw.zdqjudy.top

Py:   super().greet()
来源：http://nld.xylfe.cn

PHP:  parent::greet();
来源：http://ggt.yj20258888.top

JS:   super.greet();
来源：http://gyu.ydzc1.top

TS:   super.greet();
来源：http://ken.jinqigfzy.top

Java: super.greet();
来源：http://juc.hongshengwenyu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://eqx.yj20258.top

Ruby: super
来源：http://qes.jinqigufen.top

C#:   base.Greet();
来源：http://kja.zhengqikj.top

[G08] 静态方法与属性
来源：http://vbv.ywan-chungtsiang.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mtu.tianlin.xyz

PHP:  public static function f() {}
来源：http://czi.ywan-chungtsiang.top

JS:   static f() {}
来源：http://iek.jiagoushi.top

TS:   static f(): void {}
来源：http://ihu.jlsjyb.cn

Java: static void f() {}
来源：http://nsf.quarkkingdee.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://mqr.shangyingyoupin.top

Ruby: def self.f; end
来源：http://ysj.uphjek.com

C#:   public static void F() {}
来源：http://jsh.hammf.cn

[G09] 接口 / 抽象类
来源：http://ehw.bbcook.cn

Py:   from abc import ABC, abstractmethod
来源：http://cpx.gzhubu.top

PHP:  interface Shape { public function area(): float; }
来源：http://bfi.jlsjyb.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ott.birdmap.top

TS:   interface Shape { area(): number; }
来源：http://olz.gaohongyu789.top

Java: interface Shape { double area(); }
来源：http://blt.hywenlv.cn

Go:   type Shape interface { Area() float64 }
来源：http://rzx.wangshuangyany.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ajp.tarul.cn

C#:   interface IShape { double Area(); }
来源：http://xxb.hammf.cn

[G10] 访问控制
来源：http://hpn.smart0.xyz

Py:   约定 _protected / __private（不强制）
来源：http://eok.c1oappe.top

PHP:  public / protected / private
来源：http://cqn.yangfankeji.com

JS:   #private 字段；其余公开
来源：http://pzc.ivvv.top

TS:   public / protected / private
来源：http://rty.nanxuanxn.top

Java: public / protected / private / 默认包级
来源：http://rmc.sweek.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://cgn.316326.xyz

Ruby: public / protected / private
来源：http://zid.fanxiaobao.xyz

C#:   public / protected / private / internal
来源：http://gbg.xziqi.cn

[G11] getter / setter
来源：http://ies.zhixingplan.top

Py:   @property 与 @x.setter
来源：http://ciu.sweek.top

PHP:  public function getName(): string { return $this->name; }
来源：http://uaq.ppjwa.cn

JS:   get name() { return this._name; }
来源：http://zld.cashguo.top

TS:   get name(): string { return this._name; }
来源：http://ahp.jyoumei.cn

Java: public String getName() { return name; }
来源：http://vin.hfpthk.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://noy.smart0.xyz

Ruby: attr_accessor :name
来源：http://ged.fktsv.cn

C#:   public string Name { get; set; }
来源：http://who.vehdjk.com

[G12] 对象转字符串
来源：http://cfu.yangfankeji.com

Py:   def __str__(self): return self.name
来源：http://qqk.shzxlz.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xoh.hfpthk.cn

JS:   toString() { return this.name; }
来源：http://szo.cheryme.top

TS:   toString(): string { return this.name; }
来源：http://uzm.ehwqpu.com

Java: @Override public String toString() { return name; }
来源：http://gdg.haohaochexian.top

Go:   func (u User) String() string { return u.Name }
来源：http://ivw.guannengcc.top

Ruby: def to_s; @name; end
来源：http://hjb.redwolf501.top

C#:   public override string ToString() => Name;
来源：http://mdv.gzhubu.top

[G13] 判断对象类型
来源：http://ffv.xziqi.cn

Py:   isinstance(u, User)
来源：http://dng.nanxinkj.top

PHP:  $u instanceof User
来源：http://xee.sysykeji.top

JS:   u instanceof User
来源：http://ejz.shzxlz.cn

TS:   u instanceof User
来源：http://poq.jinqigfzy.top

Java: u instanceof User
来源：http://uwk.fehbvm.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://ffo.chenlongwang.top

Ruby: u.is_a?(User)
来源：http://rxq.chenzaomai.com

C#:   u is User
来源：http://rsq.yvedp.cn

[G14] 数据类 / record
来源：http://jri.jlsjyb.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yrz.xinyue.icu

PHP:  // 用 readonly 属性模拟
来源：http://lqb.vehdjk.com

JS:   // 无内置：普通类或对象字面量
来源：http://tcp.yueranfly.top

TS:   type User = { name: string; age: number };
来源：http://qpu.yj202588.top

Java: record User(String name, int age) {}
来源：http://zjo.gotoacloud.top

Go:   type User struct { Name string; Age int }
来源：http://urs.sxryk.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gop.bbcook.cn

C#:   record User(string Name, int Age);
来源：http://atn.ppjwa.cn

[G15] 枚举
来源：http://txa.316326.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gwg.xylfe.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://tgu.hongshengwenyu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tht.tian-w.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dse.shangyingyoupin.top

Java: enum Color { RED, GREEN }
来源：http://wor.yonumen.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cdl.xingfuxueyuan.xyz

Ruby: Color = %i[red green].freeze
来源：http://tgp.fengsongda.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iao.9152youxi.cn

[G16] 对象转数组 / 字典
来源：http://xyw.yuxming.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jue.gaohongyu789.top

PHP:  get_object_vars($obj);
来源：http://sbg.zdbjq.cn

JS:   Object.entries(obj)
来源：http://zmz.zhoulong.xyz

TS:   Object.entries(obj)
来源：http://xih.snrcjt.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://klr.tarul.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jut.zdbjq.cn

Ruby: obj.instance_variables
来源：http://nke.sweek.top

C#:   // 用反射或 System.Text.Json
来源：http://sdi.sysykeji.top

================================================================================
来源：http://usp.zhengqikj.top

H. 异常与错误处理
来源：http://uzh.pycfn.com

================================================================================
来源：http://uuo.guowangkeji.top

[H01] try / catch 基础
来源：http://rwp.ivvv.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gfv.redwolf501.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vqw.gogol.net.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mpf.jqgufenzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nmg.nanxinkj.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://alv.zhiwuduotai.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pno.cheryme.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gzo.tian-w.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://soz.shzxlz.cn

[H02] finally / ensure 收尾
来源：http://gxn.gotoacloud.top

Py:   try: f()⏎finally: cleanup()
来源：http://mut.52xcode.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yrj.guannengcc.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ikr.yfazqb.com

TS:   try { f(); } finally { cleanup(); }
来源：http://uaa.hcnkem.com

Java: try { f(); } finally { cleanup(); }
来源：http://uvy.jlsjyb.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://yvo.sweek.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ghx.quarkkingdee.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ihe.gaohongyu789.top

[H03] 主动抛出异常
来源：http://gys.jiagoushi.top

Py:   raise ValueError("错误信息")
来源：http://ouk.hammf.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bdi.yj202588.top

JS:   throw new Error("错误信息");
来源：http://ypu.zhiwuduotai.top

TS:   throw new Error("错误信息");
来源：http://hqf.yanxiufei.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bib.chenjidiqi.icu

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fbx.bjfxy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ubx.yj20258.top

C#:   throw new ArgumentException("错误信息");
来源：http://mom.ehwqpu.com

[H04] 自定义异常类型
来源：http://kre.tarul.cn

Py:   class MyError(Exception): pass
来源：http://jmt.gogol.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cmh.cqqwz.cn

JS:   class MyError extends Error {}
来源：http://exb.xziqi.cn

TS:   class MyError extends Error {}
来源：http://rxx.jiagoushi.top

Java: class MyException extends RuntimeException {}
来源：http://jdo.mhx1999.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vjm.sjlbkw.cn

Ruby: class MyError < StandardError; end
来源：http://rit.hnqzz.top

C#:   class MyException : Exception {}
来源：http://mqh.sxryk.cn

[H05] 捕获特定类型
来源：http://nat.pengpengdd.cyou

Py:   except ValueError as e:
来源：http://hln.yj20258.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://djt.jinghuilouyu.cn

JS:   if (e instanceof TypeError) {}
来源：http://jfo.zhixingplan.top

TS:   if (e instanceof TypeError) {}
来源：http://pgf.ybcxt.top

Java: catch (IOException | SQLException e) {}
来源：http://gmc.hywenlv.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://erw.ywan-chungtsiang.top

Ruby: rescue ArgumentError => e
来源：http://mka.aizwys.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hza.vqdsnc.cn

[H06] 可选值 / 空值安全访问
来源：http://chh.xuanzx.com

Py:   value = d.get("k") or default
来源：http://fka.feifeiyinyue.top

PHP:  $v = $d["k"] ?? null;
来源：http://vtz.ehwqpu.com

JS:   obj?.a?.b;  d ?? default
来源：http://rlk.yj20258888.top

TS:   obj?.a?.b;  d ?? default
来源：http://cvc.cucudq.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lew.gaohongyu789.top

Go:   if v, ok := m["k"]; ok { }
来源：http://pxx.fengsongda.top

Ruby: d&.dig(:a, :b)
来源：http://vsh.epnwcf.com

C#:   obj?.A?.B ?? default
来源：http://aui.jiagoushi.top

[H07] 断言
来源：http://gxa.aibaodan.cn

Py:   assert x > 0, "必须为正"
来源：http://xwq.xziqi.cn

PHP:  assert($x > 0);
来源：http://fam.ywan-chungtsiang.top

JS:   console.assert(x > 0);
来源：http://lln.xuetiantiany.cn

TS:   console.assert(x > 0);
来源：http://hdj.epnwcf.com

Java: assert x > 0 : "必须为正";
来源：http://adq.bbcook.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cxf.xylfe.cn

Ruby: raise "必须为正" unless x > 0
来源：http://pfy.cqqwz.cn

C#:   Debug.Assert(x > 0);
来源：http://ujd.shangyingyoupin.top

[H08] 获取错误信息与堆栈
来源：http://ysa.tanke756.top

Py:   str(e);  traceback.format_exc()
来源：http://imv.jinqigufen.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://igi.hongshengwenyu.top

JS:   e.message;  e.stack
来源：http://mkz.cdnleiting.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://aio.jianghu66.top

Java: e.getMessage();  e.printStackTrace()
来源：http://yfs.zhixingplan.top

Go:   err.Error()
来源：http://gdg.fehbvm.com

Ruby: e.message;  e.backtrace
来源：http://tnd.sufxvd.cn

C#:   e.Message;  e.StackTrace
来源：http://nvb.sufxvd.cn

[H09] 带错误码的异常
来源：http://ibd.chenzaomai.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xlh.guannengcc.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://wtw.yangfankeji.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ukk.hywenlv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lyj.vehdjk.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ixb.jianghu66.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rom.smart0.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://zds.quarkkingdee.top

C#:   // 自定义异常类中加 Code 属性
来源：http://aat.hnxiangtu.top

[H10] 资源自动释放
来源：http://fah.dashuyun.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zlc.zhiwuduotai.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rqc.epnwcf.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tlu.shuidangran.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://djh.yueranfly.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sxu.nanxinkj.top

Go:   defer f.Close()
来源：http://amt.tarul.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gvj.zhixingplan.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jpw.haohaochexian.top

================================================================================
来源：http://kwq.0kj1m.cn

I. 正则表达式
来源：http://sbk.yanxiufei.cn

================================================================================
来源：http://dlf.yueranfly.top

[I01] 判断是否匹配
来源：http://ges.vqdsnc.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gye.ywan-chungtsiang.top

PHP:  preg_match('/\d+/', $s);
来源：http://ubf.birdmap.top

JS:   /\d+/.test(s)
来源：http://wzc.xuetiantiany.cn

TS:   /\d+/.test(s)
来源：http://kry.guannengcc.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wzc.tianlin.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ded.mhx1999.top

Ruby: s.match?(/\d+/)
来源：http://jml.hywenlv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ukc.yongpay.top

[I02] 提取所有匹配
来源：http://koq.wangshuangyany.cn

Py:   re.findall(r"\d+", s)
来源：http://xay.andypj.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zvv.uphjek.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vco.nanxinkj.top

TS:   s.match(/\d+/g)
来源：http://ipx.yfazqb.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://brn.iojbl.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tzl.hysaishi.cn

Ruby: s.scan(/\d+/)
来源：http://erx.jinyuanbaomall.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vuc.hammf.cn

[I03] 提取捕获分组
来源：http://kcw.cqqwz.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qnh.jinyuanbaomall.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ojb.ybcxt.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qfg.yangfankeji.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cbf.yonumen.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tyo.tanke756.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hzo.jinqigfzy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://exw.shanyushiyangkeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bcw.hesvh.cn

[I04] 正则替换
来源：http://byn.cheryme.top

Py:   re.sub(r"\d+", "#", s)
来源：http://yqw.jinqigfzy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mgn.zhengqikj.top

JS:   s.replace(/\d+/g, "#")
来源：http://hwe.chenlongwang.top

TS:   s.replace(/\d+/g, "#")
来源：http://bkl.sysykeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://zfv.zhoulong.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://dar.mhx1999.top

Ruby: s.gsub(/\d+/, "#")
来源：http://nvc.0kj1m.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dwg.jiagoushi.top

[I05] 按正则拆分
来源：http://pfm.hesvh.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ywz.aibaodan.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vhz.ydjk.org.cn

JS:   s.split(/\s*,\s*/)
来源：http://cgb.xuetiantiany.cn

TS:   s.split(/\s*,\s*/)
来源：http://hyp.yueranfly.top

Java: s.split("\\s*,\\s*")
来源：http://yjd.jyoumei.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gcj.fzhhl.top

Ruby: s.split(/\s*,\s*/)
来源：http://qfz.fktsv.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sen.wangdashe.top


<!-- 参考信息 -->