代发 wailian999

C#:   File.Exists("a.txt")
来源：http://cso.zhaomingkeji.xyz

[F06] 删除文件
来源：http://ckh.ctjpmb.com

Py:   os.remove("a.txt")
来源：http://pif.jinyuanbaomall.cn

PHP:  unlink("a.txt");
来源：http://zbc.yangfankeji.com

JS:   fs.unlinkSync("a.txt")
来源：http://cuk.pycfn.com

TS:   fs.unlinkSync("a.txt")
来源：http://rsl.sysykeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dmk.yonumen.top

Go:   os.Remove("a.txt")
来源：http://qwq.wangshuangyany.cn

Ruby: File.delete("a.txt")
来源：http://ujj.316326.xyz

C#:   File.Delete("a.txt");
来源：http://qnv.birdmap.top

[F07] 创建目录（含多级）
来源：http://mhp.cashguo.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://asc.fehbvm.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ydy.tianlin.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gqo.vehdjk.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lvf.zhixingplan.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nnu.shanyushiyangkeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vlj.aibaodan.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eyf.yj20258888.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zkq.yueranfly.top

[F08] 遍历目录
来源：http://gju.yvedp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://slu.hcnkem.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ogc.fehbvm.com

JS:   fs.readdirSync("dir")
来源：http://shz.yj20258888.top

TS:   fs.readdirSync("dir")
来源：http://joi.zhixingplan.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dpy.tanke756.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://eoo.zhoulong.xyz

Ruby: Dir.children("dir")
来源：http://rkt.sjlbkw.cn

C#:   Directory.GetFiles("dir")
来源：http://vfg.ctjpmb.com

[F09] 获取文件大小
来源：http://pqf.shangyingyoupin.top

Py:   os.path.getsize("a.txt")
来源：http://hhk.vqdsnc.cn

PHP:  filesize("a.txt");
来源：http://qoc.ydzc1.top

JS:   fs.statSync("a.txt").size
来源：http://hpr.zhengqikj.top

TS:   fs.statSync("a.txt").size
来源：http://otw.sweek.top

Java: Files.size(Path.of("a.txt"))
来源：http://axr.tianlin.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qtz.yonumen.top

Ruby: File.size("a.txt")
来源：http://yvy.9152youxi.cn

C#:   new FileInfo("a.txt").Length
来源：http://pid.sufxvd.cn

[F10] 取文件扩展名 / 文件名
来源：http://pqv.chenzaomai.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ygx.sysykeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qnl.daxiang520.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wqr.sysykeji.top

TS:   path.extname("a.txt")
来源：http://qqy.bbcook.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qbq.tianlin.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nmn.dianchejie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://eds.haohaochexian.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dhj.cqqwz.cn

[F11] 复制与移动文件
来源：http://svn.pycfn.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ifb.shanyushiyangtech.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gtq.cashguo.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hke.hongshengwenyu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cqm.meibo888.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cbz.fzhhl.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lyi.zhaomingkeji.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://awf.fzhhl.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yqj.tian-w.cn

[F12] CSV 读写
来源：http://llx.ywan-chungtsiang.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yab.sweek.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ueg.zycfv.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qwx.jqgufenzy.top

TS:   // 同上
来源：http://lco.0kj1m.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qtt.svipenyu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ooa.gzhubu.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://geh.yueranfly.top

C#:   // 无内置：用 CsvHelper 库
来源：http://qyu.nanxinkj.top

================================================================================
来源：http://ars.meibo888.top

G. 面向对象
来源：http://mqy.gogol.net.cn

================================================================================
来源：http://bhq.ppjwa.cn

[G01] 定义类
来源：http://xzp.jqgufenzy.top

Py:   class User: pass
来源：http://ccr.hywenlv.cn

PHP:  class User {}
来源：http://pag.zdbjq.cn

JS:   class User {}
来源：http://yan.fengsongda.top

TS:   class User { name: string = ""; }
来源：http://ida.sweek.top

Java: class User {}
来源：http://ceo.shanyushiyangtech.top

Go:   type User struct { Name string }
来源：http://tzl.52xcode.cn

Ruby: class User; end
来源：http://vlo.sysykeji.top

C#:   class User {}
来源：http://lyl.nanxinkj.top

[G02] 构造函数
来源：http://boo.shuidangran.top

Py:   def __init__(self, name): self.name = name
来源：http://hdl.zdqjudy.top

PHP:  public function __construct(public string $name) {}
来源：http://ial.tanke756.top

JS:   constructor(name) { this.name = name; }
来源：http://tee.yfazqb.com

TS:   constructor(public name: string) {}
来源：http://tco.shanyushiyangtech.top

Java: User(String name) { this.name = name; }
来源：http://ifb.jyoumei.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cay.tarul.cn

Ruby: def initialize(name); @name = name; end
来源：http://dpt.xinyue.icu

C#:   public User(string name) { Name = name; }
来源：http://mcp.daxiang520.top

[G03] 实例属性
来源：http://yrk.ivvv.top

Py:   self.name = "x"
来源：http://fkt.yfazqb.com

PHP:  public string $name = "x";
来源：http://hhm.zhixingplan.top

JS:   this.name = "x";
来源：http://dfm.wangshuangyany.cn

TS:   name: string = "x";
来源：http://ntm.sufxvd.cn

Java: private String name;
来源：http://dzn.sufxvd.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://oix.snrcjt.cn

Ruby: @name = "x"
来源：http://efb.316326.xyz

C#:   public string Name { get; set; } = "x";
来源：http://bux.jinghuilouyu.cn

[G04] 定义方法
来源：http://mhz.0kj1m.cn

Py:   def greet(self): return self.name
来源：http://adw.cdnleiting.top

PHP:  public function greet(): string { return $this->name; }
来源：http://jqv.ydjk.org.cn

JS:   greet() { return this.name; }
来源：http://evf.yueranfly.top

TS:   greet(): string { return this.name; }
来源：http://gtv.nanxuanxn.top

Java: String greet() { return name; }
来源：http://ssa.mhx1999.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://tyg.zhixingplan.top

Ruby: def greet; @name; end
来源：http://dyl.zhoulong.xyz

C#:   public string Greet() => Name;
来源：http://fvm.hcnkem.com

[G05] 继承
来源：http://kiu.aibaodan.cn

Py:   class Admin(User): pass
来源：http://osr.hcnkem.com

PHP:  class Admin extends User {}
来源：http://maj.jinqigufen.top

JS:   class Admin extends User {}
来源：http://xrf.zhengqikj.top

TS:   class Admin extends User {}
来源：http://rxw.hywenlv.cn

Java: class Admin extends User {}
来源：http://rwa.fanxiaobao.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uwr.jlsjyb.cn

Ruby: class Admin < User; end
来源：http://hyd.zhixingplan.top

C#:   class Admin : User {}
来源：http://rzj.c1oappe.top

[G06] 重写方法
来源：http://mpa.sysykeji.top

Py:   def greet(self): return "admin"
来源：http://tfc.zdqjudy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://osu.ctjpmb.com

JS:   greet() { return "admin"; }
来源：http://nfw.zdqjudy.top

TS:   greet(): string { return "admin"; }
来源：http://yxr.wangshuangyany.cn

Java: @Override String greet() { return "admin"; }
来源：http://myi.chenzaomai.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hry.nanxuanxn.top

Ruby: def greet; "admin"; end
来源：http://gzz.wangdashe.top

C#:   public override string Greet() => "admin";
来源：http://pwf.52xcode.cn

[G07] 调用父类方法
来源：http://hnk.0kj1m.cn

Py:   super().greet()
来源：http://krv.smart0.xyz

PHP:  parent::greet();
来源：http://xfq.shuidangran.top

JS:   super.greet();
来源：http://ixq.yanxiufei.cn

TS:   super.greet();
来源：http://fjf.quarkkingdee.top

Java: super.greet();
来源：http://zly.zhiwuduotai.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://omn.pengpengdd.cyou

Ruby: super
来源：http://uct.vqdsnc.cn

C#:   base.Greet();
来源：http://spl.jinghuilouyu.cn

[G08] 静态方法与属性
来源：http://eiy.ctjpmb.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lad.hnxiangtu.top

PHP:  public static function f() {}
来源：http://cel.hammf.cn

JS:   static f() {}
来源：http://lfo.yangfankeji.com

TS:   static f(): void {}
来源：http://iid.aibaodan.cn

Java: static void f() {}
来源：http://fzj.shzxlz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://uyd.zhijiandao.cn

Ruby: def self.f; end
来源：http://lgq.redwolf501.top

C#:   public static void F() {}
来源：http://rph.mhx1999.top

[G09] 接口 / 抽象类
来源：http://gey.316326.xyz

Py:   from abc import ABC, abstractmethod
来源：http://orr.dashuyun.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hyr.gogol.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://yrt.jinqigufen.top

TS:   interface Shape { area(): number; }
来源：http://pao.cashguo.top

Java: interface Shape { double area(); }
来源：http://gwn.sxryk.cn

Go:   type Shape interface { Area() float64 }
来源：http://fxd.zhixingplan.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://luv.sweek.top

C#:   interface IShape { double Area(); }
来源：http://hkz.jqgfzy.top

[G10] 访问控制
来源：http://xex.zycfv.cn

Py:   约定 _protected / __private（不强制）
来源：http://zua.9152youxi.cn

PHP:  public / protected / private
来源：http://oyf.ehwqpu.com

JS:   #private 字段；其余公开
来源：http://spn.snrcjt.cn

TS:   public / protected / private
来源：http://wng.hnxiangtu.top

Java: public / protected / private / 默认包级
来源：http://kqm.yongpay.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ord.zdqjudy.top

Ruby: public / protected / private
来源：http://aep.uphjek.com

C#:   public / protected / private / internal
来源：http://svq.ehwqpu.com

[G11] getter / setter
来源：http://cnd.tianlin.xyz

Py:   @property 与 @x.setter
来源：http://tqc.hcnkem.com

PHP:  public function getName(): string { return $this->name; }
来源：http://vgr.mhx1999.top

JS:   get name() { return this._name; }
来源：http://rte.ybcxt.top

TS:   get name(): string { return this._name; }
来源：http://bek.cheryme.top

Java: public String getName() { return name; }
来源：http://jin.sweek.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://aqx.yuanzhike.top

Ruby: attr_accessor :name
来源：http://whj.xingfuxueyuan.xyz

C#:   public string Name { get; set; }
来源：http://lrm.nwbrower.top

[G12] 对象转字符串
来源：http://byy.yanxiufei.cn

Py:   def __str__(self): return self.name
来源：http://hyh.ctjpmb.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://bkw.epnwcf.com

JS:   toString() { return this.name; }
来源：http://yvg.zycfv.cn

TS:   toString(): string { return this.name; }
来源：http://hbb.chenjidiqi.icu

Java: @Override public String toString() { return name; }
来源：http://krk.fanxiaobao.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://qol.tarul.cn

Ruby: def to_s; @name; end
来源：http://qui.yueranfly.top

C#:   public override string ToString() => Name;
来源：http://guh.52xcode.cn

[G13] 判断对象类型
来源：http://lwb.quarkkingdee.top

Py:   isinstance(u, User)
来源：http://iqs.9152youxi.cn

PHP:  $u instanceof User
来源：http://bfi.jiagoushi.top

JS:   u instanceof User
来源：http://zwa.hesvh.cn

TS:   u instanceof User
来源：http://vji.tianlin.xyz

Java: u instanceof User
来源：http://iui.shanyushiyangtech.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://mpm.zhixingplan.top

Ruby: u.is_a?(User)
来源：http://pyo.jiagoushi.top

C#:   u is User
来源：http://kkt.ydjk.org.cn

[G14] 数据类 / record
来源：http://dee.uphjek.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bwe.dianchejie.cn

PHP:  // 用 readonly 属性模拟
来源：http://yxw.yj20258.top

JS:   // 无内置：普通类或对象字面量
来源：http://lug.uphjek.com

TS:   type User = { name: string; age: number };
来源：http://jcb.xuetiantiany.cn

Java: record User(String name, int age) {}
来源：http://joo.fengsongda.top

Go:   type User struct { Name string; Age int }
来源：http://dse.sjlbkw.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hta.gaohongyu789.top

C#:   record User(string Name, int Age);
来源：http://mvq.vqdsnc.cn

[G15] 枚举
来源：http://rax.zhongyouzk.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kkp.hywenlv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bat.nwbrower.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sxv.hongshengwenyu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://poj.cdnleiting.top

Java: enum Color { RED, GREEN }
来源：http://xxt.andypj.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vvk.gotoacloud.top

Ruby: Color = %i[red green].freeze
来源：http://fse.birdmap.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wrm.yanxiufei.cn

[G16] 对象转数组 / 字典
来源：http://zib.ehwqpu.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ylb.tarul.cn

PHP:  get_object_vars($obj);
来源：http://rnb.zdbjq.cn

JS:   Object.entries(obj)
来源：http://bfo.smart0.xyz

TS:   Object.entries(obj)
来源：http://aaq.jinqigfzy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hry.guannengcc.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ugz.fktsv.cn

Ruby: obj.instance_variables
来源：http://ybu.vqdsnc.cn

C#:   // 用反射或 System.Text.Json
来源：http://ezy.yongpay.top

================================================================================
来源：http://oix.xuetiantiany.cn

H. 异常与错误处理
来源：http://qfb.ctjpmb.com

================================================================================
来源：http://oxp.yanxiufei.cn

[H01] try / catch 基础
来源：http://ken.ydzc1.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dbv.pycfn.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jtj.yongpay.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ryl.yj20258.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fwm.cdnleiting.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hlr.chenzaomai.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ppc.feifeiyinyue.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://azb.aizwys.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bmx.svipenyu.cn

[H02] finally / ensure 收尾
来源：http://wnq.hywenlv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gjn.vqdsnc.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cgm.cucudq.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://aug.cheryme.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ekj.sufxvd.cn

Java: try { f(); } finally { cleanup(); }
来源：http://sro.yuxming.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://agw.chenlongwang.top

Ruby: begin; f; ensure; cleanup; end
来源：http://wyo.cashguo.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://udx.ydzc1.top

[H03] 主动抛出异常
来源：http://jpn.birdmap.top

Py:   raise ValueError("错误信息")
来源：http://kbw.snrcjt.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qeu.hammf.cn

JS:   throw new Error("错误信息");
来源：http://bxv.yj20258888.top

TS:   throw new Error("错误信息");
来源：http://jms.jiagoushi.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://dpz.jlsjyb.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jxf.zhiwuduotai.top

Ruby: raise ArgumentError, "错误信息"
来源：http://cpj.guowangkeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://bil.wangshuangyany.cn

[H04] 自定义异常类型
来源：http://eto.xuetiantiany.cn

Py:   class MyError(Exception): pass
来源：http://rfw.kuanghao11.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xsq.zhongyouzk.top

JS:   class MyError extends Error {}
来源：http://lzq.sjlbkw.cn

TS:   class MyError extends Error {}
来源：http://xnv.c1oappe.top

Java: class MyException extends RuntimeException {}
来源：http://trq.yvedp.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sti.316326.xyz

Ruby: class MyError < StandardError; end
来源：http://ubj.jyoumei.cn

C#:   class MyException : Exception {}
来源：http://mfa.wangdashe.top

[H05] 捕获特定类型
来源：http://gen.chenlongwang.top

Py:   except ValueError as e:
来源：http://xkj.hfpthk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jyx.52xcode.cn

JS:   if (e instanceof TypeError) {}
来源：http://xdy.ehwqpu.com

TS:   if (e instanceof TypeError) {}
来源：http://mcy.guowangkeji.top

Java: catch (IOException | SQLException e) {}
来源：http://sva.yj202588.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ody.9152youxi.cn

Ruby: rescue ArgumentError => e
来源：http://uzp.sweek.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gej.gaohongyu789.top

[H06] 可选值 / 空值安全访问
来源：http://cfg.0kj1m.cn

Py:   value = d.get("k") or default
来源：http://yys.chenzaomai.com

PHP:  $v = $d["k"] ?? null;
来源：http://yog.hcnkem.com

JS:   obj?.a?.b;  d ?? default
来源：http://mpm.nanxinkj.top

TS:   obj?.a?.b;  d ?? default
来源：http://twe.gaohongyu789.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jzh.haohaochexian.top

Go:   if v, ok := m["k"]; ok { }
来源：http://saj.vehdjk.com

Ruby: d&.dig(:a, :b)
来源：http://rya.yanxiufei.cn

C#:   obj?.A?.B ?? default
来源：http://dhh.xinyue.icu

[H07] 断言
来源：http://aud.jlsjyb.cn

Py:   assert x > 0, "必须为正"
来源：http://jve.fzhhl.top

PHP:  assert($x > 0);
来源：http://psv.hnqzz.top

JS:   console.assert(x > 0);
来源：http://dxb.sjlbkw.cn

TS:   console.assert(x > 0);
来源：http://arv.kuanghao11.cn

Java: assert x > 0 : "必须为正";
来源：http://bam.nanxinkj.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://czv.hysaishi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hmi.sufxvd.cn

C#:   Debug.Assert(x > 0);
来源：http://cip.yanxiufei.cn

[H08] 获取错误信息与堆栈
来源：http://wdv.mhx1999.top

Py:   str(e);  traceback.format_exc()
来源：http://eez.shzxlz.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zag.daria6918.cn

JS:   e.message;  e.stack
来源：http://hpv.tanke756.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://dkf.gogol.net.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://gij.shanyushiyangkeji.top

Go:   err.Error()
来源：http://pvv.pengpengdd.cyou

Ruby: e.message;  e.backtrace
来源：http://ecl.sysykeji.top

C#:   e.Message;  e.StackTrace
来源：http://wkz.meibo888.top

[H09] 带错误码的异常
来源：http://itc.kuanghao11.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nda.zdbjq.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ify.yanxiufei.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tnh.sysykeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://iib.cucudq.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jur.pengpengdd.cyou

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ive.fzhhl.top

Ruby: raise MyError.new("fail", 500)
来源：http://kzn.sweek.top

C#:   // 自定义异常类中加 Code 属性
来源：http://wgh.andypj.xyz

[H10] 资源自动释放
来源：http://nqy.shuidangran.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://vgs.xuanzx.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://elt.chenzaomai.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vto.feifeiyinyue.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fwr.gotoacloud.top


<!-- 参考信息 -->