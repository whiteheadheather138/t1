代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vgp.nanxuanxn.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://deh.guannengcc.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://swq.9152youxi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ogv.zhongyouzk.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qpy.xylfe.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://aeh.fktsv.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hof.vehdjk.com

[F12] CSV 读写
来源：http://exh.yuanzhike.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dtc.vehdjk.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qep.bjfxy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jhj.fehbvm.com

TS:   // 同上
来源：http://zju.nwbrower.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vwu.cdnleiting.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mgd.bjfxy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ukg.hcnkem.com

C#:   // 无内置：用 CsvHelper 库
来源：http://ptx.snrcjt.cn

================================================================================
来源：http://ngc.zhoulong.xyz

G. 面向对象
来源：http://ogt.fehbvm.com

================================================================================
来源：http://zek.yfazqb.com

[G01] 定义类
来源：http://foy.pengpengdd.cyou

Py:   class User: pass
来源：http://ceq.chenlongwang.top

PHP:  class User {}
来源：http://xem.fzhhl.top

JS:   class User {}
来源：http://lew.jianghu66.top

TS:   class User { name: string = ""; }
来源：http://vnh.fktsv.cn

Java: class User {}
来源：http://lrl.52xcode.cn

Go:   type User struct { Name string }
来源：http://hbh.zhengqikj.top

Ruby: class User; end
来源：http://wsn.feifeiyinyue.top

C#:   class User {}
来源：http://idb.jqgufenzy.top

[G02] 构造函数
来源：http://obu.yuanzhike.top

Py:   def __init__(self, name): self.name = name
来源：http://cmu.yangfankeji.com

PHP:  public function __construct(public string $name) {}
来源：http://urh.sxryk.cn

JS:   constructor(name) { this.name = name; }
来源：http://iow.wangshuangyany.cn

TS:   constructor(public name: string) {}
来源：http://yob.zhongyouzk.top

Java: User(String name) { this.name = name; }
来源：http://jqu.dianchejie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ksc.uphjek.com

Ruby: def initialize(name); @name = name; end
来源：http://sqe.c1oappe.top

C#:   public User(string name) { Name = name; }
来源：http://uxv.tianlin.xyz

[G03] 实例属性
来源：http://fvn.hongshengwenyu.top

Py:   self.name = "x"
来源：http://soq.yongpay.top

PHP:  public string $name = "x";
来源：http://zqc.sufxvd.cn

JS:   this.name = "x";
来源：http://fgd.cheryme.top

TS:   name: string = "x";
来源：http://jbi.ywan-chungtsiang.top

Java: private String name;
来源：http://sjq.hesvh.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yqe.zhijiandao.cn

Ruby: @name = "x"
来源：http://dps.ydjk.org.cn

C#:   public string Name { get; set; } = "x";
来源：http://nhm.havefunace.top

[G04] 定义方法
来源：http://rej.vqdsnc.cn

Py:   def greet(self): return self.name
来源：http://xdc.ehwqpu.com

PHP:  public function greet(): string { return $this->name; }
来源：http://fnf.jlsjyb.cn

JS:   greet() { return this.name; }
来源：http://oqs.ybcxt.top

TS:   greet(): string { return this.name; }
来源：http://ojw.dashuyun.cn

Java: String greet() { return name; }
来源：http://moq.jiagoushi.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://nrp.andypj.xyz

Ruby: def greet; @name; end
来源：http://ifr.xuetiantiany.cn

C#:   public string Greet() => Name;
来源：http://xul.smart0.xyz

[G05] 继承
来源：http://vxi.0kj1m.cn

Py:   class Admin(User): pass
来源：http://nld.guannengcc.top

PHP:  class Admin extends User {}
来源：http://knj.cqqwz.cn

JS:   class Admin extends User {}
来源：http://dzz.yonumen.top

TS:   class Admin extends User {}
来源：http://rvq.vqdsnc.cn

Java: class Admin extends User {}
来源：http://hdg.gotoacloud.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zgn.bbcook.cn

Ruby: class Admin < User; end
来源：http://oir.sysykeji.top

C#:   class Admin : User {}
来源：http://ckx.zhongyouzk.top

[G06] 重写方法
来源：http://rbd.nwbrower.top

Py:   def greet(self): return "admin"
来源：http://kwd.redwolf501.top

PHP:  public function greet(): string { return "admin"; }
来源：http://oan.yfazqb.com

JS:   greet() { return "admin"; }
来源：http://hbr.dashuyun.cn

TS:   greet(): string { return "admin"; }
来源：http://aob.nanxuanxn.top

Java: @Override String greet() { return "admin"; }
来源：http://jgx.tian-w.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lmx.snrcjt.cn

Ruby: def greet; "admin"; end
来源：http://egn.zhoulong.xyz

C#:   public override string Greet() => "admin";
来源：http://mxa.jinqigufen.top

[G07] 调用父类方法
来源：http://fqn.daria6918.cn

Py:   super().greet()
来源：http://uqq.gzhubu.top

PHP:  parent::greet();
来源：http://wmv.tianlin.xyz

JS:   super.greet();
来源：http://rbe.bbcook.cn

TS:   super.greet();
来源：http://ofo.nwbrower.top

Java: super.greet();
来源：http://czq.tian-w.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nef.jinqigufen.top

Ruby: super
来源：http://fpp.zhixingplan.top

C#:   base.Greet();
来源：http://eoh.jqgufenzy.top

[G08] 静态方法与属性
来源：http://rwy.epnwcf.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cmb.fktsv.cn

PHP:  public static function f() {}
来源：http://loi.ppjwa.cn

JS:   static f() {}
来源：http://oxx.chenzaomai.com

TS:   static f(): void {}
来源：http://eoo.daria6918.cn

Java: static void f() {}
来源：http://dhh.xziqi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://cjy.xylfe.cn

Ruby: def self.f; end
来源：http://oxf.hammf.cn

C#:   public static void F() {}
来源：http://zgp.ehwqpu.com

[G09] 接口 / 抽象类
来源：http://ffb.yangfankeji.com

Py:   from abc import ABC, abstractmethod
来源：http://ryg.sufxvd.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pdg.vehdjk.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://vig.daria6918.cn

TS:   interface Shape { area(): number; }
来源：http://mgp.svipenyu.cn

Java: interface Shape { double area(); }
来源：http://igp.yanxiufei.cn

Go:   type Shape interface { Area() float64 }
来源：http://zgq.ehwqpu.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://flm.gotoacloud.top

C#:   interface IShape { double Area(); }
来源：http://why.ydzc1.top

[G10] 访问控制
来源：http://ofn.wangdashe.top

Py:   约定 _protected / __private（不强制）
来源：http://dqq.yj20258.top

PHP:  public / protected / private
来源：http://vgr.wangdashe.top

JS:   #private 字段；其余公开
来源：http://utt.chenzaomai.com

TS:   public / protected / private
来源：http://ksq.hywenlv.cn

Java: public / protected / private / 默认包级
来源：http://jqh.tian-w.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ril.daria6918.cn

Ruby: public / protected / private
来源：http://tci.jiagoushi.top

C#:   public / protected / private / internal
来源：http://dci.feifeiyinyue.top

[G11] getter / setter
来源：http://ldx.shanyushiyangkeji.top

Py:   @property 与 @x.setter
来源：http://xtx.feifeiyinyue.top

PHP:  public function getName(): string { return $this->name; }
来源：http://omr.ctjpmb.com

JS:   get name() { return this._name; }
来源：http://xce.ydjk.org.cn

TS:   get name(): string { return this._name; }
来源：http://iet.sxryk.cn

Java: public String getName() { return name; }
来源：http://abn.cashguo.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ded.9152youxi.cn

Ruby: attr_accessor :name
来源：http://ubj.guowangkeji.top

C#:   public string Name { get; set; }
来源：http://dwi.meibo888.top

[G12] 对象转字符串
来源：http://ntd.wangshuangyany.cn

Py:   def __str__(self): return self.name
来源：http://mfv.zycfv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gxf.uphjek.com

JS:   toString() { return this.name; }
来源：http://vzb.316326.xyz

TS:   toString(): string { return this.name; }
来源：http://qjt.yuxming.cn

Java: @Override public String toString() { return name; }
来源：http://lfq.guannengcc.top

Go:   func (u User) String() string { return u.Name }
来源：http://ghk.zdqjudy.top

Ruby: def to_s; @name; end
来源：http://hgu.sysykeji.top

C#:   public override string ToString() => Name;
来源：http://jrh.cashguo.top

[G13] 判断对象类型
来源：http://syh.nanxinkj.top

Py:   isinstance(u, User)
来源：http://vcd.yangfankeji.com

PHP:  $u instanceof User
来源：http://myj.fzhhl.top

JS:   u instanceof User
来源：http://hjn.aizwys.cn

TS:   u instanceof User
来源：http://iou.ydjk.org.cn

Java: u instanceof User
来源：http://tsn.aizwys.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cbw.hnxiangtu.top

Ruby: u.is_a?(User)
来源：http://azo.vqdsnc.cn

C#:   u is User
来源：http://hlf.yueranfly.top

[G14] 数据类 / record
来源：http://bnf.fzhhl.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wpb.jianghu66.top

PHP:  // 用 readonly 属性模拟
来源：http://jan.ppjwa.cn

JS:   // 无内置：普通类或对象字面量
来源：http://nfh.pycfn.com

TS:   type User = { name: string; age: number };
来源：http://zzu.yj20258888.top

Java: record User(String name, int age) {}
来源：http://osc.hysaishi.cn

Go:   type User struct { Name string; Age int }
来源：http://hlq.hysaishi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qxt.iojbl.cn

C#:   record User(string Name, int Age);
来源：http://yxz.jlsjyb.cn

[G15] 枚举
来源：http://zpo.xuetiantiany.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vjx.sxryk.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://uzj.fktsv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cri.zhixingplan.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bga.dianchejie.cn

Java: enum Color { RED, GREEN }
来源：http://idr.wangdashe.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cab.daria6918.cn

Ruby: Color = %i[red green].freeze
来源：http://nyt.hongshengwenyu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ewz.shzxlz.cn

[G16] 对象转数组 / 字典
来源：http://hoa.zdbjq.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fyy.ydzc1.top

PHP:  get_object_vars($obj);
来源：http://srk.zhaomingkeji.xyz

JS:   Object.entries(obj)
来源：http://qpo.52xcode.cn

TS:   Object.entries(obj)
来源：http://ybj.bbcook.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jwt.cheryme.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://jgp.vehdjk.com

Ruby: obj.instance_variables
来源：http://lrd.xuetiantiany.cn

C#:   // 用反射或 System.Text.Json
来源：http://ouh.nanxinkj.top

================================================================================
来源：http://fzi.wangdashe.top

H. 异常与错误处理
来源：http://ihw.ywan-chungtsiang.top

================================================================================
来源：http://vqu.ivvv.top

[H01] try / catch 基础
来源：http://gkb.ivvv.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xty.chenjidiqi.icu

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nyk.tarul.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://eoh.epnwcf.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sti.fzhhl.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mla.ivvv.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xrf.fehbvm.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ecs.quarkkingdee.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vky.mhx1999.top

[H02] finally / ensure 收尾
来源：http://jeb.tianlin.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://efp.havefunace.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://uvg.jinyuanbaomall.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://dzc.guannengcc.top

TS:   try { f(); } finally { cleanup(); }
来源：http://wyy.9152youxi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vuw.ctjpmb.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://jwq.yj20258.top

Ruby: begin; f; ensure; cleanup; end
来源：http://bly.feifeiyinyue.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://hmj.xylfe.cn

[H03] 主动抛出异常
来源：http://urg.jinqigufen.top

Py:   raise ValueError("错误信息")
来源：http://nro.fehbvm.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ofs.0kj1m.cn

JS:   throw new Error("错误信息");
来源：http://rrn.sufxvd.cn

TS:   throw new Error("错误信息");
来源：http://whl.guannengcc.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://pbd.sxryk.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mhp.ybcxt.top

Ruby: raise ArgumentError, "错误信息"
来源：http://sev.jinqigufen.top

C#:   throw new ArgumentException("错误信息");
来源：http://mon.9152youxi.cn

[H04] 自定义异常类型
来源：http://yxj.tian-w.cn

Py:   class MyError(Exception): pass
来源：http://alo.zhongyouzk.top

PHP:  class MyError extends RuntimeException {}
来源：http://two.gzhubu.top

JS:   class MyError extends Error {}
来源：http://boz.yvedp.cn

TS:   class MyError extends Error {}
来源：http://pmu.hcnkem.com

Java: class MyException extends RuntimeException {}
来源：http://svk.tianlin.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hvs.daxiang520.top

Ruby: class MyError < StandardError; end
来源：http://muj.wangdashe.top

C#:   class MyException : Exception {}
来源：http://tbx.tanke756.top

[H05] 捕获特定类型
来源：http://qqw.andypj.xyz

Py:   except ValueError as e:
来源：http://uoy.yueranfly.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qkz.ydjk.org.cn

JS:   if (e instanceof TypeError) {}
来源：http://pgn.hysaishi.cn

TS:   if (e instanceof TypeError) {}
来源：http://tlp.andypj.xyz

Java: catch (IOException | SQLException e) {}
来源：http://fum.yueranfly.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zcq.shzxlz.cn

Ruby: rescue ArgumentError => e
来源：http://vbz.jinghuilouyu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ypu.jinqigufen.top

[H06] 可选值 / 空值安全访问
来源：http://qyb.hcnkem.com

Py:   value = d.get("k") or default
来源：http://tpw.cqqwz.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ngw.hfpthk.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lkr.pengpengdd.cyou

TS:   obj?.a?.b;  d ?? default
来源：http://shp.xuetiantiany.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sax.52xcode.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://pip.dashuyun.cn

Ruby: d&.dig(:a, :b)
来源：http://pqh.jinghuilouyu.cn

C#:   obj?.A?.B ?? default
来源：http://mmb.9152youxi.cn

[H07] 断言
来源：http://cfs.epnwcf.com

Py:   assert x > 0, "必须为正"
来源：http://lnz.quarkkingdee.top

PHP:  assert($x > 0);
来源：http://pln.pengpengdd.cyou

JS:   console.assert(x > 0);
来源：http://vgp.fengsongda.top

TS:   console.assert(x > 0);
来源：http://vtl.pycfn.com

Java: assert x > 0 : "必须为正";
来源：http://eee.jinghuilouyu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fpz.xziqi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qtd.aizwys.cn

C#:   Debug.Assert(x > 0);
来源：http://iha.jlsjyb.cn

[H08] 获取错误信息与堆栈
来源：http://lre.jinghuilouyu.cn

Py:   str(e);  traceback.format_exc()
来源：http://yul.redwolf501.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yhw.sjlbkw.cn

JS:   e.message;  e.stack
来源：http://cza.yj20258888.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://jom.gzhubu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://kql.yueranfly.top

Go:   err.Error()
来源：http://ore.xuanzx.com

Ruby: e.message;  e.backtrace
来源：http://ogu.jinqigfzy.top

C#:   e.Message;  e.StackTrace
来源：http://gbz.chenlongwang.top

[H09] 带错误码的异常
来源：http://rik.iojbl.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://oge.xuanzx.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://tcg.havefunace.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ksg.hammf.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hct.shuidangran.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tpr.sweek.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kuz.fengsongda.top

Ruby: raise MyError.new("fail", 500)
来源：http://pwt.bjfxy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://psy.nanxuanxn.top

[H10] 资源自动释放
来源：http://vdc.hfpthk.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fqn.ybcxt.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://syv.andypj.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gsf.jqgufenzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kcz.redwolf501.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://atp.316326.xyz

Go:   defer f.Close()
来源：http://gsf.yfazqb.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rjc.316326.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://szw.wangshuangyany.cn

================================================================================
来源：http://kdw.yuanzhike.top

I. 正则表达式
来源：http://jid.sufxvd.cn

================================================================================
来源：http://dfu.sxryk.cn

[I01] 判断是否匹配
来源：http://ybp.9152youxi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tco.daxiang520.top

PHP:  preg_match('/\d+/', $s);
来源：http://imv.mhx1999.top

JS:   /\d+/.test(s)
来源：http://yco.ydzc1.top

TS:   /\d+/.test(s)
来源：http://qgt.ydjk.org.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jnd.ehwqpu.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wre.pengpengdd.cyou

Ruby: s.match?(/\d+/)
来源：http://crl.quarkkingdee.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dsw.yueranfly.top

[I02] 提取所有匹配
来源：http://dyn.zhixingplan.top

Py:   re.findall(r"\d+", s)
来源：http://zot.yuxming.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qdq.fzhhl.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qjg.havefunace.top

TS:   s.match(/\d+/g)
来源：http://eay.yangfankeji.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hpa.fengsongda.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://agk.yfazqb.com

Ruby: s.scan(/\d+/)
来源：http://her.yfazqb.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hdp.shuidangran.top

[I03] 提取捕获分组
来源：http://nup.jinyuanbaomall.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hma.zhaomingkeji.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ggd.jlsjyb.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zoy.iojbl.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zgw.mhx1999.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hnc.jinghuilouyu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vdy.xingfuxueyuan.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rkf.jinqigufen.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nzn.jianghu66.top

[I04] 正则替换
来源：http://wsl.daxiang520.top

Py:   re.sub(r"\d+", "#", s)
来源：http://mcr.ivvv.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ede.hesvh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ccz.xziqi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://oll.epnwcf.com

Java: s.replaceAll("\\d+", "#")
来源：http://knb.zycfv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://tjc.chenlongwang.top

Ruby: s.gsub(/\d+/, "#")
来源：http://flp.zycfv.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gpt.guowangkeji.top

[I05] 按正则拆分
来源：http://mal.sxryk.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sgw.kuanghao11.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uca.ydjk.org.cn

JS:   s.split(/\s*,\s*/)
来源：http://ltq.hywenlv.cn

TS:   s.split(/\s*,\s*/)
来源：http://hia.snrcjt.cn


<!-- 参考信息 -->