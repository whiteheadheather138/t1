代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zbd.yj202588.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://emw.nanxinkj.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ggc.yfazqb.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vaf.52xcode.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dzq.cheryme.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tha.pengpengdd.cyou

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kdi.fengsongda.top

[F08] 遍历目录
来源：http://dtj.yvedp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mrj.cheryme.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zwv.havefunace.top

JS:   fs.readdirSync("dir")
来源：http://yfi.fktsv.cn

TS:   fs.readdirSync("dir")
来源：http://fyw.birdmap.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://uwx.xuanzx.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://ism.hcnkem.com

Ruby: Dir.children("dir")
来源：http://nzx.gaohongyu789.top

C#:   Directory.GetFiles("dir")
来源：http://ece.zhaomingkeji.xyz

[F09] 获取文件大小
来源：http://rlv.bjfxy.top

Py:   os.path.getsize("a.txt")
来源：http://jlo.kuanghao11.cn

PHP:  filesize("a.txt");
来源：http://qzi.hfpthk.cn

JS:   fs.statSync("a.txt").size
来源：http://hht.hnxiangtu.top

TS:   fs.statSync("a.txt").size
来源：http://dqw.dashuyun.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rlt.zhiwuduotai.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mco.ywan-chungtsiang.top

Ruby: File.size("a.txt")
来源：http://iws.jyoumei.cn

C#:   new FileInfo("a.txt").Length
来源：http://ceb.vqdsnc.cn

[F10] 取文件扩展名 / 文件名
来源：http://olv.yfazqb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pcd.shanyushiyangtech.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hhp.xuanzx.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tfg.havefunace.top

TS:   path.extname("a.txt")
来源：http://oqi.gaohongyu789.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tvz.xuetiantiany.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fiu.svipenyu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bin.quarkkingdee.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tbb.gzhubu.top

[F11] 复制与移动文件
来源：http://nju.316326.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dmp.chenjidiqi.icu

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rax.svipenyu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lhm.gaohongyu789.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cwp.0kj1m.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://aed.nanxinkj.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ljp.yvedp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mdy.0kj1m.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rmv.ydjk.org.cn

[F12] CSV 读写
来源：http://olf.dianchejie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zok.yj20258888.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jat.sysykeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xrs.nanxuanxn.top

TS:   // 同上
来源：http://hcs.hnxiangtu.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kjc.svipenyu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xuj.vqdsnc.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kkk.shanyushiyangkeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://lfd.fzhhl.top

================================================================================
来源：http://yzq.zdbjq.cn

G. 面向对象
来源：http://kss.jinqigfzy.top

================================================================================
来源：http://qvh.pengpengdd.cyou

[G01] 定义类
来源：http://nqg.epnwcf.com

Py:   class User: pass
来源：http://txu.yongpay.top

PHP:  class User {}
来源：http://wpc.yfazqb.com

JS:   class User {}
来源：http://svw.wangdashe.top

TS:   class User { name: string = ""; }
来源：http://kjs.fktsv.cn

Java: class User {}
来源：http://aky.hfpthk.cn

Go:   type User struct { Name string }
来源：http://tbs.yongpay.top

Ruby: class User; end
来源：http://xys.snrcjt.cn

C#:   class User {}
来源：http://ivo.dashuyun.cn

[G02] 构造函数
来源：http://kde.hywenlv.cn

Py:   def __init__(self, name): self.name = name
来源：http://xls.zdbjq.cn

PHP:  public function __construct(public string $name) {}
来源：http://jjb.shangyingyoupin.top

JS:   constructor(name) { this.name = name; }
来源：http://kgw.yj20258888.top

TS:   constructor(public name: string) {}
来源：http://ezl.meibo888.top

Java: User(String name) { this.name = name; }
来源：http://nib.dianchejie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://egv.birdmap.top

Ruby: def initialize(name); @name = name; end
来源：http://zcn.zhongyouzk.top

C#:   public User(string name) { Name = name; }
来源：http://ndx.shangyingyoupin.top

[G03] 实例属性
来源：http://mlo.gzhubu.top

Py:   self.name = "x"
来源：http://ago.yuxming.cn

PHP:  public string $name = "x";
来源：http://min.shanyushiyangtech.top

JS:   this.name = "x";
来源：http://rzz.nwbrower.top

TS:   name: string = "x";
来源：http://jrv.yj20258.top

Java: private String name;
来源：http://slc.shuidangran.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bxr.hysaishi.cn

Ruby: @name = "x"
来源：http://qvm.shanyushiyangtech.top

C#:   public string Name { get; set; } = "x";
来源：http://cmk.yvedp.cn

[G04] 定义方法
来源：http://wqv.zhijiandao.cn

Py:   def greet(self): return self.name
来源：http://qvz.sysykeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://rnx.hysaishi.cn

JS:   greet() { return this.name; }
来源：http://xfk.guannengcc.top

TS:   greet(): string { return this.name; }
来源：http://dbp.shzxlz.cn

Java: String greet() { return name; }
来源：http://zke.xylfe.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ayp.hongshengwenyu.top

Ruby: def greet; @name; end
来源：http://dzf.zhengqikj.top

C#:   public string Greet() => Name;
来源：http://scg.kuanghao11.cn

[G05] 继承
来源：http://awi.cdnleiting.top

Py:   class Admin(User): pass
来源：http://wic.birdmap.top

PHP:  class Admin extends User {}
来源：http://eoo.hnxiangtu.top

JS:   class Admin extends User {}
来源：http://dtk.zdbjq.cn

TS:   class Admin extends User {}
来源：http://gpk.pengpengdd.cyou

Java: class Admin extends User {}
来源：http://bbv.sxryk.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dbt.zhengqikj.top

Ruby: class Admin < User; end
来源：http://ype.pengpengdd.cyou

C#:   class Admin : User {}
来源：http://xcs.yonumen.top

[G06] 重写方法
来源：http://tgw.zdqjudy.top

Py:   def greet(self): return "admin"
来源：http://rtf.jinghuilouyu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ecu.wangdashe.top

JS:   greet() { return "admin"; }
来源：http://lrk.hongshengwenyu.top

TS:   greet(): string { return "admin"; }
来源：http://fgt.52xcode.cn

Java: @Override String greet() { return "admin"; }
来源：http://hlz.tarul.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vrl.vqdsnc.cn

Ruby: def greet; "admin"; end
来源：http://vfz.haohaochexian.top

C#:   public override string Greet() => "admin";
来源：http://izj.sufxvd.cn

[G07] 调用父类方法
来源：http://ifh.feifeiyinyue.top

Py:   super().greet()
来源：http://gri.shangyingyoupin.top

PHP:  parent::greet();
来源：http://rjc.havefunace.top

JS:   super.greet();
来源：http://wjk.wangshuangyany.cn

TS:   super.greet();
来源：http://ykt.316326.xyz

Java: super.greet();
来源：http://lpu.yonumen.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dvt.hysaishi.cn

Ruby: super
来源：http://pfc.cheryme.top

C#:   base.Greet();
来源：http://cbx.gzhubu.top

[G08] 静态方法与属性
来源：http://wnw.yj20258888.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jtp.chenzaomai.com

PHP:  public static function f() {}
来源：http://lnp.hysaishi.cn

JS:   static f() {}
来源：http://sjq.chenjidiqi.icu

TS:   static f(): void {}
来源：http://ssz.shangyingyoupin.top

Java: static void f() {}
来源：http://ihr.yfazqb.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://elp.xziqi.cn

Ruby: def self.f; end
来源：http://ehn.quarkkingdee.top

C#:   public static void F() {}
来源：http://sft.ywan-chungtsiang.top

[G09] 接口 / 抽象类
来源：http://xok.gzhubu.top

Py:   from abc import ABC, abstractmethod
来源：http://jfa.316326.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://ckd.zhiwuduotai.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://rww.nwbrower.top

TS:   interface Shape { area(): number; }
来源：http://flq.hfpthk.cn

Java: interface Shape { double area(); }
来源：http://oqr.fehbvm.com

Go:   type Shape interface { Area() float64 }
来源：http://avw.jqgufenzy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wny.dashuyun.cn

C#:   interface IShape { double Area(); }
来源：http://iqt.feifeiyinyue.top

[G10] 访问控制
来源：http://aiq.zycfv.cn

Py:   约定 _protected / __private（不强制）
来源：http://twg.hywenlv.cn

PHP:  public / protected / private
来源：http://yih.cucudq.cn

JS:   #private 字段；其余公开
来源：http://qji.cucudq.cn

TS:   public / protected / private
来源：http://knp.daxiang520.top

Java: public / protected / private / 默认包级
来源：http://bts.chenjidiqi.icu

Go:   首字母大写可导出，小写仅包内可见
来源：http://kff.nanxuanxn.top

Ruby: public / protected / private
来源：http://hra.yueranfly.top

C#:   public / protected / private / internal
来源：http://rby.shanyushiyangkeji.top

[G11] getter / setter
来源：http://pvb.yueranfly.top

Py:   @property 与 @x.setter
来源：http://izz.gotoacloud.top

PHP:  public function getName(): string { return $this->name; }
来源：http://nvn.hnxiangtu.top

JS:   get name() { return this._name; }
来源：http://ysx.zycfv.cn

TS:   get name(): string { return this._name; }
来源：http://vby.9152youxi.cn

Java: public String getName() { return name; }
来源：http://ejx.chenjidiqi.icu

Go:   func (u User) GetName() string { return u.Name }
来源：http://eor.sjlbkw.cn

Ruby: attr_accessor :name
来源：http://ghv.pycfn.com

C#:   public string Name { get; set; }
来源：http://gqo.jinqigfzy.top

[G12] 对象转字符串
来源：http://gnn.redwolf501.top

Py:   def __str__(self): return self.name
来源：http://fez.cdnleiting.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://znj.iojbl.cn

JS:   toString() { return this.name; }
来源：http://bii.zhoulong.xyz

TS:   toString(): string { return this.name; }
来源：http://irc.0kj1m.cn

Java: @Override public String toString() { return name; }
来源：http://rmo.kuanghao11.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fln.cheryme.top

Ruby: def to_s; @name; end
来源：http://eaq.chenjidiqi.icu

C#:   public override string ToString() => Name;
来源：http://ncs.cucudq.cn

[G13] 判断对象类型
来源：http://kqd.yongpay.top

Py:   isinstance(u, User)
来源：http://uxg.xziqi.cn

PHP:  $u instanceof User
来源：http://ibg.yvedp.cn

JS:   u instanceof User
来源：http://mon.fehbvm.com

TS:   u instanceof User
来源：http://crp.yongpay.top

Java: u instanceof User
来源：http://lfw.vqdsnc.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pls.9152youxi.cn

Ruby: u.is_a?(User)
来源：http://niv.cashguo.top

C#:   u is User
来源：http://ruf.shanyushiyangkeji.top

[G14] 数据类 / record
来源：http://dha.zdbjq.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bdx.hfpthk.cn

PHP:  // 用 readonly 属性模拟
来源：http://rzj.chenlongwang.top

JS:   // 无内置：普通类或对象字面量
来源：http://gqo.yueranfly.top

TS:   type User = { name: string; age: number };
来源：http://gbp.yuxming.cn

Java: record User(String name, int age) {}
来源：http://sbz.jinghuilouyu.cn

Go:   type User struct { Name string; Age int }
来源：http://gas.fktsv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qyk.hammf.cn

C#:   record User(string Name, int Age);
来源：http://hbm.smart0.xyz

[G15] 枚举
来源：http://kuz.yj20258.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://oyq.hnxiangtu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://plh.zhixingplan.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iqg.smart0.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://eyb.ywan-chungtsiang.top

Java: enum Color { RED, GREEN }
来源：http://gwl.yj20258888.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sxm.shzxlz.cn

Ruby: Color = %i[red green].freeze
来源：http://fcl.dashuyun.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hlo.yonumen.top

[G16] 对象转数组 / 字典
来源：http://cpi.zhongyouzk.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://byf.zhoulong.xyz

PHP:  get_object_vars($obj);
来源：http://jit.haohaochexian.top

JS:   Object.entries(obj)
来源：http://zhr.jqgufenzy.top

TS:   Object.entries(obj)
来源：http://pox.aibaodan.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rou.yonumen.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://upi.havefunace.top

Ruby: obj.instance_variables
来源：http://gzb.zhixingplan.top

C#:   // 用反射或 System.Text.Json
来源：http://mve.jinghuilouyu.cn

================================================================================
来源：http://rcu.yongpay.top

H. 异常与错误处理
来源：http://rzg.jinghuilouyu.cn

================================================================================
来源：http://twz.haohaochexian.top

[H01] try / catch 基础
来源：http://gsa.tarul.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hhc.svipenyu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jkc.xuetiantiany.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uyd.zhengqikj.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yza.wangdashe.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hgz.yuxming.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bof.xingfuxueyuan.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://eqa.yvedp.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zdd.hnxiangtu.top

[H02] finally / ensure 收尾
来源：http://vku.sjlbkw.cn

Py:   try: f()⏎finally: cleanup()
来源：http://bgd.daxiang520.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://yxb.hesvh.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://nnn.cucudq.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ksc.chenlongwang.top

Java: try { f(); } finally { cleanup(); }
来源：http://vrk.gzhubu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://kdv.pycfn.com

Ruby: begin; f; ensure; cleanup; end
来源：http://keb.vehdjk.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://lye.jqgufenzy.top

[H03] 主动抛出异常
来源：http://xfl.haohaochexian.top

Py:   raise ValueError("错误信息")
来源：http://knv.0kj1m.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rct.fktsv.cn

JS:   throw new Error("错误信息");
来源：http://avf.yvedp.cn

TS:   throw new Error("错误信息");
来源：http://ykp.dashuyun.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lap.316326.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://geu.tian-w.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://kca.hywenlv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vuf.ydzc1.top

[H04] 自定义异常类型
来源：http://jxi.quarkkingdee.top

Py:   class MyError(Exception): pass
来源：http://zal.yueranfly.top

PHP:  class MyError extends RuntimeException {}
来源：http://tfr.tarul.cn

JS:   class MyError extends Error {}
来源：http://lsq.gaohongyu789.top

TS:   class MyError extends Error {}
来源：http://dxf.meibo888.top

Java: class MyException extends RuntimeException {}
来源：http://jun.nwbrower.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://txe.316326.xyz

Ruby: class MyError < StandardError; end
来源：http://hct.c1oappe.top

C#:   class MyException : Exception {}
来源：http://iie.gogol.net.cn

[H05] 捕获特定类型
来源：http://zuz.zhixingplan.top

Py:   except ValueError as e:
来源：http://gga.chenzaomai.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qtm.jqgfzy.top

JS:   if (e instanceof TypeError) {}
来源：http://pqp.zhixingplan.top

TS:   if (e instanceof TypeError) {}
来源：http://kzv.52xcode.cn

Java: catch (IOException | SQLException e) {}
来源：http://hth.yj20258888.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gmt.fanxiaobao.xyz

Ruby: rescue ArgumentError => e
来源：http://knv.ivvv.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lst.hysaishi.cn

[H06] 可选值 / 空值安全访问
来源：http://niy.yj202588.top

Py:   value = d.get("k") or default
来源：http://mpk.guowangkeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://mdf.yanxiufei.cn

JS:   obj?.a?.b;  d ?? default
来源：http://euv.nanxinkj.top

TS:   obj?.a?.b;  d ?? default
来源：http://eca.hnqzz.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xqx.tarul.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jyo.bbcook.cn

Ruby: d&.dig(:a, :b)
来源：http://scq.fktsv.cn

C#:   obj?.A?.B ?? default
来源：http://lew.birdmap.top

[H07] 断言
来源：http://ubr.smart0.xyz

Py:   assert x > 0, "必须为正"
来源：http://ohx.cdnleiting.top

PHP:  assert($x > 0);
来源：http://rdk.nwbrower.top

JS:   console.assert(x > 0);
来源：http://lsh.tian-w.cn

TS:   console.assert(x > 0);
来源：http://naw.sxryk.cn

Java: assert x > 0 : "必须为正";
来源：http://toe.yongpay.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lrc.ctjpmb.com

Ruby: raise "必须为正" unless x > 0
来源：http://vqh.havefunace.top

C#:   Debug.Assert(x > 0);
来源：http://slc.guowangkeji.top

[H08] 获取错误信息与堆栈
来源：http://svw.zycfv.cn

Py:   str(e);  traceback.format_exc()
来源：http://rut.ywan-chungtsiang.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sut.hnqzz.top

JS:   e.message;  e.stack
来源：http://yqj.iojbl.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://joy.yj20258888.top

Java: e.getMessage();  e.printStackTrace()
来源：http://gai.yongpay.top

Go:   err.Error()
来源：http://gcp.ywan-chungtsiang.top

Ruby: e.message;  e.backtrace
来源：http://ggf.hnxiangtu.top

C#:   e.Message;  e.StackTrace
来源：http://exa.shzxlz.cn

[H09] 带错误码的异常
来源：http://bmv.ivvv.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xsz.hcnkem.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://gtq.nwbrower.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ptf.yanxiufei.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xiv.zhaomingkeji.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dum.wangshuangyany.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dsn.vqdsnc.cn

Ruby: raise MyError.new("fail", 500)
来源：http://lcd.sxryk.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ycf.epnwcf.com

[H10] 资源自动释放
来源：http://fes.kuanghao11.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://dwg.ydzc1.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mbf.gzhubu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baz.316326.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://viz.fktsv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pbq.ydjk.org.cn

Go:   defer f.Close()
来源：http://cdq.nanxinkj.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ipy.quarkkingdee.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://moa.yangfankeji.com

================================================================================
来源：http://eje.yfazqb.com

I. 正则表达式
来源：http://ede.yj202588.top

================================================================================
来源：http://bnt.sjlbkw.cn

[I01] 判断是否匹配
来源：http://iqg.yueranfly.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://iwf.yueranfly.top

PHP:  preg_match('/\d+/', $s);
来源：http://hvx.shzxlz.cn

JS:   /\d+/.test(s)
来源：http://wjt.guannengcc.top

TS:   /\d+/.test(s)
来源：http://mut.birdmap.top


<!-- 参考信息 -->