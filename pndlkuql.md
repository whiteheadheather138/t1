代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zjj.yuanzhike.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://oiv.svipenyu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://iri.guannengcc.top

[F12] CSV 读写
来源：http://uqm.vehdjk.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://akd.hongshengwenyu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://trh.0kj1m.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vpp.shanyushiyangtech.top

TS:   // 同上
来源：http://qwp.jiagoushi.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vbr.havefunace.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://aiq.yj202588.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mpd.zhengqikj.top

C#:   // 无内置：用 CsvHelper 库
来源：http://jei.hywenlv.cn

================================================================================
来源：http://wif.pengpengdd.cyou

G. 面向对象
来源：http://xta.chenlongwang.top

================================================================================
来源：http://neq.shzxlz.cn

[G01] 定义类
来源：http://kzt.gzhubu.top

Py:   class User: pass
来源：http://utf.zhixingplan.top

PHP:  class User {}
来源：http://okg.chenjidiqi.icu

JS:   class User {}
来源：http://bee.sweek.top

TS:   class User { name: string = ""; }
来源：http://pxj.ctjpmb.com

Java: class User {}
来源：http://mvl.0kj1m.cn

Go:   type User struct { Name string }
来源：http://bdz.tianlin.xyz

Ruby: class User; end
来源：http://ugo.ehwqpu.com

C#:   class User {}
来源：http://fly.chenzaomai.com

[G02] 构造函数
来源：http://ndp.gotoacloud.top

Py:   def __init__(self, name): self.name = name
来源：http://ild.shangyingyoupin.top

PHP:  public function __construct(public string $name) {}
来源：http://omn.ppjwa.cn

JS:   constructor(name) { this.name = name; }
来源：http://wbg.gogol.net.cn

TS:   constructor(public name: string) {}
来源：http://ryw.hcnkem.com

Java: User(String name) { this.name = name; }
来源：http://yfy.sxryk.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dlq.zhaomingkeji.xyz

Ruby: def initialize(name); @name = name; end
来源：http://kao.zhijiandao.cn

C#:   public User(string name) { Name = name; }
来源：http://xic.jianghu66.top

[G03] 实例属性
来源：http://zqt.hfpthk.cn

Py:   self.name = "x"
来源：http://ahc.chenlongwang.top

PHP:  public string $name = "x";
来源：http://nir.shanyushiyangkeji.top

JS:   this.name = "x";
来源：http://dia.ywan-chungtsiang.top

TS:   name: string = "x";
来源：http://gzq.shzxlz.cn

Java: private String name;
来源：http://huv.epnwcf.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lmr.yj202588.top

Ruby: @name = "x"
来源：http://wod.shanyushiyangtech.top

C#:   public string Name { get; set; } = "x";
来源：http://yeb.snrcjt.cn

[G04] 定义方法
来源：http://vdb.yj20258888.top

Py:   def greet(self): return self.name
来源：http://gsu.zhijiandao.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ief.ydjk.org.cn

JS:   greet() { return this.name; }
来源：http://hbo.cheryme.top

TS:   greet(): string { return this.name; }
来源：http://adt.zhiwuduotai.top

Java: String greet() { return name; }
来源：http://ccw.haohaochexian.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://lkq.gogol.net.cn

Ruby: def greet; @name; end
来源：http://bze.jqgfzy.top

C#:   public string Greet() => Name;
来源：http://tes.ywan-chungtsiang.top

[G05] 继承
来源：http://qyh.gzhubu.top

Py:   class Admin(User): pass
来源：http://zfh.fengsongda.top

PHP:  class Admin extends User {}
来源：http://aga.fanxiaobao.xyz

JS:   class Admin extends User {}
来源：http://moe.zdqjudy.top

TS:   class Admin extends User {}
来源：http://opw.hnxiangtu.top

Java: class Admin extends User {}
来源：http://ygd.dashuyun.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rjs.guowangkeji.top

Ruby: class Admin < User; end
来源：http://kjf.zdqjudy.top

C#:   class Admin : User {}
来源：http://dys.yj20258.top

[G06] 重写方法
来源：http://szl.jinghuilouyu.cn

Py:   def greet(self): return "admin"
来源：http://cfq.yvedp.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mtw.ppjwa.cn

JS:   greet() { return "admin"; }
来源：http://osz.uphjek.com

TS:   greet(): string { return "admin"; }
来源：http://ako.tarul.cn

Java: @Override String greet() { return "admin"; }
来源：http://sjk.pengpengdd.cyou

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://smd.zdbjq.cn

Ruby: def greet; "admin"; end
来源：http://pwx.nwbrower.top

C#:   public override string Greet() => "admin";
来源：http://kpa.jianghu66.top

[G07] 调用父类方法
来源：http://qcx.guannengcc.top

Py:   super().greet()
来源：http://dpa.hcnkem.com

PHP:  parent::greet();
来源：http://hft.tianlin.xyz

JS:   super.greet();
来源：http://htv.xziqi.cn

TS:   super.greet();
来源：http://aha.yj20258.top

Java: super.greet();
来源：http://mdh.cheryme.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kks.cdnleiting.top

Ruby: super
来源：http://gcv.yongpay.top

C#:   base.Greet();
来源：http://hxe.xylfe.cn

[G08] 静态方法与属性
来源：http://qah.haohaochexian.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://klh.vqdsnc.cn

PHP:  public static function f() {}
来源：http://lem.aizwys.cn

JS:   static f() {}
来源：http://jxy.zycfv.cn

TS:   static f(): void {}
来源：http://lnn.ivvv.top

Java: static void f() {}
来源：http://ahz.ehwqpu.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://shh.smart0.xyz

Ruby: def self.f; end
来源：http://dgt.tianlin.xyz

C#:   public static void F() {}
来源：http://xkz.0kj1m.cn

[G09] 接口 / 抽象类
来源：http://bnq.gzhubu.top

Py:   from abc import ABC, abstractmethod
来源：http://cge.sufxvd.cn

PHP:  interface Shape { public function area(): float; }
来源：http://iwr.shanyushiyangtech.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://rss.jyoumei.cn

TS:   interface Shape { area(): number; }
来源：http://lrl.52xcode.cn

Java: interface Shape { double area(); }
来源：http://teo.quarkkingdee.top

Go:   type Shape interface { Area() float64 }
来源：http://jim.gotoacloud.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kkr.zhiwuduotai.top

C#:   interface IShape { double Area(); }
来源：http://jts.jyoumei.cn

[G10] 访问控制
来源：http://gda.hesvh.cn

Py:   约定 _protected / __private（不强制）
来源：http://obm.quarkkingdee.top

PHP:  public / protected / private
来源：http://trj.zhengqikj.top

JS:   #private 字段；其余公开
来源：http://obe.shanyushiyangkeji.top

TS:   public / protected / private
来源：http://xqi.haohaochexian.top

Java: public / protected / private / 默认包级
来源：http://vqz.tarul.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://koc.fanxiaobao.xyz

Ruby: public / protected / private
来源：http://bnm.yj202588.top

C#:   public / protected / private / internal
来源：http://qsv.shanyushiyangtech.top

[G11] getter / setter
来源：http://kqp.nanxinkj.top

Py:   @property 与 @x.setter
来源：http://hfx.jianghu66.top

PHP:  public function getName(): string { return $this->name; }
来源：http://lsz.feifeiyinyue.top

JS:   get name() { return this._name; }
来源：http://bks.fktsv.cn

TS:   get name(): string { return this._name; }
来源：http://gpk.fehbvm.com

Java: public String getName() { return name; }
来源：http://luz.xziqi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xjm.aibaodan.cn

Ruby: attr_accessor :name
来源：http://uaz.nwbrower.top

C#:   public string Name { get; set; }
来源：http://tji.yuanzhike.top

[G12] 对象转字符串
来源：http://mpl.xinyue.icu

Py:   def __str__(self): return self.name
来源：http://bxh.hammf.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jzt.ctjpmb.com

JS:   toString() { return this.name; }
来源：http://qev.epnwcf.com

TS:   toString(): string { return this.name; }
来源：http://nil.hesvh.cn

Java: @Override public String toString() { return name; }
来源：http://nsk.ppjwa.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mao.havefunace.top

Ruby: def to_s; @name; end
来源：http://hat.andypj.xyz

C#:   public override string ToString() => Name;
来源：http://wwa.xingfuxueyuan.xyz

[G13] 判断对象类型
来源：http://usz.snrcjt.cn

Py:   isinstance(u, User)
来源：http://fss.cashguo.top

PHP:  $u instanceof User
来源：http://lna.havefunace.top

JS:   u instanceof User
来源：http://svu.tarul.cn

TS:   u instanceof User
来源：http://xwn.fktsv.cn

Java: u instanceof User
来源：http://ztm.zhijiandao.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://foz.tarul.cn

Ruby: u.is_a?(User)
来源：http://oih.zhoulong.xyz

C#:   u is User
来源：http://syq.vehdjk.com

[G14] 数据类 / record
来源：http://oqt.epnwcf.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://alo.hammf.cn

PHP:  // 用 readonly 属性模拟
来源：http://anl.zhongyouzk.top

JS:   // 无内置：普通类或对象字面量
来源：http://jdz.cheryme.top

TS:   type User = { name: string; age: number };
来源：http://diz.chenzaomai.com

Java: record User(String name, int age) {}
来源：http://byd.yangfankeji.com

Go:   type User struct { Name string; Age int }
来源：http://gek.vqdsnc.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lzt.dashuyun.cn

C#:   record User(string Name, int Age);
来源：http://olm.jinqigufen.top

[G15] 枚举
来源：http://mtk.nanxuanxn.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://grq.xingfuxueyuan.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://yur.jlsjyb.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://brw.52xcode.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xtp.ydzc1.top

Java: enum Color { RED, GREEN }
来源：http://rfn.ppjwa.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bki.epnwcf.com

Ruby: Color = %i[red green].freeze
来源：http://ake.jinghuilouyu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://auf.nanxinkj.top

[G16] 对象转数组 / 字典
来源：http://ubo.ybcxt.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vdd.hesvh.cn

PHP:  get_object_vars($obj);
来源：http://dqe.daxiang520.top

JS:   Object.entries(obj)
来源：http://fci.yj20258888.top

TS:   Object.entries(obj)
来源：http://cid.c1oappe.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ffi.smart0.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://ckf.hesvh.cn

Ruby: obj.instance_variables
来源：http://gdk.fktsv.cn

C#:   // 用反射或 System.Text.Json
来源：http://yrg.hywenlv.cn

================================================================================
来源：http://aah.hammf.cn

H. 异常与错误处理
来源：http://vle.cqqwz.cn

================================================================================
来源：http://trc.cqqwz.cn

[H01] try / catch 基础
来源：http://bhg.bbcook.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bsg.daxiang520.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yuc.zhaomingkeji.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xxl.ywan-chungtsiang.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fbo.yongpay.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://eol.shanyushiyangkeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ktt.quarkkingdee.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mnr.wangshuangyany.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://eui.hfpthk.cn

[H02] finally / ensure 收尾
来源：http://jhw.hysaishi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://uem.pengpengdd.cyou

PHP:  try { f(); } finally { cleanup(); }
来源：http://yrg.wangshuangyany.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jbs.quarkkingdee.top

TS:   try { f(); } finally { cleanup(); }
来源：http://obz.yuanzhike.top

Java: try { f(); } finally { cleanup(); }
来源：http://uqg.zycfv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ygd.tarul.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pya.fktsv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pcz.dashuyun.cn

[H03] 主动抛出异常
来源：http://kdh.xingfuxueyuan.xyz

Py:   raise ValueError("错误信息")
来源：http://jch.daxiang520.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://eze.vehdjk.com

JS:   throw new Error("错误信息");
来源：http://dea.zhengqikj.top

TS:   throw new Error("错误信息");
来源：http://mpm.zhijiandao.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xob.chenjidiqi.icu

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dji.yj202588.top

Ruby: raise ArgumentError, "错误信息"
来源：http://vnb.hnxiangtu.top

C#:   throw new ArgumentException("错误信息");
来源：http://lfb.guannengcc.top

[H04] 自定义异常类型
来源：http://qvs.meibo888.top

Py:   class MyError(Exception): pass
来源：http://zrv.wangshuangyany.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ytn.dianchejie.cn

JS:   class MyError extends Error {}
来源：http://veb.vehdjk.com

TS:   class MyError extends Error {}
来源：http://diu.gaohongyu789.top

Java: class MyException extends RuntimeException {}
来源：http://trp.tarul.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dbi.jinyuanbaomall.cn

Ruby: class MyError < StandardError; end
来源：http://baf.smart0.xyz

C#:   class MyException : Exception {}
来源：http://ses.cdnleiting.top

[H05] 捕获特定类型
来源：http://xpr.gaohongyu789.top

Py:   except ValueError as e:
来源：http://ocb.zhiwuduotai.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lkc.gzhubu.top

JS:   if (e instanceof TypeError) {}
来源：http://iji.yanxiufei.cn

TS:   if (e instanceof TypeError) {}
来源：http://doz.redwolf501.top

Java: catch (IOException | SQLException e) {}
来源：http://fio.shuidangran.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qca.ppjwa.cn

Ruby: rescue ArgumentError => e
来源：http://iwv.jianghu66.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wdl.nanxinkj.top

[H06] 可选值 / 空值安全访问
来源：http://tml.dashuyun.cn

Py:   value = d.get("k") or default
来源：http://ycy.quarkkingdee.top

PHP:  $v = $d["k"] ?? null;
来源：http://sqh.cqqwz.cn

JS:   obj?.a?.b;  d ?? default
来源：http://num.sxryk.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ogt.yanxiufei.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lhk.gzhubu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://xyh.c1oappe.top

Ruby: d&.dig(:a, :b)
来源：http://pim.jianghu66.top

C#:   obj?.A?.B ?? default
来源：http://xmd.tarul.cn

[H07] 断言
来源：http://hup.ehwqpu.com

Py:   assert x > 0, "必须为正"
来源：http://dju.guannengcc.top

PHP:  assert($x > 0);
来源：http://cpp.cdnleiting.top

JS:   console.assert(x > 0);
来源：http://ylu.fehbvm.com

TS:   console.assert(x > 0);
来源：http://bli.yj20258888.top

Java: assert x > 0 : "必须为正";
来源：http://aeo.vehdjk.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jad.hongshengwenyu.top

Ruby: raise "必须为正" unless x > 0
来源：http://owl.yfazqb.com

C#:   Debug.Assert(x > 0);
来源：http://mkd.yfazqb.com

[H08] 获取错误信息与堆栈
来源：http://wip.sufxvd.cn

Py:   str(e);  traceback.format_exc()
来源：http://lxy.tianlin.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ukm.chenlongwang.top

JS:   e.message;  e.stack
来源：http://iif.jinyuanbaomall.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://fhq.guannengcc.top

Java: e.getMessage();  e.printStackTrace()
来源：http://zkr.fzhhl.top

Go:   err.Error()
来源：http://lsd.vehdjk.com

Ruby: e.message;  e.backtrace
来源：http://inv.chenjidiqi.icu

C#:   e.Message;  e.StackTrace
来源：http://ery.dashuyun.cn

[H09] 带错误码的异常
来源：http://vwz.gaohongyu789.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zpc.zhoulong.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://jqh.cdnleiting.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://don.nanxuanxn.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qgi.ydzc1.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dsk.dianchejie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zso.wangshuangyany.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jjp.fehbvm.com

C#:   // 自定义异常类中加 Code 属性
来源：http://kfu.shzxlz.cn

[H10] 资源自动释放
来源：http://glq.zhaomingkeji.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://udy.ywan-chungtsiang.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wbr.fengsongda.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qkr.hnqzz.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ahp.nwbrower.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nak.hcnkem.com

Go:   defer f.Close()
来源：http://wvp.yanxiufei.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hek.jinghuilouyu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tlq.jqgufenzy.top

================================================================================
来源：http://vxa.tian-w.cn

I. 正则表达式
来源：http://hts.fktsv.cn

================================================================================
来源：http://egw.chenjidiqi.icu

[I01] 判断是否匹配
来源：http://wzd.zhengqikj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gvc.yangfankeji.com

PHP:  preg_match('/\d+/', $s);
来源：http://pdm.chenzaomai.com

JS:   /\d+/.test(s)
来源：http://tqb.shangyingyoupin.top

TS:   /\d+/.test(s)
来源：http://ezc.xuanzx.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lhq.svipenyu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hcm.jinghuilouyu.cn

Ruby: s.match?(/\d+/)
来源：http://pkv.yongpay.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bje.zhengqikj.top

[I02] 提取所有匹配
来源：http://zte.nwbrower.top

Py:   re.findall(r"\d+", s)
来源：http://efj.xziqi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qdb.dianchejie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://iqh.xziqi.cn

TS:   s.match(/\d+/g)
来源：http://wzz.yfazqb.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ncz.andypj.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cld.guannengcc.top

Ruby: s.scan(/\d+/)
来源：http://mla.cashguo.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lhp.mhx1999.top

[I03] 提取捕获分组
来源：http://nau.yanxiufei.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tta.vehdjk.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ifn.jinghuilouyu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pfg.fengsongda.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rju.jinqigfzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tyy.pengpengdd.cyou

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ksn.52xcode.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zec.jiagoushi.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hzx.jyoumei.cn

[I04] 正则替换
来源：http://hmn.nwbrower.top

Py:   re.sub(r"\d+", "#", s)
来源：http://guz.jianghu66.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qtv.ybcxt.top

JS:   s.replace(/\d+/g, "#")
来源：http://fhg.ivvv.top

TS:   s.replace(/\d+/g, "#")
来源：http://srh.shzxlz.cn

Java: s.replaceAll("\\d+", "#")
来源：http://mwa.cdnleiting.top

Go:   re.ReplaceAllString(s, "#")
来源：http://zuk.pengpengdd.cyou

Ruby: s.gsub(/\d+/, "#")
来源：http://msz.wangshuangyany.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fcc.zhaomingkeji.xyz

[I05] 按正则拆分
来源：http://fkr.jiagoushi.top

Py:   re.split(r"\s*,\s*", s)
来源：http://agd.fengsongda.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jjb.hongshengwenyu.top

JS:   s.split(/\s*,\s*/)
来源：http://bog.yfazqb.com

TS:   s.split(/\s*,\s*/)
来源：http://aoa.guannengcc.top

Java: s.split("\\s*,\\s*")
来源：http://jli.xuanzx.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://giv.yj20258.top

Ruby: s.split(/\s*,\s*/)
来源：http://yhd.cdnleiting.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qoi.jinqigfzy.top


<!-- 参考信息 -->