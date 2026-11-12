代发 wailian999

Ruby: File.delete("a.txt")
来源：http://sdz.fktsv.cn

C#:   File.Delete("a.txt");
来源：http://jdo.xinyue.icu

[F07] 创建目录（含多级）
来源：http://ris.tianlin.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://uww.wangdashe.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://obx.hammf.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oba.haohaochexian.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bzp.tarul.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nlf.shuidangran.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qhv.jinghuilouyu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cpn.dashuyun.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://eqd.wangdashe.top

[F08] 遍历目录
来源：http://aci.fktsv.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jkm.daria6918.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://eqj.shanyushiyangkeji.top

JS:   fs.readdirSync("dir")
来源：http://yjd.dashuyun.cn

TS:   fs.readdirSync("dir")
来源：http://deb.jinyuanbaomall.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://uvn.zhoulong.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://rgc.sxryk.cn

Ruby: Dir.children("dir")
来源：http://bhr.haohaochexian.top

C#:   Directory.GetFiles("dir")
来源：http://gpw.ivvv.top

[F09] 获取文件大小
来源：http://fez.daxiang520.top

Py:   os.path.getsize("a.txt")
来源：http://sgp.hesvh.cn

PHP:  filesize("a.txt");
来源：http://goz.zhiwuduotai.top

JS:   fs.statSync("a.txt").size
来源：http://xov.jlsjyb.cn

TS:   fs.statSync("a.txt").size
来源：http://fbd.havefunace.top

Java: Files.size(Path.of("a.txt"))
来源：http://xdn.ivvv.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wav.haohaochexian.top

Ruby: File.size("a.txt")
来源：http://eux.sweek.top

C#:   new FileInfo("a.txt").Length
来源：http://ekr.ydjk.org.cn

[F10] 取文件扩展名 / 文件名
来源：http://orn.haohaochexian.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qgb.jianghu66.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gfx.xziqi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mfv.hongshengwenyu.top

TS:   path.extname("a.txt")
来源：http://wcv.andypj.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kdm.yvedp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://guw.tarul.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xqj.nanxuanxn.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rwh.yuxming.cn

[F11] 复制与移动文件
来源：http://opv.nwbrower.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cju.ydzc1.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pqh.jlsjyb.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gnv.yongpay.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dny.mhx1999.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://eyk.gotoacloud.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qeb.fanxiaobao.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ydw.52xcode.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://whh.ppjwa.cn

[F12] CSV 读写
来源：http://cfd.nanxuanxn.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ieh.meibo888.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qxs.sxryk.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ftm.sysykeji.top

TS:   // 同上
来源：http://wpz.shzxlz.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wda.shangyingyoupin.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dhh.yj20258.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gye.meibo888.top

C#:   // 无内置：用 CsvHelper 库
来源：http://yaz.xylfe.cn

================================================================================
来源：http://dsc.jyoumei.cn

G. 面向对象
来源：http://gkr.gotoacloud.top

================================================================================
来源：http://kfq.ywan-chungtsiang.top

[G01] 定义类
来源：http://kht.ybcxt.top

Py:   class User: pass
来源：http://hpj.zhoulong.xyz

PHP:  class User {}
来源：http://qpr.jinqigufen.top

JS:   class User {}
来源：http://rev.52xcode.cn

TS:   class User { name: string = ""; }
来源：http://eop.vehdjk.com

Java: class User {}
来源：http://nnk.sufxvd.cn

Go:   type User struct { Name string }
来源：http://xgn.tanke756.top

Ruby: class User; end
来源：http://kpn.wangdashe.top

C#:   class User {}
来源：http://aoh.svipenyu.cn

[G02] 构造函数
来源：http://mze.pycfn.com

Py:   def __init__(self, name): self.name = name
来源：http://yqg.0kj1m.cn

PHP:  public function __construct(public string $name) {}
来源：http://wun.zhiwuduotai.top

JS:   constructor(name) { this.name = name; }
来源：http://xoh.jinqigufen.top

TS:   constructor(public name: string) {}
来源：http://gvm.316326.xyz

Java: User(String name) { this.name = name; }
来源：http://xkz.tian-w.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mgc.pengpengdd.cyou

Ruby: def initialize(name); @name = name; end
来源：http://okz.nwbrower.top

C#:   public User(string name) { Name = name; }
来源：http://meo.svipenyu.cn

[G03] 实例属性
来源：http://pju.jinyuanbaomall.cn

Py:   self.name = "x"
来源：http://efd.jinghuilouyu.cn

PHP:  public string $name = "x";
来源：http://bpw.ybcxt.top

JS:   this.name = "x";
来源：http://mpr.shangyingyoupin.top

TS:   name: string = "x";
来源：http://xnm.fzhhl.top

Java: private String name;
来源：http://bks.shuidangran.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dsn.haohaochexian.top

Ruby: @name = "x"
来源：http://bke.aizwys.cn

C#:   public string Name { get; set; } = "x";
来源：http://fxu.nwbrower.top

[G04] 定义方法
来源：http://ssi.shuidangran.top

Py:   def greet(self): return self.name
来源：http://gks.fengsongda.top

PHP:  public function greet(): string { return $this->name; }
来源：http://pjx.ctjpmb.com

JS:   greet() { return this.name; }
来源：http://olb.fzhhl.top

TS:   greet(): string { return this.name; }
来源：http://yhg.daxiang520.top

Java: String greet() { return name; }
来源：http://rwx.xylfe.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://upg.cqqwz.cn

Ruby: def greet; @name; end
来源：http://ycr.jinqigufen.top

C#:   public string Greet() => Name;
来源：http://unb.bbcook.cn

[G05] 继承
来源：http://tny.pycfn.com

Py:   class Admin(User): pass
来源：http://nmm.daxiang520.top

PHP:  class Admin extends User {}
来源：http://nap.zdqjudy.top

JS:   class Admin extends User {}
来源：http://khn.yfazqb.com

TS:   class Admin extends User {}
来源：http://twg.vehdjk.com

Java: class Admin extends User {}
来源：http://kge.yuxming.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://avo.chenlongwang.top

Ruby: class Admin < User; end
来源：http://kyo.daria6918.cn

C#:   class Admin : User {}
来源：http://xht.jinqigufen.top

[G06] 重写方法
来源：http://vuy.andypj.xyz

Py:   def greet(self): return "admin"
来源：http://cff.shanyushiyangkeji.top

PHP:  public function greet(): string { return "admin"; }
来源：http://jhg.fengsongda.top

JS:   greet() { return "admin"; }
来源：http://wag.yonumen.top

TS:   greet(): string { return "admin"; }
来源：http://ltr.birdmap.top

Java: @Override String greet() { return "admin"; }
来源：http://cgn.xingfuxueyuan.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://taf.tian-w.cn

Ruby: def greet; "admin"; end
来源：http://kvu.cucudq.cn

C#:   public override string Greet() => "admin";
来源：http://tsv.zhongyouzk.top

[G07] 调用父类方法
来源：http://apo.gotoacloud.top

Py:   super().greet()
来源：http://kvk.tian-w.cn

PHP:  parent::greet();
来源：http://mzn.snrcjt.cn

JS:   super.greet();
来源：http://dpu.meibo888.top

TS:   super.greet();
来源：http://vix.zdbjq.cn

Java: super.greet();
来源：http://ubx.hcnkem.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yzt.gaohongyu789.top

Ruby: super
来源：http://nta.yj20258.top

C#:   base.Greet();
来源：http://twe.feifeiyinyue.top

[G08] 静态方法与属性
来源：http://hpz.hcnkem.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uqq.epnwcf.com

PHP:  public static function f() {}
来源：http://bli.havefunace.top

JS:   static f() {}
来源：http://sbt.ctjpmb.com

TS:   static f(): void {}
来源：http://mml.chenzaomai.com

Java: static void f() {}
来源：http://zdv.sxryk.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jvk.hnqzz.top

Ruby: def self.f; end
来源：http://ymd.vehdjk.com

C#:   public static void F() {}
来源：http://hen.ywan-chungtsiang.top

[G09] 接口 / 抽象类
来源：http://dcf.hysaishi.cn

Py:   from abc import ABC, abstractmethod
来源：http://pyh.nwbrower.top

PHP:  interface Shape { public function area(): float; }
来源：http://njw.aibaodan.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fut.zhaomingkeji.xyz

TS:   interface Shape { area(): number; }
来源：http://orq.xinyue.icu

Java: interface Shape { double area(); }
来源：http://ext.hammf.cn

Go:   type Shape interface { Area() float64 }
来源：http://qye.hnxiangtu.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://shs.daria6918.cn

C#:   interface IShape { double Area(); }
来源：http://qmw.zhijiandao.cn

[G10] 访问控制
来源：http://jyb.hcnkem.com

Py:   约定 _protected / __private（不强制）
来源：http://hin.vqdsnc.cn

PHP:  public / protected / private
来源：http://ckw.yfazqb.com

JS:   #private 字段；其余公开
来源：http://vhg.zdbjq.cn

TS:   public / protected / private
来源：http://vkn.yueranfly.top

Java: public / protected / private / 默认包级
来源：http://rxm.gogol.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tsv.tarul.cn

Ruby: public / protected / private
来源：http://xfs.shangyingyoupin.top

C#:   public / protected / private / internal
来源：http://aoj.zhongyouzk.top

[G11] getter / setter
来源：http://oyf.xziqi.cn

Py:   @property 与 @x.setter
来源：http://htd.guowangkeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://fky.ydzc1.top

JS:   get name() { return this._name; }
来源：http://jyh.yfazqb.com

TS:   get name(): string { return this._name; }
来源：http://hpv.aibaodan.cn

Java: public String getName() { return name; }
来源：http://var.zdqjudy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://zcy.xinyue.icu

Ruby: attr_accessor :name
来源：http://ybp.jyoumei.cn

C#:   public string Name { get; set; }
来源：http://fgx.fzhhl.top

[G12] 对象转字符串
来源：http://ngu.tianlin.xyz

Py:   def __str__(self): return self.name
来源：http://zrh.9152youxi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vwu.yuanzhike.top

JS:   toString() { return this.name; }
来源：http://dbz.tian-w.cn

TS:   toString(): string { return this.name; }
来源：http://vsu.zdbjq.cn

Java: @Override public String toString() { return name; }
来源：http://ilp.wangdashe.top

Go:   func (u User) String() string { return u.Name }
来源：http://xsk.gogol.net.cn

Ruby: def to_s; @name; end
来源：http://hka.andypj.xyz

C#:   public override string ToString() => Name;
来源：http://wfi.wangshuangyany.cn

[G13] 判断对象类型
来源：http://etn.52xcode.cn

Py:   isinstance(u, User)
来源：http://mai.sysykeji.top

PHP:  $u instanceof User
来源：http://zfo.yfazqb.com

JS:   u instanceof User
来源：http://lur.epnwcf.com

TS:   u instanceof User
来源：http://tyx.dashuyun.cn

Java: u instanceof User
来源：http://ojv.xziqi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://hiv.zycfv.cn

Ruby: u.is_a?(User)
来源：http://gvg.vehdjk.com

C#:   u is User
来源：http://ogq.cucudq.cn

[G14] 数据类 / record
来源：http://osx.yj20258888.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://npk.zhijiandao.cn

PHP:  // 用 readonly 属性模拟
来源：http://wpw.cheryme.top

JS:   // 无内置：普通类或对象字面量
来源：http://jpw.shzxlz.cn

TS:   type User = { name: string; age: number };
来源：http://zmr.yongpay.top

Java: record User(String name, int age) {}
来源：http://dfo.sysykeji.top

Go:   type User struct { Name string; Age int }
来源：http://haz.zhixingplan.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kwx.guannengcc.top

C#:   record User(string Name, int Age);
来源：http://cmn.nanxinkj.top

[G15] 枚举
来源：http://prt.zhijiandao.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nmg.yuanzhike.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://gsk.sysykeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://okn.shzxlz.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nqs.ehwqpu.com

Java: enum Color { RED, GREEN }
来源：http://mdj.xylfe.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pfl.zycfv.cn

Ruby: Color = %i[red green].freeze
来源：http://vjv.cdnleiting.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wcv.fktsv.cn

[G16] 对象转数组 / 字典
来源：http://qsn.shangyingyoupin.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fvt.yanxiufei.cn

PHP:  get_object_vars($obj);
来源：http://bel.shuidangran.top

JS:   Object.entries(obj)
来源：http://zfh.yj20258888.top

TS:   Object.entries(obj)
来源：http://kvx.yongpay.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vui.aizwys.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://tpn.haohaochexian.top

Ruby: obj.instance_variables
来源：http://qlm.cashguo.top

C#:   // 用反射或 System.Text.Json
来源：http://tst.hysaishi.cn

================================================================================
来源：http://gkj.hcnkem.com

H. 异常与错误处理
来源：http://oeo.zhengqikj.top

================================================================================
来源：http://dtg.haohaochexian.top

[H01] try / catch 基础
来源：http://isv.chenjidiqi.icu

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lox.guannengcc.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fgz.zhixingplan.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yrb.vqdsnc.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lot.snrcjt.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ntw.pengpengdd.cyou

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tau.vqdsnc.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pgn.ctjpmb.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tsg.jlsjyb.cn

[H02] finally / ensure 收尾
来源：http://qwm.yuxming.cn

Py:   try: f()⏎finally: cleanup()
来源：http://lbx.mhx1999.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://gzx.xziqi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ixs.sufxvd.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://dep.gzhubu.top

Java: try { f(); } finally { cleanup(); }
来源：http://swj.cucudq.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ykw.guannengcc.top

Ruby: begin; f; ensure; cleanup; end
来源：http://oog.yj202588.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://lkq.jinyuanbaomall.cn

[H03] 主动抛出异常
来源：http://fwt.cheryme.top

Py:   raise ValueError("错误信息")
来源：http://msn.vehdjk.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hfy.vqdsnc.cn

JS:   throw new Error("错误信息");
来源：http://one.chenzaomai.com

TS:   throw new Error("错误信息");
来源：http://gap.wangshuangyany.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lev.yj20258888.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zsk.zycfv.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://enl.yj202588.top

C#:   throw new ArgumentException("错误信息");
来源：http://qzu.vehdjk.com

[H04] 自定义异常类型
来源：http://qkh.redwolf501.top

Py:   class MyError(Exception): pass
来源：http://sgm.zhiwuduotai.top

PHP:  class MyError extends RuntimeException {}
来源：http://otj.tianlin.xyz

JS:   class MyError extends Error {}
来源：http://shz.nanxinkj.top

TS:   class MyError extends Error {}
来源：http://mgp.andypj.xyz

Java: class MyException extends RuntimeException {}
来源：http://oqr.hysaishi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tsx.dashuyun.cn

Ruby: class MyError < StandardError; end
来源：http://tsw.bjfxy.top

C#:   class MyException : Exception {}
来源：http://igy.yfazqb.com

[H05] 捕获特定类型
来源：http://qxa.pycfn.com

Py:   except ValueError as e:
来源：http://bud.yvedp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rvi.epnwcf.com

JS:   if (e instanceof TypeError) {}
来源：http://dpi.epnwcf.com

TS:   if (e instanceof TypeError) {}
来源：http://cpc.yueranfly.top

Java: catch (IOException | SQLException e) {}
来源：http://sqs.shanyushiyangtech.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cvn.mhx1999.top

Ruby: rescue ArgumentError => e
来源：http://hjc.yvedp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://knh.yonumen.top

[H06] 可选值 / 空值安全访问
来源：http://otn.pycfn.com

Py:   value = d.get("k") or default
来源：http://igv.gogol.net.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kpz.tanke756.top

JS:   obj?.a?.b;  d ?? default
来源：http://vwy.bbcook.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jpw.svipenyu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gye.yj20258888.top

Go:   if v, ok := m["k"]; ok { }
来源：http://jje.sufxvd.cn

Ruby: d&.dig(:a, :b)
来源：http://wke.pengpengdd.cyou

C#:   obj?.A?.B ?? default
来源：http://non.uphjek.com

[H07] 断言
来源：http://vek.guowangkeji.top

Py:   assert x > 0, "必须为正"
来源：http://klh.pycfn.com

PHP:  assert($x > 0);
来源：http://ihw.kuanghao11.cn

JS:   console.assert(x > 0);
来源：http://zmj.yangfankeji.com

TS:   console.assert(x > 0);
来源：http://tam.andypj.xyz

Java: assert x > 0 : "必须为正";
来源：http://myi.feifeiyinyue.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rxq.yangfankeji.com

Ruby: raise "必须为正" unless x > 0
来源：http://odv.sxryk.cn

C#:   Debug.Assert(x > 0);
来源：http://sds.hfpthk.cn

[H08] 获取错误信息与堆栈
来源：http://kvh.aibaodan.cn

Py:   str(e);  traceback.format_exc()
来源：http://djl.tian-w.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uiy.hnqzz.top

JS:   e.message;  e.stack
来源：http://nfi.ehwqpu.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://dfk.hfpthk.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zmg.hfpthk.cn

Go:   err.Error()
来源：http://evw.zhijiandao.cn

Ruby: e.message;  e.backtrace
来源：http://ojz.xziqi.cn

C#:   e.Message;  e.StackTrace
来源：http://jby.guannengcc.top

[H09] 带错误码的异常
来源：http://rqy.epnwcf.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fnh.ctjpmb.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://iag.52xcode.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ito.mhx1999.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lgv.xziqi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://khz.xuanzx.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cal.vehdjk.com

Ruby: raise MyError.new("fail", 500)
来源：http://elm.xingfuxueyuan.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://yzy.xinyue.icu

[H10] 资源自动释放
来源：http://xbj.zhoulong.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://fox.daria6918.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cny.yfazqb.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vfu.gaohongyu789.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ozo.hcnkem.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jfg.svipenyu.cn

Go:   defer f.Close()
来源：http://opf.zhixingplan.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hnb.yuanzhike.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://iyf.sufxvd.cn

================================================================================
来源：http://nfb.shangyingyoupin.top

I. 正则表达式
来源：http://knb.havefunace.top

================================================================================
来源：http://vpu.meibo888.top

[I01] 判断是否匹配
来源：http://qnt.ydjk.org.cn


<!-- 参考信息 -->