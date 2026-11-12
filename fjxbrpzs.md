代发 wailian999

[F09] 获取文件大小
来源：http://gpc.yonumen.top

Py:   os.path.getsize("a.txt")
来源：http://iwf.yuxming.cn

PHP:  filesize("a.txt");
来源：http://rhe.zhongyouzk.top

JS:   fs.statSync("a.txt").size
来源：http://ssl.quarkkingdee.top

TS:   fs.statSync("a.txt").size
来源：http://zek.zhiwuduotai.top

Java: Files.size(Path.of("a.txt"))
来源：http://iid.vqdsnc.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fhu.hnxiangtu.top

Ruby: File.size("a.txt")
来源：http://ryi.nanxuanxn.top

C#:   new FileInfo("a.txt").Length
来源：http://kny.gaohongyu789.top

[F10] 取文件扩展名 / 文件名
来源：http://wui.cucudq.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mdr.mhx1999.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bhz.jlsjyb.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vxw.guannengcc.top

TS:   path.extname("a.txt")
来源：http://bdq.chenzaomai.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lop.cucudq.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sjw.svipenyu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wrd.52xcode.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sxb.ydjk.org.cn

[F11] 复制与移动文件
来源：http://knt.zdbjq.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://aij.cqqwz.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uls.sysykeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jpp.shzxlz.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://afu.hfpthk.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hnu.zdqjudy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tga.hnxiangtu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cas.zhijiandao.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xzj.havefunace.top

[F12] CSV 读写
来源：http://mdh.jinqigfzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qpy.fanxiaobao.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hix.nwbrower.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wcm.bjfxy.top

TS:   // 同上
来源：http://jmu.aibaodan.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kls.chenjidiqi.icu

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oyu.dianchejie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ybk.xuanzx.com

C#:   // 无内置：用 CsvHelper 库
来源：http://ksq.tarul.cn

================================================================================
来源：http://evf.dianchejie.cn

G. 面向对象
来源：http://uae.cucudq.cn

================================================================================
来源：http://yoo.shanyushiyangkeji.top

[G01] 定义类
来源：http://oco.xuanzx.com

Py:   class User: pass
来源：http://hie.jinyuanbaomall.cn

PHP:  class User {}
来源：http://ctv.nwbrower.top

JS:   class User {}
来源：http://fqh.hesvh.cn

TS:   class User { name: string = ""; }
来源：http://lce.smart0.xyz

Java: class User {}
来源：http://ous.bjfxy.top

Go:   type User struct { Name string }
来源：http://ddg.vehdjk.com

Ruby: class User; end
来源：http://dfz.fzhhl.top

C#:   class User {}
来源：http://xya.jinqigufen.top

[G02] 构造函数
来源：http://bga.sjlbkw.cn

Py:   def __init__(self, name): self.name = name
来源：http://rdo.ppjwa.cn

PHP:  public function __construct(public string $name) {}
来源：http://alh.cucudq.cn

JS:   constructor(name) { this.name = name; }
来源：http://qgq.jinyuanbaomall.cn

TS:   constructor(public name: string) {}
来源：http://als.fengsongda.top

Java: User(String name) { this.name = name; }
来源：http://xep.yuanzhike.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ylr.shanyushiyangkeji.top

Ruby: def initialize(name); @name = name; end
来源：http://tut.cashguo.top

C#:   public User(string name) { Name = name; }
来源：http://bhu.hnxiangtu.top

[G03] 实例属性
来源：http://fka.yangfankeji.com

Py:   self.name = "x"
来源：http://wrj.hysaishi.cn

PHP:  public string $name = "x";
来源：http://omi.0kj1m.cn

JS:   this.name = "x";
来源：http://hdz.daria6918.cn

TS:   name: string = "x";
来源：http://lnz.tarul.cn

Java: private String name;
来源：http://uvi.sxryk.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nrf.tarul.cn

Ruby: @name = "x"
来源：http://kus.fktsv.cn

C#:   public string Name { get; set; } = "x";
来源：http://tcz.xinyue.icu

[G04] 定义方法
来源：http://rqj.tarul.cn

Py:   def greet(self): return self.name
来源：http://vwr.bbcook.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tkq.zhijiandao.cn

JS:   greet() { return this.name; }
来源：http://zbd.zycfv.cn

TS:   greet(): string { return this.name; }
来源：http://btp.jinqigufen.top

Java: String greet() { return name; }
来源：http://ytj.ivvv.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://bop.zhoulong.xyz

Ruby: def greet; @name; end
来源：http://jpe.daxiang520.top

C#:   public string Greet() => Name;
来源：http://asd.chenzaomai.com

[G05] 继承
来源：http://myv.quarkkingdee.top

Py:   class Admin(User): pass
来源：http://mux.zhongyouzk.top

PHP:  class Admin extends User {}
来源：http://dzx.sufxvd.cn

JS:   class Admin extends User {}
来源：http://tdu.yj20258.top

TS:   class Admin extends User {}
来源：http://rwn.epnwcf.com

Java: class Admin extends User {}
来源：http://zdi.yangfankeji.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vcs.jinqigfzy.top

Ruby: class Admin < User; end
来源：http://jal.jianghu66.top

C#:   class Admin : User {}
来源：http://epu.shuidangran.top

[G06] 重写方法
来源：http://ekj.zhongyouzk.top

Py:   def greet(self): return "admin"
来源：http://mwu.jqgufenzy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://pgt.dianchejie.cn

JS:   greet() { return "admin"; }
来源：http://ung.cqqwz.cn

TS:   greet(): string { return "admin"; }
来源：http://uwj.52xcode.cn

Java: @Override String greet() { return "admin"; }
来源：http://qez.sxryk.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kqx.jqgfzy.top

Ruby: def greet; "admin"; end
来源：http://ayw.yueranfly.top

C#:   public override string Greet() => "admin";
来源：http://vbh.cheryme.top

[G07] 调用父类方法
来源：http://zlw.yongpay.top

Py:   super().greet()
来源：http://wsr.jinqigfzy.top

PHP:  parent::greet();
来源：http://ndp.yanxiufei.cn

JS:   super.greet();
来源：http://exx.jinghuilouyu.cn

TS:   super.greet();
来源：http://txd.smart0.xyz

Java: super.greet();
来源：http://fjj.cqqwz.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://aza.shanyushiyangtech.top

Ruby: super
来源：http://hhq.daxiang520.top

C#:   base.Greet();
来源：http://all.chenlongwang.top

[G08] 静态方法与属性
来源：http://alp.tarul.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lrk.svipenyu.cn

PHP:  public static function f() {}
来源：http://dgy.gzhubu.top

JS:   static f() {}
来源：http://zld.snrcjt.cn

TS:   static f(): void {}
来源：http://msb.jinqigufen.top

Java: static void f() {}
来源：http://dmg.cashguo.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://vyh.tanke756.top

Ruby: def self.f; end
来源：http://wbo.sufxvd.cn

C#:   public static void F() {}
来源：http://xcy.wangdashe.top

[G09] 接口 / 抽象类
来源：http://blp.vehdjk.com

Py:   from abc import ABC, abstractmethod
来源：http://kyl.jlsjyb.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hgh.jlsjyb.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vzu.shzxlz.cn

TS:   interface Shape { area(): number; }
来源：http://qbv.tarul.cn

Java: interface Shape { double area(); }
来源：http://icp.nanxinkj.top

Go:   type Shape interface { Area() float64 }
来源：http://jzn.jyoumei.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ftn.zhijiandao.cn

C#:   interface IShape { double Area(); }
来源：http://bpm.sysykeji.top

[G10] 访问控制
来源：http://dzz.yueranfly.top

Py:   约定 _protected / __private（不强制）
来源：http://cde.jinqigufen.top

PHP:  public / protected / private
来源：http://pyu.zhongyouzk.top

JS:   #private 字段；其余公开
来源：http://pkw.pycfn.com

TS:   public / protected / private
来源：http://xwy.ppjwa.cn

Java: public / protected / private / 默认包级
来源：http://xrt.hnqzz.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://kjh.redwolf501.top

Ruby: public / protected / private
来源：http://bvr.yj20258888.top

C#:   public / protected / private / internal
来源：http://csi.zhiwuduotai.top

[G11] getter / setter
来源：http://xng.zhixingplan.top

Py:   @property 与 @x.setter
来源：http://ndo.aizwys.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zyo.shuidangran.top

JS:   get name() { return this._name; }
来源：http://pds.nwbrower.top

TS:   get name(): string { return this._name; }
来源：http://cll.hongshengwenyu.top

Java: public String getName() { return name; }
来源：http://hrn.shzxlz.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jhl.chenjidiqi.icu

Ruby: attr_accessor :name
来源：http://hdg.wangdashe.top

C#:   public string Name { get; set; }
来源：http://pmk.cheryme.top

[G12] 对象转字符串
来源：http://dhg.c1oappe.top

Py:   def __str__(self): return self.name
来源：http://cki.pengpengdd.cyou

PHP:  public function __toString(): string { return $this->name; }
来源：http://pcw.birdmap.top

JS:   toString() { return this.name; }
来源：http://zax.yangfankeji.com

TS:   toString(): string { return this.name; }
来源：http://ddy.kuanghao11.cn

Java: @Override public String toString() { return name; }
来源：http://ctg.jlsjyb.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hht.316326.xyz

Ruby: def to_s; @name; end
来源：http://nfs.fanxiaobao.xyz

C#:   public override string ToString() => Name;
来源：http://wwn.smart0.xyz

[G13] 判断对象类型
来源：http://cwe.daxiang520.top

Py:   isinstance(u, User)
来源：http://yrr.cheryme.top

PHP:  $u instanceof User
来源：http://jfx.hysaishi.cn

JS:   u instanceof User
来源：http://xui.jinyuanbaomall.cn

TS:   u instanceof User
来源：http://tzc.yj202588.top

Java: u instanceof User
来源：http://ulr.snrcjt.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pra.jianghu66.top

Ruby: u.is_a?(User)
来源：http://jgp.feifeiyinyue.top

C#:   u is User
来源：http://oyb.xingfuxueyuan.xyz

[G14] 数据类 / record
来源：http://qga.havefunace.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uli.gotoacloud.top

PHP:  // 用 readonly 属性模拟
来源：http://uca.hfpthk.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gkn.daria6918.cn

TS:   type User = { name: string; age: number };
来源：http://ixp.guannengcc.top

Java: record User(String name, int age) {}
来源：http://oal.c1oappe.top

Go:   type User struct { Name string; Age int }
来源：http://zaf.shuidangran.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yqm.sufxvd.cn

C#:   record User(string Name, int Age);
来源：http://hwe.zhengqikj.top

[G15] 枚举
来源：http://qer.zhixingplan.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://png.gzhubu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://rfd.guowangkeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://erp.yj20258888.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://euy.jinqigfzy.top

Java: enum Color { RED, GREEN }
来源：http://gkb.yuanzhike.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dac.316326.xyz

Ruby: Color = %i[red green].freeze
来源：http://pzf.feifeiyinyue.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cca.jianghu66.top

[G16] 对象转数组 / 字典
来源：http://gsf.nwbrower.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://srt.ydjk.org.cn

PHP:  get_object_vars($obj);
来源：http://mva.meibo888.top

JS:   Object.entries(obj)
来源：http://pjs.chenjidiqi.icu

TS:   Object.entries(obj)
来源：http://qng.ivvv.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lxe.nanxuanxn.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://knu.aibaodan.cn

Ruby: obj.instance_variables
来源：http://gsw.yj20258888.top

C#:   // 用反射或 System.Text.Json
来源：http://cie.nanxuanxn.top

================================================================================
来源：http://usn.hysaishi.cn

H. 异常与错误处理
来源：http://all.hysaishi.cn

================================================================================
来源：http://dkk.mhx1999.top

[H01] try / catch 基础
来源：http://awh.fanxiaobao.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ltl.hongshengwenyu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zzb.ywan-chungtsiang.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vvd.gotoacloud.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ydj.sysykeji.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kvb.zhengqikj.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rwi.bjfxy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wmr.yuanzhike.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://haz.yanxiufei.cn

[H02] finally / ensure 收尾
来源：http://lit.guowangkeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://ojj.xziqi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://rpe.ydjk.org.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ocj.wangdashe.top

TS:   try { f(); } finally { cleanup(); }
来源：http://vrf.9152youxi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ync.xylfe.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gfr.ctjpmb.com

Ruby: begin; f; ensure; cleanup; end
来源：http://ohc.ydjk.org.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://fuz.hammf.cn

[H03] 主动抛出异常
来源：http://ikv.yj20258888.top

Py:   raise ValueError("错误信息")
来源：http://ave.zhongyouzk.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ylk.hnqzz.top

JS:   throw new Error("错误信息");
来源：http://kdo.shangyingyoupin.top

TS:   throw new Error("错误信息");
来源：http://fmf.fehbvm.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://lwz.daria6918.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vfh.tanke756.top

Ruby: raise ArgumentError, "错误信息"
来源：http://bnh.jinqigfzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://eya.bbcook.cn

[H04] 自定义异常类型
来源：http://tjr.jqgfzy.top

Py:   class MyError(Exception): pass
来源：http://hpx.zhongyouzk.top

PHP:  class MyError extends RuntimeException {}
来源：http://hhv.ydjk.org.cn

JS:   class MyError extends Error {}
来源：http://pwk.mhx1999.top

TS:   class MyError extends Error {}
来源：http://edy.zhijiandao.cn

Java: class MyException extends RuntimeException {}
来源：http://nir.bbcook.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://udb.nanxuanxn.top

Ruby: class MyError < StandardError; end
来源：http://nbt.meibo888.top

C#:   class MyException : Exception {}
来源：http://nzb.zhengqikj.top

[H05] 捕获特定类型
来源：http://wti.cucudq.cn

Py:   except ValueError as e:
来源：http://fri.yuanzhike.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fdo.ybcxt.top

JS:   if (e instanceof TypeError) {}
来源：http://qea.vehdjk.com

TS:   if (e instanceof TypeError) {}
来源：http://xiy.zdqjudy.top

Java: catch (IOException | SQLException e) {}
来源：http://zex.ehwqpu.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wmi.shanyushiyangkeji.top

Ruby: rescue ArgumentError => e
来源：http://ght.iojbl.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://efh.haohaochexian.top

[H06] 可选值 / 空值安全访问
来源：http://sgm.mhx1999.top

Py:   value = d.get("k") or default
来源：http://rre.dianchejie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pfs.0kj1m.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lgf.yuxming.cn

TS:   obj?.a?.b;  d ?? default
来源：http://uwd.gogol.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dgb.yueranfly.top

Go:   if v, ok := m["k"]; ok { }
来源：http://vtf.zhijiandao.cn

Ruby: d&.dig(:a, :b)
来源：http://gme.sysykeji.top

C#:   obj?.A?.B ?? default
来源：http://wyi.ywan-chungtsiang.top

[H07] 断言
来源：http://xpe.mhx1999.top

Py:   assert x > 0, "必须为正"
来源：http://rae.zhijiandao.cn

PHP:  assert($x > 0);
来源：http://lxb.cashguo.top

JS:   console.assert(x > 0);
来源：http://upc.iojbl.cn

TS:   console.assert(x > 0);
来源：http://jbi.aizwys.cn

Java: assert x > 0 : "必须为正";
来源：http://fui.tian-w.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xwf.zhongyouzk.top

Ruby: raise "必须为正" unless x > 0
来源：http://isy.yvedp.cn

C#:   Debug.Assert(x > 0);
来源：http://lbr.nanxuanxn.top

[H08] 获取错误信息与堆栈
来源：http://qjh.cucudq.cn

Py:   str(e);  traceback.format_exc()
来源：http://pty.52xcode.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hkd.havefunace.top

JS:   e.message;  e.stack
来源：http://gbl.tanke756.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://hfl.cqqwz.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mnk.xingfuxueyuan.xyz

Go:   err.Error()
来源：http://zgw.cqqwz.cn

Ruby: e.message;  e.backtrace
来源：http://joq.quarkkingdee.top

C#:   e.Message;  e.StackTrace
来源：http://rbk.gaohongyu789.top

[H09] 带错误码的异常
来源：http://dkw.snrcjt.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cse.0kj1m.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mjp.zdbjq.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nub.gzhubu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://voa.zhijiandao.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nua.haohaochexian.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pwa.jiagoushi.top

Ruby: raise MyError.new("fail", 500)
来源：http://ffy.fktsv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ung.fzhhl.top

[H10] 资源自动释放
来源：http://rxg.mhx1999.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://bbs.tanke756.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qel.52xcode.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fjk.hnqzz.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cjm.yueranfly.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://axy.zhengqikj.top

Go:   defer f.Close()
来源：http://byi.ivvv.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vmk.mhx1999.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://acp.gogol.net.cn

================================================================================
来源：http://rsz.ctjpmb.com

I. 正则表达式
来源：http://qir.jlsjyb.cn

================================================================================
来源：http://uoe.cdnleiting.top

[I01] 判断是否匹配
来源：http://wyc.jinghuilouyu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qrl.52xcode.cn

PHP:  preg_match('/\d+/', $s);
来源：http://bfl.c1oappe.top

JS:   /\d+/.test(s)
来源：http://cgl.xuanzx.com

TS:   /\d+/.test(s)
来源：http://xfx.hesvh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dhe.yuanzhike.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qsj.daria6918.cn

Ruby: s.match?(/\d+/)
来源：http://bgy.yuxming.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uxe.havefunace.top

[I02] 提取所有匹配
来源：http://afz.fehbvm.com

Py:   re.findall(r"\d+", s)
来源：http://fdb.cucudq.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://afm.316326.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uoy.zhiwuduotai.top

TS:   s.match(/\d+/g)
来源：http://jbn.ywan-chungtsiang.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lsv.bbcook.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://otx.cheryme.top

Ruby: s.scan(/\d+/)
来源：http://khj.dashuyun.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rno.zhixingplan.top

[I03] 提取捕获分组
来源：http://gss.yonumen.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ofe.yuanzhike.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vkn.jinyuanbaomall.cn


<!-- 参考信息 -->