代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ypp.ctjpmb.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uqb.fzhhl.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ald.dianchejie.cn

TS:   // 同上
来源：http://eul.cheryme.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pyu.yonumen.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://otg.snrcjt.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gwf.zhiwuduotai.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ssd.kuanghao11.cn

================================================================================
来源：http://rpq.jqgfzy.top

G. 面向对象
来源：http://ygj.cqqwz.cn

================================================================================
来源：http://ito.jqgufenzy.top

[G01] 定义类
来源：http://njm.ivvv.top

Py:   class User: pass
来源：http://yav.dashuyun.cn

PHP:  class User {}
来源：http://teq.0kj1m.cn

JS:   class User {}
来源：http://jtq.nanxinkj.top

TS:   class User { name: string = ""; }
来源：http://lzt.zhongyouzk.top

Java: class User {}
来源：http://mxe.mhx1999.top

Go:   type User struct { Name string }
来源：http://jhs.jinqigfzy.top

Ruby: class User; end
来源：http://wrb.ybcxt.top

C#:   class User {}
来源：http://rwu.mhx1999.top

[G02] 构造函数
来源：http://xyf.hnxiangtu.top

Py:   def __init__(self, name): self.name = name
来源：http://dzq.cashguo.top

PHP:  public function __construct(public string $name) {}
来源：http://iaa.guannengcc.top

JS:   constructor(name) { this.name = name; }
来源：http://iuz.redwolf501.top

TS:   constructor(public name: string) {}
来源：http://yvh.yonumen.top

Java: User(String name) { this.name = name; }
来源：http://ttn.vehdjk.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nob.wangdashe.top

Ruby: def initialize(name); @name = name; end
来源：http://hrq.hammf.cn

C#:   public User(string name) { Name = name; }
来源：http://vsn.sjlbkw.cn

[G03] 实例属性
来源：http://wge.sysykeji.top

Py:   self.name = "x"
来源：http://dpi.yj20258888.top

PHP:  public string $name = "x";
来源：http://dav.ywan-chungtsiang.top

JS:   this.name = "x";
来源：http://fkk.gogol.net.cn

TS:   name: string = "x";
来源：http://wzl.gogol.net.cn

Java: private String name;
来源：http://eln.gotoacloud.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bto.tanke756.top

Ruby: @name = "x"
来源：http://yfp.ehwqpu.com

C#:   public string Name { get; set; } = "x";
来源：http://ufh.mhx1999.top

[G04] 定义方法
来源：http://elc.yueranfly.top

Py:   def greet(self): return self.name
来源：http://has.andypj.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://luj.cheryme.top

JS:   greet() { return this.name; }
来源：http://cex.zhijiandao.cn

TS:   greet(): string { return this.name; }
来源：http://psf.hammf.cn

Java: String greet() { return name; }
来源：http://dlh.andypj.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://osr.yanxiufei.cn

Ruby: def greet; @name; end
来源：http://cno.shanyushiyangkeji.top

C#:   public string Greet() => Name;
来源：http://fnt.xinyue.icu

[G05] 继承
来源：http://pwb.gzhubu.top

Py:   class Admin(User): pass
来源：http://lop.wangdashe.top

PHP:  class Admin extends User {}
来源：http://bys.xinyue.icu

JS:   class Admin extends User {}
来源：http://xvt.yonumen.top

TS:   class Admin extends User {}
来源：http://pxf.yangfankeji.com

Java: class Admin extends User {}
来源：http://unp.sweek.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xzj.haohaochexian.top

Ruby: class Admin < User; end
来源：http://ihj.yangfankeji.com

C#:   class Admin : User {}
来源：http://czr.ivvv.top

[G06] 重写方法
来源：http://pst.nanxinkj.top

Py:   def greet(self): return "admin"
来源：http://jid.nanxinkj.top

PHP:  public function greet(): string { return "admin"; }
来源：http://aon.aizwys.cn

JS:   greet() { return "admin"; }
来源：http://ytm.316326.xyz

TS:   greet(): string { return "admin"; }
来源：http://spd.tianlin.xyz

Java: @Override String greet() { return "admin"; }
来源：http://bum.iojbl.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://obg.yj202588.top

Ruby: def greet; "admin"; end
来源：http://mxm.jiagoushi.top

C#:   public override string Greet() => "admin";
来源：http://pss.zhiwuduotai.top

[G07] 调用父类方法
来源：http://htw.shangyingyoupin.top

Py:   super().greet()
来源：http://bdj.ydjk.org.cn

PHP:  parent::greet();
来源：http://psy.52xcode.cn

JS:   super.greet();
来源：http://lbh.xuetiantiany.cn

TS:   super.greet();
来源：http://vvu.yfazqb.com

Java: super.greet();
来源：http://nqp.hnxiangtu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zqh.tanke756.top

Ruby: super
来源：http://qzx.jinghuilouyu.cn

C#:   base.Greet();
来源：http://dpa.bbcook.cn

[G08] 静态方法与属性
来源：http://igb.bjfxy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hbd.zhengqikj.top

PHP:  public static function f() {}
来源：http://bfg.hcnkem.com

JS:   static f() {}
来源：http://yle.ybcxt.top

TS:   static f(): void {}
来源：http://fvw.hywenlv.cn

Java: static void f() {}
来源：http://yxe.mhx1999.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://qhd.haohaochexian.top

Ruby: def self.f; end
来源：http://wrd.tianlin.xyz

C#:   public static void F() {}
来源：http://cai.ehwqpu.com

[G09] 接口 / 抽象类
来源：http://pdj.hcnkem.com

Py:   from abc import ABC, abstractmethod
来源：http://vpw.ydjk.org.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ugs.chenlongwang.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://rmf.jinyuanbaomall.cn

TS:   interface Shape { area(): number; }
来源：http://ioo.zhengqikj.top

Java: interface Shape { double area(); }
来源：http://hzq.vqdsnc.cn

Go:   type Shape interface { Area() float64 }
来源：http://mhj.sufxvd.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://whs.cqqwz.cn

C#:   interface IShape { double Area(); }
来源：http://wez.tarul.cn

[G10] 访问控制
来源：http://url.cqqwz.cn

Py:   约定 _protected / __private（不强制）
来源：http://ojb.yonumen.top

PHP:  public / protected / private
来源：http://unw.tarul.cn

JS:   #private 字段；其余公开
来源：http://dbl.zdbjq.cn

TS:   public / protected / private
来源：http://dri.zhengqikj.top

Java: public / protected / private / 默认包级
来源：http://qlk.dashuyun.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://yhk.dianchejie.cn

Ruby: public / protected / private
来源：http://zag.kuanghao11.cn

C#:   public / protected / private / internal
来源：http://ulx.svipenyu.cn

[G11] getter / setter
来源：http://ezz.yj202588.top

Py:   @property 与 @x.setter
来源：http://per.yanxiufei.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cij.vehdjk.com

JS:   get name() { return this._name; }
来源：http://vuu.yvedp.cn

TS:   get name(): string { return this._name; }
来源：http://iso.yongpay.top

Java: public String getName() { return name; }
来源：http://lzz.ybcxt.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://olg.ctjpmb.com

Ruby: attr_accessor :name
来源：http://gjk.ybcxt.top

C#:   public string Name { get; set; }
来源：http://yuq.zhixingplan.top

[G12] 对象转字符串
来源：http://hwl.hongshengwenyu.top

Py:   def __str__(self): return self.name
来源：http://cti.sweek.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ens.hfpthk.cn

JS:   toString() { return this.name; }
来源：http://kqc.andypj.xyz

TS:   toString(): string { return this.name; }
来源：http://lfw.tianlin.xyz

Java: @Override public String toString() { return name; }
来源：http://bhc.hammf.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cqd.cqqwz.cn

Ruby: def to_s; @name; end
来源：http://paj.hfpthk.cn

C#:   public override string ToString() => Name;
来源：http://ajb.jqgfzy.top

[G13] 判断对象类型
来源：http://afm.mhx1999.top

Py:   isinstance(u, User)
来源：http://tui.nwbrower.top

PHP:  $u instanceof User
来源：http://lde.hnqzz.top

JS:   u instanceof User
来源：http://zjt.0kj1m.cn

TS:   u instanceof User
来源：http://jpz.jinqigufen.top

Java: u instanceof User
来源：http://rqf.wangshuangyany.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://blj.fengsongda.top

Ruby: u.is_a?(User)
来源：http://aur.ivvv.top

C#:   u is User
来源：http://yet.aibaodan.cn

[G14] 数据类 / record
来源：http://ddy.jqgfzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xil.jinyuanbaomall.cn

PHP:  // 用 readonly 属性模拟
来源：http://rlc.nanxinkj.top

JS:   // 无内置：普通类或对象字面量
来源：http://zoz.jinghuilouyu.cn

TS:   type User = { name: string; age: number };
来源：http://cdm.chenlongwang.top

Java: record User(String name, int age) {}
来源：http://jhi.cucudq.cn

Go:   type User struct { Name string; Age int }
来源：http://daj.9152youxi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://giw.epnwcf.com

C#:   record User(string Name, int Age);
来源：http://aja.zhijiandao.cn

[G15] 枚举
来源：http://roi.snrcjt.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ebz.dashuyun.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ofb.zdbjq.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vlh.smart0.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://alx.mhx1999.top

Java: enum Color { RED, GREEN }
来源：http://vgu.cheryme.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nre.pengpengdd.cyou

Ruby: Color = %i[red green].freeze
来源：http://jpj.zhoulong.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wth.hnqzz.top

[G16] 对象转数组 / 字典
来源：http://vds.gotoacloud.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mir.yj20258888.top

PHP:  get_object_vars($obj);
来源：http://utv.yueranfly.top

JS:   Object.entries(obj)
来源：http://jzi.yanxiufei.cn

TS:   Object.entries(obj)
来源：http://hhy.xinyue.icu

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ylk.sjlbkw.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zqw.fengsongda.top

Ruby: obj.instance_variables
来源：http://kts.fzhhl.top

C#:   // 用反射或 System.Text.Json
来源：http://gua.zdbjq.cn

================================================================================
来源：http://fhl.zhijiandao.cn

H. 异常与错误处理
来源：http://nrb.ydjk.org.cn

================================================================================
来源：http://ntr.guannengcc.top

[H01] try / catch 基础
来源：http://iqu.jinqigufen.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qdu.redwolf501.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qlz.andypj.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rlz.dianchejie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bnj.wangdashe.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fkg.gzhubu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://whu.hnqzz.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mqg.fanxiaobao.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mqf.mhx1999.top

[H02] finally / ensure 收尾
来源：http://eob.fengsongda.top

Py:   try: f()⏎finally: cleanup()
来源：http://wto.epnwcf.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://qxz.zycfv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://trk.snrcjt.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yfn.haohaochexian.top

Java: try { f(); } finally { cleanup(); }
来源：http://pkk.fzhhl.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://woq.dashuyun.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sfq.tanke756.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://mlv.jianghu66.top

[H03] 主动抛出异常
来源：http://hji.nwbrower.top

Py:   raise ValueError("错误信息")
来源：http://nef.fktsv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://joy.sjlbkw.cn

JS:   throw new Error("错误信息");
来源：http://jyt.feifeiyinyue.top

TS:   throw new Error("错误信息");
来源：http://ysx.yuxming.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gru.birdmap.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zys.jinyuanbaomall.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xsn.xylfe.cn

C#:   throw new ArgumentException("错误信息");
来源：http://iye.gzhubu.top

[H04] 自定义异常类型
来源：http://ypc.xuetiantiany.cn

Py:   class MyError(Exception): pass
来源：http://uxt.xziqi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wia.uphjek.com

JS:   class MyError extends Error {}
来源：http://wsy.tianlin.xyz

TS:   class MyError extends Error {}
来源：http://lme.hnqzz.top

Java: class MyException extends RuntimeException {}
来源：http://imz.sxryk.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bbm.kuanghao11.cn

Ruby: class MyError < StandardError; end
来源：http://qbi.c1oappe.top

C#:   class MyException : Exception {}
来源：http://zph.hywenlv.cn

[H05] 捕获特定类型
来源：http://yee.fanxiaobao.xyz

Py:   except ValueError as e:
来源：http://nez.cashguo.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qie.xingfuxueyuan.xyz

JS:   if (e instanceof TypeError) {}
来源：http://cyv.nwbrower.top

TS:   if (e instanceof TypeError) {}
来源：http://rzk.yj202588.top

Java: catch (IOException | SQLException e) {}
来源：http://hch.yfazqb.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hug.meibo888.top

Ruby: rescue ArgumentError => e
来源：http://ypc.jyoumei.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wzo.yvedp.cn

[H06] 可选值 / 空值安全访问
来源：http://xyp.jqgfzy.top

Py:   value = d.get("k") or default
来源：http://okn.gogol.net.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qdq.ydjk.org.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qcx.quarkkingdee.top

TS:   obj?.a?.b;  d ?? default
来源：http://svz.zhongyouzk.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sys.bbcook.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ofi.mhx1999.top

Ruby: d&.dig(:a, :b)
来源：http://myc.hywenlv.cn

C#:   obj?.A?.B ?? default
来源：http://olr.sufxvd.cn

[H07] 断言
来源：http://kgh.xuetiantiany.cn

Py:   assert x > 0, "必须为正"
来源：http://nbe.zhongyouzk.top

PHP:  assert($x > 0);
来源：http://opz.shuidangran.top

JS:   console.assert(x > 0);
来源：http://uks.yvedp.cn

TS:   console.assert(x > 0);
来源：http://csb.kuanghao11.cn

Java: assert x > 0 : "必须为正";
来源：http://nej.meibo888.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lpi.vqdsnc.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jnq.nanxinkj.top

C#:   Debug.Assert(x > 0);
来源：http://adg.gogol.net.cn

[H08] 获取错误信息与堆栈
来源：http://meh.jlsjyb.cn

Py:   str(e);  traceback.format_exc()
来源：http://oqs.havefunace.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jcg.tanke756.top

JS:   e.message;  e.stack
来源：http://bpu.fktsv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pbc.gaohongyu789.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xhq.ctjpmb.com

Go:   err.Error()
来源：http://bmi.yueranfly.top

Ruby: e.message;  e.backtrace
来源：http://ols.dianchejie.cn

C#:   e.Message;  e.StackTrace
来源：http://jur.smart0.xyz

[H09] 带错误码的异常
来源：http://rys.ehwqpu.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fmr.jinghuilouyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://tnz.ehwqpu.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ybn.feifeiyinyue.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mef.xinyue.icu

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pxk.dianchejie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zcu.52xcode.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ekx.hywenlv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ijb.9152youxi.cn

[H10] 资源自动释放
来源：http://zea.ywan-chungtsiang.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://eix.yueranfly.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zgc.daxiang520.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bmo.yj20258.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://azu.aibaodan.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hlp.jyoumei.cn

Go:   defer f.Close()
来源：http://wnc.hysaishi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bnf.smart0.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vme.hnxiangtu.top

================================================================================
来源：http://qen.haohaochexian.top

I. 正则表达式
来源：http://avp.jqgufenzy.top

================================================================================
来源：http://xyt.meibo888.top

[I01] 判断是否匹配
来源：http://rbl.jianghu66.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dlk.bjfxy.top

PHP:  preg_match('/\d+/', $s);
来源：http://mdm.haohaochexian.top

JS:   /\d+/.test(s)
来源：http://rat.meibo888.top

TS:   /\d+/.test(s)
来源：http://enc.zhixingplan.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xwl.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wpi.mhx1999.top

Ruby: s.match?(/\d+/)
来源：http://swt.shanyushiyangtech.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://iym.ehwqpu.com

[I02] 提取所有匹配
来源：http://uoq.yonumen.top

Py:   re.findall(r"\d+", s)
来源：http://vie.0kj1m.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qxy.jiagoushi.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wnv.jqgufenzy.top

TS:   s.match(/\d+/g)
来源：http://wbt.yj20258.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://epc.zhijiandao.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ugx.jianghu66.top

Ruby: s.scan(/\d+/)
来源：http://zbg.tianlin.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://esi.fktsv.cn

[I03] 提取捕获分组
来源：http://lqu.hysaishi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ite.316326.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vsh.gaohongyu789.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://khw.shuidangran.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rit.yfazqb.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ewa.sysykeji.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://okq.wangdashe.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zsv.jianghu66.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ovh.zhongyouzk.top

[I04] 正则替换
来源：http://bmi.dianchejie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zaf.nanxinkj.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ryo.jinghuilouyu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wof.nanxinkj.top

TS:   s.replace(/\d+/g, "#")
来源：http://mpy.ehwqpu.com

Java: s.replaceAll("\\d+", "#")
来源：http://kwk.snrcjt.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zri.0kj1m.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xky.jinqigfzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://isb.mhx1999.top

[I05] 按正则拆分
来源：http://thb.zhengqikj.top

Py:   re.split(r"\s*,\s*", s)
来源：http://yia.yj20258888.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cxu.tarul.cn

JS:   s.split(/\s*,\s*/)
来源：http://wng.zycfv.cn

TS:   s.split(/\s*,\s*/)
来源：http://phz.xingfuxueyuan.xyz

Java: s.split("\\s*,\\s*")
来源：http://lrb.yangfankeji.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hhy.birdmap.top

Ruby: s.split(/\s*,\s*/)
来源：http://vzu.jqgufenzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ekc.nanxinkj.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pur.yuanzhike.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ohj.9152youxi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uoz.birdmap.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aet.zdbjq.cn


<!-- 参考信息 -->