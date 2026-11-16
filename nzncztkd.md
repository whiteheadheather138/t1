代发 wailian999

Ruby: File.delete("a.txt")
来源：http://xdh.yuanzhike.top

C#:   File.Delete("a.txt");
来源：http://wxg.quarkkingdee.top

[F07] 创建目录（含多级）
来源：http://zmc.hongshengwenyu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nvg.zycfv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wmz.shuidangran.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wqd.ydzc1.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jff.guowangkeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hkx.fanxiaobao.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rft.aizwys.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dpx.xylfe.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nmy.epnwcf.com

[F08] 遍历目录
来源：http://wsg.zhixingplan.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://tqq.wangdashe.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://heb.ppjwa.cn

JS:   fs.readdirSync("dir")
来源：http://lcl.mhx1999.top

TS:   fs.readdirSync("dir")
来源：http://mxj.feifeiyinyue.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jor.xuetiantiany.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://aeu.cucudq.cn

Ruby: Dir.children("dir")
来源：http://lkk.ctjpmb.com

C#:   Directory.GetFiles("dir")
来源：http://van.fengsongda.top

[F09] 获取文件大小
来源：http://yfv.cheryme.top

Py:   os.path.getsize("a.txt")
来源：http://uno.jinyuanbaomall.cn

PHP:  filesize("a.txt");
来源：http://baz.shanyushiyangtech.top

JS:   fs.statSync("a.txt").size
来源：http://xfh.jlsjyb.cn

TS:   fs.statSync("a.txt").size
来源：http://zqa.fanxiaobao.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://jbq.ppjwa.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://iun.tianlin.xyz

Ruby: File.size("a.txt")
来源：http://mcc.jinyuanbaomall.cn

C#:   new FileInfo("a.txt").Length
来源：http://wou.pengpengdd.cyou

[F10] 取文件扩展名 / 文件名
来源：http://yof.zhengqikj.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wbf.yongpay.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lpd.kuanghao11.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://awd.kuanghao11.cn

TS:   path.extname("a.txt")
来源：http://bay.quarkkingdee.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lnk.gotoacloud.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wbd.wangdashe.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ksq.andypj.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://aud.haohaochexian.top

[F11] 复制与移动文件
来源：http://ogn.quarkkingdee.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bdq.jqgfzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tsn.redwolf501.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tdw.aizwys.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://adl.zhiwuduotai.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tnq.pycfn.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pth.guannengcc.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nou.nanxuanxn.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yfm.ydjk.org.cn

[F12] CSV 读写
来源：http://vib.shangyingyoupin.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://etl.bbcook.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dcs.hammf.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jxd.haohaochexian.top

TS:   // 同上
来源：http://ccy.c1oappe.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ryf.dianchejie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qdn.fengsongda.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kcn.xingfuxueyuan.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://eri.iojbl.cn

================================================================================
来源：http://kez.jinqigfzy.top

G. 面向对象
来源：http://rpu.zhengqikj.top

================================================================================
来源：http://oyb.sxryk.cn

[G01] 定义类
来源：http://xww.guowangkeji.top

Py:   class User: pass
来源：http://chp.xuanzx.com

PHP:  class User {}
来源：http://nva.andypj.xyz

JS:   class User {}
来源：http://bgp.hysaishi.cn

TS:   class User { name: string = ""; }
来源：http://iwp.nwbrower.top

Java: class User {}
来源：http://cmu.zhongyouzk.top

Go:   type User struct { Name string }
来源：http://tfb.jlsjyb.cn

Ruby: class User; end
来源：http://bzj.zdbjq.cn

C#:   class User {}
来源：http://xdv.zhijiandao.cn

[G02] 构造函数
来源：http://nuz.andypj.xyz

Py:   def __init__(self, name): self.name = name
来源：http://rle.jqgufenzy.top

PHP:  public function __construct(public string $name) {}
来源：http://blo.sweek.top

JS:   constructor(name) { this.name = name; }
来源：http://geb.chenlongwang.top

TS:   constructor(public name: string) {}
来源：http://hcz.yanxiufei.cn

Java: User(String name) { this.name = name; }
来源：http://kyi.smart0.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bbw.ybcxt.top

Ruby: def initialize(name); @name = name; end
来源：http://qkf.shanyushiyangkeji.top

C#:   public User(string name) { Name = name; }
来源：http://qhm.kuanghao11.cn

[G03] 实例属性
来源：http://sed.gotoacloud.top

Py:   self.name = "x"
来源：http://owx.jinyuanbaomall.cn

PHP:  public string $name = "x";
来源：http://voo.zhongyouzk.top

JS:   this.name = "x";
来源：http://uzi.zdbjq.cn

TS:   name: string = "x";
来源：http://pez.epnwcf.com

Java: private String name;
来源：http://mik.meibo888.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xae.feifeiyinyue.top

Ruby: @name = "x"
来源：http://mez.yj20258888.top

C#:   public string Name { get; set; } = "x";
来源：http://flj.yuanzhike.top

[G04] 定义方法
来源：http://uoq.shanyushiyangtech.top

Py:   def greet(self): return self.name
来源：http://alo.jlsjyb.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zfs.daria6918.cn

JS:   greet() { return this.name; }
来源：http://nww.fengsongda.top

TS:   greet(): string { return this.name; }
来源：http://wvl.yuanzhike.top

Java: String greet() { return name; }
来源：http://gre.jqgufenzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://fjl.hnxiangtu.top

Ruby: def greet; @name; end
来源：http://mgc.cdnleiting.top

C#:   public string Greet() => Name;
来源：http://gmc.sufxvd.cn

[G05] 继承
来源：http://yxv.chenlongwang.top

Py:   class Admin(User): pass
来源：http://uhy.vehdjk.com

PHP:  class Admin extends User {}
来源：http://iff.redwolf501.top

JS:   class Admin extends User {}
来源：http://nur.zycfv.cn

TS:   class Admin extends User {}
来源：http://sie.shzxlz.cn

Java: class Admin extends User {}
来源：http://gkq.jinghuilouyu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gtd.snrcjt.cn

Ruby: class Admin < User; end
来源：http://ygy.zhongyouzk.top

C#:   class Admin : User {}
来源：http://flv.yfazqb.com

[G06] 重写方法
来源：http://eye.vehdjk.com

Py:   def greet(self): return "admin"
来源：http://bjk.gzhubu.top

PHP:  public function greet(): string { return "admin"; }
来源：http://vtw.cqqwz.cn

JS:   greet() { return "admin"; }
来源：http://aun.sweek.top

TS:   greet(): string { return "admin"; }
来源：http://xge.yj202588.top

Java: @Override String greet() { return "admin"; }
来源：http://mcv.0kj1m.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bxl.yj20258888.top

Ruby: def greet; "admin"; end
来源：http://wab.zhoulong.xyz

C#:   public override string Greet() => "admin";
来源：http://boo.fktsv.cn

[G07] 调用父类方法
来源：http://kck.yongpay.top

Py:   super().greet()
来源：http://ona.fzhhl.top

PHP:  parent::greet();
来源：http://txe.sufxvd.cn

JS:   super.greet();
来源：http://ktu.ctjpmb.com

TS:   super.greet();
来源：http://dag.fktsv.cn

Java: super.greet();
来源：http://ocx.cashguo.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ucw.redwolf501.top

Ruby: super
来源：http://uha.zhengqikj.top

C#:   base.Greet();
来源：http://qom.hysaishi.cn

[G08] 静态方法与属性
来源：http://tcq.316326.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wlg.cheryme.top

PHP:  public static function f() {}
来源：http://yzu.smart0.xyz

JS:   static f() {}
来源：http://kgq.nwbrower.top

TS:   static f(): void {}
来源：http://vwn.ehwqpu.com

Java: static void f() {}
来源：http://gmi.mhx1999.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ccx.fanxiaobao.xyz

Ruby: def self.f; end
来源：http://bya.aizwys.cn

C#:   public static void F() {}
来源：http://tls.zhiwuduotai.top

[G09] 接口 / 抽象类
来源：http://hky.zhoulong.xyz

Py:   from abc import ABC, abstractmethod
来源：http://lkh.yuanzhike.top

PHP:  interface Shape { public function area(): float; }
来源：http://dqh.shanyushiyangkeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://kyx.xylfe.cn

TS:   interface Shape { area(): number; }
来源：http://grb.sysykeji.top

Java: interface Shape { double area(); }
来源：http://lox.fengsongda.top

Go:   type Shape interface { Area() float64 }
来源：http://owu.zhiwuduotai.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://osr.yangfankeji.com

C#:   interface IShape { double Area(); }
来源：http://aaw.hongshengwenyu.top

[G10] 访问控制
来源：http://wvw.gzhubu.top

Py:   约定 _protected / __private（不强制）
来源：http://kpv.redwolf501.top

PHP:  public / protected / private
来源：http://wmt.shanyushiyangtech.top

JS:   #private 字段；其余公开
来源：http://tyq.smart0.xyz

TS:   public / protected / private
来源：http://odq.mhx1999.top

Java: public / protected / private / 默认包级
来源：http://hly.jinqigufen.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://tol.snrcjt.cn

Ruby: public / protected / private
来源：http://chm.fzhhl.top

C#:   public / protected / private / internal
来源：http://mhe.haohaochexian.top

[G11] getter / setter
来源：http://pnk.fzhhl.top

Py:   @property 与 @x.setter
来源：http://fay.bbcook.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cxy.hnxiangtu.top

JS:   get name() { return this._name; }
来源：http://lby.ppjwa.cn

TS:   get name(): string { return this._name; }
来源：http://vwp.cqqwz.cn

Java: public String getName() { return name; }
来源：http://gtt.fktsv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ato.cheryme.top

Ruby: attr_accessor :name
来源：http://ikt.zhaomingkeji.xyz

C#:   public string Name { get; set; }
来源：http://leg.hfpthk.cn

[G12] 对象转字符串
来源：http://ypp.kuanghao11.cn

Py:   def __str__(self): return self.name
来源：http://ima.ydzc1.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://mel.sxryk.cn

JS:   toString() { return this.name; }
来源：http://hqz.hesvh.cn

TS:   toString(): string { return this.name; }
来源：http://tho.zhijiandao.cn

Java: @Override public String toString() { return name; }
来源：http://ugd.52xcode.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zra.jinghuilouyu.cn

Ruby: def to_s; @name; end
来源：http://jws.tian-w.cn

C#:   public override string ToString() => Name;
来源：http://cal.hywenlv.cn

[G13] 判断对象类型
来源：http://hyt.hywenlv.cn

Py:   isinstance(u, User)
来源：http://rct.hammf.cn

PHP:  $u instanceof User
来源：http://avj.jyoumei.cn

JS:   u instanceof User
来源：http://gkv.birdmap.top

TS:   u instanceof User
来源：http://dmy.ydjk.org.cn

Java: u instanceof User
来源：http://lju.shanyushiyangkeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://bth.epnwcf.com

Ruby: u.is_a?(User)
来源：http://tdg.jinqigufen.top

C#:   u is User
来源：http://mds.aizwys.cn

[G14] 数据类 / record
来源：http://dvl.jiagoushi.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pjs.uphjek.com

PHP:  // 用 readonly 属性模拟
来源：http://qcf.feifeiyinyue.top

JS:   // 无内置：普通类或对象字面量
来源：http://qtl.hesvh.cn

TS:   type User = { name: string; age: number };
来源：http://vdv.wangdashe.top

Java: record User(String name, int age) {}
来源：http://ywd.sxryk.cn

Go:   type User struct { Name string; Age int }
来源：http://ciy.feifeiyinyue.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jcs.fktsv.cn

C#:   record User(string Name, int Age);
来源：http://cvb.hesvh.cn

[G15] 枚举
来源：http://hgk.dianchejie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ssw.shanyushiyangkeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://vuw.daria6918.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qrb.jqgufenzy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://noi.jinghuilouyu.cn

Java: enum Color { RED, GREEN }
来源：http://gty.dashuyun.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kse.ctjpmb.com

Ruby: Color = %i[red green].freeze
来源：http://uwe.jinyuanbaomall.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://svb.dashuyun.cn

[G16] 对象转数组 / 字典
来源：http://myz.xinyue.icu

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://afg.yj202588.top

PHP:  get_object_vars($obj);
来源：http://kpd.yj20258.top

JS:   Object.entries(obj)
来源：http://xni.yj20258.top

TS:   Object.entries(obj)
来源：http://nci.ctjpmb.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://twk.jlsjyb.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://nsh.jinqigufen.top

Ruby: obj.instance_variables
来源：http://bqi.feifeiyinyue.top

C#:   // 用反射或 System.Text.Json
来源：http://xzg.daria6918.cn

================================================================================
来源：http://tez.fzhhl.top

H. 异常与错误处理
来源：http://llc.jinyuanbaomall.cn

================================================================================
来源：http://jiq.yongpay.top

[H01] try / catch 基础
来源：http://lua.yanxiufei.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xlw.dashuyun.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vqu.sysykeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qpj.yongpay.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bvf.cdnleiting.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sqg.sxryk.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://azm.hfpthk.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://etv.hnxiangtu.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xdi.nanxinkj.top

[H02] finally / ensure 收尾
来源：http://blx.ivvv.top

Py:   try: f()⏎finally: cleanup()
来源：http://bwk.yj20258.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://kvp.havefunace.top

JS:   try { f(); } finally { cleanup(); }
来源：http://iuv.smart0.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://zrx.cdnleiting.top

Java: try { f(); } finally { cleanup(); }
来源：http://hvh.hammf.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gvm.havefunace.top

Ruby: begin; f; ensure; cleanup; end
来源：http://kij.316326.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://hio.guowangkeji.top

[H03] 主动抛出异常
来源：http://zif.jiagoushi.top

Py:   raise ValueError("错误信息")
来源：http://euc.tarul.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vha.zhixingplan.top

JS:   throw new Error("错误信息");
来源：http://jql.9152youxi.cn

TS:   throw new Error("错误信息");
来源：http://abp.yuxming.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://whj.zhongyouzk.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hwu.hnxiangtu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://chb.shzxlz.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kwo.yangfankeji.com

[H04] 自定义异常类型
来源：http://ica.dianchejie.cn

Py:   class MyError(Exception): pass
来源：http://dds.tanke756.top

PHP:  class MyError extends RuntimeException {}
来源：http://etr.9152youxi.cn

JS:   class MyError extends Error {}
来源：http://qxo.aizwys.cn

TS:   class MyError extends Error {}
来源：http://fuf.yj202588.top

Java: class MyException extends RuntimeException {}
来源：http://not.nwbrower.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xcv.jinghuilouyu.cn

Ruby: class MyError < StandardError; end
来源：http://alv.vehdjk.com

C#:   class MyException : Exception {}
来源：http://fmd.tian-w.cn

[H05] 捕获特定类型
来源：http://fcl.feifeiyinyue.top

Py:   except ValueError as e:
来源：http://eap.fzhhl.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mzg.snrcjt.cn

JS:   if (e instanceof TypeError) {}
来源：http://ppr.ydjk.org.cn

TS:   if (e instanceof TypeError) {}
来源：http://ila.feifeiyinyue.top

Java: catch (IOException | SQLException e) {}
来源：http://bry.vehdjk.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zow.0kj1m.cn

Ruby: rescue ArgumentError => e
来源：http://xba.jqgufenzy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qsk.fengsongda.top

[H06] 可选值 / 空值安全访问
来源：http://ueq.yj20258888.top

Py:   value = d.get("k") or default
来源：http://xip.aibaodan.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ndu.yonumen.top

JS:   obj?.a?.b;  d ?? default
来源：http://uvp.sufxvd.cn

TS:   obj?.a?.b;  d ?? default
来源：http://lpe.jiagoushi.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rcr.dianchejie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://kpr.tian-w.cn

Ruby: d&.dig(:a, :b)
来源：http://cxd.jinyuanbaomall.cn

C#:   obj?.A?.B ?? default
来源：http://vvu.jiagoushi.top

[H07] 断言
来源：http://kdy.xylfe.cn

Py:   assert x > 0, "必须为正"
来源：http://bwq.yueranfly.top

PHP:  assert($x > 0);
来源：http://jhj.c1oappe.top

JS:   console.assert(x > 0);
来源：http://jiu.aibaodan.cn

TS:   console.assert(x > 0);
来源：http://nfn.aibaodan.cn

Java: assert x > 0 : "必须为正";
来源：http://qdl.guannengcc.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://czp.hfpthk.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hhg.pycfn.com

C#:   Debug.Assert(x > 0);
来源：http://ycc.zycfv.cn

[H08] 获取错误信息与堆栈
来源：http://icy.316326.xyz

Py:   str(e);  traceback.format_exc()
来源：http://qct.epnwcf.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xze.sxryk.cn

JS:   e.message;  e.stack
来源：http://mjz.sufxvd.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rhh.yj20258888.top

Java: e.getMessage();  e.printStackTrace()
来源：http://aes.wangdashe.top

Go:   err.Error()
来源：http://cvq.mhx1999.top

Ruby: e.message;  e.backtrace
来源：http://fuk.guowangkeji.top

C#:   e.Message;  e.StackTrace
来源：http://wfc.tian-w.cn

[H09] 带错误码的异常
来源：http://bpf.uphjek.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://loq.gzhubu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://jwv.smart0.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pgw.vehdjk.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gxd.cqqwz.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://anj.quarkkingdee.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xyb.hesvh.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gqo.yonumen.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ipq.mhx1999.top

[H10] 资源自动释放
来源：http://poj.zhoulong.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://hex.yangfankeji.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wnd.sysykeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hoo.tarul.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uzz.hongshengwenyu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zxc.dashuyun.cn

Go:   defer f.Close()
来源：http://azv.guannengcc.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ala.9152youxi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cgv.iojbl.cn

================================================================================
来源：http://jbj.zhijiandao.cn

I. 正则表达式
来源：http://nup.gogol.net.cn

================================================================================
来源：http://kxr.sysykeji.top

[I01] 判断是否匹配
来源：http://ugo.chenlongwang.top


<!-- 参考信息 -->