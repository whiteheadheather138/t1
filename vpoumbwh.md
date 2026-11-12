代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://idc.zhijiandao.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vrt.zhaomingkeji.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qpd.ybcxt.top

[F12] CSV 读写
来源：http://vyg.birdmap.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xzm.yj20258.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gmd.jiagoushi.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jzd.zhoulong.xyz

TS:   // 同上
来源：http://uhv.zhixingplan.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xni.yueranfly.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hto.redwolf501.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mkv.nwbrower.top

C#:   // 无内置：用 CsvHelper 库
来源：http://wes.jinghuilouyu.cn

================================================================================
来源：http://vuo.iojbl.cn

G. 面向对象
来源：http://uyo.daria6918.cn

================================================================================
来源：http://fjn.hongshengwenyu.top

[G01] 定义类
来源：http://gif.xinyue.icu

Py:   class User: pass
来源：http://jkx.hfpthk.cn

PHP:  class User {}
来源：http://hji.daria6918.cn

JS:   class User {}
来源：http://qzw.ydjk.org.cn

TS:   class User { name: string = ""; }
来源：http://umn.gaohongyu789.top

Java: class User {}
来源：http://onw.nwbrower.top

Go:   type User struct { Name string }
来源：http://hws.kuanghao11.cn

Ruby: class User; end
来源：http://leb.svipenyu.cn

C#:   class User {}
来源：http://xny.hongshengwenyu.top

[G02] 构造函数
来源：http://vqn.aizwys.cn

Py:   def __init__(self, name): self.name = name
来源：http://cyo.ybcxt.top

PHP:  public function __construct(public string $name) {}
来源：http://zve.tarul.cn

JS:   constructor(name) { this.name = name; }
来源：http://aho.zhixingplan.top

TS:   constructor(public name: string) {}
来源：http://bod.hfpthk.cn

Java: User(String name) { this.name = name; }
来源：http://tdw.tianlin.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cnc.fzhhl.top

Ruby: def initialize(name); @name = name; end
来源：http://feq.gotoacloud.top

C#:   public User(string name) { Name = name; }
来源：http://dkq.zdbjq.cn

[G03] 实例属性
来源：http://zrn.haohaochexian.top

Py:   self.name = "x"
来源：http://nyx.yanxiufei.cn

PHP:  public string $name = "x";
来源：http://gzy.316326.xyz

JS:   this.name = "x";
来源：http://ruq.sjlbkw.cn

TS:   name: string = "x";
来源：http://uhz.wangshuangyany.cn

Java: private String name;
来源：http://jto.guowangkeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fqe.fehbvm.com

Ruby: @name = "x"
来源：http://zrp.andypj.xyz

C#:   public string Name { get; set; } = "x";
来源：http://uej.tianlin.xyz

[G04] 定义方法
来源：http://rvd.xingfuxueyuan.xyz

Py:   def greet(self): return self.name
来源：http://xxx.fktsv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nrq.tianlin.xyz

JS:   greet() { return this.name; }
来源：http://ntt.bjfxy.top

TS:   greet(): string { return this.name; }
来源：http://otd.epnwcf.com

Java: String greet() { return name; }
来源：http://fjg.cucudq.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://aji.jinqigfzy.top

Ruby: def greet; @name; end
来源：http://plp.shangyingyoupin.top

C#:   public string Greet() => Name;
来源：http://zon.uphjek.com

[G05] 继承
来源：http://wmw.zhiwuduotai.top

Py:   class Admin(User): pass
来源：http://aqf.fengsongda.top

PHP:  class Admin extends User {}
来源：http://lzu.sjlbkw.cn

JS:   class Admin extends User {}
来源：http://fio.zhongyouzk.top

TS:   class Admin extends User {}
来源：http://yju.xinyue.icu

Java: class Admin extends User {}
来源：http://fgd.wangshuangyany.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://awz.jlsjyb.cn

Ruby: class Admin < User; end
来源：http://aoo.haohaochexian.top

C#:   class Admin : User {}
来源：http://qwz.jianghu66.top

[G06] 重写方法
来源：http://kle.daria6918.cn

Py:   def greet(self): return "admin"
来源：http://weq.daxiang520.top

PHP:  public function greet(): string { return "admin"; }
来源：http://knp.epnwcf.com

JS:   greet() { return "admin"; }
来源：http://giv.yvedp.cn

TS:   greet(): string { return "admin"; }
来源：http://zkp.redwolf501.top

Java: @Override String greet() { return "admin"; }
来源：http://fgv.jianghu66.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://guw.havefunace.top

Ruby: def greet; "admin"; end
来源：http://kni.jyoumei.cn

C#:   public override string Greet() => "admin";
来源：http://brj.0kj1m.cn

[G07] 调用父类方法
来源：http://bqr.guowangkeji.top

Py:   super().greet()
来源：http://xuq.ydjk.org.cn

PHP:  parent::greet();
来源：http://deu.fanxiaobao.xyz

JS:   super.greet();
来源：http://pax.sysykeji.top

TS:   super.greet();
来源：http://gno.pengpengdd.cyou

Java: super.greet();
来源：http://ola.hnxiangtu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tet.kuanghao11.cn

Ruby: super
来源：http://nkr.snrcjt.cn

C#:   base.Greet();
来源：http://qnz.dashuyun.cn

[G08] 静态方法与属性
来源：http://qzh.wangshuangyany.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cqc.yueranfly.top

PHP:  public static function f() {}
来源：http://zzy.zdqjudy.top

JS:   static f() {}
来源：http://yhm.shangyingyoupin.top

TS:   static f(): void {}
来源：http://zib.chenlongwang.top

Java: static void f() {}
来源：http://evs.fktsv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ohn.gaohongyu789.top

Ruby: def self.f; end
来源：http://qsj.hongshengwenyu.top

C#:   public static void F() {}
来源：http://dgo.tanke756.top

[G09] 接口 / 抽象类
来源：http://iae.havefunace.top

Py:   from abc import ABC, abstractmethod
来源：http://hix.yanxiufei.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hzc.bjfxy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ryo.sxryk.cn

TS:   interface Shape { area(): number; }
来源：http://psk.yueranfly.top

Java: interface Shape { double area(); }
来源：http://gwx.vehdjk.com

Go:   type Shape interface { Area() float64 }
来源：http://ogg.hywenlv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cwd.mhx1999.top

C#:   interface IShape { double Area(); }
来源：http://krs.jqgufenzy.top

[G10] 访问控制
来源：http://tsq.hesvh.cn

Py:   约定 _protected / __private（不强制）
来源：http://bbq.sxryk.cn

PHP:  public / protected / private
来源：http://hrh.xinyue.icu

JS:   #private 字段；其余公开
来源：http://rjp.cashguo.top

TS:   public / protected / private
来源：http://qct.cdnleiting.top

Java: public / protected / private / 默认包级
来源：http://iqg.chenlongwang.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ope.fanxiaobao.xyz

Ruby: public / protected / private
来源：http://igm.fanxiaobao.xyz

C#:   public / protected / private / internal
来源：http://ycx.zhiwuduotai.top

[G11] getter / setter
来源：http://xkn.ybcxt.top

Py:   @property 与 @x.setter
来源：http://ujs.bjfxy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://xha.birdmap.top

JS:   get name() { return this._name; }
来源：http://ivt.iojbl.cn

TS:   get name(): string { return this._name; }
来源：http://ssi.zhijiandao.cn

Java: public String getName() { return name; }
来源：http://aat.zhoulong.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://fon.daria6918.cn

Ruby: attr_accessor :name
来源：http://woj.havefunace.top

C#:   public string Name { get; set; }
来源：http://drb.0kj1m.cn

[G12] 对象转字符串
来源：http://enr.guannengcc.top

Py:   def __str__(self): return self.name
来源：http://yiw.yj20258.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://pkq.9152youxi.cn

JS:   toString() { return this.name; }
来源：http://juh.ppjwa.cn

TS:   toString(): string { return this.name; }
来源：http://icg.dashuyun.cn

Java: @Override public String toString() { return name; }
来源：http://pvh.meibo888.top

Go:   func (u User) String() string { return u.Name }
来源：http://boc.zycfv.cn

Ruby: def to_s; @name; end
来源：http://smw.xuanzx.com

C#:   public override string ToString() => Name;
来源：http://fwd.shzxlz.cn

[G13] 判断对象类型
来源：http://iqv.dashuyun.cn

Py:   isinstance(u, User)
来源：http://hry.zdqjudy.top

PHP:  $u instanceof User
来源：http://cdb.havefunace.top

JS:   u instanceof User
来源：http://byj.jyoumei.cn

TS:   u instanceof User
来源：http://vzm.0kj1m.cn

Java: u instanceof User
来源：http://afn.wangshuangyany.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://bfn.shangyingyoupin.top

Ruby: u.is_a?(User)
来源：http://psw.nanxinkj.top

C#:   u is User
来源：http://yyl.hywenlv.cn

[G14] 数据类 / record
来源：http://zza.fzhhl.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ugg.ctjpmb.com

PHP:  // 用 readonly 属性模拟
来源：http://eaw.haohaochexian.top

JS:   // 无内置：普通类或对象字面量
来源：http://gha.yanxiufei.cn

TS:   type User = { name: string; age: number };
来源：http://tho.hfpthk.cn

Java: record User(String name, int age) {}
来源：http://mjy.jinyuanbaomall.cn

Go:   type User struct { Name string; Age int }
来源：http://ccp.meibo888.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vlk.cucudq.cn

C#:   record User(string Name, int Age);
来源：http://cgt.yonumen.top

[G15] 枚举
来源：http://cgo.daria6918.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fnr.hfpthk.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://tjm.guannengcc.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ony.cucudq.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://koi.andypj.xyz

Java: enum Color { RED, GREEN }
来源：http://tnl.wangdashe.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xev.zhiwuduotai.top

Ruby: Color = %i[red green].freeze
来源：http://rgc.zhaomingkeji.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sqj.ppjwa.cn

[G16] 对象转数组 / 字典
来源：http://prc.yj20258888.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://obx.hcnkem.com

PHP:  get_object_vars($obj);
来源：http://xzl.gotoacloud.top

JS:   Object.entries(obj)
来源：http://jpd.tarul.cn

TS:   Object.entries(obj)
来源：http://rgm.ctjpmb.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zql.ydzc1.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ezk.uphjek.com

Ruby: obj.instance_variables
来源：http://sim.fktsv.cn

C#:   // 用反射或 System.Text.Json
来源：http://dus.hfpthk.cn

================================================================================
来源：http://ixq.daria6918.cn

H. 异常与错误处理
来源：http://aop.birdmap.top

================================================================================
来源：http://uja.xinyue.icu

[H01] try / catch 基础
来源：http://tpb.hnqzz.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hww.chenzaomai.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rvs.cheryme.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fbw.sweek.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://plx.yj20258.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pkx.havefunace.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qfj.yuxming.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xox.hammf.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ynx.yanxiufei.cn

[H02] finally / ensure 收尾
来源：http://xoi.ywan-chungtsiang.top

Py:   try: f()⏎finally: cleanup()
来源：http://zyd.vqdsnc.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://thv.wangdashe.top

JS:   try { f(); } finally { cleanup(); }
来源：http://djv.jianghu66.top

TS:   try { f(); } finally { cleanup(); }
来源：http://fsn.zhengqikj.top

Java: try { f(); } finally { cleanup(); }
来源：http://khq.yanxiufei.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://kir.bbcook.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ozm.ydzc1.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://loa.tian-w.cn

[H03] 主动抛出异常
来源：http://jpw.zhijiandao.cn

Py:   raise ValueError("错误信息")
来源：http://har.dianchejie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cez.zycfv.cn

JS:   throw new Error("错误信息");
来源：http://eui.aizwys.cn

TS:   throw new Error("错误信息");
来源：http://cas.daxiang520.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://nat.birdmap.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tlg.birdmap.top

Ruby: raise ArgumentError, "错误信息"
来源：http://zst.redwolf501.top

C#:   throw new ArgumentException("错误信息");
来源：http://ouf.redwolf501.top

[H04] 自定义异常类型
来源：http://ejt.shzxlz.cn

Py:   class MyError(Exception): pass
来源：http://viq.quarkkingdee.top

PHP:  class MyError extends RuntimeException {}
来源：http://boi.hfpthk.cn

JS:   class MyError extends Error {}
来源：http://jdb.shangyingyoupin.top

TS:   class MyError extends Error {}
来源：http://efp.gzhubu.top

Java: class MyException extends RuntimeException {}
来源：http://krk.zycfv.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://afz.zhoulong.xyz

Ruby: class MyError < StandardError; end
来源：http://xxw.zhongyouzk.top

C#:   class MyException : Exception {}
来源：http://zfx.aibaodan.cn

[H05] 捕获特定类型
来源：http://jwt.pengpengdd.cyou

Py:   except ValueError as e:
来源：http://jpe.yj202588.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cmc.fktsv.cn

JS:   if (e instanceof TypeError) {}
来源：http://qun.guowangkeji.top

TS:   if (e instanceof TypeError) {}
来源：http://koe.yvedp.cn

Java: catch (IOException | SQLException e) {}
来源：http://boc.gzhubu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tfj.ybcxt.top

Ruby: rescue ArgumentError => e
来源：http://duy.uphjek.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jyl.tian-w.cn

[H06] 可选值 / 空值安全访问
来源：http://oqr.yongpay.top

Py:   value = d.get("k") or default
来源：http://jhn.cheryme.top

PHP:  $v = $d["k"] ?? null;
来源：http://tkc.tanke756.top

JS:   obj?.a?.b;  d ?? default
来源：http://dqw.fanxiaobao.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://ksx.meibo888.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zbq.ehwqpu.com

Go:   if v, ok := m["k"]; ok { }
来源：http://fxb.shzxlz.cn

Ruby: d&.dig(:a, :b)
来源：http://rrp.snrcjt.cn

C#:   obj?.A?.B ?? default
来源：http://vfy.0kj1m.cn

[H07] 断言
来源：http://oem.ydzc1.top

Py:   assert x > 0, "必须为正"
来源：http://zsn.chenzaomai.com

PHP:  assert($x > 0);
来源：http://ydu.iojbl.cn

JS:   console.assert(x > 0);
来源：http://msl.zycfv.cn

TS:   console.assert(x > 0);
来源：http://ugb.yangfankeji.com

Java: assert x > 0 : "必须为正";
来源：http://oof.sufxvd.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://npv.jyoumei.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wqz.feifeiyinyue.top

C#:   Debug.Assert(x > 0);
来源：http://nyg.hesvh.cn

[H08] 获取错误信息与堆栈
来源：http://wjh.hysaishi.cn

Py:   str(e);  traceback.format_exc()
来源：http://ell.guannengcc.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kye.havefunace.top

JS:   e.message;  e.stack
来源：http://vak.bjfxy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://xqn.kuanghao11.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nti.smart0.xyz

Go:   err.Error()
来源：http://ntu.birdmap.top

Ruby: e.message;  e.backtrace
来源：http://ivm.zhiwuduotai.top

C#:   e.Message;  e.StackTrace
来源：http://jlx.ywan-chungtsiang.top

[H09] 带错误码的异常
来源：http://ozt.sufxvd.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ifs.sxryk.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cjz.cucudq.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fnd.tarul.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bed.yongpay.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kod.xinyue.icu

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nao.xinyue.icu

Ruby: raise MyError.new("fail", 500)
来源：http://kxz.tanke756.top

C#:   // 自定义异常类中加 Code 属性
来源：http://sbs.vehdjk.com

[H10] 资源自动释放
来源：http://cyu.guowangkeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://qqu.wangdashe.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://saw.ybcxt.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://goo.hfpthk.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://aqi.xuanzx.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pzq.fzhhl.top

Go:   defer f.Close()
来源：http://pye.52xcode.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://otj.dashuyun.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mww.jinqigfzy.top

================================================================================
来源：http://jmo.wangdashe.top

I. 正则表达式
来源：http://mzf.bjfxy.top

================================================================================
来源：http://zjz.gaohongyu789.top

[I01] 判断是否匹配
来源：http://fdx.sjlbkw.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zqc.zhiwuduotai.top

PHP:  preg_match('/\d+/', $s);
来源：http://bbg.fanxiaobao.xyz

JS:   /\d+/.test(s)
来源：http://ucl.hfpthk.cn

TS:   /\d+/.test(s)
来源：http://nto.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fvx.yongpay.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zho.tarul.cn

Ruby: s.match?(/\d+/)
来源：http://qff.fehbvm.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yby.tian-w.cn

[I02] 提取所有匹配
来源：http://ozq.yj20258888.top

Py:   re.findall(r"\d+", s)
来源：http://mpl.dashuyun.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bzl.gogol.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://eyw.fengsongda.top

TS:   s.match(/\d+/g)
来源：http://gsq.zhaomingkeji.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://icr.dianchejie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ius.sweek.top

Ruby: s.scan(/\d+/)
来源：http://ifz.hysaishi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://flk.zdqjudy.top

[I03] 提取捕获分组
来源：http://roh.snrcjt.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bjc.sysykeji.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ynp.jlsjyb.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xio.yvedp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xmu.yuanzhike.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nox.hongshengwenyu.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lhn.snrcjt.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hjv.andypj.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pov.chenjidiqi.icu

[I04] 正则替换
来源：http://lli.ppjwa.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jht.birdmap.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fex.vehdjk.com

JS:   s.replace(/\d+/g, "#")
来源：http://nrm.cqqwz.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lhs.feifeiyinyue.top

Java: s.replaceAll("\\d+", "#")
来源：http://tnh.hongshengwenyu.top

Go:   re.ReplaceAllString(s, "#")
来源：http://giu.vehdjk.com

Ruby: s.gsub(/\d+/, "#")
来源：http://hhs.havefunace.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xjw.meibo888.top

[I05] 按正则拆分
来源：http://lcv.shanyushiyangkeji.top

Py:   re.split(r"\s*,\s*", s)
来源：http://blj.ydjk.org.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yqv.daria6918.cn

JS:   s.split(/\s*,\s*/)
来源：http://jwx.vqdsnc.cn

TS:   s.split(/\s*,\s*/)
来源：http://saj.0kj1m.cn

Java: s.split("\\s*,\\s*")
来源：http://xxs.pengpengdd.cyou

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://eyl.hnxiangtu.top

Ruby: s.split(/\s*,\s*/)
来源：http://wbb.shzxlz.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qio.xuetiantiany.cn


<!-- 参考信息 -->