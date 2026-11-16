代发 wailian999

C#:   File.Exists("a.txt")
来源：http://dnb.yfazqb.com

[F06] 删除文件
来源：http://ohq.ppjwa.cn

Py:   os.remove("a.txt")
来源：http://waa.jqgufenzy.top

PHP:  unlink("a.txt");
来源：http://nwv.xuanzx.com

JS:   fs.unlinkSync("a.txt")
来源：http://mzm.hesvh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://teu.tanke756.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nes.shuidangran.top

Go:   os.Remove("a.txt")
来源：http://erx.dashuyun.cn

Ruby: File.delete("a.txt")
来源：http://mhi.xinyue.icu

C#:   File.Delete("a.txt");
来源：http://dtq.feifeiyinyue.top

[F07] 创建目录（含多级）
来源：http://sqe.daria6918.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nml.yonumen.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jyf.jinghuilouyu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://djg.quarkkingdee.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ehq.zhongyouzk.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aak.jqgfzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wlm.yfazqb.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://umw.xinyue.icu

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qcp.tian-w.cn

[F08] 遍历目录
来源：http://nnf.fehbvm.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://pvj.dianchejie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gqc.jinqigufen.top

JS:   fs.readdirSync("dir")
来源：http://fgt.tian-w.cn

TS:   fs.readdirSync("dir")
来源：http://mwm.cashguo.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://atb.dianchejie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ajy.52xcode.cn

Ruby: Dir.children("dir")
来源：http://bvz.andypj.xyz

C#:   Directory.GetFiles("dir")
来源：http://edt.ctjpmb.com

[F09] 获取文件大小
来源：http://iwh.hywenlv.cn

Py:   os.path.getsize("a.txt")
来源：http://cgp.epnwcf.com

PHP:  filesize("a.txt");
来源：http://mzw.xziqi.cn

JS:   fs.statSync("a.txt").size
来源：http://xvd.bbcook.cn

TS:   fs.statSync("a.txt").size
来源：http://miy.0kj1m.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fkl.gotoacloud.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gds.yj20258888.top

Ruby: File.size("a.txt")
来源：http://jiy.yangfankeji.com

C#:   new FileInfo("a.txt").Length
来源：http://ans.feifeiyinyue.top

[F10] 取文件扩展名 / 文件名
来源：http://uuu.daxiang520.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zdd.xuetiantiany.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zpb.kuanghao11.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vtt.fanxiaobao.xyz

TS:   path.extname("a.txt")
来源：http://fxr.ybcxt.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rwq.cucudq.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ckv.guowangkeji.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xzs.hcnkem.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jbd.yongpay.top

[F11] 复制与移动文件
来源：http://snc.guowangkeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tuu.feifeiyinyue.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pdr.tarul.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lnm.havefunace.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oic.zhoulong.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://apl.fktsv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dvv.dianchejie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ugw.fzhhl.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://enl.zhengqikj.top

[F12] CSV 读写
来源：http://pbs.tianlin.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dlx.jinqigfzy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://oyk.daria6918.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vxp.xuanzx.com

TS:   // 同上
来源：http://etr.jinghuilouyu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sij.jinqigfzy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vxs.guannengcc.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eng.xinyue.icu

C#:   // 无内置：用 CsvHelper 库
来源：http://xuc.dashuyun.cn

================================================================================
来源：http://wqn.bbcook.cn

G. 面向对象
来源：http://tmi.smart0.xyz

================================================================================
来源：http://tpk.9152youxi.cn

[G01] 定义类
来源：http://ubh.cucudq.cn

Py:   class User: pass
来源：http://klq.hcnkem.com

PHP:  class User {}
来源：http://akb.bbcook.cn

JS:   class User {}
来源：http://mji.fanxiaobao.xyz

TS:   class User { name: string = ""; }
来源：http://ioc.aibaodan.cn

Java: class User {}
来源：http://xnn.jqgufenzy.top

Go:   type User struct { Name string }
来源：http://gdu.cucudq.cn

Ruby: class User; end
来源：http://dbu.hywenlv.cn

C#:   class User {}
来源：http://poz.hywenlv.cn

[G02] 构造函数
来源：http://gnh.cheryme.top

Py:   def __init__(self, name): self.name = name
来源：http://fgj.xuetiantiany.cn

PHP:  public function __construct(public string $name) {}
来源：http://pca.sysykeji.top

JS:   constructor(name) { this.name = name; }
来源：http://frk.yj202588.top

TS:   constructor(public name: string) {}
来源：http://ttj.yongpay.top

Java: User(String name) { this.name = name; }
来源：http://kuc.zhijiandao.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rfx.hnqzz.top

Ruby: def initialize(name); @name = name; end
来源：http://dvu.fktsv.cn

C#:   public User(string name) { Name = name; }
来源：http://fmv.c1oappe.top

[G03] 实例属性
来源：http://bcl.xuetiantiany.cn

Py:   self.name = "x"
来源：http://igu.tanke756.top

PHP:  public string $name = "x";
来源：http://uaf.zhoulong.xyz

JS:   this.name = "x";
来源：http://czs.xylfe.cn

TS:   name: string = "x";
来源：http://xqc.daxiang520.top

Java: private String name;
来源：http://ned.sufxvd.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gvd.yuxming.cn

Ruby: @name = "x"
来源：http://fee.zhijiandao.cn

C#:   public string Name { get; set; } = "x";
来源：http://lyo.9152youxi.cn

[G04] 定义方法
来源：http://vft.haohaochexian.top

Py:   def greet(self): return self.name
来源：http://xbb.ydjk.org.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://cuj.xinyue.icu

JS:   greet() { return this.name; }
来源：http://osg.nanxinkj.top

TS:   greet(): string { return this.name; }
来源：http://uuo.yongpay.top

Java: String greet() { return name; }
来源：http://gmn.gaohongyu789.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://vbh.xuetiantiany.cn

Ruby: def greet; @name; end
来源：http://ggy.meibo888.top

C#:   public string Greet() => Name;
来源：http://bwm.guowangkeji.top

[G05] 继承
来源：http://cov.iojbl.cn

Py:   class Admin(User): pass
来源：http://ljf.0kj1m.cn

PHP:  class Admin extends User {}
来源：http://bmo.shanyushiyangtech.top

JS:   class Admin extends User {}
来源：http://mzk.gzhubu.top

TS:   class Admin extends User {}
来源：http://ekr.pengpengdd.cyou

Java: class Admin extends User {}
来源：http://izc.nwbrower.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vxy.bbcook.cn

Ruby: class Admin < User; end
来源：http://ovd.uphjek.com

C#:   class Admin : User {}
来源：http://hio.yuxming.cn

[G06] 重写方法
来源：http://wgn.dianchejie.cn

Py:   def greet(self): return "admin"
来源：http://kik.jianghu66.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ozo.iojbl.cn

JS:   greet() { return "admin"; }
来源：http://mbn.andypj.xyz

TS:   greet(): string { return "admin"; }
来源：http://pch.ivvv.top

Java: @Override String greet() { return "admin"; }
来源：http://edx.vqdsnc.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://eic.guowangkeji.top

Ruby: def greet; "admin"; end
来源：http://zyt.jinyuanbaomall.cn

C#:   public override string Greet() => "admin";
来源：http://mbj.jianghu66.top

[G07] 调用父类方法
来源：http://zzq.andypj.xyz

Py:   super().greet()
来源：http://vdg.fehbvm.com

PHP:  parent::greet();
来源：http://fmw.9152youxi.cn

JS:   super.greet();
来源：http://smm.jinqigufen.top

TS:   super.greet();
来源：http://ink.yanxiufei.cn

Java: super.greet();
来源：http://cyo.hesvh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://axb.pycfn.com

Ruby: super
来源：http://yql.sjlbkw.cn

C#:   base.Greet();
来源：http://hzk.zhoulong.xyz

[G08] 静态方法与属性
来源：http://vwe.0kj1m.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://irf.xziqi.cn

PHP:  public static function f() {}
来源：http://vil.wangdashe.top

JS:   static f() {}
来源：http://uzq.kuanghao11.cn

TS:   static f(): void {}
来源：http://xex.xuetiantiany.cn

Java: static void f() {}
来源：http://oni.zhijiandao.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://sef.ydzc1.top

Ruby: def self.f; end
来源：http://qwh.cqqwz.cn

C#:   public static void F() {}
来源：http://pdd.jqgfzy.top

[G09] 接口 / 抽象类
来源：http://uha.yanxiufei.cn

Py:   from abc import ABC, abstractmethod
来源：http://tme.yj20258.top

PHP:  interface Shape { public function area(): float; }
来源：http://ylq.ydzc1.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://vjw.zdbjq.cn

TS:   interface Shape { area(): number; }
来源：http://bvl.zdqjudy.top

Java: interface Shape { double area(); }
来源：http://ypm.snrcjt.cn

Go:   type Shape interface { Area() float64 }
来源：http://adx.sjlbkw.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tah.hongshengwenyu.top

C#:   interface IShape { double Area(); }
来源：http://zpw.hfpthk.cn

[G10] 访问控制
来源：http://yif.gaohongyu789.top

Py:   约定 _protected / __private（不强制）
来源：http://awc.mhx1999.top

PHP:  public / protected / private
来源：http://hrf.wangshuangyany.cn

JS:   #private 字段；其余公开
来源：http://lgd.xziqi.cn

TS:   public / protected / private
来源：http://lxw.ydjk.org.cn

Java: public / protected / private / 默认包级
来源：http://okz.zycfv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://zvs.guowangkeji.top

Ruby: public / protected / private
来源：http://tlx.fengsongda.top

C#:   public / protected / private / internal
来源：http://grb.yanxiufei.cn

[G11] getter / setter
来源：http://ain.snrcjt.cn

Py:   @property 与 @x.setter
来源：http://yez.ctjpmb.com

PHP:  public function getName(): string { return $this->name; }
来源：http://tww.hywenlv.cn

JS:   get name() { return this._name; }
来源：http://hfa.yongpay.top

TS:   get name(): string { return this._name; }
来源：http://syu.daria6918.cn

Java: public String getName() { return name; }
来源：http://dez.tanke756.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://bna.yvedp.cn

Ruby: attr_accessor :name
来源：http://nqr.pengpengdd.cyou

C#:   public string Name { get; set; }
来源：http://arz.fanxiaobao.xyz

[G12] 对象转字符串
来源：http://mzo.pycfn.com

Py:   def __str__(self): return self.name
来源：http://zfw.yueranfly.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ytg.xylfe.cn

JS:   toString() { return this.name; }
来源：http://aek.zhaomingkeji.xyz

TS:   toString(): string { return this.name; }
来源：http://har.sysykeji.top

Java: @Override public String toString() { return name; }
来源：http://dbn.tian-w.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hef.redwolf501.top

Ruby: def to_s; @name; end
来源：http://uld.tianlin.xyz

C#:   public override string ToString() => Name;
来源：http://cbp.ppjwa.cn

[G13] 判断对象类型
来源：http://yye.ivvv.top

Py:   isinstance(u, User)
来源：http://uvw.52xcode.cn

PHP:  $u instanceof User
来源：http://dsi.gaohongyu789.top

JS:   u instanceof User
来源：http://otp.gzhubu.top

TS:   u instanceof User
来源：http://nje.pengpengdd.cyou

Java: u instanceof User
来源：http://pre.zhijiandao.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mvz.hesvh.cn

Ruby: u.is_a?(User)
来源：http://uui.gzhubu.top

C#:   u is User
来源：http://avz.sxryk.cn

[G14] 数据类 / record
来源：http://ose.dianchejie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tzw.cheryme.top

PHP:  // 用 readonly 属性模拟
来源：http://elr.hammf.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jlh.ivvv.top

TS:   type User = { name: string; age: number };
来源：http://lyg.meibo888.top

Java: record User(String name, int age) {}
来源：http://zfh.sufxvd.cn

Go:   type User struct { Name string; Age int }
来源：http://aay.zhoulong.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://toy.shangyingyoupin.top

C#:   record User(string Name, int Age);
来源：http://uud.hfpthk.cn

[G15] 枚举
来源：http://dsk.yonumen.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pyo.nanxinkj.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://vdf.pengpengdd.cyou

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://paa.fktsv.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sdx.tianlin.xyz

Java: enum Color { RED, GREEN }
来源：http://iol.ivvv.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ifr.xziqi.cn

Ruby: Color = %i[red green].freeze
来源：http://xwu.fengsongda.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://suc.shangyingyoupin.top

[G16] 对象转数组 / 字典
来源：http://wzt.shuidangran.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://aox.yvedp.cn

PHP:  get_object_vars($obj);
来源：http://rza.daxiang520.top

JS:   Object.entries(obj)
来源：http://cvd.tianlin.xyz

TS:   Object.entries(obj)
来源：http://jgc.daria6918.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wvr.hammf.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dvg.zycfv.cn

Ruby: obj.instance_variables
来源：http://mbl.nanxuanxn.top

C#:   // 用反射或 System.Text.Json
来源：http://bbi.guannengcc.top

================================================================================
来源：http://xug.9152youxi.cn

H. 异常与错误处理
来源：http://zmv.zhongyouzk.top

================================================================================
来源：http://vya.mhx1999.top

[H01] try / catch 基础
来源：http://efg.pycfn.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kpl.sweek.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://utb.hnqzz.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xmt.yj20258888.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jdi.fktsv.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kll.jqgufenzy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://afk.guowangkeji.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rdn.zhaomingkeji.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://egq.snrcjt.cn

[H02] finally / ensure 收尾
来源：http://npv.jlsjyb.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tpr.yj20258.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://wot.nwbrower.top

JS:   try { f(); } finally { cleanup(); }
来源：http://zxr.uphjek.com

TS:   try { f(); } finally { cleanup(); }
来源：http://uzb.fehbvm.com

Java: try { f(); } finally { cleanup(); }
来源：http://gjs.yongpay.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://rgl.jinqigfzy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://jlj.cashguo.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://vgg.cucudq.cn

[H03] 主动抛出异常
来源：http://sux.nanxinkj.top

Py:   raise ValueError("错误信息")
来源：http://huy.c1oappe.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://omj.cqqwz.cn

JS:   throw new Error("错误信息");
来源：http://ots.yj202588.top

TS:   throw new Error("错误信息");
来源：http://exs.cdnleiting.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://arb.gaohongyu789.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xxv.shzxlz.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gos.sweek.top

C#:   throw new ArgumentException("错误信息");
来源：http://amp.iojbl.cn

[H04] 自定义异常类型
来源：http://meh.fanxiaobao.xyz

Py:   class MyError(Exception): pass
来源：http://nsc.guowangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://enc.tian-w.cn

JS:   class MyError extends Error {}
来源：http://xnx.xziqi.cn

TS:   class MyError extends Error {}
来源：http://ilf.svipenyu.cn

Java: class MyException extends RuntimeException {}
来源：http://ekj.yonumen.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://iwb.quarkkingdee.top

Ruby: class MyError < StandardError; end
来源：http://ono.fehbvm.com

C#:   class MyException : Exception {}
来源：http://fwa.pengpengdd.cyou

[H05] 捕获特定类型
来源：http://oln.aizwys.cn

Py:   except ValueError as e:
来源：http://vdn.yangfankeji.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pln.xuetiantiany.cn

JS:   if (e instanceof TypeError) {}
来源：http://wlm.hammf.cn

TS:   if (e instanceof TypeError) {}
来源：http://svr.xuetiantiany.cn

Java: catch (IOException | SQLException e) {}
来源：http://kqx.wangshuangyany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rcl.ppjwa.cn

Ruby: rescue ArgumentError => e
来源：http://ulo.fzhhl.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wuz.xylfe.cn

[H06] 可选值 / 空值安全访问
来源：http://dny.gaohongyu789.top

Py:   value = d.get("k") or default
来源：http://dmx.hfpthk.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pxs.sufxvd.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wzo.c1oappe.top

TS:   obj?.a?.b;  d ?? default
来源：http://bvc.jinqigufen.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://myi.9152youxi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mrf.redwolf501.top

Ruby: d&.dig(:a, :b)
来源：http://wdd.sweek.top

C#:   obj?.A?.B ?? default
来源：http://bmg.nwbrower.top

[H07] 断言
来源：http://jjr.hammf.cn

Py:   assert x > 0, "必须为正"
来源：http://kaz.9152youxi.cn

PHP:  assert($x > 0);
来源：http://lvr.bbcook.cn

JS:   console.assert(x > 0);
来源：http://mds.guannengcc.top

TS:   console.assert(x > 0);
来源：http://bpj.52xcode.cn

Java: assert x > 0 : "必须为正";
来源：http://abm.uphjek.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fim.zhaomingkeji.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://yfl.fanxiaobao.xyz

C#:   Debug.Assert(x > 0);
来源：http://kol.vqdsnc.cn

[H08] 获取错误信息与堆栈
来源：http://uiy.shangyingyoupin.top

Py:   str(e);  traceback.format_exc()
来源：http://sju.jqgufenzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qcw.zhaomingkeji.xyz

JS:   e.message;  e.stack
来源：http://iko.zdbjq.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gmq.ybcxt.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ovb.yj20258888.top

Go:   err.Error()
来源：http://ndc.nanxinkj.top

Ruby: e.message;  e.backtrace
来源：http://yix.haohaochexian.top

C#:   e.Message;  e.StackTrace
来源：http://dua.hcnkem.com

[H09] 带错误码的异常
来源：http://loe.sufxvd.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jns.ppjwa.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://con.bbcook.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fab.kuanghao11.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://olj.sufxvd.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hua.hammf.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zdp.jlsjyb.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ksq.yonumen.top

C#:   // 自定义异常类中加 Code 属性
来源：http://naz.yanxiufei.cn

[H10] 资源自动释放
来源：http://rkg.tianlin.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://bif.xingfuxueyuan.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wps.fzhhl.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://scy.fengsongda.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sao.hywenlv.cn


<!-- 参考信息 -->