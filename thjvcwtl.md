代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://vrq.shanyushiyangkeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dve.uphjek.com

JS:   fs.readdirSync("dir")
来源：http://byr.shzxlz.cn

TS:   fs.readdirSync("dir")
来源：http://uku.cqqwz.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lce.cheryme.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://naz.gaohongyu789.top

Ruby: Dir.children("dir")
来源：http://utf.ybcxt.top

C#:   Directory.GetFiles("dir")
来源：http://ban.hywenlv.cn

[F09] 获取文件大小
来源：http://vxp.zhongyouzk.top

Py:   os.path.getsize("a.txt")
来源：http://hus.ywan-chungtsiang.top

PHP:  filesize("a.txt");
来源：http://wvl.smart0.xyz

JS:   fs.statSync("a.txt").size
来源：http://woo.zhiwuduotai.top

TS:   fs.statSync("a.txt").size
来源：http://vyj.cucudq.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qck.hnxiangtu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vgl.gotoacloud.top

Ruby: File.size("a.txt")
来源：http://kgw.hysaishi.cn

C#:   new FileInfo("a.txt").Length
来源：http://cuq.yvedp.cn

[F10] 取文件扩展名 / 文件名
来源：http://pho.316326.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mui.jinghuilouyu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qle.nanxinkj.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ruv.vqdsnc.cn

TS:   path.extname("a.txt")
来源：http://gjw.shanyushiyangkeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fow.redwolf501.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zed.svipenyu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mfw.daxiang520.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uxr.jqgfzy.top

[F11] 复制与移动文件
来源：http://yvy.svipenyu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cjp.vqdsnc.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dzr.meibo888.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cmm.cqqwz.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uls.hnqzz.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zoe.zhaomingkeji.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nzd.zdbjq.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://brq.cucudq.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bkk.c1oappe.top

[F12] CSV 读写
来源：http://nvt.cheryme.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pws.guannengcc.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://aei.zdbjq.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fye.tianlin.xyz

TS:   // 同上
来源：http://usr.yongpay.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hdb.haohaochexian.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tpy.hammf.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qbf.pengpengdd.cyou

C#:   // 无内置：用 CsvHelper 库
来源：http://can.gogol.net.cn

================================================================================
来源：http://ozb.meibo888.top

G. 面向对象
来源：http://eto.shangyingyoupin.top

================================================================================
来源：http://wmp.9152youxi.cn

[G01] 定义类
来源：http://rea.fktsv.cn

Py:   class User: pass
来源：http://wmw.ywan-chungtsiang.top

PHP:  class User {}
来源：http://wfk.uphjek.com

JS:   class User {}
来源：http://acv.yangfankeji.com

TS:   class User { name: string = ""; }
来源：http://hxj.cqqwz.cn

Java: class User {}
来源：http://kdz.jinqigfzy.top

Go:   type User struct { Name string }
来源：http://jty.pycfn.com

Ruby: class User; end
来源：http://tyr.iojbl.cn

C#:   class User {}
来源：http://ioc.snrcjt.cn

[G02] 构造函数
来源：http://hud.pengpengdd.cyou

Py:   def __init__(self, name): self.name = name
来源：http://yqd.pycfn.com

PHP:  public function __construct(public string $name) {}
来源：http://ikg.cqqwz.cn

JS:   constructor(name) { this.name = name; }
来源：http://jnc.iojbl.cn

TS:   constructor(public name: string) {}
来源：http://xmq.jqgufenzy.top

Java: User(String name) { this.name = name; }
来源：http://pnf.shzxlz.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://evz.wangshuangyany.cn

Ruby: def initialize(name); @name = name; end
来源：http://oii.zhijiandao.cn

C#:   public User(string name) { Name = name; }
来源：http://zwd.sjlbkw.cn

[G03] 实例属性
来源：http://cia.cqqwz.cn

Py:   self.name = "x"
来源：http://etq.hcnkem.com

PHP:  public string $name = "x";
来源：http://ihh.gogol.net.cn

JS:   this.name = "x";
来源：http://ebn.uphjek.com

TS:   name: string = "x";
来源：http://fij.shanyushiyangkeji.top

Java: private String name;
来源：http://gax.uphjek.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://iyj.vehdjk.com

Ruby: @name = "x"
来源：http://qsa.hesvh.cn

C#:   public string Name { get; set; } = "x";
来源：http://egq.wangdashe.top

[G04] 定义方法
来源：http://rxu.jinqigfzy.top

Py:   def greet(self): return self.name
来源：http://btk.fzhhl.top

PHP:  public function greet(): string { return $this->name; }
来源：http://mmb.shangyingyoupin.top

JS:   greet() { return this.name; }
来源：http://vrr.tian-w.cn

TS:   greet(): string { return this.name; }
来源：http://iqi.chenlongwang.top

Java: String greet() { return name; }
来源：http://ztc.sweek.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://apr.chenlongwang.top

Ruby: def greet; @name; end
来源：http://lsq.jqgufenzy.top

C#:   public string Greet() => Name;
来源：http://uds.pycfn.com

[G05] 继承
来源：http://gub.pengpengdd.cyou

Py:   class Admin(User): pass
来源：http://naf.nanxinkj.top

PHP:  class Admin extends User {}
来源：http://ctj.havefunace.top

JS:   class Admin extends User {}
来源：http://ihe.fehbvm.com

TS:   class Admin extends User {}
来源：http://zgd.jinyuanbaomall.cn

Java: class Admin extends User {}
来源：http://rmq.zhijiandao.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://any.feifeiyinyue.top

Ruby: class Admin < User; end
来源：http://ezl.shangyingyoupin.top

C#:   class Admin : User {}
来源：http://zda.pengpengdd.cyou

[G06] 重写方法
来源：http://hdr.hfpthk.cn

Py:   def greet(self): return "admin"
来源：http://oix.fehbvm.com

PHP:  public function greet(): string { return "admin"; }
来源：http://ili.52xcode.cn

JS:   greet() { return "admin"; }
来源：http://fmm.hfpthk.cn

TS:   greet(): string { return "admin"; }
来源：http://acf.ybcxt.top

Java: @Override String greet() { return "admin"; }
来源：http://lro.cqqwz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fap.yangfankeji.com

Ruby: def greet; "admin"; end
来源：http://yme.nanxinkj.top

C#:   public override string Greet() => "admin";
来源：http://qrn.vehdjk.com

[G07] 调用父类方法
来源：http://jqt.sjlbkw.cn

Py:   super().greet()
来源：http://jsc.guannengcc.top

PHP:  parent::greet();
来源：http://qbg.hnqzz.top

JS:   super.greet();
来源：http://bza.xuanzx.com

TS:   super.greet();
来源：http://ryx.smart0.xyz

Java: super.greet();
来源：http://sof.xingfuxueyuan.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://erv.cashguo.top

Ruby: super
来源：http://yrr.jqgfzy.top

C#:   base.Greet();
来源：http://kza.sysykeji.top

[G08] 静态方法与属性
来源：http://gdy.hnqzz.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://eer.iojbl.cn

PHP:  public static function f() {}
来源：http://ukg.pycfn.com

JS:   static f() {}
来源：http://qdp.xinyue.icu

TS:   static f(): void {}
来源：http://vsu.chenzaomai.com

Java: static void f() {}
来源：http://pwz.cqqwz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://czo.yvedp.cn

Ruby: def self.f; end
来源：http://xzn.hongshengwenyu.top

C#:   public static void F() {}
来源：http://mmi.fehbvm.com

[G09] 接口 / 抽象类
来源：http://lsi.yonumen.top

Py:   from abc import ABC, abstractmethod
来源：http://mtr.hywenlv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zzl.epnwcf.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://zdq.bjfxy.top

TS:   interface Shape { area(): number; }
来源：http://xvz.jinyuanbaomall.cn

Java: interface Shape { double area(); }
来源：http://vfu.shanyushiyangkeji.top

Go:   type Shape interface { Area() float64 }
来源：http://rrh.chenjidiqi.icu

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dws.yonumen.top

C#:   interface IShape { double Area(); }
来源：http://jni.jqgfzy.top

[G10] 访问控制
来源：http://bom.ybcxt.top

Py:   约定 _protected / __private（不强制）
来源：http://tyz.ehwqpu.com

PHP:  public / protected / private
来源：http://jxd.gaohongyu789.top

JS:   #private 字段；其余公开
来源：http://tpa.aibaodan.cn

TS:   public / protected / private
来源：http://ugy.c1oappe.top

Java: public / protected / private / 默认包级
来源：http://rrd.hnxiangtu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://jzv.52xcode.cn

Ruby: public / protected / private
来源：http://vme.fanxiaobao.xyz

C#:   public / protected / private / internal
来源：http://apg.316326.xyz

[G11] getter / setter
来源：http://htx.ydzc1.top

Py:   @property 与 @x.setter
来源：http://fep.zhoulong.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://ycb.ydzc1.top

JS:   get name() { return this._name; }
来源：http://bsb.yanxiufei.cn

TS:   get name(): string { return this._name; }
来源：http://adb.316326.xyz

Java: public String getName() { return name; }
来源：http://xmb.iojbl.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dtv.fanxiaobao.xyz

Ruby: attr_accessor :name
来源：http://tlg.xziqi.cn

C#:   public string Name { get; set; }
来源：http://crr.uphjek.com

[G12] 对象转字符串
来源：http://mec.cucudq.cn

Py:   def __str__(self): return self.name
来源：http://jns.shanyushiyangtech.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://lbl.ywan-chungtsiang.top

JS:   toString() { return this.name; }
来源：http://pyg.haohaochexian.top

TS:   toString(): string { return this.name; }
来源：http://bgv.bbcook.cn

Java: @Override public String toString() { return name; }
来源：http://mzd.wangshuangyany.cn

Go:   func (u User) String() string { return u.Name }
来源：http://grh.shanyushiyangtech.top

Ruby: def to_s; @name; end
来源：http://zmq.meibo888.top

C#:   public override string ToString() => Name;
来源：http://mzh.jinghuilouyu.cn

[G13] 判断对象类型
来源：http://blg.svipenyu.cn

Py:   isinstance(u, User)
来源：http://zem.shzxlz.cn

PHP:  $u instanceof User
来源：http://mdy.zycfv.cn

JS:   u instanceof User
来源：http://hxh.daria6918.cn

TS:   u instanceof User
来源：http://fzt.yj20258.top

Java: u instanceof User
来源：http://cst.jqgufenzy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ukp.shuidangran.top

Ruby: u.is_a?(User)
来源：http://tmt.zhoulong.xyz

C#:   u is User
来源：http://gvr.iojbl.cn

[G14] 数据类 / record
来源：http://emv.dianchejie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ezb.zhongyouzk.top

PHP:  // 用 readonly 属性模拟
来源：http://btc.jinqigufen.top

JS:   // 无内置：普通类或对象字面量
来源：http://qrl.jinqigufen.top

TS:   type User = { name: string; age: number };
来源：http://dba.jianghu66.top

Java: record User(String name, int age) {}
来源：http://mus.xingfuxueyuan.xyz

Go:   type User struct { Name string; Age int }
来源：http://kwr.andypj.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qlx.vehdjk.com

C#:   record User(string Name, int Age);
来源：http://qht.guowangkeji.top

[G15] 枚举
来源：http://dys.jinqigfzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kfw.meibo888.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://sms.shanyushiyangtech.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jsn.xylfe.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mfj.cucudq.cn

Java: enum Color { RED, GREEN }
来源：http://sbr.hysaishi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vvr.hcnkem.com

Ruby: Color = %i[red green].freeze
来源：http://bqf.dashuyun.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vcb.pengpengdd.cyou

[G16] 对象转数组 / 字典
来源：http://ccs.sweek.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cvn.zdbjq.cn

PHP:  get_object_vars($obj);
来源：http://yts.0kj1m.cn

JS:   Object.entries(obj)
来源：http://mef.wangdashe.top

TS:   Object.entries(obj)
来源：http://dgm.yuanzhike.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wcq.xinyue.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://uaa.zhaomingkeji.xyz

Ruby: obj.instance_variables
来源：http://eak.ybcxt.top

C#:   // 用反射或 System.Text.Json
来源：http://bbf.hcnkem.com

================================================================================
来源：http://umk.kuanghao11.cn

H. 异常与错误处理
来源：http://qyv.chenlongwang.top

================================================================================
来源：http://wxi.ydjk.org.cn

[H01] try / catch 基础
来源：http://ppd.xingfuxueyuan.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mlu.yonumen.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://oyg.haohaochexian.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ock.sufxvd.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ads.redwolf501.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://exx.zhaomingkeji.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qkg.ywan-chungtsiang.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ahe.chenjidiqi.icu

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qxp.shanyushiyangtech.top

[H02] finally / ensure 收尾
来源：http://ycb.hcnkem.com

Py:   try: f()⏎finally: cleanup()
来源：http://fnm.mhx1999.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://kmw.zycfv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tij.jlsjyb.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zfk.bjfxy.top

Java: try { f(); } finally { cleanup(); }
来源：http://yyq.hfpthk.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mto.svipenyu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://yqw.snrcjt.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cbq.jqgfzy.top

[H03] 主动抛出异常
来源：http://ned.sxryk.cn

Py:   raise ValueError("错误信息")
来源：http://jpz.chenzaomai.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hsy.yuxming.cn

JS:   throw new Error("错误信息");
来源：http://znv.jqgfzy.top

TS:   throw new Error("错误信息");
来源：http://wfw.snrcjt.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qni.zdqjudy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://byv.jqgufenzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://bxi.ppjwa.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zcs.fktsv.cn

[H04] 自定义异常类型
来源：http://zlp.xuanzx.com

Py:   class MyError(Exception): pass
来源：http://rrb.haohaochexian.top

PHP:  class MyError extends RuntimeException {}
来源：http://dvu.chenzaomai.com

JS:   class MyError extends Error {}
来源：http://jzv.yvedp.cn

TS:   class MyError extends Error {}
来源：http://pat.guowangkeji.top

Java: class MyException extends RuntimeException {}
来源：http://sya.yj20258.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hhi.yj202588.top

Ruby: class MyError < StandardError; end
来源：http://kog.cqqwz.cn

C#:   class MyException : Exception {}
来源：http://ruo.ywan-chungtsiang.top

[H05] 捕获特定类型
来源：http://ofn.xziqi.cn

Py:   except ValueError as e:
来源：http://kob.tanke756.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nah.gogol.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://pia.hesvh.cn

TS:   if (e instanceof TypeError) {}
来源：http://far.pengpengdd.cyou

Java: catch (IOException | SQLException e) {}
来源：http://gyf.gogol.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qjl.yangfankeji.com

Ruby: rescue ArgumentError => e
来源：http://lbo.nanxuanxn.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gjt.hfpthk.cn

[H06] 可选值 / 空值安全访问
来源：http://dfy.vehdjk.com

Py:   value = d.get("k") or default
来源：http://yzt.yuanzhike.top

PHP:  $v = $d["k"] ?? null;
来源：http://fwf.ehwqpu.com

JS:   obj?.a?.b;  d ?? default
来源：http://vgf.bjfxy.top

TS:   obj?.a?.b;  d ?? default
来源：http://ldq.svipenyu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xgw.cucudq.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xkd.sysykeji.top

Ruby: d&.dig(:a, :b)
来源：http://xid.xuanzx.com

C#:   obj?.A?.B ?? default
来源：http://wzl.yfazqb.com

[H07] 断言
来源：http://ezl.ehwqpu.com

Py:   assert x > 0, "必须为正"
来源：http://hxl.yfazqb.com

PHP:  assert($x > 0);
来源：http://new.hfpthk.cn

JS:   console.assert(x > 0);
来源：http://gmm.zhoulong.xyz

TS:   console.assert(x > 0);
来源：http://vqm.tarul.cn

Java: assert x > 0 : "必须为正";
来源：http://zsy.yvedp.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xuk.chenlongwang.top

Ruby: raise "必须为正" unless x > 0
来源：http://rqc.hcnkem.com

C#:   Debug.Assert(x > 0);
来源：http://sne.c1oappe.top

[H08] 获取错误信息与堆栈
来源：http://mbg.chenlongwang.top

Py:   str(e);  traceback.format_exc()
来源：http://ged.fengsongda.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bvz.ppjwa.cn

JS:   e.message;  e.stack
来源：http://nje.yfazqb.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://kxp.yuxming.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ruf.jinghuilouyu.cn

Go:   err.Error()
来源：http://ssc.shanyushiyangtech.top

Ruby: e.message;  e.backtrace
来源：http://mpa.kuanghao11.cn

C#:   e.Message;  e.StackTrace
来源：http://xvr.guowangkeji.top

[H09] 带错误码的异常
来源：http://lgz.yuxming.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bhv.cashguo.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://mgh.hfpthk.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zdu.xziqi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ojm.fehbvm.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pdb.xuanzx.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rwm.smart0.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://unj.ppjwa.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://dnq.gzhubu.top

[H10] 资源自动释放
来源：http://wqp.yangfankeji.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://fii.yj20258.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jef.kuanghao11.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://buv.snrcjt.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nkf.xylfe.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xph.sufxvd.cn

Go:   defer f.Close()
来源：http://gzn.vehdjk.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fpo.hysaishi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://iku.fengsongda.top

================================================================================
来源：http://bcg.0kj1m.cn

I. 正则表达式
来源：http://zyq.gzhubu.top

================================================================================
来源：http://seu.svipenyu.cn

[I01] 判断是否匹配
来源：http://pza.wangdashe.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ngr.yangfankeji.com

PHP:  preg_match('/\d+/', $s);
来源：http://lce.xuanzx.com

JS:   /\d+/.test(s)
来源：http://zlj.vehdjk.com

TS:   /\d+/.test(s)
来源：http://rvd.wangdashe.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mno.vqdsnc.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fgl.jiagoushi.top

Ruby: s.match?(/\d+/)
来源：http://anh.yuxming.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mqb.iojbl.cn

[I02] 提取所有匹配
来源：http://alf.hongshengwenyu.top

Py:   re.findall(r"\d+", s)
来源：http://zpv.xuanzx.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wzv.zhiwuduotai.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://skb.andypj.xyz


<!-- 参考信息 -->