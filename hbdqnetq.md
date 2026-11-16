代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lrb.zhongyouzk.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://law.jinqigufen.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uah.snrcjt.cn

[F12] CSV 读写
来源：http://czl.redwolf501.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hxn.zhiwuduotai.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zrm.sysykeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ymx.ivvv.top

TS:   // 同上
来源：http://pym.xylfe.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zjp.jlsjyb.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nqu.0kj1m.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wyi.gogol.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fax.xuanzx.com

================================================================================
来源：http://mfq.wangdashe.top

G. 面向对象
来源：http://hsz.quarkkingdee.top

================================================================================
来源：http://laj.shanyushiyangkeji.top

[G01] 定义类
来源：http://vwb.sjlbkw.cn

Py:   class User: pass
来源：http://ubp.yongpay.top

PHP:  class User {}
来源：http://two.cashguo.top

JS:   class User {}
来源：http://cxv.vqdsnc.cn

TS:   class User { name: string = ""; }
来源：http://vqt.hesvh.cn

Java: class User {}
来源：http://xcx.sjlbkw.cn

Go:   type User struct { Name string }
来源：http://pqw.yanxiufei.cn

Ruby: class User; end
来源：http://yut.mhx1999.top

C#:   class User {}
来源：http://sbk.iojbl.cn

[G02] 构造函数
来源：http://lqz.redwolf501.top

Py:   def __init__(self, name): self.name = name
来源：http://qgx.haohaochexian.top

PHP:  public function __construct(public string $name) {}
来源：http://qet.jlsjyb.cn

JS:   constructor(name) { this.name = name; }
来源：http://hdq.mhx1999.top

TS:   constructor(public name: string) {}
来源：http://yhs.tanke756.top

Java: User(String name) { this.name = name; }
来源：http://khs.zhiwuduotai.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zsj.birdmap.top

Ruby: def initialize(name); @name = name; end
来源：http://tay.zdqjudy.top

C#:   public User(string name) { Name = name; }
来源：http://vsz.316326.xyz

[G03] 实例属性
来源：http://orm.mhx1999.top

Py:   self.name = "x"
来源：http://iaj.xuetiantiany.cn

PHP:  public string $name = "x";
来源：http://trq.cucudq.cn

JS:   this.name = "x";
来源：http://gwm.zdbjq.cn

TS:   name: string = "x";
来源：http://kky.cashguo.top

Java: private String name;
来源：http://hxs.bjfxy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://szt.cheryme.top

Ruby: @name = "x"
来源：http://gkp.daxiang520.top

C#:   public string Name { get; set; } = "x";
来源：http://obd.tarul.cn

[G04] 定义方法
来源：http://gwp.shzxlz.cn

Py:   def greet(self): return self.name
来源：http://hgq.dianchejie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vjn.svipenyu.cn

JS:   greet() { return this.name; }
来源：http://dsw.yuanzhike.top

TS:   greet(): string { return this.name; }
来源：http://rni.yvedp.cn

Java: String greet() { return name; }
来源：http://luj.shangyingyoupin.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://oye.jinqigfzy.top

Ruby: def greet; @name; end
来源：http://tgm.havefunace.top

C#:   public string Greet() => Name;
来源：http://iks.guowangkeji.top

[G05] 继承
来源：http://nlm.wangshuangyany.cn

Py:   class Admin(User): pass
来源：http://myx.jinyuanbaomall.cn

PHP:  class Admin extends User {}
来源：http://wcd.jlsjyb.cn

JS:   class Admin extends User {}
来源：http://rrg.sufxvd.cn

TS:   class Admin extends User {}
来源：http://jpd.tian-w.cn

Java: class Admin extends User {}
来源：http://tig.ybcxt.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nyj.uphjek.com

Ruby: class Admin < User; end
来源：http://gjn.ydjk.org.cn

C#:   class Admin : User {}
来源：http://pjh.hammf.cn

[G06] 重写方法
来源：http://edi.tian-w.cn

Py:   def greet(self): return "admin"
来源：http://hou.feifeiyinyue.top

PHP:  public function greet(): string { return "admin"; }
来源：http://yuz.epnwcf.com

JS:   greet() { return "admin"; }
来源：http://skh.jinghuilouyu.cn

TS:   greet(): string { return "admin"; }
来源：http://iph.tianlin.xyz

Java: @Override String greet() { return "admin"; }
来源：http://prt.yuanzhike.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cys.chenjidiqi.icu

Ruby: def greet; "admin"; end
来源：http://hka.fehbvm.com

C#:   public override string Greet() => "admin";
来源：http://kbb.c1oappe.top

[G07] 调用父类方法
来源：http://def.hywenlv.cn

Py:   super().greet()
来源：http://wez.vehdjk.com

PHP:  parent::greet();
来源：http://dco.redwolf501.top

JS:   super.greet();
来源：http://qtf.cucudq.cn

TS:   super.greet();
来源：http://tvq.0kj1m.cn

Java: super.greet();
来源：http://oeh.svipenyu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xpw.sysykeji.top

Ruby: super
来源：http://tmx.quarkkingdee.top

C#:   base.Greet();
来源：http://nhu.hesvh.cn

[G08] 静态方法与属性
来源：http://jzf.shangyingyoupin.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hne.smart0.xyz

PHP:  public static function f() {}
来源：http://kwl.xuetiantiany.cn

JS:   static f() {}
来源：http://bml.jianghu66.top

TS:   static f(): void {}
来源：http://iun.yonumen.top

Java: static void f() {}
来源：http://hmi.andypj.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://rey.cucudq.cn

Ruby: def self.f; end
来源：http://idc.ctjpmb.com

C#:   public static void F() {}
来源：http://hnw.zhengqikj.top

[G09] 接口 / 抽象类
来源：http://crj.sweek.top

Py:   from abc import ABC, abstractmethod
来源：http://ill.shanyushiyangtech.top

PHP:  interface Shape { public function area(): float; }
来源：http://kpe.ivvv.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://gho.yj202588.top

TS:   interface Shape { area(): number; }
来源：http://irf.shangyingyoupin.top

Java: interface Shape { double area(); }
来源：http://dse.iojbl.cn

Go:   type Shape interface { Area() float64 }
来源：http://djh.cqqwz.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://iyn.aizwys.cn

C#:   interface IShape { double Area(); }
来源：http://btr.jinqigfzy.top

[G10] 访问控制
来源：http://kvn.iojbl.cn

Py:   约定 _protected / __private（不强制）
来源：http://oer.meibo888.top

PHP:  public / protected / private
来源：http://ppi.ivvv.top

JS:   #private 字段；其余公开
来源：http://kar.cashguo.top

TS:   public / protected / private
来源：http://hqu.shuidangran.top

Java: public / protected / private / 默认包级
来源：http://fah.yuxming.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://odk.fzhhl.top

Ruby: public / protected / private
来源：http://fad.hammf.cn

C#:   public / protected / private / internal
来源：http://wdj.ehwqpu.com

[G11] getter / setter
来源：http://wdu.zhijiandao.cn

Py:   @property 与 @x.setter
来源：http://uov.hcnkem.com

PHP:  public function getName(): string { return $this->name; }
来源：http://hfb.ehwqpu.com

JS:   get name() { return this._name; }
来源：http://zsq.yj20258888.top

TS:   get name(): string { return this._name; }
来源：http://rnr.fanxiaobao.xyz

Java: public String getName() { return name; }
来源：http://qnd.nanxuanxn.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://jir.shanyushiyangkeji.top

Ruby: attr_accessor :name
来源：http://khd.0kj1m.cn

C#:   public string Name { get; set; }
来源：http://nsz.zycfv.cn

[G12] 对象转字符串
来源：http://eku.guannengcc.top

Py:   def __str__(self): return self.name
来源：http://pqf.kuanghao11.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gjo.xziqi.cn

JS:   toString() { return this.name; }
来源：http://vwf.hysaishi.cn

TS:   toString(): string { return this.name; }
来源：http://kvb.daria6918.cn

Java: @Override public String toString() { return name; }
来源：http://qxr.hnqzz.top

Go:   func (u User) String() string { return u.Name }
来源：http://lrp.shuidangran.top

Ruby: def to_s; @name; end
来源：http://tgz.jinqigfzy.top

C#:   public override string ToString() => Name;
来源：http://jll.feifeiyinyue.top

[G13] 判断对象类型
来源：http://ojw.epnwcf.com

Py:   isinstance(u, User)
来源：http://uky.hysaishi.cn

PHP:  $u instanceof User
来源：http://ytz.yj202588.top

JS:   u instanceof User
来源：http://yzh.jiagoushi.top

TS:   u instanceof User
来源：http://xxe.sjlbkw.cn

Java: u instanceof User
来源：http://udw.pengpengdd.cyou

Go:   u, ok := v.(User)            // 类型断言
来源：http://tju.xuanzx.com

Ruby: u.is_a?(User)
来源：http://qxt.wangshuangyany.cn

C#:   u is User
来源：http://tnt.chenlongwang.top

[G14] 数据类 / record
来源：http://brv.yanxiufei.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://erk.tianlin.xyz

PHP:  // 用 readonly 属性模拟
来源：http://oux.guannengcc.top

JS:   // 无内置：普通类或对象字面量
来源：http://yro.hnxiangtu.top

TS:   type User = { name: string; age: number };
来源：http://ggf.sysykeji.top

Java: record User(String name, int age) {}
来源：http://mbl.yj20258.top

Go:   type User struct { Name string; Age int }
来源：http://hwf.hongshengwenyu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bxb.nanxuanxn.top

C#:   record User(string Name, int Age);
来源：http://tkz.hongshengwenyu.top

[G15] 枚举
来源：http://emk.sxryk.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vce.cheryme.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ldk.aibaodan.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ffi.meibo888.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qkd.shuidangran.top

Java: enum Color { RED, GREEN }
来源：http://xll.xingfuxueyuan.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yrq.tanke756.top

Ruby: Color = %i[red green].freeze
来源：http://vdd.ppjwa.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nug.ywan-chungtsiang.top

[G16] 对象转数组 / 字典
来源：http://jcs.shanyushiyangtech.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gjh.shuidangran.top

PHP:  get_object_vars($obj);
来源：http://enx.guowangkeji.top

JS:   Object.entries(obj)
来源：http://eaz.yfazqb.com

TS:   Object.entries(obj)
来源：http://dts.smart0.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zjp.cashguo.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://mcy.fzhhl.top

Ruby: obj.instance_variables
来源：http://npe.gaohongyu789.top

C#:   // 用反射或 System.Text.Json
来源：http://kmb.hcnkem.com

================================================================================
来源：http://xvz.daxiang520.top

H. 异常与错误处理
来源：http://dir.shangyingyoupin.top

================================================================================
来源：http://hmq.0kj1m.cn

[H01] try / catch 基础
来源：http://asl.cqqwz.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ruz.tanke756.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tnf.sufxvd.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nel.yueranfly.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fdu.quarkkingdee.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vat.jianghu66.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bdx.havefunace.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lgt.svipenyu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zhu.yangfankeji.com

[H02] finally / ensure 收尾
来源：http://cff.andypj.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://ijm.ydjk.org.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ana.ctjpmb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://bra.svipenyu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://egg.jqgufenzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://bmv.cheryme.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://qee.birdmap.top

Ruby: begin; f; ensure; cleanup; end
来源：http://dpr.fehbvm.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://tks.jinghuilouyu.cn

[H03] 主动抛出异常
来源：http://gdg.vqdsnc.cn

Py:   raise ValueError("错误信息")
来源：http://ihv.ydzc1.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://czi.gaohongyu789.top

JS:   throw new Error("错误信息");
来源：http://wst.zdbjq.cn

TS:   throw new Error("错误信息");
来源：http://zan.mhx1999.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://otp.fanxiaobao.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://aej.shanyushiyangtech.top

Ruby: raise ArgumentError, "错误信息"
来源：http://xhh.jyoumei.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gly.jinyuanbaomall.cn

[H04] 自定义异常类型
来源：http://duq.gogol.net.cn

Py:   class MyError(Exception): pass
来源：http://iyk.quarkkingdee.top

PHP:  class MyError extends RuntimeException {}
来源：http://bsh.shanyushiyangtech.top

JS:   class MyError extends Error {}
来源：http://arn.cheryme.top

TS:   class MyError extends Error {}
来源：http://hfr.yuxming.cn

Java: class MyException extends RuntimeException {}
来源：http://gdl.hnxiangtu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bmn.shanyushiyangkeji.top

Ruby: class MyError < StandardError; end
来源：http://cvx.hcnkem.com

C#:   class MyException : Exception {}
来源：http://nfe.xinyue.icu

[H05] 捕获特定类型
来源：http://obb.cashguo.top

Py:   except ValueError as e:
来源：http://oqv.hywenlv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ang.chenlongwang.top

JS:   if (e instanceof TypeError) {}
来源：http://moe.sweek.top

TS:   if (e instanceof TypeError) {}
来源：http://bqd.jyoumei.cn

Java: catch (IOException | SQLException e) {}
来源：http://zub.vqdsnc.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yaq.birdmap.top

Ruby: rescue ArgumentError => e
来源：http://juk.yfazqb.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uzw.bjfxy.top

[H06] 可选值 / 空值安全访问
来源：http://gcr.shangyingyoupin.top

Py:   value = d.get("k") or default
来源：http://eql.hongshengwenyu.top

PHP:  $v = $d["k"] ?? null;
来源：http://obx.wangdashe.top

JS:   obj?.a?.b;  d ?? default
来源：http://fje.xinyue.icu

TS:   obj?.a?.b;  d ?? default
来源：http://kco.kuanghao11.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ifp.fanxiaobao.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://int.cqqwz.cn

Ruby: d&.dig(:a, :b)
来源：http://zws.jinghuilouyu.cn

C#:   obj?.A?.B ?? default
来源：http://qmt.c1oappe.top

[H07] 断言
来源：http://xkb.fengsongda.top

Py:   assert x > 0, "必须为正"
来源：http://ira.yvedp.cn

PHP:  assert($x > 0);
来源：http://tcb.xingfuxueyuan.xyz

JS:   console.assert(x > 0);
来源：http://qux.shuidangran.top

TS:   console.assert(x > 0);
来源：http://ttl.pycfn.com

Java: assert x > 0 : "必须为正";
来源：http://kik.dashuyun.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kqu.c1oappe.top

Ruby: raise "必须为正" unless x > 0
来源：http://aeh.vqdsnc.cn

C#:   Debug.Assert(x > 0);
来源：http://ztk.daria6918.cn

[H08] 获取错误信息与堆栈
来源：http://kur.fzhhl.top

Py:   str(e);  traceback.format_exc()
来源：http://kfb.fanxiaobao.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wub.c1oappe.top

JS:   e.message;  e.stack
来源：http://vkp.jinqigufen.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://aur.meibo888.top

Java: e.getMessage();  e.printStackTrace()
来源：http://wcz.wangdashe.top

Go:   err.Error()
来源：http://zmh.xinyue.icu

Ruby: e.message;  e.backtrace
来源：http://ivc.nanxinkj.top

C#:   e.Message;  e.StackTrace
来源：http://asx.guowangkeji.top

[H09] 带错误码的异常
来源：http://chp.bjfxy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uwr.hammf.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dct.wangdashe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dws.dianchejie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jko.zycfv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://agy.yanxiufei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rdn.pycfn.com

Ruby: raise MyError.new("fail", 500)
来源：http://khu.guannengcc.top

C#:   // 自定义异常类中加 Code 属性
来源：http://pnq.ehwqpu.com

[H10] 资源自动释放
来源：http://nsi.birdmap.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://bdg.zhengqikj.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dwh.cheryme.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dwp.feifeiyinyue.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ppr.andypj.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://boj.c1oappe.top

Go:   defer f.Close()
来源：http://snx.quarkkingdee.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pvi.cucudq.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zhq.sweek.top

================================================================================
来源：http://jpz.havefunace.top

I. 正则表达式
来源：http://lol.hesvh.cn

================================================================================
来源：http://umg.gogol.net.cn

[I01] 判断是否匹配
来源：http://lba.hongshengwenyu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yfe.xinyue.icu

PHP:  preg_match('/\d+/', $s);
来源：http://bgz.jyoumei.cn

JS:   /\d+/.test(s)
来源：http://pir.shuidangran.top

TS:   /\d+/.test(s)
来源：http://dfs.52xcode.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bad.wangdashe.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mff.hesvh.cn

Ruby: s.match?(/\d+/)
来源：http://eon.xziqi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ewf.hnxiangtu.top

[I02] 提取所有匹配
来源：http://vjw.chenjidiqi.icu

Py:   re.findall(r"\d+", s)
来源：http://ebd.shuidangran.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jfr.yfazqb.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rnb.nanxuanxn.top

TS:   s.match(/\d+/g)
来源：http://gij.uphjek.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://iwx.wangdashe.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://oao.birdmap.top

Ruby: s.scan(/\d+/)
来源：http://erd.fanxiaobao.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://puk.shanyushiyangkeji.top

[I03] 提取捕获分组
来源：http://wxo.yonumen.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gkm.dianchejie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sqv.mhx1999.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ydx.cdnleiting.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lzh.guowangkeji.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xdj.cheryme.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tnu.dashuyun.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vpy.sufxvd.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ibb.hnxiangtu.top

[I04] 正则替换
来源：http://vef.birdmap.top

Py:   re.sub(r"\d+", "#", s)
来源：http://hvc.tanke756.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ren.yuxming.cn

JS:   s.replace(/\d+/g, "#")
来源：http://irs.daria6918.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ucu.chenlongwang.top

Java: s.replaceAll("\\d+", "#")
来源：http://wla.daria6918.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://mis.uphjek.com

Ruby: s.gsub(/\d+/, "#")
来源：http://jxb.iojbl.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kzg.bjfxy.top

[I05] 按正则拆分
来源：http://nbv.zdbjq.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hhz.daria6918.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://skn.zhixingplan.top

JS:   s.split(/\s*,\s*/)
来源：http://sso.52xcode.cn

TS:   s.split(/\s*,\s*/)
来源：http://krj.uphjek.com

Java: s.split("\\s*,\\s*")
来源：http://bwt.hammf.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ilj.ehwqpu.com

Ruby: s.split(/\s*,\s*/)
来源：http://yjb.316326.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qfj.sufxvd.cn


<!-- 参考信息 -->