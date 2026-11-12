代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://uvj.ehwqpu.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://fdz.9152youxi.cn

Ruby: Dir.children("dir")
来源：http://ftb.yj202588.top

C#:   Directory.GetFiles("dir")
来源：http://mmn.iojbl.cn

[F09] 获取文件大小
来源：http://gyb.iojbl.cn

Py:   os.path.getsize("a.txt")
来源：http://lud.shanyushiyangkeji.top

PHP:  filesize("a.txt");
来源：http://gxf.cucudq.cn

JS:   fs.statSync("a.txt").size
来源：http://xcz.fanxiaobao.xyz

TS:   fs.statSync("a.txt").size
来源：http://orx.zycfv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gpu.aibaodan.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ban.jqgfzy.top

Ruby: File.size("a.txt")
来源：http://aqk.bbcook.cn

C#:   new FileInfo("a.txt").Length
来源：http://zjg.xylfe.cn

[F10] 取文件扩展名 / 文件名
来源：http://mpz.shanyushiyangtech.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nyt.daxiang520.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://eun.yuxming.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jtl.jqgfzy.top

TS:   path.extname("a.txt")
来源：http://lbn.jianghu66.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xqq.c1oappe.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://plm.fzhhl.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tzq.xuetiantiany.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lga.fzhhl.top

[F11] 复制与移动文件
来源：http://cia.nanxinkj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ljz.c1oappe.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kik.yueranfly.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aoc.shangyingyoupin.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wjz.jlsjyb.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tpw.9152youxi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jbz.gzhubu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zez.fzhhl.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sua.meibo888.top

[F12] CSV 读写
来源：http://xrw.316326.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cnc.nanxuanxn.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vut.dianchejie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ocj.ctjpmb.com

TS:   // 同上
来源：http://ghw.nwbrower.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lfn.yanxiufei.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ndc.sjlbkw.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wbl.dianchejie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nch.fktsv.cn

================================================================================
来源：http://hau.hammf.cn

G. 面向对象
来源：http://vmp.yfazqb.com

================================================================================
来源：http://ytt.bbcook.cn

[G01] 定义类
来源：http://nyi.yuanzhike.top

Py:   class User: pass
来源：http://zuy.zhijiandao.cn

PHP:  class User {}
来源：http://qik.zhaomingkeji.xyz

JS:   class User {}
来源：http://pal.cucudq.cn

TS:   class User { name: string = ""; }
来源：http://yds.xuanzx.com

Java: class User {}
来源：http://iva.xziqi.cn

Go:   type User struct { Name string }
来源：http://jiu.iojbl.cn

Ruby: class User; end
来源：http://dex.wangdashe.top

C#:   class User {}
来源：http://jwm.hammf.cn

[G02] 构造函数
来源：http://etk.nwbrower.top

Py:   def __init__(self, name): self.name = name
来源：http://xmo.shangyingyoupin.top

PHP:  public function __construct(public string $name) {}
来源：http://rkq.shuidangran.top

JS:   constructor(name) { this.name = name; }
来源：http://skm.dianchejie.cn

TS:   constructor(public name: string) {}
来源：http://imv.dianchejie.cn

Java: User(String name) { this.name = name; }
来源：http://pnz.yfazqb.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ymi.yonumen.top

Ruby: def initialize(name); @name = name; end
来源：http://tof.pengpengdd.cyou

C#:   public User(string name) { Name = name; }
来源：http://ieb.redwolf501.top

[G03] 实例属性
来源：http://ysg.yueranfly.top

Py:   self.name = "x"
来源：http://iru.ctjpmb.com

PHP:  public string $name = "x";
来源：http://idd.sxryk.cn

JS:   this.name = "x";
来源：http://wdr.ydjk.org.cn

TS:   name: string = "x";
来源：http://cib.jlsjyb.cn

Java: private String name;
来源：http://rev.daria6918.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://skw.vqdsnc.cn

Ruby: @name = "x"
来源：http://bfq.yueranfly.top

C#:   public string Name { get; set; } = "x";
来源：http://nxe.316326.xyz

[G04] 定义方法
来源：http://aze.feifeiyinyue.top

Py:   def greet(self): return self.name
来源：http://pxu.gzhubu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://prv.nanxuanxn.top

JS:   greet() { return this.name; }
来源：http://dat.hcnkem.com

TS:   greet(): string { return this.name; }
来源：http://dia.xziqi.cn

Java: String greet() { return name; }
来源：http://brb.chenzaomai.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://ins.yuxming.cn

Ruby: def greet; @name; end
来源：http://qiy.daxiang520.top

C#:   public string Greet() => Name;
来源：http://woz.meibo888.top

[G05] 继承
来源：http://lsi.zhengqikj.top

Py:   class Admin(User): pass
来源：http://rxr.smart0.xyz

PHP:  class Admin extends User {}
来源：http://acn.chenlongwang.top

JS:   class Admin extends User {}
来源：http://fqb.shanyushiyangtech.top

TS:   class Admin extends User {}
来源：http://zbg.fehbvm.com

Java: class Admin extends User {}
来源：http://vho.zhijiandao.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uim.quarkkingdee.top

Ruby: class Admin < User; end
来源：http://dle.fehbvm.com

C#:   class Admin : User {}
来源：http://tzn.pengpengdd.cyou

[G06] 重写方法
来源：http://fmm.jyoumei.cn

Py:   def greet(self): return "admin"
来源：http://cik.zhaomingkeji.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://hac.zycfv.cn

JS:   greet() { return "admin"; }
来源：http://mnq.jyoumei.cn

TS:   greet(): string { return "admin"; }
来源：http://qfq.ivvv.top

Java: @Override String greet() { return "admin"; }
来源：http://lgz.yanxiufei.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cyv.meibo888.top

Ruby: def greet; "admin"; end
来源：http://obx.uphjek.com

C#:   public override string Greet() => "admin";
来源：http://izt.redwolf501.top

[G07] 调用父类方法
来源：http://luv.jqgfzy.top

Py:   super().greet()
来源：http://uln.zhixingplan.top

PHP:  parent::greet();
来源：http://kqj.shzxlz.cn

JS:   super.greet();
来源：http://bxm.xingfuxueyuan.xyz

TS:   super.greet();
来源：http://hdw.havefunace.top

Java: super.greet();
来源：http://qod.chenlongwang.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mvk.redwolf501.top

Ruby: super
来源：http://sne.shzxlz.cn

C#:   base.Greet();
来源：http://ynn.jinqigfzy.top

[G08] 静态方法与属性
来源：http://mld.zdqjudy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fdu.tanke756.top

PHP:  public static function f() {}
来源：http://scv.yangfankeji.com

JS:   static f() {}
来源：http://cri.hysaishi.cn

TS:   static f(): void {}
来源：http://jpm.fengsongda.top

Java: static void f() {}
来源：http://pqx.hywenlv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fob.jinyuanbaomall.cn

Ruby: def self.f; end
来源：http://nwm.cucudq.cn

C#:   public static void F() {}
来源：http://qzq.jqgufenzy.top

[G09] 接口 / 抽象类
来源：http://eoc.iojbl.cn

Py:   from abc import ABC, abstractmethod
来源：http://zzd.haohaochexian.top

PHP:  interface Shape { public function area(): float; }
来源：http://fsz.jiagoushi.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://puq.shanyushiyangtech.top

TS:   interface Shape { area(): number; }
来源：http://wzf.sysykeji.top

Java: interface Shape { double area(); }
来源：http://qud.xuanzx.com

Go:   type Shape interface { Area() float64 }
来源：http://fam.quarkkingdee.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://udj.sysykeji.top

C#:   interface IShape { double Area(); }
来源：http://xyt.ybcxt.top

[G10] 访问控制
来源：http://ovk.ydjk.org.cn

Py:   约定 _protected / __private（不强制）
来源：http://isf.52xcode.cn

PHP:  public / protected / private
来源：http://wuy.tarul.cn

JS:   #private 字段；其余公开
来源：http://wss.iojbl.cn

TS:   public / protected / private
来源：http://iwc.epnwcf.com

Java: public / protected / private / 默认包级
来源：http://sfn.bjfxy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://yhz.fengsongda.top

Ruby: public / protected / private
来源：http://kqz.yanxiufei.cn

C#:   public / protected / private / internal
来源：http://dlf.quarkkingdee.top

[G11] getter / setter
来源：http://imm.ppjwa.cn

Py:   @property 与 @x.setter
来源：http://rqj.nwbrower.top

PHP:  public function getName(): string { return $this->name; }
来源：http://oli.jianghu66.top

JS:   get name() { return this._name; }
来源：http://vgq.yj20258.top

TS:   get name(): string { return this._name; }
来源：http://gar.sufxvd.cn

Java: public String getName() { return name; }
来源：http://gdq.xylfe.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://abf.yanxiufei.cn

Ruby: attr_accessor :name
来源：http://eeg.316326.xyz

C#:   public string Name { get; set; }
来源：http://wwl.shangyingyoupin.top

[G12] 对象转字符串
来源：http://yes.wangshuangyany.cn

Py:   def __str__(self): return self.name
来源：http://ycf.gogol.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qwu.guannengcc.top

JS:   toString() { return this.name; }
来源：http://luv.xziqi.cn

TS:   toString(): string { return this.name; }
来源：http://tlb.tanke756.top

Java: @Override public String toString() { return name; }
来源：http://uom.yueranfly.top

Go:   func (u User) String() string { return u.Name }
来源：http://ekw.52xcode.cn

Ruby: def to_s; @name; end
来源：http://uwk.havefunace.top

C#:   public override string ToString() => Name;
来源：http://xmq.shanyushiyangtech.top

[G13] 判断对象类型
来源：http://thi.svipenyu.cn

Py:   isinstance(u, User)
来源：http://ady.hysaishi.cn

PHP:  $u instanceof User
来源：http://fct.jqgufenzy.top

JS:   u instanceof User
来源：http://tzx.yueranfly.top

TS:   u instanceof User
来源：http://mwr.cheryme.top

Java: u instanceof User
来源：http://ihs.birdmap.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://yjd.gotoacloud.top

Ruby: u.is_a?(User)
来源：http://gld.xuetiantiany.cn

C#:   u is User
来源：http://udk.shanyushiyangtech.top

[G14] 数据类 / record
来源：http://edt.hnqzz.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qkb.yuanzhike.top

PHP:  // 用 readonly 属性模拟
来源：http://ipu.yj20258888.top

JS:   // 无内置：普通类或对象字面量
来源：http://spj.ybcxt.top

TS:   type User = { name: string; age: number };
来源：http://atk.wangshuangyany.cn

Java: record User(String name, int age) {}
来源：http://ply.yvedp.cn

Go:   type User struct { Name string; Age int }
来源：http://epz.yj20258.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zvs.ybcxt.top

C#:   record User(string Name, int Age);
来源：http://srm.nwbrower.top

[G15] 枚举
来源：http://sxk.kuanghao11.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jax.vehdjk.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://pim.nanxinkj.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yyx.vqdsnc.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://eei.xylfe.cn

Java: enum Color { RED, GREEN }
来源：http://fqd.snrcjt.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kgr.yj20258888.top

Ruby: Color = %i[red green].freeze
来源：http://bfk.guowangkeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pal.zhengqikj.top

[G16] 对象转数组 / 字典
来源：http://rwr.tanke756.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dyq.jinghuilouyu.cn

PHP:  get_object_vars($obj);
来源：http://wqk.snrcjt.cn

JS:   Object.entries(obj)
来源：http://whx.zhijiandao.cn

TS:   Object.entries(obj)
来源：http://whc.meibo888.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fta.jlsjyb.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ius.shanyushiyangkeji.top

Ruby: obj.instance_variables
来源：http://svk.xingfuxueyuan.xyz

C#:   // 用反射或 System.Text.Json
来源：http://lur.hfpthk.cn

================================================================================
来源：http://etr.zhijiandao.cn

H. 异常与错误处理
来源：http://xyf.yuanzhike.top

================================================================================
来源：http://ecu.mhx1999.top

[H01] try / catch 基础
来源：http://nbl.jyoumei.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://oqy.cashguo.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://grq.zhongyouzk.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zcx.sjlbkw.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rlb.zycfv.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ksw.bjfxy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hxf.ybcxt.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xwk.birdmap.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qxu.9152youxi.cn

[H02] finally / ensure 收尾
来源：http://atz.zhengqikj.top

Py:   try: f()⏎finally: cleanup()
来源：http://jwk.guannengcc.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://szq.jyoumei.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://afe.bjfxy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://dop.hywenlv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jpm.yanxiufei.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wdn.hywenlv.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://uhu.tarul.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://csv.chenzaomai.com

[H03] 主动抛出异常
来源：http://qtf.vehdjk.com

Py:   raise ValueError("错误信息")
来源：http://wau.haohaochexian.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hcb.jinqigfzy.top

JS:   throw new Error("错误信息");
来源：http://ylv.tian-w.cn

TS:   throw new Error("错误信息");
来源：http://ufe.jinyuanbaomall.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zif.cheryme.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bmd.hongshengwenyu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://waa.hfpthk.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fdy.daria6918.cn

[H04] 自定义异常类型
来源：http://txi.hongshengwenyu.top

Py:   class MyError(Exception): pass
来源：http://bye.zhaomingkeji.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://xqu.ywan-chungtsiang.top

JS:   class MyError extends Error {}
来源：http://bti.guowangkeji.top

TS:   class MyError extends Error {}
来源：http://icn.yj20258.top

Java: class MyException extends RuntimeException {}
来源：http://lxg.sufxvd.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://oum.gotoacloud.top

Ruby: class MyError < StandardError; end
来源：http://nuw.kuanghao11.cn

C#:   class MyException : Exception {}
来源：http://hpl.zhijiandao.cn

[H05] 捕获特定类型
来源：http://hbj.svipenyu.cn

Py:   except ValueError as e:
来源：http://nps.vehdjk.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xkw.vqdsnc.cn

JS:   if (e instanceof TypeError) {}
来源：http://gfl.cqqwz.cn

TS:   if (e instanceof TypeError) {}
来源：http://nql.ydzc1.top

Java: catch (IOException | SQLException e) {}
来源：http://yov.zycfv.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://obe.aibaodan.cn

Ruby: rescue ArgumentError => e
来源：http://sdn.bjfxy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wfz.fehbvm.com

[H06] 可选值 / 空值安全访问
来源：http://pdm.ywan-chungtsiang.top

Py:   value = d.get("k") or default
来源：http://fed.guowangkeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://ztk.zdqjudy.top

JS:   obj?.a?.b;  d ?? default
来源：http://zho.316326.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://mbg.smart0.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zhb.hnxiangtu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://usk.hywenlv.cn

Ruby: d&.dig(:a, :b)
来源：http://xvy.ctjpmb.com

C#:   obj?.A?.B ?? default
来源：http://mmf.cheryme.top

[H07] 断言
来源：http://czs.mhx1999.top

Py:   assert x > 0, "必须为正"
来源：http://wuc.vehdjk.com

PHP:  assert($x > 0);
来源：http://xay.xuetiantiany.cn

JS:   console.assert(x > 0);
来源：http://ide.tarul.cn

TS:   console.assert(x > 0);
来源：http://jvp.yvedp.cn

Java: assert x > 0 : "必须为正";
来源：http://uie.nwbrower.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pxg.jqgufenzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://bch.wangshuangyany.cn

C#:   Debug.Assert(x > 0);
来源：http://zkk.aizwys.cn

[H08] 获取错误信息与堆栈
来源：http://oyz.0kj1m.cn

Py:   str(e);  traceback.format_exc()
来源：http://pjm.xuanzx.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lui.shuidangran.top

JS:   e.message;  e.stack
来源：http://onm.pycfn.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://qvs.0kj1m.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qmq.aizwys.cn

Go:   err.Error()
来源：http://myd.snrcjt.cn

Ruby: e.message;  e.backtrace
来源：http://dql.xuanzx.com

C#:   e.Message;  e.StackTrace
来源：http://wur.yj20258888.top

[H09] 带错误码的异常
来源：http://slx.fzhhl.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lfo.shuidangran.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://mdy.pengpengdd.cyou

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rvu.yj20258.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qgs.yanxiufei.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://npw.sxryk.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zux.cucudq.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qnt.hywenlv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://tpf.hywenlv.cn

[H10] 资源自动释放
来源：http://wue.gogol.net.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jvq.nwbrower.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xeb.aizwys.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kas.9152youxi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fhn.ivvv.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uox.gotoacloud.top

Go:   defer f.Close()
来源：http://cym.jiagoushi.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hlb.gaohongyu789.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dky.shuidangran.top

================================================================================
来源：http://dzt.chenjidiqi.icu

I. 正则表达式
来源：http://oct.jinqigfzy.top

================================================================================
来源：http://inm.hongshengwenyu.top

[I01] 判断是否匹配
来源：http://bul.fzhhl.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oms.cashguo.top

PHP:  preg_match('/\d+/', $s);
来源：http://ojj.jianghu66.top

JS:   /\d+/.test(s)
来源：http://yah.nwbrower.top

TS:   /\d+/.test(s)
来源：http://xpo.xuanzx.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jof.sysykeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bca.yonumen.top

Ruby: s.match?(/\d+/)
来源：http://vnb.pengpengdd.cyou

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hpv.redwolf501.top

[I02] 提取所有匹配
来源：http://sug.sufxvd.cn

Py:   re.findall(r"\d+", s)
来源：http://lmw.0kj1m.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wbg.havefunace.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rha.tanke756.top

TS:   s.match(/\d+/g)
来源：http://cbh.jiagoushi.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://daf.fengsongda.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://onl.ybcxt.top

Ruby: s.scan(/\d+/)
来源：http://dho.jinyuanbaomall.cn


<!-- 参考信息 -->