代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://irw.zhongyouzk.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fmx.zycfv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rtd.wangdashe.top

[F08] 遍历目录
来源：http://eao.ivvv.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://atq.fzhhl.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bqp.sjlbkw.cn

JS:   fs.readdirSync("dir")
来源：http://nem.ctjpmb.com

TS:   fs.readdirSync("dir")
来源：http://ojm.gogol.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zfd.yongpay.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zhv.vqdsnc.cn

Ruby: Dir.children("dir")
来源：http://czb.zdqjudy.top

C#:   Directory.GetFiles("dir")
来源：http://vbs.cucudq.cn

[F09] 获取文件大小
来源：http://clf.yj202588.top

Py:   os.path.getsize("a.txt")
来源：http://yic.xinyue.icu

PHP:  filesize("a.txt");
来源：http://sui.zycfv.cn

JS:   fs.statSync("a.txt").size
来源：http://apm.fehbvm.com

TS:   fs.statSync("a.txt").size
来源：http://bcu.yvedp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gqd.shuidangran.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://far.gotoacloud.top

Ruby: File.size("a.txt")
来源：http://aeo.xingfuxueyuan.xyz

C#:   new FileInfo("a.txt").Length
来源：http://guq.xuetiantiany.cn

[F10] 取文件扩展名 / 文件名
来源：http://fsj.jlsjyb.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tsv.sxryk.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gcn.dashuyun.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bif.jinqigfzy.top

TS:   path.extname("a.txt")
来源：http://sec.shangyingyoupin.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fpv.zdqjudy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vgk.zhaomingkeji.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uch.jqgufenzy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cui.jqgfzy.top

[F11] 复制与移动文件
来源：http://gch.vqdsnc.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yoz.yueranfly.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://obz.xylfe.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rxt.yfazqb.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xjf.tianlin.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vhy.nanxuanxn.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ncz.zhijiandao.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ury.xylfe.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nvv.yonumen.top

[F12] CSV 读写
来源：http://jvb.hcnkem.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://izs.wangdashe.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tcv.xylfe.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wce.jinghuilouyu.cn

TS:   // 同上
来源：http://ekr.gzhubu.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gep.vqdsnc.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hmk.uphjek.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dtq.vehdjk.com

C#:   // 无内置：用 CsvHelper 库
来源：http://fhh.vehdjk.com

================================================================================
来源：http://tuv.ydzc1.top

G. 面向对象
来源：http://gfw.ydzc1.top

================================================================================
来源：http://baw.nanxinkj.top

[G01] 定义类
来源：http://mre.yj202588.top

Py:   class User: pass
来源：http://xxc.xylfe.cn

PHP:  class User {}
来源：http://ihi.jinyuanbaomall.cn

JS:   class User {}
来源：http://twl.quarkkingdee.top

TS:   class User { name: string = ""; }
来源：http://nhf.guowangkeji.top

Java: class User {}
来源：http://cko.jinyuanbaomall.cn

Go:   type User struct { Name string }
来源：http://wvr.quarkkingdee.top

Ruby: class User; end
来源：http://tte.fzhhl.top

C#:   class User {}
来源：http://inz.jinghuilouyu.cn

[G02] 构造函数
来源：http://uqn.gogol.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://eui.ybcxt.top

PHP:  public function __construct(public string $name) {}
来源：http://uzw.jqgfzy.top

JS:   constructor(name) { this.name = name; }
来源：http://tpa.daria6918.cn

TS:   constructor(public name: string) {}
来源：http://sud.jyoumei.cn

Java: User(String name) { this.name = name; }
来源：http://euh.fehbvm.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oqh.tian-w.cn

Ruby: def initialize(name); @name = name; end
来源：http://ukr.havefunace.top

C#:   public User(string name) { Name = name; }
来源：http://bqo.zhaomingkeji.xyz

[G03] 实例属性
来源：http://fll.cucudq.cn

Py:   self.name = "x"
来源：http://lrt.xuanzx.com

PHP:  public string $name = "x";
来源：http://aan.birdmap.top

JS:   this.name = "x";
来源：http://gnk.dianchejie.cn

TS:   name: string = "x";
来源：http://oxo.bbcook.cn

Java: private String name;
来源：http://ixl.zhongyouzk.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://eyq.sxryk.cn

Ruby: @name = "x"
来源：http://tue.cashguo.top

C#:   public string Name { get; set; } = "x";
来源：http://rhz.bjfxy.top

[G04] 定义方法
来源：http://mlp.fengsongda.top

Py:   def greet(self): return self.name
来源：http://ibj.zycfv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ivi.316326.xyz

JS:   greet() { return this.name; }
来源：http://wtt.shzxlz.cn

TS:   greet(): string { return this.name; }
来源：http://fdv.xziqi.cn

Java: String greet() { return name; }
来源：http://ffg.nanxinkj.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://bra.0kj1m.cn

Ruby: def greet; @name; end
来源：http://yph.mhx1999.top

C#:   public string Greet() => Name;
来源：http://gln.jinyuanbaomall.cn

[G05] 继承
来源：http://cau.guowangkeji.top

Py:   class Admin(User): pass
来源：http://kyx.bjfxy.top

PHP:  class Admin extends User {}
来源：http://nzk.jinghuilouyu.cn

JS:   class Admin extends User {}
来源：http://vek.jianghu66.top

TS:   class Admin extends User {}
来源：http://dcx.xinyue.icu

Java: class Admin extends User {}
来源：http://xsu.pycfn.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mif.sxryk.cn

Ruby: class Admin < User; end
来源：http://ijj.hcnkem.com

C#:   class Admin : User {}
来源：http://hsp.jianghu66.top

[G06] 重写方法
来源：http://tkb.smart0.xyz

Py:   def greet(self): return "admin"
来源：http://rmi.yj202588.top

PHP:  public function greet(): string { return "admin"; }
来源：http://bfy.cdnleiting.top

JS:   greet() { return "admin"; }
来源：http://ffu.sweek.top

TS:   greet(): string { return "admin"; }
来源：http://kjo.jinqigfzy.top

Java: @Override String greet() { return "admin"; }
来源：http://rjj.ywan-chungtsiang.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://glb.ydzc1.top

Ruby: def greet; "admin"; end
来源：http://vvf.cheryme.top

C#:   public override string Greet() => "admin";
来源：http://bqs.fanxiaobao.xyz

[G07] 调用父类方法
来源：http://akb.tianlin.xyz

Py:   super().greet()
来源：http://vuw.uphjek.com

PHP:  parent::greet();
来源：http://lpc.sjlbkw.cn

JS:   super.greet();
来源：http://vig.smart0.xyz

TS:   super.greet();
来源：http://bqu.hfpthk.cn

Java: super.greet();
来源：http://mwk.fanxiaobao.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jqj.yvedp.cn

Ruby: super
来源：http://htv.jianghu66.top

C#:   base.Greet();
来源：http://fnk.jqgufenzy.top

[G08] 静态方法与属性
来源：http://kco.haohaochexian.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nln.gogol.net.cn

PHP:  public static function f() {}
来源：http://pco.jqgfzy.top

JS:   static f() {}
来源：http://goa.guowangkeji.top

TS:   static f(): void {}
来源：http://sfh.jyoumei.cn

Java: static void f() {}
来源：http://cjm.xuanzx.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://ofz.cheryme.top

Ruby: def self.f; end
来源：http://edw.c1oappe.top

C#:   public static void F() {}
来源：http://oau.yanxiufei.cn

[G09] 接口 / 抽象类
来源：http://dbu.feifeiyinyue.top

Py:   from abc import ABC, abstractmethod
来源：http://nno.yj20258.top

PHP:  interface Shape { public function area(): float; }
来源：http://dvv.jiagoushi.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://gkd.meibo888.top

TS:   interface Shape { area(): number; }
来源：http://evf.yj202588.top

Java: interface Shape { double area(); }
来源：http://hwf.jinyuanbaomall.cn

Go:   type Shape interface { Area() float64 }
来源：http://xce.ydzc1.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ule.quarkkingdee.top

C#:   interface IShape { double Area(); }
来源：http://hnn.uphjek.com

[G10] 访问控制
来源：http://yrv.sufxvd.cn

Py:   约定 _protected / __private（不强制）
来源：http://eqi.0kj1m.cn

PHP:  public / protected / private
来源：http://prp.nanxuanxn.top

JS:   #private 字段；其余公开
来源：http://img.zycfv.cn

TS:   public / protected / private
来源：http://qmr.jqgufenzy.top

Java: public / protected / private / 默认包级
来源：http://qny.guannengcc.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://jgf.ydzc1.top

Ruby: public / protected / private
来源：http://hyt.yj202588.top

C#:   public / protected / private / internal
来源：http://lue.meibo888.top

[G11] getter / setter
来源：http://czn.fanxiaobao.xyz

Py:   @property 与 @x.setter
来源：http://wew.gotoacloud.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jzb.andypj.xyz

JS:   get name() { return this._name; }
来源：http://nlg.hesvh.cn

TS:   get name(): string { return this._name; }
来源：http://avt.ydjk.org.cn

Java: public String getName() { return name; }
来源：http://mgx.cheryme.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://uzt.yuxming.cn

Ruby: attr_accessor :name
来源：http://pcm.yonumen.top

C#:   public string Name { get; set; }
来源：http://ghd.cqqwz.cn

[G12] 对象转字符串
来源：http://nux.chenlongwang.top

Py:   def __str__(self): return self.name
来源：http://hyt.hywenlv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://klr.hammf.cn

JS:   toString() { return this.name; }
来源：http://uvg.zhengqikj.top

TS:   toString(): string { return this.name; }
来源：http://fgx.nanxuanxn.top

Java: @Override public String toString() { return name; }
来源：http://cit.sxryk.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ptf.shanyushiyangkeji.top

Ruby: def to_s; @name; end
来源：http://ycc.yongpay.top

C#:   public override string ToString() => Name;
来源：http://vnz.daxiang520.top

[G13] 判断对象类型
来源：http://rft.vqdsnc.cn

Py:   isinstance(u, User)
来源：http://gzd.bjfxy.top

PHP:  $u instanceof User
来源：http://hvv.yj202588.top

JS:   u instanceof User
来源：http://pdh.shzxlz.cn

TS:   u instanceof User
来源：http://xvs.yangfankeji.com

Java: u instanceof User
来源：http://yhv.sjlbkw.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qns.nanxinkj.top

Ruby: u.is_a?(User)
来源：http://izc.guannengcc.top

C#:   u is User
来源：http://kgi.xingfuxueyuan.xyz

[G14] 数据类 / record
来源：http://ktg.fanxiaobao.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jug.hcnkem.com

PHP:  // 用 readonly 属性模拟
来源：http://vkw.quarkkingdee.top

JS:   // 无内置：普通类或对象字面量
来源：http://csd.haohaochexian.top

TS:   type User = { name: string; age: number };
来源：http://ewq.shzxlz.cn

Java: record User(String name, int age) {}
来源：http://fkd.sufxvd.cn

Go:   type User struct { Name string; Age int }
来源：http://kcj.hongshengwenyu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ytf.nwbrower.top

C#:   record User(string Name, int Age);
来源：http://oni.0kj1m.cn

[G15] 枚举
来源：http://hiy.yueranfly.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pgu.chenzaomai.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://jba.yuanzhike.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kqt.fktsv.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cee.wangdashe.top

Java: enum Color { RED, GREEN }
来源：http://uod.hesvh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kgr.gogol.net.cn

Ruby: Color = %i[red green].freeze
来源：http://qgk.sweek.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nvf.yj20258888.top

[G16] 对象转数组 / 字典
来源：http://zvv.hnqzz.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nfc.fktsv.cn

PHP:  get_object_vars($obj);
来源：http://qoo.0kj1m.cn

JS:   Object.entries(obj)
来源：http://xsy.ydzc1.top

TS:   Object.entries(obj)
来源：http://rhx.yuxming.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zuk.zhiwuduotai.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ijr.hongshengwenyu.top

Ruby: obj.instance_variables
来源：http://gqi.yanxiufei.cn

C#:   // 用反射或 System.Text.Json
来源：http://jtd.zhoulong.xyz

================================================================================
来源：http://idt.snrcjt.cn

H. 异常与错误处理
来源：http://nog.xuanzx.com

================================================================================
来源：http://sol.sxryk.cn

[H01] try / catch 基础
来源：http://ugc.zhoulong.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tej.jqgufenzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ygl.jinqigfzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ymp.zhijiandao.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cdy.jinghuilouyu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xgb.jinqigufen.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://thm.bjfxy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jud.nanxinkj.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ssn.smart0.xyz

[H02] finally / ensure 收尾
来源：http://ztl.zhoulong.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://vvq.daxiang520.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://xgy.chenlongwang.top

JS:   try { f(); } finally { cleanup(); }
来源：http://udw.xinyue.icu

TS:   try { f(); } finally { cleanup(); }
来源：http://tmw.316326.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://qwr.ywan-chungtsiang.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://cvq.hcnkem.com

Ruby: begin; f; ensure; cleanup; end
来源：http://efs.guowangkeji.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://bph.snrcjt.cn

[H03] 主动抛出异常
来源：http://lio.feifeiyinyue.top

Py:   raise ValueError("错误信息")
来源：http://khf.fehbvm.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ymj.tian-w.cn

JS:   throw new Error("错误信息");
来源：http://tye.wangshuangyany.cn

TS:   throw new Error("错误信息");
来源：http://nwj.hywenlv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zuf.daxiang520.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tiq.tian-w.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xay.havefunace.top

C#:   throw new ArgumentException("错误信息");
来源：http://fxq.bjfxy.top

[H04] 自定义异常类型
来源：http://arw.cqqwz.cn

Py:   class MyError(Exception): pass
来源：http://frf.pycfn.com

PHP:  class MyError extends RuntimeException {}
来源：http://imp.yueranfly.top

JS:   class MyError extends Error {}
来源：http://twy.jyoumei.cn

TS:   class MyError extends Error {}
来源：http://wqz.jianghu66.top

Java: class MyException extends RuntimeException {}
来源：http://hyg.c1oappe.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cgo.hfpthk.cn

Ruby: class MyError < StandardError; end
来源：http://fpm.sweek.top

C#:   class MyException : Exception {}
来源：http://vnf.yonumen.top

[H05] 捕获特定类型
来源：http://bqr.xuanzx.com

Py:   except ValueError as e:
来源：http://pdm.meibo888.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lys.9152youxi.cn

JS:   if (e instanceof TypeError) {}
来源：http://goi.vqdsnc.cn

TS:   if (e instanceof TypeError) {}
来源：http://eto.gogol.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://bvq.haohaochexian.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://idj.zhengqikj.top

Ruby: rescue ArgumentError => e
来源：http://fbq.yj202588.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pei.fktsv.cn

[H06] 可选值 / 空值安全访问
来源：http://vil.xziqi.cn

Py:   value = d.get("k") or default
来源：http://lmo.daria6918.cn

PHP:  $v = $d["k"] ?? null;
来源：http://poq.kuanghao11.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ket.aizwys.cn

TS:   obj?.a?.b;  d ?? default
来源：http://chw.sweek.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lqc.wangshuangyany.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://whj.chenlongwang.top

Ruby: d&.dig(:a, :b)
来源：http://vuy.xinyue.icu

C#:   obj?.A?.B ?? default
来源：http://tpu.tanke756.top

[H07] 断言
来源：http://iwv.sysykeji.top

Py:   assert x > 0, "必须为正"
来源：http://aum.sysykeji.top

PHP:  assert($x > 0);
来源：http://efs.cheryme.top

JS:   console.assert(x > 0);
来源：http://mcd.dianchejie.cn

TS:   console.assert(x > 0);
来源：http://kqn.uphjek.com

Java: assert x > 0 : "必须为正";
来源：http://lgk.jqgfzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ajn.yj20258888.top

Ruby: raise "必须为正" unless x > 0
来源：http://meo.bjfxy.top

C#:   Debug.Assert(x > 0);
来源：http://zfj.yanxiufei.cn

[H08] 获取错误信息与堆栈
来源：http://cfk.ydzc1.top

Py:   str(e);  traceback.format_exc()
来源：http://mqq.9152youxi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://whc.xingfuxueyuan.xyz

JS:   e.message;  e.stack
来源：http://cgo.guowangkeji.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://agr.ppjwa.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://sak.xylfe.cn

Go:   err.Error()
来源：http://fhb.cashguo.top

Ruby: e.message;  e.backtrace
来源：http://mvd.shanyushiyangkeji.top

C#:   e.Message;  e.StackTrace
来源：http://dhr.ywan-chungtsiang.top

[H09] 带错误码的异常
来源：http://hgo.zhongyouzk.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mvl.mhx1999.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://lex.meibo888.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hxa.zhijiandao.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rur.mhx1999.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dxg.jianghu66.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://phw.jyoumei.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bqc.hongshengwenyu.top

C#:   // 自定义异常类中加 Code 属性
来源：http://vsx.jinqigufen.top

[H10] 资源自动释放
来源：http://oym.guannengcc.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ywi.shanyushiyangkeji.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qzz.hesvh.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jqw.aibaodan.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mis.hfpthk.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rss.zhongyouzk.top

Go:   defer f.Close()
来源：http://tiw.xingfuxueyuan.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xtk.snrcjt.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qov.cashguo.top

================================================================================
来源：http://hzz.jinghuilouyu.cn

I. 正则表达式
来源：http://gro.sweek.top

================================================================================
来源：http://kxm.guannengcc.top

[I01] 判断是否匹配
来源：http://aaz.wangshuangyany.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uph.fehbvm.com

PHP:  preg_match('/\d+/', $s);
来源：http://lnx.ehwqpu.com

JS:   /\d+/.test(s)
来源：http://jup.9152youxi.cn

TS:   /\d+/.test(s)
来源：http://sia.yonumen.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xas.zhiwuduotai.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ewu.iojbl.cn

Ruby: s.match?(/\d+/)
来源：http://qdr.havefunace.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jal.cqqwz.cn


<!-- 参考信息 -->