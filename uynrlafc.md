代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://eqr.fktsv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lxk.yonumen.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://crg.nanxinkj.top

TS:   // 同上
来源：http://hrg.nanxuanxn.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wex.dianchejie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jrz.nanxuanxn.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vdo.zdbjq.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://izn.fktsv.cn

================================================================================
来源：http://ggx.zhijiandao.cn

G. 面向对象
来源：http://uau.yanxiufei.cn

================================================================================
来源：http://xzw.svipenyu.cn

[G01] 定义类
来源：http://vhp.ctjpmb.com

Py:   class User: pass
来源：http://xey.zhengqikj.top

PHP:  class User {}
来源：http://svh.bjfxy.top

JS:   class User {}
来源：http://nur.hnqzz.top

TS:   class User { name: string = ""; }
来源：http://frg.sweek.top

Java: class User {}
来源：http://rqr.hesvh.cn

Go:   type User struct { Name string }
来源：http://mqs.hfpthk.cn

Ruby: class User; end
来源：http://nds.yvedp.cn

C#:   class User {}
来源：http://aos.yongpay.top

[G02] 构造函数
来源：http://kyu.jinghuilouyu.cn

Py:   def __init__(self, name): self.name = name
来源：http://jgz.gaohongyu789.top

PHP:  public function __construct(public string $name) {}
来源：http://fpc.wangshuangyany.cn

JS:   constructor(name) { this.name = name; }
来源：http://xyc.daxiang520.top

TS:   constructor(public name: string) {}
来源：http://lzq.vqdsnc.cn

Java: User(String name) { this.name = name; }
来源：http://csr.hysaishi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lsr.52xcode.cn

Ruby: def initialize(name); @name = name; end
来源：http://ddz.mhx1999.top

C#:   public User(string name) { Name = name; }
来源：http://xty.316326.xyz

[G03] 实例属性
来源：http://lsv.yfazqb.com

Py:   self.name = "x"
来源：http://exm.52xcode.cn

PHP:  public string $name = "x";
来源：http://kch.c1oappe.top

JS:   this.name = "x";
来源：http://gfa.xuetiantiany.cn

TS:   name: string = "x";
来源：http://yqy.yonumen.top

Java: private String name;
来源：http://zua.tianlin.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jel.smart0.xyz

Ruby: @name = "x"
来源：http://tvb.jinqigufen.top

C#:   public string Name { get; set; } = "x";
来源：http://ucd.yanxiufei.cn

[G04] 定义方法
来源：http://wmv.haohaochexian.top

Py:   def greet(self): return self.name
来源：http://ikf.yfazqb.com

PHP:  public function greet(): string { return $this->name; }
来源：http://vhw.sweek.top

JS:   greet() { return this.name; }
来源：http://guk.zhongyouzk.top

TS:   greet(): string { return this.name; }
来源：http://zdp.aibaodan.cn

Java: String greet() { return name; }
来源：http://vvu.hnxiangtu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://obf.yongpay.top

Ruby: def greet; @name; end
来源：http://iej.zhixingplan.top

C#:   public string Greet() => Name;
来源：http://ica.chenlongwang.top

[G05] 继承
来源：http://jga.ydzc1.top

Py:   class Admin(User): pass
来源：http://nwl.yangfankeji.com

PHP:  class Admin extends User {}
来源：http://lwi.316326.xyz

JS:   class Admin extends User {}
来源：http://nmf.uphjek.com

TS:   class Admin extends User {}
来源：http://tcm.fzhhl.top

Java: class Admin extends User {}
来源：http://kxp.xingfuxueyuan.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yka.guannengcc.top

Ruby: class Admin < User; end
来源：http://zpv.shuidangran.top

C#:   class Admin : User {}
来源：http://oeh.fzhhl.top

[G06] 重写方法
来源：http://snz.xinyue.icu

Py:   def greet(self): return "admin"
来源：http://tbg.hesvh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ojh.yuxming.cn

JS:   greet() { return "admin"; }
来源：http://avv.yuanzhike.top

TS:   greet(): string { return "admin"; }
来源：http://spo.snrcjt.cn

Java: @Override String greet() { return "admin"; }
来源：http://agc.c1oappe.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mzf.xinyue.icu

Ruby: def greet; "admin"; end
来源：http://kyk.zhongyouzk.top

C#:   public override string Greet() => "admin";
来源：http://xkd.redwolf501.top

[G07] 调用父类方法
来源：http://muz.zdbjq.cn

Py:   super().greet()
来源：http://mmm.zdqjudy.top

PHP:  parent::greet();
来源：http://rbv.hongshengwenyu.top

JS:   super.greet();
来源：http://oyz.yj20258888.top

TS:   super.greet();
来源：http://svr.hcnkem.com

Java: super.greet();
来源：http://hfz.jyoumei.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://san.zhixingplan.top

Ruby: super
来源：http://hkq.zycfv.cn

C#:   base.Greet();
来源：http://tgu.hysaishi.cn

[G08] 静态方法与属性
来源：http://fpi.dashuyun.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wlk.sweek.top

PHP:  public static function f() {}
来源：http://trn.0kj1m.cn

JS:   static f() {}
来源：http://lei.cqqwz.cn

TS:   static f(): void {}
来源：http://jgw.jinghuilouyu.cn

Java: static void f() {}
来源：http://wng.xinyue.icu

Go:   // 无 static：用包级函数，按包名调用
来源：http://jlx.daxiang520.top

Ruby: def self.f; end
来源：http://hxx.ywan-chungtsiang.top

C#:   public static void F() {}
来源：http://ove.hesvh.cn

[G09] 接口 / 抽象类
来源：http://equ.redwolf501.top

Py:   from abc import ABC, abstractmethod
来源：http://buu.zdqjudy.top

PHP:  interface Shape { public function area(): float; }
来源：http://sjx.hysaishi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fyz.tanke756.top

TS:   interface Shape { area(): number; }
来源：http://snl.shuidangran.top

Java: interface Shape { double area(); }
来源：http://ore.52xcode.cn

Go:   type Shape interface { Area() float64 }
来源：http://jmz.ehwqpu.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://eus.tian-w.cn

C#:   interface IShape { double Area(); }
来源：http://rzo.jianghu66.top

[G10] 访问控制
来源：http://swz.hywenlv.cn

Py:   约定 _protected / __private（不强制）
来源：http://oyr.bjfxy.top

PHP:  public / protected / private
来源：http://uxs.yj202588.top

JS:   #private 字段；其余公开
来源：http://grt.gogol.net.cn

TS:   public / protected / private
来源：http://sjo.snrcjt.cn

Java: public / protected / private / 默认包级
来源：http://vrc.jinqigufen.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://udq.ctjpmb.com

Ruby: public / protected / private
来源：http://qku.chenzaomai.com

C#:   public / protected / private / internal
来源：http://srq.hcnkem.com

[G11] getter / setter
来源：http://vtp.jiagoushi.top

Py:   @property 与 @x.setter
来源：http://wdy.jqgfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dgf.xziqi.cn

JS:   get name() { return this._name; }
来源：http://sgb.wangshuangyany.cn

TS:   get name(): string { return this._name; }
来源：http://wun.zhaomingkeji.xyz

Java: public String getName() { return name; }
来源：http://ggh.aizwys.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tku.zdqjudy.top

Ruby: attr_accessor :name
来源：http://xdu.yongpay.top

C#:   public string Name { get; set; }
来源：http://pct.cashguo.top

[G12] 对象转字符串
来源：http://ueo.hongshengwenyu.top

Py:   def __str__(self): return self.name
来源：http://ipo.zhongyouzk.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://yvh.fehbvm.com

JS:   toString() { return this.name; }
来源：http://ozw.shzxlz.cn

TS:   toString(): string { return this.name; }
来源：http://bjk.xinyue.icu

Java: @Override public String toString() { return name; }
来源：http://tiz.bbcook.cn

Go:   func (u User) String() string { return u.Name }
来源：http://sla.ctjpmb.com

Ruby: def to_s; @name; end
来源：http://poz.birdmap.top

C#:   public override string ToString() => Name;
来源：http://obz.nanxuanxn.top

[G13] 判断对象类型
来源：http://nsd.shuidangran.top

Py:   isinstance(u, User)
来源：http://vuu.wangdashe.top

PHP:  $u instanceof User
来源：http://gfv.haohaochexian.top

JS:   u instanceof User
来源：http://gik.gogol.net.cn

TS:   u instanceof User
来源：http://fiy.9152youxi.cn

Java: u instanceof User
来源：http://fyd.sysykeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://wpp.ppjwa.cn

Ruby: u.is_a?(User)
来源：http://whe.yj202588.top

C#:   u is User
来源：http://lde.jyoumei.cn

[G14] 数据类 / record
来源：http://pfz.jinghuilouyu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://esf.shangyingyoupin.top

PHP:  // 用 readonly 属性模拟
来源：http://udc.guannengcc.top

JS:   // 无内置：普通类或对象字面量
来源：http://twm.hywenlv.cn

TS:   type User = { name: string; age: number };
来源：http://hww.ehwqpu.com

Java: record User(String name, int age) {}
来源：http://duu.ivvv.top

Go:   type User struct { Name string; Age int }
来源：http://uhd.nwbrower.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lpe.yuanzhike.top

C#:   record User(string Name, int Age);
来源：http://jis.xinyue.icu

[G15] 枚举
来源：http://znp.sjlbkw.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://erv.jlsjyb.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://czx.xuanzx.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rsj.hnqzz.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qys.guowangkeji.top

Java: enum Color { RED, GREEN }
来源：http://frb.jqgufenzy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bsf.kuanghao11.cn

Ruby: Color = %i[red green].freeze
来源：http://bzq.guannengcc.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bqc.birdmap.top

[G16] 对象转数组 / 字典
来源：http://igu.pengpengdd.cyou

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fpz.316326.xyz

PHP:  get_object_vars($obj);
来源：http://rea.jiagoushi.top

JS:   Object.entries(obj)
来源：http://fsz.hesvh.cn

TS:   Object.entries(obj)
来源：http://skz.andypj.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cpe.yonumen.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ryk.hammf.cn

Ruby: obj.instance_variables
来源：http://ccn.zycfv.cn

C#:   // 用反射或 System.Text.Json
来源：http://lqf.9152youxi.cn

================================================================================
来源：http://pmv.andypj.xyz

H. 异常与错误处理
来源：http://vxm.chenlongwang.top

================================================================================
来源：http://szr.hcnkem.com

[H01] try / catch 基础
来源：http://hvt.yfazqb.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://odr.0kj1m.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hxs.cashguo.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ayy.hnxiangtu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://los.cashguo.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pgj.cashguo.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ifr.guowangkeji.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hxs.nwbrower.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vre.xuetiantiany.cn

[H02] finally / ensure 收尾
来源：http://gcs.aizwys.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zxp.ywan-chungtsiang.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://tzi.gogol.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://nod.cheryme.top

TS:   try { f(); } finally { cleanup(); }
来源：http://csa.yonumen.top

Java: try { f(); } finally { cleanup(); }
来源：http://cqa.xziqi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://akn.jianghu66.top

Ruby: begin; f; ensure; cleanup; end
来源：http://eqh.jiagoushi.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ayu.haohaochexian.top

[H03] 主动抛出异常
来源：http://ffx.vehdjk.com

Py:   raise ValueError("错误信息")
来源：http://vkx.jinghuilouyu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://umg.sjlbkw.cn

JS:   throw new Error("错误信息");
来源：http://krk.zdbjq.cn

TS:   throw new Error("错误信息");
来源：http://frs.ehwqpu.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://upb.cheryme.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ohq.yj20258888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://lez.9152youxi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://czh.zhongyouzk.top

[H04] 自定义异常类型
来源：http://yfv.hcnkem.com

Py:   class MyError(Exception): pass
来源：http://jos.ywan-chungtsiang.top

PHP:  class MyError extends RuntimeException {}
来源：http://scz.tarul.cn

JS:   class MyError extends Error {}
来源：http://trp.cdnleiting.top

TS:   class MyError extends Error {}
来源：http://vsx.tian-w.cn

Java: class MyException extends RuntimeException {}
来源：http://jkj.zdqjudy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://crp.jinqigfzy.top

Ruby: class MyError < StandardError; end
来源：http://rjw.daria6918.cn

C#:   class MyException : Exception {}
来源：http://qgf.zdbjq.cn

[H05] 捕获特定类型
来源：http://uma.ivvv.top

Py:   except ValueError as e:
来源：http://csm.chenjidiqi.icu

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ojs.wangdashe.top

JS:   if (e instanceof TypeError) {}
来源：http://pvt.yfazqb.com

TS:   if (e instanceof TypeError) {}
来源：http://hal.smart0.xyz

Java: catch (IOException | SQLException e) {}
来源：http://vty.0kj1m.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://brc.cashguo.top

Ruby: rescue ArgumentError => e
来源：http://hjb.hesvh.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oha.ydzc1.top

[H06] 可选值 / 空值安全访问
来源：http://tcc.feifeiyinyue.top

Py:   value = d.get("k") or default
来源：http://cqe.xingfuxueyuan.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://xld.yanxiufei.cn

JS:   obj?.a?.b;  d ?? default
来源：http://tak.zhijiandao.cn

TS:   obj?.a?.b;  d ?? default
来源：http://kcc.zdbjq.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pxl.tianlin.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://rxq.hnxiangtu.top

Ruby: d&.dig(:a, :b)
来源：http://ndo.jinqigufen.top

C#:   obj?.A?.B ?? default
来源：http://twm.bjfxy.top

[H07] 断言
来源：http://pef.hnqzz.top

Py:   assert x > 0, "必须为正"
来源：http://xqx.gotoacloud.top

PHP:  assert($x > 0);
来源：http://hso.snrcjt.cn

JS:   console.assert(x > 0);
来源：http://pyk.hcnkem.com

TS:   console.assert(x > 0);
来源：http://ucl.yj202588.top

Java: assert x > 0 : "必须为正";
来源：http://stq.xuanzx.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tdm.chenzaomai.com

Ruby: raise "必须为正" unless x > 0
来源：http://che.hesvh.cn

C#:   Debug.Assert(x > 0);
来源：http://fnw.chenzaomai.com

[H08] 获取错误信息与堆栈
来源：http://aff.316326.xyz

Py:   str(e);  traceback.format_exc()
来源：http://ypb.pengpengdd.cyou

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yfv.feifeiyinyue.top

JS:   e.message;  e.stack
来源：http://cos.shzxlz.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://lqo.vqdsnc.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bcp.hesvh.cn

Go:   err.Error()
来源：http://mec.yueranfly.top

Ruby: e.message;  e.backtrace
来源：http://jkb.yvedp.cn

C#:   e.Message;  e.StackTrace
来源：http://zwp.zhengqikj.top

[H09] 带错误码的异常
来源：http://ahu.ppjwa.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tru.jqgfzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://feh.fzhhl.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ycn.hnqzz.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vkm.quarkkingdee.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ewl.fktsv.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://koq.jinyuanbaomall.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fik.hcnkem.com

C#:   // 自定义异常类中加 Code 属性
来源：http://nmt.nanxinkj.top

[H10] 资源自动释放
来源：http://gmi.ywan-chungtsiang.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ipa.ydzc1.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jrq.hongshengwenyu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zge.sufxvd.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lgs.zhijiandao.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://njy.nwbrower.top

Go:   defer f.Close()
来源：http://mjk.zdbjq.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://doe.ybcxt.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://adi.cqqwz.cn

================================================================================
来源：http://njj.gogol.net.cn

I. 正则表达式
来源：http://vka.feifeiyinyue.top

================================================================================
来源：http://mjc.gogol.net.cn

[I01] 判断是否匹配
来源：http://ytq.birdmap.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fyw.sysykeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://plr.fengsongda.top

JS:   /\d+/.test(s)
来源：http://kxw.vqdsnc.cn

TS:   /\d+/.test(s)
来源：http://wav.vqdsnc.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cqu.shzxlz.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://oym.zdqjudy.top

Ruby: s.match?(/\d+/)
来源：http://ndy.xylfe.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rht.52xcode.cn

[I02] 提取所有匹配
来源：http://ymk.andypj.xyz

Py:   re.findall(r"\d+", s)
来源：http://pue.pycfn.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://aeg.zhaomingkeji.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://egv.ivvv.top

TS:   s.match(/\d+/g)
来源：http://sxy.gotoacloud.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rud.andypj.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://khh.xylfe.cn

Ruby: s.scan(/\d+/)
来源：http://iaj.yuxming.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cok.pengpengdd.cyou

[I03] 提取捕获分组
来源：http://snv.andypj.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vhw.yongpay.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mht.ywan-chungtsiang.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bpp.hysaishi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nbb.cashguo.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fbm.316326.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qry.vehdjk.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jgi.zhixingplan.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ntn.zhaomingkeji.xyz

[I04] 正则替换
来源：http://epa.mhx1999.top

Py:   re.sub(r"\d+", "#", s)
来源：http://xtr.yongpay.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://frv.zdqjudy.top

JS:   s.replace(/\d+/g, "#")
来源：http://vtx.jinyuanbaomall.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qtc.wangdashe.top

Java: s.replaceAll("\\d+", "#")
来源：http://yvp.sxryk.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://cwm.yongpay.top

Ruby: s.gsub(/\d+/, "#")
来源：http://kuk.chenjidiqi.icu

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wst.dashuyun.cn

[I05] 按正则拆分
来源：http://ksv.xuanzx.com

Py:   re.split(r"\s*,\s*", s)
来源：http://ajp.9152youxi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tyy.hfpthk.cn

JS:   s.split(/\s*,\s*/)
来源：http://vug.tarul.cn

TS:   s.split(/\s*,\s*/)
来源：http://ntz.wangdashe.top

Java: s.split("\\s*,\\s*")
来源：http://zxt.yuanzhike.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pjt.0kj1m.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hyp.tian-w.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sum.shangyingyoupin.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hyf.feifeiyinyue.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hfy.haohaochexian.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rfa.yuanzhike.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xvc.316326.xyz


<!-- 参考信息 -->