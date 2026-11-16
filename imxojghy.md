代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://qrp.nanxinkj.top

[F10] 取文件扩展名 / 文件名
来源：http://pzb.hysaishi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qgy.wangshuangyany.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ntc.hnqzz.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ovu.epnwcf.com

TS:   path.extname("a.txt")
来源：http://xzr.jiagoushi.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://saq.shangyingyoupin.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fxu.zhijiandao.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://eom.fanxiaobao.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ttw.shanyushiyangtech.top

[F11] 复制与移动文件
来源：http://vqk.chenjidiqi.icu

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zog.bjfxy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mmt.cqqwz.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dua.chenzaomai.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ntd.tianlin.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rpk.cucudq.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://djb.sysykeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tdr.yj202588.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://twa.ivvv.top

[F12] CSV 读写
来源：http://hrp.ctjpmb.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ujx.yonumen.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://swy.wangshuangyany.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wib.daria6918.cn

TS:   // 同上
来源：http://ube.jlsjyb.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://alh.aizwys.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wdl.jinyuanbaomall.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qmt.jinghuilouyu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cha.zdbjq.cn

================================================================================
来源：http://hbw.shanyushiyangkeji.top

G. 面向对象
来源：http://qhd.jinghuilouyu.cn

================================================================================
来源：http://wqp.zhengqikj.top

[G01] 定义类
来源：http://ixx.yj202588.top

Py:   class User: pass
来源：http://gzr.jqgufenzy.top

PHP:  class User {}
来源：http://ois.zdbjq.cn

JS:   class User {}
来源：http://jnk.bjfxy.top

TS:   class User { name: string = ""; }
来源：http://plj.tanke756.top

Java: class User {}
来源：http://pyj.xuetiantiany.cn

Go:   type User struct { Name string }
来源：http://ayu.jianghu66.top

Ruby: class User; end
来源：http://mjs.daxiang520.top

C#:   class User {}
来源：http://gxg.fehbvm.com

[G02] 构造函数
来源：http://ylq.yonumen.top

Py:   def __init__(self, name): self.name = name
来源：http://kaq.yangfankeji.com

PHP:  public function __construct(public string $name) {}
来源：http://gyh.pycfn.com

JS:   constructor(name) { this.name = name; }
来源：http://zvg.yj20258888.top

TS:   constructor(public name: string) {}
来源：http://hfj.zycfv.cn

Java: User(String name) { this.name = name; }
来源：http://ftw.cucudq.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hto.smart0.xyz

Ruby: def initialize(name); @name = name; end
来源：http://ezb.yfazqb.com

C#:   public User(string name) { Name = name; }
来源：http://ska.yanxiufei.cn

[G03] 实例属性
来源：http://jsr.yj202588.top

Py:   self.name = "x"
来源：http://qcf.wangdashe.top

PHP:  public string $name = "x";
来源：http://ctq.nanxuanxn.top

JS:   this.name = "x";
来源：http://jii.hysaishi.cn

TS:   name: string = "x";
来源：http://hfp.birdmap.top

Java: private String name;
来源：http://rda.bbcook.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ujq.snrcjt.cn

Ruby: @name = "x"
来源：http://sxo.ctjpmb.com

C#:   public string Name { get; set; } = "x";
来源：http://vkf.cucudq.cn

[G04] 定义方法
来源：http://tpz.fzhhl.top

Py:   def greet(self): return self.name
来源：http://nqk.yuanzhike.top

PHP:  public function greet(): string { return $this->name; }
来源：http://umu.hongshengwenyu.top

JS:   greet() { return this.name; }
来源：http://nir.sufxvd.cn

TS:   greet(): string { return this.name; }
来源：http://kki.bbcook.cn

Java: String greet() { return name; }
来源：http://ers.fengsongda.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://vnp.nanxinkj.top

Ruby: def greet; @name; end
来源：http://abx.meibo888.top

C#:   public string Greet() => Name;
来源：http://ull.jlsjyb.cn

[G05] 继承
来源：http://cbw.ybcxt.top

Py:   class Admin(User): pass
来源：http://wmq.redwolf501.top

PHP:  class Admin extends User {}
来源：http://hxs.yanxiufei.cn

JS:   class Admin extends User {}
来源：http://rck.xziqi.cn

TS:   class Admin extends User {}
来源：http://gdm.jianghu66.top

Java: class Admin extends User {}
来源：http://qjs.redwolf501.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pui.kuanghao11.cn

Ruby: class Admin < User; end
来源：http://jrb.yuanzhike.top

C#:   class Admin : User {}
来源：http://klo.zdbjq.cn

[G06] 重写方法
来源：http://ypf.ydjk.org.cn

Py:   def greet(self): return "admin"
来源：http://nuf.tarul.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sly.0kj1m.cn

JS:   greet() { return "admin"; }
来源：http://yju.jyoumei.cn

TS:   greet(): string { return "admin"; }
来源：http://xbe.smart0.xyz

Java: @Override String greet() { return "admin"; }
来源：http://cba.jinghuilouyu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qtk.tarul.cn

Ruby: def greet; "admin"; end
来源：http://uaj.hysaishi.cn

C#:   public override string Greet() => "admin";
来源：http://nhu.aizwys.cn

[G07] 调用父类方法
来源：http://zru.cheryme.top

Py:   super().greet()
来源：http://hoj.yangfankeji.com

PHP:  parent::greet();
来源：http://dac.xuanzx.com

JS:   super.greet();
来源：http://szr.ybcxt.top

TS:   super.greet();
来源：http://mpw.guannengcc.top

Java: super.greet();
来源：http://apk.bjfxy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zpu.gogol.net.cn

Ruby: super
来源：http://mjh.xziqi.cn

C#:   base.Greet();
来源：http://pvv.daxiang520.top

[G08] 静态方法与属性
来源：http://fty.yuanzhike.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rav.xinyue.icu

PHP:  public static function f() {}
来源：http://emc.cdnleiting.top

JS:   static f() {}
来源：http://dpq.andypj.xyz

TS:   static f(): void {}
来源：http://owo.zhixingplan.top

Java: static void f() {}
来源：http://lbw.zhixingplan.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://mpf.yanxiufei.cn

Ruby: def self.f; end
来源：http://vyq.hnqzz.top

C#:   public static void F() {}
来源：http://kfd.hnqzz.top

[G09] 接口 / 抽象类
来源：http://aky.gotoacloud.top

Py:   from abc import ABC, abstractmethod
来源：http://gjg.ehwqpu.com

PHP:  interface Shape { public function area(): float; }
来源：http://cdq.cheryme.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://dbr.xingfuxueyuan.xyz

TS:   interface Shape { area(): number; }
来源：http://hwm.chenlongwang.top

Java: interface Shape { double area(); }
来源：http://lhp.chenjidiqi.icu

Go:   type Shape interface { Area() float64 }
来源：http://pad.yanxiufei.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hvu.hysaishi.cn

C#:   interface IShape { double Area(); }
来源：http://kkz.zhijiandao.cn

[G10] 访问控制
来源：http://vcr.xuanzx.com

Py:   约定 _protected / __private（不强制）
来源：http://bfh.zdqjudy.top

PHP:  public / protected / private
来源：http://cwr.jiagoushi.top

JS:   #private 字段；其余公开
来源：http://ywt.hnxiangtu.top

TS:   public / protected / private
来源：http://hzc.hesvh.cn

Java: public / protected / private / 默认包级
来源：http://qdw.shanyushiyangkeji.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qrg.xziqi.cn

Ruby: public / protected / private
来源：http://ewf.c1oappe.top

C#:   public / protected / private / internal
来源：http://qxu.ehwqpu.com

[G11] getter / setter
来源：http://clz.smart0.xyz

Py:   @property 与 @x.setter
来源：http://wdo.ppjwa.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cyi.pengpengdd.cyou

JS:   get name() { return this._name; }
来源：http://rat.yfazqb.com

TS:   get name(): string { return this._name; }
来源：http://kue.xinyue.icu

Java: public String getName() { return name; }
来源：http://ojt.yfazqb.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://bad.tian-w.cn

Ruby: attr_accessor :name
来源：http://wpa.fzhhl.top

C#:   public string Name { get; set; }
来源：http://mkd.mhx1999.top

[G12] 对象转字符串
来源：http://bvm.hesvh.cn

Py:   def __str__(self): return self.name
来源：http://ced.tarul.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://djr.xuetiantiany.cn

JS:   toString() { return this.name; }
来源：http://abf.sweek.top

TS:   toString(): string { return this.name; }
来源：http://izr.jinghuilouyu.cn

Java: @Override public String toString() { return name; }
来源：http://zmv.nwbrower.top

Go:   func (u User) String() string { return u.Name }
来源：http://twl.quarkkingdee.top

Ruby: def to_s; @name; end
来源：http://zas.0kj1m.cn

C#:   public override string ToString() => Name;
来源：http://lqf.daxiang520.top

[G13] 判断对象类型
来源：http://ngr.yj20258888.top

Py:   isinstance(u, User)
来源：http://itm.jinyuanbaomall.cn

PHP:  $u instanceof User
来源：http://ujz.ivvv.top

JS:   u instanceof User
来源：http://vda.cdnleiting.top

TS:   u instanceof User
来源：http://wow.c1oappe.top

Java: u instanceof User
来源：http://wgp.sysykeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://nvi.bjfxy.top

Ruby: u.is_a?(User)
来源：http://udb.9152youxi.cn

C#:   u is User
来源：http://cak.yuanzhike.top

[G14] 数据类 / record
来源：http://tdq.jyoumei.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wwr.haohaochexian.top

PHP:  // 用 readonly 属性模拟
来源：http://fks.yuanzhike.top

JS:   // 无内置：普通类或对象字面量
来源：http://yoh.shanyushiyangkeji.top

TS:   type User = { name: string; age: number };
来源：http://kca.yj20258.top

Java: record User(String name, int age) {}
来源：http://wyo.yanxiufei.cn

Go:   type User struct { Name string; Age int }
来源：http://tnf.fengsongda.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mdi.chenlongwang.top

C#:   record User(string Name, int Age);
来源：http://ubq.zhiwuduotai.top

[G15] 枚举
来源：http://jka.9152youxi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tjp.jyoumei.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wma.shangyingyoupin.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nen.dashuyun.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lji.haohaochexian.top

Java: enum Color { RED, GREEN }
来源：http://wbe.hcnkem.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uio.c1oappe.top

Ruby: Color = %i[red green].freeze
来源：http://avy.zdbjq.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://clw.vehdjk.com

[G16] 对象转数组 / 字典
来源：http://aas.nanxinkj.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bnk.zhijiandao.cn

PHP:  get_object_vars($obj);
来源：http://jyd.nanxuanxn.top

JS:   Object.entries(obj)
来源：http://slo.zhaomingkeji.xyz

TS:   Object.entries(obj)
来源：http://gvm.nanxinkj.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pay.c1oappe.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://lhb.ivvv.top

Ruby: obj.instance_variables
来源：http://zhe.kuanghao11.cn

C#:   // 用反射或 System.Text.Json
来源：http://rqa.ydzc1.top

================================================================================
来源：http://wck.hesvh.cn

H. 异常与错误处理
来源：http://ltp.cdnleiting.top

================================================================================
来源：http://brw.hammf.cn

[H01] try / catch 基础
来源：http://efi.chenjidiqi.icu

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ydc.0kj1m.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pjp.xingfuxueyuan.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kzp.bjfxy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sph.nanxinkj.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hhx.tianlin.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kib.yj202588.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://via.xinyue.icu

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vuv.smart0.xyz

[H02] finally / ensure 收尾
来源：http://coe.jyoumei.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rru.zhengqikj.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vko.fehbvm.com

JS:   try { f(); } finally { cleanup(); }
来源：http://dam.smart0.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://tvi.guowangkeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://ybx.vqdsnc.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sfl.kuanghao11.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://cev.xylfe.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://asx.fehbvm.com

[H03] 主动抛出异常
来源：http://ncs.guowangkeji.top

Py:   raise ValueError("错误信息")
来源：http://nju.xuetiantiany.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vdq.sweek.top

JS:   throw new Error("错误信息");
来源：http://djj.shanyushiyangkeji.top

TS:   throw new Error("错误信息");
来源：http://cbp.daria6918.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yif.c1oappe.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jvg.9152youxi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qqj.vqdsnc.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ryc.gaohongyu789.top

[H04] 自定义异常类型
来源：http://uxn.zhixingplan.top

Py:   class MyError(Exception): pass
来源：http://xgm.cqqwz.cn

PHP:  class MyError extends RuntimeException {}
来源：http://iac.haohaochexian.top

JS:   class MyError extends Error {}
来源：http://fdt.c1oappe.top

TS:   class MyError extends Error {}
来源：http://qfk.jlsjyb.cn

Java: class MyException extends RuntimeException {}
来源：http://ppz.smart0.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lvw.jinyuanbaomall.cn

Ruby: class MyError < StandardError; end
来源：http://mkh.kuanghao11.cn

C#:   class MyException : Exception {}
来源：http://cti.wangshuangyany.cn

[H05] 捕获特定类型
来源：http://dtb.daria6918.cn

Py:   except ValueError as e:
来源：http://upr.sysykeji.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://umt.tanke756.top

JS:   if (e instanceof TypeError) {}
来源：http://vrp.andypj.xyz

TS:   if (e instanceof TypeError) {}
来源：http://iex.redwolf501.top

Java: catch (IOException | SQLException e) {}
来源：http://ukt.vqdsnc.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pri.nwbrower.top

Ruby: rescue ArgumentError => e
来源：http://hbx.smart0.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cyq.yuxming.cn

[H06] 可选值 / 空值安全访问
来源：http://vor.zycfv.cn

Py:   value = d.get("k") or default
来源：http://dlk.zhaomingkeji.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://ylk.quarkkingdee.top

JS:   obj?.a?.b;  d ?? default
来源：http://vtw.ivvv.top

TS:   obj?.a?.b;  d ?? default
来源：http://kbx.cucudq.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ezw.c1oappe.top

Go:   if v, ok := m["k"]; ok { }
来源：http://tpv.jinghuilouyu.cn

Ruby: d&.dig(:a, :b)
来源：http://fpu.sysykeji.top

C#:   obj?.A?.B ?? default
来源：http://apn.nanxuanxn.top

[H07] 断言
来源：http://xqe.hfpthk.cn

Py:   assert x > 0, "必须为正"
来源：http://lcv.vqdsnc.cn

PHP:  assert($x > 0);
来源：http://sts.mhx1999.top

JS:   console.assert(x > 0);
来源：http://hvh.cqqwz.cn

TS:   console.assert(x > 0);
来源：http://igo.haohaochexian.top

Java: assert x > 0 : "必须为正";
来源：http://rxq.nanxuanxn.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ook.dashuyun.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gsv.ywan-chungtsiang.top

C#:   Debug.Assert(x > 0);
来源：http://xvy.fzhhl.top

[H08] 获取错误信息与堆栈
来源：http://ieo.gotoacloud.top

Py:   str(e);  traceback.format_exc()
来源：http://vof.316326.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ejp.yj20258.top

JS:   e.message;  e.stack
来源：http://mly.haohaochexian.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://wvy.feifeiyinyue.top

Java: e.getMessage();  e.printStackTrace()
来源：http://sec.zycfv.cn

Go:   err.Error()
来源：http://lvz.zhixingplan.top

Ruby: e.message;  e.backtrace
来源：http://uai.birdmap.top

C#:   e.Message;  e.StackTrace
来源：http://zuk.jlsjyb.cn

[H09] 带错误码的异常
来源：http://qaa.jinghuilouyu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pwu.yvedp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://chk.meibo888.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://szt.hesvh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kcs.shzxlz.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nqf.yj20258.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xir.0kj1m.cn

Ruby: raise MyError.new("fail", 500)
来源：http://sku.sxryk.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jzn.dashuyun.cn

[H10] 资源自动释放
来源：http://cwt.hfpthk.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pmm.gzhubu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://eem.zdqjudy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bau.aibaodan.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wlv.hesvh.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jrd.hnqzz.top

Go:   defer f.Close()
来源：http://wjz.uphjek.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cin.yuanzhike.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://arm.zdbjq.cn

================================================================================
来源：http://exf.nwbrower.top

I. 正则表达式
来源：http://kfp.jinqigufen.top

================================================================================
来源：http://ehg.xziqi.cn

[I01] 判断是否匹配
来源：http://qzl.tanke756.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uwp.cucudq.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gpt.sysykeji.top

JS:   /\d+/.test(s)
来源：http://qev.ppjwa.cn

TS:   /\d+/.test(s)
来源：http://jtv.zycfv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kki.zdbjq.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://erz.meibo888.top

Ruby: s.match?(/\d+/)
来源：http://zon.shangyingyoupin.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jwj.ywan-chungtsiang.top

[I02] 提取所有匹配
来源：http://kqt.bbcook.cn

Py:   re.findall(r"\d+", s)
来源：http://wzp.jinqigufen.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sfp.wangdashe.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qtg.sufxvd.cn

TS:   s.match(/\d+/g)
来源：http://nqh.chenzaomai.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zsg.fehbvm.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hug.hammf.cn

Ruby: s.scan(/\d+/)
来源：http://kdf.hesvh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vru.hywenlv.cn

[I03] 提取捕获分组
来源：http://kln.yfazqb.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pip.zhijiandao.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://afe.havefunace.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gif.zdqjudy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sdm.zhengqikj.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://skh.zhongyouzk.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ijb.nwbrower.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tti.redwolf501.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://otp.havefunace.top

[I04] 正则替换
来源：http://uqo.zhaomingkeji.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://qsi.chenlongwang.top


<!-- 参考信息 -->