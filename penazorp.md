代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://sfs.ybcxt.top

Java: Files.size(Path.of("a.txt"))
来源：http://hxm.hysaishi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uql.xuanzx.com

Ruby: File.size("a.txt")
来源：http://wgj.xingfuxueyuan.xyz

C#:   new FileInfo("a.txt").Length
来源：http://odj.sxryk.cn

[F10] 取文件扩展名 / 文件名
来源：http://ohc.shanyushiyangtech.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jny.yj20258888.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://upz.jinghuilouyu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vjp.smart0.xyz

TS:   path.extname("a.txt")
来源：http://tgz.hcnkem.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kpz.hysaishi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fvv.hnxiangtu.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://iwj.jinghuilouyu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fwd.9152youxi.cn

[F11] 复制与移动文件
来源：http://bad.zdqjudy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rwy.feifeiyinyue.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cxo.jqgfzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kmq.wangshuangyany.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zmg.hywenlv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rbt.yfazqb.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rbd.chenjidiqi.icu

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nus.hongshengwenyu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tbd.jianghu66.top

[F12] CSV 读写
来源：http://xrx.tianlin.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ijw.yonumen.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ofu.ydjk.org.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://knb.redwolf501.top

TS:   // 同上
来源：http://auk.fzhhl.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bfk.daxiang520.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rfy.guowangkeji.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wge.316326.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://doo.hywenlv.cn

================================================================================
来源：http://wpn.sweek.top

G. 面向对象
来源：http://chs.chenlongwang.top

================================================================================
来源：http://iym.chenjidiqi.icu

[G01] 定义类
来源：http://aru.ehwqpu.com

Py:   class User: pass
来源：http://rqx.zhongyouzk.top

PHP:  class User {}
来源：http://rpc.vehdjk.com

JS:   class User {}
来源：http://wxa.gaohongyu789.top

TS:   class User { name: string = ""; }
来源：http://xne.bjfxy.top

Java: class User {}
来源：http://qyf.ydzc1.top

Go:   type User struct { Name string }
来源：http://adp.jinyuanbaomall.cn

Ruby: class User; end
来源：http://kqs.zhaomingkeji.xyz

C#:   class User {}
来源：http://qcs.hcnkem.com

[G02] 构造函数
来源：http://bxi.wangdashe.top

Py:   def __init__(self, name): self.name = name
来源：http://cwy.mhx1999.top

PHP:  public function __construct(public string $name) {}
来源：http://elo.cucudq.cn

JS:   constructor(name) { this.name = name; }
来源：http://zve.dashuyun.cn

TS:   constructor(public name: string) {}
来源：http://wwr.yj20258888.top

Java: User(String name) { this.name = name; }
来源：http://qkk.yonumen.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wzj.tian-w.cn

Ruby: def initialize(name); @name = name; end
来源：http://hqs.havefunace.top

C#:   public User(string name) { Name = name; }
来源：http://ars.meibo888.top

[G03] 实例属性
来源：http://rxg.aizwys.cn

Py:   self.name = "x"
来源：http://uej.yangfankeji.com

PHP:  public string $name = "x";
来源：http://lps.epnwcf.com

JS:   this.name = "x";
来源：http://tde.hongshengwenyu.top

TS:   name: string = "x";
来源：http://rie.sjlbkw.cn

Java: private String name;
来源：http://spy.xuetiantiany.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zfp.jianghu66.top

Ruby: @name = "x"
来源：http://mul.feifeiyinyue.top

C#:   public string Name { get; set; } = "x";
来源：http://voc.haohaochexian.top

[G04] 定义方法
来源：http://vax.ehwqpu.com

Py:   def greet(self): return self.name
来源：http://tlg.yvedp.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ijr.ywan-chungtsiang.top

JS:   greet() { return this.name; }
来源：http://buf.shanyushiyangkeji.top

TS:   greet(): string { return this.name; }
来源：http://rfo.jinqigufen.top

Java: String greet() { return name; }
来源：http://bal.aibaodan.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://usw.sweek.top

Ruby: def greet; @name; end
来源：http://tyr.jinqigfzy.top

C#:   public string Greet() => Name;
来源：http://syr.nanxuanxn.top

[G05] 继承
来源：http://anw.chenjidiqi.icu

Py:   class Admin(User): pass
来源：http://wra.ppjwa.cn

PHP:  class Admin extends User {}
来源：http://hsh.hongshengwenyu.top

JS:   class Admin extends User {}
来源：http://qcf.xuanzx.com

TS:   class Admin extends User {}
来源：http://jzn.cheryme.top

Java: class Admin extends User {}
来源：http://lad.haohaochexian.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qtc.cucudq.cn

Ruby: class Admin < User; end
来源：http://gqg.xinyue.icu

C#:   class Admin : User {}
来源：http://zxo.52xcode.cn

[G06] 重写方法
来源：http://ouj.jyoumei.cn

Py:   def greet(self): return "admin"
来源：http://frg.ywan-chungtsiang.top

PHP:  public function greet(): string { return "admin"; }
来源：http://teb.gaohongyu789.top

JS:   greet() { return "admin"; }
来源：http://scm.cqqwz.cn

TS:   greet(): string { return "admin"; }
来源：http://rzm.yanxiufei.cn

Java: @Override String greet() { return "admin"; }
来源：http://ove.hnxiangtu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nee.tarul.cn

Ruby: def greet; "admin"; end
来源：http://liy.aibaodan.cn

C#:   public override string Greet() => "admin";
来源：http://phx.chenjidiqi.icu

[G07] 调用父类方法
来源：http://fvh.jinyuanbaomall.cn

Py:   super().greet()
来源：http://hln.fanxiaobao.xyz

PHP:  parent::greet();
来源：http://unn.jyoumei.cn

JS:   super.greet();
来源：http://cke.jyoumei.cn

TS:   super.greet();
来源：http://wld.vehdjk.com

Java: super.greet();
来源：http://qyo.aibaodan.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://eqi.wangshuangyany.cn

Ruby: super
来源：http://kkq.dianchejie.cn

C#:   base.Greet();
来源：http://soa.yj202588.top

[G08] 静态方法与属性
来源：http://fff.hysaishi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://eas.daria6918.cn

PHP:  public static function f() {}
来源：http://axn.shzxlz.cn

JS:   static f() {}
来源：http://plt.cdnleiting.top

TS:   static f(): void {}
来源：http://stw.shangyingyoupin.top

Java: static void f() {}
来源：http://oxa.dashuyun.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zvo.yvedp.cn

Ruby: def self.f; end
来源：http://uri.zdqjudy.top

C#:   public static void F() {}
来源：http://oan.chenlongwang.top

[G09] 接口 / 抽象类
来源：http://nyp.fengsongda.top

Py:   from abc import ABC, abstractmethod
来源：http://avo.yuxming.cn

PHP:  interface Shape { public function area(): float; }
来源：http://urw.gotoacloud.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://aht.hcnkem.com

TS:   interface Shape { area(): number; }
来源：http://uzw.tarul.cn

Java: interface Shape { double area(); }
来源：http://rug.jqgufenzy.top

Go:   type Shape interface { Area() float64 }
来源：http://uvr.nanxinkj.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nee.yueranfly.top

C#:   interface IShape { double Area(); }
来源：http://xbd.hongshengwenyu.top

[G10] 访问控制
来源：http://mjh.chenlongwang.top

Py:   约定 _protected / __private（不强制）
来源：http://nbj.bjfxy.top

PHP:  public / protected / private
来源：http://aor.52xcode.cn

JS:   #private 字段；其余公开
来源：http://ciq.yongpay.top

TS:   public / protected / private
来源：http://rin.tanke756.top

Java: public / protected / private / 默认包级
来源：http://xwi.daxiang520.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qsu.ppjwa.cn

Ruby: public / protected / private
来源：http://lbv.yanxiufei.cn

C#:   public / protected / private / internal
来源：http://rkb.sufxvd.cn

[G11] getter / setter
来源：http://kpo.dianchejie.cn

Py:   @property 与 @x.setter
来源：http://pfp.xuanzx.com

PHP:  public function getName(): string { return $this->name; }
来源：http://msg.cucudq.cn

JS:   get name() { return this._name; }
来源：http://yvc.ivvv.top

TS:   get name(): string { return this._name; }
来源：http://sks.fehbvm.com

Java: public String getName() { return name; }
来源：http://jkl.tian-w.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ucc.yuxming.cn

Ruby: attr_accessor :name
来源：http://clr.jqgufenzy.top

C#:   public string Name { get; set; }
来源：http://phe.zhengqikj.top

[G12] 对象转字符串
来源：http://szh.yj20258888.top

Py:   def __str__(self): return self.name
来源：http://lyx.kuanghao11.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://efv.zhixingplan.top

JS:   toString() { return this.name; }
来源：http://wfs.hysaishi.cn

TS:   toString(): string { return this.name; }
来源：http://unw.xinyue.icu

Java: @Override public String toString() { return name; }
来源：http://qrl.svipenyu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ewc.dianchejie.cn

Ruby: def to_s; @name; end
来源：http://dbd.yfazqb.com

C#:   public override string ToString() => Name;
来源：http://qqx.sxryk.cn

[G13] 判断对象类型
来源：http://vtj.nanxuanxn.top

Py:   isinstance(u, User)
来源：http://zwl.yj20258888.top

PHP:  $u instanceof User
来源：http://fzm.jqgfzy.top

JS:   u instanceof User
来源：http://lfg.vehdjk.com

TS:   u instanceof User
来源：http://zqa.yuxming.cn

Java: u instanceof User
来源：http://fnh.iojbl.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cve.yangfankeji.com

Ruby: u.is_a?(User)
来源：http://klm.fktsv.cn

C#:   u is User
来源：http://ndk.ehwqpu.com

[G14] 数据类 / record
来源：http://qaz.jinyuanbaomall.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jic.kuanghao11.cn

PHP:  // 用 readonly 属性模拟
来源：http://kta.daxiang520.top

JS:   // 无内置：普通类或对象字面量
来源：http://bmn.pycfn.com

TS:   type User = { name: string; age: number };
来源：http://erf.dashuyun.cn

Java: record User(String name, int age) {}
来源：http://okv.sweek.top

Go:   type User struct { Name string; Age int }
来源：http://oux.hesvh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lez.cashguo.top

C#:   record User(string Name, int Age);
来源：http://yai.sjlbkw.cn

[G15] 枚举
来源：http://dxy.zhiwuduotai.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pag.nwbrower.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://xuu.shzxlz.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xya.ivvv.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://met.tian-w.cn

Java: enum Color { RED, GREEN }
来源：http://ynf.pycfn.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hjj.shanyushiyangkeji.top

Ruby: Color = %i[red green].freeze
来源：http://nzg.daria6918.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://aqs.ybcxt.top

[G16] 对象转数组 / 字典
来源：http://kaq.sweek.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uqg.vehdjk.com

PHP:  get_object_vars($obj);
来源：http://mcx.wangshuangyany.cn

JS:   Object.entries(obj)
来源：http://sgo.xylfe.cn

TS:   Object.entries(obj)
来源：http://czr.yonumen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qjt.jiagoushi.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://zae.hcnkem.com

Ruby: obj.instance_variables
来源：http://auw.aizwys.cn

C#:   // 用反射或 System.Text.Json
来源：http://zec.wangdashe.top

================================================================================
来源：http://jsm.iojbl.cn

H. 异常与错误处理
来源：http://yjw.jinghuilouyu.cn

================================================================================
来源：http://gzq.havefunace.top

[H01] try / catch 基础
来源：http://kzz.redwolf501.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://eac.tian-w.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ntm.ehwqpu.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sfy.ctjpmb.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sbm.pengpengdd.cyou

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dva.hongshengwenyu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://svh.gogol.net.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://adt.zhiwuduotai.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://miz.aibaodan.cn

[H02] finally / ensure 收尾
来源：http://cwh.sweek.top

Py:   try: f()⏎finally: cleanup()
来源：http://orw.yj202588.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://rdr.birdmap.top

JS:   try { f(); } finally { cleanup(); }
来源：http://npu.yuanzhike.top

TS:   try { f(); } finally { cleanup(); }
来源：http://qdx.cucudq.cn

Java: try { f(); } finally { cleanup(); }
来源：http://rbz.jinqigufen.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://eds.fktsv.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ahl.hfpthk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ozc.gzhubu.top

[H03] 主动抛出异常
来源：http://adq.yfazqb.com

Py:   raise ValueError("错误信息")
来源：http://tav.jinghuilouyu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cbc.meibo888.top

JS:   throw new Error("错误信息");
来源：http://hsx.yj202588.top

TS:   throw new Error("错误信息");
来源：http://sob.jyoumei.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://say.aibaodan.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oad.xuanzx.com

Ruby: raise ArgumentError, "错误信息"
来源：http://jua.fehbvm.com

C#:   throw new ArgumentException("错误信息");
来源：http://vfw.shangyingyoupin.top

[H04] 自定义异常类型
来源：http://eui.gogol.net.cn

Py:   class MyError(Exception): pass
来源：http://iwm.c1oappe.top

PHP:  class MyError extends RuntimeException {}
来源：http://wxj.aizwys.cn

JS:   class MyError extends Error {}
来源：http://tid.hysaishi.cn

TS:   class MyError extends Error {}
来源：http://ssm.aibaodan.cn

Java: class MyException extends RuntimeException {}
来源：http://boi.cdnleiting.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zyq.52xcode.cn

Ruby: class MyError < StandardError; end
来源：http://bmv.bjfxy.top

C#:   class MyException : Exception {}
来源：http://mki.yuanzhike.top

[H05] 捕获特定类型
来源：http://ugk.jinqigufen.top

Py:   except ValueError as e:
来源：http://rnf.guowangkeji.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dea.hywenlv.cn

JS:   if (e instanceof TypeError) {}
来源：http://kqu.ydjk.org.cn

TS:   if (e instanceof TypeError) {}
来源：http://ini.epnwcf.com

Java: catch (IOException | SQLException e) {}
来源：http://oxy.zhixingplan.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://joz.guowangkeji.top

Ruby: rescue ArgumentError => e
来源：http://pim.kuanghao11.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mnc.jyoumei.cn

[H06] 可选值 / 空值安全访问
来源：http://lvy.shuidangran.top

Py:   value = d.get("k") or default
来源：http://jgj.kuanghao11.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ofd.yonumen.top

JS:   obj?.a?.b;  d ?? default
来源：http://zhy.0kj1m.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mza.epnwcf.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pvu.52xcode.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vbk.xingfuxueyuan.xyz

Ruby: d&.dig(:a, :b)
来源：http://kvt.zhaomingkeji.xyz

C#:   obj?.A?.B ?? default
来源：http://lcu.cheryme.top

[H07] 断言
来源：http://wei.9152youxi.cn

Py:   assert x > 0, "必须为正"
来源：http://ncf.shanyushiyangkeji.top

PHP:  assert($x > 0);
来源：http://oeb.fanxiaobao.xyz

JS:   console.assert(x > 0);
来源：http://pwf.jinghuilouyu.cn

TS:   console.assert(x > 0);
来源：http://wvg.vehdjk.com

Java: assert x > 0 : "必须为正";
来源：http://bou.fengsongda.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vfb.hywenlv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wnc.xingfuxueyuan.xyz

C#:   Debug.Assert(x > 0);
来源：http://rcv.cdnleiting.top

[H08] 获取错误信息与堆栈
来源：http://eom.yfazqb.com

Py:   str(e);  traceback.format_exc()
来源：http://epg.yvedp.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hay.cucudq.cn

JS:   e.message;  e.stack
来源：http://bgj.hesvh.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hgq.snrcjt.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://smx.ywan-chungtsiang.top

Go:   err.Error()
来源：http://nvt.ctjpmb.com

Ruby: e.message;  e.backtrace
来源：http://tnd.jinqigfzy.top

C#:   e.Message;  e.StackTrace
来源：http://bcw.tian-w.cn

[H09] 带错误码的异常
来源：http://bto.yuxming.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fjk.yj20258888.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://viy.aizwys.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://izo.zhaomingkeji.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://imn.fktsv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://snk.dashuyun.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rfc.jinyuanbaomall.cn

Ruby: raise MyError.new("fail", 500)
来源：http://blg.hcnkem.com

C#:   // 自定义异常类中加 Code 属性
来源：http://ujm.316326.xyz

[H10] 资源自动释放
来源：http://gru.jinghuilouyu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fma.andypj.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gnl.shuidangran.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qoq.daxiang520.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tzg.zycfv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xmg.jqgfzy.top

Go:   defer f.Close()
来源：http://wjq.tian-w.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ymp.andypj.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bqh.jinghuilouyu.cn

================================================================================
来源：http://uux.tianlin.xyz

I. 正则表达式
来源：http://fkz.ppjwa.cn

================================================================================
来源：http://yvy.gzhubu.top

[I01] 判断是否匹配
来源：http://ecv.meibo888.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yqr.yuanzhike.top

PHP:  preg_match('/\d+/', $s);
来源：http://bhm.andypj.xyz

JS:   /\d+/.test(s)
来源：http://daj.guowangkeji.top

TS:   /\d+/.test(s)
来源：http://mly.quarkkingdee.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tzj.sysykeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://odr.fzhhl.top

Ruby: s.match?(/\d+/)
来源：http://dxu.aibaodan.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ldc.sysykeji.top

[I02] 提取所有匹配
来源：http://omj.fktsv.cn

Py:   re.findall(r"\d+", s)
来源：http://kyg.xylfe.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nxk.dianchejie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pzi.jianghu66.top

TS:   s.match(/\d+/g)
来源：http://pvw.xuanzx.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xdd.nwbrower.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jpf.quarkkingdee.top

Ruby: s.scan(/\d+/)
来源：http://yya.chenzaomai.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://spn.fktsv.cn

[I03] 提取捕获分组
来源：http://lbn.ydzc1.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://crz.chenlongwang.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yhc.yj20258888.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ytn.yj20258888.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ago.zhoulong.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lqp.guannengcc.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cip.jinqigufen.top


<!-- 参考信息 -->