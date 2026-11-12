代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://euj.yj202588.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xva.jinghuilouyu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wrt.zhongyouzk.top

C#:   // 无内置：用 CsvHelper 库
来源：http://fww.zhoulong.xyz

================================================================================
来源：http://rzw.xuanzx.com

G. 面向对象
来源：http://chs.yueranfly.top

================================================================================
来源：http://vsd.nwbrower.top

[G01] 定义类
来源：http://mzr.jqgfzy.top

Py:   class User: pass
来源：http://ewo.sjlbkw.cn

PHP:  class User {}
来源：http://tup.gzhubu.top

JS:   class User {}
来源：http://myc.quarkkingdee.top

TS:   class User { name: string = ""; }
来源：http://zxh.aibaodan.cn

Java: class User {}
来源：http://zhe.c1oappe.top

Go:   type User struct { Name string }
来源：http://igf.shangyingyoupin.top

Ruby: class User; end
来源：http://nln.hnqzz.top

C#:   class User {}
来源：http://gdh.jianghu66.top

[G02] 构造函数
来源：http://iqg.sysykeji.top

Py:   def __init__(self, name): self.name = name
来源：http://avu.tian-w.cn

PHP:  public function __construct(public string $name) {}
来源：http://vyo.hcnkem.com

JS:   constructor(name) { this.name = name; }
来源：http://cfm.haohaochexian.top

TS:   constructor(public name: string) {}
来源：http://twe.shangyingyoupin.top

Java: User(String name) { this.name = name; }
来源：http://uui.xinyue.icu

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xpw.xingfuxueyuan.xyz

Ruby: def initialize(name); @name = name; end
来源：http://wkx.yanxiufei.cn

C#:   public User(string name) { Name = name; }
来源：http://tvi.guannengcc.top

[G03] 实例属性
来源：http://xxf.yvedp.cn

Py:   self.name = "x"
来源：http://smd.chenlongwang.top

PHP:  public string $name = "x";
来源：http://vgn.zhongyouzk.top

JS:   this.name = "x";
来源：http://gls.yangfankeji.com

TS:   name: string = "x";
来源：http://cye.chenlongwang.top

Java: private String name;
来源：http://lss.yj20258.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kxp.kuanghao11.cn

Ruby: @name = "x"
来源：http://cpa.jlsjyb.cn

C#:   public string Name { get; set; } = "x";
来源：http://igj.fanxiaobao.xyz

[G04] 定义方法
来源：http://sra.tianlin.xyz

Py:   def greet(self): return self.name
来源：http://nqr.xylfe.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zpv.bjfxy.top

JS:   greet() { return this.name; }
来源：http://bgm.andypj.xyz

TS:   greet(): string { return this.name; }
来源：http://vei.gaohongyu789.top

Java: String greet() { return name; }
来源：http://hdu.svipenyu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qup.zdqjudy.top

Ruby: def greet; @name; end
来源：http://ofk.jqgufenzy.top

C#:   public string Greet() => Name;
来源：http://lve.mhx1999.top

[G05] 继承
来源：http://kjy.yuanzhike.top

Py:   class Admin(User): pass
来源：http://snl.cdnleiting.top

PHP:  class Admin extends User {}
来源：http://tyk.fanxiaobao.xyz

JS:   class Admin extends User {}
来源：http://nac.xuanzx.com

TS:   class Admin extends User {}
来源：http://she.ydjk.org.cn

Java: class Admin extends User {}
来源：http://myf.cheryme.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jrn.jinyuanbaomall.cn

Ruby: class Admin < User; end
来源：http://heo.hywenlv.cn

C#:   class Admin : User {}
来源：http://dos.jinqigufen.top

[G06] 重写方法
来源：http://szp.gogol.net.cn

Py:   def greet(self): return "admin"
来源：http://zkr.daria6918.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://azv.snrcjt.cn

JS:   greet() { return "admin"; }
来源：http://hpz.sufxvd.cn

TS:   greet(): string { return "admin"; }
来源：http://gpd.jianghu66.top

Java: @Override String greet() { return "admin"; }
来源：http://ydx.zhengqikj.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pzo.yongpay.top

Ruby: def greet; "admin"; end
来源：http://kun.sysykeji.top

C#:   public override string Greet() => "admin";
来源：http://maw.hesvh.cn

[G07] 调用父类方法
来源：http://xef.0kj1m.cn

Py:   super().greet()
来源：http://osx.gaohongyu789.top

PHP:  parent::greet();
来源：http://ymt.xuetiantiany.cn

JS:   super.greet();
来源：http://adr.cheryme.top

TS:   super.greet();
来源：http://kuh.316326.xyz

Java: super.greet();
来源：http://irj.zhixingplan.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qrh.fehbvm.com

Ruby: super
来源：http://swo.yanxiufei.cn

C#:   base.Greet();
来源：http://uay.ctjpmb.com

[G08] 静态方法与属性
来源：http://ddh.sysykeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qmd.vehdjk.com

PHP:  public static function f() {}
来源：http://wxo.wangshuangyany.cn

JS:   static f() {}
来源：http://nus.yueranfly.top

TS:   static f(): void {}
来源：http://fld.havefunace.top

Java: static void f() {}
来源：http://fpw.jinghuilouyu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://eak.zhixingplan.top

Ruby: def self.f; end
来源：http://hcf.xinyue.icu

C#:   public static void F() {}
来源：http://btt.kuanghao11.cn

[G09] 接口 / 抽象类
来源：http://glt.fehbvm.com

Py:   from abc import ABC, abstractmethod
来源：http://ppd.epnwcf.com

PHP:  interface Shape { public function area(): float; }
来源：http://ogs.daria6918.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zjr.52xcode.cn

TS:   interface Shape { area(): number; }
来源：http://coo.birdmap.top

Java: interface Shape { double area(); }
来源：http://gaw.c1oappe.top

Go:   type Shape interface { Area() float64 }
来源：http://lwu.jinqigfzy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mtk.quarkkingdee.top

C#:   interface IShape { double Area(); }
来源：http://jxi.zhengqikj.top

[G10] 访问控制
来源：http://rkf.shzxlz.cn

Py:   约定 _protected / __private（不强制）
来源：http://mss.jianghu66.top

PHP:  public / protected / private
来源：http://yin.zhaomingkeji.xyz

JS:   #private 字段；其余公开
来源：http://hst.havefunace.top

TS:   public / protected / private
来源：http://jll.mhx1999.top

Java: public / protected / private / 默认包级
来源：http://nqs.yj20258888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://xls.sweek.top

Ruby: public / protected / private
来源：http://gsi.hnqzz.top

C#:   public / protected / private / internal
来源：http://psm.xingfuxueyuan.xyz

[G11] getter / setter
来源：http://ize.aibaodan.cn

Py:   @property 与 @x.setter
来源：http://gpr.hywenlv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mhv.fktsv.cn

JS:   get name() { return this._name; }
来源：http://otj.zhaomingkeji.xyz

TS:   get name(): string { return this._name; }
来源：http://eae.redwolf501.top

Java: public String getName() { return name; }
来源：http://bml.sweek.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://icr.mhx1999.top

Ruby: attr_accessor :name
来源：http://lyn.svipenyu.cn

C#:   public string Name { get; set; }
来源：http://zgc.jyoumei.cn

[G12] 对象转字符串
来源：http://jxz.sysykeji.top

Py:   def __str__(self): return self.name
来源：http://yhq.nanxinkj.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://sse.wangdashe.top

JS:   toString() { return this.name; }
来源：http://afh.chenzaomai.com

TS:   toString(): string { return this.name; }
来源：http://nbn.fktsv.cn

Java: @Override public String toString() { return name; }
来源：http://jyp.gogol.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://alv.jinghuilouyu.cn

Ruby: def to_s; @name; end
来源：http://eza.ivvv.top

C#:   public override string ToString() => Name;
来源：http://iuu.pengpengdd.cyou

[G13] 判断对象类型
来源：http://zmz.hnxiangtu.top

Py:   isinstance(u, User)
来源：http://ier.fengsongda.top

PHP:  $u instanceof User
来源：http://flz.yanxiufei.cn

JS:   u instanceof User
来源：http://nio.jinyuanbaomall.cn

TS:   u instanceof User
来源：http://eev.yongpay.top

Java: u instanceof User
来源：http://bxy.sufxvd.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ksd.gotoacloud.top

Ruby: u.is_a?(User)
来源：http://dip.ybcxt.top

C#:   u is User
来源：http://moz.ehwqpu.com

[G14] 数据类 / record
来源：http://qka.yonumen.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nfi.nanxinkj.top

PHP:  // 用 readonly 属性模拟
来源：http://kgp.yfazqb.com

JS:   // 无内置：普通类或对象字面量
来源：http://trm.havefunace.top

TS:   type User = { name: string; age: number };
来源：http://qbq.bbcook.cn

Java: record User(String name, int age) {}
来源：http://gwk.kuanghao11.cn

Go:   type User struct { Name string; Age int }
来源：http://oyf.shanyushiyangtech.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dee.nanxinkj.top

C#:   record User(string Name, int Age);
来源：http://vcp.sxryk.cn

[G15] 枚举
来源：http://ytx.shzxlz.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zbr.ctjpmb.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://fiz.fzhhl.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ccm.cdnleiting.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vla.smart0.xyz

Java: enum Color { RED, GREEN }
来源：http://zai.yangfankeji.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oyf.dianchejie.cn

Ruby: Color = %i[red green].freeze
来源：http://twa.9152youxi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ygd.daxiang520.top

[G16] 对象转数组 / 字典
来源：http://jrn.tian-w.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wnj.ydjk.org.cn

PHP:  get_object_vars($obj);
来源：http://bdk.haohaochexian.top

JS:   Object.entries(obj)
来源：http://ght.gzhubu.top

TS:   Object.entries(obj)
来源：http://lor.sweek.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vht.ydjk.org.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bko.9152youxi.cn

Ruby: obj.instance_variables
来源：http://aqd.jiagoushi.top

C#:   // 用反射或 System.Text.Json
来源：http://xrb.iojbl.cn

================================================================================
来源：http://kbf.c1oappe.top

H. 异常与错误处理
来源：http://vcd.sweek.top

================================================================================
来源：http://nar.quarkkingdee.top

[H01] try / catch 基础
来源：http://laz.zhengqikj.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mzv.vehdjk.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dga.aizwys.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://djg.zhixingplan.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cic.cheryme.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://oxf.cashguo.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://san.zhiwuduotai.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gbk.ehwqpu.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gbm.bbcook.cn

[H02] finally / ensure 收尾
来源：http://pdv.sxryk.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mxl.zhaomingkeji.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://nsb.hfpthk.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://spz.pycfn.com

TS:   try { f(); } finally { cleanup(); }
来源：http://yxc.uphjek.com

Java: try { f(); } finally { cleanup(); }
来源：http://bok.tanke756.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://rtv.fanxiaobao.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://cst.yj202588.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://jcc.daxiang520.top

[H03] 主动抛出异常
来源：http://gjh.yangfankeji.com

Py:   raise ValueError("错误信息")
来源：http://wsg.chenjidiqi.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kax.zdbjq.cn

JS:   throw new Error("错误信息");
来源：http://eag.dianchejie.cn

TS:   throw new Error("错误信息");
来源：http://hoj.jyoumei.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zjr.zdbjq.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gru.chenlongwang.top

Ruby: raise ArgumentError, "错误信息"
来源：http://cjq.dashuyun.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lrm.yj20258888.top

[H04] 自定义异常类型
来源：http://yvh.gotoacloud.top

Py:   class MyError(Exception): pass
来源：http://fjf.aizwys.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jbe.uphjek.com

JS:   class MyError extends Error {}
来源：http://mrq.hammf.cn

TS:   class MyError extends Error {}
来源：http://znb.zhijiandao.cn

Java: class MyException extends RuntimeException {}
来源：http://mlw.nanxinkj.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://aff.kuanghao11.cn

Ruby: class MyError < StandardError; end
来源：http://rum.guannengcc.top

C#:   class MyException : Exception {}
来源：http://rix.c1oappe.top

[H05] 捕获特定类型
来源：http://hcm.hysaishi.cn

Py:   except ValueError as e:
来源：http://cwc.yanxiufei.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qcv.daxiang520.top

JS:   if (e instanceof TypeError) {}
来源：http://kej.quarkkingdee.top

TS:   if (e instanceof TypeError) {}
来源：http://wyo.zhengqikj.top

Java: catch (IOException | SQLException e) {}
来源：http://grf.mhx1999.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ybd.zhongyouzk.top

Ruby: rescue ArgumentError => e
来源：http://hvi.jinyuanbaomall.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xot.nanxinkj.top

[H06] 可选值 / 空值安全访问
来源：http://hzn.zhoulong.xyz

Py:   value = d.get("k") or default
来源：http://plb.yvedp.cn

PHP:  $v = $d["k"] ?? null;
来源：http://nur.yangfankeji.com

JS:   obj?.a?.b;  d ?? default
来源：http://ely.tanke756.top

TS:   obj?.a?.b;  d ?? default
来源：http://bla.sufxvd.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bre.sjlbkw.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://awd.9152youxi.cn

Ruby: d&.dig(:a, :b)
来源：http://vav.jianghu66.top

C#:   obj?.A?.B ?? default
来源：http://dli.feifeiyinyue.top

[H07] 断言
来源：http://gcs.ehwqpu.com

Py:   assert x > 0, "必须为正"
来源：http://exw.shangyingyoupin.top

PHP:  assert($x > 0);
来源：http://sfp.ybcxt.top

JS:   console.assert(x > 0);
来源：http://uav.hfpthk.cn

TS:   console.assert(x > 0);
来源：http://gwd.sweek.top

Java: assert x > 0 : "必须为正";
来源：http://oyd.yanxiufei.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ixu.snrcjt.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zme.uphjek.com

C#:   Debug.Assert(x > 0);
来源：http://cjm.yuxming.cn

[H08] 获取错误信息与堆栈
来源：http://gkw.hywenlv.cn

Py:   str(e);  traceback.format_exc()
来源：http://dxx.jiagoushi.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mqo.zhengqikj.top

JS:   e.message;  e.stack
来源：http://wwn.guowangkeji.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://gqs.yangfankeji.com

Java: e.getMessage();  e.printStackTrace()
来源：http://gzf.zhijiandao.cn

Go:   err.Error()
来源：http://bze.shzxlz.cn

Ruby: e.message;  e.backtrace
来源：http://ahp.yj202588.top

C#:   e.Message;  e.StackTrace
来源：http://ofd.fengsongda.top

[H09] 带错误码的异常
来源：http://lor.gaohongyu789.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://krc.epnwcf.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://fxk.yfazqb.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://iso.gogol.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gnx.sxryk.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fzo.birdmap.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sqm.andypj.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://qtz.zycfv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://guo.guowangkeji.top

[H10] 资源自动释放
来源：http://ahy.dianchejie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lvl.haohaochexian.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://goi.uphjek.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hfu.zhijiandao.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nlt.xylfe.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ijx.yangfankeji.com

Go:   defer f.Close()
来源：http://lap.dianchejie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sux.tanke756.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mod.birdmap.top

================================================================================
来源：http://lnl.yuxming.cn

I. 正则表达式
来源：http://bby.bjfxy.top

================================================================================
来源：http://lbz.zhixingplan.top

[I01] 判断是否匹配
来源：http://pet.bbcook.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jok.smart0.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://tfz.yj20258888.top

JS:   /\d+/.test(s)
来源：http://utb.yuanzhike.top

TS:   /\d+/.test(s)
来源：http://xko.zdbjq.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://srr.jlsjyb.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pmt.cdnleiting.top

Ruby: s.match?(/\d+/)
来源：http://bln.chenzaomai.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fdx.aizwys.cn

[I02] 提取所有匹配
来源：http://khw.mhx1999.top

Py:   re.findall(r"\d+", s)
来源：http://eqd.yuxming.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://czu.zdqjudy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zyw.ydjk.org.cn

TS:   s.match(/\d+/g)
来源：http://tzh.fzhhl.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xhl.cashguo.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pdb.ywan-chungtsiang.top

Ruby: s.scan(/\d+/)
来源：http://aqi.cqqwz.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qfw.yj20258.top

[I03] 提取捕获分组
来源：http://ddk.9152youxi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vwr.zdbjq.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mii.yonumen.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hdv.guowangkeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mmh.wangdashe.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yka.fehbvm.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gwj.redwolf501.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qgn.gogol.net.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zlg.ehwqpu.com

[I04] 正则替换
来源：http://zoh.daxiang520.top

Py:   re.sub(r"\d+", "#", s)
来源：http://lfx.jyoumei.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vqk.jinghuilouyu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://vyi.aizwys.cn

TS:   s.replace(/\d+/g, "#")
来源：http://njr.wangdashe.top

Java: s.replaceAll("\\d+", "#")
来源：http://ndb.sysykeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://yyx.yvedp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://uyc.chenzaomai.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gpx.gogol.net.cn

[I05] 按正则拆分
来源：http://wvi.ydjk.org.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mou.zycfv.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yfi.hongshengwenyu.top

JS:   s.split(/\s*,\s*/)
来源：http://mvs.hysaishi.cn

TS:   s.split(/\s*,\s*/)
来源：http://klh.xingfuxueyuan.xyz

Java: s.split("\\s*,\\s*")
来源：http://mmw.jinqigfzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://byh.sweek.top

Ruby: s.split(/\s*,\s*/)
来源：http://qho.fanxiaobao.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hxl.ivvv.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ayu.iojbl.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://brj.yonumen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vxx.fanxiaobao.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://owe.sysykeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://few.hammf.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bjb.jlsjyb.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://oop.yvedp.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xun.daria6918.cn


<!-- 参考信息 -->