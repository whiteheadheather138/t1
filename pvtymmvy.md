代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qpu.yonumen.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dfv.jqgufenzy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://iau.yueranfly.top

[F12] CSV 读写
来源：http://xnn.tanke756.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mud.tarul.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ltk.yuxming.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://klr.wangshuangyany.cn

TS:   // 同上
来源：http://hzb.shangyingyoupin.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://auh.hnxiangtu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qfh.smart0.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ysn.shanyushiyangtech.top

C#:   // 无内置：用 CsvHelper 库
来源：http://jiy.epnwcf.com

================================================================================
来源：http://acm.dianchejie.cn

G. 面向对象
来源：http://bya.cqqwz.cn

================================================================================
来源：http://cwe.hnxiangtu.top

[G01] 定义类
来源：http://dxh.gogol.net.cn

Py:   class User: pass
来源：http://bor.ppjwa.cn

PHP:  class User {}
来源：http://oyt.dianchejie.cn

JS:   class User {}
来源：http://vee.zhongyouzk.top

TS:   class User { name: string = ""; }
来源：http://zdx.wangshuangyany.cn

Java: class User {}
来源：http://vzr.hfpthk.cn

Go:   type User struct { Name string }
来源：http://oym.gotoacloud.top

Ruby: class User; end
来源：http://yop.chenlongwang.top

C#:   class User {}
来源：http://nzr.yuanzhike.top

[G02] 构造函数
来源：http://qpl.fktsv.cn

Py:   def __init__(self, name): self.name = name
来源：http://moe.pycfn.com

PHP:  public function __construct(public string $name) {}
来源：http://weq.pengpengdd.cyou

JS:   constructor(name) { this.name = name; }
来源：http://hwd.hywenlv.cn

TS:   constructor(public name: string) {}
来源：http://rnf.yvedp.cn

Java: User(String name) { this.name = name; }
来源：http://mfw.gzhubu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qlq.dianchejie.cn

Ruby: def initialize(name); @name = name; end
来源：http://rnw.hnxiangtu.top

C#:   public User(string name) { Name = name; }
来源：http://van.quarkkingdee.top

[G03] 实例属性
来源：http://fcr.shuidangran.top

Py:   self.name = "x"
来源：http://fze.aibaodan.cn

PHP:  public string $name = "x";
来源：http://xig.jinghuilouyu.cn

JS:   this.name = "x";
来源：http://kby.aizwys.cn

TS:   name: string = "x";
来源：http://goh.yanxiufei.cn

Java: private String name;
来源：http://dxr.yanxiufei.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://odu.feifeiyinyue.top

Ruby: @name = "x"
来源：http://jkb.sxryk.cn

C#:   public string Name { get; set; } = "x";
来源：http://dui.ydzc1.top

[G04] 定义方法
来源：http://kct.fktsv.cn

Py:   def greet(self): return self.name
来源：http://orh.ivvv.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qze.tarul.cn

JS:   greet() { return this.name; }
来源：http://nsx.hesvh.cn

TS:   greet(): string { return this.name; }
来源：http://dhs.zdbjq.cn

Java: String greet() { return name; }
来源：http://nir.0kj1m.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://srv.sweek.top

Ruby: def greet; @name; end
来源：http://gwr.nwbrower.top

C#:   public string Greet() => Name;
来源：http://ypj.zhongyouzk.top

[G05] 继承
来源：http://apd.hammf.cn

Py:   class Admin(User): pass
来源：http://alw.jinqigufen.top

PHP:  class Admin extends User {}
来源：http://rmq.pycfn.com

JS:   class Admin extends User {}
来源：http://cgd.zycfv.cn

TS:   class Admin extends User {}
来源：http://mkw.tarul.cn

Java: class Admin extends User {}
来源：http://dbd.uphjek.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://avw.zhijiandao.cn

Ruby: class Admin < User; end
来源：http://qpu.cucudq.cn

C#:   class Admin : User {}
来源：http://udh.cqqwz.cn

[G06] 重写方法
来源：http://cka.bjfxy.top

Py:   def greet(self): return "admin"
来源：http://mce.aibaodan.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hsj.epnwcf.com

JS:   greet() { return "admin"; }
来源：http://ang.tian-w.cn

TS:   greet(): string { return "admin"; }
来源：http://erz.xuetiantiany.cn

Java: @Override String greet() { return "admin"; }
来源：http://aav.xinyue.icu

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ppb.fzhhl.top

Ruby: def greet; "admin"; end
来源：http://krv.xuanzx.com

C#:   public override string Greet() => "admin";
来源：http://acj.yangfankeji.com

[G07] 调用父类方法
来源：http://ohq.mhx1999.top

Py:   super().greet()
来源：http://voh.chenzaomai.com

PHP:  parent::greet();
来源：http://pgx.ydjk.org.cn

JS:   super.greet();
来源：http://blh.sufxvd.cn

TS:   super.greet();
来源：http://lqe.316326.xyz

Java: super.greet();
来源：http://mfx.hnxiangtu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jno.zhengqikj.top

Ruby: super
来源：http://taf.hnxiangtu.top

C#:   base.Greet();
来源：http://mkv.redwolf501.top

[G08] 静态方法与属性
来源：http://tvo.ivvv.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mib.zhengqikj.top

PHP:  public static function f() {}
来源：http://ozk.ppjwa.cn

JS:   static f() {}
来源：http://gre.cucudq.cn

TS:   static f(): void {}
来源：http://xvn.wangdashe.top

Java: static void f() {}
来源：http://fgu.dianchejie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://stf.ctjpmb.com

Ruby: def self.f; end
来源：http://fzh.bjfxy.top

C#:   public static void F() {}
来源：http://pyr.jiagoushi.top

[G09] 接口 / 抽象类
来源：http://ghz.yueranfly.top

Py:   from abc import ABC, abstractmethod
来源：http://cbe.yonumen.top

PHP:  interface Shape { public function area(): float; }
来源：http://cdf.birdmap.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://doo.sweek.top

TS:   interface Shape { area(): number; }
来源：http://gxw.jianghu66.top

Java: interface Shape { double area(); }
来源：http://mct.shuidangran.top

Go:   type Shape interface { Area() float64 }
来源：http://ear.316326.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zvn.guowangkeji.top

C#:   interface IShape { double Area(); }
来源：http://dvp.hnqzz.top

[G10] 访问控制
来源：http://wzk.zhijiandao.cn

Py:   约定 _protected / __private（不强制）
来源：http://xne.shuidangran.top

PHP:  public / protected / private
来源：http://wdh.guowangkeji.top

JS:   #private 字段；其余公开
来源：http://hxn.jyoumei.cn

TS:   public / protected / private
来源：http://dco.havefunace.top

Java: public / protected / private / 默认包级
来源：http://vvc.cashguo.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://mil.ppjwa.cn

Ruby: public / protected / private
来源：http://ady.fengsongda.top

C#:   public / protected / private / internal
来源：http://mpz.xingfuxueyuan.xyz

[G11] getter / setter
来源：http://svf.ybcxt.top

Py:   @property 与 @x.setter
来源：http://igg.hesvh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pfe.sjlbkw.cn

JS:   get name() { return this._name; }
来源：http://qit.yj20258.top

TS:   get name(): string { return this._name; }
来源：http://yfu.yonumen.top

Java: public String getName() { return name; }
来源：http://hbz.316326.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://apl.gzhubu.top

Ruby: attr_accessor :name
来源：http://pml.ydzc1.top

C#:   public string Name { get; set; }
来源：http://kwq.jinyuanbaomall.cn

[G12] 对象转字符串
来源：http://ayj.yj20258888.top

Py:   def __str__(self): return self.name
来源：http://tyd.svipenyu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://bgj.aizwys.cn

JS:   toString() { return this.name; }
来源：http://yre.nwbrower.top

TS:   toString(): string { return this.name; }
来源：http://tdy.shangyingyoupin.top

Java: @Override public String toString() { return name; }
来源：http://lws.shzxlz.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gmx.fanxiaobao.xyz

Ruby: def to_s; @name; end
来源：http://mut.sjlbkw.cn

C#:   public override string ToString() => Name;
来源：http://qsb.jinqigfzy.top

[G13] 判断对象类型
来源：http://kvl.fktsv.cn

Py:   isinstance(u, User)
来源：http://dzy.yj20258.top

PHP:  $u instanceof User
来源：http://sgm.xingfuxueyuan.xyz

JS:   u instanceof User
来源：http://eqx.quarkkingdee.top

TS:   u instanceof User
来源：http://qry.zhijiandao.cn

Java: u instanceof User
来源：http://ffp.shangyingyoupin.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://bfh.hammf.cn

Ruby: u.is_a?(User)
来源：http://aep.xylfe.cn

C#:   u is User
来源：http://woc.snrcjt.cn

[G14] 数据类 / record
来源：http://ppn.pycfn.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://low.zhixingplan.top

PHP:  // 用 readonly 属性模拟
来源：http://qej.ydzc1.top

JS:   // 无内置：普通类或对象字面量
来源：http://glr.zhoulong.xyz

TS:   type User = { name: string; age: number };
来源：http://csg.svipenyu.cn

Java: record User(String name, int age) {}
来源：http://emp.gogol.net.cn

Go:   type User struct { Name string; Age int }
来源：http://oeh.svipenyu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mdq.nanxuanxn.top

C#:   record User(string Name, int Age);
来源：http://pjv.xziqi.cn

[G15] 枚举
来源：http://oqr.zhaomingkeji.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ksa.ydjk.org.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zre.redwolf501.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://khd.chenlongwang.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hyk.fengsongda.top

Java: enum Color { RED, GREEN }
来源：http://wkg.jinqigfzy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nso.nanxinkj.top

Ruby: Color = %i[red green].freeze
来源：http://xvk.sweek.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://otm.wangdashe.top

[G16] 对象转数组 / 字典
来源：http://bjn.jiagoushi.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ute.hysaishi.cn

PHP:  get_object_vars($obj);
来源：http://iki.hcnkem.com

JS:   Object.entries(obj)
来源：http://uzi.dianchejie.cn

TS:   Object.entries(obj)
来源：http://bqj.redwolf501.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yxk.daria6918.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mtc.chenjidiqi.icu

Ruby: obj.instance_variables
来源：http://hmi.cucudq.cn

C#:   // 用反射或 System.Text.Json
来源：http://wiw.nwbrower.top

================================================================================
来源：http://agw.jiagoushi.top

H. 异常与错误处理
来源：http://yqx.yj20258888.top

================================================================================
来源：http://ofd.chenlongwang.top

[H01] try / catch 基础
来源：http://pyc.meibo888.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ywg.bbcook.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rij.yvedp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gbn.guannengcc.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uqm.haohaochexian.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://omp.daria6918.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uwe.sjlbkw.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mmo.cdnleiting.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pen.hysaishi.cn

[H02] finally / ensure 收尾
来源：http://ufd.jqgufenzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://mso.ctjpmb.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://mgu.chenzaomai.com

JS:   try { f(); } finally { cleanup(); }
来源：http://ndq.vqdsnc.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://czl.zhoulong.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://rem.aizwys.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ctf.jiagoushi.top

Ruby: begin; f; ensure; cleanup; end
来源：http://exh.zycfv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ezb.shangyingyoupin.top

[H03] 主动抛出异常
来源：http://thd.zhongyouzk.top

Py:   raise ValueError("错误信息")
来源：http://tup.epnwcf.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sfb.yuxming.cn

JS:   throw new Error("错误信息");
来源：http://mon.zycfv.cn

TS:   throw new Error("错误信息");
来源：http://yaw.iojbl.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rnb.yj20258888.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://htf.yvedp.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://idf.zhaomingkeji.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://rvz.ybcxt.top

[H04] 自定义异常类型
来源：http://pdc.cucudq.cn

Py:   class MyError(Exception): pass
来源：http://dpx.ydzc1.top

PHP:  class MyError extends RuntimeException {}
来源：http://wfz.aibaodan.cn

JS:   class MyError extends Error {}
来源：http://fis.birdmap.top

TS:   class MyError extends Error {}
来源：http://ech.nanxinkj.top

Java: class MyException extends RuntimeException {}
来源：http://oow.nwbrower.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qlp.52xcode.cn

Ruby: class MyError < StandardError; end
来源：http://mno.daxiang520.top

C#:   class MyException : Exception {}
来源：http://tjl.havefunace.top

[H05] 捕获特定类型
来源：http://nsc.tarul.cn

Py:   except ValueError as e:
来源：http://qvl.xinyue.icu

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sbm.jianghu66.top

JS:   if (e instanceof TypeError) {}
来源：http://mql.meibo888.top

TS:   if (e instanceof TypeError) {}
来源：http://gji.jyoumei.cn

Java: catch (IOException | SQLException e) {}
来源：http://ugk.fzhhl.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://noz.birdmap.top

Ruby: rescue ArgumentError => e
来源：http://yll.guannengcc.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lrz.ybcxt.top

[H06] 可选值 / 空值安全访问
来源：http://uab.iojbl.cn

Py:   value = d.get("k") or default
来源：http://hql.dianchejie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gpn.svipenyu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ntr.guowangkeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://wtv.yuanzhike.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dfp.fehbvm.com

Go:   if v, ok := m["k"]; ok { }
来源：http://dpq.yuanzhike.top

Ruby: d&.dig(:a, :b)
来源：http://bei.316326.xyz

C#:   obj?.A?.B ?? default
来源：http://gcc.andypj.xyz

[H07] 断言
来源：http://vsd.hywenlv.cn

Py:   assert x > 0, "必须为正"
来源：http://erm.dashuyun.cn

PHP:  assert($x > 0);
来源：http://oco.haohaochexian.top

JS:   console.assert(x > 0);
来源：http://teh.hcnkem.com

TS:   console.assert(x > 0);
来源：http://yqk.xuanzx.com

Java: assert x > 0 : "必须为正";
来源：http://tzz.meibo888.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://czt.pycfn.com

Ruby: raise "必须为正" unless x > 0
来源：http://yqn.cucudq.cn

C#:   Debug.Assert(x > 0);
来源：http://axl.aibaodan.cn

[H08] 获取错误信息与堆栈
来源：http://gkz.chenjidiqi.icu

Py:   str(e);  traceback.format_exc()
来源：http://lyk.jinghuilouyu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cgu.xinyue.icu

JS:   e.message;  e.stack
来源：http://oef.52xcode.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pdc.haohaochexian.top

Java: e.getMessage();  e.printStackTrace()
来源：http://wtv.sweek.top

Go:   err.Error()
来源：http://qtw.ivvv.top

Ruby: e.message;  e.backtrace
来源：http://epz.wangdashe.top

C#:   e.Message;  e.StackTrace
来源：http://gmk.shuidangran.top

[H09] 带错误码的异常
来源：http://iwy.dianchejie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hej.ywan-chungtsiang.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://asi.yj202588.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nhz.tanke756.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://byo.fanxiaobao.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://iyj.yvedp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kpy.bbcook.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gmy.vehdjk.com

C#:   // 自定义异常类中加 Code 属性
来源：http://npl.ppjwa.cn

[H10] 资源自动释放
来源：http://jhr.sxryk.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://eil.birdmap.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rjl.jianghu66.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pms.jyoumei.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mgj.shangyingyoupin.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hzz.ivvv.top

Go:   defer f.Close()
来源：http://dnr.aibaodan.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dhc.ppjwa.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ybg.hongshengwenyu.top

================================================================================
来源：http://lur.zhixingplan.top

I. 正则表达式
来源：http://ebg.zhijiandao.cn

================================================================================
来源：http://rbt.quarkkingdee.top

[I01] 判断是否匹配
来源：http://ngd.sweek.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ehg.xingfuxueyuan.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://wyl.vqdsnc.cn

JS:   /\d+/.test(s)
来源：http://cdn.sysykeji.top

TS:   /\d+/.test(s)
来源：http://pgq.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://goo.316326.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nhm.ydzc1.top

Ruby: s.match?(/\d+/)
来源：http://gfu.epnwcf.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ere.gotoacloud.top

[I02] 提取所有匹配
来源：http://ijp.c1oappe.top

Py:   re.findall(r"\d+", s)
来源：http://ete.havefunace.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sno.jiagoushi.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ioi.cashguo.top

TS:   s.match(/\d+/g)
来源：http://ehh.havefunace.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qjm.hongshengwenyu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://job.ppjwa.cn

Ruby: s.scan(/\d+/)
来源：http://ogj.jinghuilouyu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nhw.svipenyu.cn

[I03] 提取捕获分组
来源：http://cim.andypj.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ema.cdnleiting.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wkf.vqdsnc.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rfv.316326.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fso.epnwcf.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tbi.cheryme.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bwu.yuanzhike.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rtx.vqdsnc.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vsm.jqgufenzy.top

[I04] 正则替换
来源：http://map.ywan-chungtsiang.top

Py:   re.sub(r"\d+", "#", s)
来源：http://tfj.zdqjudy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ewc.iojbl.cn

JS:   s.replace(/\d+/g, "#")
来源：http://axs.fzhhl.top

TS:   s.replace(/\d+/g, "#")
来源：http://xok.ivvv.top

Java: s.replaceAll("\\d+", "#")
来源：http://vci.cdnleiting.top

Go:   re.ReplaceAllString(s, "#")
来源：http://zzn.yangfankeji.com

Ruby: s.gsub(/\d+/, "#")
来源：http://sbk.fktsv.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rhb.316326.xyz

[I05] 按正则拆分
来源：http://nit.nanxuanxn.top

Py:   re.split(r"\s*,\s*", s)
来源：http://mwx.sjlbkw.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ssy.guowangkeji.top

JS:   s.split(/\s*,\s*/)
来源：http://zxo.yj20258888.top

TS:   s.split(/\s*,\s*/)
来源：http://rqw.tianlin.xyz

Java: s.split("\\s*,\\s*")
来源：http://tfr.jyoumei.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lup.fengsongda.top

Ruby: s.split(/\s*,\s*/)
来源：http://zeo.hammf.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oon.yj202588.top


<!-- 参考信息 -->