代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yes.zhixingplan.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://amh.zhoulong.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vnf.uphjek.com

[F12] CSV 读写
来源：http://etv.hywenlv.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hnc.zdbjq.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://srp.fengsongda.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cig.zycfv.cn

TS:   // 同上
来源：http://qnp.vehdjk.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://svg.tianlin.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bkw.gotoacloud.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ell.hammf.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://iwn.shanyushiyangkeji.top

================================================================================
来源：http://iwu.yvedp.cn

G. 面向对象
来源：http://jbj.aizwys.cn

================================================================================
来源：http://ddy.ivvv.top

[G01] 定义类
来源：http://dky.sysykeji.top

Py:   class User: pass
来源：http://kjb.yonumen.top

PHP:  class User {}
来源：http://ljh.yj20258888.top

JS:   class User {}
来源：http://nbg.fzhhl.top

TS:   class User { name: string = ""; }
来源：http://loz.ctjpmb.com

Java: class User {}
来源：http://jdx.shangyingyoupin.top

Go:   type User struct { Name string }
来源：http://yoq.cucudq.cn

Ruby: class User; end
来源：http://hku.jqgufenzy.top

C#:   class User {}
来源：http://ffb.sweek.top

[G02] 构造函数
来源：http://uic.cucudq.cn

Py:   def __init__(self, name): self.name = name
来源：http://kvm.xingfuxueyuan.xyz

PHP:  public function __construct(public string $name) {}
来源：http://hml.guannengcc.top

JS:   constructor(name) { this.name = name; }
来源：http://mmb.gzhubu.top

TS:   constructor(public name: string) {}
来源：http://crk.c1oappe.top

Java: User(String name) { this.name = name; }
来源：http://dnu.nwbrower.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gpb.nanxinkj.top

Ruby: def initialize(name); @name = name; end
来源：http://tzu.zhengqikj.top

C#:   public User(string name) { Name = name; }
来源：http://lqw.xuetiantiany.cn

[G03] 实例属性
来源：http://fmg.hysaishi.cn

Py:   self.name = "x"
来源：http://ast.tianlin.xyz

PHP:  public string $name = "x";
来源：http://ndt.wangdashe.top

JS:   this.name = "x";
来源：http://two.zhijiandao.cn

TS:   name: string = "x";
来源：http://cux.yonumen.top

Java: private String name;
来源：http://izd.ivvv.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wly.hysaishi.cn

Ruby: @name = "x"
来源：http://wvw.yuxming.cn

C#:   public string Name { get; set; } = "x";
来源：http://gkm.cdnleiting.top

[G04] 定义方法
来源：http://bcz.zdbjq.cn

Py:   def greet(self): return self.name
来源：http://tmt.fehbvm.com

PHP:  public function greet(): string { return $this->name; }
来源：http://mgn.jinghuilouyu.cn

JS:   greet() { return this.name; }
来源：http://mqj.zhaomingkeji.xyz

TS:   greet(): string { return this.name; }
来源：http://jzu.wangshuangyany.cn

Java: String greet() { return name; }
来源：http://uuo.pycfn.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://qhy.jianghu66.top

Ruby: def greet; @name; end
来源：http://nck.52xcode.cn

C#:   public string Greet() => Name;
来源：http://wug.xinyue.icu

[G05] 继承
来源：http://kia.cqqwz.cn

Py:   class Admin(User): pass
来源：http://jrk.sweek.top

PHP:  class Admin extends User {}
来源：http://yyp.cucudq.cn

JS:   class Admin extends User {}
来源：http://vus.shzxlz.cn

TS:   class Admin extends User {}
来源：http://szr.9152youxi.cn

Java: class Admin extends User {}
来源：http://sux.fzhhl.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cnv.zhengqikj.top

Ruby: class Admin < User; end
来源：http://tlr.jlsjyb.cn

C#:   class Admin : User {}
来源：http://xqf.kuanghao11.cn

[G06] 重写方法
来源：http://hoz.aibaodan.cn

Py:   def greet(self): return "admin"
来源：http://jqe.fanxiaobao.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://led.yuanzhike.top

JS:   greet() { return "admin"; }
来源：http://ruy.bbcook.cn

TS:   greet(): string { return "admin"; }
来源：http://pae.tarul.cn

Java: @Override String greet() { return "admin"; }
来源：http://tvk.guowangkeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tfu.cheryme.top

Ruby: def greet; "admin"; end
来源：http://jzh.hcnkem.com

C#:   public override string Greet() => "admin";
来源：http://pic.cucudq.cn

[G07] 调用父类方法
来源：http://eii.yangfankeji.com

Py:   super().greet()
来源：http://ixr.tianlin.xyz

PHP:  parent::greet();
来源：http://ncp.hywenlv.cn

JS:   super.greet();
来源：http://msz.pengpengdd.cyou

TS:   super.greet();
来源：http://afk.yangfankeji.com

Java: super.greet();
来源：http://huk.yj20258888.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mjn.yj202588.top

Ruby: super
来源：http://fan.jianghu66.top

C#:   base.Greet();
来源：http://gas.yvedp.cn

[G08] 静态方法与属性
来源：http://ijm.fehbvm.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zlo.cdnleiting.top

PHP:  public static function f() {}
来源：http://ujp.bbcook.cn

JS:   static f() {}
来源：http://fba.gzhubu.top

TS:   static f(): void {}
来源：http://jdm.shangyingyoupin.top

Java: static void f() {}
来源：http://gti.chenlongwang.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://jik.yangfankeji.com

Ruby: def self.f; end
来源：http://mcb.sufxvd.cn

C#:   public static void F() {}
来源：http://jtk.gaohongyu789.top

[G09] 接口 / 抽象类
来源：http://wgg.fktsv.cn

Py:   from abc import ABC, abstractmethod
来源：http://ssi.sufxvd.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bmb.hnqzz.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://mzn.tian-w.cn

TS:   interface Shape { area(): number; }
来源：http://cwv.gotoacloud.top

Java: interface Shape { double area(); }
来源：http://drt.birdmap.top

Go:   type Shape interface { Area() float64 }
来源：http://mhb.52xcode.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yfe.52xcode.cn

C#:   interface IShape { double Area(); }
来源：http://ysm.zhengqikj.top

[G10] 访问控制
来源：http://iyx.daria6918.cn

Py:   约定 _protected / __private（不强制）
来源：http://jcs.hammf.cn

PHP:  public / protected / private
来源：http://odl.ehwqpu.com

JS:   #private 字段；其余公开
来源：http://tjn.gaohongyu789.top

TS:   public / protected / private
来源：http://pei.epnwcf.com

Java: public / protected / private / 默认包级
来源：http://cfz.pycfn.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://zcj.zhiwuduotai.top

Ruby: public / protected / private
来源：http://dey.yongpay.top

C#:   public / protected / private / internal
来源：http://nvy.shanyushiyangkeji.top

[G11] getter / setter
来源：http://oih.zhongyouzk.top

Py:   @property 与 @x.setter
来源：http://ldf.aizwys.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://kgv.jinqigufen.top

JS:   get name() { return this._name; }
来源：http://mdw.jianghu66.top

TS:   get name(): string { return this._name; }
来源：http://oef.zhiwuduotai.top

Java: public String getName() { return name; }
来源：http://hqw.zhoulong.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://oit.vehdjk.com

Ruby: attr_accessor :name
来源：http://jtp.dashuyun.cn

C#:   public string Name { get; set; }
来源：http://esf.daxiang520.top

[G12] 对象转字符串
来源：http://yhq.sweek.top

Py:   def __str__(self): return self.name
来源：http://ipa.jinyuanbaomall.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hnd.yanxiufei.cn

JS:   toString() { return this.name; }
来源：http://pfm.xylfe.cn

TS:   toString(): string { return this.name; }
来源：http://lbt.zhoulong.xyz

Java: @Override public String toString() { return name; }
来源：http://kas.tarul.cn

Go:   func (u User) String() string { return u.Name }
来源：http://rwa.xylfe.cn

Ruby: def to_s; @name; end
来源：http://zir.daxiang520.top

C#:   public override string ToString() => Name;
来源：http://nvg.aizwys.cn

[G13] 判断对象类型
来源：http://nnp.vehdjk.com

Py:   isinstance(u, User)
来源：http://vxk.yj20258888.top

PHP:  $u instanceof User
来源：http://fzs.haohaochexian.top

JS:   u instanceof User
来源：http://gcx.sweek.top

TS:   u instanceof User
来源：http://nfm.zhoulong.xyz

Java: u instanceof User
来源：http://bii.cucudq.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ddi.ehwqpu.com

Ruby: u.is_a?(User)
来源：http://vri.zhixingplan.top

C#:   u is User
来源：http://tkj.tianlin.xyz

[G14] 数据类 / record
来源：http://gtw.tanke756.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tcg.tarul.cn

PHP:  // 用 readonly 属性模拟
来源：http://ftr.aizwys.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wic.tian-w.cn

TS:   type User = { name: string; age: number };
来源：http://xss.dianchejie.cn

Java: record User(String name, int age) {}
来源：http://ewy.zhoulong.xyz

Go:   type User struct { Name string; Age int }
来源：http://qmw.yj20258.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zmf.havefunace.top

C#:   record User(string Name, int Age);
来源：http://qey.chenzaomai.com

[G15] 枚举
来源：http://itj.wangdashe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kbw.bbcook.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://cfy.zhiwuduotai.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pko.xziqi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mdn.bbcook.cn

Java: enum Color { RED, GREEN }
来源：http://jqt.shuidangran.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://url.yuanzhike.top

Ruby: Color = %i[red green].freeze
来源：http://wtf.ehwqpu.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rng.yonumen.top

[G16] 对象转数组 / 字典
来源：http://pna.9152youxi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wde.redwolf501.top

PHP:  get_object_vars($obj);
来源：http://cgu.cucudq.cn

JS:   Object.entries(obj)
来源：http://iym.mhx1999.top

TS:   Object.entries(obj)
来源：http://uuf.jiagoushi.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kca.fzhhl.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://xki.sjlbkw.cn

Ruby: obj.instance_variables
来源：http://kso.tianlin.xyz

C#:   // 用反射或 System.Text.Json
来源：http://ndb.tian-w.cn

================================================================================
来源：http://xsn.hnqzz.top

H. 异常与错误处理
来源：http://trd.xinyue.icu

================================================================================
来源：http://mwd.hnxiangtu.top

[H01] try / catch 基础
来源：http://lsa.0kj1m.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://eer.jqgfzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cql.zhiwuduotai.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ilj.tarul.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cif.tarul.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cys.zhengqikj.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ndy.yongpay.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uqc.xinyue.icu

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://avy.jinghuilouyu.cn

[H02] finally / ensure 收尾
来源：http://qbk.xingfuxueyuan.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://jng.yvedp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zqw.zhengqikj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://hiw.fehbvm.com

TS:   try { f(); } finally { cleanup(); }
来源：http://wip.jinqigfzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://ltt.chenlongwang.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://xlz.shzxlz.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wvd.iojbl.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://crg.nwbrower.top

[H03] 主动抛出异常
来源：http://tov.sjlbkw.cn

Py:   raise ValueError("错误信息")
来源：http://mgd.yuxming.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ehs.yanxiufei.cn

JS:   throw new Error("错误信息");
来源：http://jaq.sjlbkw.cn

TS:   throw new Error("错误信息");
来源：http://usk.guannengcc.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://tbi.hesvh.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tzr.yanxiufei.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hyp.tian-w.cn

C#:   throw new ArgumentException("错误信息");
来源：http://czv.aibaodan.cn

[H04] 自定义异常类型
来源：http://dvs.zhijiandao.cn

Py:   class MyError(Exception): pass
来源：http://xes.tian-w.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yhz.guowangkeji.top

JS:   class MyError extends Error {}
来源：http://nyo.redwolf501.top

TS:   class MyError extends Error {}
来源：http://cnx.yongpay.top

Java: class MyException extends RuntimeException {}
来源：http://rjh.meibo888.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lzg.sysykeji.top

Ruby: class MyError < StandardError; end
来源：http://vwp.aibaodan.cn

C#:   class MyException : Exception {}
来源：http://yls.bjfxy.top

[H05] 捕获特定类型
来源：http://wmu.ywan-chungtsiang.top

Py:   except ValueError as e:
来源：http://qof.xingfuxueyuan.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pnu.yfazqb.com

JS:   if (e instanceof TypeError) {}
来源：http://jhj.hysaishi.cn

TS:   if (e instanceof TypeError) {}
来源：http://hkx.bbcook.cn

Java: catch (IOException | SQLException e) {}
来源：http://qod.havefunace.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uda.zycfv.cn

Ruby: rescue ArgumentError => e
来源：http://vni.xuetiantiany.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fup.yj20258888.top

[H06] 可选值 / 空值安全访问
来源：http://tny.bjfxy.top

Py:   value = d.get("k") or default
来源：http://epv.yanxiufei.cn

PHP:  $v = $d["k"] ?? null;
来源：http://yzv.zhongyouzk.top

JS:   obj?.a?.b;  d ?? default
来源：http://reb.cheryme.top

TS:   obj?.a?.b;  d ?? default
来源：http://igb.ivvv.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hqb.zhengqikj.top

Go:   if v, ok := m["k"]; ok { }
来源：http://dmb.xingfuxueyuan.xyz

Ruby: d&.dig(:a, :b)
来源：http://ubg.yj20258.top

C#:   obj?.A?.B ?? default
来源：http://qwe.aibaodan.cn

[H07] 断言
来源：http://lnc.tianlin.xyz

Py:   assert x > 0, "必须为正"
来源：http://cvd.fehbvm.com

PHP:  assert($x > 0);
来源：http://fdg.xylfe.cn

JS:   console.assert(x > 0);
来源：http://unj.sufxvd.cn

TS:   console.assert(x > 0);
来源：http://hps.jqgfzy.top

Java: assert x > 0 : "必须为正";
来源：http://bfg.guannengcc.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dyg.jyoumei.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ojm.tarul.cn

C#:   Debug.Assert(x > 0);
来源：http://rck.jlsjyb.cn

[H08] 获取错误信息与堆栈
来源：http://whg.0kj1m.cn

Py:   str(e);  traceback.format_exc()
来源：http://kyv.guowangkeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://eft.cucudq.cn

JS:   e.message;  e.stack
来源：http://aub.yj202588.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://nov.ivvv.top

Java: e.getMessage();  e.printStackTrace()
来源：http://sfi.ppjwa.cn

Go:   err.Error()
来源：http://imp.bbcook.cn

Ruby: e.message;  e.backtrace
来源：http://zwj.zhixingplan.top

C#:   e.Message;  e.StackTrace
来源：http://jcl.redwolf501.top

[H09] 带错误码的异常
来源：http://guy.tanke756.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nkr.shangyingyoupin.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://yxb.cdnleiting.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ciw.aizwys.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jbb.hesvh.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ryi.jyoumei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zfz.yj20258.top

Ruby: raise MyError.new("fail", 500)
来源：http://akq.shuidangran.top

C#:   // 自定义异常类中加 Code 属性
来源：http://exu.sysykeji.top

[H10] 资源自动释放
来源：http://muv.zdbjq.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://nlx.jianghu66.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://evr.xuanzx.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ucf.zycfv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jrv.sxryk.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://spi.zhoulong.xyz

Go:   defer f.Close()
来源：http://jnm.nanxinkj.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vbx.yonumen.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://khu.yuanzhike.top

================================================================================
来源：http://rxf.shanyushiyangkeji.top

I. 正则表达式
来源：http://wmp.yfazqb.com

================================================================================
来源：http://mic.316326.xyz

[I01] 判断是否匹配
来源：http://tjp.chenlongwang.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jqo.pycfn.com

PHP:  preg_match('/\d+/', $s);
来源：http://xgv.hcnkem.com

JS:   /\d+/.test(s)
来源：http://kev.cqqwz.cn

TS:   /\d+/.test(s)
来源：http://pki.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://knj.ehwqpu.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vfc.fanxiaobao.xyz

Ruby: s.match?(/\d+/)
来源：http://onr.fanxiaobao.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dea.jinyuanbaomall.cn

[I02] 提取所有匹配
来源：http://jod.gzhubu.top

Py:   re.findall(r"\d+", s)
来源：http://oxx.aizwys.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pef.fzhhl.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mti.ppjwa.cn

TS:   s.match(/\d+/g)
来源：http://lgy.cheryme.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://djg.hongshengwenyu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zki.jqgfzy.top

Ruby: s.scan(/\d+/)
来源：http://lrp.yueranfly.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://han.yangfankeji.com

[I03] 提取捕获分组
来源：http://lvr.daria6918.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zwx.birdmap.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vqt.aizwys.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://itg.xingfuxueyuan.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jsx.xylfe.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dgn.hammf.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vge.tanke756.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jdr.316326.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ybd.cashguo.top

[I04] 正则替换
来源：http://olh.bbcook.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kdy.ehwqpu.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://azv.epnwcf.com

JS:   s.replace(/\d+/g, "#")
来源：http://lue.dianchejie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://teq.xuetiantiany.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rdt.yueranfly.top

Go:   re.ReplaceAllString(s, "#")
来源：http://uao.sufxvd.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://iwk.nanxinkj.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xvb.havefunace.top

[I05] 按正则拆分
来源：http://sib.cashguo.top

Py:   re.split(r"\s*,\s*", s)
来源：http://lnp.wangshuangyany.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://boa.ppjwa.cn

JS:   s.split(/\s*,\s*/)
来源：http://pit.hnqzz.top

TS:   s.split(/\s*,\s*/)
来源：http://loq.yuxming.cn

Java: s.split("\\s*,\\s*")
来源：http://kkn.yuxming.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nox.kuanghao11.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pyw.wangshuangyany.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zdr.bjfxy.top


<!-- 参考信息 -->