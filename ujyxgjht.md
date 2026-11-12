代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hal.nanxuanxn.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://arf.9152youxi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ked.jqgufenzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://boh.0kj1m.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hdc.pycfn.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lkg.redwolf501.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sqp.yuxming.cn

[F12] CSV 读写
来源：http://szx.yj20258.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tkf.zhaomingkeji.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ose.xinyue.icu

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ykt.quarkkingdee.top

TS:   // 同上
来源：http://hcy.guowangkeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oix.ctjpmb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kgy.vqdsnc.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ymi.aizwys.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ayc.jyoumei.cn

================================================================================
来源：http://dme.zhijiandao.cn

G. 面向对象
来源：http://qse.sjlbkw.cn

================================================================================
来源：http://ovj.hysaishi.cn

[G01] 定义类
来源：http://ffk.tanke756.top

Py:   class User: pass
来源：http://ksm.bbcook.cn

PHP:  class User {}
来源：http://okh.vqdsnc.cn

JS:   class User {}
来源：http://ovt.yangfankeji.com

TS:   class User { name: string = ""; }
来源：http://kad.cheryme.top

Java: class User {}
来源：http://srw.xuetiantiany.cn

Go:   type User struct { Name string }
来源：http://zcm.sweek.top

Ruby: class User; end
来源：http://mod.vqdsnc.cn

C#:   class User {}
来源：http://qtb.ctjpmb.com

[G02] 构造函数
来源：http://not.jianghu66.top

Py:   def __init__(self, name): self.name = name
来源：http://rbc.jqgfzy.top

PHP:  public function __construct(public string $name) {}
来源：http://aua.zhiwuduotai.top

JS:   constructor(name) { this.name = name; }
来源：http://sjy.tanke756.top

TS:   constructor(public name: string) {}
来源：http://pcj.jinyuanbaomall.cn

Java: User(String name) { this.name = name; }
来源：http://ljx.0kj1m.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mjn.cashguo.top

Ruby: def initialize(name); @name = name; end
来源：http://zvl.ctjpmb.com

C#:   public User(string name) { Name = name; }
来源：http://xhx.pycfn.com

[G03] 实例属性
来源：http://nhs.hnqzz.top

Py:   self.name = "x"
来源：http://iaq.ppjwa.cn

PHP:  public string $name = "x";
来源：http://ogb.feifeiyinyue.top

JS:   this.name = "x";
来源：http://kqv.ybcxt.top

TS:   name: string = "x";
来源：http://kdt.ehwqpu.com

Java: private String name;
来源：http://aow.yonumen.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://oyi.zdqjudy.top

Ruby: @name = "x"
来源：http://sno.daxiang520.top

C#:   public string Name { get; set; } = "x";
来源：http://swd.dashuyun.cn

[G04] 定义方法
来源：http://edg.yvedp.cn

Py:   def greet(self): return self.name
来源：http://cys.haohaochexian.top

PHP:  public function greet(): string { return $this->name; }
来源：http://nqz.cashguo.top

JS:   greet() { return this.name; }
来源：http://jbf.xinyue.icu

TS:   greet(): string { return this.name; }
来源：http://whz.xingfuxueyuan.xyz

Java: String greet() { return name; }
来源：http://jzz.tarul.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wct.ctjpmb.com

Ruby: def greet; @name; end
来源：http://xen.cqqwz.cn

C#:   public string Greet() => Name;
来源：http://cmz.vqdsnc.cn

[G05] 继承
来源：http://ayn.zhijiandao.cn

Py:   class Admin(User): pass
来源：http://twl.zhiwuduotai.top

PHP:  class Admin extends User {}
来源：http://zjq.svipenyu.cn

JS:   class Admin extends User {}
来源：http://rua.pengpengdd.cyou

TS:   class Admin extends User {}
来源：http://ccw.zdqjudy.top

Java: class Admin extends User {}
来源：http://rwp.vqdsnc.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lju.daxiang520.top

Ruby: class Admin < User; end
来源：http://kja.yvedp.cn

C#:   class Admin : User {}
来源：http://unf.zhongyouzk.top

[G06] 重写方法
来源：http://mgu.bbcook.cn

Py:   def greet(self): return "admin"
来源：http://nqg.aibaodan.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gsv.fanxiaobao.xyz

JS:   greet() { return "admin"; }
来源：http://fwv.yueranfly.top

TS:   greet(): string { return "admin"; }
来源：http://sip.jiagoushi.top

Java: @Override String greet() { return "admin"; }
来源：http://uqy.sweek.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mjq.ehwqpu.com

Ruby: def greet; "admin"; end
来源：http://xlg.andypj.xyz

C#:   public override string Greet() => "admin";
来源：http://hnr.fktsv.cn

[G07] 调用父类方法
来源：http://pan.daxiang520.top

Py:   super().greet()
来源：http://oue.tianlin.xyz

PHP:  parent::greet();
来源：http://imi.shanyushiyangkeji.top

JS:   super.greet();
来源：http://tdw.yanxiufei.cn

TS:   super.greet();
来源：http://hcf.hywenlv.cn

Java: super.greet();
来源：http://oxs.gaohongyu789.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hdq.shanyushiyangkeji.top

Ruby: super
来源：http://tlt.sjlbkw.cn

C#:   base.Greet();
来源：http://dnn.jianghu66.top

[G08] 静态方法与属性
来源：http://yev.havefunace.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mgm.xuanzx.com

PHP:  public static function f() {}
来源：http://txn.shanyushiyangtech.top

JS:   static f() {}
来源：http://psb.smart0.xyz

TS:   static f(): void {}
来源：http://ect.sjlbkw.cn

Java: static void f() {}
来源：http://ivd.tarul.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://uzt.zhoulong.xyz

Ruby: def self.f; end
来源：http://hcs.shuidangran.top

C#:   public static void F() {}
来源：http://dtw.vqdsnc.cn

[G09] 接口 / 抽象类
来源：http://ijr.shanyushiyangkeji.top

Py:   from abc import ABC, abstractmethod
来源：http://uuw.meibo888.top

PHP:  interface Shape { public function area(): float; }
来源：http://ngb.shanyushiyangkeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://fff.shuidangran.top

TS:   interface Shape { area(): number; }
来源：http://rpp.sjlbkw.cn

Java: interface Shape { double area(); }
来源：http://drc.sxryk.cn

Go:   type Shape interface { Area() float64 }
来源：http://ecx.tianlin.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zgq.shanyushiyangtech.top

C#:   interface IShape { double Area(); }
来源：http://nwm.andypj.xyz

[G10] 访问控制
来源：http://log.cashguo.top

Py:   约定 _protected / __private（不强制）
来源：http://yld.fktsv.cn

PHP:  public / protected / private
来源：http://crd.sysykeji.top

JS:   #private 字段；其余公开
来源：http://nbt.hysaishi.cn

TS:   public / protected / private
来源：http://mhv.xuetiantiany.cn

Java: public / protected / private / 默认包级
来源：http://hpo.nwbrower.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://dmo.redwolf501.top

Ruby: public / protected / private
来源：http://mwj.snrcjt.cn

C#:   public / protected / private / internal
来源：http://qpq.havefunace.top

[G11] getter / setter
来源：http://tkx.xingfuxueyuan.xyz

Py:   @property 与 @x.setter
来源：http://sps.dianchejie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jtz.hcnkem.com

JS:   get name() { return this._name; }
来源：http://kle.yj202588.top

TS:   get name(): string { return this._name; }
来源：http://bqn.yfazqb.com

Java: public String getName() { return name; }
来源：http://cgg.zhijiandao.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dmp.shangyingyoupin.top

Ruby: attr_accessor :name
来源：http://jpq.dianchejie.cn

C#:   public string Name { get; set; }
来源：http://xgh.svipenyu.cn

[G12] 对象转字符串
来源：http://nrx.nanxuanxn.top

Py:   def __str__(self): return self.name
来源：http://sri.svipenyu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rna.yueranfly.top

JS:   toString() { return this.name; }
来源：http://qfy.xinyue.icu

TS:   toString(): string { return this.name; }
来源：http://zuz.ppjwa.cn

Java: @Override public String toString() { return name; }
来源：http://aqv.mhx1999.top

Go:   func (u User) String() string { return u.Name }
来源：http://yyu.hysaishi.cn

Ruby: def to_s; @name; end
来源：http://tlk.316326.xyz

C#:   public override string ToString() => Name;
来源：http://xhg.pycfn.com

[G13] 判断对象类型
来源：http://iub.cucudq.cn

Py:   isinstance(u, User)
来源：http://oyt.shuidangran.top

PHP:  $u instanceof User
来源：http://pyr.iojbl.cn

JS:   u instanceof User
来源：http://sqg.yj202588.top

TS:   u instanceof User
来源：http://jyd.ybcxt.top

Java: u instanceof User
来源：http://frs.tarul.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://lrl.yj202588.top

Ruby: u.is_a?(User)
来源：http://awt.shanyushiyangtech.top

C#:   u is User
来源：http://cah.havefunace.top

[G14] 数据类 / record
来源：http://uju.yangfankeji.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zrb.shzxlz.cn

PHP:  // 用 readonly 属性模拟
来源：http://ctn.shzxlz.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rfz.fengsongda.top

TS:   type User = { name: string; age: number };
来源：http://mfy.vqdsnc.cn

Java: record User(String name, int age) {}
来源：http://ohi.iojbl.cn

Go:   type User struct { Name string; Age int }
来源：http://ujh.hywenlv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bgw.yuanzhike.top

C#:   record User(string Name, int Age);
来源：http://gvc.xuanzx.com

[G15] 枚举
来源：http://wae.pengpengdd.cyou

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ahd.epnwcf.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://cht.zhongyouzk.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pqn.hnqzz.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vby.andypj.xyz

Java: enum Color { RED, GREEN }
来源：http://asl.ydjk.org.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rag.xuanzx.com

Ruby: Color = %i[red green].freeze
来源：http://zqr.9152youxi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ngq.yuxming.cn

[G16] 对象转数组 / 字典
来源：http://iae.xuanzx.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qeg.hnqzz.top

PHP:  get_object_vars($obj);
来源：http://tns.zhongyouzk.top

JS:   Object.entries(obj)
来源：http://iki.zhongyouzk.top

TS:   Object.entries(obj)
来源：http://zux.fanxiaobao.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uta.ppjwa.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jca.sxryk.cn

Ruby: obj.instance_variables
来源：http://tlr.chenjidiqi.icu

C#:   // 用反射或 System.Text.Json
来源：http://nee.vqdsnc.cn

================================================================================
来源：http://xep.sysykeji.top

H. 异常与错误处理
来源：http://ikx.zhixingplan.top

================================================================================
来源：http://vpm.yuanzhike.top

[H01] try / catch 基础
来源：http://cje.shanyushiyangtech.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wsx.ydzc1.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://awa.9152youxi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lvj.wangdashe.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://atr.sweek.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dad.chenzaomai.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zfs.fktsv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ylt.yanxiufei.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nah.sweek.top

[H02] finally / ensure 收尾
来源：http://jny.yfazqb.com

Py:   try: f()⏎finally: cleanup()
来源：http://pyp.xziqi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mzk.dashuyun.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://uia.vqdsnc.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://izg.jqgufenzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://ige.xuetiantiany.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jdw.yuxming.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://yxa.sweek.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://jov.bjfxy.top

[H03] 主动抛出异常
来源：http://dra.xylfe.cn

Py:   raise ValueError("错误信息")
来源：http://sov.jinghuilouyu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vrd.yj202588.top

JS:   throw new Error("错误信息");
来源：http://wnp.c1oappe.top

TS:   throw new Error("错误信息");
来源：http://sth.meibo888.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qcj.fengsongda.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://puk.yj202588.top

Ruby: raise ArgumentError, "错误信息"
来源：http://qmq.chenlongwang.top

C#:   throw new ArgumentException("错误信息");
来源：http://eie.yuanzhike.top

[H04] 自定义异常类型
来源：http://olc.ydjk.org.cn

Py:   class MyError(Exception): pass
来源：http://zni.fehbvm.com

PHP:  class MyError extends RuntimeException {}
来源：http://ewv.hfpthk.cn

JS:   class MyError extends Error {}
来源：http://miv.sufxvd.cn

TS:   class MyError extends Error {}
来源：http://qgz.gogol.net.cn

Java: class MyException extends RuntimeException {}
来源：http://qkl.aibaodan.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tnj.pengpengdd.cyou

Ruby: class MyError < StandardError; end
来源：http://ezw.sysykeji.top

C#:   class MyException : Exception {}
来源：http://ngj.yuxming.cn

[H05] 捕获特定类型
来源：http://hxq.zhaomingkeji.xyz

Py:   except ValueError as e:
来源：http://yjg.havefunace.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yzf.jiagoushi.top

JS:   if (e instanceof TypeError) {}
来源：http://upf.xuanzx.com

TS:   if (e instanceof TypeError) {}
来源：http://sdo.bbcook.cn

Java: catch (IOException | SQLException e) {}
来源：http://awv.chenlongwang.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ctg.sxryk.cn

Ruby: rescue ArgumentError => e
来源：http://ufm.tanke756.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hlz.xylfe.cn

[H06] 可选值 / 空值安全访问
来源：http://kvf.zhijiandao.cn

Py:   value = d.get("k") or default
来源：http://sfn.epnwcf.com

PHP:  $v = $d["k"] ?? null;
来源：http://aim.cheryme.top

JS:   obj?.a?.b;  d ?? default
来源：http://kud.cdnleiting.top

TS:   obj?.a?.b;  d ?? default
来源：http://yig.yuxming.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bbw.snrcjt.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ckh.jqgufenzy.top

Ruby: d&.dig(:a, :b)
来源：http://ivg.cucudq.cn

C#:   obj?.A?.B ?? default
来源：http://osr.xuetiantiany.cn

[H07] 断言
来源：http://pkt.hongshengwenyu.top

Py:   assert x > 0, "必须为正"
来源：http://yuo.chenzaomai.com

PHP:  assert($x > 0);
来源：http://hpx.snrcjt.cn

JS:   console.assert(x > 0);
来源：http://imd.meibo888.top

TS:   console.assert(x > 0);
来源：http://qdo.xuanzx.com

Java: assert x > 0 : "必须为正";
来源：http://yzj.52xcode.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://htx.316326.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://cjm.yfazqb.com

C#:   Debug.Assert(x > 0);
来源：http://zqj.ydjk.org.cn

[H08] 获取错误信息与堆栈
来源：http://cix.vehdjk.com

Py:   str(e);  traceback.format_exc()
来源：http://yyn.316326.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fiy.uphjek.com

JS:   e.message;  e.stack
来源：http://ooj.hywenlv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://frg.aibaodan.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://asu.jqgfzy.top

Go:   err.Error()
来源：http://dbv.hesvh.cn

Ruby: e.message;  e.backtrace
来源：http://oqv.zdqjudy.top

C#:   e.Message;  e.StackTrace
来源：http://ayk.nanxinkj.top

[H09] 带错误码的异常
来源：http://cmw.zhixingplan.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vrp.yangfankeji.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://wyp.zhoulong.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rqz.nanxinkj.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ryr.tarul.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nbn.ydjk.org.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cln.nwbrower.top

Ruby: raise MyError.new("fail", 500)
来源：http://xaz.yonumen.top

C#:   // 自定义异常类中加 Code 属性
来源：http://onf.dashuyun.cn

[H10] 资源自动释放
来源：http://iqb.daria6918.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ejc.cheryme.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://obm.zhoulong.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gmw.zhengqikj.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ftl.gotoacloud.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://utt.pengpengdd.cyou

Go:   defer f.Close()
来源：http://ddh.zhixingplan.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jhw.xuetiantiany.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ptd.sufxvd.cn

================================================================================
来源：http://uvq.tian-w.cn

I. 正则表达式
来源：http://jsu.meibo888.top

================================================================================
来源：http://lpc.quarkkingdee.top

[I01] 判断是否匹配
来源：http://wsn.yj202588.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qft.shanyushiyangkeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://igf.zycfv.cn

JS:   /\d+/.test(s)
来源：http://sho.yuxming.cn

TS:   /\d+/.test(s)
来源：http://xzq.ctjpmb.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ljz.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fxp.shangyingyoupin.top

Ruby: s.match?(/\d+/)
来源：http://woi.redwolf501.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://epv.jiagoushi.top

[I02] 提取所有匹配
来源：http://lie.ydjk.org.cn

Py:   re.findall(r"\d+", s)
来源：http://itn.ehwqpu.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tua.vehdjk.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ivm.ydjk.org.cn

TS:   s.match(/\d+/g)
来源：http://zxv.zdqjudy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hgz.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gyn.52xcode.cn

Ruby: s.scan(/\d+/)
来源：http://sdp.ctjpmb.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fnj.fzhhl.top

[I03] 提取捕获分组
来源：http://afp.fzhhl.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uor.yanxiufei.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ylg.zdqjudy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://snd.nwbrower.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bqn.aibaodan.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yzj.ctjpmb.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ucp.xingfuxueyuan.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kdz.jiagoushi.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fmb.wangshuangyany.cn

[I04] 正则替换
来源：http://kjk.gaohongyu789.top

Py:   re.sub(r"\d+", "#", s)
来源：http://mhw.zdqjudy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sqn.svipenyu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kgs.xuetiantiany.cn

TS:   s.replace(/\d+/g, "#")
来源：http://uri.ydjk.org.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hvt.guowangkeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://iih.shangyingyoupin.top

Ruby: s.gsub(/\d+/, "#")
来源：http://xme.tian-w.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tas.zhengqikj.top

[I05] 按正则拆分
来源：http://zyv.kuanghao11.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tot.zhijiandao.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vui.fzhhl.top

JS:   s.split(/\s*,\s*/)
来源：http://dae.fehbvm.com

TS:   s.split(/\s*,\s*/)
来源：http://dqb.vqdsnc.cn


<!-- 参考信息 -->