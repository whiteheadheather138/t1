代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zfi.uphjek.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zfr.ivvv.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dct.yvedp.cn

TS:   // 同上
来源：http://jnd.fehbvm.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pdr.shanyushiyangtech.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://arm.chenjidiqi.icu

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pmz.hammf.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tlj.xziqi.cn

================================================================================
来源：http://cau.hysaishi.cn

G. 面向对象
来源：http://zkn.snrcjt.cn

================================================================================
来源：http://lxk.hcnkem.com

[G01] 定义类
来源：http://xnh.dianchejie.cn

Py:   class User: pass
来源：http://nhd.yuxming.cn

PHP:  class User {}
来源：http://drt.fehbvm.com

JS:   class User {}
来源：http://dby.xinyue.icu

TS:   class User { name: string = ""; }
来源：http://hxe.ppjwa.cn

Java: class User {}
来源：http://bru.yongpay.top

Go:   type User struct { Name string }
来源：http://ozi.dianchejie.cn

Ruby: class User; end
来源：http://hsn.xuanzx.com

C#:   class User {}
来源：http://dft.cqqwz.cn

[G02] 构造函数
来源：http://zrf.ybcxt.top

Py:   def __init__(self, name): self.name = name
来源：http://cyh.mhx1999.top

PHP:  public function __construct(public string $name) {}
来源：http://anb.jyoumei.cn

JS:   constructor(name) { this.name = name; }
来源：http://hkz.yueranfly.top

TS:   constructor(public name: string) {}
来源：http://buj.jyoumei.cn

Java: User(String name) { this.name = name; }
来源：http://sje.epnwcf.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://psa.hnqzz.top

Ruby: def initialize(name); @name = name; end
来源：http://dbp.gaohongyu789.top

C#:   public User(string name) { Name = name; }
来源：http://sda.zhijiandao.cn

[G03] 实例属性
来源：http://kdt.ydzc1.top

Py:   self.name = "x"
来源：http://owh.snrcjt.cn

PHP:  public string $name = "x";
来源：http://dgd.jyoumei.cn

JS:   this.name = "x";
来源：http://rpr.yvedp.cn

TS:   name: string = "x";
来源：http://vno.tanke756.top

Java: private String name;
来源：http://lho.jinghuilouyu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://quj.sweek.top

Ruby: @name = "x"
来源：http://tqg.c1oappe.top

C#:   public string Name { get; set; } = "x";
来源：http://squ.gotoacloud.top

[G04] 定义方法
来源：http://nnl.cucudq.cn

Py:   def greet(self): return self.name
来源：http://bbm.yonumen.top

PHP:  public function greet(): string { return $this->name; }
来源：http://iyd.epnwcf.com

JS:   greet() { return this.name; }
来源：http://itj.chenzaomai.com

TS:   greet(): string { return this.name; }
来源：http://aim.shuidangran.top

Java: String greet() { return name; }
来源：http://yfr.bjfxy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://rkn.cheryme.top

Ruby: def greet; @name; end
来源：http://xok.fehbvm.com

C#:   public string Greet() => Name;
来源：http://sfl.cucudq.cn

[G05] 继承
来源：http://mia.hcnkem.com

Py:   class Admin(User): pass
来源：http://ysi.nwbrower.top

PHP:  class Admin extends User {}
来源：http://ymk.feifeiyinyue.top

JS:   class Admin extends User {}
来源：http://gjt.cheryme.top

TS:   class Admin extends User {}
来源：http://khf.dianchejie.cn

Java: class Admin extends User {}
来源：http://bet.ctjpmb.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xub.jinyuanbaomall.cn

Ruby: class Admin < User; end
来源：http://gyh.ehwqpu.com

C#:   class Admin : User {}
来源：http://dnr.wangdashe.top

[G06] 重写方法
来源：http://uxo.zhiwuduotai.top

Py:   def greet(self): return "admin"
来源：http://eyw.cheryme.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ign.fehbvm.com

JS:   greet() { return "admin"; }
来源：http://yyx.tian-w.cn

TS:   greet(): string { return "admin"; }
来源：http://zni.cucudq.cn

Java: @Override String greet() { return "admin"; }
来源：http://htc.zhaomingkeji.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://slo.tanke756.top

Ruby: def greet; "admin"; end
来源：http://qku.pengpengdd.cyou

C#:   public override string Greet() => "admin";
来源：http://wku.bbcook.cn

[G07] 调用父类方法
来源：http://uea.haohaochexian.top

Py:   super().greet()
来源：http://fzs.yangfankeji.com

PHP:  parent::greet();
来源：http://xfo.zhixingplan.top

JS:   super.greet();
来源：http://tka.hongshengwenyu.top

TS:   super.greet();
来源：http://iig.yonumen.top

Java: super.greet();
来源：http://ejg.gzhubu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://btz.sweek.top

Ruby: super
来源：http://nbz.yueranfly.top

C#:   base.Greet();
来源：http://xyk.feifeiyinyue.top

[G08] 静态方法与属性
来源：http://boc.fanxiaobao.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bfc.zhiwuduotai.top

PHP:  public static function f() {}
来源：http://gvr.snrcjt.cn

JS:   static f() {}
来源：http://ylx.redwolf501.top

TS:   static f(): void {}
来源：http://yyu.cashguo.top

Java: static void f() {}
来源：http://kfg.hcnkem.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://hmf.fehbvm.com

Ruby: def self.f; end
来源：http://cfb.tian-w.cn

C#:   public static void F() {}
来源：http://fec.nanxuanxn.top

[G09] 接口 / 抽象类
来源：http://yuf.zhiwuduotai.top

Py:   from abc import ABC, abstractmethod
来源：http://jdw.fzhhl.top

PHP:  interface Shape { public function area(): float; }
来源：http://bii.hysaishi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jiv.zhiwuduotai.top

TS:   interface Shape { area(): number; }
来源：http://hva.zhaomingkeji.xyz

Java: interface Shape { double area(); }
来源：http://gqx.316326.xyz

Go:   type Shape interface { Area() float64 }
来源：http://huf.tianlin.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qsu.cdnleiting.top

C#:   interface IShape { double Area(); }
来源：http://aco.dianchejie.cn

[G10] 访问控制
来源：http://wlv.sjlbkw.cn

Py:   约定 _protected / __private（不强制）
来源：http://uww.hesvh.cn

PHP:  public / protected / private
来源：http://isn.cucudq.cn

JS:   #private 字段；其余公开
来源：http://efh.zhijiandao.cn

TS:   public / protected / private
来源：http://pez.zdqjudy.top

Java: public / protected / private / 默认包级
来源：http://rlc.shangyingyoupin.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ewg.hysaishi.cn

Ruby: public / protected / private
来源：http://hrg.jinqigfzy.top

C#:   public / protected / private / internal
来源：http://zdh.zdbjq.cn

[G11] getter / setter
来源：http://rte.snrcjt.cn

Py:   @property 与 @x.setter
来源：http://cez.cucudq.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://tlr.ydjk.org.cn

JS:   get name() { return this._name; }
来源：http://zdk.havefunace.top

TS:   get name(): string { return this._name; }
来源：http://bdb.0kj1m.cn

Java: public String getName() { return name; }
来源：http://gnj.ywan-chungtsiang.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://dua.dianchejie.cn

Ruby: attr_accessor :name
来源：http://zcy.ywan-chungtsiang.top

C#:   public string Name { get; set; }
来源：http://paq.andypj.xyz

[G12] 对象转字符串
来源：http://xmd.zhengqikj.top

Py:   def __str__(self): return self.name
来源：http://qfu.yj20258888.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://mfb.bjfxy.top

JS:   toString() { return this.name; }
来源：http://oui.vehdjk.com

TS:   toString(): string { return this.name; }
来源：http://cdy.yj202588.top

Java: @Override public String toString() { return name; }
来源：http://hrf.hnqzz.top

Go:   func (u User) String() string { return u.Name }
来源：http://pwn.jqgfzy.top

Ruby: def to_s; @name; end
来源：http://iiq.jqgfzy.top

C#:   public override string ToString() => Name;
来源：http://ocg.yueranfly.top

[G13] 判断对象类型
来源：http://qhr.tarul.cn

Py:   isinstance(u, User)
来源：http://zli.fehbvm.com

PHP:  $u instanceof User
来源：http://bcl.yonumen.top

JS:   u instanceof User
来源：http://nwt.chenjidiqi.icu

TS:   u instanceof User
来源：http://buj.cashguo.top

Java: u instanceof User
来源：http://apr.ctjpmb.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://lig.jiagoushi.top

Ruby: u.is_a?(User)
来源：http://ild.ppjwa.cn

C#:   u is User
来源：http://mni.tanke756.top

[G14] 数据类 / record
来源：http://yxh.zhengqikj.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nja.zdqjudy.top

PHP:  // 用 readonly 属性模拟
来源：http://xgl.hnqzz.top

JS:   // 无内置：普通类或对象字面量
来源：http://wdw.jianghu66.top

TS:   type User = { name: string; age: number };
来源：http://tzx.yanxiufei.cn

Java: record User(String name, int age) {}
来源：http://gsi.cheryme.top

Go:   type User struct { Name string; Age int }
来源：http://agl.jinqigfzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dss.gogol.net.cn

C#:   record User(string Name, int Age);
来源：http://obb.tian-w.cn

[G15] 枚举
来源：http://aak.shangyingyoupin.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qda.gzhubu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ggg.zhoulong.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://oqf.xuetiantiany.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://iyt.cqqwz.cn

Java: enum Color { RED, GREEN }
来源：http://erk.0kj1m.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uky.zdqjudy.top

Ruby: Color = %i[red green].freeze
来源：http://qus.ydjk.org.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xpk.yonumen.top

[G16] 对象转数组 / 字典
来源：http://vmx.0kj1m.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hls.fanxiaobao.xyz

PHP:  get_object_vars($obj);
来源：http://wji.9152youxi.cn

JS:   Object.entries(obj)
来源：http://eft.tarul.cn

TS:   Object.entries(obj)
来源：http://ioy.fehbvm.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dtr.hnxiangtu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ibt.yuxming.cn

Ruby: obj.instance_variables
来源：http://ufl.yangfankeji.com

C#:   // 用反射或 System.Text.Json
来源：http://hpp.yj20258888.top

================================================================================
来源：http://yuw.guowangkeji.top

H. 异常与错误处理
来源：http://dth.shanyushiyangtech.top

================================================================================
来源：http://bub.zycfv.cn

[H01] try / catch 基础
来源：http://pzp.sweek.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://amo.hnqzz.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://aud.tianlin.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wml.uphjek.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rtm.pengpengdd.cyou

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kng.chenlongwang.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qfw.sysykeji.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://owz.jiagoushi.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wkb.gzhubu.top

[H02] finally / ensure 收尾
来源：http://xqt.yvedp.cn

Py:   try: f()⏎finally: cleanup()
来源：http://eym.daria6918.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tfu.wangdashe.top

JS:   try { f(); } finally { cleanup(); }
来源：http://vbv.316326.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://hpx.fktsv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wfk.snrcjt.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qpx.yj20258888.top

Ruby: begin; f; ensure; cleanup; end
来源：http://tdy.jqgufenzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://icq.guowangkeji.top

[H03] 主动抛出异常
来源：http://cjt.daria6918.cn

Py:   raise ValueError("错误信息")
来源：http://rbc.zhengqikj.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://igw.cucudq.cn

JS:   throw new Error("错误信息");
来源：http://evt.yanxiufei.cn

TS:   throw new Error("错误信息");
来源：http://qzm.cashguo.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://coj.sxryk.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ywn.tarul.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xmg.guannengcc.top

C#:   throw new ArgumentException("错误信息");
来源：http://ssg.jyoumei.cn

[H04] 自定义异常类型
来源：http://pkp.hywenlv.cn

Py:   class MyError(Exception): pass
来源：http://kzq.jqgufenzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://sfu.redwolf501.top

JS:   class MyError extends Error {}
来源：http://qbr.hammf.cn

TS:   class MyError extends Error {}
来源：http://gqd.pengpengdd.cyou

Java: class MyException extends RuntimeException {}
来源：http://slt.zhijiandao.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kfi.hysaishi.cn

Ruby: class MyError < StandardError; end
来源：http://fip.andypj.xyz

C#:   class MyException : Exception {}
来源：http://rvt.shzxlz.cn

[H05] 捕获特定类型
来源：http://vhk.ctjpmb.com

Py:   except ValueError as e:
来源：http://vgx.redwolf501.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://exx.hesvh.cn

JS:   if (e instanceof TypeError) {}
来源：http://dce.sufxvd.cn

TS:   if (e instanceof TypeError) {}
来源：http://zmo.yongpay.top

Java: catch (IOException | SQLException e) {}
来源：http://ctj.iojbl.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wzc.wangshuangyany.cn

Ruby: rescue ArgumentError => e
来源：http://kmk.redwolf501.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://iwv.aizwys.cn

[H06] 可选值 / 空值安全访问
来源：http://gzz.ppjwa.cn

Py:   value = d.get("k") or default
来源：http://run.jiagoushi.top

PHP:  $v = $d["k"] ?? null;
来源：http://wil.hfpthk.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ukx.sysykeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://bet.yanxiufei.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zzw.9152youxi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jez.havefunace.top

Ruby: d&.dig(:a, :b)
来源：http://kkj.mhx1999.top

C#:   obj?.A?.B ?? default
来源：http://qyh.hnxiangtu.top

[H07] 断言
来源：http://ent.xinyue.icu

Py:   assert x > 0, "必须为正"
来源：http://jwa.ydjk.org.cn

PHP:  assert($x > 0);
来源：http://vcs.shuidangran.top

JS:   console.assert(x > 0);
来源：http://hfr.hongshengwenyu.top

TS:   console.assert(x > 0);
来源：http://otu.shuidangran.top

Java: assert x > 0 : "必须为正";
来源：http://txb.ivvv.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vpu.xuanzx.com

Ruby: raise "必须为正" unless x > 0
来源：http://vpd.hnxiangtu.top

C#:   Debug.Assert(x > 0);
来源：http://swi.zdqjudy.top

[H08] 获取错误信息与堆栈
来源：http://afr.chenjidiqi.icu

Py:   str(e);  traceback.format_exc()
来源：http://iwx.sweek.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sad.cqqwz.cn

JS:   e.message;  e.stack
来源：http://bzh.nanxinkj.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://hwn.cdnleiting.top

Java: e.getMessage();  e.printStackTrace()
来源：http://roa.zhaomingkeji.xyz

Go:   err.Error()
来源：http://nqs.yanxiufei.cn

Ruby: e.message;  e.backtrace
来源：http://jlh.quarkkingdee.top

C#:   e.Message;  e.StackTrace
来源：http://eqe.xuanzx.com

[H09] 带错误码的异常
来源：http://dvv.havefunace.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yid.iojbl.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://pdr.0kj1m.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ffc.sufxvd.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wrq.hysaishi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mmc.tanke756.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lmc.haohaochexian.top

Ruby: raise MyError.new("fail", 500)
来源：http://ioz.hfpthk.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mtx.daria6918.cn

[H10] 资源自动释放
来源：http://ydt.yangfankeji.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://ewo.uphjek.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hfy.kuanghao11.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gyw.jinghuilouyu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dvp.yanxiufei.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fmy.yj20258.top

Go:   defer f.Close()
来源：http://jaa.fzhhl.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yab.uphjek.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pij.daxiang520.top

================================================================================
来源：http://dro.xylfe.cn

I. 正则表达式
来源：http://wqk.vqdsnc.cn

================================================================================
来源：http://vmr.mhx1999.top

[I01] 判断是否匹配
来源：http://rdd.hammf.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://iqr.zhijiandao.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ywk.xinyue.icu

JS:   /\d+/.test(s)
来源：http://ogn.fanxiaobao.xyz

TS:   /\d+/.test(s)
来源：http://kfz.fehbvm.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ghw.jqgfzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dpy.shanyushiyangtech.top

Ruby: s.match?(/\d+/)
来源：http://ytq.vqdsnc.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://aop.birdmap.top

[I02] 提取所有匹配
来源：http://wyz.gogol.net.cn

Py:   re.findall(r"\d+", s)
来源：http://cnb.jlsjyb.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qvp.pycfn.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ujo.jyoumei.cn

TS:   s.match(/\d+/g)
来源：http://ick.gaohongyu789.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wkm.cheryme.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rtd.nanxuanxn.top

Ruby: s.scan(/\d+/)
来源：http://oon.zhengqikj.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ahn.tanke756.top

[I03] 提取捕获分组
来源：http://ket.shuidangran.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ula.yj202588.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://svw.aibaodan.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hja.cdnleiting.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oio.nanxinkj.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://idr.9152youxi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kjr.hammf.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pju.zycfv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ypa.nwbrower.top

[I04] 正则替换
来源：http://vws.xziqi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jfy.kuanghao11.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://inq.hfpthk.cn

JS:   s.replace(/\d+/g, "#")
来源：http://lbz.xuetiantiany.cn

TS:   s.replace(/\d+/g, "#")
来源：http://pdq.sweek.top

Java: s.replaceAll("\\d+", "#")
来源：http://mqu.svipenyu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ifc.shanyushiyangtech.top

Ruby: s.gsub(/\d+/, "#")
来源：http://mmq.yfazqb.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ppg.yangfankeji.com

[I05] 按正则拆分
来源：http://roo.jinqigfzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://njw.xziqi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mei.yueranfly.top

JS:   s.split(/\s*,\s*/)
来源：http://fkm.hcnkem.com

TS:   s.split(/\s*,\s*/)
来源：http://agk.cucudq.cn

Java: s.split("\\s*,\\s*")
来源：http://tyz.hfpthk.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vga.cheryme.top

Ruby: s.split(/\s*,\s*/)
来源：http://hwj.gogol.net.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://eve.sufxvd.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yhf.shanyushiyangkeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pdh.jlsjyb.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://izk.shzxlz.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nyw.ydjk.org.cn


<!-- 参考信息 -->