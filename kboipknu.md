代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ikg.sufxvd.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hup.hysaishi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wia.wangdashe.top

[F08] 遍历目录
来源：http://hiv.xuetiantiany.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://dxi.fanxiaobao.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uyd.nwbrower.top

JS:   fs.readdirSync("dir")
来源：http://xwj.dashuyun.cn

TS:   fs.readdirSync("dir")
来源：http://lkw.cheryme.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xuv.yuanzhike.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zcb.ywan-chungtsiang.top

Ruby: Dir.children("dir")
来源：http://egx.dianchejie.cn

C#:   Directory.GetFiles("dir")
来源：http://wgl.sjlbkw.cn

[F09] 获取文件大小
来源：http://vnf.zdbjq.cn

Py:   os.path.getsize("a.txt")
来源：http://mqf.yanxiufei.cn

PHP:  filesize("a.txt");
来源：http://xtd.nwbrower.top

JS:   fs.statSync("a.txt").size
来源：http://zcu.yfazqb.com

TS:   fs.statSync("a.txt").size
来源：http://boj.sufxvd.cn

Java: Files.size(Path.of("a.txt"))
来源：http://koq.zhiwuduotai.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://str.zhijiandao.cn

Ruby: File.size("a.txt")
来源：http://cyo.birdmap.top

C#:   new FileInfo("a.txt").Length
来源：http://dgb.zhaomingkeji.xyz

[F10] 取文件扩展名 / 文件名
来源：http://pyy.52xcode.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bag.tianlin.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://puc.gotoacloud.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://igz.jqgufenzy.top

TS:   path.extname("a.txt")
来源：http://fxj.fktsv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qxc.kuanghao11.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kym.fanxiaobao.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gcj.hywenlv.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nje.nwbrower.top

[F11] 复制与移动文件
来源：http://tkv.yanxiufei.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wch.ctjpmb.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://apd.sysykeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ypq.gotoacloud.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hzu.gaohongyu789.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xpo.jiagoushi.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nfi.uphjek.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ppf.dashuyun.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jlb.yonumen.top

[F12] CSV 读写
来源：http://dxn.zhoulong.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nxv.tanke756.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lkr.ctjpmb.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yje.hongshengwenyu.top

TS:   // 同上
来源：http://kjs.xinyue.icu

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qia.ppjwa.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://avd.fanxiaobao.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nvp.sufxvd.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cvf.aibaodan.cn

================================================================================
来源：http://ovt.dianchejie.cn

G. 面向对象
来源：http://gzc.shanyushiyangkeji.top

================================================================================
来源：http://njp.aibaodan.cn

[G01] 定义类
来源：http://lrm.daxiang520.top

Py:   class User: pass
来源：http://yqh.andypj.xyz

PHP:  class User {}
来源：http://bty.jyoumei.cn

JS:   class User {}
来源：http://zdl.aizwys.cn

TS:   class User { name: string = ""; }
来源：http://tnq.zhongyouzk.top

Java: class User {}
来源：http://ude.zhiwuduotai.top

Go:   type User struct { Name string }
来源：http://khg.cheryme.top

Ruby: class User; end
来源：http://plp.jyoumei.cn

C#:   class User {}
来源：http://wxc.hcnkem.com

[G02] 构造函数
来源：http://zvb.yongpay.top

Py:   def __init__(self, name): self.name = name
来源：http://ogt.yonumen.top

PHP:  public function __construct(public string $name) {}
来源：http://lyx.jqgfzy.top

JS:   constructor(name) { this.name = name; }
来源：http://ttk.hywenlv.cn

TS:   constructor(public name: string) {}
来源：http://hjs.svipenyu.cn

Java: User(String name) { this.name = name; }
来源：http://vam.jianghu66.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xer.hongshengwenyu.top

Ruby: def initialize(name); @name = name; end
来源：http://xxy.gotoacloud.top

C#:   public User(string name) { Name = name; }
来源：http://pco.yanxiufei.cn

[G03] 实例属性
来源：http://yye.jlsjyb.cn

Py:   self.name = "x"
来源：http://btt.sweek.top

PHP:  public string $name = "x";
来源：http://zdo.52xcode.cn

JS:   this.name = "x";
来源：http://qrn.shuidangran.top

TS:   name: string = "x";
来源：http://uwq.9152youxi.cn

Java: private String name;
来源：http://aag.jianghu66.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zym.xylfe.cn

Ruby: @name = "x"
来源：http://wid.zhoulong.xyz

C#:   public string Name { get; set; } = "x";
来源：http://sdq.sysykeji.top

[G04] 定义方法
来源：http://exo.zhengqikj.top

Py:   def greet(self): return self.name
来源：http://psu.yj202588.top

PHP:  public function greet(): string { return $this->name; }
来源：http://jkg.aizwys.cn

JS:   greet() { return this.name; }
来源：http://fzq.chenlongwang.top

TS:   greet(): string { return this.name; }
来源：http://pur.hnqzz.top

Java: String greet() { return name; }
来源：http://arq.dashuyun.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gst.svipenyu.cn

Ruby: def greet; @name; end
来源：http://egf.zhengqikj.top

C#:   public string Greet() => Name;
来源：http://aht.cheryme.top

[G05] 继承
来源：http://ahn.jianghu66.top

Py:   class Admin(User): pass
来源：http://eks.tanke756.top

PHP:  class Admin extends User {}
来源：http://dqw.hysaishi.cn

JS:   class Admin extends User {}
来源：http://xsn.meibo888.top

TS:   class Admin extends User {}
来源：http://ufd.nanxuanxn.top

Java: class Admin extends User {}
来源：http://uwh.yvedp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sew.jqgfzy.top

Ruby: class Admin < User; end
来源：http://npe.ivvv.top

C#:   class Admin : User {}
来源：http://ejf.haohaochexian.top

[G06] 重写方法
来源：http://xjb.jinghuilouyu.cn

Py:   def greet(self): return "admin"
来源：http://woq.jiagoushi.top

PHP:  public function greet(): string { return "admin"; }
来源：http://tou.shanyushiyangtech.top

JS:   greet() { return "admin"; }
来源：http://cti.xinyue.icu

TS:   greet(): string { return "admin"; }
来源：http://wjh.sxryk.cn

Java: @Override String greet() { return "admin"; }
来源：http://zly.yvedp.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qsq.yangfankeji.com

Ruby: def greet; "admin"; end
来源：http://rrt.pengpengdd.cyou

C#:   public override string Greet() => "admin";
来源：http://eiw.cucudq.cn

[G07] 调用父类方法
来源：http://jjx.chenzaomai.com

Py:   super().greet()
来源：http://xte.yj20258.top

PHP:  parent::greet();
来源：http://nkj.ywan-chungtsiang.top

JS:   super.greet();
来源：http://xlh.wangshuangyany.cn

TS:   super.greet();
来源：http://wjv.ydjk.org.cn

Java: super.greet();
来源：http://gft.tianlin.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wht.shanyushiyangkeji.top

Ruby: super
来源：http://lqz.yuanzhike.top

C#:   base.Greet();
来源：http://mcp.jqgufenzy.top

[G08] 静态方法与属性
来源：http://klf.cdnleiting.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://myo.sysykeji.top

PHP:  public static function f() {}
来源：http://fnf.mhx1999.top

JS:   static f() {}
来源：http://lpx.fzhhl.top

TS:   static f(): void {}
来源：http://jkg.gzhubu.top

Java: static void f() {}
来源：http://wfm.tian-w.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://gpe.zhaomingkeji.xyz

Ruby: def self.f; end
来源：http://gds.shangyingyoupin.top

C#:   public static void F() {}
来源：http://oql.zycfv.cn

[G09] 接口 / 抽象类
来源：http://gca.yuxming.cn

Py:   from abc import ABC, abstractmethod
来源：http://sve.ppjwa.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ffy.zdqjudy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ckf.jinghuilouyu.cn

TS:   interface Shape { area(): number; }
来源：http://ncl.zhengqikj.top

Java: interface Shape { double area(); }
来源：http://dpk.chenzaomai.com

Go:   type Shape interface { Area() float64 }
来源：http://zvl.yuanzhike.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://icp.tianlin.xyz

C#:   interface IShape { double Area(); }
来源：http://tdg.redwolf501.top

[G10] 访问控制
来源：http://xvp.zhengqikj.top

Py:   约定 _protected / __private（不强制）
来源：http://hsl.yj202588.top

PHP:  public / protected / private
来源：http://wyj.sweek.top

JS:   #private 字段；其余公开
来源：http://lou.hammf.cn

TS:   public / protected / private
来源：http://mry.0kj1m.cn

Java: public / protected / private / 默认包级
来源：http://toj.yonumen.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://bhb.aizwys.cn

Ruby: public / protected / private
来源：http://arp.jianghu66.top

C#:   public / protected / private / internal
来源：http://mcv.zhiwuduotai.top

[G11] getter / setter
来源：http://myj.shzxlz.cn

Py:   @property 与 @x.setter
来源：http://liz.jqgfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://uug.xylfe.cn

JS:   get name() { return this._name; }
来源：http://lqr.quarkkingdee.top

TS:   get name(): string { return this._name; }
来源：http://xnt.cucudq.cn

Java: public String getName() { return name; }
来源：http://lsc.ehwqpu.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://pzl.jianghu66.top

Ruby: attr_accessor :name
来源：http://pwb.9152youxi.cn

C#:   public string Name { get; set; }
来源：http://hyw.redwolf501.top

[G12] 对象转字符串
来源：http://vhr.chenjidiqi.icu

Py:   def __str__(self): return self.name
来源：http://ety.tianlin.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://mcj.uphjek.com

JS:   toString() { return this.name; }
来源：http://bcy.shangyingyoupin.top

TS:   toString(): string { return this.name; }
来源：http://prq.ivvv.top

Java: @Override public String toString() { return name; }
来源：http://kpr.yvedp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://iyh.tarul.cn

Ruby: def to_s; @name; end
来源：http://nge.aibaodan.cn

C#:   public override string ToString() => Name;
来源：http://fzb.wangdashe.top

[G13] 判断对象类型
来源：http://qjg.cucudq.cn

Py:   isinstance(u, User)
来源：http://zot.fengsongda.top

PHP:  $u instanceof User
来源：http://sdh.ivvv.top

JS:   u instanceof User
来源：http://xil.havefunace.top

TS:   u instanceof User
来源：http://tuc.cucudq.cn

Java: u instanceof User
来源：http://rxj.bjfxy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://nqm.zdqjudy.top

Ruby: u.is_a?(User)
来源：http://nzj.dianchejie.cn

C#:   u is User
来源：http://out.fengsongda.top

[G14] 数据类 / record
来源：http://ydr.bbcook.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://osn.yfazqb.com

PHP:  // 用 readonly 属性模拟
来源：http://hqh.sufxvd.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rra.zdqjudy.top

TS:   type User = { name: string; age: number };
来源：http://uog.cqqwz.cn

Java: record User(String name, int age) {}
来源：http://lwd.shanyushiyangkeji.top

Go:   type User struct { Name string; Age int }
来源：http://ego.gaohongyu789.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rvn.jinqigufen.top

C#:   record User(string Name, int Age);
来源：http://zws.52xcode.cn

[G15] 枚举
来源：http://uzr.ctjpmb.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://iro.pengpengdd.cyou

PHP:  enum Color: string { case Red = "red"; }
来源：http://pnb.fanxiaobao.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ayx.birdmap.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ifh.316326.xyz

Java: enum Color { RED, GREEN }
来源：http://xyl.smart0.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ecc.gaohongyu789.top

Ruby: Color = %i[red green].freeze
来源：http://eas.nanxuanxn.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qvp.zhengqikj.top

[G16] 对象转数组 / 字典
来源：http://yml.hammf.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://avz.shuidangran.top

PHP:  get_object_vars($obj);
来源：http://pce.wangdashe.top

JS:   Object.entries(obj)
来源：http://vdw.pengpengdd.cyou

TS:   Object.entries(obj)
来源：http://grb.vqdsnc.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xbf.fehbvm.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://wlk.guannengcc.top

Ruby: obj.instance_variables
来源：http://sfs.svipenyu.cn

C#:   // 用反射或 System.Text.Json
来源：http://ecm.fanxiaobao.xyz

================================================================================
来源：http://rhc.chenlongwang.top

H. 异常与错误处理
来源：http://ulv.pycfn.com

================================================================================
来源：http://yeq.0kj1m.cn

[H01] try / catch 基础
来源：http://kah.jinyuanbaomall.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://szr.yuanzhike.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fcx.cheryme.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://epn.sweek.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qyo.hnxiangtu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yvo.nwbrower.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yeg.yangfankeji.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dli.jiagoushi.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fwb.zhoulong.xyz

[H02] finally / ensure 收尾
来源：http://mpn.cdnleiting.top

Py:   try: f()⏎finally: cleanup()
来源：http://mra.zhaomingkeji.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://ncd.zdbjq.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ihh.zhoulong.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://pja.xuetiantiany.cn

Java: try { f(); } finally { cleanup(); }
来源：http://red.haohaochexian.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://jxg.chenlongwang.top

Ruby: begin; f; ensure; cleanup; end
来源：http://dra.ctjpmb.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://kjk.316326.xyz

[H03] 主动抛出异常
来源：http://ank.52xcode.cn

Py:   raise ValueError("错误信息")
来源：http://ylh.jinqigfzy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://iim.shangyingyoupin.top

JS:   throw new Error("错误信息");
来源：http://txg.sxryk.cn

TS:   throw new Error("错误信息");
来源：http://vjm.chenjidiqi.icu

Java: throw new IllegalArgumentException("错误信息");
来源：http://hif.snrcjt.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oxd.mhx1999.top

Ruby: raise ArgumentError, "错误信息"
来源：http://gii.guowangkeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://zuf.mhx1999.top

[H04] 自定义异常类型
来源：http://hmy.jinqigufen.top

Py:   class MyError(Exception): pass
来源：http://mdw.kuanghao11.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wsy.jinghuilouyu.cn

JS:   class MyError extends Error {}
来源：http://lsy.xuetiantiany.cn

TS:   class MyError extends Error {}
来源：http://see.xuetiantiany.cn

Java: class MyException extends RuntimeException {}
来源：http://cik.cucudq.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vte.guowangkeji.top

Ruby: class MyError < StandardError; end
来源：http://lnx.sweek.top

C#:   class MyException : Exception {}
来源：http://yjb.xuanzx.com

[H05] 捕获特定类型
来源：http://gaw.sufxvd.cn

Py:   except ValueError as e:
来源：http://nrd.svipenyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://umm.zhiwuduotai.top

JS:   if (e instanceof TypeError) {}
来源：http://vuw.daria6918.cn

TS:   if (e instanceof TypeError) {}
来源：http://yym.aibaodan.cn

Java: catch (IOException | SQLException e) {}
来源：http://ami.ctjpmb.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wsn.nanxinkj.top

Ruby: rescue ArgumentError => e
来源：http://rzp.fktsv.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mck.shzxlz.cn

[H06] 可选值 / 空值安全访问
来源：http://kmw.ctjpmb.com

Py:   value = d.get("k") or default
来源：http://qei.jinyuanbaomall.cn

PHP:  $v = $d["k"] ?? null;
来源：http://yyp.chenzaomai.com

JS:   obj?.a?.b;  d ?? default
来源：http://doh.haohaochexian.top

TS:   obj?.a?.b;  d ?? default
来源：http://mqe.epnwcf.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yzh.snrcjt.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://clh.cdnleiting.top

Ruby: d&.dig(:a, :b)
来源：http://vbe.zhengqikj.top

C#:   obj?.A?.B ?? default
来源：http://qhq.xylfe.cn

[H07] 断言
来源：http://bey.shuidangran.top

Py:   assert x > 0, "必须为正"
来源：http://hcq.jlsjyb.cn

PHP:  assert($x > 0);
来源：http://mup.cheryme.top

JS:   console.assert(x > 0);
来源：http://zny.zhixingplan.top

TS:   console.assert(x > 0);
来源：http://yrt.yueranfly.top

Java: assert x > 0 : "必须为正";
来源：http://tpz.tian-w.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kkv.jqgfzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://idt.iojbl.cn

C#:   Debug.Assert(x > 0);
来源：http://mwz.shanyushiyangtech.top

[H08] 获取错误信息与堆栈
来源：http://zrf.yj20258.top

Py:   str(e);  traceback.format_exc()
来源：http://kuy.aibaodan.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rob.smart0.xyz

JS:   e.message;  e.stack
来源：http://hqa.iojbl.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tpu.yj20258.top

Java: e.getMessage();  e.printStackTrace()
来源：http://yis.316326.xyz

Go:   err.Error()
来源：http://uan.wangdashe.top

Ruby: e.message;  e.backtrace
来源：http://tvl.pengpengdd.cyou

C#:   e.Message;  e.StackTrace
来源：http://jgh.bjfxy.top

[H09] 带错误码的异常
来源：http://yae.hywenlv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hvg.guowangkeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://wxp.yfazqb.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bhn.feifeiyinyue.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mgb.jlsjyb.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qrj.316326.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ypr.jianghu66.top

Ruby: raise MyError.new("fail", 500)
来源：http://fqj.hfpthk.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://msm.birdmap.top

[H10] 资源自动释放
来源：http://sod.cashguo.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://nfm.jinghuilouyu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://god.vehdjk.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mof.jqgfzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wdx.haohaochexian.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://car.c1oappe.top

Go:   defer f.Close()
来源：http://mov.jlsjyb.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zby.epnwcf.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yxr.yuanzhike.top

================================================================================
来源：http://sfn.316326.xyz

I. 正则表达式
来源：http://jvb.jqgfzy.top

================================================================================
来源：http://nah.yuxming.cn

[I01] 判断是否匹配
来源：http://zwk.cdnleiting.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rdv.sxryk.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gny.iojbl.cn

JS:   /\d+/.test(s)
来源：http://old.cucudq.cn

TS:   /\d+/.test(s)
来源：http://cvn.snrcjt.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nna.hammf.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://buo.tianlin.xyz

Ruby: s.match?(/\d+/)
来源：http://hjx.zhaomingkeji.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vkh.hysaishi.cn


<!-- 参考信息 -->