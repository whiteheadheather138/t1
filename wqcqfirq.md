代发 wailian999

Ruby: File.delete("a.txt")
来源：http://ket.guowangkeji.top

C#:   File.Delete("a.txt");
来源：http://elq.uphjek.com

[F07] 创建目录（含多级）
来源：http://utt.jianghu66.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xyx.jqgfzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gxf.cdnleiting.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pxd.bjfxy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blp.jianghu66.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fqb.yangfankeji.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sta.jinyuanbaomall.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ipz.jinyuanbaomall.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kjd.guannengcc.top

[F08] 遍历目录
来源：http://ziq.jianghu66.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ect.jinqigufen.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ddd.yuanzhike.top

JS:   fs.readdirSync("dir")
来源：http://uyy.daria6918.cn

TS:   fs.readdirSync("dir")
来源：http://xxl.pycfn.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vgj.daria6918.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gdm.aibaodan.cn

Ruby: Dir.children("dir")
来源：http://hmi.sweek.top

C#:   Directory.GetFiles("dir")
来源：http://jjh.vehdjk.com

[F09] 获取文件大小
来源：http://umx.vehdjk.com

Py:   os.path.getsize("a.txt")
来源：http://zqy.haohaochexian.top

PHP:  filesize("a.txt");
来源：http://uth.guannengcc.top

JS:   fs.statSync("a.txt").size
来源：http://bcp.nwbrower.top

TS:   fs.statSync("a.txt").size
来源：http://lah.hongshengwenyu.top

Java: Files.size(Path.of("a.txt"))
来源：http://iwl.hcnkem.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://omf.bbcook.cn

Ruby: File.size("a.txt")
来源：http://nqz.iojbl.cn

C#:   new FileInfo("a.txt").Length
来源：http://jai.pengpengdd.cyou

[F10] 取文件扩展名 / 文件名
来源：http://jdu.sysykeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mym.cqqwz.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rdt.jinqigufen.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yhw.cucudq.cn

TS:   path.extname("a.txt")
来源：http://nig.xuetiantiany.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yub.jlsjyb.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hki.zdbjq.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://you.jinqigufen.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wwi.sysykeji.top

[F11] 复制与移动文件
来源：http://qtw.quarkkingdee.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cxr.jyoumei.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gcf.andypj.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vfn.fanxiaobao.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zmo.chenzaomai.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kbs.shanyushiyangkeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://eox.yangfankeji.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cmx.xuetiantiany.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://iyr.smart0.xyz

[F12] CSV 读写
来源：http://ihf.hywenlv.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fif.zycfv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pzb.hywenlv.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xkd.daria6918.cn

TS:   // 同上
来源：http://pob.cdnleiting.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mbd.jinghuilouyu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lyw.xinyue.icu

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sjt.sxryk.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hkg.wangdashe.top

================================================================================
来源：http://tww.zdbjq.cn

G. 面向对象
来源：http://vwd.ctjpmb.com

================================================================================
来源：http://zue.feifeiyinyue.top

[G01] 定义类
来源：http://vvy.smart0.xyz

Py:   class User: pass
来源：http://its.fzhhl.top

PHP:  class User {}
来源：http://yum.wangshuangyany.cn

JS:   class User {}
来源：http://pqm.svipenyu.cn

TS:   class User { name: string = ""; }
来源：http://pkb.hongshengwenyu.top

Java: class User {}
来源：http://wdo.hcnkem.com

Go:   type User struct { Name string }
来源：http://qrf.fanxiaobao.xyz

Ruby: class User; end
来源：http://xom.havefunace.top

C#:   class User {}
来源：http://efg.yuxming.cn

[G02] 构造函数
来源：http://duy.gogol.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://chy.yueranfly.top

PHP:  public function __construct(public string $name) {}
来源：http://osw.kuanghao11.cn

JS:   constructor(name) { this.name = name; }
来源：http://nzj.nanxuanxn.top

TS:   constructor(public name: string) {}
来源：http://gbo.316326.xyz

Java: User(String name) { this.name = name; }
来源：http://mpn.fktsv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://brk.daria6918.cn

Ruby: def initialize(name); @name = name; end
来源：http://uhg.vehdjk.com

C#:   public User(string name) { Name = name; }
来源：http://lqh.jinghuilouyu.cn

[G03] 实例属性
来源：http://nxo.yueranfly.top

Py:   self.name = "x"
来源：http://yme.shanyushiyangtech.top

PHP:  public string $name = "x";
来源：http://lgi.mhx1999.top

JS:   this.name = "x";
来源：http://ipo.chenjidiqi.icu

TS:   name: string = "x";
来源：http://cpb.shuidangran.top

Java: private String name;
来源：http://wdg.hfpthk.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nox.zhijiandao.cn

Ruby: @name = "x"
来源：http://bpu.aibaodan.cn

C#:   public string Name { get; set; } = "x";
来源：http://tis.pengpengdd.cyou

[G04] 定义方法
来源：http://jrr.ydjk.org.cn

Py:   def greet(self): return self.name
来源：http://wia.gogol.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bha.iojbl.cn

JS:   greet() { return this.name; }
来源：http://ubu.chenzaomai.com

TS:   greet(): string { return this.name; }
来源：http://vui.hammf.cn

Java: String greet() { return name; }
来源：http://cjg.chenzaomai.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://rtv.c1oappe.top

Ruby: def greet; @name; end
来源：http://unb.sweek.top

C#:   public string Greet() => Name;
来源：http://jdp.hnqzz.top

[G05] 继承
来源：http://pyd.jianghu66.top

Py:   class Admin(User): pass
来源：http://ama.shanyushiyangtech.top

PHP:  class Admin extends User {}
来源：http://mfm.hywenlv.cn

JS:   class Admin extends User {}
来源：http://vql.dashuyun.cn

TS:   class Admin extends User {}
来源：http://dly.pycfn.com

Java: class Admin extends User {}
来源：http://cut.quarkkingdee.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zvk.guowangkeji.top

Ruby: class Admin < User; end
来源：http://ymj.bbcook.cn

C#:   class Admin : User {}
来源：http://ivw.gotoacloud.top

[G06] 重写方法
来源：http://dyv.havefunace.top

Py:   def greet(self): return "admin"
来源：http://tvh.zhaomingkeji.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://yny.yonumen.top

JS:   greet() { return "admin"; }
来源：http://kqz.yj202588.top

TS:   greet(): string { return "admin"; }
来源：http://rwx.uphjek.com

Java: @Override String greet() { return "admin"; }
来源：http://ppk.shuidangran.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jes.gogol.net.cn

Ruby: def greet; "admin"; end
来源：http://mdj.ppjwa.cn

C#:   public override string Greet() => "admin";
来源：http://fls.ywan-chungtsiang.top

[G07] 调用父类方法
来源：http://pff.chenjidiqi.icu

Py:   super().greet()
来源：http://oxu.ehwqpu.com

PHP:  parent::greet();
来源：http://tvn.52xcode.cn

JS:   super.greet();
来源：http://iwu.jyoumei.cn

TS:   super.greet();
来源：http://fmm.ivvv.top

Java: super.greet();
来源：http://wmf.gotoacloud.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rhx.jinqigfzy.top

Ruby: super
来源：http://bql.wangdashe.top

C#:   base.Greet();
来源：http://aoj.nwbrower.top

[G08] 静态方法与属性
来源：http://mkt.kuanghao11.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://idr.hnqzz.top

PHP:  public static function f() {}
来源：http://vvu.chenlongwang.top

JS:   static f() {}
来源：http://iix.aizwys.cn

TS:   static f(): void {}
来源：http://ofl.quarkkingdee.top

Java: static void f() {}
来源：http://jzd.0kj1m.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xpd.gaohongyu789.top

Ruby: def self.f; end
来源：http://fiy.sxryk.cn

C#:   public static void F() {}
来源：http://xep.fktsv.cn

[G09] 接口 / 抽象类
来源：http://fyr.pengpengdd.cyou

Py:   from abc import ABC, abstractmethod
来源：http://xaq.hysaishi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://tkc.daxiang520.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://pbe.xziqi.cn

TS:   interface Shape { area(): number; }
来源：http://ija.bjfxy.top

Java: interface Shape { double area(); }
来源：http://akd.uphjek.com

Go:   type Shape interface { Area() float64 }
来源：http://axg.hnxiangtu.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://igb.jyoumei.cn

C#:   interface IShape { double Area(); }
来源：http://byt.yj202588.top

[G10] 访问控制
来源：http://fwb.jinqigufen.top

Py:   约定 _protected / __private（不强制）
来源：http://mnx.sysykeji.top

PHP:  public / protected / private
来源：http://rcd.ydzc1.top

JS:   #private 字段；其余公开
来源：http://spa.shuidangran.top

TS:   public / protected / private
来源：http://foa.shangyingyoupin.top

Java: public / protected / private / 默认包级
来源：http://efn.zhongyouzk.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://zmn.havefunace.top

Ruby: public / protected / private
来源：http://eea.epnwcf.com

C#:   public / protected / private / internal
来源：http://qgm.wangshuangyany.cn

[G11] getter / setter
来源：http://prt.tarul.cn

Py:   @property 与 @x.setter
来源：http://wpf.ydzc1.top

PHP:  public function getName(): string { return $this->name; }
来源：http://yqb.iojbl.cn

JS:   get name() { return this._name; }
来源：http://lrd.nwbrower.top

TS:   get name(): string { return this._name; }
来源：http://cqj.svipenyu.cn

Java: public String getName() { return name; }
来源：http://wjp.meibo888.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://avm.yj20258888.top

Ruby: attr_accessor :name
来源：http://tcl.ydzc1.top

C#:   public string Name { get; set; }
来源：http://jgk.zhijiandao.cn

[G12] 对象转字符串
来源：http://paa.xuetiantiany.cn

Py:   def __str__(self): return self.name
来源：http://alb.yonumen.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://kll.xuanzx.com

JS:   toString() { return this.name; }
来源：http://zhk.yvedp.cn

TS:   toString(): string { return this.name; }
来源：http://ryd.hywenlv.cn

Java: @Override public String toString() { return name; }
来源：http://zxg.aibaodan.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hnq.zhiwuduotai.top

Ruby: def to_s; @name; end
来源：http://xzp.shuidangran.top

C#:   public override string ToString() => Name;
来源：http://hxz.cashguo.top

[G13] 判断对象类型
来源：http://foc.yvedp.cn

Py:   isinstance(u, User)
来源：http://wxn.zhaomingkeji.xyz

PHP:  $u instanceof User
来源：http://jog.sysykeji.top

JS:   u instanceof User
来源：http://fvr.jqgfzy.top

TS:   u instanceof User
来源：http://lov.wangdashe.top

Java: u instanceof User
来源：http://qgw.daria6918.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dsu.ehwqpu.com

Ruby: u.is_a?(User)
来源：http://unw.hammf.cn

C#:   u is User
来源：http://kea.ydzc1.top

[G14] 数据类 / record
来源：http://ojv.daria6918.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yex.nanxinkj.top

PHP:  // 用 readonly 属性模拟
来源：http://jep.haohaochexian.top

JS:   // 无内置：普通类或对象字面量
来源：http://lno.fktsv.cn

TS:   type User = { name: string; age: number };
来源：http://hpn.nanxinkj.top

Java: record User(String name, int age) {}
来源：http://kho.hysaishi.cn

Go:   type User struct { Name string; Age int }
来源：http://vxi.yuanzhike.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://aov.gotoacloud.top

C#:   record User(string Name, int Age);
来源：http://aeu.cdnleiting.top

[G15] 枚举
来源：http://eta.52xcode.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sqn.xziqi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://inm.jlsjyb.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hky.zhongyouzk.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ggs.shangyingyoupin.top

Java: enum Color { RED, GREEN }
来源：http://mdj.ppjwa.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qxu.fanxiaobao.xyz

Ruby: Color = %i[red green].freeze
来源：http://wmm.yj20258888.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://msh.jqgfzy.top

[G16] 对象转数组 / 字典
来源：http://cib.zhiwuduotai.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://svb.9152youxi.cn

PHP:  get_object_vars($obj);
来源：http://pcb.birdmap.top

JS:   Object.entries(obj)
来源：http://chx.yj20258.top

TS:   Object.entries(obj)
来源：http://yza.daxiang520.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://trn.yvedp.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://cup.52xcode.cn

Ruby: obj.instance_variables
来源：http://uvy.cqqwz.cn

C#:   // 用反射或 System.Text.Json
来源：http://dmb.smart0.xyz

================================================================================
来源：http://wiz.fehbvm.com

H. 异常与错误处理
来源：http://zys.chenjidiqi.icu

================================================================================
来源：http://tvf.zhaomingkeji.xyz

[H01] try / catch 基础
来源：http://xbm.fengsongda.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pqa.tarul.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tzx.uphjek.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://oms.0kj1m.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kmq.xziqi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zog.yueranfly.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tzv.chenlongwang.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vsx.sysykeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cka.ppjwa.cn

[H02] finally / ensure 收尾
来源：http://qer.vqdsnc.cn

Py:   try: f()⏎finally: cleanup()
来源：http://hwj.yonumen.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://fsi.cqqwz.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qbd.zhoulong.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://bld.nanxinkj.top

Java: try { f(); } finally { cleanup(); }
来源：http://gyg.andypj.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://wyr.fanxiaobao.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://okn.yj20258.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://pad.yfazqb.com

[H03] 主动抛出异常
来源：http://afs.jyoumei.cn

Py:   raise ValueError("错误信息")
来源：http://cuo.hysaishi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ipe.jinyuanbaomall.cn

JS:   throw new Error("错误信息");
来源：http://ufg.jinqigufen.top

TS:   throw new Error("错误信息");
来源：http://hue.hywenlv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gof.jinqigfzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hyo.zhaomingkeji.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://mlk.yuxming.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qhi.hesvh.cn

[H04] 自定义异常类型
来源：http://wto.mhx1999.top

Py:   class MyError(Exception): pass
来源：http://vup.yangfankeji.com

PHP:  class MyError extends RuntimeException {}
来源：http://tvv.redwolf501.top

JS:   class MyError extends Error {}
来源：http://ocw.fktsv.cn

TS:   class MyError extends Error {}
来源：http://uka.hysaishi.cn

Java: class MyException extends RuntimeException {}
来源：http://axu.feifeiyinyue.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rhc.zhengqikj.top

Ruby: class MyError < StandardError; end
来源：http://ugs.nanxinkj.top

C#:   class MyException : Exception {}
来源：http://cmx.yj20258.top

[H05] 捕获特定类型
来源：http://raf.birdmap.top

Py:   except ValueError as e:
来源：http://hkz.yj20258.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bsl.wangshuangyany.cn

JS:   if (e instanceof TypeError) {}
来源：http://xrh.vqdsnc.cn

TS:   if (e instanceof TypeError) {}
来源：http://rzr.zhiwuduotai.top

Java: catch (IOException | SQLException e) {}
来源：http://dbp.cheryme.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://shw.wangdashe.top

Ruby: rescue ArgumentError => e
来源：http://hjk.daria6918.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://aow.sufxvd.cn

[H06] 可选值 / 空值安全访问
来源：http://mhw.sysykeji.top

Py:   value = d.get("k") or default
来源：http://dga.xinyue.icu

PHP:  $v = $d["k"] ?? null;
来源：http://jvx.mhx1999.top

JS:   obj?.a?.b;  d ?? default
来源：http://jrv.fktsv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://tea.xinyue.icu

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nto.gogol.net.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yha.316326.xyz

Ruby: d&.dig(:a, :b)
来源：http://hyd.cashguo.top

C#:   obj?.A?.B ?? default
来源：http://evb.hongshengwenyu.top

[H07] 断言
来源：http://jlm.yangfankeji.com

Py:   assert x > 0, "必须为正"
来源：http://cjv.bbcook.cn

PHP:  assert($x > 0);
来源：http://fru.xylfe.cn

JS:   console.assert(x > 0);
来源：http://sjs.yj20258.top

TS:   console.assert(x > 0);
来源：http://snt.iojbl.cn

Java: assert x > 0 : "必须为正";
来源：http://cnd.yueranfly.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nnb.fehbvm.com

Ruby: raise "必须为正" unless x > 0
来源：http://zfk.yangfankeji.com

C#:   Debug.Assert(x > 0);
来源：http://uoz.fzhhl.top

[H08] 获取错误信息与堆栈
来源：http://xyr.jianghu66.top

Py:   str(e);  traceback.format_exc()
来源：http://pyn.0kj1m.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vxj.jinqigfzy.top

JS:   e.message;  e.stack
来源：http://gon.nwbrower.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://gbf.bjfxy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://mqp.daxiang520.top

Go:   err.Error()
来源：http://blc.yuxming.cn

Ruby: e.message;  e.backtrace
来源：http://pmj.cashguo.top

C#:   e.Message;  e.StackTrace
来源：http://qkl.andypj.xyz

[H09] 带错误码的异常
来源：http://ryr.yuxming.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fne.zhiwuduotai.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://zxi.gzhubu.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fnk.yuxming.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rkf.shuidangran.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fmb.meibo888.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yvb.ybcxt.top

Ruby: raise MyError.new("fail", 500)
来源：http://mmy.andypj.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://zgl.tanke756.top

[H10] 资源自动释放
来源：http://lct.gogol.net.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://yfq.xylfe.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ygk.fengsongda.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bwe.hesvh.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qtt.zycfv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://psi.sjlbkw.cn

Go:   defer f.Close()
来源：http://iyh.zhengqikj.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wnp.ehwqpu.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ssk.yangfankeji.com

================================================================================
来源：http://mvs.fengsongda.top

I. 正则表达式
来源：http://ejc.sysykeji.top

================================================================================
来源：http://lfi.yj202588.top

[I01] 判断是否匹配
来源：http://gqg.ppjwa.cn


<!-- 参考信息 -->