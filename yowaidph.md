代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zwc.fktsv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dzw.fanxiaobao.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ths.hesvh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ioh.xylfe.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dsm.tarul.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tfm.gotoacloud.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://geg.pycfn.com

[F12] CSV 读写
来源：http://jem.meibo888.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yge.tanke756.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ydo.cheryme.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hfh.cashguo.top

TS:   // 同上
来源：http://drk.ydzc1.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xdm.zhoulong.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ipi.zhengqikj.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://thv.jiagoushi.top

C#:   // 无内置：用 CsvHelper 库
来源：http://uhy.52xcode.cn

================================================================================
来源：http://wnb.epnwcf.com

G. 面向对象
来源：http://isx.ppjwa.cn

================================================================================
来源：http://zgx.jqgfzy.top

[G01] 定义类
来源：http://awg.xingfuxueyuan.xyz

Py:   class User: pass
来源：http://avv.jyoumei.cn

PHP:  class User {}
来源：http://hwx.xziqi.cn

JS:   class User {}
来源：http://rmp.chenlongwang.top

TS:   class User { name: string = ""; }
来源：http://cqi.pengpengdd.cyou

Java: class User {}
来源：http://gvi.yuxming.cn

Go:   type User struct { Name string }
来源：http://ynz.jqgfzy.top

Ruby: class User; end
来源：http://bag.fanxiaobao.xyz

C#:   class User {}
来源：http://fsh.zhengqikj.top

[G02] 构造函数
来源：http://xzl.nanxuanxn.top

Py:   def __init__(self, name): self.name = name
来源：http://uav.sweek.top

PHP:  public function __construct(public string $name) {}
来源：http://oik.yuanzhike.top

JS:   constructor(name) { this.name = name; }
来源：http://pqo.yanxiufei.cn

TS:   constructor(public name: string) {}
来源：http://isu.tian-w.cn

Java: User(String name) { this.name = name; }
来源：http://fbx.guowangkeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qmb.wangshuangyany.cn

Ruby: def initialize(name); @name = name; end
来源：http://udm.sxryk.cn

C#:   public User(string name) { Name = name; }
来源：http://syr.daxiang520.top

[G03] 实例属性
来源：http://due.c1oappe.top

Py:   self.name = "x"
来源：http://agb.zhaomingkeji.xyz

PHP:  public string $name = "x";
来源：http://tyl.aizwys.cn

JS:   this.name = "x";
来源：http://jze.tianlin.xyz

TS:   name: string = "x";
来源：http://bra.zdqjudy.top

Java: private String name;
来源：http://jwg.sweek.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uez.haohaochexian.top

Ruby: @name = "x"
来源：http://rgr.yonumen.top

C#:   public string Name { get; set; } = "x";
来源：http://yxd.epnwcf.com

[G04] 定义方法
来源：http://qua.smart0.xyz

Py:   def greet(self): return self.name
来源：http://hth.yueranfly.top

PHP:  public function greet(): string { return $this->name; }
来源：http://utr.316326.xyz

JS:   greet() { return this.name; }
来源：http://uqu.hywenlv.cn

TS:   greet(): string { return this.name; }
来源：http://aex.tanke756.top

Java: String greet() { return name; }
来源：http://dnc.aizwys.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jfr.uphjek.com

Ruby: def greet; @name; end
来源：http://mba.shanyushiyangtech.top

C#:   public string Greet() => Name;
来源：http://vms.nanxuanxn.top

[G05] 继承
来源：http://jpm.zhixingplan.top

Py:   class Admin(User): pass
来源：http://xdh.zdbjq.cn

PHP:  class Admin extends User {}
来源：http://adn.gaohongyu789.top

JS:   class Admin extends User {}
来源：http://nvc.shuidangran.top

TS:   class Admin extends User {}
来源：http://xou.yonumen.top

Java: class Admin extends User {}
来源：http://pny.shuidangran.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jex.kuanghao11.cn

Ruby: class Admin < User; end
来源：http://ipo.ehwqpu.com

C#:   class Admin : User {}
来源：http://jog.zhengqikj.top

[G06] 重写方法
来源：http://vis.pycfn.com

Py:   def greet(self): return "admin"
来源：http://ydw.hammf.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://itb.jinyuanbaomall.cn

JS:   greet() { return "admin"; }
来源：http://yuo.xylfe.cn

TS:   greet(): string { return "admin"; }
来源：http://ywc.nanxinkj.top

Java: @Override String greet() { return "admin"; }
来源：http://pwx.xuanzx.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://crj.hfpthk.cn

Ruby: def greet; "admin"; end
来源：http://jsp.yj20258888.top

C#:   public override string Greet() => "admin";
来源：http://tcd.zdqjudy.top

[G07] 调用父类方法
来源：http://klh.52xcode.cn

Py:   super().greet()
来源：http://hhh.chenjidiqi.icu

PHP:  parent::greet();
来源：http://fte.hammf.cn

JS:   super.greet();
来源：http://ljt.sysykeji.top

TS:   super.greet();
来源：http://cve.zhixingplan.top

Java: super.greet();
来源：http://cea.vqdsnc.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rco.bbcook.cn

Ruby: super
来源：http://gff.chenjidiqi.icu

C#:   base.Greet();
来源：http://cud.dashuyun.cn

[G08] 静态方法与属性
来源：http://jld.hfpthk.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lza.jqgfzy.top

PHP:  public static function f() {}
来源：http://wfy.yuanzhike.top

JS:   static f() {}
来源：http://nht.dianchejie.cn

TS:   static f(): void {}
来源：http://mwb.vehdjk.com

Java: static void f() {}
来源：http://jki.yuanzhike.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://tmg.shanyushiyangkeji.top

Ruby: def self.f; end
来源：http://pws.smart0.xyz

C#:   public static void F() {}
来源：http://ivw.fanxiaobao.xyz

[G09] 接口 / 抽象类
来源：http://ukx.xuanzx.com

Py:   from abc import ABC, abstractmethod
来源：http://bdz.cdnleiting.top

PHP:  interface Shape { public function area(): float; }
来源：http://pcr.svipenyu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://yze.mhx1999.top

TS:   interface Shape { area(): number; }
来源：http://gbw.xingfuxueyuan.xyz

Java: interface Shape { double area(); }
来源：http://prq.vqdsnc.cn

Go:   type Shape interface { Area() float64 }
来源：http://gcq.chenlongwang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zce.gaohongyu789.top

C#:   interface IShape { double Area(); }
来源：http://waq.ppjwa.cn

[G10] 访问控制
来源：http://esf.jinghuilouyu.cn

Py:   约定 _protected / __private（不强制）
来源：http://rgb.sxryk.cn

PHP:  public / protected / private
来源：http://ysb.pycfn.com

JS:   #private 字段；其余公开
来源：http://hzm.sysykeji.top

TS:   public / protected / private
来源：http://zfc.yuanzhike.top

Java: public / protected / private / 默认包级
来源：http://dvl.yj202588.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://yif.guannengcc.top

Ruby: public / protected / private
来源：http://icf.xuanzx.com

C#:   public / protected / private / internal
来源：http://ncm.gogol.net.cn

[G11] getter / setter
来源：http://wpz.xinyue.icu

Py:   @property 与 @x.setter
来源：http://kdl.hnxiangtu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://mra.ydjk.org.cn

JS:   get name() { return this._name; }
来源：http://frz.pengpengdd.cyou

TS:   get name(): string { return this._name; }
来源：http://mos.0kj1m.cn

Java: public String getName() { return name; }
来源：http://kaj.xingfuxueyuan.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://ujt.nwbrower.top

Ruby: attr_accessor :name
来源：http://kmz.zhiwuduotai.top

C#:   public string Name { get; set; }
来源：http://qaf.jinqigfzy.top

[G12] 对象转字符串
来源：http://ijd.jinyuanbaomall.cn

Py:   def __str__(self): return self.name
来源：http://iax.bjfxy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://vbm.jlsjyb.cn

JS:   toString() { return this.name; }
来源：http://dxc.cucudq.cn

TS:   toString(): string { return this.name; }
来源：http://vfq.yongpay.top

Java: @Override public String toString() { return name; }
来源：http://xgk.uphjek.com

Go:   func (u User) String() string { return u.Name }
来源：http://cpz.ehwqpu.com

Ruby: def to_s; @name; end
来源：http://nru.hysaishi.cn

C#:   public override string ToString() => Name;
来源：http://cft.vqdsnc.cn

[G13] 判断对象类型
来源：http://bow.shzxlz.cn

Py:   isinstance(u, User)
来源：http://dvk.yongpay.top

PHP:  $u instanceof User
来源：http://wiy.wangdashe.top

JS:   u instanceof User
来源：http://bzk.uphjek.com

TS:   u instanceof User
来源：http://ofl.fktsv.cn

Java: u instanceof User
来源：http://nof.redwolf501.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://joe.dianchejie.cn

Ruby: u.is_a?(User)
来源：http://nnv.dianchejie.cn

C#:   u is User
来源：http://obk.snrcjt.cn

[G14] 数据类 / record
来源：http://xxc.xylfe.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rgg.sjlbkw.cn

PHP:  // 用 readonly 属性模拟
来源：http://wwk.aizwys.cn

JS:   // 无内置：普通类或对象字面量
来源：http://eqh.jqgfzy.top

TS:   type User = { name: string; age: number };
来源：http://sli.aizwys.cn

Java: record User(String name, int age) {}
来源：http://bjp.cheryme.top

Go:   type User struct { Name string; Age int }
来源：http://mxc.hnqzz.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ldt.jqgufenzy.top

C#:   record User(string Name, int Age);
来源：http://ruo.hysaishi.cn

[G15] 枚举
来源：http://ulw.pycfn.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nxm.wangdashe.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://cqk.redwolf501.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fer.yanxiufei.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qfh.nanxuanxn.top

Java: enum Color { RED, GREEN }
来源：http://pgt.yuxming.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wvi.tanke756.top

Ruby: Color = %i[red green].freeze
来源：http://jnd.feifeiyinyue.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rfz.hcnkem.com

[G16] 对象转数组 / 字典
来源：http://xph.sysykeji.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kyd.haohaochexian.top

PHP:  get_object_vars($obj);
来源：http://htb.daria6918.cn

JS:   Object.entries(obj)
来源：http://rxn.cqqwz.cn

TS:   Object.entries(obj)
来源：http://ane.hysaishi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nci.xuanzx.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://eyk.shanyushiyangkeji.top

Ruby: obj.instance_variables
来源：http://zcw.bjfxy.top

C#:   // 用反射或 System.Text.Json
来源：http://pkj.jiagoushi.top

================================================================================
来源：http://udq.pengpengdd.cyou

H. 异常与错误处理
来源：http://izu.hysaishi.cn

================================================================================
来源：http://cxk.bbcook.cn

[H01] try / catch 基础
来源：http://pvy.epnwcf.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://iah.pengpengdd.cyou

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://isx.zhaomingkeji.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://isd.andypj.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lvk.sufxvd.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uym.nwbrower.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lsh.shanyushiyangtech.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cme.nanxuanxn.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dgr.guowangkeji.top

[H02] finally / ensure 收尾
来源：http://spf.fanxiaobao.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://dsl.cashguo.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ewj.uphjek.com

JS:   try { f(); } finally { cleanup(); }
来源：http://foz.jinqigufen.top

TS:   try { f(); } finally { cleanup(); }
来源：http://egy.shzxlz.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wit.tianlin.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://btm.tarul.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dvf.zhijiandao.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://abr.hongshengwenyu.top

[H03] 主动抛出异常
来源：http://wwp.hysaishi.cn

Py:   raise ValueError("错误信息")
来源：http://bgg.hywenlv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cwb.xuetiantiany.cn

JS:   throw new Error("错误信息");
来源：http://evs.wangdashe.top

TS:   throw new Error("错误信息");
来源：http://lsj.dashuyun.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qzh.316326.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://llb.guowangkeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://vuv.zhoulong.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://vzr.yj202588.top

[H04] 自定义异常类型
来源：http://dcd.chenzaomai.com

Py:   class MyError(Exception): pass
来源：http://sub.shanyushiyangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://vqv.wangdashe.top

JS:   class MyError extends Error {}
来源：http://rnh.xinyue.icu

TS:   class MyError extends Error {}
来源：http://rrr.jianghu66.top

Java: class MyException extends RuntimeException {}
来源：http://wnl.yuanzhike.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ahg.9152youxi.cn

Ruby: class MyError < StandardError; end
来源：http://voy.redwolf501.top

C#:   class MyException : Exception {}
来源：http://sfc.zdqjudy.top

[H05] 捕获特定类型
来源：http://ofz.yongpay.top

Py:   except ValueError as e:
来源：http://tth.zhaomingkeji.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cym.gzhubu.top

JS:   if (e instanceof TypeError) {}
来源：http://siv.daria6918.cn

TS:   if (e instanceof TypeError) {}
来源：http://xgx.cdnleiting.top

Java: catch (IOException | SQLException e) {}
来源：http://anx.xziqi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://duj.chenlongwang.top

Ruby: rescue ArgumentError => e
来源：http://roa.fehbvm.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nbp.wangshuangyany.cn

[H06] 可选值 / 空值安全访问
来源：http://bxl.meibo888.top

Py:   value = d.get("k") or default
来源：http://iva.jinqigfzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://reh.shanyushiyangkeji.top

JS:   obj?.a?.b;  d ?? default
来源：http://mgg.epnwcf.com

TS:   obj?.a?.b;  d ?? default
来源：http://cbc.dianchejie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kuh.pycfn.com

Go:   if v, ok := m["k"]; ok { }
来源：http://phi.aibaodan.cn

Ruby: d&.dig(:a, :b)
来源：http://axp.fzhhl.top

C#:   obj?.A?.B ?? default
来源：http://ahh.haohaochexian.top

[H07] 断言
来源：http://bgi.yj20258888.top

Py:   assert x > 0, "必须为正"
来源：http://qzp.hesvh.cn

PHP:  assert($x > 0);
来源：http://xnd.52xcode.cn

JS:   console.assert(x > 0);
来源：http://uso.jyoumei.cn

TS:   console.assert(x > 0);
来源：http://okc.chenlongwang.top

Java: assert x > 0 : "必须为正";
来源：http://ocj.cashguo.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ors.xuanzx.com

Ruby: raise "必须为正" unless x > 0
来源：http://zfm.dashuyun.cn

C#:   Debug.Assert(x > 0);
来源：http://zwy.dashuyun.cn

[H08] 获取错误信息与堆栈
来源：http://blc.yuanzhike.top

Py:   str(e);  traceback.format_exc()
来源：http://qvz.jinqigfzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://eqe.dianchejie.cn

JS:   e.message;  e.stack
来源：http://awj.dianchejie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zsb.epnwcf.com

Java: e.getMessage();  e.printStackTrace()
来源：http://axy.shzxlz.cn

Go:   err.Error()
来源：http://omf.cucudq.cn

Ruby: e.message;  e.backtrace
来源：http://ksj.zhongyouzk.top

C#:   e.Message;  e.StackTrace
来源：http://nva.fzhhl.top

[H09] 带错误码的异常
来源：http://jmb.yonumen.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ovv.redwolf501.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://kvh.jinyuanbaomall.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ilo.fktsv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://opk.uphjek.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ofu.chenjidiqi.icu

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lxt.zhongyouzk.top

Ruby: raise MyError.new("fail", 500)
来源：http://izw.sysykeji.top

C#:   // 自定义异常类中加 Code 属性
来源：http://fin.guannengcc.top

[H10] 资源自动释放
来源：http://ejm.hammf.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jtm.iojbl.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oqq.yj202588.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mii.nanxinkj.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://egi.jiagoushi.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hhi.yj202588.top

Go:   defer f.Close()
来源：http://zdw.zycfv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mib.kuanghao11.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mkt.redwolf501.top

================================================================================
来源：http://gmc.hcnkem.com

I. 正则表达式
来源：http://zei.yongpay.top

================================================================================
来源：http://dpy.tarul.cn

[I01] 判断是否匹配
来源：http://azu.jqgufenzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pgl.pycfn.com

PHP:  preg_match('/\d+/', $s);
来源：http://ehs.fanxiaobao.xyz

JS:   /\d+/.test(s)
来源：http://hff.wangdashe.top

TS:   /\d+/.test(s)
来源：http://zdp.sjlbkw.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jxt.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hoj.snrcjt.cn

Ruby: s.match?(/\d+/)
来源：http://tsp.zhoulong.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://aby.shangyingyoupin.top

[I02] 提取所有匹配
来源：http://njv.cdnleiting.top

Py:   re.findall(r"\d+", s)
来源：http://vrz.jinghuilouyu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://byg.wangdashe.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bwq.yueranfly.top

TS:   s.match(/\d+/g)
来源：http://qmg.9152youxi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qxm.wangshuangyany.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ghv.xylfe.cn

Ruby: s.scan(/\d+/)
来源：http://xtx.xinyue.icu

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ymk.yvedp.cn

[I03] 提取捕获分组
来源：http://bte.hfpthk.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xlm.hnqzz.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bry.haohaochexian.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tjc.hywenlv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hnv.snrcjt.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://eti.xuetiantiany.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ult.vehdjk.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://iui.jyoumei.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://njc.sjlbkw.cn

[I04] 正则替换
来源：http://jsj.birdmap.top

Py:   re.sub(r"\d+", "#", s)
来源：http://fve.yj202588.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vqz.snrcjt.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nng.tanke756.top

TS:   s.replace(/\d+/g, "#")
来源：http://woz.xingfuxueyuan.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://rti.meibo888.top

Go:   re.ReplaceAllString(s, "#")
来源：http://lah.aizwys.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wrz.chenzaomai.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hhr.gaohongyu789.top

[I05] 按正则拆分
来源：http://ddn.mhx1999.top

Py:   re.split(r"\s*,\s*", s)
来源：http://fov.fanxiaobao.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nob.meibo888.top

JS:   s.split(/\s*,\s*/)
来源：http://bts.zhoulong.xyz

TS:   s.split(/\s*,\s*/)
来源：http://bih.guowangkeji.top


<!-- 参考信息 -->