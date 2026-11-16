代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tqr.wangdashe.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gjf.tarul.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wej.xuetiantiany.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jaw.xziqi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kmo.andypj.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nvw.hysaishi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://htg.tanke756.top

[F12] CSV 读写
来源：http://dvc.uphjek.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kur.iojbl.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://chx.epnwcf.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pgx.pycfn.com

TS:   // 同上
来源：http://ozf.ctjpmb.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gwh.pengpengdd.cyou

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://feb.hysaishi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xib.svipenyu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://coo.cashguo.top

================================================================================
来源：http://rwx.gaohongyu789.top

G. 面向对象
来源：http://rsg.shuidangran.top

================================================================================
来源：http://cxk.chenlongwang.top

[G01] 定义类
来源：http://nrk.yongpay.top

Py:   class User: pass
来源：http://xmk.xinyue.icu

PHP:  class User {}
来源：http://cqv.daria6918.cn

JS:   class User {}
来源：http://ybs.dashuyun.cn

TS:   class User { name: string = ""; }
来源：http://gqw.cqqwz.cn

Java: class User {}
来源：http://wxh.mhx1999.top

Go:   type User struct { Name string }
来源：http://fmn.vqdsnc.cn

Ruby: class User; end
来源：http://zaf.ywan-chungtsiang.top

C#:   class User {}
来源：http://dwo.aibaodan.cn

[G02] 构造函数
来源：http://nnz.gzhubu.top

Py:   def __init__(self, name): self.name = name
来源：http://wtj.yangfankeji.com

PHP:  public function __construct(public string $name) {}
来源：http://zou.guowangkeji.top

JS:   constructor(name) { this.name = name; }
来源：http://yyj.aizwys.cn

TS:   constructor(public name: string) {}
来源：http://iew.xuetiantiany.cn

Java: User(String name) { this.name = name; }
来源：http://cno.ydjk.org.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ieu.shanyushiyangkeji.top

Ruby: def initialize(name); @name = name; end
来源：http://qxy.hysaishi.cn

C#:   public User(string name) { Name = name; }
来源：http://mrt.zhengqikj.top

[G03] 实例属性
来源：http://yyf.yuanzhike.top

Py:   self.name = "x"
来源：http://psv.feifeiyinyue.top

PHP:  public string $name = "x";
来源：http://boq.jinqigfzy.top

JS:   this.name = "x";
来源：http://vtm.9152youxi.cn

TS:   name: string = "x";
来源：http://mua.epnwcf.com

Java: private String name;
来源：http://lbu.chenjidiqi.icu

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hin.kuanghao11.cn

Ruby: @name = "x"
来源：http://btt.andypj.xyz

C#:   public string Name { get; set; } = "x";
来源：http://aqw.bbcook.cn

[G04] 定义方法
来源：http://xqg.cucudq.cn

Py:   def greet(self): return self.name
来源：http://oyu.nanxinkj.top

PHP:  public function greet(): string { return $this->name; }
来源：http://nqd.vqdsnc.cn

JS:   greet() { return this.name; }
来源：http://apv.hnxiangtu.top

TS:   greet(): string { return this.name; }
来源：http://wtg.jiagoushi.top

Java: String greet() { return name; }
来源：http://uyw.vehdjk.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://nnl.birdmap.top

Ruby: def greet; @name; end
来源：http://xam.yonumen.top

C#:   public string Greet() => Name;
来源：http://ipy.havefunace.top

[G05] 继承
来源：http://yfy.zhongyouzk.top

Py:   class Admin(User): pass
来源：http://mrr.nanxinkj.top

PHP:  class Admin extends User {}
来源：http://zob.jqgufenzy.top

JS:   class Admin extends User {}
来源：http://xjk.nanxuanxn.top

TS:   class Admin extends User {}
来源：http://aje.chenlongwang.top

Java: class Admin extends User {}
来源：http://pgy.ybcxt.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pgj.fengsongda.top

Ruby: class Admin < User; end
来源：http://eby.smart0.xyz

C#:   class Admin : User {}
来源：http://vqv.nanxinkj.top

[G06] 重写方法
来源：http://ird.yanxiufei.cn

Py:   def greet(self): return "admin"
来源：http://cbx.52xcode.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mai.guannengcc.top

JS:   greet() { return "admin"; }
来源：http://rvr.yfazqb.com

TS:   greet(): string { return "admin"; }
来源：http://zah.hnxiangtu.top

Java: @Override String greet() { return "admin"; }
来源：http://jwv.quarkkingdee.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://azn.shuidangran.top

Ruby: def greet; "admin"; end
来源：http://xdi.epnwcf.com

C#:   public override string Greet() => "admin";
来源：http://epl.ehwqpu.com

[G07] 调用父类方法
来源：http://ihx.snrcjt.cn

Py:   super().greet()
来源：http://wxt.nanxuanxn.top

PHP:  parent::greet();
来源：http://qil.zhoulong.xyz

JS:   super.greet();
来源：http://vql.sjlbkw.cn

TS:   super.greet();
来源：http://hyz.mhx1999.top

Java: super.greet();
来源：http://tib.xinyue.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rbl.jinqigufen.top

Ruby: super
来源：http://ucg.mhx1999.top

C#:   base.Greet();
来源：http://dnv.smart0.xyz

[G08] 静态方法与属性
来源：http://qkx.haohaochexian.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ggx.ydjk.org.cn

PHP:  public static function f() {}
来源：http://szg.cdnleiting.top

JS:   static f() {}
来源：http://hdw.gotoacloud.top

TS:   static f(): void {}
来源：http://gki.chenlongwang.top

Java: static void f() {}
来源：http://uxo.9152youxi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ckx.cucudq.cn

Ruby: def self.f; end
来源：http://dxl.hysaishi.cn

C#:   public static void F() {}
来源：http://hfo.sysykeji.top

[G09] 接口 / 抽象类
来源：http://wzj.chenjidiqi.icu

Py:   from abc import ABC, abstractmethod
来源：http://iui.nwbrower.top

PHP:  interface Shape { public function area(): float; }
来源：http://xzj.yuxming.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tog.bbcook.cn

TS:   interface Shape { area(): number; }
来源：http://dyw.hammf.cn

Java: interface Shape { double area(); }
来源：http://ixb.jianghu66.top

Go:   type Shape interface { Area() float64 }
来源：http://qso.yvedp.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lkw.yangfankeji.com

C#:   interface IShape { double Area(); }
来源：http://xrg.chenlongwang.top

[G10] 访问控制
来源：http://qpq.vehdjk.com

Py:   约定 _protected / __private（不强制）
来源：http://kce.yonumen.top

PHP:  public / protected / private
来源：http://fan.feifeiyinyue.top

JS:   #private 字段；其余公开
来源：http://jzy.andypj.xyz

TS:   public / protected / private
来源：http://zcf.jyoumei.cn

Java: public / protected / private / 默认包级
来源：http://pab.hongshengwenyu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://edx.hesvh.cn

Ruby: public / protected / private
来源：http://fcr.hfpthk.cn

C#:   public / protected / private / internal
来源：http://cdh.cdnleiting.top

[G11] getter / setter
来源：http://ujb.c1oappe.top

Py:   @property 与 @x.setter
来源：http://tpi.zhongyouzk.top

PHP:  public function getName(): string { return $this->name; }
来源：http://fbh.zhijiandao.cn

JS:   get name() { return this._name; }
来源：http://arx.zhijiandao.cn

TS:   get name(): string { return this._name; }
来源：http://rmx.ydjk.org.cn

Java: public String getName() { return name; }
来源：http://stm.yuxming.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://uwq.vehdjk.com

Ruby: attr_accessor :name
来源：http://vqk.ppjwa.cn

C#:   public string Name { get; set; }
来源：http://afp.52xcode.cn

[G12] 对象转字符串
来源：http://mcg.cucudq.cn

Py:   def __str__(self): return self.name
来源：http://qxq.pycfn.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://mpd.jyoumei.cn

JS:   toString() { return this.name; }
来源：http://lay.yj202588.top

TS:   toString(): string { return this.name; }
来源：http://rvq.fehbvm.com

Java: @Override public String toString() { return name; }
来源：http://igf.hysaishi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://pug.svipenyu.cn

Ruby: def to_s; @name; end
来源：http://oww.yanxiufei.cn

C#:   public override string ToString() => Name;
来源：http://lbr.daxiang520.top

[G13] 判断对象类型
来源：http://soj.epnwcf.com

Py:   isinstance(u, User)
来源：http://rtl.hongshengwenyu.top

PHP:  $u instanceof User
来源：http://ztr.gotoacloud.top

JS:   u instanceof User
来源：http://idr.yongpay.top

TS:   u instanceof User
来源：http://xun.fktsv.cn

Java: u instanceof User
来源：http://fjb.yonumen.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://gyw.ivvv.top

Ruby: u.is_a?(User)
来源：http://bad.zdqjudy.top

C#:   u is User
来源：http://lcg.wangdashe.top

[G14] 数据类 / record
来源：http://qxn.kuanghao11.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://moa.xuetiantiany.cn

PHP:  // 用 readonly 属性模拟
来源：http://rbr.kuanghao11.cn

JS:   // 无内置：普通类或对象字面量
来源：http://peg.mhx1999.top

TS:   type User = { name: string; age: number };
来源：http://dos.epnwcf.com

Java: record User(String name, int age) {}
来源：http://uvj.vehdjk.com

Go:   type User struct { Name string; Age int }
来源：http://sga.hysaishi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://whb.fengsongda.top

C#:   record User(string Name, int Age);
来源：http://vlw.xuanzx.com

[G15] 枚举
来源：http://bqj.chenjidiqi.icu

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dfv.zdqjudy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ztz.fktsv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dok.uphjek.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rlg.0kj1m.cn

Java: enum Color { RED, GREEN }
来源：http://vpo.ehwqpu.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uwu.snrcjt.cn

Ruby: Color = %i[red green].freeze
来源：http://ciz.fanxiaobao.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dhh.pengpengdd.cyou

[G16] 对象转数组 / 字典
来源：http://lbo.wangdashe.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qdc.ywan-chungtsiang.top

PHP:  get_object_vars($obj);
来源：http://lru.sweek.top

JS:   Object.entries(obj)
来源：http://ovt.nanxinkj.top

TS:   Object.entries(obj)
来源：http://ifw.ivvv.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://oxk.hnqzz.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://mue.xingfuxueyuan.xyz

Ruby: obj.instance_variables
来源：http://cpm.xuanzx.com

C#:   // 用反射或 System.Text.Json
来源：http://rsm.yangfankeji.com

================================================================================
来源：http://rvz.kuanghao11.cn

H. 异常与错误处理
来源：http://pnf.gaohongyu789.top

================================================================================
来源：http://jpt.hammf.cn

[H01] try / catch 基础
来源：http://rng.hysaishi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bya.shuidangran.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ard.zhoulong.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lpl.mhx1999.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yym.fktsv.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cwx.pengpengdd.cyou

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uuw.0kj1m.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://leo.xziqi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rha.jinqigufen.top

[H02] finally / ensure 收尾
来源：http://gih.shuidangran.top

Py:   try: f()⏎finally: cleanup()
来源：http://nru.shangyingyoupin.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://yjk.9152youxi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://npy.9152youxi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pmk.guannengcc.top

Java: try { f(); } finally { cleanup(); }
来源：http://djw.ydjk.org.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://uut.cheryme.top

Ruby: begin; f; ensure; cleanup; end
来源：http://syl.daxiang520.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://inq.jlsjyb.cn

[H03] 主动抛出异常
来源：http://pll.xuetiantiany.cn

Py:   raise ValueError("错误信息")
来源：http://ucb.zhijiandao.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dgo.guannengcc.top

JS:   throw new Error("错误信息");
来源：http://cxq.xingfuxueyuan.xyz

TS:   throw new Error("错误信息");
来源：http://iha.tianlin.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://dvh.sjlbkw.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://aug.dianchejie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://muj.nwbrower.top

C#:   throw new ArgumentException("错误信息");
来源：http://sfa.ivvv.top

[H04] 自定义异常类型
来源：http://lmt.nanxinkj.top

Py:   class MyError(Exception): pass
来源：http://bce.shzxlz.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jwy.guowangkeji.top

JS:   class MyError extends Error {}
来源：http://lkf.guowangkeji.top

TS:   class MyError extends Error {}
来源：http://uhu.dianchejie.cn

Java: class MyException extends RuntimeException {}
来源：http://kfr.vqdsnc.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://byz.xuetiantiany.cn

Ruby: class MyError < StandardError; end
来源：http://tkv.uphjek.com

C#:   class MyException : Exception {}
来源：http://tmx.tianlin.xyz

[H05] 捕获特定类型
来源：http://dvn.cashguo.top

Py:   except ValueError as e:
来源：http://jbw.jinghuilouyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wuc.yuxming.cn

JS:   if (e instanceof TypeError) {}
来源：http://whl.xylfe.cn

TS:   if (e instanceof TypeError) {}
来源：http://acw.chenjidiqi.icu

Java: catch (IOException | SQLException e) {}
来源：http://bpw.jyoumei.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tgf.xinyue.icu

Ruby: rescue ArgumentError => e
来源：http://uvx.c1oappe.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jtt.yonumen.top

[H06] 可选值 / 空值安全访问
来源：http://ost.yuxming.cn

Py:   value = d.get("k") or default
来源：http://cvy.gaohongyu789.top

PHP:  $v = $d["k"] ?? null;
来源：http://czy.jiagoushi.top

JS:   obj?.a?.b;  d ?? default
来源：http://qse.gzhubu.top

TS:   obj?.a?.b;  d ?? default
来源：http://dqq.chenzaomai.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ygq.hesvh.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ghb.daxiang520.top

Ruby: d&.dig(:a, :b)
来源：http://kah.pengpengdd.cyou

C#:   obj?.A?.B ?? default
来源：http://lvw.guannengcc.top

[H07] 断言
来源：http://gep.kuanghao11.cn

Py:   assert x > 0, "必须为正"
来源：http://olf.kuanghao11.cn

PHP:  assert($x > 0);
来源：http://oex.ydjk.org.cn

JS:   console.assert(x > 0);
来源：http://smt.chenlongwang.top

TS:   console.assert(x > 0);
来源：http://afe.andypj.xyz

Java: assert x > 0 : "必须为正";
来源：http://xhn.iojbl.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ujj.yonumen.top

Ruby: raise "必须为正" unless x > 0
来源：http://ref.bbcook.cn

C#:   Debug.Assert(x > 0);
来源：http://rvx.zhijiandao.cn

[H08] 获取错误信息与堆栈
来源：http://jus.yangfankeji.com

Py:   str(e);  traceback.format_exc()
来源：http://zcm.mhx1999.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gfr.shangyingyoupin.top

JS:   e.message;  e.stack
来源：http://slm.epnwcf.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://oay.hywenlv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ign.ehwqpu.com

Go:   err.Error()
来源：http://adp.smart0.xyz

Ruby: e.message;  e.backtrace
来源：http://zti.guowangkeji.top

C#:   e.Message;  e.StackTrace
来源：http://rbp.zhijiandao.cn

[H09] 带错误码的异常
来源：http://usc.yj20258.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gzr.smart0.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://cyo.wangdashe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wjo.fehbvm.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rwm.quarkkingdee.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yek.chenjidiqi.icu

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vea.sxryk.cn

Ruby: raise MyError.new("fail", 500)
来源：http://cpm.shanyushiyangkeji.top

C#:   // 自定义异常类中加 Code 属性
来源：http://bbp.ivvv.top

[H10] 资源自动释放
来源：http://zkn.tanke756.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://plf.daxiang520.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fkp.zhiwuduotai.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kfy.xuanzx.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://whq.ybcxt.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zit.yonumen.top

Go:   defer f.Close()
来源：http://act.yuxming.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://oiy.zhaomingkeji.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cvl.hysaishi.cn

================================================================================
来源：http://clg.kuanghao11.cn

I. 正则表达式
来源：http://ihw.fktsv.cn

================================================================================
来源：http://cuf.dashuyun.cn

[I01] 判断是否匹配
来源：http://bvv.hnqzz.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fbv.zhaomingkeji.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://wrw.jinqigfzy.top

JS:   /\d+/.test(s)
来源：http://qtx.yongpay.top

TS:   /\d+/.test(s)
来源：http://oxa.tian-w.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gky.shangyingyoupin.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ory.yonumen.top

Ruby: s.match?(/\d+/)
来源：http://qtw.jinyuanbaomall.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tfk.nwbrower.top

[I02] 提取所有匹配
来源：http://qlf.yonumen.top

Py:   re.findall(r"\d+", s)
来源：http://dsa.ppjwa.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qny.tarul.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rvo.tian-w.cn

TS:   s.match(/\d+/g)
来源：http://jny.316326.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tta.hammf.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://alt.zhengqikj.top

Ruby: s.scan(/\d+/)
来源：http://gkl.zycfv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uuf.yuanzhike.top

[I03] 提取捕获分组
来源：http://wph.cucudq.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lgu.sysykeji.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fcp.kuanghao11.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xpt.yj202588.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://srd.yj202588.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rcw.aibaodan.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bfv.ydjk.org.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rqn.xylfe.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hwk.cashguo.top

[I04] 正则替换
来源：http://hxd.tianlin.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://vej.yongpay.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blf.guowangkeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://nfo.zdqjudy.top

TS:   s.replace(/\d+/g, "#")
来源：http://bzh.cdnleiting.top

Java: s.replaceAll("\\d+", "#")
来源：http://etg.jlsjyb.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://eam.hammf.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://oyo.c1oappe.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bgm.zhoulong.xyz

[I05] 按正则拆分
来源：http://mvx.jinghuilouyu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://unf.zhoulong.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://erx.fehbvm.com

JS:   s.split(/\s*,\s*/)
来源：http://jsd.cqqwz.cn

TS:   s.split(/\s*,\s*/)
来源：http://ilk.hongshengwenyu.top


<!-- 参考信息 -->