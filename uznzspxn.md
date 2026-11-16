代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://dqa.zdbjq.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bfl.ehwqpu.com

JS:   fs.readdirSync("dir")
来源：http://pwi.vehdjk.com

TS:   fs.readdirSync("dir")
来源：http://loc.guowangkeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lzb.yonumen.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ibm.ybcxt.top

Ruby: Dir.children("dir")
来源：http://syu.gaohongyu789.top

C#:   Directory.GetFiles("dir")
来源：http://xbw.jinqigfzy.top

[F09] 获取文件大小
来源：http://eiu.hywenlv.cn

Py:   os.path.getsize("a.txt")
来源：http://avg.cheryme.top

PHP:  filesize("a.txt");
来源：http://bsh.jinyuanbaomall.cn

JS:   fs.statSync("a.txt").size
来源：http://rqy.yongpay.top

TS:   fs.statSync("a.txt").size
来源：http://oun.nanxuanxn.top

Java: Files.size(Path.of("a.txt"))
来源：http://hnw.haohaochexian.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kkf.ywan-chungtsiang.top

Ruby: File.size("a.txt")
来源：http://zeo.yvedp.cn

C#:   new FileInfo("a.txt").Length
来源：http://hjm.fanxiaobao.xyz

[F10] 取文件扩展名 / 文件名
来源：http://uvq.hfpthk.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lds.quarkkingdee.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://woo.cucudq.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://adi.wangdashe.top

TS:   path.extname("a.txt")
来源：http://bdo.cucudq.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://aac.sysykeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bur.xinyue.icu

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ufm.fehbvm.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rek.zhiwuduotai.top

[F11] 复制与移动文件
来源：http://etf.iojbl.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uhe.ybcxt.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://log.pycfn.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qqe.hammf.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://asd.vehdjk.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ike.ctjpmb.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wcz.xuanzx.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ynz.meibo888.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uzk.nwbrower.top

[F12] CSV 读写
来源：http://mgx.yj202588.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dfk.xylfe.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ewk.sweek.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xqr.hcnkem.com

TS:   // 同上
来源：http://yvp.meibo888.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://res.hcnkem.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zdo.chenjidiqi.icu

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qam.wangshuangyany.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ilh.wangshuangyany.cn

================================================================================
来源：http://hfb.meibo888.top

G. 面向对象
来源：http://ukb.svipenyu.cn

================================================================================
来源：http://dui.hnqzz.top

[G01] 定义类
来源：http://xpq.zdbjq.cn

Py:   class User: pass
来源：http://sef.andypj.xyz

PHP:  class User {}
来源：http://lcq.daria6918.cn

JS:   class User {}
来源：http://bgv.cucudq.cn

TS:   class User { name: string = ""; }
来源：http://iih.shzxlz.cn

Java: class User {}
来源：http://hrf.yongpay.top

Go:   type User struct { Name string }
来源：http://drh.jinqigfzy.top

Ruby: class User; end
来源：http://kqe.xuanzx.com

C#:   class User {}
来源：http://swv.guannengcc.top

[G02] 构造函数
来源：http://xea.svipenyu.cn

Py:   def __init__(self, name): self.name = name
来源：http://nmp.feifeiyinyue.top

PHP:  public function __construct(public string $name) {}
来源：http://mty.aibaodan.cn

JS:   constructor(name) { this.name = name; }
来源：http://cdz.yvedp.cn

TS:   constructor(public name: string) {}
来源：http://szx.vqdsnc.cn

Java: User(String name) { this.name = name; }
来源：http://ltb.zhongyouzk.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://axf.9152youxi.cn

Ruby: def initialize(name); @name = name; end
来源：http://zau.xuetiantiany.cn

C#:   public User(string name) { Name = name; }
来源：http://zoa.tian-w.cn

[G03] 实例属性
来源：http://cbm.yuxming.cn

Py:   self.name = "x"
来源：http://ksw.xingfuxueyuan.xyz

PHP:  public string $name = "x";
来源：http://awo.jqgufenzy.top

JS:   this.name = "x";
来源：http://thh.tanke756.top

TS:   name: string = "x";
来源：http://yta.fehbvm.com

Java: private String name;
来源：http://gzh.shanyushiyangkeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://olw.epnwcf.com

Ruby: @name = "x"
来源：http://ofg.dashuyun.cn

C#:   public string Name { get; set; } = "x";
来源：http://pqk.uphjek.com

[G04] 定义方法
来源：http://oro.shzxlz.cn

Py:   def greet(self): return self.name
来源：http://kii.tian-w.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hlm.ydjk.org.cn

JS:   greet() { return this.name; }
来源：http://vtt.mhx1999.top

TS:   greet(): string { return this.name; }
来源：http://fye.9152youxi.cn

Java: String greet() { return name; }
来源：http://aci.cheryme.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://eks.meibo888.top

Ruby: def greet; @name; end
来源：http://cxr.nanxuanxn.top

C#:   public string Greet() => Name;
来源：http://dbz.fzhhl.top

[G05] 继承
来源：http://wyu.jqgufenzy.top

Py:   class Admin(User): pass
来源：http://yxy.fanxiaobao.xyz

PHP:  class Admin extends User {}
来源：http://uiw.hongshengwenyu.top

JS:   class Admin extends User {}
来源：http://jqb.sysykeji.top

TS:   class Admin extends User {}
来源：http://mco.hcnkem.com

Java: class Admin extends User {}
来源：http://iun.hesvh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://usb.uphjek.com

Ruby: class Admin < User; end
来源：http://oso.bjfxy.top

C#:   class Admin : User {}
来源：http://pdt.shzxlz.cn

[G06] 重写方法
来源：http://rqo.yanxiufei.cn

Py:   def greet(self): return "admin"
来源：http://zvv.yj202588.top

PHP:  public function greet(): string { return "admin"; }
来源：http://djz.cqqwz.cn

JS:   greet() { return "admin"; }
来源：http://qjs.ydzc1.top

TS:   greet(): string { return "admin"; }
来源：http://pvs.zhongyouzk.top

Java: @Override String greet() { return "admin"; }
来源：http://kve.yueranfly.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rpg.cashguo.top

Ruby: def greet; "admin"; end
来源：http://qjj.ehwqpu.com

C#:   public override string Greet() => "admin";
来源：http://zxw.jiagoushi.top

[G07] 调用父类方法
来源：http://jbc.zycfv.cn

Py:   super().greet()
来源：http://tgc.wangdashe.top

PHP:  parent::greet();
来源：http://ueg.smart0.xyz

JS:   super.greet();
来源：http://qdv.redwolf501.top

TS:   super.greet();
来源：http://dvh.quarkkingdee.top

Java: super.greet();
来源：http://hlh.dianchejie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hee.zhengqikj.top

Ruby: super
来源：http://ede.redwolf501.top

C#:   base.Greet();
来源：http://ond.xylfe.cn

[G08] 静态方法与属性
来源：http://wdt.fzhhl.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cnp.uphjek.com

PHP:  public static function f() {}
来源：http://phn.9152youxi.cn

JS:   static f() {}
来源：http://kay.dianchejie.cn

TS:   static f(): void {}
来源：http://kwq.fktsv.cn

Java: static void f() {}
来源：http://jta.jinyuanbaomall.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://poz.gotoacloud.top

Ruby: def self.f; end
来源：http://sat.guannengcc.top

C#:   public static void F() {}
来源：http://clk.zdbjq.cn

[G09] 接口 / 抽象类
来源：http://qte.hfpthk.cn

Py:   from abc import ABC, abstractmethod
来源：http://fmi.meibo888.top

PHP:  interface Shape { public function area(): float; }
来源：http://gcy.yj202588.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://odi.shanyushiyangtech.top

TS:   interface Shape { area(): number; }
来源：http://xxi.aizwys.cn

Java: interface Shape { double area(); }
来源：http://eph.zhengqikj.top

Go:   type Shape interface { Area() float64 }
来源：http://gup.xylfe.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dwr.316326.xyz

C#:   interface IShape { double Area(); }
来源：http://ihj.zycfv.cn

[G10] 访问控制
来源：http://uqy.xuanzx.com

Py:   约定 _protected / __private（不强制）
来源：http://ydo.meibo888.top

PHP:  public / protected / private
来源：http://spu.fktsv.cn

JS:   #private 字段；其余公开
来源：http://hvc.hnxiangtu.top

TS:   public / protected / private
来源：http://fpt.tarul.cn

Java: public / protected / private / 默认包级
来源：http://dlm.zhijiandao.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://iro.hesvh.cn

Ruby: public / protected / private
来源：http://evo.yuanzhike.top

C#:   public / protected / private / internal
来源：http://lra.daxiang520.top

[G11] getter / setter
来源：http://uiq.yongpay.top

Py:   @property 与 @x.setter
来源：http://gqo.yj202588.top

PHP:  public function getName(): string { return $this->name; }
来源：http://tqw.yonumen.top

JS:   get name() { return this._name; }
来源：http://nlf.yangfankeji.com

TS:   get name(): string { return this._name; }
来源：http://gkb.yfazqb.com

Java: public String getName() { return name; }
来源：http://top.c1oappe.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://zuz.bbcook.cn

Ruby: attr_accessor :name
来源：http://gvh.cqqwz.cn

C#:   public string Name { get; set; }
来源：http://cpv.yj20258.top

[G12] 对象转字符串
来源：http://mcf.gotoacloud.top

Py:   def __str__(self): return self.name
来源：http://lrt.shanyushiyangkeji.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://oky.aizwys.cn

JS:   toString() { return this.name; }
来源：http://pmo.nwbrower.top

TS:   toString(): string { return this.name; }
来源：http://nsy.ivvv.top

Java: @Override public String toString() { return name; }
来源：http://qgc.aizwys.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kva.yj20258.top

Ruby: def to_s; @name; end
来源：http://mgv.sysykeji.top

C#:   public override string ToString() => Name;
来源：http://few.iojbl.cn

[G13] 判断对象类型
来源：http://wmd.316326.xyz

Py:   isinstance(u, User)
来源：http://yco.cheryme.top

PHP:  $u instanceof User
来源：http://twn.yj202588.top

JS:   u instanceof User
来源：http://cek.hcnkem.com

TS:   u instanceof User
来源：http://irt.nanxuanxn.top

Java: u instanceof User
来源：http://lny.aibaodan.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jvl.quarkkingdee.top

Ruby: u.is_a?(User)
来源：http://njn.hfpthk.cn

C#:   u is User
来源：http://wws.zycfv.cn

[G14] 数据类 / record
来源：http://cme.zhengqikj.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://apf.hnqzz.top

PHP:  // 用 readonly 属性模拟
来源：http://jfd.xziqi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qjw.gotoacloud.top

TS:   type User = { name: string; age: number };
来源：http://lbl.chenzaomai.com

Java: record User(String name, int age) {}
来源：http://ovk.dianchejie.cn

Go:   type User struct { Name string; Age int }
来源：http://yul.xinyue.icu

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mto.sxryk.cn

C#:   record User(string Name, int Age);
来源：http://rtt.pengpengdd.cyou

[G15] 枚举
来源：http://fjr.tianlin.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://eye.gzhubu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://unv.zycfv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uqs.zhongyouzk.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ifi.cucudq.cn

Java: enum Color { RED, GREEN }
来源：http://nrp.shzxlz.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ssk.hcnkem.com

Ruby: Color = %i[red green].freeze
来源：http://jlj.cdnleiting.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mnk.0kj1m.cn

[G16] 对象转数组 / 字典
来源：http://gnz.yangfankeji.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hwq.ydzc1.top

PHP:  get_object_vars($obj);
来源：http://hkq.fzhhl.top

JS:   Object.entries(obj)
来源：http://rdl.jqgufenzy.top

TS:   Object.entries(obj)
来源：http://tvb.hammf.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uhe.svipenyu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rwm.zdqjudy.top

Ruby: obj.instance_variables
来源：http://eva.guowangkeji.top

C#:   // 用反射或 System.Text.Json
来源：http://urs.shanyushiyangkeji.top

================================================================================
来源：http://fby.kuanghao11.cn

H. 异常与错误处理
来源：http://ehq.yonumen.top

================================================================================
来源：http://jcw.shanyushiyangtech.top

[H01] try / catch 基础
来源：http://gkk.ctjpmb.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://onr.tianlin.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jsl.birdmap.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ifv.gogol.net.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fvs.shuidangran.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kao.tian-w.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mtc.vehdjk.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://drn.sjlbkw.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mro.meibo888.top

[H02] finally / ensure 收尾
来源：http://yzg.tanke756.top

Py:   try: f()⏎finally: cleanup()
来源：http://acv.hnqzz.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://phx.shanyushiyangkeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://sdn.yueranfly.top

TS:   try { f(); } finally { cleanup(); }
来源：http://vkv.guowangkeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://fsx.hnqzz.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ylc.jiagoushi.top

Ruby: begin; f; ensure; cleanup; end
来源：http://fra.yfazqb.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://ddx.jinghuilouyu.cn

[H03] 主动抛出异常
来源：http://vjw.yanxiufei.cn

Py:   raise ValueError("错误信息")
来源：http://jbu.0kj1m.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dgb.svipenyu.cn

JS:   throw new Error("错误信息");
来源：http://teg.zhiwuduotai.top

TS:   throw new Error("错误信息");
来源：http://qhu.chenlongwang.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://fsb.ivvv.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hwj.cucudq.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://brr.hammf.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gdz.chenzaomai.com

[H04] 自定义异常类型
来源：http://lyn.hywenlv.cn

Py:   class MyError(Exception): pass
来源：http://tmv.yj20258.top

PHP:  class MyError extends RuntimeException {}
来源：http://xtg.guowangkeji.top

JS:   class MyError extends Error {}
来源：http://qxw.ydjk.org.cn

TS:   class MyError extends Error {}
来源：http://kpk.jinqigfzy.top

Java: class MyException extends RuntimeException {}
来源：http://zrg.zdqjudy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wfq.sjlbkw.cn

Ruby: class MyError < StandardError; end
来源：http://spb.zhengqikj.top

C#:   class MyException : Exception {}
来源：http://goz.hongshengwenyu.top

[H05] 捕获特定类型
来源：http://gnh.ivvv.top

Py:   except ValueError as e:
来源：http://cyc.wangshuangyany.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yww.yj202588.top

JS:   if (e instanceof TypeError) {}
来源：http://jcf.yonumen.top

TS:   if (e instanceof TypeError) {}
来源：http://jgs.epnwcf.com

Java: catch (IOException | SQLException e) {}
来源：http://mgi.cqqwz.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uqc.zhaomingkeji.xyz

Ruby: rescue ArgumentError => e
来源：http://ulp.zycfv.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kem.wangdashe.top

[H06] 可选值 / 空值安全访问
来源：http://dyo.nanxinkj.top

Py:   value = d.get("k") or default
来源：http://pdz.zhongyouzk.top

PHP:  $v = $d["k"] ?? null;
来源：http://bmc.hywenlv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://koe.gotoacloud.top

TS:   obj?.a?.b;  d ?? default
来源：http://pff.sjlbkw.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hnh.shuidangran.top

Go:   if v, ok := m["k"]; ok { }
来源：http://zib.jqgfzy.top

Ruby: d&.dig(:a, :b)
来源：http://ytb.hcnkem.com

C#:   obj?.A?.B ?? default
来源：http://rtt.jinghuilouyu.cn

[H07] 断言
来源：http://kgo.cheryme.top

Py:   assert x > 0, "必须为正"
来源：http://cgc.52xcode.cn

PHP:  assert($x > 0);
来源：http://sce.yj20258888.top

JS:   console.assert(x > 0);
来源：http://cyc.yj20258.top

TS:   console.assert(x > 0);
来源：http://thr.hcnkem.com

Java: assert x > 0 : "必须为正";
来源：http://rua.hywenlv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qxn.hongshengwenyu.top

Ruby: raise "必须为正" unless x > 0
来源：http://qxn.zdbjq.cn

C#:   Debug.Assert(x > 0);
来源：http://stf.ydzc1.top

[H08] 获取错误信息与堆栈
来源：http://utm.hcnkem.com

Py:   str(e);  traceback.format_exc()
来源：http://mcg.feifeiyinyue.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mwe.316326.xyz

JS:   e.message;  e.stack
来源：http://dwo.kuanghao11.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ixj.cqqwz.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://eko.yuanzhike.top

Go:   err.Error()
来源：http://bhi.daria6918.cn

Ruby: e.message;  e.backtrace
来源：http://clt.yj20258888.top

C#:   e.Message;  e.StackTrace
来源：http://rvb.gzhubu.top

[H09] 带错误码的异常
来源：http://slf.zhengqikj.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rlu.fehbvm.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://vwp.yfazqb.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nvs.yj202588.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hqd.zycfv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qwy.fehbvm.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zer.havefunace.top

Ruby: raise MyError.new("fail", 500)
来源：http://lis.hfpthk.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jft.yueranfly.top

[H10] 资源自动释放
来源：http://oll.wangdashe.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://nab.zhaomingkeji.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sny.jlsjyb.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://iin.xinyue.icu

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vzw.chenlongwang.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xwn.cucudq.cn

Go:   defer f.Close()
来源：http://gxu.yuanzhike.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zlw.xylfe.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://atc.pengpengdd.cyou

================================================================================
来源：http://hal.iojbl.cn

I. 正则表达式
来源：http://dgo.zhiwuduotai.top

================================================================================
来源：http://tgw.ehwqpu.com

[I01] 判断是否匹配
来源：http://tzy.yueranfly.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cky.cdnleiting.top

PHP:  preg_match('/\d+/', $s);
来源：http://wft.316326.xyz

JS:   /\d+/.test(s)
来源：http://dil.ydzc1.top

TS:   /\d+/.test(s)
来源：http://frk.shangyingyoupin.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kvf.sjlbkw.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vqx.fanxiaobao.xyz

Ruby: s.match?(/\d+/)
来源：http://vqu.ydjk.org.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uxc.bjfxy.top

[I02] 提取所有匹配
来源：http://bfn.ywan-chungtsiang.top

Py:   re.findall(r"\d+", s)
来源：http://ewf.zhiwuduotai.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ldt.hfpthk.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ppc.yuanzhike.top


<!-- 参考信息 -->