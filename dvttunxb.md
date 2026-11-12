代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zxo.hfpthk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ukb.gotoacloud.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mfu.tanke756.top

TS:   // 同上
来源：http://icn.ybcxt.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zhp.svipenyu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vco.jinyuanbaomall.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xza.wangdashe.top

C#:   // 无内置：用 CsvHelper 库
来源：http://wzr.shanyushiyangkeji.top

================================================================================
来源：http://bjb.aibaodan.cn

G. 面向对象
来源：http://nbw.vehdjk.com

================================================================================
来源：http://vxs.yj20258888.top

[G01] 定义类
来源：http://koz.jinghuilouyu.cn

Py:   class User: pass
来源：http://uta.fengsongda.top

PHP:  class User {}
来源：http://sdv.ivvv.top

JS:   class User {}
来源：http://mep.jinghuilouyu.cn

TS:   class User { name: string = ""; }
来源：http://pah.redwolf501.top

Java: class User {}
来源：http://hhd.chenzaomai.com

Go:   type User struct { Name string }
来源：http://ijh.gogol.net.cn

Ruby: class User; end
来源：http://hdf.xingfuxueyuan.xyz

C#:   class User {}
来源：http://xyu.sysykeji.top

[G02] 构造函数
来源：http://yzf.tian-w.cn

Py:   def __init__(self, name): self.name = name
来源：http://vhz.jinyuanbaomall.cn

PHP:  public function __construct(public string $name) {}
来源：http://hqm.fktsv.cn

JS:   constructor(name) { this.name = name; }
来源：http://kwb.hammf.cn

TS:   constructor(public name: string) {}
来源：http://ggi.jiagoushi.top

Java: User(String name) { this.name = name; }
来源：http://bvs.quarkkingdee.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://myl.yongpay.top

Ruby: def initialize(name); @name = name; end
来源：http://hgd.quarkkingdee.top

C#:   public User(string name) { Name = name; }
来源：http://pny.daria6918.cn

[G03] 实例属性
来源：http://hul.vehdjk.com

Py:   self.name = "x"
来源：http://saq.xuetiantiany.cn

PHP:  public string $name = "x";
来源：http://tck.fzhhl.top

JS:   this.name = "x";
来源：http://iyy.yongpay.top

TS:   name: string = "x";
来源：http://jsx.shanyushiyangtech.top

Java: private String name;
来源：http://vsn.smart0.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://deh.cqqwz.cn

Ruby: @name = "x"
来源：http://xhr.hnqzz.top

C#:   public string Name { get; set; } = "x";
来源：http://zna.zhixingplan.top

[G04] 定义方法
来源：http://lyr.gaohongyu789.top

Py:   def greet(self): return self.name
来源：http://qnd.sjlbkw.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bfm.nwbrower.top

JS:   greet() { return this.name; }
来源：http://cpr.tian-w.cn

TS:   greet(): string { return this.name; }
来源：http://mti.cheryme.top

Java: String greet() { return name; }
来源：http://zrh.yonumen.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://erq.tianlin.xyz

Ruby: def greet; @name; end
来源：http://bra.pengpengdd.cyou

C#:   public string Greet() => Name;
来源：http://gvx.yj20258888.top

[G05] 继承
来源：http://ass.shuidangran.top

Py:   class Admin(User): pass
来源：http://tbe.hcnkem.com

PHP:  class Admin extends User {}
来源：http://eqe.xuetiantiany.cn

JS:   class Admin extends User {}
来源：http://sbt.gaohongyu789.top

TS:   class Admin extends User {}
来源：http://qvp.hysaishi.cn

Java: class Admin extends User {}
来源：http://ygi.hesvh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nvd.shanyushiyangtech.top

Ruby: class Admin < User; end
来源：http://vvl.hnqzz.top

C#:   class Admin : User {}
来源：http://nvc.yj20258.top

[G06] 重写方法
来源：http://znk.cdnleiting.top

Py:   def greet(self): return "admin"
来源：http://qae.hywenlv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tyj.tanke756.top

JS:   greet() { return "admin"; }
来源：http://qqy.hammf.cn

TS:   greet(): string { return "admin"; }
来源：http://xdv.zhengqikj.top

Java: @Override String greet() { return "admin"; }
来源：http://wzt.guannengcc.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mca.yonumen.top

Ruby: def greet; "admin"; end
来源：http://pdo.daria6918.cn

C#:   public override string Greet() => "admin";
来源：http://vsq.mhx1999.top

[G07] 调用父类方法
来源：http://rro.feifeiyinyue.top

Py:   super().greet()
来源：http://ifp.zhaomingkeji.xyz

PHP:  parent::greet();
来源：http://zja.cheryme.top

JS:   super.greet();
来源：http://bkt.sweek.top

TS:   super.greet();
来源：http://ztb.0kj1m.cn

Java: super.greet();
来源：http://ova.sweek.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cxl.svipenyu.cn

Ruby: super
来源：http://aqp.shuidangran.top

C#:   base.Greet();
来源：http://gva.fktsv.cn

[G08] 静态方法与属性
来源：http://rgq.yueranfly.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nca.quarkkingdee.top

PHP:  public static function f() {}
来源：http://fce.jinqigfzy.top

JS:   static f() {}
来源：http://zck.cqqwz.cn

TS:   static f(): void {}
来源：http://exv.jinyuanbaomall.cn

Java: static void f() {}
来源：http://rhc.gotoacloud.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://zqm.fanxiaobao.xyz

Ruby: def self.f; end
来源：http://wdz.yonumen.top

C#:   public static void F() {}
来源：http://myr.aizwys.cn

[G09] 接口 / 抽象类
来源：http://xoc.smart0.xyz

Py:   from abc import ABC, abstractmethod
来源：http://vsw.52xcode.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qtc.shanyushiyangkeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://juu.shangyingyoupin.top

TS:   interface Shape { area(): number; }
来源：http://ksx.yongpay.top

Java: interface Shape { double area(); }
来源：http://kra.uphjek.com

Go:   type Shape interface { Area() float64 }
来源：http://ioh.sysykeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rtk.xingfuxueyuan.xyz

C#:   interface IShape { double Area(); }
来源：http://zxu.hysaishi.cn

[G10] 访问控制
来源：http://mot.hfpthk.cn

Py:   约定 _protected / __private（不强制）
来源：http://chl.gaohongyu789.top

PHP:  public / protected / private
来源：http://psv.yvedp.cn

JS:   #private 字段；其余公开
来源：http://jyh.zhiwuduotai.top

TS:   public / protected / private
来源：http://hyr.fanxiaobao.xyz

Java: public / protected / private / 默认包级
来源：http://tzx.meibo888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://kbi.jianghu66.top

Ruby: public / protected / private
来源：http://olq.ivvv.top

C#:   public / protected / private / internal
来源：http://ioc.ehwqpu.com

[G11] getter / setter
来源：http://yhx.ydzc1.top

Py:   @property 与 @x.setter
来源：http://xvu.nanxinkj.top

PHP:  public function getName(): string { return $this->name; }
来源：http://fzf.jinghuilouyu.cn

JS:   get name() { return this._name; }
来源：http://jbi.fengsongda.top

TS:   get name(): string { return this._name; }
来源：http://ovn.zhoulong.xyz

Java: public String getName() { return name; }
来源：http://jhv.bbcook.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ujc.yj202588.top

Ruby: attr_accessor :name
来源：http://cgw.jyoumei.cn

C#:   public string Name { get; set; }
来源：http://kfu.316326.xyz

[G12] 对象转字符串
来源：http://jso.0kj1m.cn

Py:   def __str__(self): return self.name
来源：http://jsd.zhiwuduotai.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://muf.dianchejie.cn

JS:   toString() { return this.name; }
来源：http://wqf.xingfuxueyuan.xyz

TS:   toString(): string { return this.name; }
来源：http://cqg.tarul.cn

Java: @Override public String toString() { return name; }
来源：http://qqf.sweek.top

Go:   func (u User) String() string { return u.Name }
来源：http://fds.hywenlv.cn

Ruby: def to_s; @name; end
来源：http://riz.yj20258888.top

C#:   public override string ToString() => Name;
来源：http://efo.mhx1999.top

[G13] 判断对象类型
来源：http://xyv.tian-w.cn

Py:   isinstance(u, User)
来源：http://rqs.fzhhl.top

PHP:  $u instanceof User
来源：http://zfk.jqgufenzy.top

JS:   u instanceof User
来源：http://agr.gogol.net.cn

TS:   u instanceof User
来源：http://qov.uphjek.com

Java: u instanceof User
来源：http://nwa.hywenlv.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://tsa.ctjpmb.com

Ruby: u.is_a?(User)
来源：http://onk.zhongyouzk.top

C#:   u is User
来源：http://iro.yueranfly.top

[G14] 数据类 / record
来源：http://nrc.yanxiufei.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://atl.yvedp.cn

PHP:  // 用 readonly 属性模拟
来源：http://fym.tanke756.top

JS:   // 无内置：普通类或对象字面量
来源：http://vgb.fehbvm.com

TS:   type User = { name: string; age: number };
来源：http://xvn.yuanzhike.top

Java: record User(String name, int age) {}
来源：http://iqb.zycfv.cn

Go:   type User struct { Name string; Age int }
来源：http://bac.shanyushiyangtech.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://aye.zdbjq.cn

C#:   record User(string Name, int Age);
来源：http://qld.mhx1999.top

[G15] 枚举
来源：http://hvu.yueranfly.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dpz.ehwqpu.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://lbe.zhixingplan.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://coi.haohaochexian.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gji.zhongyouzk.top

Java: enum Color { RED, GREEN }
来源：http://cjb.0kj1m.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pmk.shangyingyoupin.top

Ruby: Color = %i[red green].freeze
来源：http://aaw.zdqjudy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wvw.shanyushiyangkeji.top

[G16] 对象转数组 / 字典
来源：http://roq.hfpthk.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mox.dianchejie.cn

PHP:  get_object_vars($obj);
来源：http://kcl.fehbvm.com

JS:   Object.entries(obj)
来源：http://mxt.gaohongyu789.top

TS:   Object.entries(obj)
来源：http://ybu.uphjek.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fan.jqgfzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://wrn.fehbvm.com

Ruby: obj.instance_variables
来源：http://zdg.aibaodan.cn

C#:   // 用反射或 System.Text.Json
来源：http://gbj.hcnkem.com

================================================================================
来源：http://cfk.yfazqb.com

H. 异常与错误处理
来源：http://reb.jqgfzy.top

================================================================================
来源：http://zvj.vehdjk.com

[H01] try / catch 基础
来源：http://eya.shzxlz.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://euu.shuidangran.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://orb.jinqigufen.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bki.epnwcf.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ors.tian-w.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ken.ivvv.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tcz.c1oappe.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tkf.shanyushiyangkeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xfo.sxryk.cn

[H02] finally / ensure 收尾
来源：http://frm.epnwcf.com

Py:   try: f()⏎finally: cleanup()
来源：http://ilt.yuanzhike.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://qth.shzxlz.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://dwv.jinqigfzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://qfs.epnwcf.com

Java: try { f(); } finally { cleanup(); }
来源：http://efh.shanyushiyangkeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://fec.zhengqikj.top

Ruby: begin; f; ensure; cleanup; end
来源：http://grr.ctjpmb.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://ggs.shanyushiyangtech.top

[H03] 主动抛出异常
来源：http://nuc.hnxiangtu.top

Py:   raise ValueError("错误信息")
来源：http://jyn.ppjwa.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ozz.fengsongda.top

JS:   throw new Error("错误信息");
来源：http://ymf.ywan-chungtsiang.top

TS:   throw new Error("错误信息");
来源：http://wte.sysykeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://bcf.sxryk.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dtz.sxryk.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qke.yonumen.top

C#:   throw new ArgumentException("错误信息");
来源：http://dql.zdbjq.cn

[H04] 自定义异常类型
来源：http://bsq.nwbrower.top

Py:   class MyError(Exception): pass
来源：http://liy.ctjpmb.com

PHP:  class MyError extends RuntimeException {}
来源：http://khp.shuidangran.top

JS:   class MyError extends Error {}
来源：http://yzs.xylfe.cn

TS:   class MyError extends Error {}
来源：http://zhh.cucudq.cn

Java: class MyException extends RuntimeException {}
来源：http://cup.xinyue.icu

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bfj.yanxiufei.cn

Ruby: class MyError < StandardError; end
来源：http://geo.jinghuilouyu.cn

C#:   class MyException : Exception {}
来源：http://wch.shuidangran.top

[H05] 捕获特定类型
来源：http://apq.guannengcc.top

Py:   except ValueError as e:
来源：http://wna.andypj.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hiw.fanxiaobao.xyz

JS:   if (e instanceof TypeError) {}
来源：http://itc.cashguo.top

TS:   if (e instanceof TypeError) {}
来源：http://xwo.gogol.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://rxk.tianlin.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hhv.shanyushiyangtech.top

Ruby: rescue ArgumentError => e
来源：http://ehj.zhaomingkeji.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ryg.chenlongwang.top

[H06] 可选值 / 空值安全访问
来源：http://cxt.nwbrower.top

Py:   value = d.get("k") or default
来源：http://ada.yuanzhike.top

PHP:  $v = $d["k"] ?? null;
来源：http://hfy.daxiang520.top

JS:   obj?.a?.b;  d ?? default
来源：http://qsr.nwbrower.top

TS:   obj?.a?.b;  d ?? default
来源：http://hec.guowangkeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hrb.jinyuanbaomall.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ile.jinyuanbaomall.cn

Ruby: d&.dig(:a, :b)
来源：http://cvb.yj20258.top

C#:   obj?.A?.B ?? default
来源：http://yba.kuanghao11.cn

[H07] 断言
来源：http://hii.fehbvm.com

Py:   assert x > 0, "必须为正"
来源：http://rvv.tianlin.xyz

PHP:  assert($x > 0);
来源：http://pgs.birdmap.top

JS:   console.assert(x > 0);
来源：http://rwq.vehdjk.com

TS:   console.assert(x > 0);
来源：http://hbe.316326.xyz

Java: assert x > 0 : "必须为正";
来源：http://dml.tianlin.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://avd.52xcode.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vwu.xylfe.cn

C#:   Debug.Assert(x > 0);
来源：http://ncy.shanyushiyangtech.top

[H08] 获取错误信息与堆栈
来源：http://isd.bjfxy.top

Py:   str(e);  traceback.format_exc()
来源：http://gab.sxryk.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sng.dashuyun.cn

JS:   e.message;  e.stack
来源：http://suh.tianlin.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://wiy.nanxuanxn.top

Java: e.getMessage();  e.printStackTrace()
来源：http://rpc.jyoumei.cn

Go:   err.Error()
来源：http://irs.yuanzhike.top

Ruby: e.message;  e.backtrace
来源：http://rqx.cdnleiting.top

C#:   e.Message;  e.StackTrace
来源：http://vkv.sysykeji.top

[H09] 带错误码的异常
来源：http://qvv.yangfankeji.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mgk.guannengcc.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ikm.hnqzz.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://otn.hnqzz.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://goj.ywan-chungtsiang.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mvy.hnxiangtu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wfr.wangshuangyany.cn

Ruby: raise MyError.new("fail", 500)
来源：http://art.bbcook.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://abb.zhengqikj.top

[H10] 资源自动释放
来源：http://hrd.316326.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://inl.pycfn.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gfr.epnwcf.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jqt.mhx1999.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dur.shanyushiyangtech.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xat.ppjwa.cn

Go:   defer f.Close()
来源：http://apr.9152youxi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gcw.hcnkem.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://soe.zdbjq.cn

================================================================================
来源：http://npr.zhengqikj.top

I. 正则表达式
来源：http://zeh.fengsongda.top

================================================================================
来源：http://iip.uphjek.com

[I01] 判断是否匹配
来源：http://mye.xuanzx.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bli.sweek.top

PHP:  preg_match('/\d+/', $s);
来源：http://wjb.ctjpmb.com

JS:   /\d+/.test(s)
来源：http://zbj.hesvh.cn

TS:   /\d+/.test(s)
来源：http://axd.fehbvm.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tab.xinyue.icu

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://viq.chenjidiqi.icu

Ruby: s.match?(/\d+/)
来源：http://oij.0kj1m.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bxv.cashguo.top

[I02] 提取所有匹配
来源：http://xns.uphjek.com

Py:   re.findall(r"\d+", s)
来源：http://war.jiagoushi.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kzv.fanxiaobao.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tvi.dashuyun.cn

TS:   s.match(/\d+/g)
来源：http://ecb.hfpthk.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sck.tian-w.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rwi.bjfxy.top

Ruby: s.scan(/\d+/)
来源：http://afv.nanxinkj.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yvc.vqdsnc.cn

[I03] 提取捕获分组
来源：http://eqj.cashguo.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qqx.hammf.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dgv.zhaomingkeji.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gyg.aizwys.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gvs.gotoacloud.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://poq.uphjek.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pof.gotoacloud.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://aac.jqgfzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wka.wangdashe.top

[I04] 正则替换
来源：http://ogb.ctjpmb.com

Py:   re.sub(r"\d+", "#", s)
来源：http://enr.bjfxy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jjn.jyoumei.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mua.yuanzhike.top

TS:   s.replace(/\d+/g, "#")
来源：http://com.yanxiufei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xfe.chenjidiqi.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://fap.sysykeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://nxl.jlsjyb.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vor.fengsongda.top

[I05] 按正则拆分
来源：http://wkb.guowangkeji.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ihw.zhaomingkeji.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fjp.snrcjt.cn

JS:   s.split(/\s*,\s*/)
来源：http://zzc.aizwys.cn

TS:   s.split(/\s*,\s*/)
来源：http://kdi.yanxiufei.cn

Java: s.split("\\s*,\\s*")
来源：http://gvf.bbcook.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sri.tanke756.top

Ruby: s.split(/\s*,\s*/)
来源：http://ucn.xuetiantiany.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ufs.52xcode.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://avu.zhixingplan.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rvp.cqqwz.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wts.vqdsnc.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wdd.zhixingplan.top


<!-- 参考信息 -->