代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jxk.jinqigufen.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nyy.ydzc1.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kky.fengsongda.top

[F12] CSV 读写
来源：http://yud.fanxiaobao.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://grq.yanxiufei.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zld.ppjwa.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zla.nanxinkj.top

TS:   // 同上
来源：http://kkl.hcnkem.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ibt.dashuyun.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oxw.pengpengdd.cyou

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eec.hnqzz.top

C#:   // 无内置：用 CsvHelper 库
来源：http://iby.sjlbkw.cn

================================================================================
来源：http://idi.zhoulong.xyz

G. 面向对象
来源：http://uue.tianlin.xyz

================================================================================
来源：http://lol.yangfankeji.com

[G01] 定义类
来源：http://opd.ywan-chungtsiang.top

Py:   class User: pass
来源：http://dnn.chenjidiqi.icu

PHP:  class User {}
来源：http://ksq.fzhhl.top

JS:   class User {}
来源：http://nhk.sysykeji.top

TS:   class User { name: string = ""; }
来源：http://ngt.tarul.cn

Java: class User {}
来源：http://htx.9152youxi.cn

Go:   type User struct { Name string }
来源：http://bmx.aibaodan.cn

Ruby: class User; end
来源：http://ruf.shuidangran.top

C#:   class User {}
来源：http://srz.xingfuxueyuan.xyz

[G02] 构造函数
来源：http://kfh.jianghu66.top

Py:   def __init__(self, name): self.name = name
来源：http://bhh.tian-w.cn

PHP:  public function __construct(public string $name) {}
来源：http://lgl.daxiang520.top

JS:   constructor(name) { this.name = name; }
来源：http://xpm.gogol.net.cn

TS:   constructor(public name: string) {}
来源：http://gks.jinqigfzy.top

Java: User(String name) { this.name = name; }
来源：http://bxb.kuanghao11.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gsl.zhijiandao.cn

Ruby: def initialize(name); @name = name; end
来源：http://nsy.jqgufenzy.top

C#:   public User(string name) { Name = name; }
来源：http://lub.shuidangran.top

[G03] 实例属性
来源：http://tyk.yongpay.top

Py:   self.name = "x"
来源：http://psm.yanxiufei.cn

PHP:  public string $name = "x";
来源：http://xeg.andypj.xyz

JS:   this.name = "x";
来源：http://qwh.mhx1999.top

TS:   name: string = "x";
来源：http://fgd.zdbjq.cn

Java: private String name;
来源：http://qri.birdmap.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://npo.vehdjk.com

Ruby: @name = "x"
来源：http://ozt.tarul.cn

C#:   public string Name { get; set; } = "x";
来源：http://zku.mhx1999.top

[G04] 定义方法
来源：http://ycg.zdbjq.cn

Py:   def greet(self): return self.name
来源：http://vjk.yanxiufei.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ajy.yj202588.top

JS:   greet() { return this.name; }
来源：http://mqi.uphjek.com

TS:   greet(): string { return this.name; }
来源：http://cqn.tarul.cn

Java: String greet() { return name; }
来源：http://wtb.yueranfly.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://opv.yongpay.top

Ruby: def greet; @name; end
来源：http://qfs.jiagoushi.top

C#:   public string Greet() => Name;
来源：http://mez.tanke756.top

[G05] 继承
来源：http://yaq.316326.xyz

Py:   class Admin(User): pass
来源：http://usb.chenjidiqi.icu

PHP:  class Admin extends User {}
来源：http://xjn.pengpengdd.cyou

JS:   class Admin extends User {}
来源：http://psv.aibaodan.cn

TS:   class Admin extends User {}
来源：http://wec.jinghuilouyu.cn

Java: class Admin extends User {}
来源：http://fsm.jinyuanbaomall.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rvm.guannengcc.top

Ruby: class Admin < User; end
来源：http://laf.zdbjq.cn

C#:   class Admin : User {}
来源：http://kvj.shanyushiyangtech.top

[G06] 重写方法
来源：http://ptt.pengpengdd.cyou

Py:   def greet(self): return "admin"
来源：http://lkz.jinqigfzy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://tbp.yueranfly.top

JS:   greet() { return "admin"; }
来源：http://yjv.snrcjt.cn

TS:   greet(): string { return "admin"; }
来源：http://kwj.gogol.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://aao.yongpay.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ntn.hammf.cn

Ruby: def greet; "admin"; end
来源：http://szn.hesvh.cn

C#:   public override string Greet() => "admin";
来源：http://tln.guannengcc.top

[G07] 调用父类方法
来源：http://ltu.hcnkem.com

Py:   super().greet()
来源：http://lsw.bjfxy.top

PHP:  parent::greet();
来源：http://uhd.zycfv.cn

JS:   super.greet();
来源：http://qyp.jinghuilouyu.cn

TS:   super.greet();
来源：http://kth.tianlin.xyz

Java: super.greet();
来源：http://mqv.yuxming.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rdp.316326.xyz

Ruby: super
来源：http://uyy.dashuyun.cn

C#:   base.Greet();
来源：http://lyj.smart0.xyz

[G08] 静态方法与属性
来源：http://yeh.hfpthk.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rmz.pengpengdd.cyou

PHP:  public static function f() {}
来源：http://gzb.fanxiaobao.xyz

JS:   static f() {}
来源：http://vyk.316326.xyz

TS:   static f(): void {}
来源：http://sto.yj20258.top

Java: static void f() {}
来源：http://mbm.fehbvm.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://noy.jinyuanbaomall.cn

Ruby: def self.f; end
来源：http://svl.wangshuangyany.cn

C#:   public static void F() {}
来源：http://xde.epnwcf.com

[G09] 接口 / 抽象类
来源：http://goh.birdmap.top

Py:   from abc import ABC, abstractmethod
来源：http://qoy.quarkkingdee.top

PHP:  interface Shape { public function area(): float; }
来源：http://uca.wangshuangyany.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://sgs.jyoumei.cn

TS:   interface Shape { area(): number; }
来源：http://hsb.ppjwa.cn

Java: interface Shape { double area(); }
来源：http://bbp.chenjidiqi.icu

Go:   type Shape interface { Area() float64 }
来源：http://cxn.hnqzz.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pae.jinyuanbaomall.cn

C#:   interface IShape { double Area(); }
来源：http://hie.jqgfzy.top

[G10] 访问控制
来源：http://bzi.cheryme.top

Py:   约定 _protected / __private（不强制）
来源：http://ljp.gogol.net.cn

PHP:  public / protected / private
来源：http://vej.pengpengdd.cyou

JS:   #private 字段；其余公开
来源：http://tib.yj202588.top

TS:   public / protected / private
来源：http://yhg.sjlbkw.cn

Java: public / protected / private / 默认包级
来源：http://bsq.wangshuangyany.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lpj.xuanzx.com

Ruby: public / protected / private
来源：http://niq.jqgufenzy.top

C#:   public / protected / private / internal
来源：http://irw.snrcjt.cn

[G11] getter / setter
来源：http://uyr.andypj.xyz

Py:   @property 与 @x.setter
来源：http://xxf.fanxiaobao.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://xva.hammf.cn

JS:   get name() { return this._name; }
来源：http://pop.sweek.top

TS:   get name(): string { return this._name; }
来源：http://kzn.pycfn.com

Java: public String getName() { return name; }
来源：http://auz.daxiang520.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://qlq.jinghuilouyu.cn

Ruby: attr_accessor :name
来源：http://blg.xuetiantiany.cn

C#:   public string Name { get; set; }
来源：http://xgr.jinqigfzy.top

[G12] 对象转字符串
来源：http://osk.smart0.xyz

Py:   def __str__(self): return self.name
来源：http://jzd.jyoumei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jmu.wangshuangyany.cn

JS:   toString() { return this.name; }
来源：http://xfr.daxiang520.top

TS:   toString(): string { return this.name; }
来源：http://tpd.zhiwuduotai.top

Java: @Override public String toString() { return name; }
来源：http://zni.sxryk.cn

Go:   func (u User) String() string { return u.Name }
来源：http://flm.cashguo.top

Ruby: def to_s; @name; end
来源：http://gho.quarkkingdee.top

C#:   public override string ToString() => Name;
来源：http://ewa.fengsongda.top

[G13] 判断对象类型
来源：http://ggf.havefunace.top

Py:   isinstance(u, User)
来源：http://sjj.jinghuilouyu.cn

PHP:  $u instanceof User
来源：http://fpq.xinyue.icu

JS:   u instanceof User
来源：http://tvr.chenjidiqi.icu

TS:   u instanceof User
来源：http://qqh.yanxiufei.cn

Java: u instanceof User
来源：http://fdj.ehwqpu.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://vqe.sweek.top

Ruby: u.is_a?(User)
来源：http://qeb.yongpay.top

C#:   u is User
来源：http://sop.jinyuanbaomall.cn

[G14] 数据类 / record
来源：http://iab.fanxiaobao.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wro.dashuyun.cn

PHP:  // 用 readonly 属性模拟
来源：http://uqc.shangyingyoupin.top

JS:   // 无内置：普通类或对象字面量
来源：http://fgb.meibo888.top

TS:   type User = { name: string; age: number };
来源：http://dgh.cashguo.top

Java: record User(String name, int age) {}
来源：http://iur.zdbjq.cn

Go:   type User struct { Name string; Age int }
来源：http://qfg.jqgufenzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://miv.jqgfzy.top

C#:   record User(string Name, int Age);
来源：http://ild.xuetiantiany.cn

[G15] 枚举
来源：http://akt.vqdsnc.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zej.cdnleiting.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://mzq.c1oappe.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zft.bbcook.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tpn.jlsjyb.cn

Java: enum Color { RED, GREEN }
来源：http://mhl.hnxiangtu.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zum.birdmap.top

Ruby: Color = %i[red green].freeze
来源：http://uzv.xylfe.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gkn.fzhhl.top

[G16] 对象转数组 / 字典
来源：http://jcd.fehbvm.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mrx.cashguo.top

PHP:  get_object_vars($obj);
来源：http://peh.yueranfly.top

JS:   Object.entries(obj)
来源：http://ugm.tianlin.xyz

TS:   Object.entries(obj)
来源：http://kns.havefunace.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://oda.gzhubu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://lpa.yangfankeji.com

Ruby: obj.instance_variables
来源：http://mbv.tian-w.cn

C#:   // 用反射或 System.Text.Json
来源：http://lei.ydjk.org.cn

================================================================================
来源：http://vti.chenzaomai.com

H. 异常与错误处理
来源：http://ssk.xuanzx.com

================================================================================
来源：http://qwo.sysykeji.top

[H01] try / catch 基础
来源：http://tqi.kuanghao11.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kaa.hywenlv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://unf.jqgfzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cph.jinqigufen.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tqo.0kj1m.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yjv.c1oappe.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tqf.yonumen.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blh.shangyingyoupin.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://iae.aibaodan.cn

[H02] finally / ensure 收尾
来源：http://ynk.dashuyun.cn

Py:   try: f()⏎finally: cleanup()
来源：http://uok.9152youxi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zdl.hcnkem.com

JS:   try { f(); } finally { cleanup(); }
来源：http://uvi.tian-w.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yux.smart0.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://pwp.haohaochexian.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://kwf.jianghu66.top

Ruby: begin; f; ensure; cleanup; end
来源：http://fvs.hfpthk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tgp.hammf.cn

[H03] 主动抛出异常
来源：http://sxz.9152youxi.cn

Py:   raise ValueError("错误信息")
来源：http://nre.ppjwa.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://czh.52xcode.cn

JS:   throw new Error("错误信息");
来源：http://tmq.zhaomingkeji.xyz

TS:   throw new Error("错误信息");
来源：http://wnt.shuidangran.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://jvx.zhoulong.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cht.hcnkem.com

Ruby: raise ArgumentError, "错误信息"
来源：http://tpt.dashuyun.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bat.fanxiaobao.xyz

[H04] 自定义异常类型
来源：http://akw.yueranfly.top

Py:   class MyError(Exception): pass
来源：http://nbc.tianlin.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://gbj.sjlbkw.cn

JS:   class MyError extends Error {}
来源：http://uwy.hnxiangtu.top

TS:   class MyError extends Error {}
来源：http://kns.gaohongyu789.top

Java: class MyException extends RuntimeException {}
来源：http://bro.shzxlz.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wcv.zdbjq.cn

Ruby: class MyError < StandardError; end
来源：http://hyw.ctjpmb.com

C#:   class MyException : Exception {}
来源：http://uno.hesvh.cn

[H05] 捕获特定类型
来源：http://rwp.redwolf501.top

Py:   except ValueError as e:
来源：http://fyy.tarul.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ctx.jqgfzy.top

JS:   if (e instanceof TypeError) {}
来源：http://jae.sxryk.cn

TS:   if (e instanceof TypeError) {}
来源：http://qoq.yanxiufei.cn

Java: catch (IOException | SQLException e) {}
来源：http://uct.hysaishi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://igc.jlsjyb.cn

Ruby: rescue ArgumentError => e
来源：http://ibk.hfpthk.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uys.andypj.xyz

[H06] 可选值 / 空值安全访问
来源：http://pts.pycfn.com

Py:   value = d.get("k") or default
来源：http://oup.redwolf501.top

PHP:  $v = $d["k"] ?? null;
来源：http://mak.9152youxi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pje.kuanghao11.cn

TS:   obj?.a?.b;  d ?? default
来源：http://kct.zhongyouzk.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://urv.havefunace.top

Go:   if v, ok := m["k"]; ok { }
来源：http://qty.fzhhl.top

Ruby: d&.dig(:a, :b)
来源：http://oeb.tian-w.cn

C#:   obj?.A?.B ?? default
来源：http://mvp.jyoumei.cn

[H07] 断言
来源：http://qtg.nanxuanxn.top

Py:   assert x > 0, "必须为正"
来源：http://bnk.xuetiantiany.cn

PHP:  assert($x > 0);
来源：http://ebz.yvedp.cn

JS:   console.assert(x > 0);
来源：http://isf.mhx1999.top

TS:   console.assert(x > 0);
来源：http://osp.yvedp.cn

Java: assert x > 0 : "必须为正";
来源：http://cdv.hesvh.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zbu.svipenyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qyh.hywenlv.cn

C#:   Debug.Assert(x > 0);
来源：http://dgw.yj20258888.top

[H08] 获取错误信息与堆栈
来源：http://ger.xuanzx.com

Py:   str(e);  traceback.format_exc()
来源：http://xcr.zhongyouzk.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jhm.cdnleiting.top

JS:   e.message;  e.stack
来源：http://ihr.hysaishi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dff.sxryk.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://otd.meibo888.top

Go:   err.Error()
来源：http://emb.fzhhl.top

Ruby: e.message;  e.backtrace
来源：http://lnm.gogol.net.cn

C#:   e.Message;  e.StackTrace
来源：http://mxa.nanxuanxn.top

[H09] 带错误码的异常
来源：http://xni.redwolf501.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cep.gotoacloud.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://hzp.xingfuxueyuan.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qld.zhoulong.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tzf.cucudq.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dvl.xuetiantiany.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cuv.ywan-chungtsiang.top

Ruby: raise MyError.new("fail", 500)
来源：http://lla.epnwcf.com

C#:   // 自定义异常类中加 Code 属性
来源：http://ruf.vehdjk.com

[H10] 资源自动释放
来源：http://vqz.havefunace.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://thk.vehdjk.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lam.quarkkingdee.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jbf.gzhubu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vld.daria6918.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ecw.feifeiyinyue.top

Go:   defer f.Close()
来源：http://zjc.yonumen.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://msk.ppjwa.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://goc.bjfxy.top

================================================================================
来源：http://pig.pycfn.com

I. 正则表达式
来源：http://omy.wangdashe.top

================================================================================
来源：http://isw.fktsv.cn

[I01] 判断是否匹配
来源：http://ilz.vehdjk.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://plp.gaohongyu789.top

PHP:  preg_match('/\d+/', $s);
来源：http://nor.dashuyun.cn

JS:   /\d+/.test(s)
来源：http://wen.wangshuangyany.cn

TS:   /\d+/.test(s)
来源：http://jyb.zdbjq.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cnh.pengpengdd.cyou

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://iyq.wangshuangyany.cn

Ruby: s.match?(/\d+/)
来源：http://tnz.epnwcf.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sra.fehbvm.com

[I02] 提取所有匹配
来源：http://hkj.fengsongda.top

Py:   re.findall(r"\d+", s)
来源：http://hjt.jinghuilouyu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nca.jinghuilouyu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xfk.yanxiufei.cn

TS:   s.match(/\d+/g)
来源：http://pxu.epnwcf.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://izq.yonumen.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://udq.yj20258888.top

Ruby: s.scan(/\d+/)
来源：http://unf.fengsongda.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mfc.snrcjt.cn

[I03] 提取捕获分组
来源：http://sud.shanyushiyangkeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ree.tarul.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://poy.zdqjudy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uzb.cqqwz.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bim.vqdsnc.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kpo.sweek.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bdj.guannengcc.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://eca.yongpay.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://atc.xuanzx.com

[I04] 正则替换
来源：http://bhu.shanyushiyangtech.top

Py:   re.sub(r"\d+", "#", s)
来源：http://fke.hammf.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tqx.9152youxi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zsu.cucudq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hlj.sysykeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://shi.jinyuanbaomall.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sdw.zhoulong.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://ywp.gogol.net.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qkr.cdnleiting.top

[I05] 按正则拆分
来源：http://liv.xylfe.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qfb.sufxvd.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vqt.ybcxt.top

JS:   s.split(/\s*,\s*/)
来源：http://ezx.havefunace.top

TS:   s.split(/\s*,\s*/)
来源：http://pto.yanxiufei.cn

Java: s.split("\\s*,\\s*")
来源：http://lim.hnqzz.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qwj.fanxiaobao.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://lio.tanke756.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uvl.zhongyouzk.top


<!-- 参考信息 -->