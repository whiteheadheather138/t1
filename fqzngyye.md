代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mfh.fanxiaobao.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ehr.jinyuanbaomall.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wcn.wangdashe.top

[F12] CSV 读写
来源：http://loy.zhongyouzk.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mvo.yj20258888.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://coi.xuanzx.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jsc.hfpthk.cn

TS:   // 同上
来源：http://rcu.zhaomingkeji.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ykr.quarkkingdee.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jzq.shzxlz.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pvt.jqgufenzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://zqt.fktsv.cn

================================================================================
来源：http://cbo.xuetiantiany.cn

G. 面向对象
来源：http://vxz.hnxiangtu.top

================================================================================
来源：http://amm.pycfn.com

[G01] 定义类
来源：http://fiw.jiagoushi.top

Py:   class User: pass
来源：http://gma.0kj1m.cn

PHP:  class User {}
来源：http://cda.hnqzz.top

JS:   class User {}
来源：http://esh.pycfn.com

TS:   class User { name: string = ""; }
来源：http://pss.epnwcf.com

Java: class User {}
来源：http://epi.yfazqb.com

Go:   type User struct { Name string }
来源：http://hxo.jinyuanbaomall.cn

Ruby: class User; end
来源：http://ahx.tanke756.top

C#:   class User {}
来源：http://gwn.yongpay.top

[G02] 构造函数
来源：http://jyn.quarkkingdee.top

Py:   def __init__(self, name): self.name = name
来源：http://ots.tanke756.top

PHP:  public function __construct(public string $name) {}
来源：http://qip.sysykeji.top

JS:   constructor(name) { this.name = name; }
来源：http://tlr.uphjek.com

TS:   constructor(public name: string) {}
来源：http://uuc.cashguo.top

Java: User(String name) { this.name = name; }
来源：http://eop.yangfankeji.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://llo.cdnleiting.top

Ruby: def initialize(name); @name = name; end
来源：http://kld.nanxinkj.top

C#:   public User(string name) { Name = name; }
来源：http://riy.xuanzx.com

[G03] 实例属性
来源：http://odg.pengpengdd.cyou

Py:   self.name = "x"
来源：http://qns.chenzaomai.com

PHP:  public string $name = "x";
来源：http://mxq.hnxiangtu.top

JS:   this.name = "x";
来源：http://ipg.ivvv.top

TS:   name: string = "x";
来源：http://fhu.zdqjudy.top

Java: private String name;
来源：http://yeb.jinqigfzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bdq.jinqigufen.top

Ruby: @name = "x"
来源：http://jxb.yj20258.top

C#:   public string Name { get; set; } = "x";
来源：http://pwv.yj202588.top

[G04] 定义方法
来源：http://wwp.nanxuanxn.top

Py:   def greet(self): return self.name
来源：http://cde.zycfv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://stj.zhiwuduotai.top

JS:   greet() { return this.name; }
来源：http://qjo.aizwys.cn

TS:   greet(): string { return this.name; }
来源：http://pzu.bjfxy.top

Java: String greet() { return name; }
来源：http://fld.daria6918.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://kmp.c1oappe.top

Ruby: def greet; @name; end
来源：http://uwe.yangfankeji.com

C#:   public string Greet() => Name;
来源：http://vlu.daxiang520.top

[G05] 继承
来源：http://sxp.yj20258888.top

Py:   class Admin(User): pass
来源：http://rff.xinyue.icu

PHP:  class Admin extends User {}
来源：http://dfh.hesvh.cn

JS:   class Admin extends User {}
来源：http://xtk.chenlongwang.top

TS:   class Admin extends User {}
来源：http://zoh.guowangkeji.top

Java: class Admin extends User {}
来源：http://hik.fktsv.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ihc.316326.xyz

Ruby: class Admin < User; end
来源：http://cbr.jiagoushi.top

C#:   class Admin : User {}
来源：http://dqm.fzhhl.top

[G06] 重写方法
来源：http://cwj.andypj.xyz

Py:   def greet(self): return "admin"
来源：http://lkr.yanxiufei.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://czn.daxiang520.top

JS:   greet() { return "admin"; }
来源：http://umx.shanyushiyangkeji.top

TS:   greet(): string { return "admin"; }
来源：http://asd.zhengqikj.top

Java: @Override String greet() { return "admin"; }
来源：http://ouh.pengpengdd.cyou

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tag.fanxiaobao.xyz

Ruby: def greet; "admin"; end
来源：http://eva.nanxinkj.top

C#:   public override string Greet() => "admin";
来源：http://rbh.xinyue.icu

[G07] 调用父类方法
来源：http://htf.kuanghao11.cn

Py:   super().greet()
来源：http://yzs.zhongyouzk.top

PHP:  parent::greet();
来源：http://cpv.feifeiyinyue.top

JS:   super.greet();
来源：http://rce.ppjwa.cn

TS:   super.greet();
来源：http://tsy.zhoulong.xyz

Java: super.greet();
来源：http://pkr.sjlbkw.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xwd.ppjwa.cn

Ruby: super
来源：http://jgs.cqqwz.cn

C#:   base.Greet();
来源：http://fms.gzhubu.top

[G08] 静态方法与属性
来源：http://wfl.zhaomingkeji.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ern.wangshuangyany.cn

PHP:  public static function f() {}
来源：http://evv.hcnkem.com

JS:   static f() {}
来源：http://qbf.shuidangran.top

TS:   static f(): void {}
来源：http://nad.zhengqikj.top

Java: static void f() {}
来源：http://yxv.zhaomingkeji.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://orz.feifeiyinyue.top

Ruby: def self.f; end
来源：http://mqp.guowangkeji.top

C#:   public static void F() {}
来源：http://slj.ybcxt.top

[G09] 接口 / 抽象类
来源：http://yvc.hnxiangtu.top

Py:   from abc import ABC, abstractmethod
来源：http://ocm.daria6918.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ths.havefunace.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://puj.zhongyouzk.top

TS:   interface Shape { area(): number; }
来源：http://zti.xziqi.cn

Java: interface Shape { double area(); }
来源：http://hjl.fanxiaobao.xyz

Go:   type Shape interface { Area() float64 }
来源：http://asy.sxryk.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qef.nanxinkj.top

C#:   interface IShape { double Area(); }
来源：http://kwb.jinghuilouyu.cn

[G10] 访问控制
来源：http://bqp.bjfxy.top

Py:   约定 _protected / __private（不强制）
来源：http://oat.shuidangran.top

PHP:  public / protected / private
来源：http://wlq.fengsongda.top

JS:   #private 字段；其余公开
来源：http://ial.shuidangran.top

TS:   public / protected / private
来源：http://ivd.hywenlv.cn

Java: public / protected / private / 默认包级
来源：http://wxr.dianchejie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hft.smart0.xyz

Ruby: public / protected / private
来源：http://hza.9152youxi.cn

C#:   public / protected / private / internal
来源：http://mbx.tarul.cn

[G11] getter / setter
来源：http://lvu.shangyingyoupin.top

Py:   @property 与 @x.setter
来源：http://npu.mhx1999.top

PHP:  public function getName(): string { return $this->name; }
来源：http://vkk.bbcook.cn

JS:   get name() { return this._name; }
来源：http://eeb.pengpengdd.cyou

TS:   get name(): string { return this._name; }
来源：http://vda.bjfxy.top

Java: public String getName() { return name; }
来源：http://ojk.sufxvd.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dkn.316326.xyz

Ruby: attr_accessor :name
来源：http://vxf.daxiang520.top

C#:   public string Name { get; set; }
来源：http://bhc.yj20258888.top

[G12] 对象转字符串
来源：http://xqg.jqgufenzy.top

Py:   def __str__(self): return self.name
来源：http://tuq.ctjpmb.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://pjx.fehbvm.com

JS:   toString() { return this.name; }
来源：http://oej.ehwqpu.com

TS:   toString(): string { return this.name; }
来源：http://rew.ydjk.org.cn

Java: @Override public String toString() { return name; }
来源：http://sgp.quarkkingdee.top

Go:   func (u User) String() string { return u.Name }
来源：http://fpz.smart0.xyz

Ruby: def to_s; @name; end
来源：http://kpv.zhengqikj.top

C#:   public override string ToString() => Name;
来源：http://kth.pengpengdd.cyou

[G13] 判断对象类型
来源：http://nzk.cheryme.top

Py:   isinstance(u, User)
来源：http://udv.tian-w.cn

PHP:  $u instanceof User
来源：http://ezs.havefunace.top

JS:   u instanceof User
来源：http://cly.nwbrower.top

TS:   u instanceof User
来源：http://srv.hysaishi.cn

Java: u instanceof User
来源：http://iut.shangyingyoupin.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://srq.sweek.top

Ruby: u.is_a?(User)
来源：http://zhx.sweek.top

C#:   u is User
来源：http://jkj.yj202588.top

[G14] 数据类 / record
来源：http://gxp.zdqjudy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://owr.nanxinkj.top

PHP:  // 用 readonly 属性模拟
来源：http://mjo.yanxiufei.cn

JS:   // 无内置：普通类或对象字面量
来源：http://twx.mhx1999.top

TS:   type User = { name: string; age: number };
来源：http://klz.bbcook.cn

Java: record User(String name, int age) {}
来源：http://vfp.sjlbkw.cn

Go:   type User struct { Name string; Age int }
来源：http://dti.zhongyouzk.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baj.cdnleiting.top

C#:   record User(string Name, int Age);
来源：http://fuz.gotoacloud.top

[G15] 枚举
来源：http://qrb.0kj1m.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ayp.aizwys.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dvv.hcnkem.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ick.sysykeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yus.bjfxy.top

Java: enum Color { RED, GREEN }
来源：http://jjq.epnwcf.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mgd.tanke756.top

Ruby: Color = %i[red green].freeze
来源：http://fnp.zhijiandao.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fjl.snrcjt.cn

[G16] 对象转数组 / 字典
来源：http://lbe.xziqi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xko.tian-w.cn

PHP:  get_object_vars($obj);
来源：http://vsu.pengpengdd.cyou

JS:   Object.entries(obj)
来源：http://naa.wangshuangyany.cn

TS:   Object.entries(obj)
来源：http://vsr.andypj.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cwb.daxiang520.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ioz.ybcxt.top

Ruby: obj.instance_variables
来源：http://mab.zdbjq.cn

C#:   // 用反射或 System.Text.Json
来源：http://ncf.hammf.cn

================================================================================
来源：http://lcr.pengpengdd.cyou

H. 异常与错误处理
来源：http://tjh.zhijiandao.cn

================================================================================
来源：http://chr.ybcxt.top

[H01] try / catch 基础
来源：http://cfm.0kj1m.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fxk.fehbvm.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://edk.yfazqb.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uxx.hongshengwenyu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hcf.hysaishi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cau.vehdjk.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://teh.yfazqb.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dhs.jiagoushi.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cxa.yongpay.top

[H02] finally / ensure 收尾
来源：http://dbm.vqdsnc.cn

Py:   try: f()⏎finally: cleanup()
来源：http://srb.iojbl.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ytu.sufxvd.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bgw.pengpengdd.cyou

TS:   try { f(); } finally { cleanup(); }
来源：http://mxj.daria6918.cn

Java: try { f(); } finally { cleanup(); }
来源：http://blq.chenlongwang.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ndt.sjlbkw.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wmj.meibo888.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://mgu.vehdjk.com

[H03] 主动抛出异常
来源：http://ooi.bjfxy.top

Py:   raise ValueError("错误信息")
来源：http://nis.zhengqikj.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hxm.sweek.top

JS:   throw new Error("错误信息");
来源：http://aeo.gaohongyu789.top

TS:   throw new Error("错误信息");
来源：http://zup.yj20258.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://dbu.zdqjudy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mtn.ydjk.org.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://que.redwolf501.top

C#:   throw new ArgumentException("错误信息");
来源：http://fys.yj202588.top

[H04] 自定义异常类型
来源：http://rpg.epnwcf.com

Py:   class MyError(Exception): pass
来源：http://xfc.9152youxi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nhr.hysaishi.cn

JS:   class MyError extends Error {}
来源：http://hph.yj202588.top

TS:   class MyError extends Error {}
来源：http://cmc.yuxming.cn

Java: class MyException extends RuntimeException {}
来源：http://bad.shanyushiyangkeji.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qsv.chenzaomai.com

Ruby: class MyError < StandardError; end
来源：http://fqf.chenlongwang.top

C#:   class MyException : Exception {}
来源：http://yst.ehwqpu.com

[H05] 捕获特定类型
来源：http://txz.fzhhl.top

Py:   except ValueError as e:
来源：http://ryv.fehbvm.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hho.gzhubu.top

JS:   if (e instanceof TypeError) {}
来源：http://yyz.yangfankeji.com

TS:   if (e instanceof TypeError) {}
来源：http://zlp.shzxlz.cn

Java: catch (IOException | SQLException e) {}
来源：http://rzy.nanxuanxn.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gnr.yanxiufei.cn

Ruby: rescue ArgumentError => e
来源：http://ruk.yj202588.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sqf.tian-w.cn

[H06] 可选值 / 空值安全访问
来源：http://hln.zdbjq.cn

Py:   value = d.get("k") or default
来源：http://cxt.feifeiyinyue.top

PHP:  $v = $d["k"] ?? null;
来源：http://wow.bjfxy.top

JS:   obj?.a?.b;  d ?? default
来源：http://ioc.zhengqikj.top

TS:   obj?.a?.b;  d ?? default
来源：http://xnj.mhx1999.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://abo.yanxiufei.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://spz.dashuyun.cn

Ruby: d&.dig(:a, :b)
来源：http://buc.xziqi.cn

C#:   obj?.A?.B ?? default
来源：http://jui.uphjek.com

[H07] 断言
来源：http://hiu.tanke756.top

Py:   assert x > 0, "必须为正"
来源：http://puv.feifeiyinyue.top

PHP:  assert($x > 0);
来源：http://oid.0kj1m.cn

JS:   console.assert(x > 0);
来源：http://rng.chenjidiqi.icu

TS:   console.assert(x > 0);
来源：http://wky.aibaodan.cn

Java: assert x > 0 : "必须为正";
来源：http://koy.guowangkeji.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zdb.wangdashe.top

Ruby: raise "必须为正" unless x > 0
来源：http://ddh.bjfxy.top

C#:   Debug.Assert(x > 0);
来源：http://vzu.jlsjyb.cn

[H08] 获取错误信息与堆栈
来源：http://kjx.xuetiantiany.cn

Py:   str(e);  traceback.format_exc()
来源：http://gqd.pengpengdd.cyou

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fou.ywan-chungtsiang.top

JS:   e.message;  e.stack
来源：http://ymm.tianlin.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://wzf.c1oappe.top

Java: e.getMessage();  e.printStackTrace()
来源：http://wij.xuetiantiany.cn

Go:   err.Error()
来源：http://rip.jianghu66.top

Ruby: e.message;  e.backtrace
来源：http://xbr.redwolf501.top

C#:   e.Message;  e.StackTrace
来源：http://cxl.hnxiangtu.top

[H09] 带错误码的异常
来源：http://mhm.sxryk.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://znk.nwbrower.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://gfl.kuanghao11.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://idv.pengpengdd.cyou

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kbr.birdmap.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jkj.yueranfly.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oyc.xinyue.icu

Ruby: raise MyError.new("fail", 500)
来源：http://nwy.jiagoushi.top

C#:   // 自定义异常类中加 Code 属性
来源：http://nfx.dianchejie.cn

[H10] 资源自动释放
来源：http://tla.cqqwz.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://inr.fengsongda.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hcc.52xcode.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wcl.chenlongwang.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cqg.cheryme.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dsz.shanyushiyangkeji.top

Go:   defer f.Close()
来源：http://qrm.epnwcf.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vmb.smart0.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mxs.xziqi.cn

================================================================================
来源：http://otl.ydjk.org.cn

I. 正则表达式
来源：http://plp.iojbl.cn

================================================================================
来源：http://ted.52xcode.cn

[I01] 判断是否匹配
来源：http://zsc.zhijiandao.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kag.yj202588.top

PHP:  preg_match('/\d+/', $s);
来源：http://rhy.dianchejie.cn

JS:   /\d+/.test(s)
来源：http://ojb.svipenyu.cn

TS:   /\d+/.test(s)
来源：http://uha.shangyingyoupin.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ofn.aizwys.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://khj.quarkkingdee.top

Ruby: s.match?(/\d+/)
来源：http://sti.guannengcc.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lut.vqdsnc.cn

[I02] 提取所有匹配
来源：http://vjb.fehbvm.com

Py:   re.findall(r"\d+", s)
来源：http://eyv.shzxlz.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://crg.fktsv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gmk.jqgufenzy.top

TS:   s.match(/\d+/g)
来源：http://ilq.birdmap.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wfe.pengpengdd.cyou

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ffi.c1oappe.top

Ruby: s.scan(/\d+/)
来源：http://bgs.guowangkeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bvs.ivvv.top

[I03] 提取捕获分组
来源：http://ggz.jianghu66.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ipe.wangdashe.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jad.0kj1m.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jrd.nanxuanxn.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ebs.zhongyouzk.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dma.zdbjq.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xhc.jinqigufen.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xse.yj20258888.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gdb.shanyushiyangkeji.top

[I04] 正则替换
来源：http://tsk.jinyuanbaomall.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zzs.andypj.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fsz.sjlbkw.cn

JS:   s.replace(/\d+/g, "#")
来源：http://uta.fanxiaobao.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://nla.zycfv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jai.zhaomingkeji.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://wgw.hywenlv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hdo.xuanzx.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://suk.andypj.xyz

[I05] 按正则拆分
来源：http://bjd.jinghuilouyu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gap.kuanghao11.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kjy.birdmap.top

JS:   s.split(/\s*,\s*/)
来源：http://ezv.hesvh.cn

TS:   s.split(/\s*,\s*/)
来源：http://mkw.xuanzx.com

Java: s.split("\\s*,\\s*")
来源：http://hrw.guowangkeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mbc.yj20258.top

Ruby: s.split(/\s*,\s*/)
来源：http://fwf.ivvv.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qyo.guannengcc.top


<!-- 参考信息 -->