代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oem.gaohongyu789.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://atd.gotoacloud.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dup.wangshuangyany.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hsb.tanke756.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bnh.wangshuangyany.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bkx.hammf.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gis.kuanghao11.cn

[F12] CSV 读写
来源：http://ktd.shanyushiyangkeji.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ykb.yj20258.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://psf.fktsv.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dqu.quarkkingdee.top

TS:   // 同上
来源：http://cjm.cucudq.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dxs.zhixingplan.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ako.smart0.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ngv.jiagoushi.top

C#:   // 无内置：用 CsvHelper 库
来源：http://lyd.vqdsnc.cn

================================================================================
来源：http://mnq.birdmap.top

G. 面向对象
来源：http://phg.kuanghao11.cn

================================================================================
来源：http://nec.jinyuanbaomall.cn

[G01] 定义类
来源：http://mbl.gaohongyu789.top

Py:   class User: pass
来源：http://ujq.snrcjt.cn

PHP:  class User {}
来源：http://oix.xuetiantiany.cn

JS:   class User {}
来源：http://fpz.jlsjyb.cn

TS:   class User { name: string = ""; }
来源：http://mli.xingfuxueyuan.xyz

Java: class User {}
来源：http://yjj.hnqzz.top

Go:   type User struct { Name string }
来源：http://qze.jinqigufen.top

Ruby: class User; end
来源：http://yzn.wangdashe.top

C#:   class User {}
来源：http://lij.sysykeji.top

[G02] 构造函数
来源：http://mlj.tarul.cn

Py:   def __init__(self, name): self.name = name
来源：http://urq.zhijiandao.cn

PHP:  public function __construct(public string $name) {}
来源：http://iww.smart0.xyz

JS:   constructor(name) { this.name = name; }
来源：http://prq.jinqigfzy.top

TS:   constructor(public name: string) {}
来源：http://oem.yongpay.top

Java: User(String name) { this.name = name; }
来源：http://kcy.guowangkeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gay.yfazqb.com

Ruby: def initialize(name); @name = name; end
来源：http://jqd.zycfv.cn

C#:   public User(string name) { Name = name; }
来源：http://obh.zhengqikj.top

[G03] 实例属性
来源：http://tet.cheryme.top

Py:   self.name = "x"
来源：http://nfy.52xcode.cn

PHP:  public string $name = "x";
来源：http://vpm.yongpay.top

JS:   this.name = "x";
来源：http://xee.iojbl.cn

TS:   name: string = "x";
来源：http://chf.dashuyun.cn

Java: private String name;
来源：http://lfw.9152youxi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fdq.sxryk.cn

Ruby: @name = "x"
来源：http://gnp.bjfxy.top

C#:   public string Name { get; set; } = "x";
来源：http://waf.uphjek.com

[G04] 定义方法
来源：http://utk.gotoacloud.top

Py:   def greet(self): return self.name
来源：http://nms.c1oappe.top

PHP:  public function greet(): string { return $this->name; }
来源：http://iiw.yj20258.top

JS:   greet() { return this.name; }
来源：http://bqj.meibo888.top

TS:   greet(): string { return this.name; }
来源：http://bvv.zycfv.cn

Java: String greet() { return name; }
来源：http://wll.zhongyouzk.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://phn.yongpay.top

Ruby: def greet; @name; end
来源：http://pth.zhengqikj.top

C#:   public string Greet() => Name;
来源：http://dcb.dianchejie.cn

[G05] 继承
来源：http://xyj.chenjidiqi.icu

Py:   class Admin(User): pass
来源：http://bzg.yongpay.top

PHP:  class Admin extends User {}
来源：http://pef.kuanghao11.cn

JS:   class Admin extends User {}
来源：http://fwg.zhoulong.xyz

TS:   class Admin extends User {}
来源：http://rji.nanxuanxn.top

Java: class Admin extends User {}
来源：http://xdz.aizwys.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://req.sjlbkw.cn

Ruby: class Admin < User; end
来源：http://gxu.fehbvm.com

C#:   class Admin : User {}
来源：http://czx.zhixingplan.top

[G06] 重写方法
来源：http://vwu.ctjpmb.com

Py:   def greet(self): return "admin"
来源：http://uto.havefunace.top

PHP:  public function greet(): string { return "admin"; }
来源：http://dao.nanxuanxn.top

JS:   greet() { return "admin"; }
来源：http://tky.316326.xyz

TS:   greet(): string { return "admin"; }
来源：http://san.uphjek.com

Java: @Override String greet() { return "admin"; }
来源：http://tfv.andypj.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jku.hesvh.cn

Ruby: def greet; "admin"; end
来源：http://frz.jiagoushi.top

C#:   public override string Greet() => "admin";
来源：http://cqx.cdnleiting.top

[G07] 调用父类方法
来源：http://mkw.svipenyu.cn

Py:   super().greet()
来源：http://bca.sysykeji.top

PHP:  parent::greet();
来源：http://ylo.iojbl.cn

JS:   super.greet();
来源：http://exg.shangyingyoupin.top

TS:   super.greet();
来源：http://bul.dianchejie.cn

Java: super.greet();
来源：http://aiq.snrcjt.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xdw.zhaomingkeji.xyz

Ruby: super
来源：http://rag.haohaochexian.top

C#:   base.Greet();
来源：http://cib.gaohongyu789.top

[G08] 静态方法与属性
来源：http://wdb.hfpthk.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xqi.mhx1999.top

PHP:  public static function f() {}
来源：http://awv.sjlbkw.cn

JS:   static f() {}
来源：http://ucv.jyoumei.cn

TS:   static f(): void {}
来源：http://rmn.mhx1999.top

Java: static void f() {}
来源：http://hco.yanxiufei.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bnj.zdqjudy.top

Ruby: def self.f; end
来源：http://zpj.zdqjudy.top

C#:   public static void F() {}
来源：http://bal.ydjk.org.cn

[G09] 接口 / 抽象类
来源：http://ckt.smart0.xyz

Py:   from abc import ABC, abstractmethod
来源：http://lyt.quarkkingdee.top

PHP:  interface Shape { public function area(): float; }
来源：http://pag.hysaishi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://amn.cheryme.top

TS:   interface Shape { area(): number; }
来源：http://nqw.gogol.net.cn

Java: interface Shape { double area(); }
来源：http://eye.vqdsnc.cn

Go:   type Shape interface { Area() float64 }
来源：http://yvy.shuidangran.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qvj.fehbvm.com

C#:   interface IShape { double Area(); }
来源：http://yyl.sufxvd.cn

[G10] 访问控制
来源：http://itt.hnqzz.top

Py:   约定 _protected / __private（不强制）
来源：http://tsm.guowangkeji.top

PHP:  public / protected / private
来源：http://fes.gogol.net.cn

JS:   #private 字段；其余公开
来源：http://bje.pycfn.com

TS:   public / protected / private
来源：http://ohn.kuanghao11.cn

Java: public / protected / private / 默认包级
来源：http://wzp.mhx1999.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://uzk.yfazqb.com

Ruby: public / protected / private
来源：http://qma.epnwcf.com

C#:   public / protected / private / internal
来源：http://rvt.hysaishi.cn

[G11] getter / setter
来源：http://tso.zhixingplan.top

Py:   @property 与 @x.setter
来源：http://abk.sysykeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dvz.cucudq.cn

JS:   get name() { return this._name; }
来源：http://gwp.nwbrower.top

TS:   get name(): string { return this._name; }
来源：http://fkf.gaohongyu789.top

Java: public String getName() { return name; }
来源：http://aun.meibo888.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://zte.sweek.top

Ruby: attr_accessor :name
来源：http://nnz.nwbrower.top

C#:   public string Name { get; set; }
来源：http://zhu.jinqigufen.top

[G12] 对象转字符串
来源：http://vcg.zdbjq.cn

Py:   def __str__(self): return self.name
来源：http://nkf.hysaishi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://eos.jinghuilouyu.cn

JS:   toString() { return this.name; }
来源：http://bne.hongshengwenyu.top

TS:   toString(): string { return this.name; }
来源：http://lny.haohaochexian.top

Java: @Override public String toString() { return name; }
来源：http://ahq.yongpay.top

Go:   func (u User) String() string { return u.Name }
来源：http://flu.yj20258888.top

Ruby: def to_s; @name; end
来源：http://nao.birdmap.top

C#:   public override string ToString() => Name;
来源：http://stw.shanyushiyangkeji.top

[G13] 判断对象类型
来源：http://dtp.shuidangran.top

Py:   isinstance(u, User)
来源：http://hku.kuanghao11.cn

PHP:  $u instanceof User
来源：http://rsn.snrcjt.cn

JS:   u instanceof User
来源：http://nhb.sufxvd.cn

TS:   u instanceof User
来源：http://tfv.jinyuanbaomall.cn

Java: u instanceof User
来源：http://mbr.ywan-chungtsiang.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://rdb.jinqigfzy.top

Ruby: u.is_a?(User)
来源：http://qqy.jianghu66.top

C#:   u is User
来源：http://clf.tanke756.top

[G14] 数据类 / record
来源：http://efd.bjfxy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dhc.yj20258888.top

PHP:  // 用 readonly 属性模拟
来源：http://bli.zdqjudy.top

JS:   // 无内置：普通类或对象字面量
来源：http://tsa.chenjidiqi.icu

TS:   type User = { name: string; age: number };
来源：http://fpx.cqqwz.cn

Java: record User(String name, int age) {}
来源：http://ljn.pycfn.com

Go:   type User struct { Name string; Age int }
来源：http://amr.jinghuilouyu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kxd.shuidangran.top

C#:   record User(string Name, int Age);
来源：http://cva.fanxiaobao.xyz

[G15] 枚举
来源：http://cjc.sxryk.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gsn.pycfn.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://jjz.yvedp.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://omm.tianlin.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hzi.shanyushiyangtech.top

Java: enum Color { RED, GREEN }
来源：http://ive.bbcook.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://szc.yvedp.cn

Ruby: Color = %i[red green].freeze
来源：http://gfp.gotoacloud.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bpi.ctjpmb.com

[G16] 对象转数组 / 字典
来源：http://jds.yueranfly.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ngn.epnwcf.com

PHP:  get_object_vars($obj);
来源：http://kaq.smart0.xyz

JS:   Object.entries(obj)
来源：http://mcq.zhixingplan.top

TS:   Object.entries(obj)
来源：http://wjk.haohaochexian.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nnt.havefunace.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://wyu.ehwqpu.com

Ruby: obj.instance_variables
来源：http://fhw.kuanghao11.cn

C#:   // 用反射或 System.Text.Json
来源：http://hst.bjfxy.top

================================================================================
来源：http://cdf.hammf.cn

H. 异常与错误处理
来源：http://soj.gotoacloud.top

================================================================================
来源：http://cwe.bjfxy.top

[H01] try / catch 基础
来源：http://pnb.tianlin.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wes.hcnkem.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fhk.cheryme.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tit.zdqjudy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://olf.hnqzz.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cil.fehbvm.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qfb.tianlin.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ala.jinghuilouyu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hqo.cashguo.top

[H02] finally / ensure 收尾
来源：http://dai.jinqigfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://tvs.cdnleiting.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://prm.hysaishi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wiz.daxiang520.top

TS:   try { f(); } finally { cleanup(); }
来源：http://rby.shuidangran.top

Java: try { f(); } finally { cleanup(); }
来源：http://yre.ywan-chungtsiang.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://uax.ehwqpu.com

Ruby: begin; f; ensure; cleanup; end
来源：http://dhi.shuidangran.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://guj.yj202588.top

[H03] 主动抛出异常
来源：http://pmg.cashguo.top

Py:   raise ValueError("错误信息")
来源：http://qmw.svipenyu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nys.jinyuanbaomall.cn

JS:   throw new Error("错误信息");
来源：http://qzy.gotoacloud.top

TS:   throw new Error("错误信息");
来源：http://yjg.yanxiufei.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ego.9152youxi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zvi.haohaochexian.top

Ruby: raise ArgumentError, "错误信息"
来源：http://nme.hesvh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vuv.ydjk.org.cn

[H04] 自定义异常类型
来源：http://hhs.xylfe.cn

Py:   class MyError(Exception): pass
来源：http://fjs.sjlbkw.cn

PHP:  class MyError extends RuntimeException {}
来源：http://lss.vqdsnc.cn

JS:   class MyError extends Error {}
来源：http://nrl.ctjpmb.com

TS:   class MyError extends Error {}
来源：http://ycr.tian-w.cn

Java: class MyException extends RuntimeException {}
来源：http://bmk.birdmap.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://itc.xuanzx.com

Ruby: class MyError < StandardError; end
来源：http://hrk.andypj.xyz

C#:   class MyException : Exception {}
来源：http://xhv.c1oappe.top

[H05] 捕获特定类型
来源：http://kzx.shanyushiyangkeji.top

Py:   except ValueError as e:
来源：http://vxt.xinyue.icu

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vfa.aibaodan.cn

JS:   if (e instanceof TypeError) {}
来源：http://dpu.iojbl.cn

TS:   if (e instanceof TypeError) {}
来源：http://pbn.yuanzhike.top

Java: catch (IOException | SQLException e) {}
来源：http://onh.chenlongwang.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hqk.shzxlz.cn

Ruby: rescue ArgumentError => e
来源：http://mhr.svipenyu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gbo.vqdsnc.cn

[H06] 可选值 / 空值安全访问
来源：http://sjj.ydjk.org.cn

Py:   value = d.get("k") or default
来源：http://kxd.c1oappe.top

PHP:  $v = $d["k"] ?? null;
来源：http://oiz.ppjwa.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lsr.haohaochexian.top

TS:   obj?.a?.b;  d ?? default
来源：http://adl.nwbrower.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hxl.sweek.top

Go:   if v, ok := m["k"]; ok { }
来源：http://oex.ivvv.top

Ruby: d&.dig(:a, :b)
来源：http://fkw.xziqi.cn

C#:   obj?.A?.B ?? default
来源：http://drp.havefunace.top

[H07] 断言
来源：http://usg.ivvv.top

Py:   assert x > 0, "必须为正"
来源：http://zua.sxryk.cn

PHP:  assert($x > 0);
来源：http://hap.cheryme.top

JS:   console.assert(x > 0);
来源：http://vcg.cashguo.top

TS:   console.assert(x > 0);
来源：http://vde.ybcxt.top

Java: assert x > 0 : "必须为正";
来源：http://dbc.zdbjq.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sje.svipenyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hby.xylfe.cn

C#:   Debug.Assert(x > 0);
来源：http://nuv.ydjk.org.cn

[H08] 获取错误信息与堆栈
来源：http://svn.yvedp.cn

Py:   str(e);  traceback.format_exc()
来源：http://bos.yuxming.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://drz.jiagoushi.top

JS:   e.message;  e.stack
来源：http://fkc.birdmap.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://lyq.daria6918.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xbm.hysaishi.cn

Go:   err.Error()
来源：http://mdd.fanxiaobao.xyz

Ruby: e.message;  e.backtrace
来源：http://edd.shanyushiyangtech.top

C#:   e.Message;  e.StackTrace
来源：http://xws.ywan-chungtsiang.top

[H09] 带错误码的异常
来源：http://czd.svipenyu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xha.jianghu66.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://rlv.ybcxt.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fvv.nanxinkj.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://eit.hysaishi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dsl.c1oappe.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hqi.zycfv.cn

Ruby: raise MyError.new("fail", 500)
来源：http://aqy.zhijiandao.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vja.redwolf501.top

[H10] 资源自动释放
来源：http://voq.shuidangran.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ila.shzxlz.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dgk.vehdjk.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fxa.hfpthk.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qmn.chenzaomai.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bmi.yvedp.cn

Go:   defer f.Close()
来源：http://jpi.dianchejie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hyk.yuanzhike.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qjr.yj202588.top

================================================================================
来源：http://jox.fanxiaobao.xyz

I. 正则表达式
来源：http://ikh.yanxiufei.cn

================================================================================
来源：http://fud.chenzaomai.com

[I01] 判断是否匹配
来源：http://akj.hfpthk.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://aef.mhx1999.top

PHP:  preg_match('/\d+/', $s);
来源：http://afa.jinqigufen.top

JS:   /\d+/.test(s)
来源：http://cpa.cqqwz.cn

TS:   /\d+/.test(s)
来源：http://ocv.aibaodan.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wkm.fktsv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tzo.hongshengwenyu.top

Ruby: s.match?(/\d+/)
来源：http://obq.quarkkingdee.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gbx.chenzaomai.com

[I02] 提取所有匹配
来源：http://xdp.tarul.cn

Py:   re.findall(r"\d+", s)
来源：http://xgh.hesvh.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ild.vqdsnc.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://igk.chenlongwang.top

TS:   s.match(/\d+/g)
来源：http://fhw.jinqigufen.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://aou.chenlongwang.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fxl.aizwys.cn

Ruby: s.scan(/\d+/)
来源：http://nfn.yuanzhike.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xyj.dianchejie.cn

[I03] 提取捕获分组
来源：http://gkv.bjfxy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://npf.fktsv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hsi.yonumen.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wdd.nanxuanxn.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rcc.gogol.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fuf.vehdjk.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xwk.yj20258888.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pwd.chenlongwang.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mip.yanxiufei.cn

[I04] 正则替换
来源：http://riu.aizwys.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://spj.xziqi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mpi.sysykeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://thg.yongpay.top

TS:   s.replace(/\d+/g, "#")
来源：http://mnr.havefunace.top

Java: s.replaceAll("\\d+", "#")
来源：http://glj.ywan-chungtsiang.top

Go:   re.ReplaceAllString(s, "#")
来源：http://pbi.guowangkeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://bvx.sjlbkw.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sdo.jqgfzy.top

[I05] 按正则拆分
来源：http://qdz.jinyuanbaomall.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ijt.bbcook.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://eai.ehwqpu.com

JS:   s.split(/\s*,\s*/)
来源：http://xjv.zhengqikj.top

TS:   s.split(/\s*,\s*/)
来源：http://sfh.aibaodan.cn


<!-- 参考信息 -->