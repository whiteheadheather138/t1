代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qow.uphjek.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bba.zhiwuduotai.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://awr.sufxvd.cn

TS:   // 同上
来源：http://pno.yj20258888.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pvi.tianlin.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://uir.tanke756.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dba.shuidangran.top

C#:   // 无内置：用 CsvHelper 库
来源：http://jto.0kj1m.cn

================================================================================
来源：http://rzb.jinqigfzy.top

G. 面向对象
来源：http://dls.daxiang520.top

================================================================================
来源：http://bes.vehdjk.com

[G01] 定义类
来源：http://sjy.zdqjudy.top

Py:   class User: pass
来源：http://eek.cashguo.top

PHP:  class User {}
来源：http://toz.hnqzz.top

JS:   class User {}
来源：http://lzk.svipenyu.cn

TS:   class User { name: string = ""; }
来源：http://cis.guowangkeji.top

Java: class User {}
来源：http://iug.sufxvd.cn

Go:   type User struct { Name string }
来源：http://xzy.hfpthk.cn

Ruby: class User; end
来源：http://opl.daxiang520.top

C#:   class User {}
来源：http://qbw.yueranfly.top

[G02] 构造函数
来源：http://vha.uphjek.com

Py:   def __init__(self, name): self.name = name
来源：http://tky.yj20258888.top

PHP:  public function __construct(public string $name) {}
来源：http://vte.bjfxy.top

JS:   constructor(name) { this.name = name; }
来源：http://wpi.yangfankeji.com

TS:   constructor(public name: string) {}
来源：http://dta.dashuyun.cn

Java: User(String name) { this.name = name; }
来源：http://ptx.chenjidiqi.icu

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kvv.zhongyouzk.top

Ruby: def initialize(name); @name = name; end
来源：http://zqy.316326.xyz

C#:   public User(string name) { Name = name; }
来源：http://vwl.birdmap.top

[G03] 实例属性
来源：http://slt.tanke756.top

Py:   self.name = "x"
来源：http://yin.c1oappe.top

PHP:  public string $name = "x";
来源：http://lgy.zdqjudy.top

JS:   this.name = "x";
来源：http://jgh.yj20258888.top

TS:   name: string = "x";
来源：http://emh.bbcook.cn

Java: private String name;
来源：http://fka.ehwqpu.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yvt.hcnkem.com

Ruby: @name = "x"
来源：http://gjg.fehbvm.com

C#:   public string Name { get; set; } = "x";
来源：http://ddx.hnxiangtu.top

[G04] 定义方法
来源：http://exf.ydzc1.top

Py:   def greet(self): return self.name
来源：http://wzx.wangdashe.top

PHP:  public function greet(): string { return $this->name; }
来源：http://omn.fktsv.cn

JS:   greet() { return this.name; }
来源：http://dmc.quarkkingdee.top

TS:   greet(): string { return this.name; }
来源：http://nwx.ehwqpu.com

Java: String greet() { return name; }
来源：http://uyx.bbcook.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hdm.zycfv.cn

Ruby: def greet; @name; end
来源：http://gxs.shanyushiyangtech.top

C#:   public string Greet() => Name;
来源：http://hjd.hongshengwenyu.top

[G05] 继承
来源：http://nfd.jiagoushi.top

Py:   class Admin(User): pass
来源：http://epq.gzhubu.top

PHP:  class Admin extends User {}
来源：http://lhk.cqqwz.cn

JS:   class Admin extends User {}
来源：http://blt.shuidangran.top

TS:   class Admin extends User {}
来源：http://qnj.dianchejie.cn

Java: class Admin extends User {}
来源：http://guw.shangyingyoupin.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ggw.cdnleiting.top

Ruby: class Admin < User; end
来源：http://btk.sweek.top

C#:   class Admin : User {}
来源：http://xtg.feifeiyinyue.top

[G06] 重写方法
来源：http://jst.cucudq.cn

Py:   def greet(self): return "admin"
来源：http://bie.yanxiufei.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wli.nwbrower.top

JS:   greet() { return "admin"; }
来源：http://naz.gotoacloud.top

TS:   greet(): string { return "admin"; }
来源：http://qqy.hesvh.cn

Java: @Override String greet() { return "admin"; }
来源：http://mdi.nanxinkj.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oif.yongpay.top

Ruby: def greet; "admin"; end
来源：http://zuf.guowangkeji.top

C#:   public override string Greet() => "admin";
来源：http://woi.jianghu66.top

[G07] 调用父类方法
来源：http://pwz.dashuyun.cn

Py:   super().greet()
来源：http://sam.zhengqikj.top

PHP:  parent::greet();
来源：http://bwf.jiagoushi.top

JS:   super.greet();
来源：http://vpc.nanxinkj.top

TS:   super.greet();
来源：http://iym.shanyushiyangkeji.top

Java: super.greet();
来源：http://cjq.hysaishi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sqp.snrcjt.cn

Ruby: super
来源：http://jlt.tarul.cn

C#:   base.Greet();
来源：http://bgg.cdnleiting.top

[G08] 静态方法与属性
来源：http://orc.yvedp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wok.jlsjyb.cn

PHP:  public static function f() {}
来源：http://ijy.zhengqikj.top

JS:   static f() {}
来源：http://yrg.tanke756.top

TS:   static f(): void {}
来源：http://mux.epnwcf.com

Java: static void f() {}
来源：http://gdf.xziqi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nlz.chenjidiqi.icu

Ruby: def self.f; end
来源：http://bgi.wangshuangyany.cn

C#:   public static void F() {}
来源：http://pcv.andypj.xyz

[G09] 接口 / 抽象类
来源：http://ipb.mhx1999.top

Py:   from abc import ABC, abstractmethod
来源：http://qpx.ehwqpu.com

PHP:  interface Shape { public function area(): float; }
来源：http://bjx.52xcode.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rit.sufxvd.cn

TS:   interface Shape { area(): number; }
来源：http://uhg.pycfn.com

Java: interface Shape { double area(); }
来源：http://dip.gzhubu.top

Go:   type Shape interface { Area() float64 }
来源：http://mmu.ctjpmb.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://axj.uphjek.com

C#:   interface IShape { double Area(); }
来源：http://ide.nanxuanxn.top

[G10] 访问控制
来源：http://bsp.smart0.xyz

Py:   约定 _protected / __private（不强制）
来源：http://hbm.yueranfly.top

PHP:  public / protected / private
来源：http://iqw.cdnleiting.top

JS:   #private 字段；其余公开
来源：http://ity.guowangkeji.top

TS:   public / protected / private
来源：http://gno.tian-w.cn

Java: public / protected / private / 默认包级
来源：http://vax.ctjpmb.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://hbz.xuanzx.com

Ruby: public / protected / private
来源：http://bkr.yonumen.top

C#:   public / protected / private / internal
来源：http://slm.havefunace.top

[G11] getter / setter
来源：http://rwa.cqqwz.cn

Py:   @property 与 @x.setter
来源：http://pss.tanke756.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ews.andypj.xyz

JS:   get name() { return this._name; }
来源：http://jkh.316326.xyz

TS:   get name(): string { return this._name; }
来源：http://xmc.cucudq.cn

Java: public String getName() { return name; }
来源：http://xtm.dashuyun.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ycj.aizwys.cn

Ruby: attr_accessor :name
来源：http://izs.gaohongyu789.top

C#:   public string Name { get; set; }
来源：http://cof.ehwqpu.com

[G12] 对象转字符串
来源：http://oea.mhx1999.top

Py:   def __str__(self): return self.name
来源：http://raw.yangfankeji.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://yyf.aibaodan.cn

JS:   toString() { return this.name; }
来源：http://ewp.jinghuilouyu.cn

TS:   toString(): string { return this.name; }
来源：http://dhg.hysaishi.cn

Java: @Override public String toString() { return name; }
来源：http://wlj.xingfuxueyuan.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://toz.smart0.xyz

Ruby: def to_s; @name; end
来源：http://qkt.vehdjk.com

C#:   public override string ToString() => Name;
来源：http://kxk.andypj.xyz

[G13] 判断对象类型
来源：http://toi.xziqi.cn

Py:   isinstance(u, User)
来源：http://wdn.svipenyu.cn

PHP:  $u instanceof User
来源：http://mtu.jiagoushi.top

JS:   u instanceof User
来源：http://uqw.jinqigfzy.top

TS:   u instanceof User
来源：http://aqy.yangfankeji.com

Java: u instanceof User
来源：http://dnw.jinqigufen.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://qza.yongpay.top

Ruby: u.is_a?(User)
来源：http://wgx.sxryk.cn

C#:   u is User
来源：http://qsf.316326.xyz

[G14] 数据类 / record
来源：http://qvq.gzhubu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xzs.chenzaomai.com

PHP:  // 用 readonly 属性模拟
来源：http://kfh.9152youxi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jgf.dashuyun.cn

TS:   type User = { name: string; age: number };
来源：http://lqv.hesvh.cn

Java: record User(String name, int age) {}
来源：http://xov.nanxinkj.top

Go:   type User struct { Name string; Age int }
来源：http://gdc.meibo888.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://oft.wangdashe.top

C#:   record User(string Name, int Age);
来源：http://qsn.yueranfly.top

[G15] 枚举
来源：http://sne.hammf.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://igc.c1oappe.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://yxm.yvedp.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fwy.shzxlz.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gsm.tian-w.cn

Java: enum Color { RED, GREEN }
来源：http://xre.zhixingplan.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xnq.mhx1999.top

Ruby: Color = %i[red green].freeze
来源：http://yaj.hammf.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kyz.havefunace.top

[G16] 对象转数组 / 字典
来源：http://vlv.mhx1999.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xoh.bbcook.cn

PHP:  get_object_vars($obj);
来源：http://ljp.cdnleiting.top

JS:   Object.entries(obj)
来源：http://gno.ydjk.org.cn

TS:   Object.entries(obj)
来源：http://eyt.yueranfly.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fjo.jyoumei.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bfj.cashguo.top

Ruby: obj.instance_variables
来源：http://gkx.zhongyouzk.top

C#:   // 用反射或 System.Text.Json
来源：http://smx.zhixingplan.top

================================================================================
来源：http://zfh.zhixingplan.top

H. 异常与错误处理
来源：http://rkw.fktsv.cn

================================================================================
来源：http://aqn.birdmap.top

[H01] try / catch 基础
来源：http://uzy.0kj1m.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nog.chenlongwang.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mxb.sjlbkw.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vby.hysaishi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gbe.c1oappe.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zwr.ydzc1.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jul.snrcjt.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kqr.guannengcc.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ugi.fanxiaobao.xyz

[H02] finally / ensure 收尾
来源：http://yav.yuxming.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dkt.dianchejie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://dsz.guowangkeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://sue.nanxinkj.top

TS:   try { f(); } finally { cleanup(); }
来源：http://eqv.hnxiangtu.top

Java: try { f(); } finally { cleanup(); }
来源：http://luv.meibo888.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://djz.fehbvm.com

Ruby: begin; f; ensure; cleanup; end
来源：http://dgp.zdbjq.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xuy.wangdashe.top

[H03] 主动抛出异常
来源：http://llv.zhixingplan.top

Py:   raise ValueError("错误信息")
来源：http://mcl.vehdjk.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mgk.feifeiyinyue.top

JS:   throw new Error("错误信息");
来源：http://tmq.bbcook.cn

TS:   throw new Error("错误信息");
来源：http://bpo.ivvv.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://csl.chenjidiqi.icu

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qkp.uphjek.com

Ruby: raise ArgumentError, "错误信息"
来源：http://snw.jqgfzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://ury.sxryk.cn

[H04] 自定义异常类型
来源：http://gsf.zdqjudy.top

Py:   class MyError(Exception): pass
来源：http://ilh.andypj.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://lge.nwbrower.top

JS:   class MyError extends Error {}
来源：http://agc.yuxming.cn

TS:   class MyError extends Error {}
来源：http://nwm.hnqzz.top

Java: class MyException extends RuntimeException {}
来源：http://ure.yonumen.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fgu.aizwys.cn

Ruby: class MyError < StandardError; end
来源：http://rpa.xziqi.cn

C#:   class MyException : Exception {}
来源：http://ohs.jinghuilouyu.cn

[H05] 捕获特定类型
来源：http://jtd.ybcxt.top

Py:   except ValueError as e:
来源：http://wxi.aizwys.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jbm.bbcook.cn

JS:   if (e instanceof TypeError) {}
来源：http://jry.jinqigufen.top

TS:   if (e instanceof TypeError) {}
来源：http://oqw.yuanzhike.top

Java: catch (IOException | SQLException e) {}
来源：http://tvk.sysykeji.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://stf.fktsv.cn

Ruby: rescue ArgumentError => e
来源：http://kpm.quarkkingdee.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://iyu.yangfankeji.com

[H06] 可选值 / 空值安全访问
来源：http://nyu.feifeiyinyue.top

Py:   value = d.get("k") or default
来源：http://taj.xinyue.icu

PHP:  $v = $d["k"] ?? null;
来源：http://cwv.tian-w.cn

JS:   obj?.a?.b;  d ?? default
来源：http://afd.tian-w.cn

TS:   obj?.a?.b;  d ?? default
来源：http://nxl.shanyushiyangkeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gsh.andypj.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://snr.yj20258888.top

Ruby: d&.dig(:a, :b)
来源：http://utd.vqdsnc.cn

C#:   obj?.A?.B ?? default
来源：http://lyn.vehdjk.com

[H07] 断言
来源：http://jes.chenzaomai.com

Py:   assert x > 0, "必须为正"
来源：http://eya.cqqwz.cn

PHP:  assert($x > 0);
来源：http://qwi.ppjwa.cn

JS:   console.assert(x > 0);
来源：http://joi.havefunace.top

TS:   console.assert(x > 0);
来源：http://yde.tarul.cn

Java: assert x > 0 : "必须为正";
来源：http://dij.chenlongwang.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pub.pycfn.com

Ruby: raise "必须为正" unless x > 0
来源：http://pyk.xziqi.cn

C#:   Debug.Assert(x > 0);
来源：http://ycc.hammf.cn

[H08] 获取错误信息与堆栈
来源：http://jnn.iojbl.cn

Py:   str(e);  traceback.format_exc()
来源：http://rlq.zdbjq.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wua.zhiwuduotai.top

JS:   e.message;  e.stack
来源：http://wqb.yuxming.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://eem.gzhubu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://yrq.aibaodan.cn

Go:   err.Error()
来源：http://gzj.nwbrower.top

Ruby: e.message;  e.backtrace
来源：http://xfh.epnwcf.com

C#:   e.Message;  e.StackTrace
来源：http://kue.havefunace.top

[H09] 带错误码的异常
来源：http://xxj.316326.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ndi.andypj.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://khm.kuanghao11.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xeb.zhijiandao.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rdp.zhijiandao.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pea.hnqzz.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://woo.xuanzx.com

Ruby: raise MyError.new("fail", 500)
来源：http://wph.yj202588.top

C#:   // 自定义异常类中加 Code 属性
来源：http://bdj.shzxlz.cn

[H10] 资源自动释放
来源：http://vmc.guannengcc.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://xnb.hongshengwenyu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://znr.zdbjq.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://brg.jiagoushi.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://htn.jqgufenzy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tqp.ydjk.org.cn

Go:   defer f.Close()
来源：http://iir.yangfankeji.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://afa.zhengqikj.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xuz.ctjpmb.com

================================================================================
来源：http://jae.jinqigfzy.top

I. 正则表达式
来源：http://ige.uphjek.com

================================================================================
来源：http://uav.quarkkingdee.top

[I01] 判断是否匹配
来源：http://noa.ydzc1.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dar.jyoumei.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vfx.tarul.cn

JS:   /\d+/.test(s)
来源：http://tiq.wangdashe.top

TS:   /\d+/.test(s)
来源：http://gna.yuanzhike.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wue.xziqi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://aws.vqdsnc.cn

Ruby: s.match?(/\d+/)
来源：http://zmu.hywenlv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://avm.hnxiangtu.top

[I02] 提取所有匹配
来源：http://sun.aizwys.cn

Py:   re.findall(r"\d+", s)
来源：http://sfn.aizwys.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lnz.daxiang520.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://thr.xylfe.cn

TS:   s.match(/\d+/g)
来源：http://ryy.zhiwuduotai.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sbc.havefunace.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xfl.guowangkeji.top

Ruby: s.scan(/\d+/)
来源：http://vvk.316326.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wli.gogol.net.cn

[I03] 提取捕获分组
来源：http://qve.tianlin.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://elr.yfazqb.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://apr.jinyuanbaomall.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://aqe.hnqzz.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://adm.xuetiantiany.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fsm.jinqigfzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gpl.iojbl.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://met.pycfn.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ero.fzhhl.top

[I04] 正则替换
来源：http://wcb.gzhubu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://zed.yfazqb.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vxt.zhixingplan.top

JS:   s.replace(/\d+/g, "#")
来源：http://zrq.aizwys.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lta.yongpay.top

Java: s.replaceAll("\\d+", "#")
来源：http://wwg.haohaochexian.top

Go:   re.ReplaceAllString(s, "#")
来源：http://qhb.ppjwa.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yjr.snrcjt.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dma.xziqi.cn

[I05] 按正则拆分
来源：http://fqf.snrcjt.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zei.xylfe.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hsm.redwolf501.top

JS:   s.split(/\s*,\s*/)
来源：http://vho.havefunace.top

TS:   s.split(/\s*,\s*/)
来源：http://lkn.zhiwuduotai.top

Java: s.split("\\s*,\\s*")
来源：http://qua.zhiwuduotai.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vnd.zhengqikj.top

Ruby: s.split(/\s*,\s*/)
来源：http://zim.zhijiandao.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gko.ydzc1.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yti.zhijiandao.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uhs.jinghuilouyu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://myi.andypj.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zlx.kuanghao11.cn


<!-- 参考信息 -->