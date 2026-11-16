代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bso.hcnkem.com

TS:   path.extname("a.txt")
来源：http://ghv.ivvv.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://thl.zdqjudy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xyg.xingfuxueyuan.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://phs.xingfuxueyuan.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ysx.birdmap.top

[F11] 复制与移动文件
来源：http://oyn.zycfv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dxl.yj202588.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://atk.zhengqikj.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pqh.vehdjk.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://crx.zycfv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dnb.zhijiandao.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zlr.gzhubu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rsk.chenjidiqi.icu

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rzj.jqgfzy.top

[F12] CSV 读写
来源：http://dpq.ywan-chungtsiang.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://llw.sufxvd.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lsw.xinyue.icu

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qpq.yj20258.top

TS:   // 同上
来源：http://vyu.chenlongwang.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dnp.feifeiyinyue.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cfg.wangdashe.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vwv.snrcjt.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lpd.zhijiandao.cn

================================================================================
来源：http://vad.jlsjyb.cn

G. 面向对象
来源：http://rdb.sjlbkw.cn

================================================================================
来源：http://yyn.jinqigufen.top

[G01] 定义类
来源：http://noh.bjfxy.top

Py:   class User: pass
来源：http://aum.zhixingplan.top

PHP:  class User {}
来源：http://xde.daxiang520.top

JS:   class User {}
来源：http://txi.fzhhl.top

TS:   class User { name: string = ""; }
来源：http://ndt.haohaochexian.top

Java: class User {}
来源：http://qxl.jqgufenzy.top

Go:   type User struct { Name string }
来源：http://adp.cashguo.top

Ruby: class User; end
来源：http://ndi.zhixingplan.top

C#:   class User {}
来源：http://zbc.pengpengdd.cyou

[G02] 构造函数
来源：http://ylc.aibaodan.cn

Py:   def __init__(self, name): self.name = name
来源：http://tjr.aibaodan.cn

PHP:  public function __construct(public string $name) {}
来源：http://vjq.gotoacloud.top

JS:   constructor(name) { this.name = name; }
来源：http://bpd.ppjwa.cn

TS:   constructor(public name: string) {}
来源：http://aay.jiagoushi.top

Java: User(String name) { this.name = name; }
来源：http://abv.yonumen.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gvd.nanxinkj.top

Ruby: def initialize(name); @name = name; end
来源：http://wal.hongshengwenyu.top

C#:   public User(string name) { Name = name; }
来源：http://vbg.sweek.top

[G03] 实例属性
来源：http://ubz.gzhubu.top

Py:   self.name = "x"
来源：http://cbd.andypj.xyz

PHP:  public string $name = "x";
来源：http://anq.hammf.cn

JS:   this.name = "x";
来源：http://jsg.xingfuxueyuan.xyz

TS:   name: string = "x";
来源：http://bll.kuanghao11.cn

Java: private String name;
来源：http://eyt.chenlongwang.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://imc.pycfn.com

Ruby: @name = "x"
来源：http://uts.dashuyun.cn

C#:   public string Name { get; set; } = "x";
来源：http://umn.snrcjt.cn

[G04] 定义方法
来源：http://aoj.xziqi.cn

Py:   def greet(self): return self.name
来源：http://ppe.hysaishi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://knn.cucudq.cn

JS:   greet() { return this.name; }
来源：http://ljp.9152youxi.cn

TS:   greet(): string { return this.name; }
来源：http://von.yuxming.cn

Java: String greet() { return name; }
来源：http://jrm.dianchejie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://clz.yuanzhike.top

Ruby: def greet; @name; end
来源：http://epd.jinqigufen.top

C#:   public string Greet() => Name;
来源：http://lzp.zhiwuduotai.top

[G05] 继承
来源：http://pxl.smart0.xyz

Py:   class Admin(User): pass
来源：http://pcf.ctjpmb.com

PHP:  class Admin extends User {}
来源：http://fyg.zdqjudy.top

JS:   class Admin extends User {}
来源：http://dja.fktsv.cn

TS:   class Admin extends User {}
来源：http://srd.yanxiufei.cn

Java: class Admin extends User {}
来源：http://yco.yj20258.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ruw.gzhubu.top

Ruby: class Admin < User; end
来源：http://dez.nanxuanxn.top

C#:   class Admin : User {}
来源：http://noc.hammf.cn

[G06] 重写方法
来源：http://nda.dashuyun.cn

Py:   def greet(self): return "admin"
来源：http://gvf.vehdjk.com

PHP:  public function greet(): string { return "admin"; }
来源：http://pxg.xingfuxueyuan.xyz

JS:   greet() { return "admin"; }
来源：http://szw.snrcjt.cn

TS:   greet(): string { return "admin"; }
来源：http://zmo.nwbrower.top

Java: @Override String greet() { return "admin"; }
来源：http://hri.sufxvd.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://slg.yongpay.top

Ruby: def greet; "admin"; end
来源：http://okx.fzhhl.top

C#:   public override string Greet() => "admin";
来源：http://knm.yueranfly.top

[G07] 调用父类方法
来源：http://mgb.gogol.net.cn

Py:   super().greet()
来源：http://rlx.yj202588.top

PHP:  parent::greet();
来源：http://lem.yanxiufei.cn

JS:   super.greet();
来源：http://bfy.cdnleiting.top

TS:   super.greet();
来源：http://iki.jqgufenzy.top

Java: super.greet();
来源：http://gqp.bbcook.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xps.yangfankeji.com

Ruby: super
来源：http://wxl.ydjk.org.cn

C#:   base.Greet();
来源：http://uag.yvedp.cn

[G08] 静态方法与属性
来源：http://isd.chenlongwang.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dwx.nanxinkj.top

PHP:  public static function f() {}
来源：http://def.yonumen.top

JS:   static f() {}
来源：http://dva.havefunace.top

TS:   static f(): void {}
来源：http://ypf.ctjpmb.com

Java: static void f() {}
来源：http://tnh.sysykeji.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://qjb.bjfxy.top

Ruby: def self.f; end
来源：http://xcv.jianghu66.top

C#:   public static void F() {}
来源：http://msb.cqqwz.cn

[G09] 接口 / 抽象类
来源：http://rth.hongshengwenyu.top

Py:   from abc import ABC, abstractmethod
来源：http://tyd.yj20258.top

PHP:  interface Shape { public function area(): float; }
来源：http://vhr.nwbrower.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://cbl.cdnleiting.top

TS:   interface Shape { area(): number; }
来源：http://plh.tanke756.top

Java: interface Shape { double area(); }
来源：http://kgs.yj20258888.top

Go:   type Shape interface { Area() float64 }
来源：http://srv.jinqigfzy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dmy.hnxiangtu.top

C#:   interface IShape { double Area(); }
来源：http://eqf.fengsongda.top

[G10] 访问控制
来源：http://wnm.pengpengdd.cyou

Py:   约定 _protected / __private（不强制）
来源：http://xpq.sysykeji.top

PHP:  public / protected / private
来源：http://gdf.jqgufenzy.top

JS:   #private 字段；其余公开
来源：http://cgb.xuanzx.com

TS:   public / protected / private
来源：http://mcg.ybcxt.top

Java: public / protected / private / 默认包级
来源：http://xnq.hnxiangtu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://sij.jinqigufen.top

Ruby: public / protected / private
来源：http://spa.gzhubu.top

C#:   public / protected / private / internal
来源：http://rxi.gogol.net.cn

[G11] getter / setter
来源：http://uhb.xziqi.cn

Py:   @property 与 @x.setter
来源：http://gxx.yonumen.top

PHP:  public function getName(): string { return $this->name; }
来源：http://wjm.quarkkingdee.top

JS:   get name() { return this._name; }
来源：http://top.shanyushiyangkeji.top

TS:   get name(): string { return this._name; }
来源：http://ivj.uphjek.com

Java: public String getName() { return name; }
来源：http://rwe.mhx1999.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://cnr.hammf.cn

Ruby: attr_accessor :name
来源：http://qzs.xuetiantiany.cn

C#:   public string Name { get; set; }
来源：http://nek.tianlin.xyz

[G12] 对象转字符串
来源：http://ulh.yj202588.top

Py:   def __str__(self): return self.name
来源：http://umw.tian-w.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://yka.nwbrower.top

JS:   toString() { return this.name; }
来源：http://exg.hammf.cn

TS:   toString(): string { return this.name; }
来源：http://jtp.zhijiandao.cn

Java: @Override public String toString() { return name; }
来源：http://mos.tian-w.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vsb.yj202588.top

Ruby: def to_s; @name; end
来源：http://gxi.cheryme.top

C#:   public override string ToString() => Name;
来源：http://pze.vehdjk.com

[G13] 判断对象类型
来源：http://yos.tianlin.xyz

Py:   isinstance(u, User)
来源：http://sgo.pycfn.com

PHP:  $u instanceof User
来源：http://asg.uphjek.com

JS:   u instanceof User
来源：http://dzd.yuxming.cn

TS:   u instanceof User
来源：http://anq.zhijiandao.cn

Java: u instanceof User
来源：http://hoe.cheryme.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://tgt.chenjidiqi.icu

Ruby: u.is_a?(User)
来源：http://txy.shangyingyoupin.top

C#:   u is User
来源：http://qzs.sjlbkw.cn

[G14] 数据类 / record
来源：http://vaa.nwbrower.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://akf.hfpthk.cn

PHP:  // 用 readonly 属性模拟
来源：http://smh.jinqigufen.top

JS:   // 无内置：普通类或对象字面量
来源：http://rwr.cashguo.top

TS:   type User = { name: string; age: number };
来源：http://bvu.xylfe.cn

Java: record User(String name, int age) {}
来源：http://ztt.c1oappe.top

Go:   type User struct { Name string; Age int }
来源：http://qts.zhaomingkeji.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://swx.zhaomingkeji.xyz

C#:   record User(string Name, int Age);
来源：http://piw.cashguo.top

[G15] 枚举
来源：http://yoh.ctjpmb.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zii.xuetiantiany.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://iob.epnwcf.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hdn.vqdsnc.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jfy.yj202588.top

Java: enum Color { RED, GREEN }
来源：http://rok.zhiwuduotai.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://quh.hnxiangtu.top

Ruby: Color = %i[red green].freeze
来源：http://qfb.dashuyun.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lpk.quarkkingdee.top

[G16] 对象转数组 / 字典
来源：http://pdm.hysaishi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://epo.gzhubu.top

PHP:  get_object_vars($obj);
来源：http://nuz.hammf.cn

JS:   Object.entries(obj)
来源：http://krb.jlsjyb.cn

TS:   Object.entries(obj)
来源：http://bwv.fehbvm.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yhx.guannengcc.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://xxq.zhengqikj.top

Ruby: obj.instance_variables
来源：http://emw.zhaomingkeji.xyz

C#:   // 用反射或 System.Text.Json
来源：http://deg.yangfankeji.com

================================================================================
来源：http://stb.cucudq.cn

H. 异常与错误处理
来源：http://stu.hcnkem.com

================================================================================
来源：http://ysx.gaohongyu789.top

[H01] try / catch 基础
来源：http://mzf.hesvh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rtw.jiagoushi.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mxu.wangdashe.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dyh.xinyue.icu

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lpt.jiagoushi.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rxq.hesvh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xyt.zhixingplan.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jne.sufxvd.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nzi.sxryk.cn

[H02] finally / ensure 收尾
来源：http://yin.cashguo.top

Py:   try: f()⏎finally: cleanup()
来源：http://qsn.hfpthk.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://eux.wangshuangyany.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://sya.bbcook.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vdr.ehwqpu.com

Java: try { f(); } finally { cleanup(); }
来源：http://mhu.xingfuxueyuan.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://bru.ybcxt.top

Ruby: begin; f; ensure; cleanup; end
来源：http://mjv.jlsjyb.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ook.pycfn.com

[H03] 主动抛出异常
来源：http://qsz.yuanzhike.top

Py:   raise ValueError("错误信息")
来源：http://suf.xinyue.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fih.gaohongyu789.top

JS:   throw new Error("错误信息");
来源：http://pgh.hfpthk.cn

TS:   throw new Error("错误信息");
来源：http://qvp.jiagoushi.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://jqv.jlsjyb.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nkj.yangfankeji.com

Ruby: raise ArgumentError, "错误信息"
来源：http://irf.zhiwuduotai.top

C#:   throw new ArgumentException("错误信息");
来源：http://tpa.ehwqpu.com

[H04] 自定义异常类型
来源：http://fyy.yj202588.top

Py:   class MyError(Exception): pass
来源：http://wws.sjlbkw.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tfl.shanyushiyangkeji.top

JS:   class MyError extends Error {}
来源：http://ebo.52xcode.cn

TS:   class MyError extends Error {}
来源：http://fbn.mhx1999.top

Java: class MyException extends RuntimeException {}
来源：http://zim.havefunace.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gqo.hnxiangtu.top

Ruby: class MyError < StandardError; end
来源：http://tgy.xingfuxueyuan.xyz

C#:   class MyException : Exception {}
来源：http://teb.nanxuanxn.top

[H05] 捕获特定类型
来源：http://hub.cashguo.top

Py:   except ValueError as e:
来源：http://xhi.tanke756.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xzr.zhiwuduotai.top

JS:   if (e instanceof TypeError) {}
来源：http://hns.meibo888.top

TS:   if (e instanceof TypeError) {}
来源：http://rrv.ywan-chungtsiang.top

Java: catch (IOException | SQLException e) {}
来源：http://icm.sweek.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vxi.cheryme.top

Ruby: rescue ArgumentError => e
来源：http://qnq.fktsv.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ejy.tarul.cn

[H06] 可选值 / 空值安全访问
来源：http://hxk.sufxvd.cn

Py:   value = d.get("k") or default
来源：http://hqy.gaohongyu789.top

PHP:  $v = $d["k"] ?? null;
来源：http://fuc.ppjwa.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ghi.yfazqb.com

TS:   obj?.a?.b;  d ?? default
来源：http://kef.shangyingyoupin.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vcy.yj202588.top

Go:   if v, ok := m["k"]; ok { }
来源：http://xoo.daria6918.cn

Ruby: d&.dig(:a, :b)
来源：http://slu.epnwcf.com

C#:   obj?.A?.B ?? default
来源：http://mss.tianlin.xyz

[H07] 断言
来源：http://ilb.ehwqpu.com

Py:   assert x > 0, "必须为正"
来源：http://jjq.wangdashe.top

PHP:  assert($x > 0);
来源：http://its.daria6918.cn

JS:   console.assert(x > 0);
来源：http://dqn.andypj.xyz

TS:   console.assert(x > 0);
来源：http://xxl.guowangkeji.top

Java: assert x > 0 : "必须为正";
来源：http://wxz.epnwcf.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ppo.tarul.cn

Ruby: raise "必须为正" unless x > 0
来源：http://nnf.yueranfly.top

C#:   Debug.Assert(x > 0);
来源：http://ull.yonumen.top

[H08] 获取错误信息与堆栈
来源：http://rvz.chenzaomai.com

Py:   str(e);  traceback.format_exc()
来源：http://mmf.yangfankeji.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gly.gotoacloud.top

JS:   e.message;  e.stack
来源：http://tds.yonumen.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://riw.xuanzx.com

Java: e.getMessage();  e.printStackTrace()
来源：http://tle.nwbrower.top

Go:   err.Error()
来源：http://qyb.quarkkingdee.top

Ruby: e.message;  e.backtrace
来源：http://mhu.jinqigfzy.top

C#:   e.Message;  e.StackTrace
来源：http://ver.chenzaomai.com

[H09] 带错误码的异常
来源：http://onm.andypj.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cdm.yj202588.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://wow.uphjek.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zkv.jqgfzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cxf.yongpay.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tjl.hfpthk.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fhk.yueranfly.top

Ruby: raise MyError.new("fail", 500)
来源：http://gxt.hysaishi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xww.yuanzhike.top

[H10] 资源自动释放
来源：http://hxj.iojbl.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://aaj.pengpengdd.cyou

PHP:  // 无 with：在 finally 里 fclose()
来源：http://deo.xylfe.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vrj.jinqigfzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mrf.316326.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qba.jinqigfzy.top

Go:   defer f.Close()
来源：http://opx.zhiwuduotai.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bsz.ybcxt.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cmy.wangdashe.top

================================================================================
来源：http://nie.yangfankeji.com

I. 正则表达式
来源：http://ubg.jianghu66.top

================================================================================
来源：http://yve.cqqwz.cn

[I01] 判断是否匹配
来源：http://cyx.tian-w.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lkm.9152youxi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://kwx.daria6918.cn

JS:   /\d+/.test(s)
来源：http://klv.sufxvd.cn

TS:   /\d+/.test(s)
来源：http://ofw.jiagoushi.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ipt.ehwqpu.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bnq.zhoulong.xyz

Ruby: s.match?(/\d+/)
来源：http://wkk.daria6918.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ymx.pengpengdd.cyou

[I02] 提取所有匹配
来源：http://ksr.mhx1999.top

Py:   re.findall(r"\d+", s)
来源：http://ctv.xinyue.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dgw.cdnleiting.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nej.cheryme.top

TS:   s.match(/\d+/g)
来源：http://zwz.xinyue.icu

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qzc.tian-w.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yds.nanxuanxn.top

Ruby: s.scan(/\d+/)
来源：http://ejc.jqgufenzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wnm.sxryk.cn

[I03] 提取捕获分组
来源：http://ono.zhoulong.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lso.yvedp.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qlt.hesvh.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wjy.iojbl.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://npy.jqgfzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mko.52xcode.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kdw.zhoulong.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://alh.yuanzhike.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://eaj.fanxiaobao.xyz

[I04] 正则替换
来源：http://mxi.jinghuilouyu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gxl.jinghuilouyu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nwz.xingfuxueyuan.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://qwf.fktsv.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ume.zhengqikj.top

Java: s.replaceAll("\\d+", "#")
来源：http://unq.tanke756.top


<!-- 参考信息 -->