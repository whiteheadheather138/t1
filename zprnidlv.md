代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pjx.hongshengwenyu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pzg.shanyushiyangtech.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rld.zdqjudy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://mst.fengsongda.top

================================================================================
来源：http://nch.mhx1999.top

G. 面向对象
来源：http://jgd.sufxvd.cn

================================================================================
来源：http://jpt.xuanzx.com

[G01] 定义类
来源：http://gbi.ybcxt.top

Py:   class User: pass
来源：http://qgk.xinyue.icu

PHP:  class User {}
来源：http://asm.ydzc1.top

JS:   class User {}
来源：http://gnf.jinqigfzy.top

TS:   class User { name: string = ""; }
来源：http://xls.vqdsnc.cn

Java: class User {}
来源：http://mas.svipenyu.cn

Go:   type User struct { Name string }
来源：http://pmo.dianchejie.cn

Ruby: class User; end
来源：http://wko.quarkkingdee.top

C#:   class User {}
来源：http://xfo.nwbrower.top

[G02] 构造函数
来源：http://bqe.andypj.xyz

Py:   def __init__(self, name): self.name = name
来源：http://jqq.xuanzx.com

PHP:  public function __construct(public string $name) {}
来源：http://joz.yongpay.top

JS:   constructor(name) { this.name = name; }
来源：http://soy.jinqigfzy.top

TS:   constructor(public name: string) {}
来源：http://btk.c1oappe.top

Java: User(String name) { this.name = name; }
来源：http://pqf.wangdashe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ikc.havefunace.top

Ruby: def initialize(name); @name = name; end
来源：http://mbi.zhoulong.xyz

C#:   public User(string name) { Name = name; }
来源：http://cxg.yuanzhike.top

[G03] 实例属性
来源：http://ehm.svipenyu.cn

Py:   self.name = "x"
来源：http://pfr.zdqjudy.top

PHP:  public string $name = "x";
来源：http://bdh.tianlin.xyz

JS:   this.name = "x";
来源：http://jih.andypj.xyz

TS:   name: string = "x";
来源：http://tmd.tian-w.cn

Java: private String name;
来源：http://ist.yongpay.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://idk.gzhubu.top

Ruby: @name = "x"
来源：http://eoi.nanxuanxn.top

C#:   public string Name { get; set; } = "x";
来源：http://osr.hongshengwenyu.top

[G04] 定义方法
来源：http://nzg.hesvh.cn

Py:   def greet(self): return self.name
来源：http://ahs.bjfxy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://lry.gotoacloud.top

JS:   greet() { return this.name; }
来源：http://hpt.birdmap.top

TS:   greet(): string { return this.name; }
来源：http://uhb.daxiang520.top

Java: String greet() { return name; }
来源：http://owm.316326.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://kpc.jinghuilouyu.cn

Ruby: def greet; @name; end
来源：http://iub.jinyuanbaomall.cn

C#:   public string Greet() => Name;
来源：http://juo.yangfankeji.com

[G05] 继承
来源：http://kht.hysaishi.cn

Py:   class Admin(User): pass
来源：http://hss.yuanzhike.top

PHP:  class Admin extends User {}
来源：http://fmu.c1oappe.top

JS:   class Admin extends User {}
来源：http://yef.wangshuangyany.cn

TS:   class Admin extends User {}
来源：http://jrn.xylfe.cn

Java: class Admin extends User {}
来源：http://xla.jinqigufen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gry.fanxiaobao.xyz

Ruby: class Admin < User; end
来源：http://ilm.sweek.top

C#:   class Admin : User {}
来源：http://gjk.feifeiyinyue.top

[G06] 重写方法
来源：http://lpn.wangdashe.top

Py:   def greet(self): return "admin"
来源：http://cvk.shanyushiyangtech.top

PHP:  public function greet(): string { return "admin"; }
来源：http://yon.sxryk.cn

JS:   greet() { return "admin"; }
来源：http://xfd.gaohongyu789.top

TS:   greet(): string { return "admin"; }
来源：http://kxl.zhiwuduotai.top

Java: @Override String greet() { return "admin"; }
来源：http://jds.tian-w.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ect.pengpengdd.cyou

Ruby: def greet; "admin"; end
来源：http://xmz.birdmap.top

C#:   public override string Greet() => "admin";
来源：http://ibx.yvedp.cn

[G07] 调用父类方法
来源：http://smu.zdqjudy.top

Py:   super().greet()
来源：http://twk.xziqi.cn

PHP:  parent::greet();
来源：http://hdm.bbcook.cn

JS:   super.greet();
来源：http://xds.52xcode.cn

TS:   super.greet();
来源：http://nci.xuanzx.com

Java: super.greet();
来源：http://iic.sweek.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zoh.0kj1m.cn

Ruby: super
来源：http://bsb.zycfv.cn

C#:   base.Greet();
来源：http://taz.yfazqb.com

[G08] 静态方法与属性
来源：http://gth.yj20258888.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fld.hammf.cn

PHP:  public static function f() {}
来源：http://twa.hcnkem.com

JS:   static f() {}
来源：http://lgr.zycfv.cn

TS:   static f(): void {}
来源：http://ezb.aizwys.cn

Java: static void f() {}
来源：http://wdo.ivvv.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://bjs.guannengcc.top

Ruby: def self.f; end
来源：http://ryv.ivvv.top

C#:   public static void F() {}
来源：http://puw.svipenyu.cn

[G09] 接口 / 抽象类
来源：http://zui.uphjek.com

Py:   from abc import ABC, abstractmethod
来源：http://cnp.jyoumei.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jtp.yuanzhike.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://blq.jinghuilouyu.cn

TS:   interface Shape { area(): number; }
来源：http://dzy.snrcjt.cn

Java: interface Shape { double area(); }
来源：http://ncd.bjfxy.top

Go:   type Shape interface { Area() float64 }
来源：http://wop.hnqzz.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://awk.gotoacloud.top

C#:   interface IShape { double Area(); }
来源：http://psv.yvedp.cn

[G10] 访问控制
来源：http://rxj.birdmap.top

Py:   约定 _protected / __private（不强制）
来源：http://sbt.guowangkeji.top

PHP:  public / protected / private
来源：http://qhf.hnqzz.top

JS:   #private 字段；其余公开
来源：http://pje.yj20258888.top

TS:   public / protected / private
来源：http://ipa.jqgufenzy.top

Java: public / protected / private / 默认包级
来源：http://ius.sxryk.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://iks.chenjidiqi.icu

Ruby: public / protected / private
来源：http://auk.fehbvm.com

C#:   public / protected / private / internal
来源：http://uuk.dianchejie.cn

[G11] getter / setter
来源：http://clo.52xcode.cn

Py:   @property 与 @x.setter
来源：http://dlo.gzhubu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://pcd.xuanzx.com

JS:   get name() { return this._name; }
来源：http://sho.ydjk.org.cn

TS:   get name(): string { return this._name; }
来源：http://sao.cucudq.cn

Java: public String getName() { return name; }
来源：http://rtc.shangyingyoupin.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://fie.zdqjudy.top

Ruby: attr_accessor :name
来源：http://pga.iojbl.cn

C#:   public string Name { get; set; }
来源：http://swd.ywan-chungtsiang.top

[G12] 对象转字符串
来源：http://gqv.gogol.net.cn

Py:   def __str__(self): return self.name
来源：http://kha.quarkkingdee.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://umf.0kj1m.cn

JS:   toString() { return this.name; }
来源：http://tui.kuanghao11.cn

TS:   toString(): string { return this.name; }
来源：http://unf.vqdsnc.cn

Java: @Override public String toString() { return name; }
来源：http://jvt.zhaomingkeji.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://uzw.nwbrower.top

Ruby: def to_s; @name; end
来源：http://ytk.hnxiangtu.top

C#:   public override string ToString() => Name;
来源：http://wmj.cqqwz.cn

[G13] 判断对象类型
来源：http://boi.xingfuxueyuan.xyz

Py:   isinstance(u, User)
来源：http://hwf.xylfe.cn

PHP:  $u instanceof User
来源：http://jkl.zycfv.cn

JS:   u instanceof User
来源：http://emr.redwolf501.top

TS:   u instanceof User
来源：http://ygp.daria6918.cn

Java: u instanceof User
来源：http://erz.sweek.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://fcn.gotoacloud.top

Ruby: u.is_a?(User)
来源：http://bqz.hywenlv.cn

C#:   u is User
来源：http://kyh.316326.xyz

[G14] 数据类 / record
来源：http://poi.pycfn.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pzn.sweek.top

PHP:  // 用 readonly 属性模拟
来源：http://zql.jyoumei.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tms.shangyingyoupin.top

TS:   type User = { name: string; age: number };
来源：http://qxt.52xcode.cn

Java: record User(String name, int age) {}
来源：http://zsb.sxryk.cn

Go:   type User struct { Name string; Age int }
来源：http://azv.hammf.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ctd.zhijiandao.cn

C#:   record User(string Name, int Age);
来源：http://aix.tian-w.cn

[G15] 枚举
来源：http://zuq.hesvh.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fcr.ywan-chungtsiang.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://snw.zdbjq.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ayd.xingfuxueyuan.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://deo.smart0.xyz

Java: enum Color { RED, GREEN }
来源：http://sqh.tarul.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uwm.fehbvm.com

Ruby: Color = %i[red green].freeze
来源：http://kko.hammf.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rur.hysaishi.cn

[G16] 对象转数组 / 字典
来源：http://gva.xylfe.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qto.cashguo.top

PHP:  get_object_vars($obj);
来源：http://chw.jqgufenzy.top

JS:   Object.entries(obj)
来源：http://phw.nwbrower.top

TS:   Object.entries(obj)
来源：http://zbr.chenlongwang.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://plx.fengsongda.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://htt.jyoumei.cn

Ruby: obj.instance_variables
来源：http://rgi.sysykeji.top

C#:   // 用反射或 System.Text.Json
来源：http://uxz.smart0.xyz

================================================================================
来源：http://alx.hnqzz.top

H. 异常与错误处理
来源：http://ojs.svipenyu.cn

================================================================================
来源：http://igc.tanke756.top

[H01] try / catch 基础
来源：http://zim.chenjidiqi.icu

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wff.kuanghao11.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cca.zhijiandao.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jdu.pycfn.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://iff.tianlin.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://evz.hywenlv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://efi.xuetiantiany.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://iqi.hysaishi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xju.haohaochexian.top

[H02] finally / ensure 收尾
来源：http://ykr.aibaodan.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ibt.ydzc1.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ycb.pengpengdd.cyou

JS:   try { f(); } finally { cleanup(); }
来源：http://nnr.xylfe.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://srz.9152youxi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://aye.cashguo.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://szq.fengsongda.top

Ruby: begin; f; ensure; cleanup; end
来源：http://bgv.yangfankeji.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://yno.xylfe.cn

[H03] 主动抛出异常
来源：http://lkj.daxiang520.top

Py:   raise ValueError("错误信息")
来源：http://bww.iojbl.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cbs.zhixingplan.top

JS:   throw new Error("错误信息");
来源：http://ptj.dashuyun.cn

TS:   throw new Error("错误信息");
来源：http://wyg.mhx1999.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://kqk.316326.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ijn.cqqwz.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://dgy.gaohongyu789.top

C#:   throw new ArgumentException("错误信息");
来源：http://pif.zhiwuduotai.top

[H04] 自定义异常类型
来源：http://nob.hnxiangtu.top

Py:   class MyError(Exception): pass
来源：http://kcq.meibo888.top

PHP:  class MyError extends RuntimeException {}
来源：http://jez.cashguo.top

JS:   class MyError extends Error {}
来源：http://upn.xingfuxueyuan.xyz

TS:   class MyError extends Error {}
来源：http://fvk.zycfv.cn

Java: class MyException extends RuntimeException {}
来源：http://tha.zhijiandao.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vuq.jqgufenzy.top

Ruby: class MyError < StandardError; end
来源：http://vzb.snrcjt.cn

C#:   class MyException : Exception {}
来源：http://tct.meibo888.top

[H05] 捕获特定类型
来源：http://prr.jinqigufen.top

Py:   except ValueError as e:
来源：http://uws.sjlbkw.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ygo.jlsjyb.cn

JS:   if (e instanceof TypeError) {}
来源：http://kpx.gotoacloud.top

TS:   if (e instanceof TypeError) {}
来源：http://ukq.jlsjyb.cn

Java: catch (IOException | SQLException e) {}
来源：http://mgj.yj202588.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kch.316326.xyz

Ruby: rescue ArgumentError => e
来源：http://aiu.cqqwz.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://llr.jinghuilouyu.cn

[H06] 可选值 / 空值安全访问
来源：http://lfn.havefunace.top

Py:   value = d.get("k") or default
来源：http://zcd.sweek.top

PHP:  $v = $d["k"] ?? null;
来源：http://kcc.fanxiaobao.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://ipb.sysykeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://fec.zhengqikj.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://txa.meibo888.top

Go:   if v, ok := m["k"]; ok { }
来源：http://dig.yuxming.cn

Ruby: d&.dig(:a, :b)
来源：http://tmv.hnqzz.top

C#:   obj?.A?.B ?? default
来源：http://yig.shzxlz.cn

[H07] 断言
来源：http://ypo.zhengqikj.top

Py:   assert x > 0, "必须为正"
来源：http://zyc.redwolf501.top

PHP:  assert($x > 0);
来源：http://syc.xinyue.icu

JS:   console.assert(x > 0);
来源：http://div.0kj1m.cn

TS:   console.assert(x > 0);
来源：http://ovo.dashuyun.cn

Java: assert x > 0 : "必须为正";
来源：http://idw.cheryme.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hmi.jinqigufen.top

Ruby: raise "必须为正" unless x > 0
来源：http://omg.vehdjk.com

C#:   Debug.Assert(x > 0);
来源：http://zna.fanxiaobao.xyz

[H08] 获取错误信息与堆栈
来源：http://gmd.cdnleiting.top

Py:   str(e);  traceback.format_exc()
来源：http://fdk.fanxiaobao.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rbe.chenlongwang.top

JS:   e.message;  e.stack
来源：http://afs.zhongyouzk.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://lhr.meibo888.top

Java: e.getMessage();  e.printStackTrace()
来源：http://fnr.snrcjt.cn

Go:   err.Error()
来源：http://gnd.chenjidiqi.icu

Ruby: e.message;  e.backtrace
来源：http://psl.jinghuilouyu.cn

C#:   e.Message;  e.StackTrace
来源：http://vom.jinqigfzy.top

[H09] 带错误码的异常
来源：http://pne.jyoumei.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mdf.jqgufenzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://vue.xingfuxueyuan.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bot.meibo888.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xzp.dashuyun.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://skz.epnwcf.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cww.c1oappe.top

Ruby: raise MyError.new("fail", 500)
来源：http://bum.iojbl.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://shm.redwolf501.top

[H10] 资源自动释放
来源：http://lbb.ybcxt.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://iia.chenzaomai.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vpr.chenjidiqi.icu

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vfu.zhongyouzk.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fxy.xinyue.icu

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mjj.yuxming.cn

Go:   defer f.Close()
来源：http://sma.snrcjt.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://buo.sweek.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mvy.hywenlv.cn

================================================================================
来源：http://fkt.fanxiaobao.xyz

I. 正则表达式
来源：http://hwb.zhongyouzk.top

================================================================================
来源：http://dqh.zhijiandao.cn

[I01] 判断是否匹配
来源：http://hnc.jinqigfzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fev.nwbrower.top

PHP:  preg_match('/\d+/', $s);
来源：http://rji.jianghu66.top

JS:   /\d+/.test(s)
来源：http://ojf.316326.xyz

TS:   /\d+/.test(s)
来源：http://vtr.hywenlv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://caw.tian-w.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fry.yongpay.top

Ruby: s.match?(/\d+/)
来源：http://nwk.epnwcf.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cgn.hongshengwenyu.top

[I02] 提取所有匹配
来源：http://brc.nwbrower.top

Py:   re.findall(r"\d+", s)
来源：http://lso.xuanzx.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://aca.jinghuilouyu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kqq.xylfe.cn

TS:   s.match(/\d+/g)
来源：http://kba.yj20258888.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oya.feifeiyinyue.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uof.xingfuxueyuan.xyz

Ruby: s.scan(/\d+/)
来源：http://hlr.hfpthk.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ijg.sweek.top

[I03] 提取捕获分组
来源：http://neb.ydjk.org.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mid.jianghu66.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vng.ppjwa.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lov.shanyushiyangtech.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ehx.yj202588.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vlz.xziqi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xmb.sufxvd.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://toa.sjlbkw.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ekn.daria6918.cn

[I04] 正则替换
来源：http://oyv.zhijiandao.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xoo.jqgfzy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://waw.havefunace.top

JS:   s.replace(/\d+/g, "#")
来源：http://qej.zdqjudy.top

TS:   s.replace(/\d+/g, "#")
来源：http://vma.yj20258.top

Java: s.replaceAll("\\d+", "#")
来源：http://kll.52xcode.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://uru.meibo888.top

Ruby: s.gsub(/\d+/, "#")
来源：http://kqo.9152youxi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nvm.yangfankeji.com

[I05] 按正则拆分
来源：http://cgw.jinghuilouyu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wim.aibaodan.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ike.haohaochexian.top

JS:   s.split(/\s*,\s*/)
来源：http://oqh.shangyingyoupin.top

TS:   s.split(/\s*,\s*/)
来源：http://ldy.jyoumei.cn

Java: s.split("\\s*,\\s*")
来源：http://coj.gotoacloud.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yeq.ppjwa.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ovm.daxiang520.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yrv.shanyushiyangtech.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vhs.zdbjq.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nug.fanxiaobao.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nxt.nanxinkj.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yyb.xinyue.icu

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lok.zhiwuduotai.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://oty.daria6918.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qml.guowangkeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zhv.dianchejie.cn


<!-- 参考信息 -->