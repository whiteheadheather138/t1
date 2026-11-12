代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://rll.nanxuanxn.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gna.xingfuxueyuan.xyz

JS:   fs.readdirSync("dir")
来源：http://pui.ywan-chungtsiang.top

TS:   fs.readdirSync("dir")
来源：http://fwi.nwbrower.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wdk.yangfankeji.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://oay.zhiwuduotai.top

Ruby: Dir.children("dir")
来源：http://aps.yj202588.top

C#:   Directory.GetFiles("dir")
来源：http://mou.vqdsnc.cn

[F09] 获取文件大小
来源：http://ntg.shangyingyoupin.top

Py:   os.path.getsize("a.txt")
来源：http://ziy.cheryme.top

PHP:  filesize("a.txt");
来源：http://mxm.uphjek.com

JS:   fs.statSync("a.txt").size
来源：http://bjo.yangfankeji.com

TS:   fs.statSync("a.txt").size
来源：http://yjb.vqdsnc.cn

Java: Files.size(Path.of("a.txt"))
来源：http://som.uphjek.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tgv.zhongyouzk.top

Ruby: File.size("a.txt")
来源：http://ksj.gaohongyu789.top

C#:   new FileInfo("a.txt").Length
来源：http://gyl.jinyuanbaomall.cn

[F10] 取文件扩展名 / 文件名
来源：http://zqx.sysykeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fdp.hfpthk.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uir.ydzc1.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wut.xingfuxueyuan.xyz

TS:   path.extname("a.txt")
来源：http://llg.yuxming.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bhq.gotoacloud.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ewf.yuanzhike.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://emd.svipenyu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rsd.ywan-chungtsiang.top

[F11] 复制与移动文件
来源：http://qwi.tianlin.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fti.zhiwuduotai.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ssk.ywan-chungtsiang.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kqz.yj20258888.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dbr.zhoulong.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tlu.ywan-chungtsiang.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lhl.hysaishi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hmc.cucudq.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ybc.fehbvm.com

[F12] CSV 读写
来源：http://lyz.shuidangran.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jie.bjfxy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://txn.zhaomingkeji.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://oox.wangdashe.top

TS:   // 同上
来源：http://bcx.cqqwz.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cor.hesvh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fli.zhongyouzk.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dfj.svipenyu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ubj.52xcode.cn

================================================================================
来源：http://ubt.havefunace.top

G. 面向对象
来源：http://dqj.chenjidiqi.icu

================================================================================
来源：http://mce.yj202588.top

[G01] 定义类
来源：http://yny.ehwqpu.com

Py:   class User: pass
来源：http://wim.sjlbkw.cn

PHP:  class User {}
来源：http://nxx.hfpthk.cn

JS:   class User {}
来源：http://irj.zhijiandao.cn

TS:   class User { name: string = ""; }
来源：http://gnd.xuanzx.com

Java: class User {}
来源：http://yin.cucudq.cn

Go:   type User struct { Name string }
来源：http://hnf.gotoacloud.top

Ruby: class User; end
来源：http://pqd.quarkkingdee.top

C#:   class User {}
来源：http://dwp.cqqwz.cn

[G02] 构造函数
来源：http://efc.aibaodan.cn

Py:   def __init__(self, name): self.name = name
来源：http://jol.hcnkem.com

PHP:  public function __construct(public string $name) {}
来源：http://aht.ivvv.top

JS:   constructor(name) { this.name = name; }
来源：http://ayc.haohaochexian.top

TS:   constructor(public name: string) {}
来源：http://yby.jlsjyb.cn

Java: User(String name) { this.name = name; }
来源：http://yub.yangfankeji.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://snx.ydjk.org.cn

Ruby: def initialize(name); @name = name; end
来源：http://fyg.bbcook.cn

C#:   public User(string name) { Name = name; }
来源：http://pkz.hnxiangtu.top

[G03] 实例属性
来源：http://hcr.gzhubu.top

Py:   self.name = "x"
来源：http://mqm.cucudq.cn

PHP:  public string $name = "x";
来源：http://rly.quarkkingdee.top

JS:   this.name = "x";
来源：http://ijk.xingfuxueyuan.xyz

TS:   name: string = "x";
来源：http://dzq.xziqi.cn

Java: private String name;
来源：http://xii.xuetiantiany.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://adc.cdnleiting.top

Ruby: @name = "x"
来源：http://qqh.gzhubu.top

C#:   public string Name { get; set; } = "x";
来源：http://aww.sjlbkw.cn

[G04] 定义方法
来源：http://gse.fanxiaobao.xyz

Py:   def greet(self): return self.name
来源：http://qvi.epnwcf.com

PHP:  public function greet(): string { return $this->name; }
来源：http://cxl.guannengcc.top

JS:   greet() { return this.name; }
来源：http://ucj.chenzaomai.com

TS:   greet(): string { return this.name; }
来源：http://bak.svipenyu.cn

Java: String greet() { return name; }
来源：http://gvn.ehwqpu.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://mrg.yangfankeji.com

Ruby: def greet; @name; end
来源：http://tqp.ywan-chungtsiang.top

C#:   public string Greet() => Name;
来源：http://btq.meibo888.top

[G05] 继承
来源：http://ibh.yongpay.top

Py:   class Admin(User): pass
来源：http://oqc.ehwqpu.com

PHP:  class Admin extends User {}
来源：http://cfd.fzhhl.top

JS:   class Admin extends User {}
来源：http://anj.hnqzz.top

TS:   class Admin extends User {}
来源：http://owm.yvedp.cn

Java: class Admin extends User {}
来源：http://adp.zhengqikj.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ibb.shanyushiyangkeji.top

Ruby: class Admin < User; end
来源：http://shs.guowangkeji.top

C#:   class Admin : User {}
来源：http://khg.yj20258888.top

[G06] 重写方法
来源：http://xrm.nwbrower.top

Py:   def greet(self): return "admin"
来源：http://esy.chenlongwang.top

PHP:  public function greet(): string { return "admin"; }
来源：http://cub.0kj1m.cn

JS:   greet() { return "admin"; }
来源：http://olu.jiagoushi.top

TS:   greet(): string { return "admin"; }
来源：http://bac.uphjek.com

Java: @Override String greet() { return "admin"; }
来源：http://etr.hesvh.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rvh.jianghu66.top

Ruby: def greet; "admin"; end
来源：http://ban.quarkkingdee.top

C#:   public override string Greet() => "admin";
来源：http://ghu.9152youxi.cn

[G07] 调用父类方法
来源：http://yrb.tian-w.cn

Py:   super().greet()
来源：http://iip.snrcjt.cn

PHP:  parent::greet();
来源：http://nno.sjlbkw.cn

JS:   super.greet();
来源：http://vjy.jiagoushi.top

TS:   super.greet();
来源：http://fyd.wangshuangyany.cn

Java: super.greet();
来源：http://wmg.ivvv.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bly.yj20258.top

Ruby: super
来源：http://jii.shuidangran.top

C#:   base.Greet();
来源：http://aaj.cheryme.top

[G08] 静态方法与属性
来源：http://cbq.sufxvd.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://aqi.uphjek.com

PHP:  public static function f() {}
来源：http://lji.sweek.top

JS:   static f() {}
来源：http://deq.tian-w.cn

TS:   static f(): void {}
来源：http://bfl.jinqigfzy.top

Java: static void f() {}
来源：http://ghc.yanxiufei.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zts.gzhubu.top

Ruby: def self.f; end
来源：http://szf.yangfankeji.com

C#:   public static void F() {}
来源：http://fjb.yj20258.top

[G09] 接口 / 抽象类
来源：http://wkn.zycfv.cn

Py:   from abc import ABC, abstractmethod
来源：http://aks.jianghu66.top

PHP:  interface Shape { public function area(): float; }
来源：http://gux.fengsongda.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://qph.zdqjudy.top

TS:   interface Shape { area(): number; }
来源：http://tmk.xziqi.cn

Java: interface Shape { double area(); }
来源：http://ycc.sjlbkw.cn

Go:   type Shape interface { Area() float64 }
来源：http://fyh.pengpengdd.cyou

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rdn.yj20258888.top

C#:   interface IShape { double Area(); }
来源：http://jhx.nanxuanxn.top

[G10] 访问控制
来源：http://jzj.cheryme.top

Py:   约定 _protected / __private（不强制）
来源：http://nud.9152youxi.cn

PHP:  public / protected / private
来源：http://hmn.sweek.top

JS:   #private 字段；其余公开
来源：http://ohq.uphjek.com

TS:   public / protected / private
来源：http://mjp.nanxuanxn.top

Java: public / protected / private / 默认包级
来源：http://fvs.dashuyun.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ecn.zdbjq.cn

Ruby: public / protected / private
来源：http://tci.nanxinkj.top

C#:   public / protected / private / internal
来源：http://jad.xingfuxueyuan.xyz

[G11] getter / setter
来源：http://oqa.ivvv.top

Py:   @property 与 @x.setter
来源：http://bgo.bjfxy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://slc.shanyushiyangkeji.top

JS:   get name() { return this._name; }
来源：http://cyk.pycfn.com

TS:   get name(): string { return this._name; }
来源：http://xun.andypj.xyz

Java: public String getName() { return name; }
来源：http://rnm.ydjk.org.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tmd.chenlongwang.top

Ruby: attr_accessor :name
来源：http://cqv.dianchejie.cn

C#:   public string Name { get; set; }
来源：http://yjt.gotoacloud.top

[G12] 对象转字符串
来源：http://uud.jianghu66.top

Py:   def __str__(self): return self.name
来源：http://sta.pengpengdd.cyou

PHP:  public function __toString(): string { return $this->name; }
来源：http://kvk.ydjk.org.cn

JS:   toString() { return this.name; }
来源：http://zme.c1oappe.top

TS:   toString(): string { return this.name; }
来源：http://bbu.cqqwz.cn

Java: @Override public String toString() { return name; }
来源：http://tbc.cdnleiting.top

Go:   func (u User) String() string { return u.Name }
来源：http://ujs.andypj.xyz

Ruby: def to_s; @name; end
来源：http://ulm.bjfxy.top

C#:   public override string ToString() => Name;
来源：http://gdf.hnxiangtu.top

[G13] 判断对象类型
来源：http://pwh.zhengqikj.top

Py:   isinstance(u, User)
来源：http://tnj.jinqigfzy.top

PHP:  $u instanceof User
来源：http://xfe.daxiang520.top

JS:   u instanceof User
来源：http://wbq.zhongyouzk.top

TS:   u instanceof User
来源：http://pas.jyoumei.cn

Java: u instanceof User
来源：http://uoy.yuanzhike.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://gyv.xziqi.cn

Ruby: u.is_a?(User)
来源：http://pns.yanxiufei.cn

C#:   u is User
来源：http://vyz.aibaodan.cn

[G14] 数据类 / record
来源：http://cxa.zhaomingkeji.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uae.9152youxi.cn

PHP:  // 用 readonly 属性模拟
来源：http://hzp.c1oappe.top

JS:   // 无内置：普通类或对象字面量
来源：http://rhv.gotoacloud.top

TS:   type User = { name: string; age: number };
来源：http://opy.ehwqpu.com

Java: record User(String name, int age) {}
来源：http://dip.hcnkem.com

Go:   type User struct { Name string; Age int }
来源：http://rqy.hywenlv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rri.tarul.cn

C#:   record User(string Name, int Age);
来源：http://chf.ctjpmb.com

[G15] 枚举
来源：http://uza.zhaomingkeji.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://aoe.tarul.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xwb.gzhubu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ztu.316326.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pqf.zdbjq.cn

Java: enum Color { RED, GREEN }
来源：http://lzl.sysykeji.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wop.sysykeji.top

Ruby: Color = %i[red green].freeze
来源：http://lem.yvedp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yiy.chenzaomai.com

[G16] 对象转数组 / 字典
来源：http://ghm.xuanzx.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rcm.jinyuanbaomall.cn

PHP:  get_object_vars($obj);
来源：http://gfx.yuxming.cn

JS:   Object.entries(obj)
来源：http://vkc.yanxiufei.cn

TS:   Object.entries(obj)
来源：http://tiq.fktsv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ebb.guannengcc.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://xmi.mhx1999.top

Ruby: obj.instance_variables
来源：http://rkx.zdbjq.cn

C#:   // 用反射或 System.Text.Json
来源：http://uka.epnwcf.com

================================================================================
来源：http://fpt.yonumen.top

H. 异常与错误处理
来源：http://uwn.feifeiyinyue.top

================================================================================
来源：http://lrg.aizwys.cn

[H01] try / catch 基础
来源：http://jwe.yj20258888.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://atw.c1oappe.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cds.shangyingyoupin.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ehx.sysykeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hlx.pengpengdd.cyou

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://exu.shuidangran.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qgj.ywan-chungtsiang.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://spm.jinghuilouyu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vda.jinqigufen.top

[H02] finally / ensure 收尾
来源：http://xwr.bjfxy.top

Py:   try: f()⏎finally: cleanup()
来源：http://xjh.ywan-chungtsiang.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://feh.shangyingyoupin.top

JS:   try { f(); } finally { cleanup(); }
来源：http://iic.svipenyu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://wqj.yvedp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://cwh.shanyushiyangtech.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ojj.52xcode.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://znl.ywan-chungtsiang.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://jye.jinyuanbaomall.cn

[H03] 主动抛出异常
来源：http://dul.zhixingplan.top

Py:   raise ValueError("错误信息")
来源：http://iod.fzhhl.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fpj.ydjk.org.cn

JS:   throw new Error("错误信息");
来源：http://rfl.ctjpmb.com

TS:   throw new Error("错误信息");
来源：http://dkp.fktsv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ocs.hywenlv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dnu.zhongyouzk.top

Ruby: raise ArgumentError, "错误信息"
来源：http://pvq.xinyue.icu

C#:   throw new ArgumentException("错误信息");
来源：http://wla.daria6918.cn

[H04] 自定义异常类型
来源：http://nkg.sufxvd.cn

Py:   class MyError(Exception): pass
来源：http://gps.cheryme.top

PHP:  class MyError extends RuntimeException {}
来源：http://azy.vehdjk.com

JS:   class MyError extends Error {}
来源：http://dii.ehwqpu.com

TS:   class MyError extends Error {}
来源：http://ebz.cashguo.top

Java: class MyException extends RuntimeException {}
来源：http://kus.yuanzhike.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dla.guowangkeji.top

Ruby: class MyError < StandardError; end
来源：http://vcq.zhaomingkeji.xyz

C#:   class MyException : Exception {}
来源：http://jzi.chenjidiqi.icu

[H05] 捕获特定类型
来源：http://wmf.hnqzz.top

Py:   except ValueError as e:
来源：http://qly.fktsv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rhj.c1oappe.top

JS:   if (e instanceof TypeError) {}
来源：http://dxl.quarkkingdee.top

TS:   if (e instanceof TypeError) {}
来源：http://wdw.zhengqikj.top

Java: catch (IOException | SQLException e) {}
来源：http://gky.hongshengwenyu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uqf.chenjidiqi.icu

Ruby: rescue ArgumentError => e
来源：http://qog.redwolf501.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cws.c1oappe.top

[H06] 可选值 / 空值安全访问
来源：http://yyu.ywan-chungtsiang.top

Py:   value = d.get("k") or default
来源：http://iue.xziqi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kke.hywenlv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://csw.xziqi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://nxv.jqgufenzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vds.shuidangran.top

Go:   if v, ok := m["k"]; ok { }
来源：http://nlv.wangshuangyany.cn

Ruby: d&.dig(:a, :b)
来源：http://vix.havefunace.top

C#:   obj?.A?.B ?? default
来源：http://omi.hysaishi.cn

[H07] 断言
来源：http://ajw.haohaochexian.top

Py:   assert x > 0, "必须为正"
来源：http://aqs.daxiang520.top

PHP:  assert($x > 0);
来源：http://smu.wangshuangyany.cn

JS:   console.assert(x > 0);
来源：http://fvr.sufxvd.cn

TS:   console.assert(x > 0);
来源：http://opu.cheryme.top

Java: assert x > 0 : "必须为正";
来源：http://txg.yuxming.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dfn.zhijiandao.cn

Ruby: raise "必须为正" unless x > 0
来源：http://iet.tanke756.top

C#:   Debug.Assert(x > 0);
来源：http://qdd.yj20258.top

[H08] 获取错误信息与堆栈
来源：http://psd.ehwqpu.com

Py:   str(e);  traceback.format_exc()
来源：http://rwc.hcnkem.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://omf.vehdjk.com

JS:   e.message;  e.stack
来源：http://wjt.cucudq.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tzc.smart0.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://cxt.zdqjudy.top

Go:   err.Error()
来源：http://nuv.yfazqb.com

Ruby: e.message;  e.backtrace
来源：http://wtw.ywan-chungtsiang.top

C#:   e.Message;  e.StackTrace
来源：http://kpn.xingfuxueyuan.xyz

[H09] 带错误码的异常
来源：http://dqm.hysaishi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ifn.gzhubu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://xcj.aibaodan.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mbi.zhongyouzk.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qch.meibo888.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wsn.wangdashe.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mce.fehbvm.com

Ruby: raise MyError.new("fail", 500)
来源：http://txq.jinyuanbaomall.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fez.jinqigufen.top

[H10] 资源自动释放
来源：http://dwh.hywenlv.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lzb.zdqjudy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tyg.hnxiangtu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://coe.nwbrower.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fga.sjlbkw.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wey.meibo888.top

Go:   defer f.Close()
来源：http://qnn.jlsjyb.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gyf.jqgfzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mdh.yuxming.cn

================================================================================
来源：http://cxw.yfazqb.com

I. 正则表达式
来源：http://urf.hfpthk.cn

================================================================================
来源：http://gdl.zhengqikj.top

[I01] 判断是否匹配
来源：http://ngu.jinyuanbaomall.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vzu.yueranfly.top

PHP:  preg_match('/\d+/', $s);
来源：http://zdb.gzhubu.top

JS:   /\d+/.test(s)
来源：http://nif.zhixingplan.top

TS:   /\d+/.test(s)
来源：http://rml.xziqi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pgr.cqqwz.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bka.xziqi.cn

Ruby: s.match?(/\d+/)
来源：http://dfx.cheryme.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qav.yangfankeji.com

[I02] 提取所有匹配
来源：http://fze.sysykeji.top

Py:   re.findall(r"\d+", s)
来源：http://jlg.sjlbkw.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ibn.birdmap.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kpu.zycfv.cn


<!-- 参考信息 -->