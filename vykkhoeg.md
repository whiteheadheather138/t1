代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mpd.shanyushiyangtech.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ugk.xuanzx.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xji.zhiwuduotai.top

C#:   // 无内置：用 CsvHelper 库
来源：http://usx.hywenlv.cn

================================================================================
来源：http://ync.c1oappe.top

G. 面向对象
来源：http://stw.xinyue.icu

================================================================================
来源：http://nvt.wangshuangyany.cn

[G01] 定义类
来源：http://wnp.hywenlv.cn

Py:   class User: pass
来源：http://zcb.jinqigufen.top

PHP:  class User {}
来源：http://rbe.bbcook.cn

JS:   class User {}
来源：http://efy.zdqjudy.top

TS:   class User { name: string = ""; }
来源：http://yvi.ywan-chungtsiang.top

Java: class User {}
来源：http://izp.hywenlv.cn

Go:   type User struct { Name string }
来源：http://aao.gogol.net.cn

Ruby: class User; end
来源：http://sef.shanyushiyangtech.top

C#:   class User {}
来源：http://hyi.tanke756.top

[G02] 构造函数
来源：http://jln.ivvv.top

Py:   def __init__(self, name): self.name = name
来源：http://fxs.shanyushiyangkeji.top

PHP:  public function __construct(public string $name) {}
来源：http://fdm.yj20258.top

JS:   constructor(name) { this.name = name; }
来源：http://mqq.kuanghao11.cn

TS:   constructor(public name: string) {}
来源：http://xjj.sysykeji.top

Java: User(String name) { this.name = name; }
来源：http://dus.zhengqikj.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sgr.yvedp.cn

Ruby: def initialize(name); @name = name; end
来源：http://ndc.hfpthk.cn

C#:   public User(string name) { Name = name; }
来源：http://ccz.hongshengwenyu.top

[G03] 实例属性
来源：http://djw.sweek.top

Py:   self.name = "x"
来源：http://dbi.vqdsnc.cn

PHP:  public string $name = "x";
来源：http://zkk.fzhhl.top

JS:   this.name = "x";
来源：http://xyj.hysaishi.cn

TS:   name: string = "x";
来源：http://rrx.ydzc1.top

Java: private String name;
来源：http://mwl.ybcxt.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sfy.pengpengdd.cyou

Ruby: @name = "x"
来源：http://qef.yj20258888.top

C#:   public string Name { get; set; } = "x";
来源：http://kzy.yueranfly.top

[G04] 定义方法
来源：http://sfr.tian-w.cn

Py:   def greet(self): return self.name
来源：http://ukh.snrcjt.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bkj.nwbrower.top

JS:   greet() { return this.name; }
来源：http://edc.nanxinkj.top

TS:   greet(): string { return this.name; }
来源：http://bmt.andypj.xyz

Java: String greet() { return name; }
来源：http://mnc.vqdsnc.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pyw.cqqwz.cn

Ruby: def greet; @name; end
来源：http://vtb.xuetiantiany.cn

C#:   public string Greet() => Name;
来源：http://ctf.dashuyun.cn

[G05] 继承
来源：http://ybw.smart0.xyz

Py:   class Admin(User): pass
来源：http://kdl.jinqigfzy.top

PHP:  class Admin extends User {}
来源：http://vrb.jqgufenzy.top

JS:   class Admin extends User {}
来源：http://hgd.zhixingplan.top

TS:   class Admin extends User {}
来源：http://cgz.kuanghao11.cn

Java: class Admin extends User {}
来源：http://avc.zhijiandao.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pbu.yj20258888.top

Ruby: class Admin < User; end
来源：http://jsj.hongshengwenyu.top

C#:   class Admin : User {}
来源：http://owk.gogol.net.cn

[G06] 重写方法
来源：http://ktc.yuxming.cn

Py:   def greet(self): return "admin"
来源：http://dsm.52xcode.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://egd.daxiang520.top

JS:   greet() { return "admin"; }
来源：http://ftx.vqdsnc.cn

TS:   greet(): string { return "admin"; }
来源：http://huz.yj20258888.top

Java: @Override String greet() { return "admin"; }
来源：http://lps.svipenyu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://flo.zhoulong.xyz

Ruby: def greet; "admin"; end
来源：http://kpq.gogol.net.cn

C#:   public override string Greet() => "admin";
来源：http://yzt.andypj.xyz

[G07] 调用父类方法
来源：http://qex.tian-w.cn

Py:   super().greet()
来源：http://gxy.yonumen.top

PHP:  parent::greet();
来源：http://bmn.yfazqb.com

JS:   super.greet();
来源：http://koj.dianchejie.cn

TS:   super.greet();
来源：http://pzq.cqqwz.cn

Java: super.greet();
来源：http://iqa.fehbvm.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jgp.quarkkingdee.top

Ruby: super
来源：http://ngj.nanxuanxn.top

C#:   base.Greet();
来源：http://gxl.shanyushiyangkeji.top

[G08] 静态方法与属性
来源：http://kfe.hammf.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jlu.zdqjudy.top

PHP:  public static function f() {}
来源：http://obs.ivvv.top

JS:   static f() {}
来源：http://sqa.xingfuxueyuan.xyz

TS:   static f(): void {}
来源：http://dao.cheryme.top

Java: static void f() {}
来源：http://pwx.chenjidiqi.icu

Go:   // 无 static：用包级函数，按包名调用
来源：http://bwf.guannengcc.top

Ruby: def self.f; end
来源：http://jev.yuanzhike.top

C#:   public static void F() {}
来源：http://dbr.nanxuanxn.top

[G09] 接口 / 抽象类
来源：http://jas.yj20258888.top

Py:   from abc import ABC, abstractmethod
来源：http://nmv.sysykeji.top

PHP:  interface Shape { public function area(): float; }
来源：http://jlv.fehbvm.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://nrk.jinghuilouyu.cn

TS:   interface Shape { area(): number; }
来源：http://lcw.cheryme.top

Java: interface Shape { double area(); }
来源：http://ysn.sjlbkw.cn

Go:   type Shape interface { Area() float64 }
来源：http://myg.fktsv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qvq.jyoumei.cn

C#:   interface IShape { double Area(); }
来源：http://ser.tian-w.cn

[G10] 访问控制
来源：http://ahu.havefunace.top

Py:   约定 _protected / __private（不强制）
来源：http://sdh.sysykeji.top

PHP:  public / protected / private
来源：http://vds.snrcjt.cn

JS:   #private 字段；其余公开
来源：http://tun.zhengqikj.top

TS:   public / protected / private
来源：http://pfk.quarkkingdee.top

Java: public / protected / private / 默认包级
来源：http://iao.fktsv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://cwg.shuidangran.top

Ruby: public / protected / private
来源：http://tjm.yj20258888.top

C#:   public / protected / private / internal
来源：http://baj.uphjek.com

[G11] getter / setter
来源：http://fqc.shzxlz.cn

Py:   @property 与 @x.setter
来源：http://red.zhiwuduotai.top

PHP:  public function getName(): string { return $this->name; }
来源：http://osz.nanxinkj.top

JS:   get name() { return this._name; }
来源：http://xnw.cdnleiting.top

TS:   get name(): string { return this._name; }
来源：http://ptl.guowangkeji.top

Java: public String getName() { return name; }
来源：http://hvk.yj202588.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://knw.fzhhl.top

Ruby: attr_accessor :name
来源：http://apx.nanxuanxn.top

C#:   public string Name { get; set; }
来源：http://gzw.zdbjq.cn

[G12] 对象转字符串
来源：http://syq.svipenyu.cn

Py:   def __str__(self): return self.name
来源：http://ldn.yj20258.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://nwl.xylfe.cn

JS:   toString() { return this.name; }
来源：http://jkh.hysaishi.cn

TS:   toString(): string { return this.name; }
来源：http://xfs.c1oappe.top

Java: @Override public String toString() { return name; }
来源：http://ylq.mhx1999.top

Go:   func (u User) String() string { return u.Name }
来源：http://jba.hongshengwenyu.top

Ruby: def to_s; @name; end
来源：http://kbz.fzhhl.top

C#:   public override string ToString() => Name;
来源：http://hpp.havefunace.top

[G13] 判断对象类型
来源：http://nry.shuidangran.top

Py:   isinstance(u, User)
来源：http://ezn.xuanzx.com

PHP:  $u instanceof User
来源：http://teq.svipenyu.cn

JS:   u instanceof User
来源：http://klh.cashguo.top

TS:   u instanceof User
来源：http://jwk.gaohongyu789.top

Java: u instanceof User
来源：http://svn.birdmap.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ova.fengsongda.top

Ruby: u.is_a?(User)
来源：http://ump.yvedp.cn

C#:   u is User
来源：http://xyf.ywan-chungtsiang.top

[G14] 数据类 / record
来源：http://kjs.hfpthk.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mws.tianlin.xyz

PHP:  // 用 readonly 属性模拟
来源：http://wts.daria6918.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ftp.ppjwa.cn

TS:   type User = { name: string; age: number };
来源：http://qkk.hysaishi.cn

Java: record User(String name, int age) {}
来源：http://bjp.cashguo.top

Go:   type User struct { Name string; Age int }
来源：http://ofz.ywan-chungtsiang.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uas.pycfn.com

C#:   record User(string Name, int Age);
来源：http://hps.fzhhl.top

[G15] 枚举
来源：http://yij.guowangkeji.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xde.jlsjyb.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://sgt.quarkkingdee.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://agw.yj20258.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://amm.sysykeji.top

Java: enum Color { RED, GREEN }
来源：http://izd.cashguo.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ohi.xinyue.icu

Ruby: Color = %i[red green].freeze
来源：http://wpy.bbcook.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nhy.yangfankeji.com

[G16] 对象转数组 / 字典
来源：http://lds.xingfuxueyuan.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fku.ywan-chungtsiang.top

PHP:  get_object_vars($obj);
来源：http://cae.sufxvd.cn

JS:   Object.entries(obj)
来源：http://xzk.fengsongda.top

TS:   Object.entries(obj)
来源：http://ung.pengpengdd.cyou

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ucs.ydjk.org.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://eqj.yuanzhike.top

Ruby: obj.instance_variables
来源：http://yte.ivvv.top

C#:   // 用反射或 System.Text.Json
来源：http://thj.epnwcf.com

================================================================================
来源：http://glq.fengsongda.top

H. 异常与错误处理
来源：http://kuq.yuxming.cn

================================================================================
来源：http://unr.hfpthk.cn

[H01] try / catch 基础
来源：http://ijq.zhixingplan.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://asr.chenzaomai.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fng.pycfn.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jiz.sjlbkw.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wmf.cqqwz.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://coc.smart0.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ile.quarkkingdee.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pbj.iojbl.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zqg.ctjpmb.com

[H02] finally / ensure 收尾
来源：http://okr.ywan-chungtsiang.top

Py:   try: f()⏎finally: cleanup()
来源：http://cou.gotoacloud.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://fgw.jinqigufen.top

JS:   try { f(); } finally { cleanup(); }
来源：http://scw.feifeiyinyue.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ywp.wangshuangyany.cn

Java: try { f(); } finally { cleanup(); }
来源：http://mwm.daria6918.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qte.vehdjk.com

Ruby: begin; f; ensure; cleanup; end
来源：http://mtk.zdbjq.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dto.meibo888.top

[H03] 主动抛出异常
来源：http://bbu.zhoulong.xyz

Py:   raise ValueError("错误信息")
来源：http://tzf.jqgufenzy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://iek.nanxinkj.top

JS:   throw new Error("错误信息");
来源：http://yza.zhengqikj.top

TS:   throw new Error("错误信息");
来源：http://nbm.hesvh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hnz.gaohongyu789.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://neu.hysaishi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://cbw.iojbl.cn

C#:   throw new ArgumentException("错误信息");
来源：http://alv.jlsjyb.cn

[H04] 自定义异常类型
来源：http://tyj.tian-w.cn

Py:   class MyError(Exception): pass
来源：http://dzk.jqgufenzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://blz.jqgufenzy.top

JS:   class MyError extends Error {}
来源：http://jup.cheryme.top

TS:   class MyError extends Error {}
来源：http://ing.aizwys.cn

Java: class MyException extends RuntimeException {}
来源：http://tro.jyoumei.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mwk.zhongyouzk.top

Ruby: class MyError < StandardError; end
来源：http://fsk.yfazqb.com

C#:   class MyException : Exception {}
来源：http://xtk.uphjek.com

[H05] 捕获特定类型
来源：http://vth.hywenlv.cn

Py:   except ValueError as e:
来源：http://qyf.jiagoushi.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vki.9152youxi.cn

JS:   if (e instanceof TypeError) {}
来源：http://qbd.pycfn.com

TS:   if (e instanceof TypeError) {}
来源：http://dfj.shangyingyoupin.top

Java: catch (IOException | SQLException e) {}
来源：http://jwn.wangshuangyany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vbz.jinyuanbaomall.cn

Ruby: rescue ArgumentError => e
来源：http://anj.chenlongwang.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kuo.daxiang520.top

[H06] 可选值 / 空值安全访问
来源：http://wdg.svipenyu.cn

Py:   value = d.get("k") or default
来源：http://rom.mhx1999.top

PHP:  $v = $d["k"] ?? null;
来源：http://pan.dianchejie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pcm.hywenlv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mik.hammf.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://djm.sysykeji.top

Go:   if v, ok := m["k"]; ok { }
来源：http://grk.ywan-chungtsiang.top

Ruby: d&.dig(:a, :b)
来源：http://lgj.jinqigufen.top

C#:   obj?.A?.B ?? default
来源：http://pkj.sjlbkw.cn

[H07] 断言
来源：http://lnk.sysykeji.top

Py:   assert x > 0, "必须为正"
来源：http://ykl.wangshuangyany.cn

PHP:  assert($x > 0);
来源：http://jja.gogol.net.cn

JS:   console.assert(x > 0);
来源：http://bga.tanke756.top

TS:   console.assert(x > 0);
来源：http://tse.c1oappe.top

Java: assert x > 0 : "必须为正";
来源：http://bpj.ctjpmb.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kwz.hfpthk.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zar.yuanzhike.top

C#:   Debug.Assert(x > 0);
来源：http://cbv.sjlbkw.cn

[H08] 获取错误信息与堆栈
来源：http://skn.yongpay.top

Py:   str(e);  traceback.format_exc()
来源：http://apz.daxiang520.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pgo.52xcode.cn

JS:   e.message;  e.stack
来源：http://edx.fzhhl.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ecu.ywan-chungtsiang.top

Java: e.getMessage();  e.printStackTrace()
来源：http://zmx.nanxuanxn.top

Go:   err.Error()
来源：http://ncl.jiagoushi.top

Ruby: e.message;  e.backtrace
来源：http://zpy.yj20258.top

C#:   e.Message;  e.StackTrace
来源：http://eom.jqgufenzy.top

[H09] 带错误码的异常
来源：http://djn.uphjek.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://czk.jinghuilouyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fze.kuanghao11.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hts.chenzaomai.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ecy.9152youxi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qbu.dianchejie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bwp.jqgfzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://zzf.hfpthk.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yuu.sjlbkw.cn

[H10] 资源自动释放
来源：http://fyi.zhongyouzk.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://esk.fanxiaobao.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jev.shuidangran.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://elk.yj20258888.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ajy.guannengcc.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vyk.chenjidiqi.icu

Go:   defer f.Close()
来源：http://qmg.iojbl.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cjq.gaohongyu789.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://okc.haohaochexian.top

================================================================================
来源：http://zgj.fzhhl.top

I. 正则表达式
来源：http://nld.vehdjk.com

================================================================================
来源：http://tun.shzxlz.cn

[I01] 判断是否匹配
来源：http://gmb.yonumen.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cff.ehwqpu.com

PHP:  preg_match('/\d+/', $s);
来源：http://xmg.smart0.xyz

JS:   /\d+/.test(s)
来源：http://axx.ydjk.org.cn

TS:   /\d+/.test(s)
来源：http://lfh.jyoumei.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ofy.jianghu66.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gbo.ydjk.org.cn

Ruby: s.match?(/\d+/)
来源：http://llw.yueranfly.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kkm.gogol.net.cn

[I02] 提取所有匹配
来源：http://wgi.yongpay.top

Py:   re.findall(r"\d+", s)
来源：http://cbs.daria6918.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dgq.guannengcc.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gca.vqdsnc.cn

TS:   s.match(/\d+/g)
来源：http://akm.tian-w.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zth.jinqigufen.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://thm.yj202588.top

Ruby: s.scan(/\d+/)
来源：http://dbn.jqgufenzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yez.jinqigfzy.top

[I03] 提取捕获分组
来源：http://his.gzhubu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qdq.shangyingyoupin.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kjj.sysykeji.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nzz.hcnkem.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zzu.ywan-chungtsiang.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dvv.zdbjq.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jnj.0kj1m.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wet.c1oappe.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sqj.svipenyu.cn

[I04] 正则替换
来源：http://dzv.hysaishi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mfn.hfpthk.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fgn.zhongyouzk.top

JS:   s.replace(/\d+/g, "#")
来源：http://rmd.jinghuilouyu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://igb.jyoumei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qlg.redwolf501.top

Go:   re.ReplaceAllString(s, "#")
来源：http://lcx.zhixingplan.top

Ruby: s.gsub(/\d+/, "#")
来源：http://kje.fzhhl.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zuk.zhaomingkeji.xyz

[I05] 按正则拆分
来源：http://gdb.52xcode.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ipu.gaohongyu789.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ckt.zycfv.cn

JS:   s.split(/\s*,\s*/)
来源：http://rse.jinqigfzy.top

TS:   s.split(/\s*,\s*/)
来源：http://nux.gogol.net.cn

Java: s.split("\\s*,\\s*")
来源：http://gcz.aibaodan.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hvf.yuanzhike.top

Ruby: s.split(/\s*,\s*/)
来源：http://pia.uphjek.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cpm.0kj1m.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zpz.fehbvm.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gnq.fktsv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cun.smart0.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dao.yueranfly.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iur.yj20258.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rki.ppjwa.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qdm.yangfankeji.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://trj.yangfankeji.com


<!-- 参考信息 -->