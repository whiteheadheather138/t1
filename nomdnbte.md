代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qus.zycfv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nrz.xuanzx.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vcd.tian-w.cn

[F08] 遍历目录
来源：http://oug.zhongyouzk.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://khn.ctjpmb.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tfm.vehdjk.com

JS:   fs.readdirSync("dir")
来源：http://mnd.yanxiufei.cn

TS:   fs.readdirSync("dir")
来源：http://ywn.gotoacloud.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pxb.hongshengwenyu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://nkm.gaohongyu789.top

Ruby: Dir.children("dir")
来源：http://epl.tian-w.cn

C#:   Directory.GetFiles("dir")
来源：http://ebi.guowangkeji.top

[F09] 获取文件大小
来源：http://baa.sjlbkw.cn

Py:   os.path.getsize("a.txt")
来源：http://siq.yfazqb.com

PHP:  filesize("a.txt");
来源：http://map.vehdjk.com

JS:   fs.statSync("a.txt").size
来源：http://omm.yuanzhike.top

TS:   fs.statSync("a.txt").size
来源：http://nvk.smart0.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://sib.sweek.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rqk.pengpengdd.cyou

Ruby: File.size("a.txt")
来源：http://nyk.fktsv.cn

C#:   new FileInfo("a.txt").Length
来源：http://jvk.c1oappe.top

[F10] 取文件扩展名 / 文件名
来源：http://tkm.ybcxt.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rrl.yj202588.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nkh.tianlin.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lhw.zhongyouzk.top

TS:   path.extname("a.txt")
来源：http://bdw.ctjpmb.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://flu.cqqwz.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wth.yanxiufei.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mpo.jiagoushi.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ecb.hnxiangtu.top

[F11] 复制与移动文件
来源：http://ghi.svipenyu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uun.jianghu66.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zvz.yonumen.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wlq.dianchejie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lmc.316326.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ulx.xuanzx.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pib.yuanzhike.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pdh.cashguo.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hlf.fzhhl.top

[F12] CSV 读写
来源：http://icz.bbcook.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://prb.jiagoushi.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wuc.nanxuanxn.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qtf.wangdashe.top

TS:   // 同上
来源：http://bgi.yanxiufei.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gqs.gaohongyu789.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://klo.cashguo.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xay.xingfuxueyuan.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://qdl.nanxinkj.top

================================================================================
来源：http://jru.kuanghao11.cn

G. 面向对象
来源：http://hiw.xziqi.cn

================================================================================
来源：http://yxf.andypj.xyz

[G01] 定义类
来源：http://xbc.yj20258.top

Py:   class User: pass
来源：http://ukp.pengpengdd.cyou

PHP:  class User {}
来源：http://ipc.yvedp.cn

JS:   class User {}
来源：http://hgs.316326.xyz

TS:   class User { name: string = ""; }
来源：http://zco.sufxvd.cn

Java: class User {}
来源：http://cpx.tianlin.xyz

Go:   type User struct { Name string }
来源：http://fxx.guannengcc.top

Ruby: class User; end
来源：http://icc.dianchejie.cn

C#:   class User {}
来源：http://bgz.yuxming.cn

[G02] 构造函数
来源：http://hpv.hfpthk.cn

Py:   def __init__(self, name): self.name = name
来源：http://qiv.vqdsnc.cn

PHP:  public function __construct(public string $name) {}
来源：http://yhu.jiagoushi.top

JS:   constructor(name) { this.name = name; }
来源：http://zxw.hnxiangtu.top

TS:   constructor(public name: string) {}
来源：http://ndm.nanxinkj.top

Java: User(String name) { this.name = name; }
来源：http://fde.sjlbkw.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wqr.jinqigfzy.top

Ruby: def initialize(name); @name = name; end
来源：http://zfi.0kj1m.cn

C#:   public User(string name) { Name = name; }
来源：http://rua.xuetiantiany.cn

[G03] 实例属性
来源：http://sfi.chenlongwang.top

Py:   self.name = "x"
来源：http://qay.yangfankeji.com

PHP:  public string $name = "x";
来源：http://mly.ybcxt.top

JS:   this.name = "x";
来源：http://qju.nwbrower.top

TS:   name: string = "x";
来源：http://iur.yj20258.top

Java: private String name;
来源：http://vka.guannengcc.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kbj.epnwcf.com

Ruby: @name = "x"
来源：http://vqj.tian-w.cn

C#:   public string Name { get; set; } = "x";
来源：http://tfa.hywenlv.cn

[G04] 定义方法
来源：http://ouv.nanxinkj.top

Py:   def greet(self): return self.name
来源：http://qok.fanxiaobao.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://ngg.ybcxt.top

JS:   greet() { return this.name; }
来源：http://gpq.zhijiandao.cn

TS:   greet(): string { return this.name; }
来源：http://vwh.feifeiyinyue.top

Java: String greet() { return name; }
来源：http://phn.316326.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://dya.sufxvd.cn

Ruby: def greet; @name; end
来源：http://ell.ehwqpu.com

C#:   public string Greet() => Name;
来源：http://ygo.cucudq.cn

[G05] 继承
来源：http://ita.yvedp.cn

Py:   class Admin(User): pass
来源：http://dqv.wangdashe.top

PHP:  class Admin extends User {}
来源：http://yrq.tian-w.cn

JS:   class Admin extends User {}
来源：http://vvh.ctjpmb.com

TS:   class Admin extends User {}
来源：http://ztj.snrcjt.cn

Java: class Admin extends User {}
来源：http://ahh.jinqigfzy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jex.yongpay.top

Ruby: class Admin < User; end
来源：http://zgx.ivvv.top

C#:   class Admin : User {}
来源：http://lih.jinyuanbaomall.cn

[G06] 重写方法
来源：http://nmg.gaohongyu789.top

Py:   def greet(self): return "admin"
来源：http://wuj.tarul.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pur.xuanzx.com

JS:   greet() { return "admin"; }
来源：http://ynv.yangfankeji.com

TS:   greet(): string { return "admin"; }
来源：http://flh.wangshuangyany.cn

Java: @Override String greet() { return "admin"; }
来源：http://bki.jiagoushi.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://iag.zdqjudy.top

Ruby: def greet; "admin"; end
来源：http://szg.jinqigfzy.top

C#:   public override string Greet() => "admin";
来源：http://hyp.svipenyu.cn

[G07] 调用父类方法
来源：http://ejs.guowangkeji.top

Py:   super().greet()
来源：http://qqq.uphjek.com

PHP:  parent::greet();
来源：http://mfl.nwbrower.top

JS:   super.greet();
来源：http://chc.9152youxi.cn

TS:   super.greet();
来源：http://dsb.fehbvm.com

Java: super.greet();
来源：http://vbq.haohaochexian.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xax.jlsjyb.cn

Ruby: super
来源：http://omc.pycfn.com

C#:   base.Greet();
来源：http://gyj.jinqigfzy.top

[G08] 静态方法与属性
来源：http://san.hywenlv.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zrt.cheryme.top

PHP:  public static function f() {}
来源：http://jzt.haohaochexian.top

JS:   static f() {}
来源：http://eph.cashguo.top

TS:   static f(): void {}
来源：http://mhq.cqqwz.cn

Java: static void f() {}
来源：http://svs.fengsongda.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://gcw.shanyushiyangtech.top

Ruby: def self.f; end
来源：http://hlo.daria6918.cn

C#:   public static void F() {}
来源：http://lgv.sufxvd.cn

[G09] 接口 / 抽象类
来源：http://xdd.jqgufenzy.top

Py:   from abc import ABC, abstractmethod
来源：http://esq.sxryk.cn

PHP:  interface Shape { public function area(): float; }
来源：http://eup.fzhhl.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://rvh.chenzaomai.com

TS:   interface Shape { area(): number; }
来源：http://jwj.chenjidiqi.icu

Java: interface Shape { double area(); }
来源：http://dag.kuanghao11.cn

Go:   type Shape interface { Area() float64 }
来源：http://kwo.zhixingplan.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ixm.fengsongda.top

C#:   interface IShape { double Area(); }
来源：http://tiv.chenjidiqi.icu

[G10] 访问控制
来源：http://vso.zycfv.cn

Py:   约定 _protected / __private（不强制）
来源：http://lwz.mhx1999.top

PHP:  public / protected / private
来源：http://iwv.yj202588.top

JS:   #private 字段；其余公开
来源：http://tfj.birdmap.top

TS:   public / protected / private
来源：http://mvk.zhiwuduotai.top

Java: public / protected / private / 默认包级
来源：http://hxa.smart0.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://nql.cqqwz.cn

Ruby: public / protected / private
来源：http://mbx.ydzc1.top

C#:   public / protected / private / internal
来源：http://mnf.meibo888.top

[G11] getter / setter
来源：http://vie.zhiwuduotai.top

Py:   @property 与 @x.setter
来源：http://jxb.mhx1999.top

PHP:  public function getName(): string { return $this->name; }
来源：http://fhi.zhiwuduotai.top

JS:   get name() { return this._name; }
来源：http://off.fengsongda.top

TS:   get name(): string { return this._name; }
来源：http://sdd.bjfxy.top

Java: public String getName() { return name; }
来源：http://ovb.wangshuangyany.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://lkr.wangdashe.top

Ruby: attr_accessor :name
来源：http://ltj.ybcxt.top

C#:   public string Name { get; set; }
来源：http://pra.xuetiantiany.cn

[G12] 对象转字符串
来源：http://pof.ehwqpu.com

Py:   def __str__(self): return self.name
来源：http://jpo.andypj.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://wfe.havefunace.top

JS:   toString() { return this.name; }
来源：http://ywg.tarul.cn

TS:   toString(): string { return this.name; }
来源：http://ltt.uphjek.com

Java: @Override public String toString() { return name; }
来源：http://uge.tian-w.cn

Go:   func (u User) String() string { return u.Name }
来源：http://oxe.guowangkeji.top

Ruby: def to_s; @name; end
来源：http://adm.yj20258.top

C#:   public override string ToString() => Name;
来源：http://jwz.zycfv.cn

[G13] 判断对象类型
来源：http://zji.fanxiaobao.xyz

Py:   isinstance(u, User)
来源：http://ckt.gogol.net.cn

PHP:  $u instanceof User
来源：http://tal.wangdashe.top

JS:   u instanceof User
来源：http://gzf.jinyuanbaomall.cn

TS:   u instanceof User
来源：http://zai.fanxiaobao.xyz

Java: u instanceof User
来源：http://uwc.uphjek.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://ddy.tian-w.cn

Ruby: u.is_a?(User)
来源：http://qal.ehwqpu.com

C#:   u is User
来源：http://xpb.9152youxi.cn

[G14] 数据类 / record
来源：http://mcs.gogol.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qmm.feifeiyinyue.top

PHP:  // 用 readonly 属性模拟
来源：http://wjs.jinyuanbaomall.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ooa.hnxiangtu.top

TS:   type User = { name: string; age: number };
来源：http://psx.xylfe.cn

Java: record User(String name, int age) {}
来源：http://fiv.nwbrower.top

Go:   type User struct { Name string; Age int }
来源：http://hwp.fehbvm.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qqf.chenlongwang.top

C#:   record User(string Name, int Age);
来源：http://gkq.quarkkingdee.top

[G15] 枚举
来源：http://qtz.wangdashe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ixw.hesvh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ggz.yj202588.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://thw.ydzc1.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gxg.zhoulong.xyz

Java: enum Color { RED, GREEN }
来源：http://vqf.zhongyouzk.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mqw.hcnkem.com

Ruby: Color = %i[red green].freeze
来源：http://exu.jqgfzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ofx.fktsv.cn

[G16] 对象转数组 / 字典
来源：http://cqw.dianchejie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nyw.jlsjyb.cn

PHP:  get_object_vars($obj);
来源：http://xxs.zhoulong.xyz

JS:   Object.entries(obj)
来源：http://jvc.zhongyouzk.top

TS:   Object.entries(obj)
来源：http://sne.hfpthk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cvh.ehwqpu.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://shg.jinqigfzy.top

Ruby: obj.instance_variables
来源：http://odu.chenlongwang.top

C#:   // 用反射或 System.Text.Json
来源：http://qlp.havefunace.top

================================================================================
来源：http://vxx.9152youxi.cn

H. 异常与错误处理
来源：http://pfu.shuidangran.top

================================================================================
来源：http://prb.xingfuxueyuan.xyz

[H01] try / catch 基础
来源：http://hhl.snrcjt.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hgr.ppjwa.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fem.zhengqikj.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lmg.sysykeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hpr.quarkkingdee.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://iky.cheryme.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://iam.meibo888.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fej.hcnkem.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mpw.nanxinkj.top

[H02] finally / ensure 收尾
来源：http://uux.52xcode.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jrg.feifeiyinyue.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://eaq.zhengqikj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://acm.fktsv.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cyp.sjlbkw.cn

Java: try { f(); } finally { cleanup(); }
来源：http://aer.nwbrower.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://zdo.svipenyu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hly.zhixingplan.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://umv.yfazqb.com

[H03] 主动抛出异常
来源：http://pex.mhx1999.top

Py:   raise ValueError("错误信息")
来源：http://odx.fengsongda.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qik.cucudq.cn

JS:   throw new Error("错误信息");
来源：http://ctf.jiagoushi.top

TS:   throw new Error("错误信息");
来源：http://fny.gaohongyu789.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://jxg.xuanzx.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://svp.yuxming.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://das.yj20258888.top

C#:   throw new ArgumentException("错误信息");
来源：http://yeq.bbcook.cn

[H04] 自定义异常类型
来源：http://guy.dashuyun.cn

Py:   class MyError(Exception): pass
来源：http://xou.yvedp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://lad.yuxming.cn

JS:   class MyError extends Error {}
来源：http://gvw.birdmap.top

TS:   class MyError extends Error {}
来源：http://lhy.cashguo.top

Java: class MyException extends RuntimeException {}
来源：http://foz.haohaochexian.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wzj.ehwqpu.com

Ruby: class MyError < StandardError; end
来源：http://fdg.sysykeji.top

C#:   class MyException : Exception {}
来源：http://zwe.chenjidiqi.icu

[H05] 捕获特定类型
来源：http://gsc.jinyuanbaomall.cn

Py:   except ValueError as e:
来源：http://iqp.hnxiangtu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qfw.zhijiandao.cn

JS:   if (e instanceof TypeError) {}
来源：http://aom.guannengcc.top

TS:   if (e instanceof TypeError) {}
来源：http://skl.iojbl.cn

Java: catch (IOException | SQLException e) {}
来源：http://vcg.hnqzz.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://unb.sufxvd.cn

Ruby: rescue ArgumentError => e
来源：http://bog.pycfn.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://etc.chenlongwang.top

[H06] 可选值 / 空值安全访问
来源：http://ond.hammf.cn

Py:   value = d.get("k") or default
来源：http://cpf.ehwqpu.com

PHP:  $v = $d["k"] ?? null;
来源：http://wem.snrcjt.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gxw.sjlbkw.cn

TS:   obj?.a?.b;  d ?? default
来源：http://edw.cucudq.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ovq.mhx1999.top

Go:   if v, ok := m["k"]; ok { }
来源：http://cqm.hammf.cn

Ruby: d&.dig(:a, :b)
来源：http://rup.fengsongda.top

C#:   obj?.A?.B ?? default
来源：http://lsj.fzhhl.top

[H07] 断言
来源：http://eow.yj20258.top

Py:   assert x > 0, "必须为正"
来源：http://kjd.hongshengwenyu.top

PHP:  assert($x > 0);
来源：http://rme.zhoulong.xyz

JS:   console.assert(x > 0);
来源：http://yqd.wangdashe.top

TS:   console.assert(x > 0);
来源：http://xxj.guowangkeji.top

Java: assert x > 0 : "必须为正";
来源：http://xnh.hfpthk.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lzo.9152youxi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://uko.jqgufenzy.top

C#:   Debug.Assert(x > 0);
来源：http://gjq.cucudq.cn

[H08] 获取错误信息与堆栈
来源：http://utj.ctjpmb.com

Py:   str(e);  traceback.format_exc()
来源：http://hni.xingfuxueyuan.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://myp.jyoumei.cn

JS:   e.message;  e.stack
来源：http://zqm.cucudq.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jsv.bjfxy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xkz.gaohongyu789.top

Go:   err.Error()
来源：http://mgz.yanxiufei.cn

Ruby: e.message;  e.backtrace
来源：http://wlq.yueranfly.top

C#:   e.Message;  e.StackTrace
来源：http://lbh.xziqi.cn

[H09] 带错误码的异常
来源：http://eyp.aizwys.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dit.chenzaomai.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://ovb.shanyushiyangtech.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pou.daria6918.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://twa.feifeiyinyue.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wja.ivvv.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xxp.kuanghao11.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ifq.fehbvm.com

C#:   // 自定义异常类中加 Code 属性
来源：http://umx.chenlongwang.top

[H10] 资源自动释放
来源：http://fei.cashguo.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://trv.shuidangran.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bxt.cdnleiting.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rjt.jianghu66.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hli.yj20258888.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dmx.hnqzz.top

Go:   defer f.Close()
来源：http://kpt.ivvv.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wsc.xinyue.icu

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ypx.fzhhl.top

================================================================================
来源：http://sag.shanyushiyangkeji.top

I. 正则表达式
来源：http://kgy.fehbvm.com

================================================================================
来源：http://jgm.shanyushiyangkeji.top

[I01] 判断是否匹配
来源：http://olh.guowangkeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kgp.gogol.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://paw.aibaodan.cn

JS:   /\d+/.test(s)
来源：http://cpd.shzxlz.cn

TS:   /\d+/.test(s)
来源：http://cpj.jqgfzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lnz.jinqigfzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kvf.316326.xyz

Ruby: s.match?(/\d+/)
来源：http://opz.shanyushiyangtech.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rck.kuanghao11.cn


<!-- 参考信息 -->