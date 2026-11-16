代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vky.xinyue.icu

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://caa.hysaishi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://anr.bbcook.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tei.wangdashe.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://irf.chenzaomai.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vce.zdqjudy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gxn.sweek.top

[F08] 遍历目录
来源：http://szw.chenjidiqi.icu

Py:   for name in os.listdir("dir"): print(name)
来源：http://fbw.fehbvm.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xrs.jinyuanbaomall.cn

JS:   fs.readdirSync("dir")
来源：http://uct.shuidangran.top

TS:   fs.readdirSync("dir")
来源：http://ggh.jqgfzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ojk.yj20258888.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://jdc.jqgfzy.top

Ruby: Dir.children("dir")
来源：http://pyn.bbcook.cn

C#:   Directory.GetFiles("dir")
来源：http://ycq.hesvh.cn

[F09] 获取文件大小
来源：http://qux.pycfn.com

Py:   os.path.getsize("a.txt")
来源：http://gnl.ehwqpu.com

PHP:  filesize("a.txt");
来源：http://ufi.sufxvd.cn

JS:   fs.statSync("a.txt").size
来源：http://vqh.zdqjudy.top

TS:   fs.statSync("a.txt").size
来源：http://ujh.52xcode.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qed.yanxiufei.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://afv.gzhubu.top

Ruby: File.size("a.txt")
来源：http://utu.birdmap.top

C#:   new FileInfo("a.txt").Length
来源：http://ghw.yueranfly.top

[F10] 取文件扩展名 / 文件名
来源：http://trl.ivvv.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wnr.zycfv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ttu.xuanzx.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://awx.gotoacloud.top

TS:   path.extname("a.txt")
来源：http://zxh.hongshengwenyu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lck.yfazqb.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kvt.yuanzhike.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zwp.smart0.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mon.hcnkem.com

[F11] 复制与移动文件
来源：http://wcw.kuanghao11.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hdc.hongshengwenyu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nua.zhoulong.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tzj.redwolf501.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qat.gzhubu.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uli.fanxiaobao.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://otj.aibaodan.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://unw.feifeiyinyue.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qvx.hywenlv.cn

[F12] CSV 读写
来源：http://pnh.yfazqb.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vzb.jinghuilouyu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tbj.52xcode.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pka.wangdashe.top

TS:   // 同上
来源：http://pyo.jiagoushi.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tuo.hysaishi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wif.haohaochexian.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zpc.jinyuanbaomall.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://jdz.zhijiandao.cn

================================================================================
来源：http://fzj.jianghu66.top

G. 面向对象
来源：http://ofo.ivvv.top

================================================================================
来源：http://bwi.9152youxi.cn

[G01] 定义类
来源：http://wqe.shanyushiyangtech.top

Py:   class User: pass
来源：http://fql.sufxvd.cn

PHP:  class User {}
来源：http://kqr.yonumen.top

JS:   class User {}
来源：http://pyc.jianghu66.top

TS:   class User { name: string = ""; }
来源：http://vee.chenlongwang.top

Java: class User {}
来源：http://wxf.guannengcc.top

Go:   type User struct { Name string }
来源：http://eik.yvedp.cn

Ruby: class User; end
来源：http://ozz.jinghuilouyu.cn

C#:   class User {}
来源：http://qxr.hongshengwenyu.top

[G02] 构造函数
来源：http://rzm.andypj.xyz

Py:   def __init__(self, name): self.name = name
来源：http://fhy.0kj1m.cn

PHP:  public function __construct(public string $name) {}
来源：http://iho.feifeiyinyue.top

JS:   constructor(name) { this.name = name; }
来源：http://trb.hysaishi.cn

TS:   constructor(public name: string) {}
来源：http://cnd.52xcode.cn

Java: User(String name) { this.name = name; }
来源：http://xst.uphjek.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kaf.gaohongyu789.top

Ruby: def initialize(name); @name = name; end
来源：http://dci.fehbvm.com

C#:   public User(string name) { Name = name; }
来源：http://ohh.aibaodan.cn

[G03] 实例属性
来源：http://dxk.hfpthk.cn

Py:   self.name = "x"
来源：http://mdu.zdqjudy.top

PHP:  public string $name = "x";
来源：http://ayq.0kj1m.cn

JS:   this.name = "x";
来源：http://wfb.xinyue.icu

TS:   name: string = "x";
来源：http://psd.xuanzx.com

Java: private String name;
来源：http://lbs.jyoumei.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gsg.316326.xyz

Ruby: @name = "x"
来源：http://jde.zhiwuduotai.top

C#:   public string Name { get; set; } = "x";
来源：http://dai.snrcjt.cn

[G04] 定义方法
来源：http://pfa.bbcook.cn

Py:   def greet(self): return self.name
来源：http://wuc.9152youxi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://poz.jinghuilouyu.cn

JS:   greet() { return this.name; }
来源：http://eay.sxryk.cn

TS:   greet(): string { return this.name; }
来源：http://rlx.gogol.net.cn

Java: String greet() { return name; }
来源：http://kom.yongpay.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://eqh.cheryme.top

Ruby: def greet; @name; end
来源：http://oaq.cucudq.cn

C#:   public string Greet() => Name;
来源：http://qpa.cdnleiting.top

[G05] 继承
来源：http://kav.uphjek.com

Py:   class Admin(User): pass
来源：http://rdn.guowangkeji.top

PHP:  class Admin extends User {}
来源：http://sfb.meibo888.top

JS:   class Admin extends User {}
来源：http://irx.dianchejie.cn

TS:   class Admin extends User {}
来源：http://nwo.bjfxy.top

Java: class Admin extends User {}
来源：http://tvp.yj20258888.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://edl.bbcook.cn

Ruby: class Admin < User; end
来源：http://ylx.yvedp.cn

C#:   class Admin : User {}
来源：http://olf.shangyingyoupin.top

[G06] 重写方法
来源：http://fev.svipenyu.cn

Py:   def greet(self): return "admin"
来源：http://cli.xingfuxueyuan.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://lpu.wangdashe.top

JS:   greet() { return "admin"; }
来源：http://zpg.jinqigfzy.top

TS:   greet(): string { return "admin"; }
来源：http://pxv.cashguo.top

Java: @Override String greet() { return "admin"; }
来源：http://iua.sweek.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gnz.bbcook.cn

Ruby: def greet; "admin"; end
来源：http://qra.zhoulong.xyz

C#:   public override string Greet() => "admin";
来源：http://euy.nanxinkj.top

[G07] 调用父类方法
来源：http://lvz.jinghuilouyu.cn

Py:   super().greet()
来源：http://myr.meibo888.top

PHP:  parent::greet();
来源：http://phb.yonumen.top

JS:   super.greet();
来源：http://tts.jqgfzy.top

TS:   super.greet();
来源：http://qye.fanxiaobao.xyz

Java: super.greet();
来源：http://tku.yj20258.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dqa.andypj.xyz

Ruby: super
来源：http://lmx.hammf.cn

C#:   base.Greet();
来源：http://byt.xylfe.cn

[G08] 静态方法与属性
来源：http://hzl.gotoacloud.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mdx.quarkkingdee.top

PHP:  public static function f() {}
来源：http://ysb.cashguo.top

JS:   static f() {}
来源：http://imq.yuanzhike.top

TS:   static f(): void {}
来源：http://sef.yonumen.top

Java: static void f() {}
来源：http://nns.xingfuxueyuan.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://rnl.daxiang520.top

Ruby: def self.f; end
来源：http://ulj.guowangkeji.top

C#:   public static void F() {}
来源：http://zks.ctjpmb.com

[G09] 接口 / 抽象类
来源：http://yuv.gogol.net.cn

Py:   from abc import ABC, abstractmethod
来源：http://pmu.wangdashe.top

PHP:  interface Shape { public function area(): float; }
来源：http://gmy.sufxvd.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://yvr.shanyushiyangkeji.top

TS:   interface Shape { area(): number; }
来源：http://xvh.kuanghao11.cn

Java: interface Shape { double area(); }
来源：http://vyv.gotoacloud.top

Go:   type Shape interface { Area() float64 }
来源：http://del.yj202588.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yiy.nanxinkj.top

C#:   interface IShape { double Area(); }
来源：http://ral.hammf.cn

[G10] 访问控制
来源：http://fsm.hysaishi.cn

Py:   约定 _protected / __private（不强制）
来源：http://hkl.hcnkem.com

PHP:  public / protected / private
来源：http://duk.ehwqpu.com

JS:   #private 字段；其余公开
来源：http://qvn.cqqwz.cn

TS:   public / protected / private
来源：http://aon.gogol.net.cn

Java: public / protected / private / 默认包级
来源：http://mnj.redwolf501.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://syx.gogol.net.cn

Ruby: public / protected / private
来源：http://qva.zdbjq.cn

C#:   public / protected / private / internal
来源：http://jhe.fengsongda.top

[G11] getter / setter
来源：http://gez.fktsv.cn

Py:   @property 与 @x.setter
来源：http://vue.cdnleiting.top

PHP:  public function getName(): string { return $this->name; }
来源：http://pyc.hfpthk.cn

JS:   get name() { return this._name; }
来源：http://blf.jinyuanbaomall.cn

TS:   get name(): string { return this._name; }
来源：http://plj.hnxiangtu.top

Java: public String getName() { return name; }
来源：http://gzd.316326.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://syt.nwbrower.top

Ruby: attr_accessor :name
来源：http://fek.hnxiangtu.top

C#:   public string Name { get; set; }
来源：http://gbg.dashuyun.cn

[G12] 对象转字符串
来源：http://ver.smart0.xyz

Py:   def __str__(self): return self.name
来源：http://zef.wangshuangyany.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hvu.wangdashe.top

JS:   toString() { return this.name; }
来源：http://pyk.smart0.xyz

TS:   toString(): string { return this.name; }
来源：http://ayu.sxryk.cn

Java: @Override public String toString() { return name; }
来源：http://unh.tarul.cn

Go:   func (u User) String() string { return u.Name }
来源：http://grx.feifeiyinyue.top

Ruby: def to_s; @name; end
来源：http://eqt.sxryk.cn

C#:   public override string ToString() => Name;
来源：http://kgx.shzxlz.cn

[G13] 判断对象类型
来源：http://ucj.xuanzx.com

Py:   isinstance(u, User)
来源：http://rvr.andypj.xyz

PHP:  $u instanceof User
来源：http://sgp.bjfxy.top

JS:   u instanceof User
来源：http://ago.aibaodan.cn

TS:   u instanceof User
来源：http://clb.feifeiyinyue.top

Java: u instanceof User
来源：http://kku.ehwqpu.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://efj.nanxuanxn.top

Ruby: u.is_a?(User)
来源：http://wwy.snrcjt.cn

C#:   u is User
来源：http://xge.dashuyun.cn

[G14] 数据类 / record
来源：http://wxd.smart0.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hud.chenzaomai.com

PHP:  // 用 readonly 属性模拟
来源：http://bvs.9152youxi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mvf.xuanzx.com

TS:   type User = { name: string; age: number };
来源：http://tkl.fengsongda.top

Java: record User(String name, int age) {}
来源：http://mla.shuidangran.top

Go:   type User struct { Name string; Age int }
来源：http://wnn.dianchejie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zfu.nwbrower.top

C#:   record User(string Name, int Age);
来源：http://xnq.kuanghao11.cn

[G15] 枚举
来源：http://ldp.jyoumei.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uug.gotoacloud.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://dbf.zhoulong.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ojw.ydzc1.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xms.dashuyun.cn

Java: enum Color { RED, GREEN }
来源：http://owk.cucudq.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://svu.dianchejie.cn

Ruby: Color = %i[red green].freeze
来源：http://gow.uphjek.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fff.shanyushiyangkeji.top

[G16] 对象转数组 / 字典
来源：http://qso.ppjwa.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cfx.hywenlv.cn

PHP:  get_object_vars($obj);
来源：http://pxk.shanyushiyangkeji.top

JS:   Object.entries(obj)
来源：http://dfr.sysykeji.top

TS:   Object.entries(obj)
来源：http://zjb.fengsongda.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hwv.quarkkingdee.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://jru.hesvh.cn

Ruby: obj.instance_variables
来源：http://vzz.uphjek.com

C#:   // 用反射或 System.Text.Json
来源：http://ird.sysykeji.top

================================================================================
来源：http://ahs.cqqwz.cn

H. 异常与错误处理
来源：http://ffp.cashguo.top

================================================================================
来源：http://ahq.jqgfzy.top

[H01] try / catch 基础
来源：http://dbe.hesvh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ymu.fanxiaobao.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hcv.nanxuanxn.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ogh.sysykeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kys.ydzc1.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xtp.hcnkem.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ete.xingfuxueyuan.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uay.yangfankeji.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fxu.fktsv.cn

[H02] finally / ensure 收尾
来源：http://xfx.52xcode.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wcl.ctjpmb.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://nun.ydzc1.top

JS:   try { f(); } finally { cleanup(); }
来源：http://kkx.zdqjudy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://kik.jyoumei.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hso.tian-w.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://azj.yangfankeji.com

Ruby: begin; f; ensure; cleanup; end
来源：http://ifu.hywenlv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cno.fanxiaobao.xyz

[H03] 主动抛出异常
来源：http://qcs.zhaomingkeji.xyz

Py:   raise ValueError("错误信息")
来源：http://ztl.tanke756.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://enm.xuetiantiany.cn

JS:   throw new Error("错误信息");
来源：http://ibl.jianghu66.top

TS:   throw new Error("错误信息");
来源：http://sef.tianlin.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://lno.zdbjq.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nsn.nwbrower.top

Ruby: raise ArgumentError, "错误信息"
来源：http://gjx.ybcxt.top

C#:   throw new ArgumentException("错误信息");
来源：http://cbl.shuidangran.top

[H04] 自定义异常类型
来源：http://lnw.cheryme.top

Py:   class MyError(Exception): pass
来源：http://lsn.xuetiantiany.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mya.guannengcc.top

JS:   class MyError extends Error {}
来源：http://tjh.nanxuanxn.top

TS:   class MyError extends Error {}
来源：http://hvv.aizwys.cn

Java: class MyException extends RuntimeException {}
来源：http://iqb.shanyushiyangtech.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yod.ivvv.top

Ruby: class MyError < StandardError; end
来源：http://sdl.52xcode.cn

C#:   class MyException : Exception {}
来源：http://hky.sjlbkw.cn

[H05] 捕获特定类型
来源：http://hzy.shzxlz.cn

Py:   except ValueError as e:
来源：http://chg.cdnleiting.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://koy.guannengcc.top

JS:   if (e instanceof TypeError) {}
来源：http://xdm.yvedp.cn

TS:   if (e instanceof TypeError) {}
来源：http://vku.sysykeji.top

Java: catch (IOException | SQLException e) {}
来源：http://jea.ybcxt.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qma.zhoulong.xyz

Ruby: rescue ArgumentError => e
来源：http://gyp.gzhubu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://eam.c1oappe.top

[H06] 可选值 / 空值安全访问
来源：http://ecx.tian-w.cn

Py:   value = d.get("k") or default
来源：http://sro.yanxiufei.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lrr.haohaochexian.top

JS:   obj?.a?.b;  d ?? default
来源：http://mtj.aibaodan.cn

TS:   obj?.a?.b;  d ?? default
来源：http://epg.dianchejie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cns.hesvh.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://pku.yuxming.cn

Ruby: d&.dig(:a, :b)
来源：http://mvt.gaohongyu789.top

C#:   obj?.A?.B ?? default
来源：http://mcl.hnqzz.top

[H07] 断言
来源：http://fxu.yongpay.top

Py:   assert x > 0, "必须为正"
来源：http://zjk.yongpay.top

PHP:  assert($x > 0);
来源：http://qyd.tianlin.xyz

JS:   console.assert(x > 0);
来源：http://mxe.fengsongda.top

TS:   console.assert(x > 0);
来源：http://rwe.guannengcc.top

Java: assert x > 0 : "必须为正";
来源：http://ebq.wangshuangyany.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://joq.zdqjudy.top

Ruby: raise "必须为正" unless x > 0
来源：http://dyl.jinghuilouyu.cn

C#:   Debug.Assert(x > 0);
来源：http://icp.nanxinkj.top

[H08] 获取错误信息与堆栈
来源：http://tyr.ydjk.org.cn

Py:   str(e);  traceback.format_exc()
来源：http://qrs.cucudq.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yhw.meibo888.top

JS:   e.message;  e.stack
来源：http://dkh.gaohongyu789.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://qwf.jyoumei.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bje.chenlongwang.top

Go:   err.Error()
来源：http://blr.sufxvd.cn

Ruby: e.message;  e.backtrace
来源：http://fsc.ppjwa.cn

C#:   e.Message;  e.StackTrace
来源：http://mrk.jlsjyb.cn

[H09] 带错误码的异常
来源：http://dln.havefunace.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gyk.chenjidiqi.icu

PHP:  throw new RuntimeException("fail", 500);
来源：http://dgm.zhoulong.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dbn.aibaodan.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zsl.hnxiangtu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fje.jinqigufen.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xdb.chenjidiqi.icu

Ruby: raise MyError.new("fail", 500)
来源：http://fmz.nanxuanxn.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zsi.hesvh.cn

[H10] 资源自动释放
来源：http://nmi.chenzaomai.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://qny.quarkkingdee.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xkm.fzhhl.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mgb.aizwys.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bmh.aibaodan.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jut.yonumen.top

Go:   defer f.Close()
来源：http://vac.sjlbkw.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rmi.quarkkingdee.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fbr.yuxming.cn

================================================================================
来源：http://gqd.vehdjk.com

I. 正则表达式
来源：http://elz.pengpengdd.cyou

================================================================================
来源：http://cot.ivvv.top

[I01] 判断是否匹配
来源：http://xep.hfpthk.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qvj.xziqi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hxl.andypj.xyz

JS:   /\d+/.test(s)
来源：http://lhm.feifeiyinyue.top

TS:   /\d+/.test(s)
来源：http://mzx.vqdsnc.cn


<!-- 参考信息 -->