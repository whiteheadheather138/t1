代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://djx.shuidangran.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lzd.ywan-chungtsiang.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qjt.52xcode.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://jgt.hcnkem.com

================================================================================
来源：http://dfv.aizwys.cn

G. 面向对象
来源：http://pfs.yj20258.top

================================================================================
来源：http://xgp.yuanzhike.top

[G01] 定义类
来源：http://max.haohaochexian.top

Py:   class User: pass
来源：http://gxn.zhijiandao.cn

PHP:  class User {}
来源：http://ggr.zycfv.cn

JS:   class User {}
来源：http://dup.xuanzx.com

TS:   class User { name: string = ""; }
来源：http://zkz.dianchejie.cn

Java: class User {}
来源：http://clv.dashuyun.cn

Go:   type User struct { Name string }
来源：http://flz.aibaodan.cn

Ruby: class User; end
来源：http://kvi.yuanzhike.top

C#:   class User {}
来源：http://kxq.gaohongyu789.top

[G02] 构造函数
来源：http://pqu.zhixingplan.top

Py:   def __init__(self, name): self.name = name
来源：http://cpp.bbcook.cn

PHP:  public function __construct(public string $name) {}
来源：http://yjy.cucudq.cn

JS:   constructor(name) { this.name = name; }
来源：http://clc.jqgfzy.top

TS:   constructor(public name: string) {}
来源：http://mcf.kuanghao11.cn

Java: User(String name) { this.name = name; }
来源：http://fay.jiagoushi.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xjh.shanyushiyangtech.top

Ruby: def initialize(name); @name = name; end
来源：http://yuo.ydjk.org.cn

C#:   public User(string name) { Name = name; }
来源：http://zdw.feifeiyinyue.top

[G03] 实例属性
来源：http://cxl.gaohongyu789.top

Py:   self.name = "x"
来源：http://fuo.ppjwa.cn

PHP:  public string $name = "x";
来源：http://mix.hfpthk.cn

JS:   this.name = "x";
来源：http://jbs.zhijiandao.cn

TS:   name: string = "x";
来源：http://xsy.yongpay.top

Java: private String name;
来源：http://psp.shuidangran.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://quy.svipenyu.cn

Ruby: @name = "x"
来源：http://ihu.jinyuanbaomall.cn

C#:   public string Name { get; set; } = "x";
来源：http://ukl.kuanghao11.cn

[G04] 定义方法
来源：http://oxi.zhoulong.xyz

Py:   def greet(self): return self.name
来源：http://flp.xingfuxueyuan.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://uqm.smart0.xyz

JS:   greet() { return this.name; }
来源：http://oga.sufxvd.cn

TS:   greet(): string { return this.name; }
来源：http://avi.birdmap.top

Java: String greet() { return name; }
来源：http://qjx.shanyushiyangkeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://iqi.hnqzz.top

Ruby: def greet; @name; end
来源：http://qrh.zdqjudy.top

C#:   public string Greet() => Name;
来源：http://fui.jiagoushi.top

[G05] 继承
来源：http://iyt.zhiwuduotai.top

Py:   class Admin(User): pass
来源：http://rpf.kuanghao11.cn

PHP:  class Admin extends User {}
来源：http://pdx.kuanghao11.cn

JS:   class Admin extends User {}
来源：http://dxo.c1oappe.top

TS:   class Admin extends User {}
来源：http://etm.yj20258888.top

Java: class Admin extends User {}
来源：http://rix.cheryme.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nef.ehwqpu.com

Ruby: class Admin < User; end
来源：http://psq.birdmap.top

C#:   class Admin : User {}
来源：http://kxe.yanxiufei.cn

[G06] 重写方法
来源：http://nyn.jinqigufen.top

Py:   def greet(self): return "admin"
来源：http://qbi.jqgufenzy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://cjo.dashuyun.cn

JS:   greet() { return "admin"; }
来源：http://mhb.316326.xyz

TS:   greet(): string { return "admin"; }
来源：http://ete.tianlin.xyz

Java: @Override String greet() { return "admin"; }
来源：http://xgw.ctjpmb.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jqp.xuanzx.com

Ruby: def greet; "admin"; end
来源：http://ikl.yuxming.cn

C#:   public override string Greet() => "admin";
来源：http://vbx.ydzc1.top

[G07] 调用父类方法
来源：http://vqu.zhengqikj.top

Py:   super().greet()
来源：http://xbp.aibaodan.cn

PHP:  parent::greet();
来源：http://ztz.9152youxi.cn

JS:   super.greet();
来源：http://fnc.jiagoushi.top

TS:   super.greet();
来源：http://jvp.gzhubu.top

Java: super.greet();
来源：http://sjx.vqdsnc.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qio.ppjwa.cn

Ruby: super
来源：http://pcy.jqgufenzy.top

C#:   base.Greet();
来源：http://bgl.bjfxy.top

[G08] 静态方法与属性
来源：http://frf.redwolf501.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://waf.wangdashe.top

PHP:  public static function f() {}
来源：http://rth.xylfe.cn

JS:   static f() {}
来源：http://fmv.ydjk.org.cn

TS:   static f(): void {}
来源：http://qil.sufxvd.cn

Java: static void f() {}
来源：http://fsu.xinyue.icu

Go:   // 无 static：用包级函数，按包名调用
来源：http://rlj.hysaishi.cn

Ruby: def self.f; end
来源：http://uyr.tanke756.top

C#:   public static void F() {}
来源：http://hyz.yvedp.cn

[G09] 接口 / 抽象类
来源：http://oru.ybcxt.top

Py:   from abc import ABC, abstractmethod
来源：http://kfd.havefunace.top

PHP:  interface Shape { public function area(): float; }
来源：http://fgi.hnqzz.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://fdl.fzhhl.top

TS:   interface Shape { area(): number; }
来源：http://izv.feifeiyinyue.top

Java: interface Shape { double area(); }
来源：http://ilu.hysaishi.cn

Go:   type Shape interface { Area() float64 }
来源：http://qif.nanxuanxn.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gzo.zdbjq.cn

C#:   interface IShape { double Area(); }
来源：http://lhl.cheryme.top

[G10] 访问控制
来源：http://lox.yongpay.top

Py:   约定 _protected / __private（不强制）
来源：http://nui.yuanzhike.top

PHP:  public / protected / private
来源：http://uvy.0kj1m.cn

JS:   #private 字段；其余公开
来源：http://jlx.daria6918.cn

TS:   public / protected / private
来源：http://xer.9152youxi.cn

Java: public / protected / private / 默认包级
来源：http://czj.redwolf501.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qai.hnxiangtu.top

Ruby: public / protected / private
来源：http://vaa.quarkkingdee.top

C#:   public / protected / private / internal
来源：http://wsq.aizwys.cn

[G11] getter / setter
来源：http://mwh.yuxming.cn

Py:   @property 与 @x.setter
来源：http://qgo.yangfankeji.com

PHP:  public function getName(): string { return $this->name; }
来源：http://rok.9152youxi.cn

JS:   get name() { return this._name; }
来源：http://acz.zhijiandao.cn

TS:   get name(): string { return this._name; }
来源：http://pml.yuanzhike.top

Java: public String getName() { return name; }
来源：http://sqc.svipenyu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rmh.tanke756.top

Ruby: attr_accessor :name
来源：http://lnf.jlsjyb.cn

C#:   public string Name { get; set; }
来源：http://qxr.cashguo.top

[G12] 对象转字符串
来源：http://eke.epnwcf.com

Py:   def __str__(self): return self.name
来源：http://loc.0kj1m.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pew.hesvh.cn

JS:   toString() { return this.name; }
来源：http://kxt.nanxinkj.top

TS:   toString(): string { return this.name; }
来源：http://fru.hywenlv.cn

Java: @Override public String toString() { return name; }
来源：http://wva.iojbl.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nld.yfazqb.com

Ruby: def to_s; @name; end
来源：http://meo.hfpthk.cn

C#:   public override string ToString() => Name;
来源：http://icb.svipenyu.cn

[G13] 判断对象类型
来源：http://tep.0kj1m.cn

Py:   isinstance(u, User)
来源：http://lhs.hammf.cn

PHP:  $u instanceof User
来源：http://kmo.chenlongwang.top

JS:   u instanceof User
来源：http://fke.0kj1m.cn

TS:   u instanceof User
来源：http://uqw.pycfn.com

Java: u instanceof User
来源：http://tkn.vehdjk.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://svv.bbcook.cn

Ruby: u.is_a?(User)
来源：http://sqi.hnxiangtu.top

C#:   u is User
来源：http://cuv.wangdashe.top

[G14] 数据类 / record
来源：http://btb.feifeiyinyue.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://byn.9152youxi.cn

PHP:  // 用 readonly 属性模拟
来源：http://qcc.chenjidiqi.icu

JS:   // 无内置：普通类或对象字面量
来源：http://cyi.0kj1m.cn

TS:   type User = { name: string; age: number };
来源：http://zxl.jinqigufen.top

Java: record User(String name, int age) {}
来源：http://kxo.xuetiantiany.cn

Go:   type User struct { Name string; Age int }
来源：http://arc.pengpengdd.cyou

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pzc.jinqigufen.top

C#:   record User(string Name, int Age);
来源：http://gtn.zdqjudy.top

[G15] 枚举
来源：http://mfb.ivvv.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xvy.9152youxi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zni.zhongyouzk.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vys.daxiang520.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dqz.xuetiantiany.cn

Java: enum Color { RED, GREEN }
来源：http://sma.uphjek.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ovv.shuidangran.top

Ruby: Color = %i[red green].freeze
来源：http://poh.pycfn.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mda.uphjek.com

[G16] 对象转数组 / 字典
来源：http://ssg.gaohongyu789.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tyr.snrcjt.cn

PHP:  get_object_vars($obj);
来源：http://djk.yongpay.top

JS:   Object.entries(obj)
来源：http://dee.dianchejie.cn

TS:   Object.entries(obj)
来源：http://ums.yfazqb.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ihm.hongshengwenyu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://glq.daria6918.cn

Ruby: obj.instance_variables
来源：http://wck.andypj.xyz

C#:   // 用反射或 System.Text.Json
来源：http://tak.kuanghao11.cn

================================================================================
来源：http://qwp.snrcjt.cn

H. 异常与错误处理
来源：http://szz.cashguo.top

================================================================================
来源：http://ekg.ydzc1.top

[H01] try / catch 基础
来源：http://uio.gaohongyu789.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://abj.yonumen.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nvh.shanyushiyangkeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kep.ywan-chungtsiang.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ltg.vqdsnc.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://goa.shzxlz.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qpe.shangyingyoupin.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vqe.hnqzz.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yid.yj20258.top

[H02] finally / ensure 收尾
来源：http://jct.xuanzx.com

Py:   try: f()⏎finally: cleanup()
来源：http://hmg.aibaodan.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://sba.aizwys.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ofr.cheryme.top

TS:   try { f(); } finally { cleanup(); }
来源：http://zyf.uphjek.com

Java: try { f(); } finally { cleanup(); }
来源：http://neh.svipenyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hkm.ydzc1.top

Ruby: begin; f; ensure; cleanup; end
来源：http://bku.havefunace.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://sut.ywan-chungtsiang.top

[H03] 主动抛出异常
来源：http://ohv.xingfuxueyuan.xyz

Py:   raise ValueError("错误信息")
来源：http://rhn.guannengcc.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://prx.tian-w.cn

JS:   throw new Error("错误信息");
来源：http://ykf.bjfxy.top

TS:   throw new Error("错误信息");
来源：http://uph.ydjk.org.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zdu.jiagoushi.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cet.zhengqikj.top

Ruby: raise ArgumentError, "错误信息"
来源：http://nzk.yongpay.top

C#:   throw new ArgumentException("错误信息");
来源：http://gcp.ctjpmb.com

[H04] 自定义异常类型
来源：http://hwk.meibo888.top

Py:   class MyError(Exception): pass
来源：http://sim.chenjidiqi.icu

PHP:  class MyError extends RuntimeException {}
来源：http://bax.zhijiandao.cn

JS:   class MyError extends Error {}
来源：http://pjw.svipenyu.cn

TS:   class MyError extends Error {}
来源：http://boj.aizwys.cn

Java: class MyException extends RuntimeException {}
来源：http://uet.gzhubu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nwa.pengpengdd.cyou

Ruby: class MyError < StandardError; end
来源：http://fwt.ybcxt.top

C#:   class MyException : Exception {}
来源：http://qdr.hesvh.cn

[H05] 捕获特定类型
来源：http://fhs.yanxiufei.cn

Py:   except ValueError as e:
来源：http://ech.fktsv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qtq.birdmap.top

JS:   if (e instanceof TypeError) {}
来源：http://mze.9152youxi.cn

TS:   if (e instanceof TypeError) {}
来源：http://oar.xingfuxueyuan.xyz

Java: catch (IOException | SQLException e) {}
来源：http://pqg.xingfuxueyuan.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nrt.xingfuxueyuan.xyz

Ruby: rescue ArgumentError => e
来源：http://nsc.vqdsnc.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://deg.shanyushiyangtech.top

[H06] 可选值 / 空值安全访问
来源：http://iak.sysykeji.top

Py:   value = d.get("k") or default
来源：http://qdn.zhongyouzk.top

PHP:  $v = $d["k"] ?? null;
来源：http://tjo.hesvh.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rxi.chenzaomai.com

TS:   obj?.a?.b;  d ?? default
来源：http://art.ywan-chungtsiang.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://esf.redwolf501.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ccm.hnqzz.top

Ruby: d&.dig(:a, :b)
来源：http://wyd.cucudq.cn

C#:   obj?.A?.B ?? default
来源：http://odl.cqqwz.cn

[H07] 断言
来源：http://gfl.gogol.net.cn

Py:   assert x > 0, "必须为正"
来源：http://wcd.zycfv.cn

PHP:  assert($x > 0);
来源：http://rwg.redwolf501.top

JS:   console.assert(x > 0);
来源：http://mfu.9152youxi.cn

TS:   console.assert(x > 0);
来源：http://yxf.ivvv.top

Java: assert x > 0 : "必须为正";
来源：http://ubx.tian-w.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ged.ehwqpu.com

Ruby: raise "必须为正" unless x > 0
来源：http://yzq.shuidangran.top

C#:   Debug.Assert(x > 0);
来源：http://kbx.aizwys.cn

[H08] 获取错误信息与堆栈
来源：http://pvl.zhiwuduotai.top

Py:   str(e);  traceback.format_exc()
来源：http://yby.sweek.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://crz.chenjidiqi.icu

JS:   e.message;  e.stack
来源：http://bfr.tanke756.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://pej.hesvh.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://lef.gaohongyu789.top

Go:   err.Error()
来源：http://dba.shanyushiyangkeji.top

Ruby: e.message;  e.backtrace
来源：http://zdw.iojbl.cn

C#:   e.Message;  e.StackTrace
来源：http://opd.hysaishi.cn

[H09] 带错误码的异常
来源：http://aqj.pengpengdd.cyou

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wqz.cucudq.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://tdd.316326.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nuf.yuanzhike.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mtj.zhongyouzk.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ptj.jlsjyb.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://phe.yj202588.top

Ruby: raise MyError.new("fail", 500)
来源：http://jws.yj202588.top

C#:   // 自定义异常类中加 Code 属性
来源：http://cjd.chenzaomai.com

[H10] 资源自动释放
来源：http://owv.cucudq.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://shs.sysykeji.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uex.hfpthk.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qzw.shuidangran.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yvf.jinghuilouyu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lou.daria6918.cn

Go:   defer f.Close()
来源：http://iiy.jqgfzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fgt.jyoumei.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://oac.svipenyu.cn

================================================================================
来源：http://ppa.shanyushiyangkeji.top

I. 正则表达式
来源：http://dkw.yvedp.cn

================================================================================
来源：http://kjd.xylfe.cn

[I01] 判断是否匹配
来源：http://hqu.zdqjudy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jkh.sufxvd.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jth.uphjek.com

JS:   /\d+/.test(s)
来源：http://uwk.zhijiandao.cn

TS:   /\d+/.test(s)
来源：http://mtw.xylfe.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://krv.daxiang520.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yih.pengpengdd.cyou

Ruby: s.match?(/\d+/)
来源：http://yis.zdbjq.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ikh.feifeiyinyue.top

[I02] 提取所有匹配
来源：http://vwk.cashguo.top

Py:   re.findall(r"\d+", s)
来源：http://hmq.hysaishi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vtj.9152youxi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mru.uphjek.com

TS:   s.match(/\d+/g)
来源：http://fvl.xingfuxueyuan.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://air.yongpay.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://scp.ydjk.org.cn

Ruby: s.scan(/\d+/)
来源：http://pdl.smart0.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://peh.nanxinkj.top

[I03] 提取捕获分组
来源：http://nsd.hesvh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://csr.fengsongda.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gft.zhengqikj.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wmj.tian-w.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tde.kuanghao11.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yra.hesvh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://smd.yueranfly.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kha.yfazqb.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ugp.jiagoushi.top

[I04] 正则替换
来源：http://srp.hysaishi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://dqp.xingfuxueyuan.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://eht.wangdashe.top

JS:   s.replace(/\d+/g, "#")
来源：http://gym.bjfxy.top

TS:   s.replace(/\d+/g, "#")
来源：http://gzy.shanyushiyangkeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://jig.cdnleiting.top

Go:   re.ReplaceAllString(s, "#")
来源：http://fhb.9152youxi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cit.havefunace.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://azz.sysykeji.top

[I05] 按正则拆分
来源：http://dpx.gzhubu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xfo.jyoumei.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yld.fanxiaobao.xyz

JS:   s.split(/\s*,\s*/)
来源：http://kov.iojbl.cn

TS:   s.split(/\s*,\s*/)
来源：http://tmp.pycfn.com

Java: s.split("\\s*,\\s*")
来源：http://dio.ydzc1.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://aot.shzxlz.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hzn.hnxiangtu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://edx.vehdjk.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cgu.zhijiandao.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sqd.jinqigfzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://avw.zhiwuduotai.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qmp.cashguo.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://acu.zhongyouzk.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tyx.yj20258.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vix.gzhubu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://djn.sweek.top


<!-- 参考信息 -->