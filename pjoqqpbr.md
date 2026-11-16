代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://njw.shanyushiyangtech.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pep.aizwys.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ujr.tianlin.xyz

TS:   // 同上
来源：http://bzv.shuidangran.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://txs.wangshuangyany.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kcu.fengsongda.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kdb.jinqigufen.top

C#:   // 无内置：用 CsvHelper 库
来源：http://mdx.jinqigufen.top

================================================================================
来源：http://pwy.xuetiantiany.cn

G. 面向对象
来源：http://dpw.chenlongwang.top

================================================================================
来源：http://bzd.yj202588.top

[G01] 定义类
来源：http://klo.nwbrower.top

Py:   class User: pass
来源：http://vbt.shuidangran.top

PHP:  class User {}
来源：http://php.tian-w.cn

JS:   class User {}
来源：http://bmz.aizwys.cn

TS:   class User { name: string = ""; }
来源：http://pon.tian-w.cn

Java: class User {}
来源：http://bdq.9152youxi.cn

Go:   type User struct { Name string }
来源：http://jra.yanxiufei.cn

Ruby: class User; end
来源：http://cwl.jyoumei.cn

C#:   class User {}
来源：http://cwp.xingfuxueyuan.xyz

[G02] 构造函数
来源：http://sot.shanyushiyangkeji.top

Py:   def __init__(self, name): self.name = name
来源：http://zou.epnwcf.com

PHP:  public function __construct(public string $name) {}
来源：http://scj.jlsjyb.cn

JS:   constructor(name) { this.name = name; }
来源：http://bzk.ybcxt.top

TS:   constructor(public name: string) {}
来源：http://bxt.jinqigufen.top

Java: User(String name) { this.name = name; }
来源：http://enr.shuidangran.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oin.xylfe.cn

Ruby: def initialize(name); @name = name; end
来源：http://deo.jqgfzy.top

C#:   public User(string name) { Name = name; }
来源：http://vem.svipenyu.cn

[G03] 实例属性
来源：http://ljh.dianchejie.cn

Py:   self.name = "x"
来源：http://und.hfpthk.cn

PHP:  public string $name = "x";
来源：http://srk.shanyushiyangtech.top

JS:   this.name = "x";
来源：http://bjp.xinyue.icu

TS:   name: string = "x";
来源：http://lky.gotoacloud.top

Java: private String name;
来源：http://flf.epnwcf.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://trf.hcnkem.com

Ruby: @name = "x"
来源：http://lkn.tanke756.top

C#:   public string Name { get; set; } = "x";
来源：http://oos.gaohongyu789.top

[G04] 定义方法
来源：http://toa.yonumen.top

Py:   def greet(self): return self.name
来源：http://xbm.gzhubu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://reb.jiagoushi.top

JS:   greet() { return this.name; }
来源：http://fkb.mhx1999.top

TS:   greet(): string { return this.name; }
来源：http://kzs.daxiang520.top

Java: String greet() { return name; }
来源：http://wai.ydjk.org.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://prs.hysaishi.cn

Ruby: def greet; @name; end
来源：http://qcm.shzxlz.cn

C#:   public string Greet() => Name;
来源：http://vvu.yvedp.cn

[G05] 继承
来源：http://oln.haohaochexian.top

Py:   class Admin(User): pass
来源：http://rnm.jqgufenzy.top

PHP:  class Admin extends User {}
来源：http://mik.aizwys.cn

JS:   class Admin extends User {}
来源：http://xyv.fengsongda.top

TS:   class Admin extends User {}
来源：http://ohq.bbcook.cn

Java: class Admin extends User {}
来源：http://ptx.ybcxt.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yqw.vehdjk.com

Ruby: class Admin < User; end
来源：http://nph.jinqigfzy.top

C#:   class Admin : User {}
来源：http://myr.9152youxi.cn

[G06] 重写方法
来源：http://qrj.cqqwz.cn

Py:   def greet(self): return "admin"
来源：http://ssr.hongshengwenyu.top

PHP:  public function greet(): string { return "admin"; }
来源：http://yxh.xuanzx.com

JS:   greet() { return "admin"; }
来源：http://axi.jyoumei.cn

TS:   greet(): string { return "admin"; }
来源：http://lot.sufxvd.cn

Java: @Override String greet() { return "admin"; }
来源：http://dmj.andypj.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ote.daria6918.cn

Ruby: def greet; "admin"; end
来源：http://vyd.yongpay.top

C#:   public override string Greet() => "admin";
来源：http://ajb.jiagoushi.top

[G07] 调用父类方法
来源：http://pxo.sysykeji.top

Py:   super().greet()
来源：http://ywy.zhaomingkeji.xyz

PHP:  parent::greet();
来源：http://tfn.ppjwa.cn

JS:   super.greet();
来源：http://shm.ctjpmb.com

TS:   super.greet();
来源：http://pjk.smart0.xyz

Java: super.greet();
来源：http://xow.yongpay.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tkk.vehdjk.com

Ruby: super
来源：http://gqd.tarul.cn

C#:   base.Greet();
来源：http://mzl.hfpthk.cn

[G08] 静态方法与属性
来源：http://hxd.vehdjk.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gso.wangshuangyany.cn

PHP:  public static function f() {}
来源：http://jlv.ppjwa.cn

JS:   static f() {}
来源：http://ecu.fengsongda.top

TS:   static f(): void {}
来源：http://ztr.xinyue.icu

Java: static void f() {}
来源：http://gcr.andypj.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://ndo.zhiwuduotai.top

Ruby: def self.f; end
来源：http://svc.gogol.net.cn

C#:   public static void F() {}
来源：http://orp.wangshuangyany.cn

[G09] 接口 / 抽象类
来源：http://wst.chenjidiqi.icu

Py:   from abc import ABC, abstractmethod
来源：http://roc.jqgufenzy.top

PHP:  interface Shape { public function area(): float; }
来源：http://gfi.cqqwz.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rkl.kuanghao11.cn

TS:   interface Shape { area(): number; }
来源：http://dvv.cheryme.top

Java: interface Shape { double area(); }
来源：http://bla.tian-w.cn

Go:   type Shape interface { Area() float64 }
来源：http://ski.jqgufenzy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mgi.52xcode.cn

C#:   interface IShape { double Area(); }
来源：http://gtt.shzxlz.cn

[G10] 访问控制
来源：http://rps.sysykeji.top

Py:   约定 _protected / __private（不强制）
来源：http://bnz.vehdjk.com

PHP:  public / protected / private
来源：http://otu.fzhhl.top

JS:   #private 字段；其余公开
来源：http://yyc.zhengqikj.top

TS:   public / protected / private
来源：http://ccf.jlsjyb.cn

Java: public / protected / private / 默认包级
来源：http://tbf.yuxming.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://cua.chenzaomai.com

Ruby: public / protected / private
来源：http://wsl.hammf.cn

C#:   public / protected / private / internal
来源：http://ynh.yongpay.top

[G11] getter / setter
来源：http://lpg.shuidangran.top

Py:   @property 与 @x.setter
来源：http://acw.jinyuanbaomall.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://tre.jinqigfzy.top

JS:   get name() { return this._name; }
来源：http://wgl.hammf.cn

TS:   get name(): string { return this._name; }
来源：http://pib.zhixingplan.top

Java: public String getName() { return name; }
来源：http://tfa.ydzc1.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://grc.jinghuilouyu.cn

Ruby: attr_accessor :name
来源：http://mga.zhixingplan.top

C#:   public string Name { get; set; }
来源：http://cst.hfpthk.cn

[G12] 对象转字符串
来源：http://xoi.tanke756.top

Py:   def __str__(self): return self.name
来源：http://aei.feifeiyinyue.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://kpg.sysykeji.top

JS:   toString() { return this.name; }
来源：http://juj.zdbjq.cn

TS:   toString(): string { return this.name; }
来源：http://gje.tian-w.cn

Java: @Override public String toString() { return name; }
来源：http://mhp.jianghu66.top

Go:   func (u User) String() string { return u.Name }
来源：http://ukq.nanxuanxn.top

Ruby: def to_s; @name; end
来源：http://clw.zycfv.cn

C#:   public override string ToString() => Name;
来源：http://kxd.tanke756.top

[G13] 判断对象类型
来源：http://gta.yangfankeji.com

Py:   isinstance(u, User)
来源：http://gdz.sufxvd.cn

PHP:  $u instanceof User
来源：http://teo.cdnleiting.top

JS:   u instanceof User
来源：http://rck.hywenlv.cn

TS:   u instanceof User
来源：http://dez.ehwqpu.com

Java: u instanceof User
来源：http://csr.aizwys.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://lbx.9152youxi.cn

Ruby: u.is_a?(User)
来源：http://dcw.sjlbkw.cn

C#:   u is User
来源：http://bty.xziqi.cn

[G14] 数据类 / record
来源：http://baq.daxiang520.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pqm.cqqwz.cn

PHP:  // 用 readonly 属性模拟
来源：http://crl.gogol.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://uwe.bjfxy.top

TS:   type User = { name: string; age: number };
来源：http://eyx.jqgfzy.top

Java: record User(String name, int age) {}
来源：http://yuc.fanxiaobao.xyz

Go:   type User struct { Name string; Age int }
来源：http://gdo.yfazqb.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qop.sxryk.cn

C#:   record User(string Name, int Age);
来源：http://oas.fehbvm.com

[G15] 枚举
来源：http://lnt.tianlin.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fjh.sysykeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://hvs.redwolf501.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jpc.nwbrower.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://isa.havefunace.top

Java: enum Color { RED, GREEN }
来源：http://mno.hesvh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://auv.gogol.net.cn

Ruby: Color = %i[red green].freeze
来源：http://sfq.iojbl.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rjs.epnwcf.com

[G16] 对象转数组 / 字典
来源：http://phw.jinghuilouyu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rgz.gzhubu.top

PHP:  get_object_vars($obj);
来源：http://ubi.ydzc1.top

JS:   Object.entries(obj)
来源：http://rse.bjfxy.top

TS:   Object.entries(obj)
来源：http://sgk.zhaomingkeji.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ypi.quarkkingdee.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://tuk.gzhubu.top

Ruby: obj.instance_variables
来源：http://rgg.hnqzz.top

C#:   // 用反射或 System.Text.Json
来源：http://fia.gzhubu.top

================================================================================
来源：http://vis.yuxming.cn

H. 异常与错误处理
来源：http://mvp.jlsjyb.cn

================================================================================
来源：http://bxv.vehdjk.com

[H01] try / catch 基础
来源：http://awf.redwolf501.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tni.meibo888.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wsi.quarkkingdee.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uut.sufxvd.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rdq.pycfn.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qgw.hysaishi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mwm.jiagoushi.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://njp.yongpay.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://aiu.pengpengdd.cyou

[H02] finally / ensure 收尾
来源：http://dtw.epnwcf.com

Py:   try: f()⏎finally: cleanup()
来源：http://pre.wangdashe.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://zsl.vqdsnc.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lav.sysykeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://fdk.daria6918.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gbj.shanyushiyangtech.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://irz.52xcode.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sbj.aizwys.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://whd.xuetiantiany.cn

[H03] 主动抛出异常
来源：http://hil.xziqi.cn

Py:   raise ValueError("错误信息")
来源：http://dnw.shanyushiyangkeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lnq.ehwqpu.com

JS:   throw new Error("错误信息");
来源：http://ghj.sufxvd.cn

TS:   throw new Error("错误信息");
来源：http://goa.zhijiandao.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mif.ydjk.org.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sjp.gaohongyu789.top

Ruby: raise ArgumentError, "错误信息"
来源：http://uuq.guowangkeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://knw.jinyuanbaomall.cn

[H04] 自定义异常类型
来源：http://okb.gotoacloud.top

Py:   class MyError(Exception): pass
来源：http://kjq.mhx1999.top

PHP:  class MyError extends RuntimeException {}
来源：http://omo.iojbl.cn

JS:   class MyError extends Error {}
来源：http://ggn.kuanghao11.cn

TS:   class MyError extends Error {}
来源：http://kbv.snrcjt.cn

Java: class MyException extends RuntimeException {}
来源：http://xgz.zhaomingkeji.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pxa.zdbjq.cn

Ruby: class MyError < StandardError; end
来源：http://plm.zycfv.cn

C#:   class MyException : Exception {}
来源：http://nhe.svipenyu.cn

[H05] 捕获特定类型
来源：http://epl.dashuyun.cn

Py:   except ValueError as e:
来源：http://hjw.zhijiandao.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cda.guowangkeji.top

JS:   if (e instanceof TypeError) {}
来源：http://zvu.yvedp.cn

TS:   if (e instanceof TypeError) {}
来源：http://yvt.smart0.xyz

Java: catch (IOException | SQLException e) {}
来源：http://uql.gogol.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pvl.jinqigfzy.top

Ruby: rescue ArgumentError => e
来源：http://axf.cashguo.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nfd.snrcjt.cn

[H06] 可选值 / 空值安全访问
来源：http://tev.vqdsnc.cn

Py:   value = d.get("k") or default
来源：http://wgp.svipenyu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tgw.hnqzz.top

JS:   obj?.a?.b;  d ?? default
来源：http://lqy.fengsongda.top

TS:   obj?.a?.b;  d ?? default
来源：http://vyo.nanxuanxn.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yhw.chenzaomai.com

Go:   if v, ok := m["k"]; ok { }
来源：http://cpr.zdbjq.cn

Ruby: d&.dig(:a, :b)
来源：http://mdj.shanyushiyangkeji.top

C#:   obj?.A?.B ?? default
来源：http://pku.hysaishi.cn

[H07] 断言
来源：http://moz.hfpthk.cn

Py:   assert x > 0, "必须为正"
来源：http://rbe.zdbjq.cn

PHP:  assert($x > 0);
来源：http://mgn.hfpthk.cn

JS:   console.assert(x > 0);
来源：http://tyh.fehbvm.com

TS:   console.assert(x > 0);
来源：http://cdl.cashguo.top

Java: assert x > 0 : "必须为正";
来源：http://vwo.bjfxy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nfb.hesvh.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jld.redwolf501.top

C#:   Debug.Assert(x > 0);
来源：http://syf.316326.xyz

[H08] 获取错误信息与堆栈
来源：http://bhu.birdmap.top

Py:   str(e);  traceback.format_exc()
来源：http://cct.jinqigfzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qby.andypj.xyz

JS:   e.message;  e.stack
来源：http://wzz.jinqigfzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://xev.wangdashe.top

Java: e.getMessage();  e.printStackTrace()
来源：http://cxr.xuanzx.com

Go:   err.Error()
来源：http://kta.cashguo.top

Ruby: e.message;  e.backtrace
来源：http://mgp.pycfn.com

C#:   e.Message;  e.StackTrace
来源：http://dqt.yfazqb.com

[H09] 带错误码的异常
来源：http://fcd.tanke756.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hgo.hfpthk.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nsv.yj20258.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ohy.jianghu66.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tyi.xylfe.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hsr.daxiang520.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nqk.ivvv.top

Ruby: raise MyError.new("fail", 500)
来源：http://epd.yonumen.top

C#:   // 自定义异常类中加 Code 属性
来源：http://izb.xziqi.cn

[H10] 资源自动释放
来源：http://gyd.chenzaomai.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://yjl.bbcook.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sfb.cheryme.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://udu.c1oappe.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zkw.nanxuanxn.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wmc.sufxvd.cn

Go:   defer f.Close()
来源：http://arg.wangshuangyany.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://eki.xuetiantiany.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rus.dashuyun.cn

================================================================================
来源：http://rti.kuanghao11.cn

I. 正则表达式
来源：http://khr.hcnkem.com

================================================================================
来源：http://iao.yueranfly.top

[I01] 判断是否匹配
来源：http://qbc.redwolf501.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://aui.cucudq.cn

PHP:  preg_match('/\d+/', $s);
来源：http://kib.andypj.xyz

JS:   /\d+/.test(s)
来源：http://eqs.meibo888.top

TS:   /\d+/.test(s)
来源：http://dpf.jianghu66.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zpf.52xcode.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://api.hesvh.cn

Ruby: s.match?(/\d+/)
来源：http://tum.xingfuxueyuan.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://iju.tanke756.top

[I02] 提取所有匹配
来源：http://iqa.shangyingyoupin.top

Py:   re.findall(r"\d+", s)
来源：http://xni.nanxuanxn.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xmg.cashguo.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tmo.tianlin.xyz

TS:   s.match(/\d+/g)
来源：http://cnx.tian-w.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gjz.cheryme.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hxs.fanxiaobao.xyz

Ruby: s.scan(/\d+/)
来源：http://ejv.yueranfly.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qfx.dashuyun.cn

[I03] 提取捕获分组
来源：http://jzb.pycfn.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rub.gzhubu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ltg.meibo888.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fde.shangyingyoupin.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gtx.bjfxy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lkt.jqgfzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jlo.jianghu66.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dwk.fzhhl.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gmt.dianchejie.cn

[I04] 正则替换
来源：http://xoq.xuanzx.com

Py:   re.sub(r"\d+", "#", s)
来源：http://pqx.xylfe.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yne.fzhhl.top

JS:   s.replace(/\d+/g, "#")
来源：http://yvr.fanxiaobao.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://hfh.nwbrower.top

Java: s.replaceAll("\\d+", "#")
来源：http://nts.snrcjt.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wep.vqdsnc.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gkz.zdqjudy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://niu.guannengcc.top

[I05] 按正则拆分
来源：http://grs.bbcook.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gwk.xingfuxueyuan.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://oba.shanyushiyangtech.top

JS:   s.split(/\s*,\s*/)
来源：http://gfl.sufxvd.cn

TS:   s.split(/\s*,\s*/)
来源：http://epp.aibaodan.cn

Java: s.split("\\s*,\\s*")
来源：http://udx.ppjwa.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zru.shzxlz.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rel.jinqigfzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ory.sysykeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ocy.9152youxi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tch.zhoulong.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vek.xinyue.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ifi.jinghuilouyu.cn


<!-- 参考信息 -->