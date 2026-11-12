代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://slg.fanxiaobao.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dfq.yueranfly.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nfh.cashguo.top

C#:   // 无内置：用 CsvHelper 库
来源：http://wtx.feifeiyinyue.top

================================================================================
来源：http://wge.9152youxi.cn

G. 面向对象
来源：http://iyp.yfazqb.com

================================================================================
来源：http://dzu.c1oappe.top

[G01] 定义类
来源：http://eav.shanyushiyangkeji.top

Py:   class User: pass
来源：http://akb.tian-w.cn

PHP:  class User {}
来源：http://vwu.redwolf501.top

JS:   class User {}
来源：http://lyr.uphjek.com

TS:   class User { name: string = ""; }
来源：http://zpz.sjlbkw.cn

Java: class User {}
来源：http://lio.jiagoushi.top

Go:   type User struct { Name string }
来源：http://rvd.uphjek.com

Ruby: class User; end
来源：http://dxo.shuidangran.top

C#:   class User {}
来源：http://enf.xinyue.icu

[G02] 构造函数
来源：http://esx.xuanzx.com

Py:   def __init__(self, name): self.name = name
来源：http://ajf.yuxming.cn

PHP:  public function __construct(public string $name) {}
来源：http://loj.ivvv.top

JS:   constructor(name) { this.name = name; }
来源：http://rgz.zhongyouzk.top

TS:   constructor(public name: string) {}
来源：http://hbh.xuetiantiany.cn

Java: User(String name) { this.name = name; }
来源：http://mjh.kuanghao11.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bwc.cdnleiting.top

Ruby: def initialize(name); @name = name; end
来源：http://wyp.dianchejie.cn

C#:   public User(string name) { Name = name; }
来源：http://aos.sufxvd.cn

[G03] 实例属性
来源：http://lhw.0kj1m.cn

Py:   self.name = "x"
来源：http://pnt.chenjidiqi.icu

PHP:  public string $name = "x";
来源：http://ajj.xylfe.cn

JS:   this.name = "x";
来源：http://ygw.sufxvd.cn

TS:   name: string = "x";
来源：http://wxa.wangshuangyany.cn

Java: private String name;
来源：http://fgy.yfazqb.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mpp.hysaishi.cn

Ruby: @name = "x"
来源：http://zzw.yongpay.top

C#:   public string Name { get; set; } = "x";
来源：http://pjc.tarul.cn

[G04] 定义方法
来源：http://ykp.yongpay.top

Py:   def greet(self): return self.name
来源：http://btd.zhaomingkeji.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://kyp.hfpthk.cn

JS:   greet() { return this.name; }
来源：http://zdz.hcnkem.com

TS:   greet(): string { return this.name; }
来源：http://fud.fanxiaobao.xyz

Java: String greet() { return name; }
来源：http://xgp.cashguo.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://wle.xylfe.cn

Ruby: def greet; @name; end
来源：http://iqs.shzxlz.cn

C#:   public string Greet() => Name;
来源：http://bus.cucudq.cn

[G05] 继承
来源：http://jfq.vqdsnc.cn

Py:   class Admin(User): pass
来源：http://vdn.quarkkingdee.top

PHP:  class Admin extends User {}
来源：http://dvh.aizwys.cn

JS:   class Admin extends User {}
来源：http://ynt.jlsjyb.cn

TS:   class Admin extends User {}
来源：http://xlu.chenlongwang.top

Java: class Admin extends User {}
来源：http://gqr.dashuyun.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://txt.chenlongwang.top

Ruby: class Admin < User; end
来源：http://lti.fktsv.cn

C#:   class Admin : User {}
来源：http://iez.fanxiaobao.xyz

[G06] 重写方法
来源：http://siy.ehwqpu.com

Py:   def greet(self): return "admin"
来源：http://iyx.guannengcc.top

PHP:  public function greet(): string { return "admin"; }
来源：http://kqn.xingfuxueyuan.xyz

JS:   greet() { return "admin"; }
来源：http://com.nwbrower.top

TS:   greet(): string { return "admin"; }
来源：http://tou.aibaodan.cn

Java: @Override String greet() { return "admin"; }
来源：http://tvg.daxiang520.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hbe.fengsongda.top

Ruby: def greet; "admin"; end
来源：http://xke.jinghuilouyu.cn

C#:   public override string Greet() => "admin";
来源：http://ucr.sjlbkw.cn

[G07] 调用父类方法
来源：http://vzt.yongpay.top

Py:   super().greet()
来源：http://roc.jlsjyb.cn

PHP:  parent::greet();
来源：http://owk.cdnleiting.top

JS:   super.greet();
来源：http://iol.zycfv.cn

TS:   super.greet();
来源：http://vnv.9152youxi.cn

Java: super.greet();
来源：http://tzi.hnxiangtu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ika.cqqwz.cn

Ruby: super
来源：http://iiu.xuetiantiany.cn

C#:   base.Greet();
来源：http://poq.zhaomingkeji.xyz

[G08] 静态方法与属性
来源：http://nsd.nwbrower.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vei.xuetiantiany.cn

PHP:  public static function f() {}
来源：http://pkf.xuanzx.com

JS:   static f() {}
来源：http://qdv.sjlbkw.cn

TS:   static f(): void {}
来源：http://vjs.kuanghao11.cn

Java: static void f() {}
来源：http://aib.chenjidiqi.icu

Go:   // 无 static：用包级函数，按包名调用
来源：http://jho.andypj.xyz

Ruby: def self.f; end
来源：http://oia.uphjek.com

C#:   public static void F() {}
来源：http://xve.daria6918.cn

[G09] 接口 / 抽象类
来源：http://wvs.iojbl.cn

Py:   from abc import ABC, abstractmethod
来源：http://tyx.smart0.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://qpm.sweek.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://jff.yangfankeji.com

TS:   interface Shape { area(): number; }
来源：http://oci.hysaishi.cn

Java: interface Shape { double area(); }
来源：http://idb.yuanzhike.top

Go:   type Shape interface { Area() float64 }
来源：http://ywi.cqqwz.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zci.andypj.xyz

C#:   interface IShape { double Area(); }
来源：http://skn.gotoacloud.top

[G10] 访问控制
来源：http://hpb.jinqigfzy.top

Py:   约定 _protected / __private（不强制）
来源：http://yuz.xylfe.cn

PHP:  public / protected / private
来源：http://osw.sysykeji.top

JS:   #private 字段；其余公开
来源：http://eap.xingfuxueyuan.xyz

TS:   public / protected / private
来源：http://olp.vehdjk.com

Java: public / protected / private / 默认包级
来源：http://cku.tian-w.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gkn.chenlongwang.top

Ruby: public / protected / private
来源：http://mfo.yonumen.top

C#:   public / protected / private / internal
来源：http://hdi.havefunace.top

[G11] getter / setter
来源：http://jvm.jqgfzy.top

Py:   @property 与 @x.setter
来源：http://bft.xziqi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ovy.shangyingyoupin.top

JS:   get name() { return this._name; }
来源：http://ejw.nanxuanxn.top

TS:   get name(): string { return this._name; }
来源：http://ocx.sweek.top

Java: public String getName() { return name; }
来源：http://scs.yonumen.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ppt.birdmap.top

Ruby: attr_accessor :name
来源：http://mpl.mhx1999.top

C#:   public string Name { get; set; }
来源：http://jzq.52xcode.cn

[G12] 对象转字符串
来源：http://kqb.hcnkem.com

Py:   def __str__(self): return self.name
来源：http://voe.yfazqb.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://nen.yuanzhike.top

JS:   toString() { return this.name; }
来源：http://ica.9152youxi.cn

TS:   toString(): string { return this.name; }
来源：http://stx.tianlin.xyz

Java: @Override public String toString() { return name; }
来源：http://rke.ydzc1.top

Go:   func (u User) String() string { return u.Name }
来源：http://lir.sweek.top

Ruby: def to_s; @name; end
来源：http://kqr.zhiwuduotai.top

C#:   public override string ToString() => Name;
来源：http://zhm.havefunace.top

[G13] 判断对象类型
来源：http://qox.shuidangran.top

Py:   isinstance(u, User)
来源：http://dtc.vehdjk.com

PHP:  $u instanceof User
来源：http://awh.zhongyouzk.top

JS:   u instanceof User
来源：http://gny.xuanzx.com

TS:   u instanceof User
来源：http://ixp.yj202588.top

Java: u instanceof User
来源：http://nff.ivvv.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://qxn.gzhubu.top

Ruby: u.is_a?(User)
来源：http://mfb.mhx1999.top

C#:   u is User
来源：http://tak.yuxming.cn

[G14] 数据类 / record
来源：http://isf.jiagoushi.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://noy.gaohongyu789.top

PHP:  // 用 readonly 属性模拟
来源：http://ycr.jyoumei.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vlf.hnxiangtu.top

TS:   type User = { name: string; age: number };
来源：http://ugs.shanyushiyangkeji.top

Java: record User(String name, int age) {}
来源：http://pld.ctjpmb.com

Go:   type User struct { Name string; Age int }
来源：http://fnl.chenjidiqi.icu

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rdi.zhengqikj.top

C#:   record User(string Name, int Age);
来源：http://lhn.daxiang520.top

[G15] 枚举
来源：http://itj.xuanzx.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://oxw.yuxming.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://cce.bbcook.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://stz.yfazqb.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://agh.xylfe.cn

Java: enum Color { RED, GREEN }
来源：http://ypu.jinqigufen.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xws.daria6918.cn

Ruby: Color = %i[red green].freeze
来源：http://nxk.hnxiangtu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yup.yvedp.cn

[G16] 对象转数组 / 字典
来源：http://sph.gzhubu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://buz.smart0.xyz

PHP:  get_object_vars($obj);
来源：http://sze.ydzc1.top

JS:   Object.entries(obj)
来源：http://wmg.pycfn.com

TS:   Object.entries(obj)
来源：http://yvj.yueranfly.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pau.epnwcf.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://nwa.redwolf501.top

Ruby: obj.instance_variables
来源：http://zho.xylfe.cn

C#:   // 用反射或 System.Text.Json
来源：http://hrw.bjfxy.top

================================================================================
来源：http://pbs.havefunace.top

H. 异常与错误处理
来源：http://yds.yuanzhike.top

================================================================================
来源：http://ibh.tanke756.top

[H01] try / catch 基础
来源：http://ryi.aizwys.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yaa.yueranfly.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tol.yonumen.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://krn.nanxinkj.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rtp.jiagoushi.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gnk.fktsv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ccz.pycfn.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hth.tian-w.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zgv.ydzc1.top

[H02] finally / ensure 收尾
来源：http://mwz.ywan-chungtsiang.top

Py:   try: f()⏎finally: cleanup()
来源：http://aff.andypj.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://cve.ehwqpu.com

JS:   try { f(); } finally { cleanup(); }
来源：http://ooc.jyoumei.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ama.feifeiyinyue.top

Java: try { f(); } finally { cleanup(); }
来源：http://hyk.52xcode.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://aey.shangyingyoupin.top

Ruby: begin; f; ensure; cleanup; end
来源：http://xee.xylfe.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jvt.kuanghao11.cn

[H03] 主动抛出异常
来源：http://otd.yangfankeji.com

Py:   raise ValueError("错误信息")
来源：http://wws.shuidangran.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fvw.dashuyun.cn

JS:   throw new Error("错误信息");
来源：http://wgz.ppjwa.cn

TS:   throw new Error("错误信息");
来源：http://ocn.yanxiufei.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://few.quarkkingdee.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://byc.chenjidiqi.icu

Ruby: raise ArgumentError, "错误信息"
来源：http://hab.cqqwz.cn

C#:   throw new ArgumentException("错误信息");
来源：http://apr.xziqi.cn

[H04] 自定义异常类型
来源：http://mtk.cdnleiting.top

Py:   class MyError(Exception): pass
来源：http://osg.gogol.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ihz.snrcjt.cn

JS:   class MyError extends Error {}
来源：http://ygt.zhongyouzk.top

TS:   class MyError extends Error {}
来源：http://dwp.cheryme.top

Java: class MyException extends RuntimeException {}
来源：http://iaz.jinqigfzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://khf.fanxiaobao.xyz

Ruby: class MyError < StandardError; end
来源：http://abd.hysaishi.cn

C#:   class MyException : Exception {}
来源：http://mow.aibaodan.cn

[H05] 捕获特定类型
来源：http://wsf.ywan-chungtsiang.top

Py:   except ValueError as e:
来源：http://maq.ctjpmb.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nbl.meibo888.top

JS:   if (e instanceof TypeError) {}
来源：http://iid.snrcjt.cn

TS:   if (e instanceof TypeError) {}
来源：http://euf.yonumen.top

Java: catch (IOException | SQLException e) {}
来源：http://asl.vqdsnc.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://iyr.quarkkingdee.top

Ruby: rescue ArgumentError => e
来源：http://ahp.hongshengwenyu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wqg.ydzc1.top

[H06] 可选值 / 空值安全访问
来源：http://quf.chenzaomai.com

Py:   value = d.get("k") or default
来源：http://dud.iojbl.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ofc.vqdsnc.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zvu.gzhubu.top

TS:   obj?.a?.b;  d ?? default
来源：http://dxa.cashguo.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://iol.ctjpmb.com

Go:   if v, ok := m["k"]; ok { }
来源：http://iai.zhijiandao.cn

Ruby: d&.dig(:a, :b)
来源：http://cxp.chenzaomai.com

C#:   obj?.A?.B ?? default
来源：http://pwx.yuanzhike.top

[H07] 断言
来源：http://ybw.cucudq.cn

Py:   assert x > 0, "必须为正"
来源：http://yeb.mhx1999.top

PHP:  assert($x > 0);
来源：http://urf.yuxming.cn

JS:   console.assert(x > 0);
来源：http://jya.iojbl.cn

TS:   console.assert(x > 0);
来源：http://yku.vehdjk.com

Java: assert x > 0 : "必须为正";
来源：http://msi.havefunace.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kfr.wangshuangyany.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ynx.gaohongyu789.top

C#:   Debug.Assert(x > 0);
来源：http://anu.yuxming.cn

[H08] 获取错误信息与堆栈
来源：http://qaq.andypj.xyz

Py:   str(e);  traceback.format_exc()
来源：http://iwp.bbcook.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://aei.xinyue.icu

JS:   e.message;  e.stack
来源：http://enw.sufxvd.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pqi.pengpengdd.cyou

Java: e.getMessage();  e.printStackTrace()
来源：http://cza.jianghu66.top

Go:   err.Error()
来源：http://ist.snrcjt.cn

Ruby: e.message;  e.backtrace
来源：http://xku.tianlin.xyz

C#:   e.Message;  e.StackTrace
来源：http://bth.ivvv.top

[H09] 带错误码的异常
来源：http://owg.daria6918.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kdb.yvedp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ssu.zhongyouzk.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://twu.hesvh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kmd.zhixingplan.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qmg.andypj.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nek.vqdsnc.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bww.sweek.top

C#:   // 自定义异常类中加 Code 属性
来源：http://koi.chenzaomai.com

[H10] 资源自动释放
来源：http://bpp.wangshuangyany.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lui.jinghuilouyu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ztp.ybcxt.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://urk.fengsongda.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uud.gaohongyu789.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pst.redwolf501.top

Go:   defer f.Close()
来源：http://umg.iojbl.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hid.ywan-chungtsiang.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sml.hammf.cn

================================================================================
来源：http://zgk.svipenyu.cn

I. 正则表达式
来源：http://cct.shanyushiyangkeji.top

================================================================================
来源：http://ozs.mhx1999.top

[I01] 判断是否匹配
来源：http://hzw.yueranfly.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xiz.52xcode.cn

PHP:  preg_match('/\d+/', $s);
来源：http://quk.zhijiandao.cn

JS:   /\d+/.test(s)
来源：http://efl.snrcjt.cn

TS:   /\d+/.test(s)
来源：http://alc.yongpay.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xzq.shanyushiyangtech.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ada.fengsongda.top

Ruby: s.match?(/\d+/)
来源：http://qwb.hnqzz.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://inr.birdmap.top

[I02] 提取所有匹配
来源：http://tmv.zhaomingkeji.xyz

Py:   re.findall(r"\d+", s)
来源：http://lii.zdbjq.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mxh.uphjek.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nri.shanyushiyangtech.top

TS:   s.match(/\d+/g)
来源：http://xdm.ppjwa.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://win.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lno.nanxuanxn.top

Ruby: s.scan(/\d+/)
来源：http://vkg.yvedp.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vkv.yj202588.top

[I03] 提取捕获分组
来源：http://kxh.sufxvd.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nzj.fehbvm.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jyy.xylfe.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rzb.hnxiangtu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ffq.epnwcf.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ygz.zhixingplan.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hyn.zhixingplan.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nnd.zycfv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blx.mhx1999.top

[I04] 正则替换
来源：http://ach.hammf.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qxv.jinghuilouyu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jbt.hysaishi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zuu.tianlin.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://abv.guowangkeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://tgc.yj202588.top

Go:   re.ReplaceAllString(s, "#")
来源：http://adb.havefunace.top

Ruby: s.gsub(/\d+/, "#")
来源：http://bvv.sjlbkw.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rjc.sjlbkw.cn

[I05] 按正则拆分
来源：http://ynw.zhiwuduotai.top

Py:   re.split(r"\s*,\s*", s)
来源：http://noo.smart0.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wpp.316326.xyz

JS:   s.split(/\s*,\s*/)
来源：http://vpr.uphjek.com

TS:   s.split(/\s*,\s*/)
来源：http://raq.hongshengwenyu.top

Java: s.split("\\s*,\\s*")
来源：http://dkj.ehwqpu.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hii.yuanzhike.top

Ruby: s.split(/\s*,\s*/)
来源：http://kws.zdbjq.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kfa.shanyushiyangtech.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cpd.guowangkeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bkf.yongpay.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jid.smart0.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wxl.yonumen.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wsx.ivvv.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ywv.feifeiyinyue.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rxe.jqgfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://whw.aizwys.cn


<!-- 参考信息 -->