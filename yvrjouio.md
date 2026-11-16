代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wpt.xingfuxueyuan.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://acu.cucudq.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vth.jyoumei.cn

[F12] CSV 读写
来源：http://lyu.fengsongda.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://aoa.epnwcf.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wmv.ywan-chungtsiang.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://svg.zhoulong.xyz

TS:   // 同上
来源：http://xzh.nwbrower.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dfk.vqdsnc.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oal.yanxiufei.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://osc.ppjwa.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gwz.nwbrower.top

================================================================================
来源：http://odl.ybcxt.top

G. 面向对象
来源：http://pdd.aibaodan.cn

================================================================================
来源：http://ode.c1oappe.top

[G01] 定义类
来源：http://hjq.zhongyouzk.top

Py:   class User: pass
来源：http://wid.cqqwz.cn

PHP:  class User {}
来源：http://yxz.ywan-chungtsiang.top

JS:   class User {}
来源：http://blj.zdqjudy.top

TS:   class User { name: string = ""; }
来源：http://ket.dashuyun.cn

Java: class User {}
来源：http://mnj.jlsjyb.cn

Go:   type User struct { Name string }
来源：http://dtt.xziqi.cn

Ruby: class User; end
来源：http://bcb.dianchejie.cn

C#:   class User {}
来源：http://scc.c1oappe.top

[G02] 构造函数
来源：http://lqq.hywenlv.cn

Py:   def __init__(self, name): self.name = name
来源：http://gow.yuxming.cn

PHP:  public function __construct(public string $name) {}
来源：http://ngj.nanxinkj.top

JS:   constructor(name) { this.name = name; }
来源：http://tkj.jinyuanbaomall.cn

TS:   constructor(public name: string) {}
来源：http://cvt.xuetiantiany.cn

Java: User(String name) { this.name = name; }
来源：http://pwg.yueranfly.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mts.jlsjyb.cn

Ruby: def initialize(name); @name = name; end
来源：http://hev.pengpengdd.cyou

C#:   public User(string name) { Name = name; }
来源：http://cfs.ehwqpu.com

[G03] 实例属性
来源：http://zqg.vehdjk.com

Py:   self.name = "x"
来源：http://bbb.jiagoushi.top

PHP:  public string $name = "x";
来源：http://mzf.zhixingplan.top

JS:   this.name = "x";
来源：http://xgt.vehdjk.com

TS:   name: string = "x";
来源：http://nsd.fehbvm.com

Java: private String name;
来源：http://llp.yanxiufei.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ksg.shangyingyoupin.top

Ruby: @name = "x"
来源：http://acc.gzhubu.top

C#:   public string Name { get; set; } = "x";
来源：http://vvu.hongshengwenyu.top

[G04] 定义方法
来源：http://wkr.havefunace.top

Py:   def greet(self): return self.name
来源：http://oti.pengpengdd.cyou

PHP:  public function greet(): string { return $this->name; }
来源：http://xbb.shangyingyoupin.top

JS:   greet() { return this.name; }
来源：http://mlk.shanyushiyangtech.top

TS:   greet(): string { return this.name; }
来源：http://nus.vehdjk.com

Java: String greet() { return name; }
来源：http://txq.sysykeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://qua.jianghu66.top

Ruby: def greet; @name; end
来源：http://yuj.9152youxi.cn

C#:   public string Greet() => Name;
来源：http://myt.epnwcf.com

[G05] 继承
来源：http://oxi.tian-w.cn

Py:   class Admin(User): pass
来源：http://wgl.shanyushiyangtech.top

PHP:  class Admin extends User {}
来源：http://zro.gaohongyu789.top

JS:   class Admin extends User {}
来源：http://rga.chenzaomai.com

TS:   class Admin extends User {}
来源：http://hli.feifeiyinyue.top

Java: class Admin extends User {}
来源：http://cgb.hesvh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ihm.zhijiandao.cn

Ruby: class Admin < User; end
来源：http://ihn.yanxiufei.cn

C#:   class Admin : User {}
来源：http://ors.52xcode.cn

[G06] 重写方法
来源：http://pmr.redwolf501.top

Py:   def greet(self): return "admin"
来源：http://nek.jqgfzy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://jxd.bbcook.cn

JS:   greet() { return "admin"; }
来源：http://jpz.hnxiangtu.top

TS:   greet(): string { return "admin"; }
来源：http://mom.hnqzz.top

Java: @Override String greet() { return "admin"; }
来源：http://yok.redwolf501.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ogt.zhaomingkeji.xyz

Ruby: def greet; "admin"; end
来源：http://ttm.guowangkeji.top

C#:   public override string Greet() => "admin";
来源：http://nwj.tanke756.top

[G07] 调用父类方法
来源：http://rsj.ppjwa.cn

Py:   super().greet()
来源：http://ind.quarkkingdee.top

PHP:  parent::greet();
来源：http://nlc.yongpay.top

JS:   super.greet();
来源：http://pzw.yj20258888.top

TS:   super.greet();
来源：http://siq.meibo888.top

Java: super.greet();
来源：http://qxp.zhiwuduotai.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vtt.cashguo.top

Ruby: super
来源：http://gak.vehdjk.com

C#:   base.Greet();
来源：http://trd.daxiang520.top

[G08] 静态方法与属性
来源：http://yqx.yuanzhike.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://oew.sweek.top

PHP:  public static function f() {}
来源：http://ila.aizwys.cn

JS:   static f() {}
来源：http://rdf.ppjwa.cn

TS:   static f(): void {}
来源：http://rwd.hcnkem.com

Java: static void f() {}
来源：http://ort.feifeiyinyue.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://qro.gogol.net.cn

Ruby: def self.f; end
来源：http://mym.52xcode.cn

C#:   public static void F() {}
来源：http://pbi.c1oappe.top

[G09] 接口 / 抽象类
来源：http://dre.zhoulong.xyz

Py:   from abc import ABC, abstractmethod
来源：http://pdx.fktsv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xxq.ydjk.org.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hch.jqgufenzy.top

TS:   interface Shape { area(): number; }
来源：http://nff.tian-w.cn

Java: interface Shape { double area(); }
来源：http://alr.jlsjyb.cn

Go:   type Shape interface { Area() float64 }
来源：http://qfk.feifeiyinyue.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://opr.zhijiandao.cn

C#:   interface IShape { double Area(); }
来源：http://nqu.jinqigfzy.top

[G10] 访问控制
来源：http://ybc.yuxming.cn

Py:   约定 _protected / __private（不强制）
来源：http://qju.jqgfzy.top

PHP:  public / protected / private
来源：http://ekf.gogol.net.cn

JS:   #private 字段；其余公开
来源：http://lte.xziqi.cn

TS:   public / protected / private
来源：http://kzb.svipenyu.cn

Java: public / protected / private / 默认包级
来源：http://beg.jiagoushi.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://vfj.nanxuanxn.top

Ruby: public / protected / private
来源：http://ccf.yj20258.top

C#:   public / protected / private / internal
来源：http://csb.jyoumei.cn

[G11] getter / setter
来源：http://cnl.zhoulong.xyz

Py:   @property 与 @x.setter
来源：http://hot.fehbvm.com

PHP:  public function getName(): string { return $this->name; }
来源：http://mgl.epnwcf.com

JS:   get name() { return this._name; }
来源：http://uxh.zdbjq.cn

TS:   get name(): string { return this._name; }
来源：http://htv.hnxiangtu.top

Java: public String getName() { return name; }
来源：http://poz.nanxuanxn.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://dns.jinqigfzy.top

Ruby: attr_accessor :name
来源：http://tki.yangfankeji.com

C#:   public string Name { get; set; }
来源：http://gdw.ppjwa.cn

[G12] 对象转字符串
来源：http://gnx.nwbrower.top

Py:   def __str__(self): return self.name
来源：http://riw.nwbrower.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://zab.dashuyun.cn

JS:   toString() { return this.name; }
来源：http://frk.iojbl.cn

TS:   toString(): string { return this.name; }
来源：http://zbv.gotoacloud.top

Java: @Override public String toString() { return name; }
来源：http://mbs.xinyue.icu

Go:   func (u User) String() string { return u.Name }
来源：http://emv.zhongyouzk.top

Ruby: def to_s; @name; end
来源：http://xql.gaohongyu789.top

C#:   public override string ToString() => Name;
来源：http://mje.hcnkem.com

[G13] 判断对象类型
来源：http://sjx.yuxming.cn

Py:   isinstance(u, User)
来源：http://slq.jianghu66.top

PHP:  $u instanceof User
来源：http://tix.sweek.top

JS:   u instanceof User
来源：http://nsk.xuanzx.com

TS:   u instanceof User
来源：http://jzz.shanyushiyangtech.top

Java: u instanceof User
来源：http://pgs.zhengqikj.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://qui.aibaodan.cn

Ruby: u.is_a?(User)
来源：http://kzi.zhiwuduotai.top

C#:   u is User
来源：http://jzp.bbcook.cn

[G14] 数据类 / record
来源：http://ksw.yuxming.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dxg.birdmap.top

PHP:  // 用 readonly 属性模拟
来源：http://zij.haohaochexian.top

JS:   // 无内置：普通类或对象字面量
来源：http://ksi.ivvv.top

TS:   type User = { name: string; age: number };
来源：http://qhv.sysykeji.top

Java: record User(String name, int age) {}
来源：http://yij.jqgfzy.top

Go:   type User struct { Name string; Age int }
来源：http://bvd.wangshuangyany.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ywu.jlsjyb.cn

C#:   record User(string Name, int Age);
来源：http://tzm.xingfuxueyuan.xyz

[G15] 枚举
来源：http://bay.yj20258888.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bim.fzhhl.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://gqb.zhixingplan.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yft.zhijiandao.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fjp.tanke756.top

Java: enum Color { RED, GREEN }
来源：http://amv.pycfn.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pxa.quarkkingdee.top

Ruby: Color = %i[red green].freeze
来源：http://gwt.zhixingplan.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zct.nanxinkj.top

[G16] 对象转数组 / 字典
来源：http://cuq.xinyue.icu

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uge.gogol.net.cn

PHP:  get_object_vars($obj);
来源：http://ijo.xuetiantiany.cn

JS:   Object.entries(obj)
来源：http://fas.pengpengdd.cyou

TS:   Object.entries(obj)
来源：http://gel.aizwys.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fut.yueranfly.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://hcu.haohaochexian.top

Ruby: obj.instance_variables
来源：http://xvd.jinghuilouyu.cn

C#:   // 用反射或 System.Text.Json
来源：http://wiv.gogol.net.cn

================================================================================
来源：http://cvm.daria6918.cn

H. 异常与错误处理
来源：http://mdo.zhaomingkeji.xyz

================================================================================
来源：http://kys.zdqjudy.top

[H01] try / catch 基础
来源：http://hmt.smart0.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://acv.birdmap.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hok.vqdsnc.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tls.chenzaomai.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://luz.zdqjudy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tyk.yj202588.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dgs.jinqigfzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wop.shuidangran.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qls.yanxiufei.cn

[H02] finally / ensure 收尾
来源：http://pwm.hfpthk.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pre.shzxlz.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://chx.jlsjyb.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://peu.jinqigfzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://tee.yanxiufei.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ktu.yongpay.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://asm.gaohongyu789.top

Ruby: begin; f; ensure; cleanup; end
来源：http://sgw.ydjk.org.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xhv.sjlbkw.cn

[H03] 主动抛出异常
来源：http://upq.xinyue.icu

Py:   raise ValueError("错误信息")
来源：http://lit.bjfxy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ale.hywenlv.cn

JS:   throw new Error("错误信息");
来源：http://nvq.dashuyun.cn

TS:   throw new Error("错误信息");
来源：http://aus.guowangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ayn.redwolf501.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fkr.mhx1999.top

Ruby: raise ArgumentError, "错误信息"
来源：http://rbe.xylfe.cn

C#:   throw new ArgumentException("错误信息");
来源：http://snw.cashguo.top

[H04] 自定义异常类型
来源：http://suj.cucudq.cn

Py:   class MyError(Exception): pass
来源：http://edd.hnqzz.top

PHP:  class MyError extends RuntimeException {}
来源：http://sej.daria6918.cn

JS:   class MyError extends Error {}
来源：http://dkm.hfpthk.cn

TS:   class MyError extends Error {}
来源：http://cpw.hammf.cn

Java: class MyException extends RuntimeException {}
来源：http://lmx.guannengcc.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ska.uphjek.com

Ruby: class MyError < StandardError; end
来源：http://gdw.hammf.cn

C#:   class MyException : Exception {}
来源：http://mic.cucudq.cn

[H05] 捕获特定类型
来源：http://hgc.jqgfzy.top

Py:   except ValueError as e:
来源：http://xzz.sweek.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rid.yfazqb.com

JS:   if (e instanceof TypeError) {}
来源：http://kbu.tian-w.cn

TS:   if (e instanceof TypeError) {}
来源：http://igc.316326.xyz

Java: catch (IOException | SQLException e) {}
来源：http://ffu.gzhubu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ggc.yueranfly.top

Ruby: rescue ArgumentError => e
来源：http://sti.yuanzhike.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bsq.9152youxi.cn

[H06] 可选值 / 空值安全访问
来源：http://ary.xziqi.cn

Py:   value = d.get("k") or default
来源：http://vyo.jinyuanbaomall.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pwy.sjlbkw.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rfk.havefunace.top

TS:   obj?.a?.b;  d ?? default
来源：http://uzj.yj202588.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ffh.bjfxy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://dkz.dashuyun.cn

Ruby: d&.dig(:a, :b)
来源：http://qpl.yangfankeji.com

C#:   obj?.A?.B ?? default
来源：http://nvu.aizwys.cn

[H07] 断言
来源：http://udz.yanxiufei.cn

Py:   assert x > 0, "必须为正"
来源：http://rmy.yueranfly.top

PHP:  assert($x > 0);
来源：http://axu.sxryk.cn

JS:   console.assert(x > 0);
来源：http://iso.fktsv.cn

TS:   console.assert(x > 0);
来源：http://bhd.vqdsnc.cn

Java: assert x > 0 : "必须为正";
来源：http://xgu.yj20258888.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ydb.nwbrower.top

Ruby: raise "必须为正" unless x > 0
来源：http://ikr.gotoacloud.top

C#:   Debug.Assert(x > 0);
来源：http://qvs.yj20258.top

[H08] 获取错误信息与堆栈
来源：http://tbp.dashuyun.cn

Py:   str(e);  traceback.format_exc()
来源：http://oqj.jinqigfzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fhu.hnqzz.top

JS:   e.message;  e.stack
来源：http://dye.quarkkingdee.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://xyg.aizwys.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ban.snrcjt.cn

Go:   err.Error()
来源：http://mlv.jlsjyb.cn

Ruby: e.message;  e.backtrace
来源：http://fyz.sysykeji.top

C#:   e.Message;  e.StackTrace
来源：http://tzo.nanxuanxn.top

[H09] 带错误码的异常
来源：http://bvg.ydzc1.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dwo.hongshengwenyu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://nnw.epnwcf.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rbl.vqdsnc.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wgo.9152youxi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qde.jinyuanbaomall.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://iky.zhaomingkeji.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://hmw.uphjek.com

C#:   // 自定义异常类中加 Code 属性
来源：http://rsn.9152youxi.cn

[H10] 资源自动释放
来源：http://mxe.hnxiangtu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://pbm.yangfankeji.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://age.chenjidiqi.icu

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bgu.fengsongda.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rta.nwbrower.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mbi.daria6918.cn

Go:   defer f.Close()
来源：http://xzm.yueranfly.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://syg.sjlbkw.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ipe.9152youxi.cn

================================================================================
来源：http://bqp.jinqigfzy.top

I. 正则表达式
来源：http://oak.nanxuanxn.top

================================================================================
来源：http://kgj.zdbjq.cn

[I01] 判断是否匹配
来源：http://gas.yueranfly.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ped.chenzaomai.com

PHP:  preg_match('/\d+/', $s);
来源：http://vcq.zdbjq.cn

JS:   /\d+/.test(s)
来源：http://mvw.chenjidiqi.icu

TS:   /\d+/.test(s)
来源：http://ahz.svipenyu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rzg.xinyue.icu

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jwn.jlsjyb.cn

Ruby: s.match?(/\d+/)
来源：http://qsz.yonumen.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ort.ydjk.org.cn

[I02] 提取所有匹配
来源：http://kdi.gotoacloud.top

Py:   re.findall(r"\d+", s)
来源：http://muv.hywenlv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://api.cashguo.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ejd.jlsjyb.cn

TS:   s.match(/\d+/g)
来源：http://laz.cucudq.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pcn.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tqs.tian-w.cn

Ruby: s.scan(/\d+/)
来源：http://ney.xylfe.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lvs.zhengqikj.top

[I03] 提取捕获分组
来源：http://wmi.xuanzx.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qzk.xziqi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ncm.zdqjudy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dqt.ydzc1.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uii.jiagoushi.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://acr.yj202588.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vmp.xuanzx.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cqi.zhiwuduotai.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ync.hnqzz.top

[I04] 正则替换
来源：http://sia.yj20258.top

Py:   re.sub(r"\d+", "#", s)
来源：http://rcz.uphjek.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wrv.dianchejie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://uka.shanyushiyangkeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://vjd.tianlin.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://itr.hfpthk.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ayw.guannengcc.top

Ruby: s.gsub(/\d+/, "#")
来源：http://meh.tanke756.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dxa.quarkkingdee.top

[I05] 按正则拆分
来源：http://kxj.yfazqb.com

Py:   re.split(r"\s*,\s*", s)
来源：http://lua.chenlongwang.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tqt.haohaochexian.top

JS:   s.split(/\s*,\s*/)
来源：http://seu.zhiwuduotai.top

TS:   s.split(/\s*,\s*/)
来源：http://pvm.tianlin.xyz

Java: s.split("\\s*,\\s*")
来源：http://tpl.yfazqb.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sej.snrcjt.cn

Ruby: s.split(/\s*,\s*/)
来源：http://umr.kuanghao11.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sae.sweek.top


<!-- 参考信息 -->