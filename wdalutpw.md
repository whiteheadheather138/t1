代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://soc.xuetiantiany.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jnl.yuanzhike.top

[F11] 复制与移动文件
来源：http://gmw.hnxiangtu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gvr.cdnleiting.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://two.yueranfly.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hyg.52xcode.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dsu.hysaishi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lkb.gzhubu.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jrd.0kj1m.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ugi.hysaishi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yic.jinghuilouyu.cn

[F12] CSV 读写
来源：http://iob.shanyushiyangkeji.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vrb.kuanghao11.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vxt.gaohongyu789.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://clw.hammf.cn

TS:   // 同上
来源：http://xba.c1oappe.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nci.yangfankeji.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dxk.cheryme.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wal.xziqi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ruj.ydzc1.top

================================================================================
来源：http://xwo.cucudq.cn

G. 面向对象
来源：http://beg.zycfv.cn

================================================================================
来源：http://ivf.zhaomingkeji.xyz

[G01] 定义类
来源：http://woj.feifeiyinyue.top

Py:   class User: pass
来源：http://kbh.svipenyu.cn

PHP:  class User {}
来源：http://oum.hnxiangtu.top

JS:   class User {}
来源：http://khj.tarul.cn

TS:   class User { name: string = ""; }
来源：http://udr.ppjwa.cn

Java: class User {}
来源：http://zhd.quarkkingdee.top

Go:   type User struct { Name string }
来源：http://qmh.yvedp.cn

Ruby: class User; end
来源：http://fdc.shzxlz.cn

C#:   class User {}
来源：http://knd.tianlin.xyz

[G02] 构造函数
来源：http://cdj.gogol.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://dbs.hysaishi.cn

PHP:  public function __construct(public string $name) {}
来源：http://qwe.xziqi.cn

JS:   constructor(name) { this.name = name; }
来源：http://yrs.ywan-chungtsiang.top

TS:   constructor(public name: string) {}
来源：http://pvl.zhixingplan.top

Java: User(String name) { this.name = name; }
来源：http://lxo.fzhhl.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rdq.aizwys.cn

Ruby: def initialize(name); @name = name; end
来源：http://srq.ydjk.org.cn

C#:   public User(string name) { Name = name; }
来源：http://zqx.epnwcf.com

[G03] 实例属性
来源：http://eiz.smart0.xyz

Py:   self.name = "x"
来源：http://eam.xziqi.cn

PHP:  public string $name = "x";
来源：http://uep.nwbrower.top

JS:   this.name = "x";
来源：http://cno.redwolf501.top

TS:   name: string = "x";
来源：http://xxa.gzhubu.top

Java: private String name;
来源：http://kmj.fzhhl.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dfl.fanxiaobao.xyz

Ruby: @name = "x"
来源：http://aae.xingfuxueyuan.xyz

C#:   public string Name { get; set; } = "x";
来源：http://cwx.jinqigufen.top

[G04] 定义方法
来源：http://nlw.gzhubu.top

Py:   def greet(self): return self.name
来源：http://nps.fktsv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tkz.ybcxt.top

JS:   greet() { return this.name; }
来源：http://iui.zdbjq.cn

TS:   greet(): string { return this.name; }
来源：http://pqr.zhijiandao.cn

Java: String greet() { return name; }
来源：http://wlh.316326.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://kcj.ybcxt.top

Ruby: def greet; @name; end
来源：http://smz.andypj.xyz

C#:   public string Greet() => Name;
来源：http://fwe.xinyue.icu

[G05] 继承
来源：http://eot.jiagoushi.top

Py:   class Admin(User): pass
来源：http://zig.meibo888.top

PHP:  class Admin extends User {}
来源：http://kwt.yfazqb.com

JS:   class Admin extends User {}
来源：http://oqg.hnqzz.top

TS:   class Admin extends User {}
来源：http://mya.snrcjt.cn

Java: class Admin extends User {}
来源：http://gkm.shuidangran.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://oot.sxryk.cn

Ruby: class Admin < User; end
来源：http://zad.meibo888.top

C#:   class Admin : User {}
来源：http://dzq.guowangkeji.top

[G06] 重写方法
来源：http://xrh.jyoumei.cn

Py:   def greet(self): return "admin"
来源：http://hmd.wangdashe.top

PHP:  public function greet(): string { return "admin"; }
来源：http://rvt.pengpengdd.cyou

JS:   greet() { return "admin"; }
来源：http://jzt.zhaomingkeji.xyz

TS:   greet(): string { return "admin"; }
来源：http://ucf.birdmap.top

Java: @Override String greet() { return "admin"; }
来源：http://wah.bjfxy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://boy.xingfuxueyuan.xyz

Ruby: def greet; "admin"; end
来源：http://fwa.yuxming.cn

C#:   public override string Greet() => "admin";
来源：http://aut.zdbjq.cn

[G07] 调用父类方法
来源：http://yby.hcnkem.com

Py:   super().greet()
来源：http://eol.ydzc1.top

PHP:  parent::greet();
来源：http://ujg.meibo888.top

JS:   super.greet();
来源：http://msh.tian-w.cn

TS:   super.greet();
来源：http://ekr.c1oappe.top

Java: super.greet();
来源：http://qqk.iojbl.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kws.zhengqikj.top

Ruby: super
来源：http://rld.chenjidiqi.icu

C#:   base.Greet();
来源：http://enh.gaohongyu789.top

[G08] 静态方法与属性
来源：http://maz.feifeiyinyue.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jrh.tianlin.xyz

PHP:  public static function f() {}
来源：http://vwp.tianlin.xyz

JS:   static f() {}
来源：http://dtp.yj20258888.top

TS:   static f(): void {}
来源：http://yok.guowangkeji.top

Java: static void f() {}
来源：http://skz.cucudq.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pic.yj20258.top

Ruby: def self.f; end
来源：http://svu.tian-w.cn

C#:   public static void F() {}
来源：http://yoq.tian-w.cn

[G09] 接口 / 抽象类
来源：http://cev.9152youxi.cn

Py:   from abc import ABC, abstractmethod
来源：http://stt.hysaishi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://npz.vehdjk.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://ewt.hysaishi.cn

TS:   interface Shape { area(): number; }
来源：http://ylq.cqqwz.cn

Java: interface Shape { double area(); }
来源：http://nld.ydzc1.top

Go:   type Shape interface { Area() float64 }
来源：http://hib.ydjk.org.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wnj.aibaodan.cn

C#:   interface IShape { double Area(); }
来源：http://ext.yj20258.top

[G10] 访问控制
来源：http://ume.epnwcf.com

Py:   约定 _protected / __private（不强制）
来源：http://zco.aibaodan.cn

PHP:  public / protected / private
来源：http://tvk.jinqigufen.top

JS:   #private 字段；其余公开
来源：http://urk.bjfxy.top

TS:   public / protected / private
来源：http://hty.hcnkem.com

Java: public / protected / private / 默认包级
来源：http://zcv.tarul.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ljh.yj202588.top

Ruby: public / protected / private
来源：http://dnn.quarkkingdee.top

C#:   public / protected / private / internal
来源：http://kvh.52xcode.cn

[G11] getter / setter
来源：http://kzt.316326.xyz

Py:   @property 与 @x.setter
来源：http://ate.dianchejie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://omx.shanyushiyangtech.top

JS:   get name() { return this._name; }
来源：http://yxd.jinghuilouyu.cn

TS:   get name(): string { return this._name; }
来源：http://hgt.yanxiufei.cn

Java: public String getName() { return name; }
来源：http://yli.ehwqpu.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://sfy.zhixingplan.top

Ruby: attr_accessor :name
来源：http://zuu.zycfv.cn

C#:   public string Name { get; set; }
来源：http://mwv.zhengqikj.top

[G12] 对象转字符串
来源：http://ktb.bbcook.cn

Py:   def __str__(self): return self.name
来源：http://xwa.xuanzx.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://dte.bjfxy.top

JS:   toString() { return this.name; }
来源：http://uju.yueranfly.top

TS:   toString(): string { return this.name; }
来源：http://nbl.bjfxy.top

Java: @Override public String toString() { return name; }
来源：http://miu.hfpthk.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vtz.hywenlv.cn

Ruby: def to_s; @name; end
来源：http://ziv.daxiang520.top

C#:   public override string ToString() => Name;
来源：http://cbl.gzhubu.top

[G13] 判断对象类型
来源：http://ink.ivvv.top

Py:   isinstance(u, User)
来源：http://suq.yfazqb.com

PHP:  $u instanceof User
来源：http://lmw.bbcook.cn

JS:   u instanceof User
来源：http://gtg.gogol.net.cn

TS:   u instanceof User
来源：http://tfk.shangyingyoupin.top

Java: u instanceof User
来源：http://izo.fehbvm.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://gct.chenzaomai.com

Ruby: u.is_a?(User)
来源：http://dxa.bjfxy.top

C#:   u is User
来源：http://boq.c1oappe.top

[G14] 数据类 / record
来源：http://ymm.xziqi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yad.c1oappe.top

PHP:  // 用 readonly 属性模拟
来源：http://waz.jqgufenzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://iji.zycfv.cn

TS:   type User = { name: string; age: number };
来源：http://jrf.havefunace.top

Java: record User(String name, int age) {}
来源：http://eqn.wangshuangyany.cn

Go:   type User struct { Name string; Age int }
来源：http://clw.chenlongwang.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://css.gaohongyu789.top

C#:   record User(string Name, int Age);
来源：http://yrp.nwbrower.top

[G15] 枚举
来源：http://bne.ctjpmb.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://iij.fengsongda.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ari.hesvh.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mtx.xuanzx.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qwc.zhixingplan.top

Java: enum Color { RED, GREEN }
来源：http://khr.yj20258.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://krk.ybcxt.top

Ruby: Color = %i[red green].freeze
来源：http://ubc.svipenyu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tcq.gzhubu.top

[G16] 对象转数组 / 字典
来源：http://xbp.xingfuxueyuan.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pzd.sxryk.cn

PHP:  get_object_vars($obj);
来源：http://okg.jianghu66.top

JS:   Object.entries(obj)
来源：http://snt.shzxlz.cn

TS:   Object.entries(obj)
来源：http://vcq.zdqjudy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ced.ydjk.org.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hlt.nanxuanxn.top

Ruby: obj.instance_variables
来源：http://zsz.xingfuxueyuan.xyz

C#:   // 用反射或 System.Text.Json
来源：http://mds.zhengqikj.top

================================================================================
来源：http://gjd.fzhhl.top

H. 异常与错误处理
来源：http://los.sweek.top

================================================================================
来源：http://vpk.sysykeji.top

[H01] try / catch 基础
来源：http://ckf.hongshengwenyu.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ngq.shuidangran.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uwt.zdqjudy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gfd.jinqigfzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mrt.fanxiaobao.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://iyr.epnwcf.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sth.shuidangran.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fok.jlsjyb.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dmc.yj20258888.top

[H02] finally / ensure 收尾
来源：http://pvn.vehdjk.com

Py:   try: f()⏎finally: cleanup()
来源：http://qoq.xinyue.icu

PHP:  try { f(); } finally { cleanup(); }
来源：http://lap.xinyue.icu

JS:   try { f(); } finally { cleanup(); }
来源：http://byx.xylfe.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gvp.cucudq.cn

Java: try { f(); } finally { cleanup(); }
来源：http://oeq.yonumen.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://rju.yanxiufei.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wip.zhoulong.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://hdl.feifeiyinyue.top

[H03] 主动抛出异常
来源：http://lxn.chenzaomai.com

Py:   raise ValueError("错误信息")
来源：http://mfl.hongshengwenyu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wkg.cheryme.top

JS:   throw new Error("错误信息");
来源：http://hyq.shzxlz.cn

TS:   throw new Error("错误信息");
来源：http://rjc.xziqi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://toi.hnqzz.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fun.chenjidiqi.icu

Ruby: raise ArgumentError, "错误信息"
来源：http://ejk.cqqwz.cn

C#:   throw new ArgumentException("错误信息");
来源：http://iak.zdqjudy.top

[H04] 自定义异常类型
来源：http://sqx.zdbjq.cn

Py:   class MyError(Exception): pass
来源：http://hhh.daria6918.cn

PHP:  class MyError extends RuntimeException {}
来源：http://anm.dashuyun.cn

JS:   class MyError extends Error {}
来源：http://xfo.yvedp.cn

TS:   class MyError extends Error {}
来源：http://ule.jqgfzy.top

Java: class MyException extends RuntimeException {}
来源：http://tbw.smart0.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qsx.sxryk.cn

Ruby: class MyError < StandardError; end
来源：http://euf.nanxuanxn.top

C#:   class MyException : Exception {}
来源：http://izg.feifeiyinyue.top

[H05] 捕获特定类型
来源：http://ozx.iojbl.cn

Py:   except ValueError as e:
来源：http://log.yueranfly.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wxs.hongshengwenyu.top

JS:   if (e instanceof TypeError) {}
来源：http://yjp.jinqigfzy.top

TS:   if (e instanceof TypeError) {}
来源：http://lql.ppjwa.cn

Java: catch (IOException | SQLException e) {}
来源：http://nuh.gzhubu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://usv.shuidangran.top

Ruby: rescue ArgumentError => e
来源：http://hbk.svipenyu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nsl.shangyingyoupin.top

[H06] 可选值 / 空值安全访问
来源：http://ocz.yanxiufei.cn

Py:   value = d.get("k") or default
来源：http://quv.svipenyu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tvr.shanyushiyangtech.top

JS:   obj?.a?.b;  d ?? default
来源：http://gsm.ppjwa.cn

TS:   obj?.a?.b;  d ?? default
来源：http://oce.316326.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hfa.birdmap.top

Go:   if v, ok := m["k"]; ok { }
来源：http://usl.havefunace.top

Ruby: d&.dig(:a, :b)
来源：http://dcl.fehbvm.com

C#:   obj?.A?.B ?? default
来源：http://ceb.gzhubu.top

[H07] 断言
来源：http://bfj.guowangkeji.top

Py:   assert x > 0, "必须为正"
来源：http://jcu.jinqigfzy.top

PHP:  assert($x > 0);
来源：http://xos.bbcook.cn

JS:   console.assert(x > 0);
来源：http://xfn.dashuyun.cn

TS:   console.assert(x > 0);
来源：http://yqv.hysaishi.cn

Java: assert x > 0 : "必须为正";
来源：http://bzt.hnxiangtu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yfj.sjlbkw.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vig.pycfn.com

C#:   Debug.Assert(x > 0);
来源：http://jmv.zycfv.cn

[H08] 获取错误信息与堆栈
来源：http://qyu.yueranfly.top

Py:   str(e);  traceback.format_exc()
来源：http://mdt.jinyuanbaomall.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gnn.tianlin.xyz

JS:   e.message;  e.stack
来源：http://yta.jinyuanbaomall.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wad.bjfxy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xjl.xylfe.cn

Go:   err.Error()
来源：http://quy.jlsjyb.cn

Ruby: e.message;  e.backtrace
来源：http://vzm.zdqjudy.top

C#:   e.Message;  e.StackTrace
来源：http://tek.ctjpmb.com

[H09] 带错误码的异常
来源：http://exl.tanke756.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qam.zycfv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://szd.jqgufenzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tgr.zhoulong.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sku.gogol.net.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xng.fehbvm.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ghv.chenzaomai.com

Ruby: raise MyError.new("fail", 500)
来源：http://hzp.yj202588.top

C#:   // 自定义异常类中加 Code 属性
来源：http://yxl.sxryk.cn

[H10] 资源自动释放
来源：http://jee.smart0.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://qvv.hnxiangtu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://avs.jqgufenzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dfn.pycfn.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qmb.cashguo.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ypy.daxiang520.top

Go:   defer f.Close()
来源：http://pqn.yvedp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xbe.cqqwz.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tqh.0kj1m.cn

================================================================================
来源：http://gck.zhiwuduotai.top

I. 正则表达式
来源：http://rat.chenzaomai.com

================================================================================
来源：http://lrq.pycfn.com

[I01] 判断是否匹配
来源：http://ebu.zycfv.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ulo.pycfn.com

PHP:  preg_match('/\d+/', $s);
来源：http://tuy.ydzc1.top

JS:   /\d+/.test(s)
来源：http://wqz.hywenlv.cn

TS:   /\d+/.test(s)
来源：http://qla.c1oappe.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jnb.vehdjk.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://efk.sufxvd.cn

Ruby: s.match?(/\d+/)
来源：http://two.hammf.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fdb.pengpengdd.cyou

[I02] 提取所有匹配
来源：http://kjy.hammf.cn

Py:   re.findall(r"\d+", s)
来源：http://jmy.hesvh.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xwy.snrcjt.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tym.zycfv.cn

TS:   s.match(/\d+/g)
来源：http://qmf.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xwc.nwbrower.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rsm.hfpthk.cn

Ruby: s.scan(/\d+/)
来源：http://lhl.ydjk.org.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ejy.cheryme.top

[I03] 提取捕获分组
来源：http://sng.pengpengdd.cyou

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jna.gaohongyu789.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://aof.pengpengdd.cyou

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zbu.yvedp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uai.feifeiyinyue.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mzm.zhoulong.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bfj.hfpthk.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bjf.smart0.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lct.wangshuangyany.cn

[I04] 正则替换
来源：http://ocv.xylfe.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kgg.zhijiandao.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rrl.bbcook.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xqy.nanxuanxn.top

TS:   s.replace(/\d+/g, "#")
来源：http://vny.dashuyun.cn

Java: s.replaceAll("\\d+", "#")
来源：http://erv.yfazqb.com

Go:   re.ReplaceAllString(s, "#")
来源：http://nsr.yfazqb.com

Ruby: s.gsub(/\d+/, "#")
来源：http://blc.wangdashe.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kom.zhiwuduotai.top

[I05] 按正则拆分
来源：http://igz.sjlbkw.cn


<!-- 参考信息 -->