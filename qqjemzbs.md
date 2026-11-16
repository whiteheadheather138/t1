代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://swo.jinyuanbaomall.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gkr.sweek.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fbi.zhijiandao.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ayt.jinqigufen.top

================================================================================
来源：http://dal.jqgfzy.top

G. 面向对象
来源：http://ljk.yuanzhike.top

================================================================================
来源：http://wle.zhengqikj.top

[G01] 定义类
来源：http://bhh.redwolf501.top

Py:   class User: pass
来源：http://uuu.cheryme.top

PHP:  class User {}
来源：http://bke.uphjek.com

JS:   class User {}
来源：http://pnv.fzhhl.top

TS:   class User { name: string = ""; }
来源：http://mbn.daria6918.cn

Java: class User {}
来源：http://xay.cheryme.top

Go:   type User struct { Name string }
来源：http://buj.gotoacloud.top

Ruby: class User; end
来源：http://qjk.shangyingyoupin.top

C#:   class User {}
来源：http://hem.ehwqpu.com

[G02] 构造函数
来源：http://xtx.hesvh.cn

Py:   def __init__(self, name): self.name = name
来源：http://hir.shangyingyoupin.top

PHP:  public function __construct(public string $name) {}
来源：http://utt.xylfe.cn

JS:   constructor(name) { this.name = name; }
来源：http://chm.sweek.top

TS:   constructor(public name: string) {}
来源：http://rus.sysykeji.top

Java: User(String name) { this.name = name; }
来源：http://epa.zhongyouzk.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://toz.cqqwz.cn

Ruby: def initialize(name); @name = name; end
来源：http://tzw.kuanghao11.cn

C#:   public User(string name) { Name = name; }
来源：http://gla.nwbrower.top

[G03] 实例属性
来源：http://kxc.c1oappe.top

Py:   self.name = "x"
来源：http://ect.cashguo.top

PHP:  public string $name = "x";
来源：http://vbm.zdbjq.cn

JS:   this.name = "x";
来源：http://het.hesvh.cn

TS:   name: string = "x";
来源：http://vcw.jlsjyb.cn

Java: private String name;
来源：http://yrc.redwolf501.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jjp.sweek.top

Ruby: @name = "x"
来源：http://qrv.sweek.top

C#:   public string Name { get; set; } = "x";
来源：http://uol.mhx1999.top

[G04] 定义方法
来源：http://zuj.cdnleiting.top

Py:   def greet(self): return self.name
来源：http://ynu.jinqigufen.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hcp.cucudq.cn

JS:   greet() { return this.name; }
来源：http://ujw.vqdsnc.cn

TS:   greet(): string { return this.name; }
来源：http://mvn.gotoacloud.top

Java: String greet() { return name; }
来源：http://gyg.hnqzz.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://tnp.chenlongwang.top

Ruby: def greet; @name; end
来源：http://mvn.316326.xyz

C#:   public string Greet() => Name;
来源：http://jtk.jinqigfzy.top

[G05] 继承
来源：http://nzd.guowangkeji.top

Py:   class Admin(User): pass
来源：http://kwn.zdqjudy.top

PHP:  class Admin extends User {}
来源：http://pii.hongshengwenyu.top

JS:   class Admin extends User {}
来源：http://syt.hongshengwenyu.top

TS:   class Admin extends User {}
来源：http://kwo.svipenyu.cn

Java: class Admin extends User {}
来源：http://yex.haohaochexian.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lon.yonumen.top

Ruby: class Admin < User; end
来源：http://but.yj20258.top

C#:   class Admin : User {}
来源：http://oak.dianchejie.cn

[G06] 重写方法
来源：http://cgc.ehwqpu.com

Py:   def greet(self): return "admin"
来源：http://trd.nwbrower.top

PHP:  public function greet(): string { return "admin"; }
来源：http://exb.meibo888.top

JS:   greet() { return "admin"; }
来源：http://fsg.meibo888.top

TS:   greet(): string { return "admin"; }
来源：http://qta.ydzc1.top

Java: @Override String greet() { return "admin"; }
来源：http://sih.ydjk.org.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tmx.smart0.xyz

Ruby: def greet; "admin"; end
来源：http://klh.cdnleiting.top

C#:   public override string Greet() => "admin";
来源：http://azu.yvedp.cn

[G07] 调用父类方法
来源：http://sra.epnwcf.com

Py:   super().greet()
来源：http://dql.0kj1m.cn

PHP:  parent::greet();
来源：http://rhd.dashuyun.cn

JS:   super.greet();
来源：http://hjf.dianchejie.cn

TS:   super.greet();
来源：http://eqe.hfpthk.cn

Java: super.greet();
来源：http://waz.zhongyouzk.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fng.nwbrower.top

Ruby: super
来源：http://yem.haohaochexian.top

C#:   base.Greet();
来源：http://qpf.ybcxt.top

[G08] 静态方法与属性
来源：http://aer.epnwcf.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://itn.daxiang520.top

PHP:  public static function f() {}
来源：http://hlq.fzhhl.top

JS:   static f() {}
来源：http://hik.yj202588.top

TS:   static f(): void {}
来源：http://gfb.guannengcc.top

Java: static void f() {}
来源：http://slr.daria6918.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://npl.iojbl.cn

Ruby: def self.f; end
来源：http://mrl.zdbjq.cn

C#:   public static void F() {}
来源：http://kvn.aizwys.cn

[G09] 接口 / 抽象类
来源：http://rye.haohaochexian.top

Py:   from abc import ABC, abstractmethod
来源：http://cqp.meibo888.top

PHP:  interface Shape { public function area(): float; }
来源：http://ogs.gaohongyu789.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://jme.pengpengdd.cyou

TS:   interface Shape { area(): number; }
来源：http://bfr.ybcxt.top

Java: interface Shape { double area(); }
来源：http://txh.fktsv.cn

Go:   type Shape interface { Area() float64 }
来源：http://ixg.sxryk.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yer.zhiwuduotai.top

C#:   interface IShape { double Area(); }
来源：http://zmd.sufxvd.cn

[G10] 访问控制
来源：http://dto.hywenlv.cn

Py:   约定 _protected / __private（不强制）
来源：http://ntf.iojbl.cn

PHP:  public / protected / private
来源：http://hro.chenzaomai.com

JS:   #private 字段；其余公开
来源：http://hcf.gaohongyu789.top

TS:   public / protected / private
来源：http://rjd.jqgufenzy.top

Java: public / protected / private / 默认包级
来源：http://qau.xinyue.icu

Go:   首字母大写可导出，小写仅包内可见
来源：http://kmi.316326.xyz

Ruby: public / protected / private
来源：http://qjd.meibo888.top

C#:   public / protected / private / internal
来源：http://abb.yvedp.cn

[G11] getter / setter
来源：http://tpr.gotoacloud.top

Py:   @property 与 @x.setter
来源：http://rkz.redwolf501.top

PHP:  public function getName(): string { return $this->name; }
来源：http://kml.0kj1m.cn

JS:   get name() { return this._name; }
来源：http://paz.hcnkem.com

TS:   get name(): string { return this._name; }
来源：http://swt.bjfxy.top

Java: public String getName() { return name; }
来源：http://yih.shanyushiyangtech.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://cyb.bbcook.cn

Ruby: attr_accessor :name
来源：http://fjd.dianchejie.cn

C#:   public string Name { get; set; }
来源：http://lky.hysaishi.cn

[G12] 对象转字符串
来源：http://dbi.yuanzhike.top

Py:   def __str__(self): return self.name
来源：http://rtn.yvedp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hsd.jqgfzy.top

JS:   toString() { return this.name; }
来源：http://sxb.cheryme.top

TS:   toString(): string { return this.name; }
来源：http://flh.jqgufenzy.top

Java: @Override public String toString() { return name; }
来源：http://dnc.zycfv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://rcb.nanxuanxn.top

Ruby: def to_s; @name; end
来源：http://dnk.daxiang520.top

C#:   public override string ToString() => Name;
来源：http://rhe.haohaochexian.top

[G13] 判断对象类型
来源：http://apa.snrcjt.cn

Py:   isinstance(u, User)
来源：http://qgp.52xcode.cn

PHP:  $u instanceof User
来源：http://xoq.c1oappe.top

JS:   u instanceof User
来源：http://vxv.tianlin.xyz

TS:   u instanceof User
来源：http://ilm.hysaishi.cn

Java: u instanceof User
来源：http://yib.cdnleiting.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://msp.hysaishi.cn

Ruby: u.is_a?(User)
来源：http://vna.bjfxy.top

C#:   u is User
来源：http://mjq.9152youxi.cn

[G14] 数据类 / record
来源：http://ver.nanxinkj.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://djn.fzhhl.top

PHP:  // 用 readonly 属性模拟
来源：http://ges.jianghu66.top

JS:   // 无内置：普通类或对象字面量
来源：http://euo.hnxiangtu.top

TS:   type User = { name: string; age: number };
来源：http://ppt.pengpengdd.cyou

Java: record User(String name, int age) {}
来源：http://owp.wangshuangyany.cn

Go:   type User struct { Name string; Age int }
来源：http://wvv.zhengqikj.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xrs.pycfn.com

C#:   record User(string Name, int Age);
来源：http://oit.guannengcc.top

[G15] 枚举
来源：http://lgx.gogol.net.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://eyi.yvedp.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://iig.shzxlz.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sgv.hywenlv.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ywh.ydjk.org.cn

Java: enum Color { RED, GREEN }
来源：http://ecz.xinyue.icu

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qok.ybcxt.top

Ruby: Color = %i[red green].freeze
来源：http://ujo.snrcjt.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pvd.316326.xyz

[G16] 对象转数组 / 字典
来源：http://qem.yangfankeji.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ckx.yonumen.top

PHP:  get_object_vars($obj);
来源：http://tym.hysaishi.cn

JS:   Object.entries(obj)
来源：http://ami.zhoulong.xyz

TS:   Object.entries(obj)
来源：http://lrd.hnxiangtu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pop.ybcxt.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://fvd.52xcode.cn

Ruby: obj.instance_variables
来源：http://pwt.chenzaomai.com

C#:   // 用反射或 System.Text.Json
来源：http://vwq.zhaomingkeji.xyz

================================================================================
来源：http://gdt.gotoacloud.top

H. 异常与错误处理
来源：http://xxa.hesvh.cn

================================================================================
来源：http://qbj.tanke756.top

[H01] try / catch 基础
来源：http://krx.jianghu66.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vdg.zhoulong.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gti.pengpengdd.cyou

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tpz.hnqzz.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ero.tian-w.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ocp.xuanzx.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vbs.sweek.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mxc.yuxming.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qhz.yj202588.top

[H02] finally / ensure 收尾
来源：http://nwi.jinqigufen.top

Py:   try: f()⏎finally: cleanup()
来源：http://nxg.tian-w.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bqw.yj20258888.top

JS:   try { f(); } finally { cleanup(); }
来源：http://pnn.fehbvm.com

TS:   try { f(); } finally { cleanup(); }
来源：http://lcw.smart0.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://oor.gaohongyu789.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://veg.fzhhl.top

Ruby: begin; f; ensure; cleanup; end
来源：http://lmy.yfazqb.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://snz.jqgfzy.top

[H03] 主动抛出异常
来源：http://bty.birdmap.top

Py:   raise ValueError("错误信息")
来源：http://rtq.jiagoushi.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rca.0kj1m.cn

JS:   throw new Error("错误信息");
来源：http://ltb.shanyushiyangkeji.top

TS:   throw new Error("错误信息");
来源：http://ttv.jinqigufen.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ryl.wangshuangyany.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fcu.tianlin.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://xni.shuidangran.top

C#:   throw new ArgumentException("错误信息");
来源：http://ohh.tian-w.cn

[H04] 自定义异常类型
来源：http://mdw.vqdsnc.cn

Py:   class MyError(Exception): pass
来源：http://lid.sufxvd.cn

PHP:  class MyError extends RuntimeException {}
来源：http://lek.yj20258.top

JS:   class MyError extends Error {}
来源：http://ytq.gzhubu.top

TS:   class MyError extends Error {}
来源：http://eti.guannengcc.top

Java: class MyException extends RuntimeException {}
来源：http://xpn.wangdashe.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zrl.guowangkeji.top

Ruby: class MyError < StandardError; end
来源：http://dtn.zhiwuduotai.top

C#:   class MyException : Exception {}
来源：http://itz.jqgfzy.top

[H05] 捕获特定类型
来源：http://qwj.316326.xyz

Py:   except ValueError as e:
来源：http://xjj.hammf.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://odj.tanke756.top

JS:   if (e instanceof TypeError) {}
来源：http://xlm.jyoumei.cn

TS:   if (e instanceof TypeError) {}
来源：http://tlx.yangfankeji.com

Java: catch (IOException | SQLException e) {}
来源：http://ord.hongshengwenyu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nzs.nwbrower.top

Ruby: rescue ArgumentError => e
来源：http://sxk.kuanghao11.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://geo.0kj1m.cn

[H06] 可选值 / 空值安全访问
来源：http://sav.zdbjq.cn

Py:   value = d.get("k") or default
来源：http://urg.aizwys.cn

PHP:  $v = $d["k"] ?? null;
来源：http://hhs.hywenlv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://eui.52xcode.cn

TS:   obj?.a?.b;  d ?? default
来源：http://kzi.chenlongwang.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hta.c1oappe.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hwp.yongpay.top

Ruby: d&.dig(:a, :b)
来源：http://phb.yj20258.top

C#:   obj?.A?.B ?? default
来源：http://klj.ywan-chungtsiang.top

[H07] 断言
来源：http://ecq.zhaomingkeji.xyz

Py:   assert x > 0, "必须为正"
来源：http://avv.jinqigfzy.top

PHP:  assert($x > 0);
来源：http://krn.xingfuxueyuan.xyz

JS:   console.assert(x > 0);
来源：http://esx.zhixingplan.top

TS:   console.assert(x > 0);
来源：http://sqa.jyoumei.cn

Java: assert x > 0 : "必须为正";
来源：http://ctm.havefunace.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pbu.birdmap.top

Ruby: raise "必须为正" unless x > 0
来源：http://qez.zhaomingkeji.xyz

C#:   Debug.Assert(x > 0);
来源：http://mna.bjfxy.top

[H08] 获取错误信息与堆栈
来源：http://wqm.quarkkingdee.top

Py:   str(e);  traceback.format_exc()
来源：http://hje.xinyue.icu

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ghs.jinqigufen.top

JS:   e.message;  e.stack
来源：http://jnq.tarul.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gzd.zhixingplan.top

Java: e.getMessage();  e.printStackTrace()
来源：http://gzm.tianlin.xyz

Go:   err.Error()
来源：http://lpa.andypj.xyz

Ruby: e.message;  e.backtrace
来源：http://qac.shuidangran.top

C#:   e.Message;  e.StackTrace
来源：http://yxp.yj20258.top

[H09] 带错误码的异常
来源：http://jug.jinyuanbaomall.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cxm.iojbl.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mqw.svipenyu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kfx.dianchejie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gwm.yueranfly.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vxm.guowangkeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vzp.jinyuanbaomall.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jcz.tianlin.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://huy.vqdsnc.cn

[H10] 资源自动释放
来源：http://pyg.zdqjudy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://csv.tian-w.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://njz.bjfxy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xqb.hnqzz.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fhv.ehwqpu.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sbx.cqqwz.cn

Go:   defer f.Close()
来源：http://qxr.meibo888.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://oau.fzhhl.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rve.hammf.cn

================================================================================
来源：http://udd.yangfankeji.com

I. 正则表达式
来源：http://kxw.sjlbkw.cn

================================================================================
来源：http://ngg.sufxvd.cn

[I01] 判断是否匹配
来源：http://dnf.shangyingyoupin.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pxz.cucudq.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ahe.sjlbkw.cn

JS:   /\d+/.test(s)
来源：http://kmi.bbcook.cn

TS:   /\d+/.test(s)
来源：http://lhl.bbcook.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uwf.tanke756.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fnn.c1oappe.top

Ruby: s.match?(/\d+/)
来源：http://gsp.xingfuxueyuan.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://irp.yj202588.top

[I02] 提取所有匹配
来源：http://qvc.cqqwz.cn

Py:   re.findall(r"\d+", s)
来源：http://nnb.chenjidiqi.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yqd.hnxiangtu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vyj.aibaodan.cn

TS:   s.match(/\d+/g)
来源：http://whw.jlsjyb.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lck.jqgfzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ojz.shzxlz.cn

Ruby: s.scan(/\d+/)
来源：http://ced.shanyushiyangtech.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qyj.zhongyouzk.top

[I03] 提取捕获分组
来源：http://xrm.wangshuangyany.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wov.zdbjq.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ork.yonumen.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zwe.ivvv.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rcs.tianlin.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://iyp.shuidangran.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rsr.jinqigfzy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bdi.guowangkeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rdz.shanyushiyangkeji.top

[I04] 正则替换
来源：http://vsg.quarkkingdee.top

Py:   re.sub(r"\d+", "#", s)
来源：http://slr.vqdsnc.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mvj.0kj1m.cn

JS:   s.replace(/\d+/g, "#")
来源：http://juu.sysykeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://inm.jyoumei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wtm.jiagoushi.top

Go:   re.ReplaceAllString(s, "#")
来源：http://sgc.c1oappe.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ras.jinghuilouyu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pdq.yj20258.top

[I05] 按正则拆分
来源：http://ygz.316326.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://bde.sjlbkw.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fbd.quarkkingdee.top

JS:   s.split(/\s*,\s*/)
来源：http://yql.jyoumei.cn

TS:   s.split(/\s*,\s*/)
来源：http://giv.jinqigufen.top

Java: s.split("\\s*,\\s*")
来源：http://ojo.feifeiyinyue.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pny.sweek.top

Ruby: s.split(/\s*,\s*/)
来源：http://skr.gaohongyu789.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ubs.daria6918.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xlp.nanxuanxn.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://frz.fktsv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kmn.yuanzhike.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tha.dashuyun.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nla.yanxiufei.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://shw.meibo888.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hvn.yvedp.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tlo.svipenyu.cn


<!-- 参考信息 -->