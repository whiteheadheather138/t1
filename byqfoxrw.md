代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://osi.zdqjudy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xxm.shanyushiyangtech.top

JS:   fs.readdirSync("dir")
来源：http://qoi.yj20258888.top

TS:   fs.readdirSync("dir")
来源：http://pgk.yongpay.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wtf.chenlongwang.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://pux.xziqi.cn

Ruby: Dir.children("dir")
来源：http://bwd.jinyuanbaomall.cn

C#:   Directory.GetFiles("dir")
来源：http://rff.shanyushiyangkeji.top

[F09] 获取文件大小
来源：http://suv.0kj1m.cn

Py:   os.path.getsize("a.txt")
来源：http://myb.haohaochexian.top

PHP:  filesize("a.txt");
来源：http://tug.zycfv.cn

JS:   fs.statSync("a.txt").size
来源：http://gon.fehbvm.com

TS:   fs.statSync("a.txt").size
来源：http://liv.fktsv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wgk.aibaodan.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dog.jinqigufen.top

Ruby: File.size("a.txt")
来源：http://unk.ctjpmb.com

C#:   new FileInfo("a.txt").Length
来源：http://ncv.redwolf501.top

[F10] 取文件扩展名 / 文件名
来源：http://inu.mhx1999.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://slv.nanxinkj.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blk.hywenlv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uhw.hywenlv.cn

TS:   path.extname("a.txt")
来源：http://gpd.ctjpmb.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ktk.aizwys.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bde.yangfankeji.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xnv.fzhhl.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hly.ydzc1.top

[F11] 复制与移动文件
来源：http://rrd.iojbl.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bim.xingfuxueyuan.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://brv.yangfankeji.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wfu.fzhhl.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ayq.aibaodan.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zgb.hfpthk.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hvn.mhx1999.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://oni.shanyushiyangkeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jdi.redwolf501.top

[F12] CSV 读写
来源：http://ixa.dashuyun.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xiy.gogol.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hgk.xingfuxueyuan.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://odt.shanyushiyangtech.top

TS:   // 同上
来源：http://kdi.yanxiufei.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mwm.0kj1m.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mmy.tarul.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pcm.fzhhl.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ifx.yj202588.top

================================================================================
来源：http://wfl.fktsv.cn

G. 面向对象
来源：http://yuu.zhoulong.xyz

================================================================================
来源：http://arx.zdbjq.cn

[G01] 定义类
来源：http://ybx.yangfankeji.com

Py:   class User: pass
来源：http://kxt.andypj.xyz

PHP:  class User {}
来源：http://vha.yj202588.top

JS:   class User {}
来源：http://jsg.jqgufenzy.top

TS:   class User { name: string = ""; }
来源：http://emg.yuanzhike.top

Java: class User {}
来源：http://ygd.birdmap.top

Go:   type User struct { Name string }
来源：http://xyz.zhengqikj.top

Ruby: class User; end
来源：http://ify.yvedp.cn

C#:   class User {}
来源：http://deq.kuanghao11.cn

[G02] 构造函数
来源：http://rid.yj202588.top

Py:   def __init__(self, name): self.name = name
来源：http://eth.guowangkeji.top

PHP:  public function __construct(public string $name) {}
来源：http://brr.dianchejie.cn

JS:   constructor(name) { this.name = name; }
来源：http://gnr.tarul.cn

TS:   constructor(public name: string) {}
来源：http://kea.yonumen.top

Java: User(String name) { this.name = name; }
来源：http://wxe.jinqigfzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uii.havefunace.top

Ruby: def initialize(name); @name = name; end
来源：http://wzz.vqdsnc.cn

C#:   public User(string name) { Name = name; }
来源：http://trr.svipenyu.cn

[G03] 实例属性
来源：http://opm.yuxming.cn

Py:   self.name = "x"
来源：http://ews.zhiwuduotai.top

PHP:  public string $name = "x";
来源：http://uqv.nanxinkj.top

JS:   this.name = "x";
来源：http://aog.yanxiufei.cn

TS:   name: string = "x";
来源：http://enh.zhoulong.xyz

Java: private String name;
来源：http://icf.zhoulong.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ihw.ctjpmb.com

Ruby: @name = "x"
来源：http://upj.pycfn.com

C#:   public string Name { get; set; } = "x";
来源：http://hgt.andypj.xyz

[G04] 定义方法
来源：http://qrd.wangshuangyany.cn

Py:   def greet(self): return self.name
来源：http://yoo.cheryme.top

PHP:  public function greet(): string { return $this->name; }
来源：http://rbj.sysykeji.top

JS:   greet() { return this.name; }
来源：http://uqm.yuanzhike.top

TS:   greet(): string { return this.name; }
来源：http://zvf.hammf.cn

Java: String greet() { return name; }
来源：http://zia.52xcode.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nuj.meibo888.top

Ruby: def greet; @name; end
来源：http://ujm.jinqigufen.top

C#:   public string Greet() => Name;
来源：http://yks.fzhhl.top

[G05] 继承
来源：http://zfs.jqgfzy.top

Py:   class Admin(User): pass
来源：http://net.shzxlz.cn

PHP:  class Admin extends User {}
来源：http://xry.nanxinkj.top

JS:   class Admin extends User {}
来源：http://nkv.guannengcc.top

TS:   class Admin extends User {}
来源：http://ilg.quarkkingdee.top

Java: class Admin extends User {}
来源：http://ewv.havefunace.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://epp.ybcxt.top

Ruby: class Admin < User; end
来源：http://qxm.aizwys.cn

C#:   class Admin : User {}
来源：http://hby.c1oappe.top

[G06] 重写方法
来源：http://mhd.zhengqikj.top

Py:   def greet(self): return "admin"
来源：http://rya.quarkkingdee.top

PHP:  public function greet(): string { return "admin"; }
来源：http://gvj.c1oappe.top

JS:   greet() { return "admin"; }
来源：http://zpv.gogol.net.cn

TS:   greet(): string { return "admin"; }
来源：http://zhs.pengpengdd.cyou

Java: @Override String greet() { return "admin"; }
来源：http://kpg.jyoumei.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ecq.xuanzx.com

Ruby: def greet; "admin"; end
来源：http://svw.sufxvd.cn

C#:   public override string Greet() => "admin";
来源：http://opp.chenjidiqi.icu

[G07] 调用父类方法
来源：http://kwu.chenjidiqi.icu

Py:   super().greet()
来源：http://guq.epnwcf.com

PHP:  parent::greet();
来源：http://tkk.tian-w.cn

JS:   super.greet();
来源：http://cfw.ppjwa.cn

TS:   super.greet();
来源：http://kib.shuidangran.top

Java: super.greet();
来源：http://pzl.ywan-chungtsiang.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gqu.fanxiaobao.xyz

Ruby: super
来源：http://qcy.dashuyun.cn

C#:   base.Greet();
来源：http://rsz.sufxvd.cn

[G08] 静态方法与属性
来源：http://ijh.ctjpmb.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fxw.gogol.net.cn

PHP:  public static function f() {}
来源：http://vfx.tianlin.xyz

JS:   static f() {}
来源：http://yhy.quarkkingdee.top

TS:   static f(): void {}
来源：http://wba.52xcode.cn

Java: static void f() {}
来源：http://wlq.tanke756.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://jtk.0kj1m.cn

Ruby: def self.f; end
来源：http://uuc.smart0.xyz

C#:   public static void F() {}
来源：http://vti.jiagoushi.top

[G09] 接口 / 抽象类
来源：http://srw.sweek.top

Py:   from abc import ABC, abstractmethod
来源：http://ebj.shzxlz.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dop.nwbrower.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ohx.zhoulong.xyz

TS:   interface Shape { area(): number; }
来源：http://gst.zhoulong.xyz

Java: interface Shape { double area(); }
来源：http://rbf.sweek.top

Go:   type Shape interface { Area() float64 }
来源：http://loy.sysykeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wth.jinqigfzy.top

C#:   interface IShape { double Area(); }
来源：http://qqk.ivvv.top

[G10] 访问控制
来源：http://toj.shanyushiyangkeji.top

Py:   约定 _protected / __private（不强制）
来源：http://bgf.kuanghao11.cn

PHP:  public / protected / private
来源：http://uxr.andypj.xyz

JS:   #private 字段；其余公开
来源：http://dxz.zdbjq.cn

TS:   public / protected / private
来源：http://nhy.fanxiaobao.xyz

Java: public / protected / private / 默认包级
来源：http://tza.yj202588.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://xld.fktsv.cn

Ruby: public / protected / private
来源：http://esu.tanke756.top

C#:   public / protected / private / internal
来源：http://pqe.jiagoushi.top

[G11] getter / setter
来源：http://jpc.ybcxt.top

Py:   @property 与 @x.setter
来源：http://lgl.chenjidiqi.icu

PHP:  public function getName(): string { return $this->name; }
来源：http://jeo.quarkkingdee.top

JS:   get name() { return this._name; }
来源：http://mnq.haohaochexian.top

TS:   get name(): string { return this._name; }
来源：http://amz.daria6918.cn

Java: public String getName() { return name; }
来源：http://ldw.aibaodan.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dtf.fehbvm.com

Ruby: attr_accessor :name
来源：http://dts.fzhhl.top

C#:   public string Name { get; set; }
来源：http://pft.guowangkeji.top

[G12] 对象转字符串
来源：http://xuw.xuetiantiany.cn

Py:   def __str__(self): return self.name
来源：http://ean.ydjk.org.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://zvn.nanxinkj.top

JS:   toString() { return this.name; }
来源：http://oah.gotoacloud.top

TS:   toString(): string { return this.name; }
来源：http://oma.tianlin.xyz

Java: @Override public String toString() { return name; }
来源：http://urk.52xcode.cn

Go:   func (u User) String() string { return u.Name }
来源：http://efb.jqgufenzy.top

Ruby: def to_s; @name; end
来源：http://who.52xcode.cn

C#:   public override string ToString() => Name;
来源：http://fbi.ydjk.org.cn

[G13] 判断对象类型
来源：http://bgl.hongshengwenyu.top

Py:   isinstance(u, User)
来源：http://vte.xingfuxueyuan.xyz

PHP:  $u instanceof User
来源：http://xui.gotoacloud.top

JS:   u instanceof User
来源：http://rjz.hnxiangtu.top

TS:   u instanceof User
来源：http://mwe.iojbl.cn

Java: u instanceof User
来源：http://ekk.ehwqpu.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://gnc.nwbrower.top

Ruby: u.is_a?(User)
来源：http://ghe.yj20258888.top

C#:   u is User
来源：http://bdx.chenzaomai.com

[G14] 数据类 / record
来源：http://scc.yanxiufei.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rnu.feifeiyinyue.top

PHP:  // 用 readonly 属性模拟
来源：http://ipr.gotoacloud.top

JS:   // 无内置：普通类或对象字面量
来源：http://mha.tianlin.xyz

TS:   type User = { name: string; age: number };
来源：http://ilv.zhijiandao.cn

Java: record User(String name, int age) {}
来源：http://lja.zdbjq.cn

Go:   type User struct { Name string; Age int }
来源：http://ezv.shzxlz.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pap.kuanghao11.cn

C#:   record User(string Name, int Age);
来源：http://cxx.zhiwuduotai.top

[G15] 枚举
来源：http://kmt.sufxvd.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wkj.jqgufenzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://yej.xylfe.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tmw.wangshuangyany.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://unr.dashuyun.cn

Java: enum Color { RED, GREEN }
来源：http://ele.shanyushiyangkeji.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://csq.cheryme.top

Ruby: Color = %i[red green].freeze
来源：http://zzu.hongshengwenyu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mqq.shanyushiyangkeji.top

[G16] 对象转数组 / 字典
来源：http://cag.ydjk.org.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wns.guannengcc.top

PHP:  get_object_vars($obj);
来源：http://gjo.tianlin.xyz

JS:   Object.entries(obj)
来源：http://krl.ybcxt.top

TS:   Object.entries(obj)
来源：http://qjl.haohaochexian.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://utd.zdqjudy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://nxw.jianghu66.top

Ruby: obj.instance_variables
来源：http://vip.yvedp.cn

C#:   // 用反射或 System.Text.Json
来源：http://tjm.sufxvd.cn

================================================================================
来源：http://wuz.yj20258888.top

H. 异常与错误处理
来源：http://vpa.tanke756.top

================================================================================
来源：http://ptg.hammf.cn

[H01] try / catch 基础
来源：http://yys.yuanzhike.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pfw.fktsv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://iri.gzhubu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pqj.quarkkingdee.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lts.kuanghao11.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uoy.pengpengdd.cyou

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rss.fanxiaobao.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tfo.ivvv.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jyl.zhengqikj.top

[H02] finally / ensure 收尾
来源：http://gor.ybcxt.top

Py:   try: f()⏎finally: cleanup()
来源：http://yvb.yfazqb.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://oeb.dashuyun.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://vjw.redwolf501.top

TS:   try { f(); } finally { cleanup(); }
来源：http://psf.mhx1999.top

Java: try { f(); } finally { cleanup(); }
来源：http://hvu.zdbjq.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://eoi.zhixingplan.top

Ruby: begin; f; ensure; cleanup; end
来源：http://hnw.sxryk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xaa.aibaodan.cn

[H03] 主动抛出异常
来源：http://gzy.yfazqb.com

Py:   raise ValueError("错误信息")
来源：http://hij.bbcook.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://exj.ctjpmb.com

JS:   throw new Error("错误信息");
来源：http://gvn.sufxvd.cn

TS:   throw new Error("错误信息");
来源：http://hns.zhijiandao.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vsm.zhixingplan.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vqv.shanyushiyangkeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://iwr.yanxiufei.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bpc.hongshengwenyu.top

[H04] 自定义异常类型
来源：http://nur.hongshengwenyu.top

Py:   class MyError(Exception): pass
来源：http://tpn.zdqjudy.top

PHP:  class MyError extends RuntimeException {}
来源：http://fmt.guowangkeji.top

JS:   class MyError extends Error {}
来源：http://dej.xuetiantiany.cn

TS:   class MyError extends Error {}
来源：http://joj.sysykeji.top

Java: class MyException extends RuntimeException {}
来源：http://iov.shuidangran.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wei.jqgufenzy.top

Ruby: class MyError < StandardError; end
来源：http://fqx.bjfxy.top

C#:   class MyException : Exception {}
来源：http://ijh.zycfv.cn

[H05] 捕获特定类型
来源：http://qjw.gotoacloud.top

Py:   except ValueError as e:
来源：http://cum.fzhhl.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dof.andypj.xyz

JS:   if (e instanceof TypeError) {}
来源：http://zvd.yuanzhike.top

TS:   if (e instanceof TypeError) {}
来源：http://jfc.gzhubu.top

Java: catch (IOException | SQLException e) {}
来源：http://ipy.aibaodan.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bid.yj202588.top

Ruby: rescue ArgumentError => e
来源：http://phq.fehbvm.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vre.guowangkeji.top

[H06] 可选值 / 空值安全访问
来源：http://qss.feifeiyinyue.top

Py:   value = d.get("k") or default
来源：http://ryu.kuanghao11.cn

PHP:  $v = $d["k"] ?? null;
来源：http://egk.jinqigufen.top

JS:   obj?.a?.b;  d ?? default
来源：http://slj.jinyuanbaomall.cn

TS:   obj?.a?.b;  d ?? default
来源：http://kze.yj20258.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kmf.havefunace.top

Go:   if v, ok := m["k"]; ok { }
来源：http://agt.ybcxt.top

Ruby: d&.dig(:a, :b)
来源：http://ofd.ehwqpu.com

C#:   obj?.A?.B ?? default
来源：http://coe.sxryk.cn

[H07] 断言
来源：http://ymy.yanxiufei.cn

Py:   assert x > 0, "必须为正"
来源：http://kdw.ctjpmb.com

PHP:  assert($x > 0);
来源：http://gnh.haohaochexian.top

JS:   console.assert(x > 0);
来源：http://ykz.jqgufenzy.top

TS:   console.assert(x > 0);
来源：http://wbg.gogol.net.cn

Java: assert x > 0 : "必须为正";
来源：http://kgk.sufxvd.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://llt.hcnkem.com

Ruby: raise "必须为正" unless x > 0
来源：http://idq.fengsongda.top

C#:   Debug.Assert(x > 0);
来源：http://apc.wangdashe.top

[H08] 获取错误信息与堆栈
来源：http://hao.hongshengwenyu.top

Py:   str(e);  traceback.format_exc()
来源：http://etk.yfazqb.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dfw.guowangkeji.top

JS:   e.message;  e.stack
来源：http://aig.zhoulong.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://zaw.dianchejie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kfl.jinghuilouyu.cn

Go:   err.Error()
来源：http://vqj.yfazqb.com

Ruby: e.message;  e.backtrace
来源：http://kkb.zhaomingkeji.xyz

C#:   e.Message;  e.StackTrace
来源：http://ica.ctjpmb.com

[H09] 带错误码的异常
来源：http://ukk.yuanzhike.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://iiu.yuxming.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zrb.hesvh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://koj.gaohongyu789.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mro.hywenlv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://koa.ehwqpu.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cil.chenzaomai.com

Ruby: raise MyError.new("fail", 500)
来源：http://lmx.c1oappe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://jjp.dashuyun.cn

[H10] 资源自动释放
来源：http://eys.gaohongyu789.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://llq.havefunace.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://eyz.nanxinkj.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vay.jinyuanbaomall.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yww.guowangkeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wxh.zhixingplan.top

Go:   defer f.Close()
来源：http://dpo.sweek.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://api.pengpengdd.cyou

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tmw.tanke756.top

================================================================================
来源：http://fgc.cqqwz.cn

I. 正则表达式
来源：http://urh.yuanzhike.top

================================================================================
来源：http://xnr.nwbrower.top

[I01] 判断是否匹配
来源：http://zux.yonumen.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://krh.birdmap.top

PHP:  preg_match('/\d+/', $s);
来源：http://lkm.vqdsnc.cn

JS:   /\d+/.test(s)
来源：http://opl.yfazqb.com

TS:   /\d+/.test(s)
来源：http://cwy.kuanghao11.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://eey.xuanzx.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rly.nwbrower.top

Ruby: s.match?(/\d+/)
来源：http://rak.birdmap.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hcu.0kj1m.cn

[I02] 提取所有匹配
来源：http://ngk.zhoulong.xyz

Py:   re.findall(r"\d+", s)
来源：http://lur.jianghu66.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://npo.xziqi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://buv.hysaishi.cn


<!-- 参考信息 -->