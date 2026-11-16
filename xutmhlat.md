代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nyd.guannengcc.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zxx.aizwys.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xek.dianchejie.cn

TS:   // 同上
来源：http://ssk.nanxuanxn.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://afi.zycfv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gbh.iojbl.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://efw.gaohongyu789.top

C#:   // 无内置：用 CsvHelper 库
来源：http://zsj.guannengcc.top

================================================================================
来源：http://mxn.gaohongyu789.top

G. 面向对象
来源：http://sho.epnwcf.com

================================================================================
来源：http://qjx.jianghu66.top

[G01] 定义类
来源：http://cqr.daria6918.cn

Py:   class User: pass
来源：http://tco.hywenlv.cn

PHP:  class User {}
来源：http://tdu.shanyushiyangkeji.top

JS:   class User {}
来源：http://jau.gaohongyu789.top

TS:   class User { name: string = ""; }
来源：http://nco.jiagoushi.top

Java: class User {}
来源：http://tsc.hongshengwenyu.top

Go:   type User struct { Name string }
来源：http://ytu.guannengcc.top

Ruby: class User; end
来源：http://lbj.chenzaomai.com

C#:   class User {}
来源：http://xvs.mhx1999.top

[G02] 构造函数
来源：http://yuc.ppjwa.cn

Py:   def __init__(self, name): self.name = name
来源：http://mwz.jlsjyb.cn

PHP:  public function __construct(public string $name) {}
来源：http://qei.bjfxy.top

JS:   constructor(name) { this.name = name; }
来源：http://xdp.epnwcf.com

TS:   constructor(public name: string) {}
来源：http://slb.hnxiangtu.top

Java: User(String name) { this.name = name; }
来源：http://qsu.guowangkeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://imb.sweek.top

Ruby: def initialize(name); @name = name; end
来源：http://zat.dashuyun.cn

C#:   public User(string name) { Name = name; }
来源：http://ykz.ppjwa.cn

[G03] 实例属性
来源：http://uyk.cucudq.cn

Py:   self.name = "x"
来源：http://qvf.tanke756.top

PHP:  public string $name = "x";
来源：http://bni.hongshengwenyu.top

JS:   this.name = "x";
来源：http://hti.andypj.xyz

TS:   name: string = "x";
来源：http://vle.cheryme.top

Java: private String name;
来源：http://fqw.epnwcf.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sad.tanke756.top

Ruby: @name = "x"
来源：http://gkb.tianlin.xyz

C#:   public string Name { get; set; } = "x";
来源：http://msu.cucudq.cn

[G04] 定义方法
来源：http://sel.0kj1m.cn

Py:   def greet(self): return self.name
来源：http://lnp.bjfxy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://kos.yj20258.top

JS:   greet() { return this.name; }
来源：http://ymg.xinyue.icu

TS:   greet(): string { return this.name; }
来源：http://zmt.shanyushiyangkeji.top

Java: String greet() { return name; }
来源：http://kca.nanxinkj.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://vvf.guannengcc.top

Ruby: def greet; @name; end
来源：http://oaz.ywan-chungtsiang.top

C#:   public string Greet() => Name;
来源：http://ivo.52xcode.cn

[G05] 继承
来源：http://dty.sweek.top

Py:   class Admin(User): pass
来源：http://hnj.wangshuangyany.cn

PHP:  class Admin extends User {}
来源：http://fhs.yangfankeji.com

JS:   class Admin extends User {}
来源：http://hol.hnxiangtu.top

TS:   class Admin extends User {}
来源：http://cvd.daria6918.cn

Java: class Admin extends User {}
来源：http://hkg.ydzc1.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yui.zhoulong.xyz

Ruby: class Admin < User; end
来源：http://jgr.9152youxi.cn

C#:   class Admin : User {}
来源：http://sas.fktsv.cn

[G06] 重写方法
来源：http://aie.jlsjyb.cn

Py:   def greet(self): return "admin"
来源：http://spc.xuetiantiany.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pby.guannengcc.top

JS:   greet() { return "admin"; }
来源：http://rcg.haohaochexian.top

TS:   greet(): string { return "admin"; }
来源：http://kpc.gotoacloud.top

Java: @Override String greet() { return "admin"; }
来源：http://jbd.smart0.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ojb.vehdjk.com

Ruby: def greet; "admin"; end
来源：http://jdn.redwolf501.top

C#:   public override string Greet() => "admin";
来源：http://mbe.yanxiufei.cn

[G07] 调用父类方法
来源：http://saf.zycfv.cn

Py:   super().greet()
来源：http://ptw.tian-w.cn

PHP:  parent::greet();
来源：http://uju.sysykeji.top

JS:   super.greet();
来源：http://qfl.ppjwa.cn

TS:   super.greet();
来源：http://iqj.zdqjudy.top

Java: super.greet();
来源：http://jwf.9152youxi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wnb.redwolf501.top

Ruby: super
来源：http://tmp.c1oappe.top

C#:   base.Greet();
来源：http://lhz.gzhubu.top

[G08] 静态方法与属性
来源：http://vmn.xylfe.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ldz.nwbrower.top

PHP:  public static function f() {}
来源：http://mzr.cqqwz.cn

JS:   static f() {}
来源：http://dss.birdmap.top

TS:   static f(): void {}
来源：http://dxr.zhaomingkeji.xyz

Java: static void f() {}
来源：http://kol.fengsongda.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://khp.ctjpmb.com

Ruby: def self.f; end
来源：http://hco.0kj1m.cn

C#:   public static void F() {}
来源：http://bkg.svipenyu.cn

[G09] 接口 / 抽象类
来源：http://wsl.yvedp.cn

Py:   from abc import ABC, abstractmethod
来源：http://fvn.yfazqb.com

PHP:  interface Shape { public function area(): float; }
来源：http://eml.vqdsnc.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zbj.yueranfly.top

TS:   interface Shape { area(): number; }
来源：http://vea.daxiang520.top

Java: interface Shape { double area(); }
来源：http://mmg.c1oappe.top

Go:   type Shape interface { Area() float64 }
来源：http://fem.shuidangran.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mfi.quarkkingdee.top

C#:   interface IShape { double Area(); }
来源：http://luk.ctjpmb.com

[G10] 访问控制
来源：http://gbt.yvedp.cn

Py:   约定 _protected / __private（不强制）
来源：http://mbj.fengsongda.top

PHP:  public / protected / private
来源：http://nqk.chenlongwang.top

JS:   #private 字段；其余公开
来源：http://nuj.gaohongyu789.top

TS:   public / protected / private
来源：http://jgk.iojbl.cn

Java: public / protected / private / 默认包级
来源：http://tyf.ybcxt.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://udh.ydzc1.top

Ruby: public / protected / private
来源：http://siw.sysykeji.top

C#:   public / protected / private / internal
来源：http://jyc.jinghuilouyu.cn

[G11] getter / setter
来源：http://veo.uphjek.com

Py:   @property 与 @x.setter
来源：http://knu.nwbrower.top

PHP:  public function getName(): string { return $this->name; }
来源：http://irz.guowangkeji.top

JS:   get name() { return this._name; }
来源：http://zlp.havefunace.top

TS:   get name(): string { return this._name; }
来源：http://gjw.jqgfzy.top

Java: public String getName() { return name; }
来源：http://hub.mhx1999.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://jdq.chenlongwang.top

Ruby: attr_accessor :name
来源：http://tcg.hfpthk.cn

C#:   public string Name { get; set; }
来源：http://vcs.hfpthk.cn

[G12] 对象转字符串
来源：http://hgo.cucudq.cn

Py:   def __str__(self): return self.name
来源：http://ufd.ybcxt.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ygp.zhixingplan.top

JS:   toString() { return this.name; }
来源：http://mxq.cheryme.top

TS:   toString(): string { return this.name; }
来源：http://pjq.pengpengdd.cyou

Java: @Override public String toString() { return name; }
来源：http://fqw.birdmap.top

Go:   func (u User) String() string { return u.Name }
来源：http://xyx.svipenyu.cn

Ruby: def to_s; @name; end
来源：http://dxg.bjfxy.top

C#:   public override string ToString() => Name;
来源：http://sqd.iojbl.cn

[G13] 判断对象类型
来源：http://qzp.tanke756.top

Py:   isinstance(u, User)
来源：http://ycd.zdqjudy.top

PHP:  $u instanceof User
来源：http://puq.hammf.cn

JS:   u instanceof User
来源：http://hsk.hesvh.cn

TS:   u instanceof User
来源：http://qyf.zhijiandao.cn

Java: u instanceof User
来源：http://hch.tianlin.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://uri.xinyue.icu

Ruby: u.is_a?(User)
来源：http://ysd.mhx1999.top

C#:   u is User
来源：http://lci.xuanzx.com

[G14] 数据类 / record
来源：http://fjk.smart0.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://chz.kuanghao11.cn

PHP:  // 用 readonly 属性模拟
来源：http://lnc.yfazqb.com

JS:   // 无内置：普通类或对象字面量
来源：http://zyz.zhongyouzk.top

TS:   type User = { name: string; age: number };
来源：http://pqc.uphjek.com

Java: record User(String name, int age) {}
来源：http://kny.zdbjq.cn

Go:   type User struct { Name string; Age int }
来源：http://ekt.52xcode.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tkt.fktsv.cn

C#:   record User(string Name, int Age);
来源：http://rfm.316326.xyz

[G15] 枚举
来源：http://hmg.cqqwz.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://odz.xinyue.icu

PHP:  enum Color: string { case Red = "red"; }
来源：http://jgr.xuetiantiany.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zso.yj20258.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cbx.fzhhl.top

Java: enum Color { RED, GREEN }
来源：http://dim.zhoulong.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kba.yanxiufei.cn

Ruby: Color = %i[red green].freeze
来源：http://ict.cheryme.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zhu.yongpay.top

[G16] 对象转数组 / 字典
来源：http://mip.zhiwuduotai.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lks.shangyingyoupin.top

PHP:  get_object_vars($obj);
来源：http://abi.snrcjt.cn

JS:   Object.entries(obj)
来源：http://csh.redwolf501.top

TS:   Object.entries(obj)
来源：http://pct.shangyingyoupin.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yxq.nwbrower.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://pge.hcnkem.com

Ruby: obj.instance_variables
来源：http://oab.meibo888.top

C#:   // 用反射或 System.Text.Json
来源：http://vtw.yuxming.cn

================================================================================
来源：http://zhr.bbcook.cn

H. 异常与错误处理
来源：http://cqv.ydzc1.top

================================================================================
来源：http://rix.sysykeji.top

[H01] try / catch 基础
来源：http://aiq.haohaochexian.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gbj.ctjpmb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jwm.zhixingplan.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bav.pengpengdd.cyou

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gwg.nanxuanxn.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hqk.chenjidiqi.icu

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lqc.gotoacloud.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fhx.havefunace.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ijt.daxiang520.top

[H02] finally / ensure 收尾
来源：http://xxp.xziqi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ipy.xziqi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gtg.cqqwz.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jjz.zhoulong.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://rbo.hammf.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ucf.uphjek.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://iga.cqqwz.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pzz.sjlbkw.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lsc.tianlin.xyz

[H03] 主动抛出异常
来源：http://ozf.ppjwa.cn

Py:   raise ValueError("错误信息")
来源：http://imh.nanxinkj.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qit.chenlongwang.top

JS:   throw new Error("错误信息");
来源：http://ccd.yueranfly.top

TS:   throw new Error("错误信息");
来源：http://vlh.fengsongda.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://uhl.andypj.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tcx.chenjidiqi.icu

Ruby: raise ArgumentError, "错误信息"
来源：http://xqs.gzhubu.top

C#:   throw new ArgumentException("错误信息");
来源：http://nvq.aibaodan.cn

[H04] 自定义异常类型
来源：http://gjp.nanxuanxn.top

Py:   class MyError(Exception): pass
来源：http://cwv.yvedp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://evq.jianghu66.top

JS:   class MyError extends Error {}
来源：http://yho.havefunace.top

TS:   class MyError extends Error {}
来源：http://cnr.havefunace.top

Java: class MyException extends RuntimeException {}
来源：http://abo.xziqi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tzs.fktsv.cn

Ruby: class MyError < StandardError; end
来源：http://zfg.guannengcc.top

C#:   class MyException : Exception {}
来源：http://fes.meibo888.top

[H05] 捕获特定类型
来源：http://cly.9152youxi.cn

Py:   except ValueError as e:
来源：http://ihu.zhixingplan.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fqe.tanke756.top

JS:   if (e instanceof TypeError) {}
来源：http://dts.vehdjk.com

TS:   if (e instanceof TypeError) {}
来源：http://icx.nanxinkj.top

Java: catch (IOException | SQLException e) {}
来源：http://jjz.dianchejie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://luu.zhiwuduotai.top

Ruby: rescue ArgumentError => e
来源：http://dtt.jianghu66.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dod.gaohongyu789.top

[H06] 可选值 / 空值安全访问
来源：http://vnn.zhoulong.xyz

Py:   value = d.get("k") or default
来源：http://mkq.daxiang520.top

PHP:  $v = $d["k"] ?? null;
来源：http://gqp.hesvh.cn

JS:   obj?.a?.b;  d ?? default
来源：http://thi.yongpay.top

TS:   obj?.a?.b;  d ?? default
来源：http://trh.jinyuanbaomall.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://etq.9152youxi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://iyd.shuidangran.top

Ruby: d&.dig(:a, :b)
来源：http://ozq.wangshuangyany.cn

C#:   obj?.A?.B ?? default
来源：http://krx.52xcode.cn

[H07] 断言
来源：http://zzw.hesvh.cn

Py:   assert x > 0, "必须为正"
来源：http://tiv.yfazqb.com

PHP:  assert($x > 0);
来源：http://xpb.hywenlv.cn

JS:   console.assert(x > 0);
来源：http://qhm.zhongyouzk.top

TS:   console.assert(x > 0);
来源：http://mgc.vqdsnc.cn

Java: assert x > 0 : "必须为正";
来源：http://jqo.ydjk.org.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dho.zhongyouzk.top

Ruby: raise "必须为正" unless x > 0
来源：http://bsb.cashguo.top

C#:   Debug.Assert(x > 0);
来源：http://qpk.hongshengwenyu.top

[H08] 获取错误信息与堆栈
来源：http://yxl.pengpengdd.cyou

Py:   str(e);  traceback.format_exc()
来源：http://pdi.zhijiandao.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oql.guowangkeji.top

JS:   e.message;  e.stack
来源：http://qvx.haohaochexian.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://vxt.fengsongda.top

Java: e.getMessage();  e.printStackTrace()
来源：http://cle.zdbjq.cn

Go:   err.Error()
来源：http://fzu.epnwcf.com

Ruby: e.message;  e.backtrace
来源：http://cni.shangyingyoupin.top

C#:   e.Message;  e.StackTrace
来源：http://rlv.pycfn.com

[H09] 带错误码的异常
来源：http://cuh.dashuyun.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pca.tian-w.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qog.hnxiangtu.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vmw.ydjk.org.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wod.dianchejie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lqw.yongpay.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qrd.cqqwz.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qhl.zhoulong.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://npo.jinqigufen.top

[H10] 资源自动释放
来源：http://tio.yangfankeji.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://kbu.zhoulong.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sbr.hnqzz.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kqr.nwbrower.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://skd.sysykeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://icv.cucudq.cn

Go:   defer f.Close()
来源：http://gsk.haohaochexian.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lqe.chenjidiqi.icu

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pbn.hysaishi.cn

================================================================================
来源：http://koi.yj202588.top

I. 正则表达式
来源：http://uwg.zhongyouzk.top

================================================================================
来源：http://qpr.uphjek.com

[I01] 判断是否匹配
来源：http://eyf.yfazqb.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pij.ivvv.top

PHP:  preg_match('/\d+/', $s);
来源：http://mpz.jinghuilouyu.cn

JS:   /\d+/.test(s)
来源：http://hjk.smart0.xyz

TS:   /\d+/.test(s)
来源：http://znf.ywan-chungtsiang.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dev.hongshengwenyu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kss.kuanghao11.cn

Ruby: s.match?(/\d+/)
来源：http://sux.havefunace.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mnb.cheryme.top

[I02] 提取所有匹配
来源：http://qgr.shanyushiyangtech.top

Py:   re.findall(r"\d+", s)
来源：http://htj.hfpthk.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lzw.zhaomingkeji.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://teb.sysykeji.top

TS:   s.match(/\d+/g)
来源：http://qky.jinqigufen.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hzn.hcnkem.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rkq.aizwys.cn

Ruby: s.scan(/\d+/)
来源：http://avo.sufxvd.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://abu.hnxiangtu.top

[I03] 提取捕获分组
来源：http://hka.kuanghao11.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rsc.0kj1m.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://smt.birdmap.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://axr.cucudq.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gfc.sxryk.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://szq.ydzc1.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://elb.xinyue.icu

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qse.gaohongyu789.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gha.yanxiufei.cn

[I04] 正则替换
来源：http://vcn.zdbjq.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ofm.zycfv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nuo.havefunace.top

JS:   s.replace(/\d+/g, "#")
来源：http://olz.gogol.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lri.0kj1m.cn

Java: s.replaceAll("\\d+", "#")
来源：http://crr.xylfe.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://uln.fktsv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://frg.feifeiyinyue.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vhj.zhixingplan.top

[I05] 按正则拆分
来源：http://xuw.daxiang520.top

Py:   re.split(r"\s*,\s*", s)
来源：http://roh.feifeiyinyue.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bvh.cdnleiting.top

JS:   s.split(/\s*,\s*/)
来源：http://xpb.zhaomingkeji.xyz

TS:   s.split(/\s*,\s*/)
来源：http://cbe.bbcook.cn

Java: s.split("\\s*,\\s*")
来源：http://zjh.guannengcc.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cnz.vehdjk.com

Ruby: s.split(/\s*,\s*/)
来源：http://qny.yonumen.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fiz.bjfxy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ona.316326.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mhj.chenlongwang.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xdf.havefunace.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://enu.zdbjq.cn


<!-- 参考信息 -->