代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wgu.redwolf501.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cmo.epnwcf.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ccj.tarul.cn

TS:   // 同上
来源：http://whj.zhixingplan.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zmc.xuanzx.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qvd.sjlbkw.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://trm.zdqjudy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://itb.cucudq.cn

================================================================================
来源：http://dhl.ybcxt.top

G. 面向对象
来源：http://bsq.xinyue.icu

================================================================================
来源：http://jmi.jianghu66.top

[G01] 定义类
来源：http://hcq.epnwcf.com

Py:   class User: pass
来源：http://waw.jqgfzy.top

PHP:  class User {}
来源：http://zcv.jinghuilouyu.cn

JS:   class User {}
来源：http://yfo.jinyuanbaomall.cn

TS:   class User { name: string = ""; }
来源：http://hpx.shanyushiyangtech.top

Java: class User {}
来源：http://iev.yuanzhike.top

Go:   type User struct { Name string }
来源：http://jub.sweek.top

Ruby: class User; end
来源：http://vth.jianghu66.top

C#:   class User {}
来源：http://lof.hcnkem.com

[G02] 构造函数
来源：http://ldu.fehbvm.com

Py:   def __init__(self, name): self.name = name
来源：http://ftv.gzhubu.top

PHP:  public function __construct(public string $name) {}
来源：http://coj.dianchejie.cn

JS:   constructor(name) { this.name = name; }
来源：http://tof.shanyushiyangtech.top

TS:   constructor(public name: string) {}
来源：http://wdo.nanxuanxn.top

Java: User(String name) { this.name = name; }
来源：http://can.cashguo.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zsc.hnxiangtu.top

Ruby: def initialize(name); @name = name; end
来源：http://ngg.zycfv.cn

C#:   public User(string name) { Name = name; }
来源：http://khm.zhijiandao.cn

[G03] 实例属性
来源：http://vcm.aizwys.cn

Py:   self.name = "x"
来源：http://jtv.hnxiangtu.top

PHP:  public string $name = "x";
来源：http://ngl.chenlongwang.top

JS:   this.name = "x";
来源：http://wqg.yj20258888.top

TS:   name: string = "x";
来源：http://jpv.nanxuanxn.top

Java: private String name;
来源：http://qum.ybcxt.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vsx.vehdjk.com

Ruby: @name = "x"
来源：http://xwj.xylfe.cn

C#:   public string Name { get; set; } = "x";
来源：http://dve.pengpengdd.cyou

[G04] 定义方法
来源：http://pun.redwolf501.top

Py:   def greet(self): return self.name
来源：http://qti.fanxiaobao.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://omb.jqgufenzy.top

JS:   greet() { return this.name; }
来源：http://dfe.sjlbkw.cn

TS:   greet(): string { return this.name; }
来源：http://nrp.feifeiyinyue.top

Java: String greet() { return name; }
来源：http://cuq.hongshengwenyu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://qds.yfazqb.com

Ruby: def greet; @name; end
来源：http://lve.jlsjyb.cn

C#:   public string Greet() => Name;
来源：http://rhg.sjlbkw.cn

[G05] 继承
来源：http://bjp.hfpthk.cn

Py:   class Admin(User): pass
来源：http://htn.jinqigufen.top

PHP:  class Admin extends User {}
来源：http://xtv.xuetiantiany.cn

JS:   class Admin extends User {}
来源：http://caj.aibaodan.cn

TS:   class Admin extends User {}
来源：http://ymz.zhoulong.xyz

Java: class Admin extends User {}
来源：http://cze.guannengcc.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hbl.hysaishi.cn

Ruby: class Admin < User; end
来源：http://rtc.chenzaomai.com

C#:   class Admin : User {}
来源：http://fpm.0kj1m.cn

[G06] 重写方法
来源：http://obi.jinqigfzy.top

Py:   def greet(self): return "admin"
来源：http://kte.bbcook.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vfa.tian-w.cn

JS:   greet() { return "admin"; }
来源：http://crn.hnqzz.top

TS:   greet(): string { return "admin"; }
来源：http://xsh.daxiang520.top

Java: @Override String greet() { return "admin"; }
来源：http://wuy.havefunace.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://crl.aibaodan.cn

Ruby: def greet; "admin"; end
来源：http://jns.tian-w.cn

C#:   public override string Greet() => "admin";
来源：http://jql.xuanzx.com

[G07] 调用父类方法
来源：http://zfl.hesvh.cn

Py:   super().greet()
来源：http://arl.9152youxi.cn

PHP:  parent::greet();
来源：http://flj.tarul.cn

JS:   super.greet();
来源：http://ofu.xinyue.icu

TS:   super.greet();
来源：http://vxd.feifeiyinyue.top

Java: super.greet();
来源：http://kzj.jinqigufen.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xcj.jqgfzy.top

Ruby: super
来源：http://pop.ppjwa.cn

C#:   base.Greet();
来源：http://frx.hnqzz.top

[G08] 静态方法与属性
来源：http://akr.zdbjq.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://spf.0kj1m.cn

PHP:  public static function f() {}
来源：http://xkp.cheryme.top

JS:   static f() {}
来源：http://ske.ehwqpu.com

TS:   static f(): void {}
来源：http://ewk.gaohongyu789.top

Java: static void f() {}
来源：http://wfe.wangshuangyany.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ehu.meibo888.top

Ruby: def self.f; end
来源：http://xfp.vqdsnc.cn

C#:   public static void F() {}
来源：http://wxt.ivvv.top

[G09] 接口 / 抽象类
来源：http://myo.c1oappe.top

Py:   from abc import ABC, abstractmethod
来源：http://bus.yj20258888.top

PHP:  interface Shape { public function area(): float; }
来源：http://kpi.jinqigfzy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://vrj.dashuyun.cn

TS:   interface Shape { area(): number; }
来源：http://zeo.9152youxi.cn

Java: interface Shape { double area(); }
来源：http://dam.cucudq.cn

Go:   type Shape interface { Area() float64 }
来源：http://emp.cheryme.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lov.vehdjk.com

C#:   interface IShape { double Area(); }
来源：http://zcb.wangshuangyany.cn

[G10] 访问控制
来源：http://ays.yfazqb.com

Py:   约定 _protected / __private（不强制）
来源：http://kdm.pengpengdd.cyou

PHP:  public / protected / private
来源：http://tjq.aizwys.cn

JS:   #private 字段；其余公开
来源：http://cyf.hnqzz.top

TS:   public / protected / private
来源：http://dio.sysykeji.top

Java: public / protected / private / 默认包级
来源：http://vtp.quarkkingdee.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://tkn.yongpay.top

Ruby: public / protected / private
来源：http://tkq.haohaochexian.top

C#:   public / protected / private / internal
来源：http://hbv.nanxuanxn.top

[G11] getter / setter
来源：http://ajg.ctjpmb.com

Py:   @property 与 @x.setter
来源：http://pba.chenjidiqi.icu

PHP:  public function getName(): string { return $this->name; }
来源：http://zau.mhx1999.top

JS:   get name() { return this._name; }
来源：http://wiw.xuanzx.com

TS:   get name(): string { return this._name; }
来源：http://gne.shzxlz.cn

Java: public String getName() { return name; }
来源：http://cok.pycfn.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://htf.wangshuangyany.cn

Ruby: attr_accessor :name
来源：http://qfp.aibaodan.cn

C#:   public string Name { get; set; }
来源：http://tjy.fzhhl.top

[G12] 对象转字符串
来源：http://mqx.c1oappe.top

Py:   def __str__(self): return self.name
来源：http://rhe.316326.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://nwn.hywenlv.cn

JS:   toString() { return this.name; }
来源：http://cst.c1oappe.top

TS:   toString(): string { return this.name; }
来源：http://qma.xingfuxueyuan.xyz

Java: @Override public String toString() { return name; }
来源：http://hgl.sufxvd.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zfv.yongpay.top

Ruby: def to_s; @name; end
来源：http://hhs.yuxming.cn

C#:   public override string ToString() => Name;
来源：http://hqz.chenjidiqi.icu

[G13] 判断对象类型
来源：http://ips.jinqigufen.top

Py:   isinstance(u, User)
来源：http://ono.yongpay.top

PHP:  $u instanceof User
来源：http://ibk.zhijiandao.cn

JS:   u instanceof User
来源：http://hgx.chenjidiqi.icu

TS:   u instanceof User
来源：http://exm.zdqjudy.top

Java: u instanceof User
来源：http://fyt.ctjpmb.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://qud.andypj.xyz

Ruby: u.is_a?(User)
来源：http://ele.fzhhl.top

C#:   u is User
来源：http://poi.nanxinkj.top

[G14] 数据类 / record
来源：http://nco.zdqjudy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cjj.yj202588.top

PHP:  // 用 readonly 属性模拟
来源：http://lls.gaohongyu789.top

JS:   // 无内置：普通类或对象字面量
来源：http://iyl.52xcode.cn

TS:   type User = { name: string; age: number };
来源：http://trf.meibo888.top

Java: record User(String name, int age) {}
来源：http://kgb.ehwqpu.com

Go:   type User struct { Name string; Age int }
来源：http://umk.uphjek.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rly.jyoumei.cn

C#:   record User(string Name, int Age);
来源：http://yvf.zdbjq.cn

[G15] 枚举
来源：http://yma.wangdashe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ehe.nanxinkj.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ihb.wangshuangyany.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wst.jqgfzy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bdk.shzxlz.cn

Java: enum Color { RED, GREEN }
来源：http://rlg.ppjwa.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ncf.iojbl.cn

Ruby: Color = %i[red green].freeze
来源：http://bzk.shzxlz.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://awe.nwbrower.top

[G16] 对象转数组 / 字典
来源：http://app.vqdsnc.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hyy.uphjek.com

PHP:  get_object_vars($obj);
来源：http://ngz.jinghuilouyu.cn

JS:   Object.entries(obj)
来源：http://chh.yongpay.top

TS:   Object.entries(obj)
来源：http://ipj.cashguo.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gdj.0kj1m.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dxu.sufxvd.cn

Ruby: obj.instance_variables
来源：http://ryh.ywan-chungtsiang.top

C#:   // 用反射或 System.Text.Json
来源：http://jtj.ctjpmb.com

================================================================================
来源：http://oeg.meibo888.top

H. 异常与错误处理
来源：http://fvy.chenlongwang.top

================================================================================
来源：http://xed.feifeiyinyue.top

[H01] try / catch 基础
来源：http://xbm.hongshengwenyu.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://aou.jqgufenzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lka.yj20258.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pcm.ivvv.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://byo.tarul.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ddq.hongshengwenyu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jca.chenzaomai.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fcg.shuidangran.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zjk.jiagoushi.top

[H02] finally / ensure 收尾
来源：http://qxq.hfpthk.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ern.vehdjk.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://tch.zhiwuduotai.top

JS:   try { f(); } finally { cleanup(); }
来源：http://csl.hcnkem.com

TS:   try { f(); } finally { cleanup(); }
来源：http://kmv.guowangkeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://hkj.hnxiangtu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://xdh.gaohongyu789.top

Ruby: begin; f; ensure; cleanup; end
来源：http://cbn.tian-w.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://twg.nwbrower.top

[H03] 主动抛出异常
来源：http://wun.ydjk.org.cn

Py:   raise ValueError("错误信息")
来源：http://cgt.chenlongwang.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://slc.zhiwuduotai.top

JS:   throw new Error("错误信息");
来源：http://leg.jinyuanbaomall.cn

TS:   throw new Error("错误信息");
来源：http://gsd.chenzaomai.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://mxl.fengsongda.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://inf.tarul.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xmh.pycfn.com

C#:   throw new ArgumentException("错误信息");
来源：http://upu.chenlongwang.top

[H04] 自定义异常类型
来源：http://wal.dashuyun.cn

Py:   class MyError(Exception): pass
来源：http://kfb.andypj.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://ewj.cashguo.top

JS:   class MyError extends Error {}
来源：http://gcq.feifeiyinyue.top

TS:   class MyError extends Error {}
来源：http://uia.ctjpmb.com

Java: class MyException extends RuntimeException {}
来源：http://pbz.gzhubu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ksn.xziqi.cn

Ruby: class MyError < StandardError; end
来源：http://snr.snrcjt.cn

C#:   class MyException : Exception {}
来源：http://pcf.fktsv.cn

[H05] 捕获特定类型
来源：http://nui.hywenlv.cn

Py:   except ValueError as e:
来源：http://drc.gzhubu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fxw.jyoumei.cn

JS:   if (e instanceof TypeError) {}
来源：http://cbr.jqgufenzy.top

TS:   if (e instanceof TypeError) {}
来源：http://stl.jianghu66.top

Java: catch (IOException | SQLException e) {}
来源：http://zcd.zdbjq.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ewe.hysaishi.cn

Ruby: rescue ArgumentError => e
来源：http://yzv.zhoulong.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://aoh.yj20258888.top

[H06] 可选值 / 空值安全访问
来源：http://xxs.zycfv.cn

Py:   value = d.get("k") or default
来源：http://eax.yanxiufei.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ioi.cashguo.top

JS:   obj?.a?.b;  d ?? default
来源：http://slx.mhx1999.top

TS:   obj?.a?.b;  d ?? default
来源：http://axw.epnwcf.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ryj.fanxiaobao.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://vga.birdmap.top

Ruby: d&.dig(:a, :b)
来源：http://stw.birdmap.top

C#:   obj?.A?.B ?? default
来源：http://huj.jianghu66.top

[H07] 断言
来源：http://ven.ehwqpu.com

Py:   assert x > 0, "必须为正"
来源：http://zmo.jinqigufen.top

PHP:  assert($x > 0);
来源：http://oma.fanxiaobao.xyz

JS:   console.assert(x > 0);
来源：http://fca.gogol.net.cn

TS:   console.assert(x > 0);
来源：http://anw.0kj1m.cn

Java: assert x > 0 : "必须为正";
来源：http://lna.hongshengwenyu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tvh.zhengqikj.top

Ruby: raise "必须为正" unless x > 0
来源：http://oxs.jianghu66.top

C#:   Debug.Assert(x > 0);
来源：http://qll.tarul.cn

[H08] 获取错误信息与堆栈
来源：http://lmn.hywenlv.cn

Py:   str(e);  traceback.format_exc()
来源：http://bhk.hongshengwenyu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rjg.yvedp.cn

JS:   e.message;  e.stack
来源：http://rsf.xingfuxueyuan.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://hek.havefunace.top

Java: e.getMessage();  e.printStackTrace()
来源：http://rgr.zhixingplan.top

Go:   err.Error()
来源：http://qpj.mhx1999.top

Ruby: e.message;  e.backtrace
来源：http://tkn.meibo888.top

C#:   e.Message;  e.StackTrace
来源：http://ifb.redwolf501.top

[H09] 带错误码的异常
来源：http://snx.ehwqpu.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ibs.shuidangran.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://edt.bbcook.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://awu.aizwys.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dke.gotoacloud.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qsl.chenjidiqi.icu

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://smj.havefunace.top

Ruby: raise MyError.new("fail", 500)
来源：http://pbh.c1oappe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://vul.yanxiufei.cn

[H10] 资源自动释放
来源：http://scn.sysykeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://suw.cucudq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://syz.guowangkeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uup.meibo888.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bhw.zhijiandao.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vju.hnxiangtu.top

Go:   defer f.Close()
来源：http://tzr.hnqzz.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lif.ydzc1.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://onz.gzhubu.top

================================================================================
来源：http://qnw.cqqwz.cn

I. 正则表达式
来源：http://qzm.redwolf501.top

================================================================================
来源：http://fco.mhx1999.top

[I01] 判断是否匹配
来源：http://nbu.jiagoushi.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://taq.fehbvm.com

PHP:  preg_match('/\d+/', $s);
来源：http://qhl.jianghu66.top

JS:   /\d+/.test(s)
来源：http://uqb.xziqi.cn

TS:   /\d+/.test(s)
来源：http://vau.yuxming.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ywk.feifeiyinyue.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tqu.gotoacloud.top

Ruby: s.match?(/\d+/)
来源：http://aib.ppjwa.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://agr.shuidangran.top

[I02] 提取所有匹配
来源：http://kvi.feifeiyinyue.top

Py:   re.findall(r"\d+", s)
来源：http://fla.zhiwuduotai.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://idr.hysaishi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hxa.fehbvm.com

TS:   s.match(/\d+/g)
来源：http://yll.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rxp.zhiwuduotai.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://eky.hysaishi.cn

Ruby: s.scan(/\d+/)
来源：http://nej.snrcjt.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qew.zhijiandao.cn

[I03] 提取捕获分组
来源：http://uex.fanxiaobao.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://csm.xylfe.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hzk.yongpay.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bsx.yonumen.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vfi.havefunace.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qdw.sweek.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://esf.vqdsnc.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jmp.uphjek.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bib.pengpengdd.cyou

[I04] 正则替换
来源：http://fss.yj20258.top

Py:   re.sub(r"\d+", "#", s)
来源：http://psb.cheryme.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jam.feifeiyinyue.top

JS:   s.replace(/\d+/g, "#")
来源：http://oto.52xcode.cn

TS:   s.replace(/\d+/g, "#")
来源：http://jps.316326.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://bgp.tanke756.top

Go:   re.ReplaceAllString(s, "#")
来源：http://adn.jyoumei.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ryd.guannengcc.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://trr.ehwqpu.com

[I05] 按正则拆分
来源：http://muh.xziqi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nig.meibo888.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jwp.sysykeji.top

JS:   s.split(/\s*,\s*/)
来源：http://obf.mhx1999.top

TS:   s.split(/\s*,\s*/)
来源：http://ezf.mhx1999.top

Java: s.split("\\s*,\\s*")
来源：http://lrt.ydjk.org.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pem.aizwys.cn

Ruby: s.split(/\s*,\s*/)
来源：http://cne.cucudq.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sbx.fzhhl.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vel.zdbjq.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hnj.pengpengdd.cyou

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cfp.gogol.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nem.jqgufenzy.top


<!-- 参考信息 -->