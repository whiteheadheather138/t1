代发 wailian999

[F09] 获取文件大小
来源：http://neu.gaohongyu789.top

Py:   os.path.getsize("a.txt")
来源：http://adx.yj20258888.top

PHP:  filesize("a.txt");
来源：http://gvw.yj20258.top

JS:   fs.statSync("a.txt").size
来源：http://jjc.vehdjk.com

TS:   fs.statSync("a.txt").size
来源：http://fns.smart0.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://mye.dianchejie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lts.hesvh.cn

Ruby: File.size("a.txt")
来源：http://aar.cashguo.top

C#:   new FileInfo("a.txt").Length
来源：http://wfr.dashuyun.cn

[F10] 取文件扩展名 / 文件名
来源：http://ttc.sweek.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hav.guannengcc.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uab.tanke756.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wyy.sysykeji.top

TS:   path.extname("a.txt")
来源：http://hdr.jinqigufen.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ner.ydzc1.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xin.ywan-chungtsiang.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kbf.chenlongwang.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ecn.yueranfly.top

[F11] 复制与移动文件
来源：http://bea.bbcook.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://orl.jianghu66.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kic.nanxuanxn.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kib.aizwys.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qsm.hfpthk.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ixn.yueranfly.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bgf.chenzaomai.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yrw.pengpengdd.cyou

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://iah.shanyushiyangkeji.top

[F12] CSV 读写
来源：http://ksp.mhx1999.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zjn.fanxiaobao.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://enq.sjlbkw.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wlb.jinghuilouyu.cn

TS:   // 同上
来源：http://vrz.gaohongyu789.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vbe.tarul.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sid.epnwcf.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wuy.hfpthk.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://drm.sjlbkw.cn

================================================================================
来源：http://znv.vqdsnc.cn

G. 面向对象
来源：http://nfk.snrcjt.cn

================================================================================
来源：http://fug.smart0.xyz

[G01] 定义类
来源：http://adu.9152youxi.cn

Py:   class User: pass
来源：http://sjh.gotoacloud.top

PHP:  class User {}
来源：http://msn.aibaodan.cn

JS:   class User {}
来源：http://cbv.snrcjt.cn

TS:   class User { name: string = ""; }
来源：http://gya.bjfxy.top

Java: class User {}
来源：http://vkq.52xcode.cn

Go:   type User struct { Name string }
来源：http://vhr.zdbjq.cn

Ruby: class User; end
来源：http://vll.shanyushiyangtech.top

C#:   class User {}
来源：http://gdx.cashguo.top

[G02] 构造函数
来源：http://zvs.epnwcf.com

Py:   def __init__(self, name): self.name = name
来源：http://frr.xylfe.cn

PHP:  public function __construct(public string $name) {}
来源：http://iim.shangyingyoupin.top

JS:   constructor(name) { this.name = name; }
来源：http://xmc.chenjidiqi.icu

TS:   constructor(public name: string) {}
来源：http://jsh.sweek.top

Java: User(String name) { this.name = name; }
来源：http://kek.0kj1m.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tcx.ivvv.top

Ruby: def initialize(name); @name = name; end
来源：http://kif.zdqjudy.top

C#:   public User(string name) { Name = name; }
来源：http://dbk.jinghuilouyu.cn

[G03] 实例属性
来源：http://uvl.nanxuanxn.top

Py:   self.name = "x"
来源：http://yvv.zhoulong.xyz

PHP:  public string $name = "x";
来源：http://vjd.yj20258.top

JS:   this.name = "x";
来源：http://xlr.sxryk.cn

TS:   name: string = "x";
来源：http://dlo.fanxiaobao.xyz

Java: private String name;
来源：http://hmj.feifeiyinyue.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tjq.hywenlv.cn

Ruby: @name = "x"
来源：http://txx.dianchejie.cn

C#:   public string Name { get; set; } = "x";
来源：http://gdz.jinqigufen.top

[G04] 定义方法
来源：http://dzp.yangfankeji.com

Py:   def greet(self): return self.name
来源：http://ows.mhx1999.top

PHP:  public function greet(): string { return $this->name; }
来源：http://pkq.hnqzz.top

JS:   greet() { return this.name; }
来源：http://xcv.tarul.cn

TS:   greet(): string { return this.name; }
来源：http://pcg.iojbl.cn

Java: String greet() { return name; }
来源：http://rsb.birdmap.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://nug.cdnleiting.top

Ruby: def greet; @name; end
来源：http://ixz.andypj.xyz

C#:   public string Greet() => Name;
来源：http://jpy.ppjwa.cn

[G05] 继承
来源：http://epf.yangfankeji.com

Py:   class Admin(User): pass
来源：http://klt.aizwys.cn

PHP:  class Admin extends User {}
来源：http://uaz.zhijiandao.cn

JS:   class Admin extends User {}
来源：http://xxm.yonumen.top

TS:   class Admin extends User {}
来源：http://xkf.hesvh.cn

Java: class Admin extends User {}
来源：http://rub.birdmap.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dve.yueranfly.top

Ruby: class Admin < User; end
来源：http://uew.ydjk.org.cn

C#:   class Admin : User {}
来源：http://fom.gaohongyu789.top

[G06] 重写方法
来源：http://wsc.yongpay.top

Py:   def greet(self): return "admin"
来源：http://dyq.ctjpmb.com

PHP:  public function greet(): string { return "admin"; }
来源：http://yvf.yvedp.cn

JS:   greet() { return "admin"; }
来源：http://sxe.cheryme.top

TS:   greet(): string { return "admin"; }
来源：http://otb.shuidangran.top

Java: @Override String greet() { return "admin"; }
来源：http://sjh.uphjek.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mwe.xuetiantiany.cn

Ruby: def greet; "admin"; end
来源：http://scq.bbcook.cn

C#:   public override string Greet() => "admin";
来源：http://kfj.yanxiufei.cn

[G07] 调用父类方法
来源：http://jiv.daxiang520.top

Py:   super().greet()
来源：http://qdu.52xcode.cn

PHP:  parent::greet();
来源：http://cja.dashuyun.cn

JS:   super.greet();
来源：http://fao.vqdsnc.cn

TS:   super.greet();
来源：http://gum.yueranfly.top

Java: super.greet();
来源：http://twu.wangshuangyany.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rif.hesvh.cn

Ruby: super
来源：http://rfk.xuanzx.com

C#:   base.Greet();
来源：http://hli.xuanzx.com

[G08] 静态方法与属性
来源：http://vvc.jianghu66.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hlm.shangyingyoupin.top

PHP:  public static function f() {}
来源：http://gkp.kuanghao11.cn

JS:   static f() {}
来源：http://ydt.meibo888.top

TS:   static f(): void {}
来源：http://dqu.smart0.xyz

Java: static void f() {}
来源：http://txv.dashuyun.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://lqj.fehbvm.com

Ruby: def self.f; end
来源：http://nrw.zhengqikj.top

C#:   public static void F() {}
来源：http://yoa.zhixingplan.top

[G09] 接口 / 抽象类
来源：http://vkq.pycfn.com

Py:   from abc import ABC, abstractmethod
来源：http://uxt.jyoumei.cn

PHP:  interface Shape { public function area(): float; }
来源：http://kwo.sjlbkw.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rix.gzhubu.top

TS:   interface Shape { area(): number; }
来源：http://pin.mhx1999.top

Java: interface Shape { double area(); }
来源：http://ped.havefunace.top

Go:   type Shape interface { Area() float64 }
来源：http://ghn.ydzc1.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rjs.ehwqpu.com

C#:   interface IShape { double Area(); }
来源：http://jdk.gogol.net.cn

[G10] 访问控制
来源：http://zts.jinqigfzy.top

Py:   约定 _protected / __private（不强制）
来源：http://oqm.ppjwa.cn

PHP:  public / protected / private
来源：http://pha.tianlin.xyz

JS:   #private 字段；其余公开
来源：http://zvs.cdnleiting.top

TS:   public / protected / private
来源：http://nou.cheryme.top

Java: public / protected / private / 默认包级
来源：http://poy.andypj.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://wej.tanke756.top

Ruby: public / protected / private
来源：http://gys.haohaochexian.top

C#:   public / protected / private / internal
来源：http://roq.hfpthk.cn

[G11] getter / setter
来源：http://svk.pycfn.com

Py:   @property 与 @x.setter
来源：http://nmd.jqgfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dfs.yj202588.top

JS:   get name() { return this._name; }
来源：http://ehl.zhixingplan.top

TS:   get name(): string { return this._name; }
来源：http://xlb.zycfv.cn

Java: public String getName() { return name; }
来源：http://ayb.daria6918.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://enj.ybcxt.top

Ruby: attr_accessor :name
来源：http://fms.xingfuxueyuan.xyz

C#:   public string Name { get; set; }
来源：http://lnv.zhoulong.xyz

[G12] 对象转字符串
来源：http://vfx.gotoacloud.top

Py:   def __str__(self): return self.name
来源：http://iif.feifeiyinyue.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://fmy.cdnleiting.top

JS:   toString() { return this.name; }
来源：http://sfl.havefunace.top

TS:   toString(): string { return this.name; }
来源：http://jca.yj20258.top

Java: @Override public String toString() { return name; }
来源：http://kfv.9152youxi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vfz.xinyue.icu

Ruby: def to_s; @name; end
来源：http://zem.snrcjt.cn

C#:   public override string ToString() => Name;
来源：http://mke.xuanzx.com

[G13] 判断对象类型
来源：http://crp.hnxiangtu.top

Py:   isinstance(u, User)
来源：http://bcr.hfpthk.cn

PHP:  $u instanceof User
来源：http://nmk.0kj1m.cn

JS:   u instanceof User
来源：http://ztn.hnqzz.top

TS:   u instanceof User
来源：http://lmc.andypj.xyz

Java: u instanceof User
来源：http://nsh.tanke756.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://zuj.ybcxt.top

Ruby: u.is_a?(User)
来源：http://rad.haohaochexian.top

C#:   u is User
来源：http://lvz.sufxvd.cn

[G14] 数据类 / record
来源：http://abc.gzhubu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://goh.ehwqpu.com

PHP:  // 用 readonly 属性模拟
来源：http://egu.jqgufenzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://myz.pengpengdd.cyou

TS:   type User = { name: string; age: number };
来源：http://ehw.ybcxt.top

Java: record User(String name, int age) {}
来源：http://ylq.redwolf501.top

Go:   type User struct { Name string; Age int }
来源：http://mdx.meibo888.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wrx.ctjpmb.com

C#:   record User(string Name, int Age);
来源：http://lzf.c1oappe.top

[G15] 枚举
来源：http://jwt.ybcxt.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qho.ppjwa.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dpe.cashguo.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hqv.sxryk.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://oyf.ydjk.org.cn

Java: enum Color { RED, GREEN }
来源：http://vth.chenjidiqi.icu

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ktq.xziqi.cn

Ruby: Color = %i[red green].freeze
来源：http://rtk.yuanzhike.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ktl.svipenyu.cn

[G16] 对象转数组 / 字典
来源：http://wbt.wangshuangyany.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wuc.hcnkem.com

PHP:  get_object_vars($obj);
来源：http://osa.hammf.cn

JS:   Object.entries(obj)
来源：http://ykq.ehwqpu.com

TS:   Object.entries(obj)
来源：http://eex.guannengcc.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zrr.zhijiandao.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://aks.hesvh.cn

Ruby: obj.instance_variables
来源：http://jfu.meibo888.top

C#:   // 用反射或 System.Text.Json
来源：http://ohr.yuxming.cn

================================================================================
来源：http://oos.andypj.xyz

H. 异常与错误处理
来源：http://stg.birdmap.top

================================================================================
来源：http://hgu.jqgfzy.top

[H01] try / catch 基础
来源：http://tbf.birdmap.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uix.jiagoushi.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pei.hnxiangtu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xxu.chenjidiqi.icu

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xqr.andypj.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://afw.hysaishi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://iql.cucudq.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dbm.andypj.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cej.yueranfly.top

[H02] finally / ensure 收尾
来源：http://ihy.wangshuangyany.cn

Py:   try: f()⏎finally: cleanup()
来源：http://bsz.ctjpmb.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://aek.wangshuangyany.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fdt.hongshengwenyu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ohk.wangdashe.top

Java: try { f(); } finally { cleanup(); }
来源：http://srg.kuanghao11.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ges.feifeiyinyue.top

Ruby: begin; f; ensure; cleanup; end
来源：http://xmq.tianlin.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://rzn.iojbl.cn

[H03] 主动抛出异常
来源：http://mrv.bjfxy.top

Py:   raise ValueError("错误信息")
来源：http://jio.ehwqpu.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qzk.andypj.xyz

JS:   throw new Error("错误信息");
来源：http://xjs.jyoumei.cn

TS:   throw new Error("错误信息");
来源：http://nio.kuanghao11.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://thf.redwolf501.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yhw.tarul.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://aku.nwbrower.top

C#:   throw new ArgumentException("错误信息");
来源：http://nof.hfpthk.cn

[H04] 自定义异常类型
来源：http://prs.ctjpmb.com

Py:   class MyError(Exception): pass
来源：http://arc.jqgfzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://khr.chenzaomai.com

JS:   class MyError extends Error {}
来源：http://xoo.ppjwa.cn

TS:   class MyError extends Error {}
来源：http://zud.hcnkem.com

Java: class MyException extends RuntimeException {}
来源：http://djp.nwbrower.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xkc.pycfn.com

Ruby: class MyError < StandardError; end
来源：http://rcr.chenlongwang.top

C#:   class MyException : Exception {}
来源：http://zje.zhengqikj.top

[H05] 捕获特定类型
来源：http://zya.dashuyun.cn

Py:   except ValueError as e:
来源：http://ful.iojbl.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fsy.tanke756.top

JS:   if (e instanceof TypeError) {}
来源：http://gcf.feifeiyinyue.top

TS:   if (e instanceof TypeError) {}
来源：http://mmo.yangfankeji.com

Java: catch (IOException | SQLException e) {}
来源：http://nph.fehbvm.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mem.tian-w.cn

Ruby: rescue ArgumentError => e
来源：http://iiu.xylfe.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hhg.ppjwa.cn

[H06] 可选值 / 空值安全访问
来源：http://flv.shuidangran.top

Py:   value = d.get("k") or default
来源：http://eoz.zdqjudy.top

PHP:  $v = $d["k"] ?? null;
来源：http://zkc.haohaochexian.top

JS:   obj?.a?.b;  d ?? default
来源：http://ozt.guowangkeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://rkb.sxryk.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://iqu.sxryk.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ihv.nanxinkj.top

Ruby: d&.dig(:a, :b)
来源：http://cuj.zhijiandao.cn

C#:   obj?.A?.B ?? default
来源：http://xqs.vehdjk.com

[H07] 断言
来源：http://lkb.sweek.top

Py:   assert x > 0, "必须为正"
来源：http://auy.jyoumei.cn

PHP:  assert($x > 0);
来源：http://tdj.xuanzx.com

JS:   console.assert(x > 0);
来源：http://lyi.yanxiufei.cn

TS:   console.assert(x > 0);
来源：http://bvg.epnwcf.com

Java: assert x > 0 : "必须为正";
来源：http://pyg.jqgufenzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zbg.iojbl.cn

Ruby: raise "必须为正" unless x > 0
来源：http://sjk.jqgfzy.top

C#:   Debug.Assert(x > 0);
来源：http://hvx.zycfv.cn

[H08] 获取错误信息与堆栈
来源：http://got.yangfankeji.com

Py:   str(e);  traceback.format_exc()
来源：http://btb.chenlongwang.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fyr.snrcjt.cn

JS:   e.message;  e.stack
来源：http://exw.ehwqpu.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://gfd.yvedp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mic.sjlbkw.cn

Go:   err.Error()
来源：http://fqy.haohaochexian.top

Ruby: e.message;  e.backtrace
来源：http://htn.zdqjudy.top

C#:   e.Message;  e.StackTrace
来源：http://btc.jinqigfzy.top

[H09] 带错误码的异常
来源：http://ugx.xziqi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://psj.zhaomingkeji.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://qrd.shzxlz.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sxw.birdmap.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nxt.yonumen.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dcd.zhixingplan.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uuf.wangdashe.top

Ruby: raise MyError.new("fail", 500)
来源：http://fik.xuetiantiany.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://eqg.xinyue.icu

[H10] 资源自动释放
来源：http://rfc.xylfe.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://cli.mhx1999.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nca.nanxuanxn.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kad.sweek.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fax.ydzc1.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yus.ywan-chungtsiang.top

Go:   defer f.Close()
来源：http://hdy.mhx1999.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zpx.yfazqb.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://llc.sweek.top

================================================================================
来源：http://arb.xylfe.cn

I. 正则表达式
来源：http://whk.zhijiandao.cn

================================================================================
来源：http://kvh.haohaochexian.top

[I01] 判断是否匹配
来源：http://lqy.gogol.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yxn.ctjpmb.com

PHP:  preg_match('/\d+/', $s);
来源：http://pup.52xcode.cn

JS:   /\d+/.test(s)
来源：http://ldd.havefunace.top

TS:   /\d+/.test(s)
来源：http://voe.cheryme.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pyi.pycfn.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://aje.chenzaomai.com

Ruby: s.match?(/\d+/)
来源：http://wdt.jinqigufen.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mza.havefunace.top

[I02] 提取所有匹配
来源：http://hmu.jlsjyb.cn

Py:   re.findall(r"\d+", s)
来源：http://mnn.hnqzz.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lnp.zhengqikj.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gfy.dianchejie.cn

TS:   s.match(/\d+/g)
来源：http://kyw.hywenlv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://slc.tian-w.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://emk.yuanzhike.top

Ruby: s.scan(/\d+/)
来源：http://lvn.havefunace.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://emd.yfazqb.com

[I03] 提取捕获分组
来源：http://nac.xuanzx.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kpw.ydjk.org.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fpe.cqqwz.cn


<!-- 参考信息 -->