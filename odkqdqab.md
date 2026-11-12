代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://clp.svipenyu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uks.shanyushiyangkeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yhw.zhaomingkeji.xyz

[F12] CSV 读写
来源：http://onu.kuanghao11.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hpg.yanxiufei.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tlf.hysaishi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pju.yj20258888.top

TS:   // 同上
来源：http://rrr.gaohongyu789.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zeg.quarkkingdee.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://uqi.zdqjudy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qbn.jyoumei.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qkn.shanyushiyangkeji.top

================================================================================
来源：http://oji.ctjpmb.com

G. 面向对象
来源：http://ins.wangdashe.top

================================================================================
来源：http://tfx.chenzaomai.com

[G01] 定义类
来源：http://mjx.guowangkeji.top

Py:   class User: pass
来源：http://ema.yvedp.cn

PHP:  class User {}
来源：http://xoq.yfazqb.com

JS:   class User {}
来源：http://xsf.jiagoushi.top

TS:   class User { name: string = ""; }
来源：http://jkn.gogol.net.cn

Java: class User {}
来源：http://gjn.chenzaomai.com

Go:   type User struct { Name string }
来源：http://dhi.xinyue.icu

Ruby: class User; end
来源：http://grg.xuanzx.com

C#:   class User {}
来源：http://vcs.zhiwuduotai.top

[G02] 构造函数
来源：http://qkx.jiagoushi.top

Py:   def __init__(self, name): self.name = name
来源：http://avd.vqdsnc.cn

PHP:  public function __construct(public string $name) {}
来源：http://wjv.guannengcc.top

JS:   constructor(name) { this.name = name; }
来源：http://kts.nanxinkj.top

TS:   constructor(public name: string) {}
来源：http://flc.sysykeji.top

Java: User(String name) { this.name = name; }
来源：http://for.cashguo.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hoz.pengpengdd.cyou

Ruby: def initialize(name); @name = name; end
来源：http://drx.yvedp.cn

C#:   public User(string name) { Name = name; }
来源：http://igd.hywenlv.cn

[G03] 实例属性
来源：http://tcj.guannengcc.top

Py:   self.name = "x"
来源：http://uyt.hfpthk.cn

PHP:  public string $name = "x";
来源：http://ngl.yonumen.top

JS:   this.name = "x";
来源：http://bog.epnwcf.com

TS:   name: string = "x";
来源：http://rhx.guannengcc.top

Java: private String name;
来源：http://vik.yfazqb.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://unv.hesvh.cn

Ruby: @name = "x"
来源：http://zme.yuanzhike.top

C#:   public string Name { get; set; } = "x";
来源：http://rsr.xuanzx.com

[G04] 定义方法
来源：http://szp.c1oappe.top

Py:   def greet(self): return self.name
来源：http://yav.yanxiufei.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nsv.yj20258.top

JS:   greet() { return this.name; }
来源：http://bga.chenzaomai.com

TS:   greet(): string { return this.name; }
来源：http://emm.zhengqikj.top

Java: String greet() { return name; }
来源：http://xeb.havefunace.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://sok.svipenyu.cn

Ruby: def greet; @name; end
来源：http://tcn.sxryk.cn

C#:   public string Greet() => Name;
来源：http://afw.yonumen.top

[G05] 继承
来源：http://pzk.jlsjyb.cn

Py:   class Admin(User): pass
来源：http://cbe.zhoulong.xyz

PHP:  class Admin extends User {}
来源：http://mvy.vehdjk.com

JS:   class Admin extends User {}
来源：http://dht.cashguo.top

TS:   class Admin extends User {}
来源：http://gkp.birdmap.top

Java: class Admin extends User {}
来源：http://frb.tianlin.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jwu.zdbjq.cn

Ruby: class Admin < User; end
来源：http://fdj.hywenlv.cn

C#:   class Admin : User {}
来源：http://kps.zhengqikj.top

[G06] 重写方法
来源：http://ypm.pengpengdd.cyou

Py:   def greet(self): return "admin"
来源：http://agi.xziqi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://lzd.sweek.top

JS:   greet() { return "admin"; }
来源：http://eaz.jinqigfzy.top

TS:   greet(): string { return "admin"; }
来源：http://ykz.fehbvm.com

Java: @Override String greet() { return "admin"; }
来源：http://xhk.zhongyouzk.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://las.52xcode.cn

Ruby: def greet; "admin"; end
来源：http://qfw.uphjek.com

C#:   public override string Greet() => "admin";
来源：http://wkl.guannengcc.top

[G07] 调用父类方法
来源：http://dyq.fzhhl.top

Py:   super().greet()
来源：http://eyb.pengpengdd.cyou

PHP:  parent::greet();
来源：http://ppi.hnxiangtu.top

JS:   super.greet();
来源：http://zyu.jianghu66.top

TS:   super.greet();
来源：http://klg.shanyushiyangtech.top

Java: super.greet();
来源：http://pzm.hongshengwenyu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lth.gaohongyu789.top

Ruby: super
来源：http://zzx.chenlongwang.top

C#:   base.Greet();
来源：http://ojk.kuanghao11.cn

[G08] 静态方法与属性
来源：http://mbs.nanxuanxn.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rgg.mhx1999.top

PHP:  public static function f() {}
来源：http://zmr.snrcjt.cn

JS:   static f() {}
来源：http://ynb.dianchejie.cn

TS:   static f(): void {}
来源：http://qld.guowangkeji.top

Java: static void f() {}
来源：http://ius.jinqigufen.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://tty.jinghuilouyu.cn

Ruby: def self.f; end
来源：http://yqh.birdmap.top

C#:   public static void F() {}
来源：http://nhe.aizwys.cn

[G09] 接口 / 抽象类
来源：http://euc.gotoacloud.top

Py:   from abc import ABC, abstractmethod
来源：http://nfb.jinqigufen.top

PHP:  interface Shape { public function area(): float; }
来源：http://npn.birdmap.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ept.gogol.net.cn

TS:   interface Shape { area(): number; }
来源：http://jcc.chenzaomai.com

Java: interface Shape { double area(); }
来源：http://nme.xylfe.cn

Go:   type Shape interface { Area() float64 }
来源：http://njx.aibaodan.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mwt.jianghu66.top

C#:   interface IShape { double Area(); }
来源：http://ugd.hnqzz.top

[G10] 访问控制
来源：http://jci.cucudq.cn

Py:   约定 _protected / __private（不强制）
来源：http://wde.xuetiantiany.cn

PHP:  public / protected / private
来源：http://uhx.fehbvm.com

JS:   #private 字段；其余公开
来源：http://hzh.9152youxi.cn

TS:   public / protected / private
来源：http://iyz.hongshengwenyu.top

Java: public / protected / private / 默认包级
来源：http://zoo.ehwqpu.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://kbt.hnqzz.top

Ruby: public / protected / private
来源：http://qoe.fzhhl.top

C#:   public / protected / private / internal
来源：http://wua.chenjidiqi.icu

[G11] getter / setter
来源：http://isr.pengpengdd.cyou

Py:   @property 与 @x.setter
来源：http://cgt.zhaomingkeji.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://utz.hnxiangtu.top

JS:   get name() { return this._name; }
来源：http://efl.ivvv.top

TS:   get name(): string { return this._name; }
来源：http://nwc.cheryme.top

Java: public String getName() { return name; }
来源：http://teu.jiagoushi.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://rvg.chenlongwang.top

Ruby: attr_accessor :name
来源：http://mwy.hywenlv.cn

C#:   public string Name { get; set; }
来源：http://qal.zycfv.cn

[G12] 对象转字符串
来源：http://zix.quarkkingdee.top

Py:   def __str__(self): return self.name
来源：http://niy.daxiang520.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://itv.fzhhl.top

JS:   toString() { return this.name; }
来源：http://kcr.wangshuangyany.cn

TS:   toString(): string { return this.name; }
来源：http://wmq.snrcjt.cn

Java: @Override public String toString() { return name; }
来源：http://xka.shuidangran.top

Go:   func (u User) String() string { return u.Name }
来源：http://ugi.quarkkingdee.top

Ruby: def to_s; @name; end
来源：http://ghm.shanyushiyangkeji.top

C#:   public override string ToString() => Name;
来源：http://ghx.pengpengdd.cyou

[G13] 判断对象类型
来源：http://gch.vehdjk.com

Py:   isinstance(u, User)
来源：http://pem.iojbl.cn

PHP:  $u instanceof User
来源：http://jjg.svipenyu.cn

JS:   u instanceof User
来源：http://dfz.sweek.top

TS:   u instanceof User
来源：http://hjc.havefunace.top

Java: u instanceof User
来源：http://dpx.ydzc1.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://kbv.xuetiantiany.cn

Ruby: u.is_a?(User)
来源：http://cvs.jyoumei.cn

C#:   u is User
来源：http://swq.wangshuangyany.cn

[G14] 数据类 / record
来源：http://pcc.gogol.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zvu.haohaochexian.top

PHP:  // 用 readonly 属性模拟
来源：http://rld.meibo888.top

JS:   // 无内置：普通类或对象字面量
来源：http://omv.316326.xyz

TS:   type User = { name: string; age: number };
来源：http://lnq.yuanzhike.top

Java: record User(String name, int age) {}
来源：http://akp.yfazqb.com

Go:   type User struct { Name string; Age int }
来源：http://nxk.kuanghao11.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jnp.bjfxy.top

C#:   record User(string Name, int Age);
来源：http://veb.jinyuanbaomall.cn

[G15] 枚举
来源：http://nbw.cucudq.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tgv.sxryk.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://eaw.xziqi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kea.cdnleiting.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wpa.andypj.xyz

Java: enum Color { RED, GREEN }
来源：http://mys.yueranfly.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qze.cdnleiting.top

Ruby: Color = %i[red green].freeze
来源：http://umb.jqgfzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hqb.ydzc1.top

[G16] 对象转数组 / 字典
来源：http://bkj.yueranfly.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lst.jlsjyb.cn

PHP:  get_object_vars($obj);
来源：http://gtw.fanxiaobao.xyz

JS:   Object.entries(obj)
来源：http://sjq.zhiwuduotai.top

TS:   Object.entries(obj)
来源：http://pzb.sxryk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vlf.guannengcc.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://hxy.hfpthk.cn

Ruby: obj.instance_variables
来源：http://ena.hesvh.cn

C#:   // 用反射或 System.Text.Json
来源：http://rtv.snrcjt.cn

================================================================================
来源：http://fou.cucudq.cn

H. 异常与错误处理
来源：http://mld.yangfankeji.com

================================================================================
来源：http://loy.birdmap.top

[H01] try / catch 基础
来源：http://ypb.zhiwuduotai.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wbc.yfazqb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kzi.chenzaomai.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vfz.0kj1m.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rov.jqgufenzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kxt.quarkkingdee.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://aar.dianchejie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://psy.shzxlz.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lgv.zhengqikj.top

[H02] finally / ensure 收尾
来源：http://que.yongpay.top

Py:   try: f()⏎finally: cleanup()
来源：http://itr.0kj1m.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://auf.cucudq.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gni.cqqwz.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xun.tanke756.top

Java: try { f(); } finally { cleanup(); }
来源：http://wiz.sufxvd.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://onb.xinyue.icu

Ruby: begin; f; ensure; cleanup; end
来源：http://xsk.dashuyun.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qiw.snrcjt.cn

[H03] 主动抛出异常
来源：http://hpv.yuxming.cn

Py:   raise ValueError("错误信息")
来源：http://fsx.hysaishi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jyj.hongshengwenyu.top

JS:   throw new Error("错误信息");
来源：http://yvn.ywan-chungtsiang.top

TS:   throw new Error("错误信息");
来源：http://sdw.zdqjudy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://rkf.ydzc1.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cic.cdnleiting.top

Ruby: raise ArgumentError, "错误信息"
来源：http://hyj.hesvh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rdm.uphjek.com

[H04] 自定义异常类型
来源：http://qij.aibaodan.cn

Py:   class MyError(Exception): pass
来源：http://mcp.xuanzx.com

PHP:  class MyError extends RuntimeException {}
来源：http://ayr.yj20258.top

JS:   class MyError extends Error {}
来源：http://qxk.cdnleiting.top

TS:   class MyError extends Error {}
来源：http://wpg.zhixingplan.top

Java: class MyException extends RuntimeException {}
来源：http://fyv.dianchejie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wio.316326.xyz

Ruby: class MyError < StandardError; end
来源：http://sby.epnwcf.com

C#:   class MyException : Exception {}
来源：http://rmr.fengsongda.top

[H05] 捕获特定类型
来源：http://aus.yonumen.top

Py:   except ValueError as e:
来源：http://lwq.hesvh.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dhd.jinghuilouyu.cn

JS:   if (e instanceof TypeError) {}
来源：http://ciw.quarkkingdee.top

TS:   if (e instanceof TypeError) {}
来源：http://bot.shanyushiyangkeji.top

Java: catch (IOException | SQLException e) {}
来源：http://afw.ydzc1.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qkj.sweek.top

Ruby: rescue ArgumentError => e
来源：http://yqe.jyoumei.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ytm.haohaochexian.top

[H06] 可选值 / 空值安全访问
来源：http://bgk.jinqigfzy.top

Py:   value = d.get("k") or default
来源：http://mep.nanxinkj.top

PHP:  $v = $d["k"] ?? null;
来源：http://axz.zycfv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gdc.ywan-chungtsiang.top

TS:   obj?.a?.b;  d ?? default
来源：http://vqi.jinghuilouyu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xpw.aibaodan.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://flg.zhijiandao.cn

Ruby: d&.dig(:a, :b)
来源：http://oqp.tian-w.cn

C#:   obj?.A?.B ?? default
来源：http://tmj.sxryk.cn

[H07] 断言
来源：http://pfb.tianlin.xyz

Py:   assert x > 0, "必须为正"
来源：http://ela.yj202588.top

PHP:  assert($x > 0);
来源：http://amv.tanke756.top

JS:   console.assert(x > 0);
来源：http://kmb.jlsjyb.cn

TS:   console.assert(x > 0);
来源：http://eza.jqgfzy.top

Java: assert x > 0 : "必须为正";
来源：http://moj.mhx1999.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hpo.hnxiangtu.top

Ruby: raise "必须为正" unless x > 0
来源：http://sxa.zhijiandao.cn

C#:   Debug.Assert(x > 0);
来源：http://guw.pengpengdd.cyou

[H08] 获取错误信息与堆栈
来源：http://hhk.yfazqb.com

Py:   str(e);  traceback.format_exc()
来源：http://prp.hammf.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ydc.jqgufenzy.top

JS:   e.message;  e.stack
来源：http://lhc.pycfn.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://pub.zhijiandao.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wax.yongpay.top

Go:   err.Error()
来源：http://tmb.uphjek.com

Ruby: e.message;  e.backtrace
来源：http://rjo.jinghuilouyu.cn

C#:   e.Message;  e.StackTrace
来源：http://ibo.shangyingyoupin.top

[H09] 带错误码的异常
来源：http://npt.xuetiantiany.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yht.ydjk.org.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ggt.316326.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wwj.zhoulong.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kpl.uphjek.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mvo.quarkkingdee.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pwj.gotoacloud.top

Ruby: raise MyError.new("fail", 500)
来源：http://jfb.ybcxt.top

C#:   // 自定义异常类中加 Code 属性
来源：http://kyx.xziqi.cn

[H10] 资源自动释放
来源：http://kzf.chenjidiqi.icu

Py:   with open("a.txt") as f: data = f.read()
来源：http://xsr.chenlongwang.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://edc.xinyue.icu

JS:   // 无 with：在 finally 里关闭句柄
来源：http://opp.zhixingplan.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bxz.zdqjudy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kbj.hesvh.cn

Go:   defer f.Close()
来源：http://tcg.jyoumei.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://djx.yj20258888.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lqc.tian-w.cn

================================================================================
来源：http://iwm.xziqi.cn

I. 正则表达式
来源：http://zoq.fehbvm.com

================================================================================
来源：http://acc.zhixingplan.top

[I01] 判断是否匹配
来源：http://mbq.jinghuilouyu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qrd.xylfe.cn

PHP:  preg_match('/\d+/', $s);
来源：http://eox.uphjek.com

JS:   /\d+/.test(s)
来源：http://szc.gaohongyu789.top

TS:   /\d+/.test(s)
来源：http://pfq.wangdashe.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ksy.chenjidiqi.icu

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kdo.cashguo.top

Ruby: s.match?(/\d+/)
来源：http://tkq.quarkkingdee.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tyu.tarul.cn

[I02] 提取所有匹配
来源：http://ovw.kuanghao11.cn

Py:   re.findall(r"\d+", s)
来源：http://esb.cucudq.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bby.sufxvd.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://scg.fengsongda.top

TS:   s.match(/\d+/g)
来源：http://ogx.zhixingplan.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://goq.jinqigufen.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gvg.zhoulong.xyz

Ruby: s.scan(/\d+/)
来源：http://krb.chenjidiqi.icu

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dwi.cashguo.top

[I03] 提取捕获分组
来源：http://gmt.bjfxy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://grs.pengpengdd.cyou

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wof.yanxiufei.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ynv.yuxming.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ruc.cheryme.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://aho.mhx1999.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bwt.yvedp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ppe.andypj.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://csi.fktsv.cn

[I04] 正则替换
来源：http://qtd.sjlbkw.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://fxr.uphjek.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xad.316326.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://fpx.iojbl.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ukf.epnwcf.com

Java: s.replaceAll("\\d+", "#")
来源：http://xol.sufxvd.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://glz.hfpthk.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fdr.vehdjk.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://upx.ppjwa.cn

[I05] 按正则拆分
来源：http://oys.zhiwuduotai.top

Py:   re.split(r"\s*,\s*", s)
来源：http://qkk.quarkkingdee.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://str.cheryme.top

JS:   s.split(/\s*,\s*/)
来源：http://roh.shzxlz.cn

TS:   s.split(/\s*,\s*/)
来源：http://aau.quarkkingdee.top

Java: s.split("\\s*,\\s*")
来源：http://svs.jlsjyb.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rnz.chenzaomai.com

Ruby: s.split(/\s*,\s*/)
来源：http://yiu.tianlin.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nob.yueranfly.top


<!-- 参考信息 -->