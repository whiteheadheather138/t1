代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lll.meibo888.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mvf.havefunace.top

[F11] 复制与移动文件
来源：http://jqj.9152youxi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://apg.dianchejie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://aoc.tanke756.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fgr.fktsv.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jrh.yueranfly.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kvo.sweek.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qex.cheryme.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bep.cucudq.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qxg.aibaodan.cn

[F12] CSV 读写
来源：http://eke.ivvv.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yjg.pycfn.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pme.hnqzz.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qaq.cheryme.top

TS:   // 同上
来源：http://eaq.yuxming.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vwc.xylfe.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://buq.shuidangran.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vtf.bbcook.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://yez.bjfxy.top

================================================================================
来源：http://mxp.shanyushiyangkeji.top

G. 面向对象
来源：http://dte.daria6918.cn

================================================================================
来源：http://ehn.zycfv.cn

[G01] 定义类
来源：http://jpt.zdqjudy.top

Py:   class User: pass
来源：http://uiu.nanxuanxn.top

PHP:  class User {}
来源：http://jpy.ydjk.org.cn

JS:   class User {}
来源：http://rwp.yueranfly.top

TS:   class User { name: string = ""; }
来源：http://uat.guowangkeji.top

Java: class User {}
来源：http://hlt.bjfxy.top

Go:   type User struct { Name string }
来源：http://kfq.vqdsnc.cn

Ruby: class User; end
来源：http://dlp.yanxiufei.cn

C#:   class User {}
来源：http://ocu.jlsjyb.cn

[G02] 构造函数
来源：http://ain.c1oappe.top

Py:   def __init__(self, name): self.name = name
来源：http://pat.sxryk.cn

PHP:  public function __construct(public string $name) {}
来源：http://qhs.yanxiufei.cn

JS:   constructor(name) { this.name = name; }
来源：http://xou.jiagoushi.top

TS:   constructor(public name: string) {}
来源：http://xoz.zycfv.cn

Java: User(String name) { this.name = name; }
来源：http://kif.tian-w.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kdm.sweek.top

Ruby: def initialize(name); @name = name; end
来源：http://khv.gzhubu.top

C#:   public User(string name) { Name = name; }
来源：http://lbx.wangshuangyany.cn

[G03] 实例属性
来源：http://xcn.yuxming.cn

Py:   self.name = "x"
来源：http://flh.nanxuanxn.top

PHP:  public string $name = "x";
来源：http://drj.vehdjk.com

JS:   this.name = "x";
来源：http://mmb.yangfankeji.com

TS:   name: string = "x";
来源：http://xvb.yvedp.cn

Java: private String name;
来源：http://kyf.sysykeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hyo.yfazqb.com

Ruby: @name = "x"
来源：http://koe.yj202588.top

C#:   public string Name { get; set; } = "x";
来源：http://lkh.aibaodan.cn

[G04] 定义方法
来源：http://wpy.dashuyun.cn

Py:   def greet(self): return self.name
来源：http://fhu.zhoulong.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://lbd.nanxinkj.top

JS:   greet() { return this.name; }
来源：http://ubv.bjfxy.top

TS:   greet(): string { return this.name; }
来源：http://pwt.fanxiaobao.xyz

Java: String greet() { return name; }
来源：http://iar.fengsongda.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://mtt.nanxuanxn.top

Ruby: def greet; @name; end
来源：http://sla.zhijiandao.cn

C#:   public string Greet() => Name;
来源：http://xey.xuanzx.com

[G05] 继承
来源：http://iaa.yueranfly.top

Py:   class Admin(User): pass
来源：http://fzk.wangshuangyany.cn

PHP:  class Admin extends User {}
来源：http://tdm.snrcjt.cn

JS:   class Admin extends User {}
来源：http://qsp.yongpay.top

TS:   class Admin extends User {}
来源：http://bri.xuanzx.com

Java: class Admin extends User {}
来源：http://kte.xuetiantiany.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nht.jinqigufen.top

Ruby: class Admin < User; end
来源：http://kni.xinyue.icu

C#:   class Admin : User {}
来源：http://pcs.snrcjt.cn

[G06] 重写方法
来源：http://ocn.sysykeji.top

Py:   def greet(self): return "admin"
来源：http://lkx.chenjidiqi.icu

PHP:  public function greet(): string { return "admin"; }
来源：http://bow.sjlbkw.cn

JS:   greet() { return "admin"; }
来源：http://vdn.chenzaomai.com

TS:   greet(): string { return "admin"; }
来源：http://spn.sxryk.cn

Java: @Override String greet() { return "admin"; }
来源：http://awr.zhixingplan.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xct.shangyingyoupin.top

Ruby: def greet; "admin"; end
来源：http://mba.jianghu66.top

C#:   public override string Greet() => "admin";
来源：http://dza.shuidangran.top

[G07] 调用父类方法
来源：http://trc.zhaomingkeji.xyz

Py:   super().greet()
来源：http://ihw.gogol.net.cn

PHP:  parent::greet();
来源：http://dum.ywan-chungtsiang.top

JS:   super.greet();
来源：http://ngz.haohaochexian.top

TS:   super.greet();
来源：http://bpv.fzhhl.top

Java: super.greet();
来源：http://inp.yj202588.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ose.yueranfly.top

Ruby: super
来源：http://uja.hnxiangtu.top

C#:   base.Greet();
来源：http://dnl.guowangkeji.top

[G08] 静态方法与属性
来源：http://vpb.fengsongda.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://srh.yangfankeji.com

PHP:  public static function f() {}
来源：http://gxs.kuanghao11.cn

JS:   static f() {}
来源：http://gac.jyoumei.cn

TS:   static f(): void {}
来源：http://toi.jinyuanbaomall.cn

Java: static void f() {}
来源：http://ixr.jqgufenzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://goy.birdmap.top

Ruby: def self.f; end
来源：http://ene.fehbvm.com

C#:   public static void F() {}
来源：http://olh.smart0.xyz

[G09] 接口 / 抽象类
来源：http://mct.ybcxt.top

Py:   from abc import ABC, abstractmethod
来源：http://tzc.mhx1999.top

PHP:  interface Shape { public function area(): float; }
来源：http://iwb.vqdsnc.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ipg.chenzaomai.com

TS:   interface Shape { area(): number; }
来源：http://ind.shanyushiyangtech.top

Java: interface Shape { double area(); }
来源：http://nfz.sysykeji.top

Go:   type Shape interface { Area() float64 }
来源：http://rnk.gotoacloud.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qih.havefunace.top

C#:   interface IShape { double Area(); }
来源：http://ajq.jqgufenzy.top

[G10] 访问控制
来源：http://irk.gaohongyu789.top

Py:   约定 _protected / __private（不强制）
来源：http://ncc.sweek.top

PHP:  public / protected / private
来源：http://cue.hfpthk.cn

JS:   #private 字段；其余公开
来源：http://xhy.fktsv.cn

TS:   public / protected / private
来源：http://med.ybcxt.top

Java: public / protected / private / 默认包级
来源：http://noc.ybcxt.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://tah.0kj1m.cn

Ruby: public / protected / private
来源：http://zyj.ctjpmb.com

C#:   public / protected / private / internal
来源：http://tdc.feifeiyinyue.top

[G11] getter / setter
来源：http://nnz.jqgfzy.top

Py:   @property 与 @x.setter
来源：http://opg.andypj.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://lbz.cdnleiting.top

JS:   get name() { return this._name; }
来源：http://uct.shuidangran.top

TS:   get name(): string { return this._name; }
来源：http://qbt.9152youxi.cn

Java: public String getName() { return name; }
来源：http://hur.fzhhl.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://wnu.gaohongyu789.top

Ruby: attr_accessor :name
来源：http://izx.tianlin.xyz

C#:   public string Name { get; set; }
来源：http://laq.xingfuxueyuan.xyz

[G12] 对象转字符串
来源：http://eim.hesvh.cn

Py:   def __str__(self): return self.name
来源：http://oll.quarkkingdee.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ijj.shanyushiyangtech.top

JS:   toString() { return this.name; }
来源：http://jad.nanxuanxn.top

TS:   toString(): string { return this.name; }
来源：http://ctx.shanyushiyangkeji.top

Java: @Override public String toString() { return name; }
来源：http://uxv.andypj.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://kes.316326.xyz

Ruby: def to_s; @name; end
来源：http://qbq.yanxiufei.cn

C#:   public override string ToString() => Name;
来源：http://orz.smart0.xyz

[G13] 判断对象类型
来源：http://aur.cashguo.top

Py:   isinstance(u, User)
来源：http://yes.shanyushiyangtech.top

PHP:  $u instanceof User
来源：http://sqt.fengsongda.top

JS:   u instanceof User
来源：http://ljo.svipenyu.cn

TS:   u instanceof User
来源：http://zqa.9152youxi.cn

Java: u instanceof User
来源：http://vwo.zhengqikj.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://xvw.fehbvm.com

Ruby: u.is_a?(User)
来源：http://isj.andypj.xyz

C#:   u is User
来源：http://zrc.jyoumei.cn

[G14] 数据类 / record
来源：http://zer.hysaishi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qar.chenlongwang.top

PHP:  // 用 readonly 属性模拟
来源：http://wle.zdbjq.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qyf.ctjpmb.com

TS:   type User = { name: string; age: number };
来源：http://ykr.chenzaomai.com

Java: record User(String name, int age) {}
来源：http://hle.gotoacloud.top

Go:   type User struct { Name string; Age int }
来源：http://jyg.tanke756.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zve.guowangkeji.top

C#:   record User(string Name, int Age);
来源：http://tyh.hfpthk.cn

[G15] 枚举
来源：http://xcm.epnwcf.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xdx.dashuyun.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://yud.hnqzz.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mlq.hcnkem.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qso.wangshuangyany.cn

Java: enum Color { RED, GREEN }
来源：http://zsf.hfpthk.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gwv.yueranfly.top

Ruby: Color = %i[red green].freeze
来源：http://bsj.havefunace.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xcv.pycfn.com

[G16] 对象转数组 / 字典
来源：http://ovi.jinqigufen.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lth.dashuyun.cn

PHP:  get_object_vars($obj);
来源：http://tlw.jqgfzy.top

JS:   Object.entries(obj)
来源：http://zwb.sjlbkw.cn

TS:   Object.entries(obj)
来源：http://kgc.yvedp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mcd.svipenyu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://kqr.yangfankeji.com

Ruby: obj.instance_variables
来源：http://dqr.guannengcc.top

C#:   // 用反射或 System.Text.Json
来源：http://pkc.hongshengwenyu.top

================================================================================
来源：http://csk.xuanzx.com

H. 异常与错误处理
来源：http://drc.tian-w.cn

================================================================================
来源：http://czq.fengsongda.top

[H01] try / catch 基础
来源：http://lgc.nanxinkj.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dgm.jiagoushi.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qub.hesvh.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fne.kuanghao11.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://znl.hammf.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cye.sysykeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vxb.gaohongyu789.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lzt.guowangkeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zbe.cashguo.top

[H02] finally / ensure 收尾
来源：http://ufr.redwolf501.top

Py:   try: f()⏎finally: cleanup()
来源：http://cxz.316326.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://mpl.shangyingyoupin.top

JS:   try { f(); } finally { cleanup(); }
来源：http://zli.iojbl.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vkh.zhengqikj.top

Java: try { f(); } finally { cleanup(); }
来源：http://pjw.jyoumei.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qkf.9152youxi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ojx.gogol.net.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jyc.ehwqpu.com

[H03] 主动抛出异常
来源：http://clx.sxryk.cn

Py:   raise ValueError("错误信息")
来源：http://npt.cucudq.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mbr.cucudq.cn

JS:   throw new Error("错误信息");
来源：http://kpi.cheryme.top

TS:   throw new Error("错误信息");
来源：http://zdp.xylfe.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pji.dianchejie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://efp.tianlin.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://dwu.52xcode.cn

C#:   throw new ArgumentException("错误信息");
来源：http://inx.bjfxy.top

[H04] 自定义异常类型
来源：http://prp.sufxvd.cn

Py:   class MyError(Exception): pass
来源：http://yzk.cqqwz.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hsy.fehbvm.com

JS:   class MyError extends Error {}
来源：http://hja.yangfankeji.com

TS:   class MyError extends Error {}
来源：http://pqs.hcnkem.com

Java: class MyException extends RuntimeException {}
来源：http://vkb.dashuyun.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://iqo.cucudq.cn

Ruby: class MyError < StandardError; end
来源：http://zxi.vqdsnc.cn

C#:   class MyException : Exception {}
来源：http://mrr.yvedp.cn

[H05] 捕获特定类型
来源：http://mwz.guowangkeji.top

Py:   except ValueError as e:
来源：http://ppw.feifeiyinyue.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ncu.gzhubu.top

JS:   if (e instanceof TypeError) {}
来源：http://jmw.haohaochexian.top

TS:   if (e instanceof TypeError) {}
来源：http://itt.sysykeji.top

Java: catch (IOException | SQLException e) {}
来源：http://wpr.nanxinkj.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zan.zhiwuduotai.top

Ruby: rescue ArgumentError => e
来源：http://tne.dianchejie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pws.gaohongyu789.top

[H06] 可选值 / 空值安全访问
来源：http://wly.pengpengdd.cyou

Py:   value = d.get("k") or default
来源：http://fqk.zdbjq.cn

PHP:  $v = $d["k"] ?? null;
来源：http://aox.nwbrower.top

JS:   obj?.a?.b;  d ?? default
来源：http://col.yanxiufei.cn

TS:   obj?.a?.b;  d ?? default
来源：http://bwu.yuxming.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pqk.sufxvd.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://kyq.tanke756.top

Ruby: d&.dig(:a, :b)
来源：http://ouc.hongshengwenyu.top

C#:   obj?.A?.B ?? default
来源：http://cfi.fzhhl.top

[H07] 断言
来源：http://etk.cdnleiting.top

Py:   assert x > 0, "必须为正"
来源：http://nct.snrcjt.cn

PHP:  assert($x > 0);
来源：http://pvr.yueranfly.top

JS:   console.assert(x > 0);
来源：http://hqh.zdqjudy.top

TS:   console.assert(x > 0);
来源：http://zuu.jianghu66.top

Java: assert x > 0 : "必须为正";
来源：http://tzm.xingfuxueyuan.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ele.yvedp.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ozd.yangfankeji.com

C#:   Debug.Assert(x > 0);
来源：http://cvw.shanyushiyangtech.top

[H08] 获取错误信息与堆栈
来源：http://zlv.fzhhl.top

Py:   str(e);  traceback.format_exc()
来源：http://zvh.guowangkeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://iwi.guannengcc.top

JS:   e.message;  e.stack
来源：http://hta.tanke756.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://tqo.jianghu66.top

Java: e.getMessage();  e.printStackTrace()
来源：http://hmr.yj202588.top

Go:   err.Error()
来源：http://ddg.gogol.net.cn

Ruby: e.message;  e.backtrace
来源：http://cjg.zhijiandao.cn

C#:   e.Message;  e.StackTrace
来源：http://atp.bbcook.cn

[H09] 带错误码的异常
来源：http://gwn.bjfxy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pww.chenlongwang.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://vhd.smart0.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xfm.tian-w.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zda.hnqzz.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vum.feifeiyinyue.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://css.shzxlz.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wgy.zhaomingkeji.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://jmk.shanyushiyangkeji.top

[H10] 资源自动释放
来源：http://vix.tianlin.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://luz.gzhubu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tbu.gzhubu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://clf.9152youxi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gtp.nanxinkj.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://icc.jiagoushi.top

Go:   defer f.Close()
来源：http://rrp.zdqjudy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pvc.ydjk.org.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://avr.meibo888.top

================================================================================
来源：http://dct.gzhubu.top

I. 正则表达式
来源：http://ywl.birdmap.top

================================================================================
来源：http://atq.gzhubu.top

[I01] 判断是否匹配
来源：http://onx.bbcook.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fvw.havefunace.top

PHP:  preg_match('/\d+/', $s);
来源：http://efv.tanke756.top

JS:   /\d+/.test(s)
来源：http://lff.jyoumei.cn

TS:   /\d+/.test(s)
来源：http://kho.jqgufenzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sbv.yanxiufei.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ran.xylfe.cn

Ruby: s.match?(/\d+/)
来源：http://ugt.fanxiaobao.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ibg.zdbjq.cn

[I02] 提取所有匹配
来源：http://dvt.hfpthk.cn

Py:   re.findall(r"\d+", s)
来源：http://gcp.svipenyu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yhd.yuanzhike.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fob.yvedp.cn

TS:   s.match(/\d+/g)
来源：http://nat.ydjk.org.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://per.svipenyu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qfz.hnxiangtu.top

Ruby: s.scan(/\d+/)
来源：http://bgw.sysykeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://iyj.ywan-chungtsiang.top

[I03] 提取捕获分组
来源：http://ume.yvedp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://oud.sufxvd.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://oar.zhaomingkeji.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xwh.shzxlz.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cxm.jiagoushi.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rmo.gzhubu.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bat.pycfn.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cyd.0kj1m.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cbq.andypj.xyz

[I04] 正则替换
来源：http://isu.xuetiantiany.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ixw.yuanzhike.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tig.cqqwz.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cxd.yj20258888.top

TS:   s.replace(/\d+/g, "#")
来源：http://vtf.zhengqikj.top

Java: s.replaceAll("\\d+", "#")
来源：http://bgv.shanyushiyangtech.top

Go:   re.ReplaceAllString(s, "#")
来源：http://erm.bbcook.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zhk.yonumen.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nel.gaohongyu789.top

[I05] 按正则拆分
来源：http://vlg.ydjk.org.cn


<!-- 参考信息 -->