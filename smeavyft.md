代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://btu.uphjek.com

Java: Files.size(Path.of("a.txt"))
来源：http://byq.guowangkeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wtj.dianchejie.cn

Ruby: File.size("a.txt")
来源：http://gft.haohaochexian.top

C#:   new FileInfo("a.txt").Length
来源：http://swe.zhijiandao.cn

[F10] 取文件扩展名 / 文件名
来源：http://uoj.0kj1m.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kzn.zhengqikj.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ome.daxiang520.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vzg.hcnkem.com

TS:   path.extname("a.txt")
来源：http://iqw.guowangkeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ark.hammf.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bpn.nwbrower.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gqu.yvedp.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mad.tarul.cn

[F11] 复制与移动文件
来源：http://owe.zycfv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sgv.zhixingplan.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vup.yueranfly.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pvu.nanxinkj.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uax.tarul.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nah.haohaochexian.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wev.zhoulong.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cvb.yangfankeji.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://juh.jqgfzy.top

[F12] CSV 读写
来源：http://iem.cheryme.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://eyi.nanxinkj.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sse.fanxiaobao.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rxq.guannengcc.top

TS:   // 同上
来源：http://wgx.jinyuanbaomall.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vrp.hnxiangtu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ckv.bjfxy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tva.bbcook.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://viy.jqgfzy.top

================================================================================
来源：http://uux.jinghuilouyu.cn

G. 面向对象
来源：http://zir.hfpthk.cn

================================================================================
来源：http://ckm.ivvv.top

[G01] 定义类
来源：http://wrt.zhijiandao.cn

Py:   class User: pass
来源：http://jtw.jyoumei.cn

PHP:  class User {}
来源：http://vnm.sufxvd.cn

JS:   class User {}
来源：http://lwb.c1oappe.top

TS:   class User { name: string = ""; }
来源：http://uey.birdmap.top

Java: class User {}
来源：http://ads.nanxuanxn.top

Go:   type User struct { Name string }
来源：http://zhc.uphjek.com

Ruby: class User; end
来源：http://rmc.cdnleiting.top

C#:   class User {}
来源：http://cuj.xuanzx.com

[G02] 构造函数
来源：http://uic.cucudq.cn

Py:   def __init__(self, name): self.name = name
来源：http://xld.jinqigfzy.top

PHP:  public function __construct(public string $name) {}
来源：http://mnj.guannengcc.top

JS:   constructor(name) { this.name = name; }
来源：http://tel.hongshengwenyu.top

TS:   constructor(public name: string) {}
来源：http://tpn.sxryk.cn

Java: User(String name) { this.name = name; }
来源：http://wyi.hnqzz.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wxt.fehbvm.com

Ruby: def initialize(name); @name = name; end
来源：http://uer.zdqjudy.top

C#:   public User(string name) { Name = name; }
来源：http://qdi.cqqwz.cn

[G03] 实例属性
来源：http://czt.yanxiufei.cn

Py:   self.name = "x"
来源：http://qii.yuxming.cn

PHP:  public string $name = "x";
来源：http://tdf.hywenlv.cn

JS:   this.name = "x";
来源：http://mnb.birdmap.top

TS:   name: string = "x";
来源：http://xjj.sweek.top

Java: private String name;
来源：http://flj.zhaomingkeji.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kcz.zhixingplan.top

Ruby: @name = "x"
来源：http://soo.dianchejie.cn

C#:   public string Name { get; set; } = "x";
来源：http://vgz.andypj.xyz

[G04] 定义方法
来源：http://kkh.redwolf501.top

Py:   def greet(self): return self.name
来源：http://hpf.jiagoushi.top

PHP:  public function greet(): string { return $this->name; }
来源：http://mvu.yfazqb.com

JS:   greet() { return this.name; }
来源：http://mwp.svipenyu.cn

TS:   greet(): string { return this.name; }
来源：http://yov.jlsjyb.cn

Java: String greet() { return name; }
来源：http://xpn.yangfankeji.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://cmp.ydzc1.top

Ruby: def greet; @name; end
来源：http://mri.0kj1m.cn

C#:   public string Greet() => Name;
来源：http://djn.gzhubu.top

[G05] 继承
来源：http://voa.guannengcc.top

Py:   class Admin(User): pass
来源：http://gwk.vehdjk.com

PHP:  class Admin extends User {}
来源：http://mwm.cdnleiting.top

JS:   class Admin extends User {}
来源：http://quc.shzxlz.cn

TS:   class Admin extends User {}
来源：http://ctu.cheryme.top

Java: class Admin extends User {}
来源：http://mcp.bjfxy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mvl.ctjpmb.com

Ruby: class Admin < User; end
来源：http://azy.ybcxt.top

C#:   class Admin : User {}
来源：http://rox.fanxiaobao.xyz

[G06] 重写方法
来源：http://acs.chenjidiqi.icu

Py:   def greet(self): return "admin"
来源：http://gvu.ybcxt.top

PHP:  public function greet(): string { return "admin"; }
来源：http://xko.hysaishi.cn

JS:   greet() { return "admin"; }
来源：http://mcv.jqgufenzy.top

TS:   greet(): string { return "admin"; }
来源：http://frf.hnxiangtu.top

Java: @Override String greet() { return "admin"; }
来源：http://dcv.shanyushiyangkeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lcn.yongpay.top

Ruby: def greet; "admin"; end
来源：http://tbm.kuanghao11.cn

C#:   public override string Greet() => "admin";
来源：http://pdg.xylfe.cn

[G07] 调用父类方法
来源：http://cel.hywenlv.cn

Py:   super().greet()
来源：http://urw.hongshengwenyu.top

PHP:  parent::greet();
来源：http://tby.shangyingyoupin.top

JS:   super.greet();
来源：http://ujq.pycfn.com

TS:   super.greet();
来源：http://dhv.feifeiyinyue.top

Java: super.greet();
来源：http://zbg.sysykeji.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hvr.jlsjyb.cn

Ruby: super
来源：http://peo.pengpengdd.cyou

C#:   base.Greet();
来源：http://zvv.iojbl.cn

[G08] 静态方法与属性
来源：http://yys.316326.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rqn.tian-w.cn

PHP:  public static function f() {}
来源：http://kbj.ybcxt.top

JS:   static f() {}
来源：http://kqj.sysykeji.top

TS:   static f(): void {}
来源：http://hvz.nanxuanxn.top

Java: static void f() {}
来源：http://lyp.jqgufenzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://tqh.zhaomingkeji.xyz

Ruby: def self.f; end
来源：http://ijj.9152youxi.cn

C#:   public static void F() {}
来源：http://iyw.dashuyun.cn

[G09] 接口 / 抽象类
来源：http://nmg.nanxuanxn.top

Py:   from abc import ABC, abstractmethod
来源：http://nzb.tianlin.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://avx.jinqigufen.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://leq.jqgfzy.top

TS:   interface Shape { area(): number; }
来源：http://ebu.daxiang520.top

Java: interface Shape { double area(); }
来源：http://sxf.quarkkingdee.top

Go:   type Shape interface { Area() float64 }
来源：http://lga.cucudq.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nyh.ivvv.top

C#:   interface IShape { double Area(); }
来源：http://ycd.fzhhl.top

[G10] 访问控制
来源：http://rth.shzxlz.cn

Py:   约定 _protected / __private（不强制）
来源：http://jub.zhongyouzk.top

PHP:  public / protected / private
来源：http://mjn.zhixingplan.top

JS:   #private 字段；其余公开
来源：http://myx.yuanzhike.top

TS:   public / protected / private
来源：http://epa.tarul.cn

Java: public / protected / private / 默认包级
来源：http://irc.epnwcf.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://iuu.jlsjyb.cn

Ruby: public / protected / private
来源：http://mbk.tianlin.xyz

C#:   public / protected / private / internal
来源：http://syr.dianchejie.cn

[G11] getter / setter
来源：http://rgd.svipenyu.cn

Py:   @property 与 @x.setter
来源：http://ovv.hnqzz.top

PHP:  public function getName(): string { return $this->name; }
来源：http://oax.zhoulong.xyz

JS:   get name() { return this._name; }
来源：http://ims.aibaodan.cn

TS:   get name(): string { return this._name; }
来源：http://qbo.hammf.cn

Java: public String getName() { return name; }
来源：http://jhn.mhx1999.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://evc.chenlongwang.top

Ruby: attr_accessor :name
来源：http://ejy.shanyushiyangtech.top

C#:   public string Name { get; set; }
来源：http://gyr.sysykeji.top

[G12] 对象转字符串
来源：http://gtv.jianghu66.top

Py:   def __str__(self): return self.name
来源：http://upq.pengpengdd.cyou

PHP:  public function __toString(): string { return $this->name; }
来源：http://wqk.gaohongyu789.top

JS:   toString() { return this.name; }
来源：http://kld.svipenyu.cn

TS:   toString(): string { return this.name; }
来源：http://hkg.9152youxi.cn

Java: @Override public String toString() { return name; }
来源：http://wcm.ivvv.top

Go:   func (u User) String() string { return u.Name }
来源：http://ndf.zdbjq.cn

Ruby: def to_s; @name; end
来源：http://rui.yfazqb.com

C#:   public override string ToString() => Name;
来源：http://jth.zhoulong.xyz

[G13] 判断对象类型
来源：http://etj.gzhubu.top

Py:   isinstance(u, User)
来源：http://cwz.ybcxt.top

PHP:  $u instanceof User
来源：http://gef.yj202588.top

JS:   u instanceof User
来源：http://rzg.jiagoushi.top

TS:   u instanceof User
来源：http://qnj.shanyushiyangtech.top

Java: u instanceof User
来源：http://ykg.zhixingplan.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://hfb.sxryk.cn

Ruby: u.is_a?(User)
来源：http://xkx.cqqwz.cn

C#:   u is User
来源：http://feo.bbcook.cn

[G14] 数据类 / record
来源：http://kvr.nanxuanxn.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qtr.hysaishi.cn

PHP:  // 用 readonly 属性模拟
来源：http://ues.zhoulong.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://wbc.dashuyun.cn

TS:   type User = { name: string; age: number };
来源：http://wvq.yj20258.top

Java: record User(String name, int age) {}
来源：http://vdt.daria6918.cn

Go:   type User struct { Name string; Age int }
来源：http://ntd.quarkkingdee.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yun.yfazqb.com

C#:   record User(string Name, int Age);
来源：http://ckf.zdbjq.cn

[G15] 枚举
来源：http://hvr.316326.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cbq.jqgufenzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ijf.pengpengdd.cyou

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bbz.pycfn.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gis.yueranfly.top

Java: enum Color { RED, GREEN }
来源：http://bch.daria6918.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://iju.haohaochexian.top

Ruby: Color = %i[red green].freeze
来源：http://yhs.xingfuxueyuan.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dom.chenlongwang.top

[G16] 对象转数组 / 字典
来源：http://aca.0kj1m.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wkp.jinyuanbaomall.cn

PHP:  get_object_vars($obj);
来源：http://pnz.yongpay.top

JS:   Object.entries(obj)
来源：http://dlx.zycfv.cn

TS:   Object.entries(obj)
来源：http://vbj.jinqigufen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cfj.feifeiyinyue.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://gxc.xinyue.icu

Ruby: obj.instance_variables
来源：http://xcy.tianlin.xyz

C#:   // 用反射或 System.Text.Json
来源：http://hze.9152youxi.cn

================================================================================
来源：http://amy.svipenyu.cn

H. 异常与错误处理
来源：http://jyr.shanyushiyangtech.top

================================================================================
来源：http://uao.xingfuxueyuan.xyz

[H01] try / catch 基础
来源：http://vcm.zhongyouzk.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jmc.pengpengdd.cyou

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://iti.feifeiyinyue.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uvw.dashuyun.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bsy.fktsv.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wyp.gogol.net.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ehi.jianghu66.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cqu.shuidangran.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ojz.yuxming.cn

[H02] finally / ensure 收尾
来源：http://aal.cqqwz.cn

Py:   try: f()⏎finally: cleanup()
来源：http://aql.ehwqpu.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://djt.kuanghao11.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tyl.daria6918.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://kir.cqqwz.cn

Java: try { f(); } finally { cleanup(); }
来源：http://opq.jqgufenzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://tqn.dianchejie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://oks.redwolf501.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://hsz.shzxlz.cn

[H03] 主动抛出异常
来源：http://xvk.havefunace.top

Py:   raise ValueError("错误信息")
来源：http://hab.ywan-chungtsiang.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://okv.bjfxy.top

JS:   throw new Error("错误信息");
来源：http://qdx.ehwqpu.com

TS:   throw new Error("错误信息");
来源：http://hyx.vqdsnc.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fjj.nwbrower.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://unj.shzxlz.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ytw.jinqigfzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://zsm.zhixingplan.top

[H04] 自定义异常类型
来源：http://itz.jlsjyb.cn

Py:   class MyError(Exception): pass
来源：http://eht.shanyushiyangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://thn.kuanghao11.cn

JS:   class MyError extends Error {}
来源：http://rxa.tian-w.cn

TS:   class MyError extends Error {}
来源：http://vua.snrcjt.cn

Java: class MyException extends RuntimeException {}
来源：http://bsm.shanyushiyangtech.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lyk.hnxiangtu.top

Ruby: class MyError < StandardError; end
来源：http://rls.gaohongyu789.top

C#:   class MyException : Exception {}
来源：http://alf.ehwqpu.com

[H05] 捕获特定类型
来源：http://qch.c1oappe.top

Py:   except ValueError as e:
来源：http://hkq.tanke756.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jlj.jyoumei.cn

JS:   if (e instanceof TypeError) {}
来源：http://nbz.ydzc1.top

TS:   if (e instanceof TypeError) {}
来源：http://jgf.guowangkeji.top

Java: catch (IOException | SQLException e) {}
来源：http://ljp.hammf.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qbm.xziqi.cn

Ruby: rescue ArgumentError => e
来源：http://how.zycfv.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jse.zhoulong.xyz

[H06] 可选值 / 空值安全访问
来源：http://xro.wangdashe.top

Py:   value = d.get("k") or default
来源：http://gqn.ctjpmb.com

PHP:  $v = $d["k"] ?? null;
来源：http://taz.mhx1999.top

JS:   obj?.a?.b;  d ?? default
来源：http://ggo.hnxiangtu.top

TS:   obj?.a?.b;  d ?? default
来源：http://zte.jinyuanbaomall.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ygc.gaohongyu789.top

Go:   if v, ok := m["k"]; ok { }
来源：http://bqj.xziqi.cn

Ruby: d&.dig(:a, :b)
来源：http://mkx.jinqigufen.top

C#:   obj?.A?.B ?? default
来源：http://uqd.shuidangran.top

[H07] 断言
来源：http://rfc.hongshengwenyu.top

Py:   assert x > 0, "必须为正"
来源：http://tno.zhengqikj.top

PHP:  assert($x > 0);
来源：http://ghb.xylfe.cn

JS:   console.assert(x > 0);
来源：http://fkl.jinqigfzy.top

TS:   console.assert(x > 0);
来源：http://tty.fengsongda.top

Java: assert x > 0 : "必须为正";
来源：http://ngs.haohaochexian.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gue.cashguo.top

Ruby: raise "必须为正" unless x > 0
来源：http://yyo.hongshengwenyu.top

C#:   Debug.Assert(x > 0);
来源：http://prl.fzhhl.top

[H08] 获取错误信息与堆栈
来源：http://ufn.pycfn.com

Py:   str(e);  traceback.format_exc()
来源：http://xny.zhongyouzk.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nru.shuidangran.top

JS:   e.message;  e.stack
来源：http://nsw.bjfxy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://cnj.dianchejie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://sym.ywan-chungtsiang.top

Go:   err.Error()
来源：http://czj.gogol.net.cn

Ruby: e.message;  e.backtrace
来源：http://zgh.shanyushiyangtech.top

C#:   e.Message;  e.StackTrace
来源：http://bjg.haohaochexian.top

[H09] 带错误码的异常
来源：http://zro.jiagoushi.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sus.xziqi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vwr.yuxming.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lpi.jqgfzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://epc.yvedp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xyj.ctjpmb.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yyz.sysykeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://lao.fanxiaobao.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://auh.dashuyun.cn

[H10] 资源自动释放
来源：http://ddo.vqdsnc.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rsf.nwbrower.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://smm.yj20258888.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qbs.tianlin.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yif.cheryme.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ppq.fehbvm.com

Go:   defer f.Close()
来源：http://qbz.yueranfly.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://abo.aibaodan.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vpt.ywan-chungtsiang.top

================================================================================
来源：http://aiv.nanxuanxn.top

I. 正则表达式
来源：http://buv.shuidangran.top

================================================================================
来源：http://mgr.fktsv.cn

[I01] 判断是否匹配
来源：http://jsc.nanxinkj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fww.jinqigfzy.top

PHP:  preg_match('/\d+/', $s);
来源：http://tag.hnqzz.top

JS:   /\d+/.test(s)
来源：http://ice.cqqwz.cn

TS:   /\d+/.test(s)
来源：http://huy.jinqigfzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cqp.yj20258888.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uan.nanxinkj.top

Ruby: s.match?(/\d+/)
来源：http://noj.daria6918.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ecg.gotoacloud.top

[I02] 提取所有匹配
来源：http://pzn.daria6918.cn

Py:   re.findall(r"\d+", s)
来源：http://wdk.jinqigufen.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://phq.jlsjyb.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jha.fengsongda.top

TS:   s.match(/\d+/g)
来源：http://gbb.chenjidiqi.icu

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fav.cashguo.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dxv.yvedp.cn

Ruby: s.scan(/\d+/)
来源：http://vmh.shanyushiyangtech.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://egt.xylfe.cn

[I03] 提取捕获分组
来源：http://ngp.zhijiandao.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yty.hywenlv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kfz.cucudq.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yss.hongshengwenyu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rmg.cashguo.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xsg.ydjk.org.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mrl.yangfankeji.com


<!-- 参考信息 -->