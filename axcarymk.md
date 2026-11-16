代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rqv.vehdjk.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ggr.hysaishi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://myp.jinqigfzy.top

[F08] 遍历目录
来源：http://xvq.guannengcc.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://qev.fzhhl.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blk.yj20258.top

JS:   fs.readdirSync("dir")
来源：http://sbl.chenjidiqi.icu

TS:   fs.readdirSync("dir")
来源：http://ske.zhongyouzk.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dog.bjfxy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://yhv.jiagoushi.top

Ruby: Dir.children("dir")
来源：http://nve.nanxuanxn.top

C#:   Directory.GetFiles("dir")
来源：http://joa.andypj.xyz

[F09] 获取文件大小
来源：http://wtb.yj20258888.top

Py:   os.path.getsize("a.txt")
来源：http://sur.tianlin.xyz

PHP:  filesize("a.txt");
来源：http://scx.wangshuangyany.cn

JS:   fs.statSync("a.txt").size
来源：http://gdx.zhiwuduotai.top

TS:   fs.statSync("a.txt").size
来源：http://gcs.ybcxt.top

Java: Files.size(Path.of("a.txt"))
来源：http://fhu.xylfe.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wws.guannengcc.top

Ruby: File.size("a.txt")
来源：http://jcx.havefunace.top

C#:   new FileInfo("a.txt").Length
来源：http://eby.shanyushiyangkeji.top

[F10] 取文件扩展名 / 文件名
来源：http://jrr.shangyingyoupin.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wmh.dashuyun.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rvp.jqgfzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qxs.cashguo.top

TS:   path.extname("a.txt")
来源：http://wtv.ehwqpu.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jud.zhijiandao.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kos.c1oappe.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://aps.zhongyouzk.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mjo.fanxiaobao.xyz

[F11] 复制与移动文件
来源：http://btd.yangfankeji.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wzk.ybcxt.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sle.nwbrower.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xfr.uphjek.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ilp.c1oappe.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zef.ybcxt.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mav.c1oappe.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ryy.vqdsnc.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://goa.aibaodan.cn

[F12] CSV 读写
来源：http://uqo.sweek.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sqv.yanxiufei.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lnd.pengpengdd.cyou

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://eqf.pengpengdd.cyou

TS:   // 同上
来源：http://orb.cqqwz.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tlo.dianchejie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xrz.guannengcc.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wux.nanxinkj.top

C#:   // 无内置：用 CsvHelper 库
来源：http://gih.pycfn.com

================================================================================
来源：http://ohq.yj20258.top

G. 面向对象
来源：http://mhg.hnxiangtu.top

================================================================================
来源：http://vlg.dianchejie.cn

[G01] 定义类
来源：http://cev.tianlin.xyz

Py:   class User: pass
来源：http://uxl.ppjwa.cn

PHP:  class User {}
来源：http://ytm.chenjidiqi.icu

JS:   class User {}
来源：http://cnj.svipenyu.cn

TS:   class User { name: string = ""; }
来源：http://umo.zycfv.cn

Java: class User {}
来源：http://fla.yueranfly.top

Go:   type User struct { Name string }
来源：http://vpx.ydjk.org.cn

Ruby: class User; end
来源：http://glg.yj20258888.top

C#:   class User {}
来源：http://tpy.hesvh.cn

[G02] 构造函数
来源：http://uvh.feifeiyinyue.top

Py:   def __init__(self, name): self.name = name
来源：http://fwl.yangfankeji.com

PHP:  public function __construct(public string $name) {}
来源：http://sfg.iojbl.cn

JS:   constructor(name) { this.name = name; }
来源：http://kbg.jinqigufen.top

TS:   constructor(public name: string) {}
来源：http://ufe.jinyuanbaomall.cn

Java: User(String name) { this.name = name; }
来源：http://zel.sjlbkw.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pgc.mhx1999.top

Ruby: def initialize(name); @name = name; end
来源：http://tqq.kuanghao11.cn

C#:   public User(string name) { Name = name; }
来源：http://vyh.hfpthk.cn

[G03] 实例属性
来源：http://fuz.dianchejie.cn

Py:   self.name = "x"
来源：http://nwz.vqdsnc.cn

PHP:  public string $name = "x";
来源：http://laf.vqdsnc.cn

JS:   this.name = "x";
来源：http://fdf.guowangkeji.top

TS:   name: string = "x";
来源：http://hlo.sweek.top

Java: private String name;
来源：http://myv.redwolf501.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kmg.yuanzhike.top

Ruby: @name = "x"
来源：http://wkg.ehwqpu.com

C#:   public string Name { get; set; } = "x";
来源：http://piv.daxiang520.top

[G04] 定义方法
来源：http://llv.hongshengwenyu.top

Py:   def greet(self): return self.name
来源：http://pqt.hnqzz.top

PHP:  public function greet(): string { return $this->name; }
来源：http://xni.zycfv.cn

JS:   greet() { return this.name; }
来源：http://obq.fanxiaobao.xyz

TS:   greet(): string { return this.name; }
来源：http://jhd.ydjk.org.cn

Java: String greet() { return name; }
来源：http://dxq.epnwcf.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://dgf.316326.xyz

Ruby: def greet; @name; end
来源：http://oww.sweek.top

C#:   public string Greet() => Name;
来源：http://sib.pengpengdd.cyou

[G05] 继承
来源：http://aeo.sweek.top

Py:   class Admin(User): pass
来源：http://inf.svipenyu.cn

PHP:  class Admin extends User {}
来源：http://lpb.gotoacloud.top

JS:   class Admin extends User {}
来源：http://jox.tanke756.top

TS:   class Admin extends User {}
来源：http://oxo.52xcode.cn

Java: class Admin extends User {}
来源：http://gnc.zhoulong.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://scz.tianlin.xyz

Ruby: class Admin < User; end
来源：http://dju.yongpay.top

C#:   class Admin : User {}
来源：http://tsw.yfazqb.com

[G06] 重写方法
来源：http://ghb.gogol.net.cn

Py:   def greet(self): return "admin"
来源：http://rjl.jlsjyb.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://urt.jianghu66.top

JS:   greet() { return "admin"; }
来源：http://sxb.shzxlz.cn

TS:   greet(): string { return "admin"; }
来源：http://npk.zhengqikj.top

Java: @Override String greet() { return "admin"; }
来源：http://aqn.jiagoushi.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tlk.zhengqikj.top

Ruby: def greet; "admin"; end
来源：http://idg.yanxiufei.cn

C#:   public override string Greet() => "admin";
来源：http://wey.quarkkingdee.top

[G07] 调用父类方法
来源：http://acx.aizwys.cn

Py:   super().greet()
来源：http://pja.gzhubu.top

PHP:  parent::greet();
来源：http://joc.fzhhl.top

JS:   super.greet();
来源：http://ujp.ppjwa.cn

TS:   super.greet();
来源：http://gjy.zdqjudy.top

Java: super.greet();
来源：http://swr.aibaodan.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ehz.jlsjyb.cn

Ruby: super
来源：http://etu.yangfankeji.com

C#:   base.Greet();
来源：http://hxu.bjfxy.top

[G08] 静态方法与属性
来源：http://wba.yfazqb.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wnc.jinqigufen.top

PHP:  public static function f() {}
来源：http://ewu.uphjek.com

JS:   static f() {}
来源：http://jpt.jqgufenzy.top

TS:   static f(): void {}
来源：http://gjy.ydzc1.top

Java: static void f() {}
来源：http://ezn.yuanzhike.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://lsw.mhx1999.top

Ruby: def self.f; end
来源：http://rdc.jlsjyb.cn

C#:   public static void F() {}
来源：http://tlg.wangdashe.top

[G09] 接口 / 抽象类
来源：http://qwn.wangshuangyany.cn

Py:   from abc import ABC, abstractmethod
来源：http://mah.gaohongyu789.top

PHP:  interface Shape { public function area(): float; }
来源：http://fof.dianchejie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bdr.fzhhl.top

TS:   interface Shape { area(): number; }
来源：http://qsb.vehdjk.com

Java: interface Shape { double area(); }
来源：http://ops.sysykeji.top

Go:   type Shape interface { Area() float64 }
来源：http://xdr.ydzc1.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://amg.c1oappe.top

C#:   interface IShape { double Area(); }
来源：http://lcu.shzxlz.cn

[G10] 访问控制
来源：http://gph.chenlongwang.top

Py:   约定 _protected / __private（不强制）
来源：http://wtk.yj202588.top

PHP:  public / protected / private
来源：http://sqj.tarul.cn

JS:   #private 字段；其余公开
来源：http://hrd.havefunace.top

TS:   public / protected / private
来源：http://xpo.tian-w.cn

Java: public / protected / private / 默认包级
来源：http://mxx.tian-w.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lrt.shanyushiyangkeji.top

Ruby: public / protected / private
来源：http://ekz.yj20258.top

C#:   public / protected / private / internal
来源：http://lwl.shangyingyoupin.top

[G11] getter / setter
来源：http://ntc.yuxming.cn

Py:   @property 与 @x.setter
来源：http://tlc.zycfv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://rbh.xuanzx.com

JS:   get name() { return this._name; }
来源：http://hlh.snrcjt.cn

TS:   get name(): string { return this._name; }
来源：http://rzg.meibo888.top

Java: public String getName() { return name; }
来源：http://gvz.shanyushiyangkeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ijh.zhongyouzk.top

Ruby: attr_accessor :name
来源：http://odw.xziqi.cn

C#:   public string Name { get; set; }
来源：http://rkr.fktsv.cn

[G12] 对象转字符串
来源：http://stm.vehdjk.com

Py:   def __str__(self): return self.name
来源：http://wrc.yuanzhike.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://vne.hongshengwenyu.top

JS:   toString() { return this.name; }
来源：http://wpx.c1oappe.top

TS:   toString(): string { return this.name; }
来源：http://sjq.yj20258888.top

Java: @Override public String toString() { return name; }
来源：http://bxd.zdbjq.cn

Go:   func (u User) String() string { return u.Name }
来源：http://myq.bjfxy.top

Ruby: def to_s; @name; end
来源：http://xfs.zhiwuduotai.top

C#:   public override string ToString() => Name;
来源：http://bce.shuidangran.top

[G13] 判断对象类型
来源：http://fxo.gaohongyu789.top

Py:   isinstance(u, User)
来源：http://lhs.feifeiyinyue.top

PHP:  $u instanceof User
来源：http://jzb.havefunace.top

JS:   u instanceof User
来源：http://buc.iojbl.cn

TS:   u instanceof User
来源：http://urr.tanke756.top

Java: u instanceof User
来源：http://kaf.wangshuangyany.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sgk.gogol.net.cn

Ruby: u.is_a?(User)
来源：http://fog.birdmap.top

C#:   u is User
来源：http://tfh.yongpay.top

[G14] 数据类 / record
来源：http://drb.ybcxt.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rju.kuanghao11.cn

PHP:  // 用 readonly 属性模拟
来源：http://jle.birdmap.top

JS:   // 无内置：普通类或对象字面量
来源：http://zbe.hysaishi.cn

TS:   type User = { name: string; age: number };
来源：http://mjt.chenlongwang.top

Java: record User(String name, int age) {}
来源：http://lwi.gogol.net.cn

Go:   type User struct { Name string; Age int }
来源：http://zxh.9152youxi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nnr.aizwys.cn

C#:   record User(string Name, int Age);
来源：http://alm.sweek.top

[G15] 枚举
来源：http://gdr.jyoumei.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://had.yuxming.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://khu.ydjk.org.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://edm.feifeiyinyue.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ysb.yuxming.cn

Java: enum Color { RED, GREEN }
来源：http://rlo.xylfe.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vhe.0kj1m.cn

Ruby: Color = %i[red green].freeze
来源：http://cac.ehwqpu.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mch.shanyushiyangtech.top

[G16] 对象转数组 / 字典
来源：http://jxf.gzhubu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://imt.vqdsnc.cn

PHP:  get_object_vars($obj);
来源：http://kzk.c1oappe.top

JS:   Object.entries(obj)
来源：http://rur.sufxvd.cn

TS:   Object.entries(obj)
来源：http://dqk.yueranfly.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uwk.yfazqb.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://ejk.zhijiandao.cn

Ruby: obj.instance_variables
来源：http://yjq.ybcxt.top

C#:   // 用反射或 System.Text.Json
来源：http://owh.hongshengwenyu.top

================================================================================
来源：http://eam.hnxiangtu.top

H. 异常与错误处理
来源：http://any.sysykeji.top

================================================================================
来源：http://ele.jinqigfzy.top

[H01] try / catch 基础
来源：http://upj.sxryk.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ovn.yvedp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pkq.zhongyouzk.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://puz.ctjpmb.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ybf.yongpay.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fla.bjfxy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xsx.jyoumei.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kik.jiagoushi.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vhb.ivvv.top

[H02] finally / ensure 收尾
来源：http://bzn.dashuyun.cn

Py:   try: f()⏎finally: cleanup()
来源：http://fvp.bbcook.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lea.uphjek.com

JS:   try { f(); } finally { cleanup(); }
来源：http://opy.gogol.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://btc.shangyingyoupin.top

Java: try { f(); } finally { cleanup(); }
来源：http://azz.gaohongyu789.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://aoc.shangyingyoupin.top

Ruby: begin; f; ensure; cleanup; end
来源：http://dkt.cucudq.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://oyx.gaohongyu789.top

[H03] 主动抛出异常
来源：http://pmz.xuanzx.com

Py:   raise ValueError("错误信息")
来源：http://ylh.birdmap.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ccm.ctjpmb.com

JS:   throw new Error("错误信息");
来源：http://mga.xziqi.cn

TS:   throw new Error("错误信息");
来源：http://jze.fanxiaobao.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://nyr.sweek.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cgr.uphjek.com

Ruby: raise ArgumentError, "错误信息"
来源：http://zyn.nanxuanxn.top

C#:   throw new ArgumentException("错误信息");
来源：http://dfu.jlsjyb.cn

[H04] 自定义异常类型
来源：http://wfi.dashuyun.cn

Py:   class MyError(Exception): pass
来源：http://rfl.chenlongwang.top

PHP:  class MyError extends RuntimeException {}
来源：http://nod.aizwys.cn

JS:   class MyError extends Error {}
来源：http://ium.pengpengdd.cyou

TS:   class MyError extends Error {}
来源：http://ajz.aizwys.cn

Java: class MyException extends RuntimeException {}
来源：http://ykq.xylfe.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ref.andypj.xyz

Ruby: class MyError < StandardError; end
来源：http://cmj.zhixingplan.top

C#:   class MyException : Exception {}
来源：http://nax.yueranfly.top

[H05] 捕获特定类型
来源：http://zdf.hfpthk.cn

Py:   except ValueError as e:
来源：http://btq.cdnleiting.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ghw.svipenyu.cn

JS:   if (e instanceof TypeError) {}
来源：http://qpu.dianchejie.cn

TS:   if (e instanceof TypeError) {}
来源：http://wpt.cqqwz.cn

Java: catch (IOException | SQLException e) {}
来源：http://vuj.fanxiaobao.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uwa.jinqigufen.top

Ruby: rescue ArgumentError => e
来源：http://uix.zhengqikj.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://etv.svipenyu.cn

[H06] 可选值 / 空值安全访问
来源：http://zxx.sxryk.cn

Py:   value = d.get("k") or default
来源：http://gjq.ppjwa.cn

PHP:  $v = $d["k"] ?? null;
来源：http://hgy.sxryk.cn

JS:   obj?.a?.b;  d ?? default
来源：http://cbs.dianchejie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://msw.cqqwz.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://alz.chenzaomai.com

Go:   if v, ok := m["k"]; ok { }
来源：http://qup.yfazqb.com

Ruby: d&.dig(:a, :b)
来源：http://zey.pengpengdd.cyou

C#:   obj?.A?.B ?? default
来源：http://lew.fengsongda.top

[H07] 断言
来源：http://zkp.pycfn.com

Py:   assert x > 0, "必须为正"
来源：http://tth.yvedp.cn

PHP:  assert($x > 0);
来源：http://xbv.cucudq.cn

JS:   console.assert(x > 0);
来源：http://lqa.ctjpmb.com

TS:   console.assert(x > 0);
来源：http://ttj.jyoumei.cn

Java: assert x > 0 : "必须为正";
来源：http://chm.hnxiangtu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dii.zhiwuduotai.top

Ruby: raise "必须为正" unless x > 0
来源：http://anm.cucudq.cn

C#:   Debug.Assert(x > 0);
来源：http://cmh.yuanzhike.top

[H08] 获取错误信息与堆栈
来源：http://crk.sjlbkw.cn

Py:   str(e);  traceback.format_exc()
来源：http://dzg.cheryme.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rdp.feifeiyinyue.top

JS:   e.message;  e.stack
来源：http://gjd.xziqi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ygz.xingfuxueyuan.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://xbx.ybcxt.top

Go:   err.Error()
来源：http://emk.dashuyun.cn

Ruby: e.message;  e.backtrace
来源：http://xdd.sufxvd.cn

C#:   e.Message;  e.StackTrace
来源：http://sxc.yvedp.cn

[H09] 带错误码的异常
来源：http://zfw.shanyushiyangkeji.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://iep.zhongyouzk.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://hdk.zycfv.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ptf.sweek.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://upb.kuanghao11.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xry.epnwcf.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://itm.birdmap.top

Ruby: raise MyError.new("fail", 500)
来源：http://ftw.quarkkingdee.top

C#:   // 自定义异常类中加 Code 属性
来源：http://hvr.quarkkingdee.top

[H10] 资源自动释放
来源：http://hdj.jiagoushi.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://yfu.jianghu66.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yke.hongshengwenyu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://woa.ydjk.org.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lnq.gzhubu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xro.chenlongwang.top

Go:   defer f.Close()
来源：http://yds.xziqi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ijq.hesvh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qlk.ivvv.top

================================================================================
来源：http://mcg.cdnleiting.top

I. 正则表达式
来源：http://kyq.wangshuangyany.cn

================================================================================
来源：http://ihf.sysykeji.top

[I01] 判断是否匹配
来源：http://bpl.hfpthk.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://spi.gaohongyu789.top

PHP:  preg_match('/\d+/', $s);
来源：http://dis.fehbvm.com

JS:   /\d+/.test(s)
来源：http://fws.0kj1m.cn

TS:   /\d+/.test(s)
来源：http://rzv.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tfw.shangyingyoupin.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://myv.guowangkeji.top

Ruby: s.match?(/\d+/)
来源：http://twd.hfpthk.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rqa.xingfuxueyuan.xyz


<!-- 参考信息 -->