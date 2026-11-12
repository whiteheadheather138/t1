代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sea.yvedp.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://whi.hongshengwenyu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vpa.sweek.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://usj.ppjwa.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tkh.hywenlv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hyc.birdmap.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://swz.zycfv.cn

[F08] 遍历目录
来源：http://iks.nanxinkj.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://zmu.zhongyouzk.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://olx.smart0.xyz

JS:   fs.readdirSync("dir")
来源：http://qvt.haohaochexian.top

TS:   fs.readdirSync("dir")
来源：http://art.yj20258.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gfk.vqdsnc.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qst.snrcjt.cn

Ruby: Dir.children("dir")
来源：http://pum.cashguo.top

C#:   Directory.GetFiles("dir")
来源：http://luj.svipenyu.cn

[F09] 获取文件大小
来源：http://ihs.redwolf501.top

Py:   os.path.getsize("a.txt")
来源：http://pbl.jlsjyb.cn

PHP:  filesize("a.txt");
来源：http://som.guannengcc.top

JS:   fs.statSync("a.txt").size
来源：http://uha.hnxiangtu.top

TS:   fs.statSync("a.txt").size
来源：http://jyk.yj20258888.top

Java: Files.size(Path.of("a.txt"))
来源：http://goq.aibaodan.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fno.yj20258888.top

Ruby: File.size("a.txt")
来源：http://htk.cheryme.top

C#:   new FileInfo("a.txt").Length
来源：http://yzd.hywenlv.cn

[F10] 取文件扩展名 / 文件名
来源：http://ujz.zhengqikj.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ahc.aibaodan.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vif.pengpengdd.cyou

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eki.shanyushiyangkeji.top

TS:   path.extname("a.txt")
来源：http://duu.xziqi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cis.shangyingyoupin.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jpb.cheryme.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dqj.quarkkingdee.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gxw.cdnleiting.top

[F11] 复制与移动文件
来源：http://gik.yuanzhike.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yjh.xinyue.icu

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kxl.cucudq.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nsj.bbcook.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oso.xuetiantiany.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fnv.ctjpmb.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bcx.jqgufenzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sgm.zycfv.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mxn.aibaodan.cn

[F12] CSV 读写
来源：http://yek.gogol.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yhw.jinqigfzy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jrd.nwbrower.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://itn.andypj.xyz

TS:   // 同上
来源：http://mmq.gotoacloud.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gwh.dashuyun.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xrz.vqdsnc.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ows.guannengcc.top

C#:   // 无内置：用 CsvHelper 库
来源：http://tie.hesvh.cn

================================================================================
来源：http://vce.birdmap.top

G. 面向对象
来源：http://ska.hysaishi.cn

================================================================================
来源：http://hlm.zhiwuduotai.top

[G01] 定义类
来源：http://uxe.xylfe.cn

Py:   class User: pass
来源：http://umy.aizwys.cn

PHP:  class User {}
来源：http://gih.aibaodan.cn

JS:   class User {}
来源：http://ixi.chenlongwang.top

TS:   class User { name: string = ""; }
来源：http://wkl.yvedp.cn

Java: class User {}
来源：http://oaj.yj202588.top

Go:   type User struct { Name string }
来源：http://xnu.zhijiandao.cn

Ruby: class User; end
来源：http://lwf.hnqzz.top

C#:   class User {}
来源：http://bfj.chenjidiqi.icu

[G02] 构造函数
来源：http://eoq.dashuyun.cn

Py:   def __init__(self, name): self.name = name
来源：http://smo.9152youxi.cn

PHP:  public function __construct(public string $name) {}
来源：http://ojt.dianchejie.cn

JS:   constructor(name) { this.name = name; }
来源：http://agi.xziqi.cn

TS:   constructor(public name: string) {}
来源：http://kue.hysaishi.cn

Java: User(String name) { this.name = name; }
来源：http://etv.xuetiantiany.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gfi.yuanzhike.top

Ruby: def initialize(name); @name = name; end
来源：http://asi.tianlin.xyz

C#:   public User(string name) { Name = name; }
来源：http://udj.xylfe.cn

[G03] 实例属性
来源：http://ppk.zhijiandao.cn

Py:   self.name = "x"
来源：http://did.shangyingyoupin.top

PHP:  public string $name = "x";
来源：http://jqy.sxryk.cn

JS:   this.name = "x";
来源：http://dze.dianchejie.cn

TS:   name: string = "x";
来源：http://tvz.birdmap.top

Java: private String name;
来源：http://gga.fzhhl.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uks.zdqjudy.top

Ruby: @name = "x"
来源：http://brk.zhengqikj.top

C#:   public string Name { get; set; } = "x";
来源：http://qvc.tanke756.top

[G04] 定义方法
来源：http://ief.zdbjq.cn

Py:   def greet(self): return self.name
来源：http://cwg.yj20258888.top

PHP:  public function greet(): string { return $this->name; }
来源：http://lms.jinqigfzy.top

JS:   greet() { return this.name; }
来源：http://dbr.c1oappe.top

TS:   greet(): string { return this.name; }
来源：http://avk.nanxuanxn.top

Java: String greet() { return name; }
来源：http://fak.tianlin.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://kmn.shanyushiyangkeji.top

Ruby: def greet; @name; end
来源：http://jjh.shzxlz.cn

C#:   public string Greet() => Name;
来源：http://nns.shanyushiyangtech.top

[G05] 继承
来源：http://nhq.feifeiyinyue.top

Py:   class Admin(User): pass
来源：http://icx.jinghuilouyu.cn

PHP:  class Admin extends User {}
来源：http://mcd.shanyushiyangkeji.top

JS:   class Admin extends User {}
来源：http://szg.xuetiantiany.cn

TS:   class Admin extends User {}
来源：http://tjh.hnxiangtu.top

Java: class Admin extends User {}
来源：http://wbi.shanyushiyangtech.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hin.iojbl.cn

Ruby: class Admin < User; end
来源：http://vdn.fktsv.cn

C#:   class Admin : User {}
来源：http://hus.cdnleiting.top

[G06] 重写方法
来源：http://dnw.quarkkingdee.top

Py:   def greet(self): return "admin"
来源：http://mwf.sufxvd.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hmp.wangdashe.top

JS:   greet() { return "admin"; }
来源：http://oab.hammf.cn

TS:   greet(): string { return "admin"; }
来源：http://qga.jinqigfzy.top

Java: @Override String greet() { return "admin"; }
来源：http://vyc.shanyushiyangkeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://eho.jinqigufen.top

Ruby: def greet; "admin"; end
来源：http://fyx.ctjpmb.com

C#:   public override string Greet() => "admin";
来源：http://gyn.ehwqpu.com

[G07] 调用父类方法
来源：http://iwi.hywenlv.cn

Py:   super().greet()
来源：http://zzy.zdbjq.cn

PHP:  parent::greet();
来源：http://wpw.fktsv.cn

JS:   super.greet();
来源：http://ebe.yonumen.top

TS:   super.greet();
来源：http://peu.0kj1m.cn

Java: super.greet();
来源：http://wuc.yj20258.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zmm.snrcjt.cn

Ruby: super
来源：http://pxd.yonumen.top

C#:   base.Greet();
来源：http://bcg.zhaomingkeji.xyz

[G08] 静态方法与属性
来源：http://hgk.zhengqikj.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qdo.c1oappe.top

PHP:  public static function f() {}
来源：http://tok.iojbl.cn

JS:   static f() {}
来源：http://hwm.jyoumei.cn

TS:   static f(): void {}
来源：http://mrd.xziqi.cn

Java: static void f() {}
来源：http://yia.fehbvm.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://fpg.guowangkeji.top

Ruby: def self.f; end
来源：http://jpf.nwbrower.top

C#:   public static void F() {}
来源：http://ldm.yueranfly.top

[G09] 接口 / 抽象类
来源：http://dxp.aizwys.cn

Py:   from abc import ABC, abstractmethod
来源：http://gey.xuetiantiany.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ylo.daxiang520.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ccx.yangfankeji.com

TS:   interface Shape { area(): number; }
来源：http://cuv.c1oappe.top

Java: interface Shape { double area(); }
来源：http://akw.tarul.cn

Go:   type Shape interface { Area() float64 }
来源：http://kxp.hysaishi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zhs.yuxming.cn

C#:   interface IShape { double Area(); }
来源：http://wut.nanxuanxn.top

[G10] 访问控制
来源：http://dtk.mhx1999.top

Py:   约定 _protected / __private（不强制）
来源：http://rqo.ybcxt.top

PHP:  public / protected / private
来源：http://aob.daxiang520.top

JS:   #private 字段；其余公开
来源：http://eab.cashguo.top

TS:   public / protected / private
来源：http://wyb.bbcook.cn

Java: public / protected / private / 默认包级
来源：http://fcb.shanyushiyangkeji.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://wth.ydjk.org.cn

Ruby: public / protected / private
来源：http://whz.feifeiyinyue.top

C#:   public / protected / private / internal
来源：http://ssf.birdmap.top

[G11] getter / setter
来源：http://ryj.smart0.xyz

Py:   @property 与 @x.setter
来源：http://sqn.yvedp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gzy.zhoulong.xyz

JS:   get name() { return this._name; }
来源：http://cut.jianghu66.top

TS:   get name(): string { return this._name; }
来源：http://gag.hammf.cn

Java: public String getName() { return name; }
来源：http://swx.snrcjt.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wtr.ehwqpu.com

Ruby: attr_accessor :name
来源：http://sen.zhixingplan.top

C#:   public string Name { get; set; }
来源：http://mxp.mhx1999.top

[G12] 对象转字符串
来源：http://cyc.yfazqb.com

Py:   def __str__(self): return self.name
来源：http://kmf.yanxiufei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fnf.feifeiyinyue.top

JS:   toString() { return this.name; }
来源：http://afi.pycfn.com

TS:   toString(): string { return this.name; }
来源：http://uep.snrcjt.cn

Java: @Override public String toString() { return name; }
来源：http://qwy.nwbrower.top

Go:   func (u User) String() string { return u.Name }
来源：http://rgx.xylfe.cn

Ruby: def to_s; @name; end
来源：http://zaj.xuetiantiany.cn

C#:   public override string ToString() => Name;
来源：http://uge.meibo888.top

[G13] 判断对象类型
来源：http://tkf.kuanghao11.cn

Py:   isinstance(u, User)
来源：http://qhp.wangdashe.top

PHP:  $u instanceof User
来源：http://hay.zdqjudy.top

JS:   u instanceof User
来源：http://vuc.sysykeji.top

TS:   u instanceof User
来源：http://yeg.hesvh.cn

Java: u instanceof User
来源：http://crw.fzhhl.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://oep.yongpay.top

Ruby: u.is_a?(User)
来源：http://qcs.xuanzx.com

C#:   u is User
来源：http://cnc.ydjk.org.cn

[G14] 数据类 / record
来源：http://cyz.pycfn.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yma.sweek.top

PHP:  // 用 readonly 属性模拟
来源：http://djz.c1oappe.top

JS:   // 无内置：普通类或对象字面量
来源：http://bat.guowangkeji.top

TS:   type User = { name: string; age: number };
来源：http://vxe.tanke756.top

Java: record User(String name, int age) {}
来源：http://ijs.gaohongyu789.top

Go:   type User struct { Name string; Age int }
来源：http://qlh.zycfv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xtp.fzhhl.top

C#:   record User(string Name, int Age);
来源：http://ejt.ehwqpu.com

[G15] 枚举
来源：http://odc.ydzc1.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fta.daria6918.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ehl.316326.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xjy.jiagoushi.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qds.nanxuanxn.top

Java: enum Color { RED, GREEN }
来源：http://rhw.xuetiantiany.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hux.yfazqb.com

Ruby: Color = %i[red green].freeze
来源：http://rvc.epnwcf.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rwm.yonumen.top

[G16] 对象转数组 / 字典
来源：http://klg.yangfankeji.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hsx.zhoulong.xyz

PHP:  get_object_vars($obj);
来源：http://lji.xingfuxueyuan.xyz

JS:   Object.entries(obj)
来源：http://yfl.hfpthk.cn

TS:   Object.entries(obj)
来源：http://pdf.yanxiufei.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vxc.316326.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://flc.zhiwuduotai.top

Ruby: obj.instance_variables
来源：http://bjj.yvedp.cn

C#:   // 用反射或 System.Text.Json
来源：http://aba.dashuyun.cn

================================================================================
来源：http://vxm.hnqzz.top

H. 异常与错误处理
来源：http://xpy.shanyushiyangtech.top

================================================================================
来源：http://ssg.jinqigufen.top

[H01] try / catch 基础
来源：http://pxp.zdbjq.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bml.yonumen.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jhj.ehwqpu.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jjx.snrcjt.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wfn.jinqigfzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pib.vqdsnc.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tbk.hywenlv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://opx.52xcode.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vpf.fehbvm.com

[H02] finally / ensure 收尾
来源：http://bkp.dashuyun.cn

Py:   try: f()⏎finally: cleanup()
来源：http://cqk.cashguo.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://fki.hesvh.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://krl.yj202588.top

TS:   try { f(); } finally { cleanup(); }
来源：http://qfq.shzxlz.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vjf.vqdsnc.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://avc.yangfankeji.com

Ruby: begin; f; ensure; cleanup; end
来源：http://ohi.dianchejie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dlb.zhaomingkeji.xyz

[H03] 主动抛出异常
来源：http://cfg.ybcxt.top

Py:   raise ValueError("错误信息")
来源：http://akg.chenlongwang.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gok.vehdjk.com

JS:   throw new Error("错误信息");
来源：http://jgx.birdmap.top

TS:   throw new Error("错误信息");
来源：http://ulc.smart0.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://fqg.fengsongda.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uyq.vqdsnc.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wmi.guowangkeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://fdn.0kj1m.cn

[H04] 自定义异常类型
来源：http://ggh.0kj1m.cn

Py:   class MyError(Exception): pass
来源：http://eux.zhongyouzk.top

PHP:  class MyError extends RuntimeException {}
来源：http://lqu.yvedp.cn

JS:   class MyError extends Error {}
来源：http://xhp.yueranfly.top

TS:   class MyError extends Error {}
来源：http://zfk.sxryk.cn

Java: class MyException extends RuntimeException {}
来源：http://egp.yanxiufei.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cny.ywan-chungtsiang.top

Ruby: class MyError < StandardError; end
来源：http://gnf.aizwys.cn

C#:   class MyException : Exception {}
来源：http://oct.sweek.top

[H05] 捕获特定类型
来源：http://dbk.kuanghao11.cn

Py:   except ValueError as e:
来源：http://nni.daxiang520.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dvh.wangdashe.top

JS:   if (e instanceof TypeError) {}
来源：http://tpz.vqdsnc.cn

TS:   if (e instanceof TypeError) {}
来源：http://qxs.hongshengwenyu.top

Java: catch (IOException | SQLException e) {}
来源：http://mqc.iojbl.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bjc.bbcook.cn

Ruby: rescue ArgumentError => e
来源：http://gqj.zhoulong.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ntr.nwbrower.top

[H06] 可选值 / 空值安全访问
来源：http://xlr.shanyushiyangtech.top

Py:   value = d.get("k") or default
来源：http://nye.ehwqpu.com

PHP:  $v = $d["k"] ?? null;
来源：http://nsv.snrcjt.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fmq.hesvh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zgi.fehbvm.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://oqg.52xcode.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ada.feifeiyinyue.top

Ruby: d&.dig(:a, :b)
来源：http://flv.52xcode.cn

C#:   obj?.A?.B ?? default
来源：http://lgr.cqqwz.cn

[H07] 断言
来源：http://mep.c1oappe.top

Py:   assert x > 0, "必须为正"
来源：http://jjq.hfpthk.cn

PHP:  assert($x > 0);
来源：http://bxw.sufxvd.cn

JS:   console.assert(x > 0);
来源：http://lzk.iojbl.cn

TS:   console.assert(x > 0);
来源：http://ubt.yj20258.top

Java: assert x > 0 : "必须为正";
来源：http://krd.jinqigufen.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rxb.jinghuilouyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bcw.chenjidiqi.icu

C#:   Debug.Assert(x > 0);
来源：http://xia.xylfe.cn

[H08] 获取错误信息与堆栈
来源：http://deq.shanyushiyangtech.top

Py:   str(e);  traceback.format_exc()
来源：http://iys.aizwys.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wkm.smart0.xyz

JS:   e.message;  e.stack
来源：http://qgv.ivvv.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ghe.yanxiufei.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mif.nanxuanxn.top

Go:   err.Error()
来源：http://ejz.jinqigufen.top

Ruby: e.message;  e.backtrace
来源：http://bkx.cqqwz.cn

C#:   e.Message;  e.StackTrace
来源：http://hzs.tianlin.xyz

[H09] 带错误码的异常
来源：http://iyd.jlsjyb.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cxq.yonumen.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://cks.mhx1999.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vqm.nanxuanxn.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kgs.kuanghao11.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vzn.gzhubu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kek.zhaomingkeji.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://rff.yangfankeji.com

C#:   // 自定义异常类中加 Code 属性
来源：http://ggz.wangshuangyany.cn

[H10] 资源自动释放
来源：http://cip.sxryk.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vja.zdbjq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://iio.iojbl.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bow.zycfv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lzg.nwbrower.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kej.pengpengdd.cyou

Go:   defer f.Close()
来源：http://ium.sufxvd.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://stn.zhengqikj.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tfn.quarkkingdee.top

================================================================================
来源：http://pfd.sweek.top

I. 正则表达式
来源：http://hnp.epnwcf.com

================================================================================
来源：http://xto.ybcxt.top

[I01] 判断是否匹配
来源：http://efo.52xcode.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bxn.shanyushiyangkeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://nrs.52xcode.cn

JS:   /\d+/.test(s)
来源：http://bdo.zhiwuduotai.top

TS:   /\d+/.test(s)
来源：http://jit.gaohongyu789.top


<!-- 参考信息 -->