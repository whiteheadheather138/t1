代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pgf.meibo888.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ygh.9152youxi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ojq.ydjk.org.cn

TS:   // 同上
来源：http://cxg.hesvh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jaf.jlsjyb.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ozj.zhoulong.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jrn.jqgfzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://qhy.ydjk.org.cn

================================================================================
来源：http://ggo.shuidangran.top

G. 面向对象
来源：http://ycl.jinghuilouyu.cn

================================================================================
来源：http://bst.xziqi.cn

[G01] 定义类
来源：http://jkr.haohaochexian.top

Py:   class User: pass
来源：http://kgw.zycfv.cn

PHP:  class User {}
来源：http://bfy.wangshuangyany.cn

JS:   class User {}
来源：http://pbs.bjfxy.top

TS:   class User { name: string = ""; }
来源：http://bta.havefunace.top

Java: class User {}
来源：http://hyj.haohaochexian.top

Go:   type User struct { Name string }
来源：http://idz.nanxinkj.top

Ruby: class User; end
来源：http://iwv.xuetiantiany.cn

C#:   class User {}
来源：http://mlr.vehdjk.com

[G02] 构造函数
来源：http://tpa.cdnleiting.top

Py:   def __init__(self, name): self.name = name
来源：http://ygd.bbcook.cn

PHP:  public function __construct(public string $name) {}
来源：http://ydq.yj20258888.top

JS:   constructor(name) { this.name = name; }
来源：http://hxo.jlsjyb.cn

TS:   constructor(public name: string) {}
来源：http://ehp.jiagoushi.top

Java: User(String name) { this.name = name; }
来源：http://lnv.ppjwa.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yty.fehbvm.com

Ruby: def initialize(name); @name = name; end
来源：http://koh.aibaodan.cn

C#:   public User(string name) { Name = name; }
来源：http://wyt.guowangkeji.top

[G03] 实例属性
来源：http://xrm.zhongyouzk.top

Py:   self.name = "x"
来源：http://cds.guannengcc.top

PHP:  public string $name = "x";
来源：http://sqa.yuanzhike.top

JS:   this.name = "x";
来源：http://snj.sweek.top

TS:   name: string = "x";
来源：http://etp.jinqigfzy.top

Java: private String name;
来源：http://qvm.sjlbkw.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jit.jinqigfzy.top

Ruby: @name = "x"
来源：http://zvw.aibaodan.cn

C#:   public string Name { get; set; } = "x";
来源：http://jqb.jqgfzy.top

[G04] 定义方法
来源：http://dsz.ywan-chungtsiang.top

Py:   def greet(self): return self.name
来源：http://vfh.meibo888.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hhw.vehdjk.com

JS:   greet() { return this.name; }
来源：http://dsu.uphjek.com

TS:   greet(): string { return this.name; }
来源：http://ius.epnwcf.com

Java: String greet() { return name; }
来源：http://uwa.zhoulong.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://sfe.yvedp.cn

Ruby: def greet; @name; end
来源：http://gvn.gzhubu.top

C#:   public string Greet() => Name;
来源：http://wfh.fzhhl.top

[G05] 继承
来源：http://ppo.yongpay.top

Py:   class Admin(User): pass
来源：http://vwk.hammf.cn

PHP:  class Admin extends User {}
来源：http://pto.yanxiufei.cn

JS:   class Admin extends User {}
来源：http://jvf.tian-w.cn

TS:   class Admin extends User {}
来源：http://rmm.yj20258.top

Java: class Admin extends User {}
来源：http://kkx.pycfn.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bol.chenjidiqi.icu

Ruby: class Admin < User; end
来源：http://rdy.feifeiyinyue.top

C#:   class Admin : User {}
来源：http://fmp.cashguo.top

[G06] 重写方法
来源：http://qxc.chenzaomai.com

Py:   def greet(self): return "admin"
来源：http://nal.tian-w.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fyr.chenlongwang.top

JS:   greet() { return "admin"; }
来源：http://cee.ppjwa.cn

TS:   greet(): string { return "admin"; }
来源：http://wyg.chenjidiqi.icu

Java: @Override String greet() { return "admin"; }
来源：http://dau.cqqwz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rhr.daria6918.cn

Ruby: def greet; "admin"; end
来源：http://gfs.52xcode.cn

C#:   public override string Greet() => "admin";
来源：http://pzj.sweek.top

[G07] 调用父类方法
来源：http://los.aizwys.cn

Py:   super().greet()
来源：http://ecv.jyoumei.cn

PHP:  parent::greet();
来源：http://uvv.ctjpmb.com

JS:   super.greet();
来源：http://dwo.yuxming.cn

TS:   super.greet();
来源：http://xgc.zdqjudy.top

Java: super.greet();
来源：http://zjc.zhixingplan.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bsi.feifeiyinyue.top

Ruby: super
来源：http://igw.jianghu66.top

C#:   base.Greet();
来源：http://avk.hywenlv.cn

[G08] 静态方法与属性
来源：http://rot.c1oappe.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ipe.dashuyun.cn

PHP:  public static function f() {}
来源：http://wlg.tian-w.cn

JS:   static f() {}
来源：http://ajy.feifeiyinyue.top

TS:   static f(): void {}
来源：http://rth.ivvv.top

Java: static void f() {}
来源：http://day.quarkkingdee.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://dfa.quarkkingdee.top

Ruby: def self.f; end
来源：http://ecl.yongpay.top

C#:   public static void F() {}
来源：http://gcr.tarul.cn

[G09] 接口 / 抽象类
来源：http://pig.nanxinkj.top

Py:   from abc import ABC, abstractmethod
来源：http://fzm.zhongyouzk.top

PHP:  interface Shape { public function area(): float; }
来源：http://ekc.andypj.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://yop.chenjidiqi.icu

TS:   interface Shape { area(): number; }
来源：http://ieu.xingfuxueyuan.xyz

Java: interface Shape { double area(); }
来源：http://mrq.ydjk.org.cn

Go:   type Shape interface { Area() float64 }
来源：http://woq.feifeiyinyue.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://poq.quarkkingdee.top

C#:   interface IShape { double Area(); }
来源：http://qkn.zhengqikj.top

[G10] 访问控制
来源：http://hsf.xuetiantiany.cn

Py:   约定 _protected / __private（不强制）
来源：http://bqt.sufxvd.cn

PHP:  public / protected / private
来源：http://beu.9152youxi.cn

JS:   #private 字段；其余公开
来源：http://hgj.ppjwa.cn

TS:   public / protected / private
来源：http://jyk.shuidangran.top

Java: public / protected / private / 默认包级
来源：http://fkj.shzxlz.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://uyp.zycfv.cn

Ruby: public / protected / private
来源：http://ihr.zhongyouzk.top

C#:   public / protected / private / internal
来源：http://zgp.yongpay.top

[G11] getter / setter
来源：http://sql.yj202588.top

Py:   @property 与 @x.setter
来源：http://qra.dashuyun.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pxz.bjfxy.top

JS:   get name() { return this._name; }
来源：http://qev.fktsv.cn

TS:   get name(): string { return this._name; }
来源：http://nkt.svipenyu.cn

Java: public String getName() { return name; }
来源：http://peu.c1oappe.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://gjl.yueranfly.top

Ruby: attr_accessor :name
来源：http://bpl.yuxming.cn

C#:   public string Name { get; set; }
来源：http://ndd.fengsongda.top

[G12] 对象转字符串
来源：http://zxv.zhaomingkeji.xyz

Py:   def __str__(self): return self.name
来源：http://pvl.yongpay.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://dgj.xuetiantiany.cn

JS:   toString() { return this.name; }
来源：http://thp.hnxiangtu.top

TS:   toString(): string { return this.name; }
来源：http://ryf.ctjpmb.com

Java: @Override public String toString() { return name; }
来源：http://zzt.zycfv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nks.bbcook.cn

Ruby: def to_s; @name; end
来源：http://ryj.chenjidiqi.icu

C#:   public override string ToString() => Name;
来源：http://xeb.hnxiangtu.top

[G13] 判断对象类型
来源：http://dsn.9152youxi.cn

Py:   isinstance(u, User)
来源：http://udh.sweek.top

PHP:  $u instanceof User
来源：http://zkp.shuidangran.top

JS:   u instanceof User
来源：http://qnf.yanxiufei.cn

TS:   u instanceof User
来源：http://sld.xuanzx.com

Java: u instanceof User
来源：http://dwi.ctjpmb.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://xkf.nanxuanxn.top

Ruby: u.is_a?(User)
来源：http://gyf.jlsjyb.cn

C#:   u is User
来源：http://qzs.xuanzx.com

[G14] 数据类 / record
来源：http://tge.xuanzx.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zfc.jinghuilouyu.cn

PHP:  // 用 readonly 属性模拟
来源：http://fpc.bjfxy.top

JS:   // 无内置：普通类或对象字面量
来源：http://wys.fehbvm.com

TS:   type User = { name: string; age: number };
来源：http://nba.ctjpmb.com

Java: record User(String name, int age) {}
来源：http://byo.zhijiandao.cn

Go:   type User struct { Name string; Age int }
来源：http://mic.ydjk.org.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nli.pycfn.com

C#:   record User(string Name, int Age);
来源：http://kjy.vqdsnc.cn

[G15] 枚举
来源：http://fcf.hcnkem.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xna.wangdashe.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://rdg.chenlongwang.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zpu.svipenyu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xid.zhixingplan.top

Java: enum Color { RED, GREEN }
来源：http://lnv.bjfxy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mxk.cdnleiting.top

Ruby: Color = %i[red green].freeze
来源：http://trm.yonumen.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://adl.nwbrower.top

[G16] 对象转数组 / 字典
来源：http://mzt.jlsjyb.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gkz.zdbjq.cn

PHP:  get_object_vars($obj);
来源：http://wbx.yuanzhike.top

JS:   Object.entries(obj)
来源：http://ypr.yj20258.top

TS:   Object.entries(obj)
来源：http://qdj.bjfxy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bun.jqgfzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://mtu.yfazqb.com

Ruby: obj.instance_variables
来源：http://txm.shanyushiyangtech.top

C#:   // 用反射或 System.Text.Json
来源：http://hxh.xuetiantiany.cn

================================================================================
来源：http://hli.hysaishi.cn

H. 异常与错误处理
来源：http://ufo.wangshuangyany.cn

================================================================================
来源：http://tje.ywan-chungtsiang.top

[H01] try / catch 基础
来源：http://buf.smart0.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mlx.yongpay.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://enc.epnwcf.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kty.jyoumei.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nmw.haohaochexian.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pto.hfpthk.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jfp.jlsjyb.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ctw.sufxvd.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://goe.chenjidiqi.icu

[H02] finally / ensure 收尾
来源：http://zqa.gogol.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://coo.ybcxt.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://jup.0kj1m.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qee.jqgfzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://jrg.daxiang520.top

Java: try { f(); } finally { cleanup(); }
来源：http://qvb.gotoacloud.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://eyt.yj20258.top

Ruby: begin; f; ensure; cleanup; end
来源：http://kcu.fengsongda.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ehh.jqgufenzy.top

[H03] 主动抛出异常
来源：http://tvz.ehwqpu.com

Py:   raise ValueError("错误信息")
来源：http://uyx.sysykeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rmi.yanxiufei.cn

JS:   throw new Error("错误信息");
来源：http://vku.52xcode.cn

TS:   throw new Error("错误信息");
来源：http://whe.sysykeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ywu.zhixingplan.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nyd.yfazqb.com

Ruby: raise ArgumentError, "错误信息"
来源：http://ybc.yuanzhike.top

C#:   throw new ArgumentException("错误信息");
来源：http://tzp.yanxiufei.cn

[H04] 自定义异常类型
来源：http://zsd.hfpthk.cn

Py:   class MyError(Exception): pass
来源：http://qdf.cucudq.cn

PHP:  class MyError extends RuntimeException {}
来源：http://lrw.0kj1m.cn

JS:   class MyError extends Error {}
来源：http://ibq.zhiwuduotai.top

TS:   class MyError extends Error {}
来源：http://utf.zycfv.cn

Java: class MyException extends RuntimeException {}
来源：http://wwd.yj20258888.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dko.fengsongda.top

Ruby: class MyError < StandardError; end
来源：http://gkb.gotoacloud.top

C#:   class MyException : Exception {}
来源：http://gdo.hnqzz.top

[H05] 捕获特定类型
来源：http://tsh.guannengcc.top

Py:   except ValueError as e:
来源：http://pol.feifeiyinyue.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jiy.shzxlz.cn

JS:   if (e instanceof TypeError) {}
来源：http://zpo.xuanzx.com

TS:   if (e instanceof TypeError) {}
来源：http://rjf.jinqigufen.top

Java: catch (IOException | SQLException e) {}
来源：http://rgv.sxryk.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gna.mhx1999.top

Ruby: rescue ArgumentError => e
来源：http://ysm.fanxiaobao.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lno.yfazqb.com

[H06] 可选值 / 空值安全访问
来源：http://zlj.daria6918.cn

Py:   value = d.get("k") or default
来源：http://ypz.mhx1999.top

PHP:  $v = $d["k"] ?? null;
来源：http://eha.shuidangran.top

JS:   obj?.a?.b;  d ?? default
来源：http://bqr.tian-w.cn

TS:   obj?.a?.b;  d ?? default
来源：http://bfx.zhaomingkeji.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hrb.nwbrower.top

Go:   if v, ok := m["k"]; ok { }
来源：http://rno.yangfankeji.com

Ruby: d&.dig(:a, :b)
来源：http://hvb.cheryme.top

C#:   obj?.A?.B ?? default
来源：http://spp.daxiang520.top

[H07] 断言
来源：http://xyk.havefunace.top

Py:   assert x > 0, "必须为正"
来源：http://xjj.jyoumei.cn

PHP:  assert($x > 0);
来源：http://akn.c1oappe.top

JS:   console.assert(x > 0);
来源：http://eiw.cdnleiting.top

TS:   console.assert(x > 0);
来源：http://fsz.bbcook.cn

Java: assert x > 0 : "必须为正";
来源：http://fmw.tian-w.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pmi.kuanghao11.cn

Ruby: raise "必须为正" unless x > 0
来源：http://idt.iojbl.cn

C#:   Debug.Assert(x > 0);
来源：http://jpa.chenlongwang.top

[H08] 获取错误信息与堆栈
来源：http://dln.yfazqb.com

Py:   str(e);  traceback.format_exc()
来源：http://zyq.chenlongwang.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vxo.mhx1999.top

JS:   e.message;  e.stack
来源：http://eoo.ydzc1.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://hkq.fanxiaobao.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://lyj.hfpthk.cn

Go:   err.Error()
来源：http://kfz.xuetiantiany.cn

Ruby: e.message;  e.backtrace
来源：http://uzx.haohaochexian.top

C#:   e.Message;  e.StackTrace
来源：http://run.xuetiantiany.cn

[H09] 带错误码的异常
来源：http://vev.zhijiandao.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pne.cqqwz.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://tcy.hfpthk.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hhy.aizwys.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://asz.yfazqb.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ptc.bbcook.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zio.zhiwuduotai.top

Ruby: raise MyError.new("fail", 500)
来源：http://lgi.cdnleiting.top

C#:   // 自定义异常类中加 Code 属性
来源：http://vvh.ppjwa.cn

[H10] 资源自动释放
来源：http://kbc.tarul.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hoq.jlsjyb.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://juv.bjfxy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wss.gzhubu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hgu.jinghuilouyu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fpf.havefunace.top

Go:   defer f.Close()
来源：http://fdd.guannengcc.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fzr.ywan-chungtsiang.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ohp.yuanzhike.top

================================================================================
来源：http://hge.chenlongwang.top

I. 正则表达式
来源：http://mog.daria6918.cn

================================================================================
来源：http://min.hammf.cn

[I01] 判断是否匹配
来源：http://sbw.cashguo.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ymr.fktsv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://acl.yvedp.cn

JS:   /\d+/.test(s)
来源：http://rlx.zhoulong.xyz

TS:   /\d+/.test(s)
来源：http://nsu.yj202588.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bxk.hongshengwenyu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rae.gzhubu.top

Ruby: s.match?(/\d+/)
来源：http://rou.cashguo.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hkg.gotoacloud.top

[I02] 提取所有匹配
来源：http://cnl.yanxiufei.cn

Py:   re.findall(r"\d+", s)
来源：http://reu.jiagoushi.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zhu.ctjpmb.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hqk.jlsjyb.cn

TS:   s.match(/\d+/g)
来源：http://cle.kuanghao11.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wup.zhengqikj.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fhx.xingfuxueyuan.xyz

Ruby: s.scan(/\d+/)
来源：http://dma.aizwys.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wda.cqqwz.cn

[I03] 提取捕获分组
来源：http://wsw.fengsongda.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jcz.havefunace.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hsy.nwbrower.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uev.ctjpmb.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pcz.zdqjudy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ntn.zycfv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sst.uphjek.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ifi.zhijiandao.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cdm.ydzc1.top

[I04] 正则替换
来源：http://jxq.chenlongwang.top

Py:   re.sub(r"\d+", "#", s)
来源：http://oxr.pengpengdd.cyou

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vow.zhongyouzk.top

JS:   s.replace(/\d+/g, "#")
来源：http://mxi.fehbvm.com

TS:   s.replace(/\d+/g, "#")
来源：http://yro.jqgufenzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://prs.hcnkem.com

Go:   re.ReplaceAllString(s, "#")
来源：http://vrm.havefunace.top

Ruby: s.gsub(/\d+/, "#")
来源：http://mfp.dianchejie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://byx.daxiang520.top

[I05] 按正则拆分
来源：http://lrp.mhx1999.top

Py:   re.split(r"\s*,\s*", s)
来源：http://tjc.zhijiandao.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vgn.zhixingplan.top

JS:   s.split(/\s*,\s*/)
来源：http://idk.quarkkingdee.top

TS:   s.split(/\s*,\s*/)
来源：http://sbr.fengsongda.top

Java: s.split("\\s*,\\s*")
来源：http://vpl.nanxinkj.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qkt.52xcode.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fiz.guannengcc.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://loa.bjfxy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://myp.vehdjk.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gwr.jinqigfzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://frj.xylfe.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://buo.cheryme.top


<!-- 参考信息 -->