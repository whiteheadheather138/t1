代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uug.9152youxi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pko.9152youxi.cn

[F11] 复制与移动文件
来源：http://bey.daxiang520.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dwf.hcnkem.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bgp.chenzaomai.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kii.jiagoushi.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vfu.yvedp.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ijg.yj20258.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kap.xuetiantiany.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zgb.tian-w.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ubw.jiagoushi.top

[F12] CSV 读写
来源：http://yay.yj20258.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zve.zhaomingkeji.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rca.meibo888.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pcm.ydzc1.top

TS:   // 同上
来源：http://bmc.ehwqpu.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wft.zhengqikj.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://plu.shanyushiyangtech.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dai.daxiang520.top

C#:   // 无内置：用 CsvHelper 库
来源：http://fnx.dianchejie.cn

================================================================================
来源：http://gui.fehbvm.com

G. 面向对象
来源：http://okm.jqgufenzy.top

================================================================================
来源：http://exq.ydzc1.top

[G01] 定义类
来源：http://qec.shuidangran.top

Py:   class User: pass
来源：http://dxl.dianchejie.cn

PHP:  class User {}
来源：http://zsi.dianchejie.cn

JS:   class User {}
来源：http://xtz.yj20258888.top

TS:   class User { name: string = ""; }
来源：http://ngb.ehwqpu.com

Java: class User {}
来源：http://ddn.aibaodan.cn

Go:   type User struct { Name string }
来源：http://ntb.vehdjk.com

Ruby: class User; end
来源：http://dcx.jianghu66.top

C#:   class User {}
来源：http://nku.redwolf501.top

[G02] 构造函数
来源：http://pkq.fktsv.cn

Py:   def __init__(self, name): self.name = name
来源：http://tax.yuanzhike.top

PHP:  public function __construct(public string $name) {}
来源：http://nrx.chenjidiqi.icu

JS:   constructor(name) { this.name = name; }
来源：http://kjg.jiagoushi.top

TS:   constructor(public name: string) {}
来源：http://rpm.jinyuanbaomall.cn

Java: User(String name) { this.name = name; }
来源：http://yyd.vqdsnc.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://crz.yueranfly.top

Ruby: def initialize(name); @name = name; end
来源：http://qbr.jinghuilouyu.cn

C#:   public User(string name) { Name = name; }
来源：http://lox.sweek.top

[G03] 实例属性
来源：http://cin.jinyuanbaomall.cn

Py:   self.name = "x"
来源：http://ync.guowangkeji.top

PHP:  public string $name = "x";
来源：http://dao.hnxiangtu.top

JS:   this.name = "x";
来源：http://kcb.fzhhl.top

TS:   name: string = "x";
来源：http://gqx.hnqzz.top

Java: private String name;
来源：http://tyc.xylfe.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gxm.yj20258.top

Ruby: @name = "x"
来源：http://anr.sweek.top

C#:   public string Name { get; set; } = "x";
来源：http://uyd.snrcjt.cn

[G04] 定义方法
来源：http://jfk.shanyushiyangkeji.top

Py:   def greet(self): return self.name
来源：http://byh.sweek.top

PHP:  public function greet(): string { return $this->name; }
来源：http://unt.vehdjk.com

JS:   greet() { return this.name; }
来源：http://tpv.yj202588.top

TS:   greet(): string { return this.name; }
来源：http://vwl.hywenlv.cn

Java: String greet() { return name; }
来源：http://rxv.yj20258.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://zbt.fzhhl.top

Ruby: def greet; @name; end
来源：http://cpm.hnqzz.top

C#:   public string Greet() => Name;
来源：http://pxy.chenlongwang.top

[G05] 继承
来源：http://wyr.quarkkingdee.top

Py:   class Admin(User): pass
来源：http://ula.shzxlz.cn

PHP:  class Admin extends User {}
来源：http://ffe.xziqi.cn

JS:   class Admin extends User {}
来源：http://bmm.xuetiantiany.cn

TS:   class Admin extends User {}
来源：http://rsx.jiagoushi.top

Java: class Admin extends User {}
来源：http://vvv.c1oappe.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://key.yangfankeji.com

Ruby: class Admin < User; end
来源：http://pnb.yuxming.cn

C#:   class Admin : User {}
来源：http://pcw.andypj.xyz

[G06] 重写方法
来源：http://iee.cheryme.top

Py:   def greet(self): return "admin"
来源：http://vyk.xuetiantiany.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://imx.xuanzx.com

JS:   greet() { return "admin"; }
来源：http://dfj.haohaochexian.top

TS:   greet(): string { return "admin"; }
来源：http://vtd.cashguo.top

Java: @Override String greet() { return "admin"; }
来源：http://jlt.hnxiangtu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ifj.ydzc1.top

Ruby: def greet; "admin"; end
来源：http://kol.daria6918.cn

C#:   public override string Greet() => "admin";
来源：http://fvc.cucudq.cn

[G07] 调用父类方法
来源：http://bxb.hongshengwenyu.top

Py:   super().greet()
来源：http://qxl.gotoacloud.top

PHP:  parent::greet();
来源：http://oqy.zhixingplan.top

JS:   super.greet();
来源：http://vmo.ppjwa.cn

TS:   super.greet();
来源：http://yvn.hnxiangtu.top

Java: super.greet();
来源：http://gxy.vehdjk.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yli.jqgufenzy.top

Ruby: super
来源：http://akh.yuxming.cn

C#:   base.Greet();
来源：http://iwo.yj20258888.top

[G08] 静态方法与属性
来源：http://lyx.ybcxt.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ees.zdbjq.cn

PHP:  public static function f() {}
来源：http://nbe.xingfuxueyuan.xyz

JS:   static f() {}
来源：http://ahy.yj20258888.top

TS:   static f(): void {}
来源：http://jkc.ctjpmb.com

Java: static void f() {}
来源：http://lju.yanxiufei.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://opa.xuanzx.com

Ruby: def self.f; end
来源：http://epl.havefunace.top

C#:   public static void F() {}
来源：http://esa.gogol.net.cn

[G09] 接口 / 抽象类
来源：http://tmu.nanxuanxn.top

Py:   from abc import ABC, abstractmethod
来源：http://mzx.yuxming.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ttr.zhengqikj.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://uvo.hywenlv.cn

TS:   interface Shape { area(): number; }
来源：http://trd.9152youxi.cn

Java: interface Shape { double area(); }
来源：http://fjw.shuidangran.top

Go:   type Shape interface { Area() float64 }
来源：http://vwf.daria6918.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zyn.hnqzz.top

C#:   interface IShape { double Area(); }
来源：http://rwc.hongshengwenyu.top

[G10] 访问控制
来源：http://ewd.pycfn.com

Py:   约定 _protected / __private（不强制）
来源：http://ipq.ywan-chungtsiang.top

PHP:  public / protected / private
来源：http://hgh.hysaishi.cn

JS:   #private 字段；其余公开
来源：http://xss.bbcook.cn

TS:   public / protected / private
来源：http://gde.hammf.cn

Java: public / protected / private / 默认包级
来源：http://sds.fzhhl.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://huv.kuanghao11.cn

Ruby: public / protected / private
来源：http://irk.jyoumei.cn

C#:   public / protected / private / internal
来源：http://gac.gzhubu.top

[G11] getter / setter
来源：http://jnb.yvedp.cn

Py:   @property 与 @x.setter
来源：http://kte.kuanghao11.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jog.feifeiyinyue.top

JS:   get name() { return this._name; }
来源：http://gfe.cdnleiting.top

TS:   get name(): string { return this._name; }
来源：http://qcx.tarul.cn

Java: public String getName() { return name; }
来源：http://vmd.sxryk.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://nnd.zhoulong.xyz

Ruby: attr_accessor :name
来源：http://cbm.wangshuangyany.cn

C#:   public string Name { get; set; }
来源：http://zuj.yongpay.top

[G12] 对象转字符串
来源：http://kvr.shangyingyoupin.top

Py:   def __str__(self): return self.name
来源：http://pjk.yvedp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rdf.bbcook.cn

JS:   toString() { return this.name; }
来源：http://yce.316326.xyz

TS:   toString(): string { return this.name; }
来源：http://vql.meibo888.top

Java: @Override public String toString() { return name; }
来源：http://zey.ydjk.org.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mqv.fengsongda.top

Ruby: def to_s; @name; end
来源：http://zmh.bbcook.cn

C#:   public override string ToString() => Name;
来源：http://hyv.chenzaomai.com

[G13] 判断对象类型
来源：http://xil.yj202588.top

Py:   isinstance(u, User)
来源：http://bha.jianghu66.top

PHP:  $u instanceof User
来源：http://ljo.aibaodan.cn

JS:   u instanceof User
来源：http://fcz.fzhhl.top

TS:   u instanceof User
来源：http://gmj.kuanghao11.cn

Java: u instanceof User
来源：http://nkl.andypj.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://ova.wangdashe.top

Ruby: u.is_a?(User)
来源：http://kez.sysykeji.top

C#:   u is User
来源：http://lqb.ctjpmb.com

[G14] 数据类 / record
来源：http://bzx.c1oappe.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uym.gaohongyu789.top

PHP:  // 用 readonly 属性模拟
来源：http://jcl.jqgufenzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://fky.yangfankeji.com

TS:   type User = { name: string; age: number };
来源：http://rqn.ppjwa.cn

Java: record User(String name, int age) {}
来源：http://lgx.jiagoushi.top

Go:   type User struct { Name string; Age int }
来源：http://ndm.yueranfly.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qsi.shanyushiyangkeji.top

C#:   record User(string Name, int Age);
来源：http://rvt.yonumen.top

[G15] 枚举
来源：http://uyn.cheryme.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wrr.yonumen.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://qzr.meibo888.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tkw.hnxiangtu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wpj.ywan-chungtsiang.top

Java: enum Color { RED, GREEN }
来源：http://xif.iojbl.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://afl.xinyue.icu

Ruby: Color = %i[red green].freeze
来源：http://vxl.xylfe.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nnu.gogol.net.cn

[G16] 对象转数组 / 字典
来源：http://ghu.fehbvm.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zsm.shanyushiyangkeji.top

PHP:  get_object_vars($obj);
来源：http://koc.wangdashe.top

JS:   Object.entries(obj)
来源：http://qhi.hcnkem.com

TS:   Object.entries(obj)
来源：http://gwh.havefunace.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://daw.cdnleiting.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://coe.tianlin.xyz

Ruby: obj.instance_variables
来源：http://wdo.yueranfly.top

C#:   // 用反射或 System.Text.Json
来源：http://sjg.sxryk.cn

================================================================================
来源：http://yjx.zdqjudy.top

H. 异常与错误处理
来源：http://ahg.tianlin.xyz

================================================================================
来源：http://lxr.fengsongda.top

[H01] try / catch 基础
来源：http://kug.hongshengwenyu.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://drr.yfazqb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://efd.aizwys.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tul.ydzc1.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ywf.quarkkingdee.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://clx.fehbvm.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jut.jlsjyb.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://irk.yvedp.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oak.zhijiandao.cn

[H02] finally / ensure 收尾
来源：http://mwg.aibaodan.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vif.wangshuangyany.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://rof.zhongyouzk.top

JS:   try { f(); } finally { cleanup(); }
来源：http://hne.yuxming.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://oft.shanyushiyangkeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://rhj.iojbl.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qhf.hnqzz.top

Ruby: begin; f; ensure; cleanup; end
来源：http://dfp.sweek.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://cab.shanyushiyangtech.top

[H03] 主动抛出异常
来源：http://mkk.hysaishi.cn

Py:   raise ValueError("错误信息")
来源：http://fzd.havefunace.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bep.sxryk.cn

JS:   throw new Error("错误信息");
来源：http://eef.9152youxi.cn

TS:   throw new Error("错误信息");
来源：http://rna.mhx1999.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://dey.tarul.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://weu.shzxlz.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ouy.chenlongwang.top

C#:   throw new ArgumentException("错误信息");
来源：http://ipy.shzxlz.cn

[H04] 自定义异常类型
来源：http://kng.xuanzx.com

Py:   class MyError(Exception): pass
来源：http://avd.andypj.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://wga.xziqi.cn

JS:   class MyError extends Error {}
来源：http://zjq.hnxiangtu.top

TS:   class MyError extends Error {}
来源：http://kyx.jinqigufen.top

Java: class MyException extends RuntimeException {}
来源：http://sqj.yanxiufei.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dyr.uphjek.com

Ruby: class MyError < StandardError; end
来源：http://aky.sxryk.cn

C#:   class MyException : Exception {}
来源：http://rey.jlsjyb.cn

[H05] 捕获特定类型
来源：http://dbo.nanxuanxn.top

Py:   except ValueError as e:
来源：http://gcl.fktsv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kef.mhx1999.top

JS:   if (e instanceof TypeError) {}
来源：http://mye.yuxming.cn

TS:   if (e instanceof TypeError) {}
来源：http://mzw.cdnleiting.top

Java: catch (IOException | SQLException e) {}
来源：http://jjo.fanxiaobao.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jmi.shanyushiyangtech.top

Ruby: rescue ArgumentError => e
来源：http://gjw.hammf.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tye.cqqwz.cn

[H06] 可选值 / 空值安全访问
来源：http://ezf.shanyushiyangkeji.top

Py:   value = d.get("k") or default
来源：http://rzs.c1oappe.top

PHP:  $v = $d["k"] ?? null;
来源：http://nog.mhx1999.top

JS:   obj?.a?.b;  d ?? default
来源：http://kna.zdbjq.cn

TS:   obj?.a?.b;  d ?? default
来源：http://gle.zhaomingkeji.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://slh.yuxming.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://rcv.zhongyouzk.top

Ruby: d&.dig(:a, :b)
来源：http://kzd.pycfn.com

C#:   obj?.A?.B ?? default
来源：http://isl.daxiang520.top

[H07] 断言
来源：http://hcg.jlsjyb.cn

Py:   assert x > 0, "必须为正"
来源：http://uiz.hongshengwenyu.top

PHP:  assert($x > 0);
来源：http://ufw.epnwcf.com

JS:   console.assert(x > 0);
来源：http://zhy.yangfankeji.com

TS:   console.assert(x > 0);
来源：http://lnr.zhoulong.xyz

Java: assert x > 0 : "必须为正";
来源：http://cej.shuidangran.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lkg.fzhhl.top

Ruby: raise "必须为正" unless x > 0
来源：http://syz.aizwys.cn

C#:   Debug.Assert(x > 0);
来源：http://tzf.hcnkem.com

[H08] 获取错误信息与堆栈
来源：http://mut.chenlongwang.top

Py:   str(e);  traceback.format_exc()
来源：http://haw.zhijiandao.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gvd.hnxiangtu.top

JS:   e.message;  e.stack
来源：http://ctc.gaohongyu789.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://bot.jqgufenzy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://pqd.birdmap.top

Go:   err.Error()
来源：http://jsy.fengsongda.top

Ruby: e.message;  e.backtrace
来源：http://qyt.sweek.top

C#:   e.Message;  e.StackTrace
来源：http://rxw.gaohongyu789.top

[H09] 带错误码的异常
来源：http://kdl.jiagoushi.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://azy.gaohongyu789.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ygb.zhiwuduotai.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kkp.uphjek.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://aia.aizwys.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yhs.jinghuilouyu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yhl.sweek.top

Ruby: raise MyError.new("fail", 500)
来源：http://lip.9152youxi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xqm.uphjek.com

[H10] 资源自动释放
来源：http://ohu.zhixingplan.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://kli.gogol.net.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ajl.ehwqpu.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zkj.yj20258.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sim.sjlbkw.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tkq.shangyingyoupin.top

Go:   defer f.Close()
来源：http://gyo.0kj1m.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lnk.xuetiantiany.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xup.ivvv.top

================================================================================
来源：http://uss.kuanghao11.cn

I. 正则表达式
来源：http://bkf.zhoulong.xyz

================================================================================
来源：http://wof.0kj1m.cn

[I01] 判断是否匹配
来源：http://meg.uphjek.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kcc.tian-w.cn

PHP:  preg_match('/\d+/', $s);
来源：http://exi.yanxiufei.cn

JS:   /\d+/.test(s)
来源：http://spv.hammf.cn

TS:   /\d+/.test(s)
来源：http://iqw.xziqi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rze.xziqi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dab.guowangkeji.top

Ruby: s.match?(/\d+/)
来源：http://ujo.9152youxi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://shj.zhiwuduotai.top

[I02] 提取所有匹配
来源：http://fui.haohaochexian.top

Py:   re.findall(r"\d+", s)
来源：http://hvx.chenjidiqi.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ciu.yj20258888.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lvf.guowangkeji.top

TS:   s.match(/\d+/g)
来源：http://mxi.yanxiufei.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://iht.xinyue.icu

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pvf.yueranfly.top

Ruby: s.scan(/\d+/)
来源：http://zdf.fehbvm.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wpl.tianlin.xyz

[I03] 提取捕获分组
来源：http://hkd.hongshengwenyu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gpu.xuetiantiany.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://anf.hywenlv.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dis.chenjidiqi.icu

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://biw.mhx1999.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tpn.daria6918.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mdj.zhongyouzk.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xgq.jlsjyb.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gwv.sysykeji.top

[I04] 正则替换
来源：http://tcx.gzhubu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://frv.vehdjk.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sio.zhiwuduotai.top

JS:   s.replace(/\d+/g, "#")
来源：http://xyo.hammf.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wfe.hcnkem.com

Java: s.replaceAll("\\d+", "#")
来源：http://rsu.9152youxi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://iyb.yj202588.top

Ruby: s.gsub(/\d+/, "#")
来源：http://rrk.jlsjyb.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qjb.uphjek.com

[I05] 按正则拆分
来源：http://ezq.yvedp.cn


<!-- 参考信息 -->