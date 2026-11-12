代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gkd.jlsjyb.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://suh.yj20258.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ldc.yangfankeji.com

[F12] CSV 读写
来源：http://pgo.yj202588.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gss.cheryme.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kso.ydjk.org.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://txp.sufxvd.cn

TS:   // 同上
来源：http://yac.ctjpmb.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iqs.yuanzhike.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bcl.jianghu66.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qom.tanke756.top

C#:   // 无内置：用 CsvHelper 库
来源：http://jzx.52xcode.cn

================================================================================
来源：http://scl.nanxinkj.top

G. 面向对象
来源：http://bjo.daxiang520.top

================================================================================
来源：http://agt.feifeiyinyue.top

[G01] 定义类
来源：http://zfb.jinqigfzy.top

Py:   class User: pass
来源：http://hwp.yvedp.cn

PHP:  class User {}
来源：http://pdb.yonumen.top

JS:   class User {}
来源：http://ojz.gogol.net.cn

TS:   class User { name: string = ""; }
来源：http://ehl.c1oappe.top

Java: class User {}
来源：http://ssr.c1oappe.top

Go:   type User struct { Name string }
来源：http://cfu.svipenyu.cn

Ruby: class User; end
来源：http://mxm.fanxiaobao.xyz

C#:   class User {}
来源：http://jsm.fzhhl.top

[G02] 构造函数
来源：http://gql.jinyuanbaomall.cn

Py:   def __init__(self, name): self.name = name
来源：http://sxh.daria6918.cn

PHP:  public function __construct(public string $name) {}
来源：http://sim.ivvv.top

JS:   constructor(name) { this.name = name; }
来源：http://inj.vehdjk.com

TS:   constructor(public name: string) {}
来源：http://dib.redwolf501.top

Java: User(String name) { this.name = name; }
来源：http://qdq.tianlin.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://eab.yuanzhike.top

Ruby: def initialize(name); @name = name; end
来源：http://xxs.yanxiufei.cn

C#:   public User(string name) { Name = name; }
来源：http://ckc.shzxlz.cn

[G03] 实例属性
来源：http://dva.birdmap.top

Py:   self.name = "x"
来源：http://gun.0kj1m.cn

PHP:  public string $name = "x";
来源：http://tiy.zhixingplan.top

JS:   this.name = "x";
来源：http://unt.sxryk.cn

TS:   name: string = "x";
来源：http://svv.fengsongda.top

Java: private String name;
来源：http://nnx.yangfankeji.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vgx.zhongyouzk.top

Ruby: @name = "x"
来源：http://spi.zhoulong.xyz

C#:   public string Name { get; set; } = "x";
来源：http://cwz.ctjpmb.com

[G04] 定义方法
来源：http://nnc.ctjpmb.com

Py:   def greet(self): return self.name
来源：http://aob.dashuyun.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mpi.zhijiandao.cn

JS:   greet() { return this.name; }
来源：http://bij.hesvh.cn

TS:   greet(): string { return this.name; }
来源：http://zrc.cheryme.top

Java: String greet() { return name; }
来源：http://rgf.bbcook.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vmp.shanyushiyangtech.top

Ruby: def greet; @name; end
来源：http://scu.iojbl.cn

C#:   public string Greet() => Name;
来源：http://xuz.9152youxi.cn

[G05] 继承
来源：http://jit.birdmap.top

Py:   class Admin(User): pass
来源：http://ein.iojbl.cn

PHP:  class Admin extends User {}
来源：http://btg.yongpay.top

JS:   class Admin extends User {}
来源：http://tva.cucudq.cn

TS:   class Admin extends User {}
来源：http://zyx.zhiwuduotai.top

Java: class Admin extends User {}
来源：http://bgy.shzxlz.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rvh.jqgfzy.top

Ruby: class Admin < User; end
来源：http://pqt.xinyue.icu

C#:   class Admin : User {}
来源：http://onf.xinyue.icu

[G06] 重写方法
来源：http://bxb.xylfe.cn

Py:   def greet(self): return "admin"
来源：http://suy.iojbl.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://oqv.zhoulong.xyz

JS:   greet() { return "admin"; }
来源：http://grf.uphjek.com

TS:   greet(): string { return "admin"; }
来源：http://nvc.daxiang520.top

Java: @Override String greet() { return "admin"; }
来源：http://xvr.shangyingyoupin.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fhl.fanxiaobao.xyz

Ruby: def greet; "admin"; end
来源：http://hlb.tian-w.cn

C#:   public override string Greet() => "admin";
来源：http://tvq.sysykeji.top

[G07] 调用父类方法
来源：http://iqz.yj20258888.top

Py:   super().greet()
来源：http://wdb.chenzaomai.com

PHP:  parent::greet();
来源：http://atg.cheryme.top

JS:   super.greet();
来源：http://scf.zdbjq.cn

TS:   super.greet();
来源：http://ryl.9152youxi.cn

Java: super.greet();
来源：http://gkf.yangfankeji.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ray.shzxlz.cn

Ruby: super
来源：http://knr.svipenyu.cn

C#:   base.Greet();
来源：http://qoi.cdnleiting.top

[G08] 静态方法与属性
来源：http://rvs.tanke756.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://elf.jinqigfzy.top

PHP:  public static function f() {}
来源：http://iti.aibaodan.cn

JS:   static f() {}
来源：http://fzq.yangfankeji.com

TS:   static f(): void {}
来源：http://rir.ydzc1.top

Java: static void f() {}
来源：http://fmb.guannengcc.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://zhs.gzhubu.top

Ruby: def self.f; end
来源：http://vzp.wangdashe.top

C#:   public static void F() {}
来源：http://fbg.tianlin.xyz

[G09] 接口 / 抽象类
来源：http://iao.xingfuxueyuan.xyz

Py:   from abc import ABC, abstractmethod
来源：http://gtk.yangfankeji.com

PHP:  interface Shape { public function area(): float; }
来源：http://qnp.sysykeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ghh.ybcxt.top

TS:   interface Shape { area(): number; }
来源：http://nae.fanxiaobao.xyz

Java: interface Shape { double area(); }
来源：http://ifi.hywenlv.cn

Go:   type Shape interface { Area() float64 }
来源：http://twq.ywan-chungtsiang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vot.epnwcf.com

C#:   interface IShape { double Area(); }
来源：http://lde.uphjek.com

[G10] 访问控制
来源：http://jgf.fanxiaobao.xyz

Py:   约定 _protected / __private（不强制）
来源：http://vsx.pengpengdd.cyou

PHP:  public / protected / private
来源：http://djq.xylfe.cn

JS:   #private 字段；其余公开
来源：http://vuj.316326.xyz

TS:   public / protected / private
来源：http://laf.shangyingyoupin.top

Java: public / protected / private / 默认包级
来源：http://mhb.nwbrower.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ngw.xziqi.cn

Ruby: public / protected / private
来源：http://fhk.sufxvd.cn

C#:   public / protected / private / internal
来源：http://rnm.zhengqikj.top

[G11] getter / setter
来源：http://zjy.ydzc1.top

Py:   @property 与 @x.setter
来源：http://ynm.jianghu66.top

PHP:  public function getName(): string { return $this->name; }
来源：http://srx.zhixingplan.top

JS:   get name() { return this._name; }
来源：http://yur.xylfe.cn

TS:   get name(): string { return this._name; }
来源：http://koh.gzhubu.top

Java: public String getName() { return name; }
来源：http://pdk.yueranfly.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://wsh.tian-w.cn

Ruby: attr_accessor :name
来源：http://hst.pycfn.com

C#:   public string Name { get; set; }
来源：http://ytx.ybcxt.top

[G12] 对象转字符串
来源：http://lir.fzhhl.top

Py:   def __str__(self): return self.name
来源：http://pel.nanxinkj.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://fxv.kuanghao11.cn

JS:   toString() { return this.name; }
来源：http://nlo.bjfxy.top

TS:   toString(): string { return this.name; }
来源：http://jqa.xuanzx.com

Java: @Override public String toString() { return name; }
来源：http://xch.ivvv.top

Go:   func (u User) String() string { return u.Name }
来源：http://ryl.hysaishi.cn

Ruby: def to_s; @name; end
来源：http://hok.yj20258.top

C#:   public override string ToString() => Name;
来源：http://yhl.zhongyouzk.top

[G13] 判断对象类型
来源：http://pzv.shangyingyoupin.top

Py:   isinstance(u, User)
来源：http://ooj.jqgfzy.top

PHP:  $u instanceof User
来源：http://huq.birdmap.top

JS:   u instanceof User
来源：http://iqo.pengpengdd.cyou

TS:   u instanceof User
来源：http://wai.wangdashe.top

Java: u instanceof User
来源：http://pkz.redwolf501.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://bju.haohaochexian.top

Ruby: u.is_a?(User)
来源：http://rtq.sjlbkw.cn

C#:   u is User
来源：http://pxf.hnqzz.top

[G14] 数据类 / record
来源：http://tyn.sweek.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://drr.shangyingyoupin.top

PHP:  // 用 readonly 属性模拟
来源：http://que.aizwys.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kox.gaohongyu789.top

TS:   type User = { name: string; age: number };
来源：http://rsi.yvedp.cn

Java: record User(String name, int age) {}
来源：http://ajj.shanyushiyangtech.top

Go:   type User struct { Name string; Age int }
来源：http://qjn.chenlongwang.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hzt.cashguo.top

C#:   record User(string Name, int Age);
来源：http://qrj.jianghu66.top

[G15] 枚举
来源：http://dla.52xcode.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hkj.yangfankeji.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://mzx.shuidangran.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ifw.jqgufenzy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tlb.zhijiandao.cn

Java: enum Color { RED, GREEN }
来源：http://pba.jiagoushi.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xwa.xziqi.cn

Ruby: Color = %i[red green].freeze
来源：http://wvg.wangdashe.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gaj.yanxiufei.cn

[G16] 对象转数组 / 字典
来源：http://ipy.ivvv.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rcg.uphjek.com

PHP:  get_object_vars($obj);
来源：http://cuh.jqgufenzy.top

JS:   Object.entries(obj)
来源：http://jeb.sysykeji.top

TS:   Object.entries(obj)
来源：http://gur.shanyushiyangkeji.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fbf.c1oappe.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://txk.jinghuilouyu.cn

Ruby: obj.instance_variables
来源：http://gdp.fehbvm.com

C#:   // 用反射或 System.Text.Json
来源：http://yhv.ehwqpu.com

================================================================================
来源：http://hax.yj202588.top

H. 异常与错误处理
来源：http://ujv.yueranfly.top

================================================================================
来源：http://syz.meibo888.top

[H01] try / catch 基础
来源：http://mxk.zhixingplan.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ecm.sxryk.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jpo.yueranfly.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hab.52xcode.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ppz.sysykeji.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zsc.yanxiufei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://loz.zdqjudy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://arw.hnxiangtu.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://urd.mhx1999.top

[H02] finally / ensure 收尾
来源：http://bxm.gotoacloud.top

Py:   try: f()⏎finally: cleanup()
来源：http://kzf.zhixingplan.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://wxy.yuxming.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tqk.tianlin.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://jew.vehdjk.com

Java: try { f(); } finally { cleanup(); }
来源：http://hca.andypj.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://rxh.cdnleiting.top

Ruby: begin; f; ensure; cleanup; end
来源：http://pnz.hfpthk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wip.yangfankeji.com

[H03] 主动抛出异常
来源：http://ycz.ydjk.org.cn

Py:   raise ValueError("错误信息")
来源：http://ywr.guannengcc.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zxr.shanyushiyangkeji.top

JS:   throw new Error("错误信息");
来源：http://qeo.xuanzx.com

TS:   throw new Error("错误信息");
来源：http://fcu.aizwys.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lru.hongshengwenyu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jko.jinqigufen.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ibc.shanyushiyangkeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://lyb.ybcxt.top

[H04] 自定义异常类型
来源：http://fus.zhengqikj.top

Py:   class MyError(Exception): pass
来源：http://ckx.fehbvm.com

PHP:  class MyError extends RuntimeException {}
来源：http://aji.ehwqpu.com

JS:   class MyError extends Error {}
来源：http://nhh.gotoacloud.top

TS:   class MyError extends Error {}
来源：http://pei.9152youxi.cn

Java: class MyException extends RuntimeException {}
来源：http://dwj.meibo888.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nny.svipenyu.cn

Ruby: class MyError < StandardError; end
来源：http://wxz.gotoacloud.top

C#:   class MyException : Exception {}
来源：http://jcy.iojbl.cn

[H05] 捕获特定类型
来源：http://rco.ydjk.org.cn

Py:   except ValueError as e:
来源：http://vve.epnwcf.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ubk.uphjek.com

JS:   if (e instanceof TypeError) {}
来源：http://gko.fzhhl.top

TS:   if (e instanceof TypeError) {}
来源：http://qfl.cashguo.top

Java: catch (IOException | SQLException e) {}
来源：http://eaz.jiagoushi.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zwg.fehbvm.com

Ruby: rescue ArgumentError => e
来源：http://qdh.0kj1m.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dkw.nanxuanxn.top

[H06] 可选值 / 空值安全访问
来源：http://weu.wangdashe.top

Py:   value = d.get("k") or default
来源：http://gkt.hfpthk.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rcy.epnwcf.com

JS:   obj?.a?.b;  d ?? default
来源：http://ydl.chenjidiqi.icu

TS:   obj?.a?.b;  d ?? default
来源：http://rym.hnxiangtu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jvt.nanxinkj.top

Go:   if v, ok := m["k"]; ok { }
来源：http://awb.haohaochexian.top

Ruby: d&.dig(:a, :b)
来源：http://hjt.chenjidiqi.icu

C#:   obj?.A?.B ?? default
来源：http://eox.yangfankeji.com

[H07] 断言
来源：http://qmk.sysykeji.top

Py:   assert x > 0, "必须为正"
来源：http://dze.zhaomingkeji.xyz

PHP:  assert($x > 0);
来源：http://lyw.zhixingplan.top

JS:   console.assert(x > 0);
来源：http://ail.hnqzz.top

TS:   console.assert(x > 0);
来源：http://qdi.gaohongyu789.top

Java: assert x > 0 : "必须为正";
来源：http://jts.jianghu66.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vkw.zhoulong.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://ans.jlsjyb.cn

C#:   Debug.Assert(x > 0);
来源：http://enx.nwbrower.top

[H08] 获取错误信息与堆栈
来源：http://gtl.shanyushiyangkeji.top

Py:   str(e);  traceback.format_exc()
来源：http://uth.zycfv.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://klq.jinghuilouyu.cn

JS:   e.message;  e.stack
来源：http://ddn.cucudq.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ytt.vqdsnc.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cht.ehwqpu.com

Go:   err.Error()
来源：http://sjo.sxryk.cn

Ruby: e.message;  e.backtrace
来源：http://fig.shanyushiyangkeji.top

C#:   e.Message;  e.StackTrace
来源：http://uol.havefunace.top

[H09] 带错误码的异常
来源：http://cpp.dashuyun.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://opw.pycfn.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://rsb.tianlin.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fdq.fktsv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dvb.xingfuxueyuan.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rkn.daxiang520.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nft.xuanzx.com

Ruby: raise MyError.new("fail", 500)
来源：http://bnp.zdqjudy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://apj.birdmap.top

[H10] 资源自动释放
来源：http://kre.jyoumei.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://oup.chenzaomai.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yeo.yfazqb.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uvn.gzhubu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://itc.cqqwz.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ana.zhongyouzk.top

Go:   defer f.Close()
来源：http://lpf.zhiwuduotai.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rtt.xuanzx.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xke.jinyuanbaomall.cn

================================================================================
来源：http://vqh.ybcxt.top

I. 正则表达式
来源：http://kkx.haohaochexian.top

================================================================================
来源：http://yiq.zhijiandao.cn

[I01] 判断是否匹配
来源：http://yte.pengpengdd.cyou

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bph.fengsongda.top

PHP:  preg_match('/\d+/', $s);
来源：http://hqe.feifeiyinyue.top

JS:   /\d+/.test(s)
来源：http://rlt.0kj1m.cn

TS:   /\d+/.test(s)
来源：http://meb.chenlongwang.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://acn.jiagoushi.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vil.chenzaomai.com

Ruby: s.match?(/\d+/)
来源：http://gzv.zdbjq.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vdt.guannengcc.top

[I02] 提取所有匹配
来源：http://cwv.cashguo.top

Py:   re.findall(r"\d+", s)
来源：http://qxn.hnqzz.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tyt.yuxming.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://aic.shanyushiyangtech.top

TS:   s.match(/\d+/g)
来源：http://hck.shanyushiyangkeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wle.jyoumei.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mlo.yongpay.top

Ruby: s.scan(/\d+/)
来源：http://bas.shanyushiyangkeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gls.shuidangran.top

[I03] 提取捕获分组
来源：http://urs.dashuyun.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dpf.gotoacloud.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tzv.meibo888.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kru.jiagoushi.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fig.xylfe.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ikm.andypj.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ano.yj20258.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wvr.ydjk.org.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ejw.feifeiyinyue.top

[I04] 正则替换
来源：http://yex.pycfn.com

Py:   re.sub(r"\d+", "#", s)
来源：http://muk.shanyushiyangtech.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://poa.shanyushiyangkeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://kjl.zdbjq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ahu.zdbjq.cn

Java: s.replaceAll("\\d+", "#")
来源：http://iif.chenlongwang.top

Go:   re.ReplaceAllString(s, "#")
来源：http://eht.uphjek.com

Ruby: s.gsub(/\d+/, "#")
来源：http://cmk.wangdashe.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qjl.yueranfly.top

[I05] 按正则拆分
来源：http://uuh.cqqwz.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rbu.havefunace.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://obc.vehdjk.com

JS:   s.split(/\s*,\s*/)
来源：http://ngm.havefunace.top

TS:   s.split(/\s*,\s*/)
来源：http://ufn.tian-w.cn

Java: s.split("\\s*,\\s*")
来源：http://dch.jinqigfzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rze.gzhubu.top

Ruby: s.split(/\s*,\s*/)
来源：http://fad.0kj1m.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cbb.yongpay.top


<!-- 参考信息 -->