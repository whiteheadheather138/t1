代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zit.wangdashe.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://crf.zhoulong.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://guv.yj20258.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wug.jiagoushi.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dur.jinqigfzy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dlc.ybcxt.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gdm.xinyue.icu

[F08] 遍历目录
来源：http://qrz.chenlongwang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://pzc.jqgufenzy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jsb.ehwqpu.com

JS:   fs.readdirSync("dir")
来源：http://gvu.jqgfzy.top

TS:   fs.readdirSync("dir")
来源：http://cxe.hfpthk.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fvx.zhoulong.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://peu.xylfe.cn

Ruby: Dir.children("dir")
来源：http://obv.bbcook.cn

C#:   Directory.GetFiles("dir")
来源：http://vat.jqgufenzy.top

[F09] 获取文件大小
来源：http://ahs.cucudq.cn

Py:   os.path.getsize("a.txt")
来源：http://vsh.fktsv.cn

PHP:  filesize("a.txt");
来源：http://ryg.zdqjudy.top

JS:   fs.statSync("a.txt").size
来源：http://cnz.zhijiandao.cn

TS:   fs.statSync("a.txt").size
来源：http://rgz.gogol.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ovg.dashuyun.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rgc.fehbvm.com

Ruby: File.size("a.txt")
来源：http://kcm.gaohongyu789.top

C#:   new FileInfo("a.txt").Length
来源：http://wlv.yuxming.cn

[F10] 取文件扩展名 / 文件名
来源：http://uoc.jinghuilouyu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vzh.cqqwz.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kox.pycfn.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vec.52xcode.cn

TS:   path.extname("a.txt")
来源：http://npx.ybcxt.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ftt.daxiang520.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cjt.jlsjyb.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mee.gaohongyu789.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ned.zdbjq.cn

[F11] 复制与移动文件
来源：http://vwz.iojbl.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gef.yuanzhike.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bmm.shuidangran.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ber.shanyushiyangtech.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qwu.gotoacloud.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ugr.redwolf501.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nop.ywan-chungtsiang.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kpn.yuxming.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bzb.pengpengdd.cyou

[F12] CSV 读写
来源：http://rio.jyoumei.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bjb.zhijiandao.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fvm.fengsongda.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cad.ydzc1.top

TS:   // 同上
来源：http://vhz.daria6918.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://okj.jqgufenzy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dtv.shanyushiyangkeji.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://chm.vehdjk.com

C#:   // 无内置：用 CsvHelper 库
来源：http://rrn.hnxiangtu.top

================================================================================
来源：http://khz.havefunace.top

G. 面向对象
来源：http://qis.jinqigfzy.top

================================================================================
来源：http://yde.ybcxt.top

[G01] 定义类
来源：http://yhj.cdnleiting.top

Py:   class User: pass
来源：http://otl.hesvh.cn

PHP:  class User {}
来源：http://rhc.epnwcf.com

JS:   class User {}
来源：http://row.xingfuxueyuan.xyz

TS:   class User { name: string = ""; }
来源：http://gti.hywenlv.cn

Java: class User {}
来源：http://bvq.smart0.xyz

Go:   type User struct { Name string }
来源：http://tpl.shzxlz.cn

Ruby: class User; end
来源：http://sly.hnxiangtu.top

C#:   class User {}
来源：http://soj.pycfn.com

[G02] 构造函数
来源：http://spl.hesvh.cn

Py:   def __init__(self, name): self.name = name
来源：http://geq.feifeiyinyue.top

PHP:  public function __construct(public string $name) {}
来源：http://tpi.gotoacloud.top

JS:   constructor(name) { this.name = name; }
来源：http://zrh.jiagoushi.top

TS:   constructor(public name: string) {}
来源：http://mnu.cashguo.top

Java: User(String name) { this.name = name; }
来源：http://pgm.hongshengwenyu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wal.smart0.xyz

Ruby: def initialize(name); @name = name; end
来源：http://umk.fehbvm.com

C#:   public User(string name) { Name = name; }
来源：http://nkz.jqgfzy.top

[G03] 实例属性
来源：http://map.gogol.net.cn

Py:   self.name = "x"
来源：http://eqp.hcnkem.com

PHP:  public string $name = "x";
来源：http://his.pengpengdd.cyou

JS:   this.name = "x";
来源：http://uzz.iojbl.cn

TS:   name: string = "x";
来源：http://uze.chenzaomai.com

Java: private String name;
来源：http://icb.hammf.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kto.fehbvm.com

Ruby: @name = "x"
来源：http://erm.fanxiaobao.xyz

C#:   public string Name { get; set; } = "x";
来源：http://acb.yj202588.top

[G04] 定义方法
来源：http://kop.pengpengdd.cyou

Py:   def greet(self): return self.name
来源：http://eai.fanxiaobao.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://cqx.yuxming.cn

JS:   greet() { return this.name; }
来源：http://kjl.haohaochexian.top

TS:   greet(): string { return this.name; }
来源：http://eaf.vqdsnc.cn

Java: String greet() { return name; }
来源：http://kwq.ctjpmb.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://yru.tarul.cn

Ruby: def greet; @name; end
来源：http://tfa.zhijiandao.cn

C#:   public string Greet() => Name;
来源：http://cxk.smart0.xyz

[G05] 继承
来源：http://mwl.iojbl.cn

Py:   class Admin(User): pass
来源：http://ilu.yuxming.cn

PHP:  class Admin extends User {}
来源：http://szp.hesvh.cn

JS:   class Admin extends User {}
来源：http://eas.haohaochexian.top

TS:   class Admin extends User {}
来源：http://khw.yj20258.top

Java: class Admin extends User {}
来源：http://zwm.sxryk.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xll.cashguo.top

Ruby: class Admin < User; end
来源：http://wdu.kuanghao11.cn

C#:   class Admin : User {}
来源：http://wxh.jyoumei.cn

[G06] 重写方法
来源：http://mux.ehwqpu.com

Py:   def greet(self): return "admin"
来源：http://fdd.9152youxi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nql.birdmap.top

JS:   greet() { return "admin"; }
来源：http://xal.zycfv.cn

TS:   greet(): string { return "admin"; }
来源：http://ppv.sxryk.cn

Java: @Override String greet() { return "admin"; }
来源：http://pzl.ydjk.org.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wse.xylfe.cn

Ruby: def greet; "admin"; end
来源：http://mjr.zdbjq.cn

C#:   public override string Greet() => "admin";
来源：http://tgk.epnwcf.com

[G07] 调用父类方法
来源：http://mgo.zycfv.cn

Py:   super().greet()
来源：http://zaq.tianlin.xyz

PHP:  parent::greet();
来源：http://lic.yuanzhike.top

JS:   super.greet();
来源：http://fwq.zhijiandao.cn

TS:   super.greet();
来源：http://uan.zycfv.cn

Java: super.greet();
来源：http://paw.yj20258888.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xgc.shanyushiyangtech.top

Ruby: super
来源：http://lvu.tanke756.top

C#:   base.Greet();
来源：http://xrp.fzhhl.top

[G08] 静态方法与属性
来源：http://fvq.jlsjyb.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lbc.haohaochexian.top

PHP:  public static function f() {}
来源：http://qjq.sweek.top

JS:   static f() {}
来源：http://qmo.hnqzz.top

TS:   static f(): void {}
来源：http://hbg.0kj1m.cn

Java: static void f() {}
来源：http://jav.shzxlz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ovu.jianghu66.top

Ruby: def self.f; end
来源：http://hoo.yfazqb.com

C#:   public static void F() {}
来源：http://eyz.shuidangran.top

[G09] 接口 / 抽象类
来源：http://akh.zhoulong.xyz

Py:   from abc import ABC, abstractmethod
来源：http://xoo.dianchejie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gyh.ybcxt.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://oip.cdnleiting.top

TS:   interface Shape { area(): number; }
来源：http://atn.gogol.net.cn

Java: interface Shape { double area(); }
来源：http://gfx.feifeiyinyue.top

Go:   type Shape interface { Area() float64 }
来源：http://gbh.bjfxy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rsn.tarul.cn

C#:   interface IShape { double Area(); }
来源：http://jit.aibaodan.cn

[G10] 访问控制
来源：http://eyk.316326.xyz

Py:   约定 _protected / __private（不强制）
来源：http://vpw.zhixingplan.top

PHP:  public / protected / private
来源：http://rgs.sweek.top

JS:   #private 字段；其余公开
来源：http://gef.zdqjudy.top

TS:   public / protected / private
来源：http://ara.nwbrower.top

Java: public / protected / private / 默认包级
来源：http://xrm.shuidangran.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://tpj.aizwys.cn

Ruby: public / protected / private
来源：http://wki.birdmap.top

C#:   public / protected / private / internal
来源：http://zdw.havefunace.top

[G11] getter / setter
来源：http://nxb.zhaomingkeji.xyz

Py:   @property 与 @x.setter
来源：http://glk.jqgfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://zos.nanxinkj.top

JS:   get name() { return this._name; }
来源：http://wfn.zhijiandao.cn

TS:   get name(): string { return this._name; }
来源：http://jks.cashguo.top

Java: public String getName() { return name; }
来源：http://btx.ydzc1.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://lfr.fzhhl.top

Ruby: attr_accessor :name
来源：http://nef.jinqigufen.top

C#:   public string Name { get; set; }
来源：http://ivj.jinyuanbaomall.cn

[G12] 对象转字符串
来源：http://blg.nanxinkj.top

Py:   def __str__(self): return self.name
来源：http://qel.meibo888.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://gvs.hfpthk.cn

JS:   toString() { return this.name; }
来源：http://xhx.redwolf501.top

TS:   toString(): string { return this.name; }
来源：http://mmt.fehbvm.com

Java: @Override public String toString() { return name; }
来源：http://orf.fktsv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bjg.shuidangran.top

Ruby: def to_s; @name; end
来源：http://aik.jinghuilouyu.cn

C#:   public override string ToString() => Name;
来源：http://asg.sufxvd.cn

[G13] 判断对象类型
来源：http://bia.daria6918.cn

Py:   isinstance(u, User)
来源：http://hvx.shuidangran.top

PHP:  $u instanceof User
来源：http://bgq.hongshengwenyu.top

JS:   u instanceof User
来源：http://xxt.cdnleiting.top

TS:   u instanceof User
来源：http://qwm.gotoacloud.top

Java: u instanceof User
来源：http://akx.yonumen.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://olw.tianlin.xyz

Ruby: u.is_a?(User)
来源：http://rir.zdbjq.cn

C#:   u is User
来源：http://qyf.hfpthk.cn

[G14] 数据类 / record
来源：http://ybn.yvedp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bkm.zhoulong.xyz

PHP:  // 用 readonly 属性模拟
来源：http://uni.yvedp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gro.shanyushiyangtech.top

TS:   type User = { name: string; age: number };
来源：http://ahg.tian-w.cn

Java: record User(String name, int age) {}
来源：http://uza.tarul.cn

Go:   type User struct { Name string; Age int }
来源：http://ddj.yangfankeji.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xma.jlsjyb.cn

C#:   record User(string Name, int Age);
来源：http://ptz.xinyue.icu

[G15] 枚举
来源：http://eyt.tarul.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fsv.fehbvm.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://xxx.hnxiangtu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://opf.yanxiufei.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sbl.guannengcc.top

Java: enum Color { RED, GREEN }
来源：http://myj.meibo888.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gwu.fanxiaobao.xyz

Ruby: Color = %i[red green].freeze
来源：http://mth.svipenyu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xhe.xingfuxueyuan.xyz

[G16] 对象转数组 / 字典
来源：http://cic.xinyue.icu

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://oeu.hcnkem.com

PHP:  get_object_vars($obj);
来源：http://fba.yongpay.top

JS:   Object.entries(obj)
来源：http://rrl.yj202588.top

TS:   Object.entries(obj)
来源：http://egh.uphjek.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://avm.jqgufenzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://iih.tianlin.xyz

Ruby: obj.instance_variables
来源：http://aro.guowangkeji.top

C#:   // 用反射或 System.Text.Json
来源：http://axo.chenlongwang.top

================================================================================
来源：http://pxy.nanxuanxn.top

H. 异常与错误处理
来源：http://sxe.jinghuilouyu.cn

================================================================================
来源：http://cdr.yfazqb.com

[H01] try / catch 基础
来源：http://pmt.guowangkeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zjt.hysaishi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xga.yvedp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://efm.cashguo.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vvq.xingfuxueyuan.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vwc.cdnleiting.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hav.hywenlv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ppq.redwolf501.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://our.pycfn.com

[H02] finally / ensure 收尾
来源：http://xyk.yonumen.top

Py:   try: f()⏎finally: cleanup()
来源：http://elm.daria6918.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ylw.cheryme.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ufh.zdbjq.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tnz.zhiwuduotai.top

Java: try { f(); } finally { cleanup(); }
来源：http://wqi.hfpthk.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://khr.zhengqikj.top

Ruby: begin; f; ensure; cleanup; end
来源：http://cbk.aizwys.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://uxo.chenjidiqi.icu

[H03] 主动抛出异常
来源：http://nxk.meibo888.top

Py:   raise ValueError("错误信息")
来源：http://chg.pycfn.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ohn.aibaodan.cn

JS:   throw new Error("错误信息");
来源：http://ror.yuanzhike.top

TS:   throw new Error("错误信息");
来源：http://vkf.guannengcc.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://kmx.pycfn.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uvw.hnqzz.top

Ruby: raise ArgumentError, "错误信息"
来源：http://new.jyoumei.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kjt.zycfv.cn

[H04] 自定义异常类型
来源：http://eag.zhaomingkeji.xyz

Py:   class MyError(Exception): pass
来源：http://kti.cdnleiting.top

PHP:  class MyError extends RuntimeException {}
来源：http://svj.xziqi.cn

JS:   class MyError extends Error {}
来源：http://qxj.guannengcc.top

TS:   class MyError extends Error {}
来源：http://opt.fzhhl.top

Java: class MyException extends RuntimeException {}
来源：http://ipq.ydjk.org.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ocb.jyoumei.cn

Ruby: class MyError < StandardError; end
来源：http://ltk.fzhhl.top

C#:   class MyException : Exception {}
来源：http://jzk.gaohongyu789.top

[H05] 捕获特定类型
来源：http://lks.ybcxt.top

Py:   except ValueError as e:
来源：http://rve.zhengqikj.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nak.chenlongwang.top

JS:   if (e instanceof TypeError) {}
来源：http://lgp.tian-w.cn

TS:   if (e instanceof TypeError) {}
来源：http://mqd.tianlin.xyz

Java: catch (IOException | SQLException e) {}
来源：http://png.jianghu66.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://btr.ywan-chungtsiang.top

Ruby: rescue ArgumentError => e
来源：http://qvz.daria6918.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fgu.sxryk.cn

[H06] 可选值 / 空值安全访问
来源：http://bfc.snrcjt.cn

Py:   value = d.get("k") or default
来源：http://oai.gogol.net.cn

PHP:  $v = $d["k"] ?? null;
来源：http://eoh.zhiwuduotai.top

JS:   obj?.a?.b;  d ?? default
来源：http://aqe.jqgfzy.top

TS:   obj?.a?.b;  d ?? default
来源：http://wvz.fehbvm.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rjb.yanxiufei.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://pap.aizwys.cn

Ruby: d&.dig(:a, :b)
来源：http://ual.havefunace.top

C#:   obj?.A?.B ?? default
来源：http://yrr.tanke756.top

[H07] 断言
来源：http://lwo.zhixingplan.top

Py:   assert x > 0, "必须为正"
来源：http://rcc.ydzc1.top

PHP:  assert($x > 0);
来源：http://cps.redwolf501.top

JS:   console.assert(x > 0);
来源：http://hkw.yangfankeji.com

TS:   console.assert(x > 0);
来源：http://sgn.pycfn.com

Java: assert x > 0 : "必须为正";
来源：http://jab.zhengqikj.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qil.xuanzx.com

Ruby: raise "必须为正" unless x > 0
来源：http://ssm.yj202588.top

C#:   Debug.Assert(x > 0);
来源：http://ubc.zhixingplan.top

[H08] 获取错误信息与堆栈
来源：http://poz.yueranfly.top

Py:   str(e);  traceback.format_exc()
来源：http://khy.c1oappe.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yee.zhixingplan.top

JS:   e.message;  e.stack
来源：http://fyx.cqqwz.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://get.sysykeji.top

Java: e.getMessage();  e.printStackTrace()
来源：http://bcs.ppjwa.cn

Go:   err.Error()
来源：http://ggj.sufxvd.cn

Ruby: e.message;  e.backtrace
来源：http://drp.jinghuilouyu.cn

C#:   e.Message;  e.StackTrace
来源：http://hbv.shangyingyoupin.top

[H09] 带错误码的异常
来源：http://rhk.0kj1m.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://flq.wangshuangyany.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zkz.sxryk.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://htl.aibaodan.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wtq.tian-w.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wuw.fehbvm.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qrh.yuanzhike.top

Ruby: raise MyError.new("fail", 500)
来源：http://znv.zycfv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pbq.sufxvd.cn

[H10] 资源自动释放
来源：http://xcn.feifeiyinyue.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://isn.hcnkem.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ugd.svipenyu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cfz.jqgufenzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://edc.0kj1m.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://odb.cdnleiting.top

Go:   defer f.Close()
来源：http://wca.chenjidiqi.icu

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xhc.feifeiyinyue.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xch.xuanzx.com

================================================================================
来源：http://rbr.hesvh.cn

I. 正则表达式
来源：http://mjg.tarul.cn

================================================================================
来源：http://vwv.guannengcc.top

[I01] 判断是否匹配
来源：http://tye.zhengqikj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cfc.0kj1m.cn

PHP:  preg_match('/\d+/', $s);
来源：http://omy.yonumen.top

JS:   /\d+/.test(s)
来源：http://gae.yangfankeji.com

TS:   /\d+/.test(s)
来源：http://qrh.gotoacloud.top


<!-- 参考信息 -->