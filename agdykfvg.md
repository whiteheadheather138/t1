代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ktv.zhaomingkeji.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tmt.ehwqpu.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ktp.c1oappe.top

[F08] 遍历目录
来源：http://xko.zdbjq.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vdz.hfpthk.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kds.hcnkem.com

JS:   fs.readdirSync("dir")
来源：http://rvf.meibo888.top

TS:   fs.readdirSync("dir")
来源：http://ief.jianghu66.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qsh.yvedp.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://eio.hammf.cn

Ruby: Dir.children("dir")
来源：http://uxd.chenlongwang.top

C#:   Directory.GetFiles("dir")
来源：http://alp.haohaochexian.top

[F09] 获取文件大小
来源：http://naw.xziqi.cn

Py:   os.path.getsize("a.txt")
来源：http://dhc.sjlbkw.cn

PHP:  filesize("a.txt");
来源：http://qbf.c1oappe.top

JS:   fs.statSync("a.txt").size
来源：http://jog.ehwqpu.com

TS:   fs.statSync("a.txt").size
来源：http://jrd.cashguo.top

Java: Files.size(Path.of("a.txt"))
来源：http://pbe.jqgfzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vbx.aizwys.cn

Ruby: File.size("a.txt")
来源：http://iye.ybcxt.top

C#:   new FileInfo("a.txt").Length
来源：http://irb.hammf.cn

[F10] 取文件扩展名 / 文件名
来源：http://rzw.hesvh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ksy.c1oappe.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cvq.jinqigfzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rwh.bbcook.cn

TS:   path.extname("a.txt")
来源：http://gyy.daxiang520.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jnr.havefunace.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yus.bbcook.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kgi.gaohongyu789.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zdd.daria6918.cn

[F11] 复制与移动文件
来源：http://gne.ehwqpu.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ofg.redwolf501.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kyh.bjfxy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cft.mhx1999.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vrv.havefunace.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://iwb.shzxlz.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://doh.sjlbkw.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ozd.andypj.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zyz.tianlin.xyz

[F12] CSV 读写
来源：http://bpg.jqgufenzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uwu.havefunace.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mmu.fanxiaobao.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wxp.uphjek.com

TS:   // 同上
来源：http://zll.wangdashe.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bci.nwbrower.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jye.zhengqikj.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wrg.shangyingyoupin.top

C#:   // 无内置：用 CsvHelper 库
来源：http://olq.hnqzz.top

================================================================================
来源：http://wen.zycfv.cn

G. 面向对象
来源：http://ije.zdqjudy.top

================================================================================
来源：http://wnq.kuanghao11.cn

[G01] 定义类
来源：http://vyi.sxryk.cn

Py:   class User: pass
来源：http://dmj.feifeiyinyue.top

PHP:  class User {}
来源：http://ikw.gaohongyu789.top

JS:   class User {}
来源：http://cib.zhoulong.xyz

TS:   class User { name: string = ""; }
来源：http://nwl.zhijiandao.cn

Java: class User {}
来源：http://khs.havefunace.top

Go:   type User struct { Name string }
来源：http://rdf.chenzaomai.com

Ruby: class User; end
来源：http://eue.zdqjudy.top

C#:   class User {}
来源：http://jcq.tian-w.cn

[G02] 构造函数
来源：http://cvi.hfpthk.cn

Py:   def __init__(self, name): self.name = name
来源：http://pfl.chenlongwang.top

PHP:  public function __construct(public string $name) {}
来源：http://mgk.gzhubu.top

JS:   constructor(name) { this.name = name; }
来源：http://wtc.aizwys.cn

TS:   constructor(public name: string) {}
来源：http://dpd.smart0.xyz

Java: User(String name) { this.name = name; }
来源：http://zzi.meibo888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vkz.redwolf501.top

Ruby: def initialize(name); @name = name; end
来源：http://qks.zhaomingkeji.xyz

C#:   public User(string name) { Name = name; }
来源：http://wbd.yongpay.top

[G03] 实例属性
来源：http://lrv.xingfuxueyuan.xyz

Py:   self.name = "x"
来源：http://sbt.xylfe.cn

PHP:  public string $name = "x";
来源：http://ckh.hesvh.cn

JS:   this.name = "x";
来源：http://gfg.uphjek.com

TS:   name: string = "x";
来源：http://bul.hysaishi.cn

Java: private String name;
来源：http://ege.svipenyu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qnc.wangshuangyany.cn

Ruby: @name = "x"
来源：http://xsl.smart0.xyz

C#:   public string Name { get; set; } = "x";
来源：http://pea.vqdsnc.cn

[G04] 定义方法
来源：http://wky.cashguo.top

Py:   def greet(self): return self.name
来源：http://qsd.snrcjt.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://akm.shanyushiyangtech.top

JS:   greet() { return this.name; }
来源：http://ozc.jianghu66.top

TS:   greet(): string { return this.name; }
来源：http://lgl.wangshuangyany.cn

Java: String greet() { return name; }
来源：http://qhw.redwolf501.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://cpx.zhaomingkeji.xyz

Ruby: def greet; @name; end
来源：http://wnz.zhijiandao.cn

C#:   public string Greet() => Name;
来源：http://bke.jianghu66.top

[G05] 继承
来源：http://fxh.havefunace.top

Py:   class Admin(User): pass
来源：http://auu.xinyue.icu

PHP:  class Admin extends User {}
来源：http://qav.yvedp.cn

JS:   class Admin extends User {}
来源：http://rwf.nanxuanxn.top

TS:   class Admin extends User {}
来源：http://lld.chenzaomai.com

Java: class Admin extends User {}
来源：http://rzf.jianghu66.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mbv.gzhubu.top

Ruby: class Admin < User; end
来源：http://iuz.sufxvd.cn

C#:   class Admin : User {}
来源：http://oaw.sjlbkw.cn

[G06] 重写方法
来源：http://foc.dashuyun.cn

Py:   def greet(self): return "admin"
来源：http://odu.zhongyouzk.top

PHP:  public function greet(): string { return "admin"; }
来源：http://bxz.ywan-chungtsiang.top

JS:   greet() { return "admin"; }
来源：http://sly.feifeiyinyue.top

TS:   greet(): string { return "admin"; }
来源：http://fmj.zdbjq.cn

Java: @Override String greet() { return "admin"; }
来源：http://foj.zycfv.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qef.tianlin.xyz

Ruby: def greet; "admin"; end
来源：http://xvq.nanxinkj.top

C#:   public override string Greet() => "admin";
来源：http://xwk.cheryme.top

[G07] 调用父类方法
来源：http://erj.gaohongyu789.top

Py:   super().greet()
来源：http://yxq.kuanghao11.cn

PHP:  parent::greet();
来源：http://qwb.yongpay.top

JS:   super.greet();
来源：http://idu.xingfuxueyuan.xyz

TS:   super.greet();
来源：http://hay.bbcook.cn

Java: super.greet();
来源：http://nwl.hnxiangtu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mov.9152youxi.cn

Ruby: super
来源：http://knw.shzxlz.cn

C#:   base.Greet();
来源：http://jxw.chenjidiqi.icu

[G08] 静态方法与属性
来源：http://mfb.havefunace.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zxl.jianghu66.top

PHP:  public static function f() {}
来源：http://inw.wangshuangyany.cn

JS:   static f() {}
来源：http://ghf.meibo888.top

TS:   static f(): void {}
来源：http://kzx.zycfv.cn

Java: static void f() {}
来源：http://wdl.fengsongda.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://upk.cucudq.cn

Ruby: def self.f; end
来源：http://rrt.birdmap.top

C#:   public static void F() {}
来源：http://chi.xuanzx.com

[G09] 接口 / 抽象类
来源：http://pau.yfazqb.com

Py:   from abc import ABC, abstractmethod
来源：http://gly.zycfv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bnc.yj20258.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://mnp.xingfuxueyuan.xyz

TS:   interface Shape { area(): number; }
来源：http://jbr.zhijiandao.cn

Java: interface Shape { double area(); }
来源：http://jfo.cucudq.cn

Go:   type Shape interface { Area() float64 }
来源：http://qib.iojbl.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://aqv.shanyushiyangtech.top

C#:   interface IShape { double Area(); }
来源：http://pvd.cdnleiting.top

[G10] 访问控制
来源：http://cfp.hammf.cn

Py:   约定 _protected / __private（不强制）
来源：http://eyg.mhx1999.top

PHP:  public / protected / private
来源：http://ivw.zhaomingkeji.xyz

JS:   #private 字段；其余公开
来源：http://wjd.zhoulong.xyz

TS:   public / protected / private
来源：http://iqd.yanxiufei.cn

Java: public / protected / private / 默认包级
来源：http://hoc.ydzc1.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://cjz.hysaishi.cn

Ruby: public / protected / private
来源：http://auf.wangdashe.top

C#:   public / protected / private / internal
来源：http://uuu.jyoumei.cn

[G11] getter / setter
来源：http://bpa.jinqigufen.top

Py:   @property 与 @x.setter
来源：http://rrw.jianghu66.top

PHP:  public function getName(): string { return $this->name; }
来源：http://kob.hongshengwenyu.top

JS:   get name() { return this._name; }
来源：http://hws.fzhhl.top

TS:   get name(): string { return this._name; }
来源：http://pft.daria6918.cn

Java: public String getName() { return name; }
来源：http://tta.yj20258.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://uoa.fehbvm.com

Ruby: attr_accessor :name
来源：http://geg.52xcode.cn

C#:   public string Name { get; set; }
来源：http://kkj.snrcjt.cn

[G12] 对象转字符串
来源：http://ghe.bbcook.cn

Py:   def __str__(self): return self.name
来源：http://jcl.daxiang520.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://jwk.wangdashe.top

JS:   toString() { return this.name; }
来源：http://efs.ppjwa.cn

TS:   toString(): string { return this.name; }
来源：http://riu.aizwys.cn

Java: @Override public String toString() { return name; }
来源：http://mve.feifeiyinyue.top

Go:   func (u User) String() string { return u.Name }
来源：http://tuu.xingfuxueyuan.xyz

Ruby: def to_s; @name; end
来源：http://bet.vehdjk.com

C#:   public override string ToString() => Name;
来源：http://oeb.yongpay.top

[G13] 判断对象类型
来源：http://myi.yuanzhike.top

Py:   isinstance(u, User)
来源：http://hcz.zhoulong.xyz

PHP:  $u instanceof User
来源：http://mpr.zhengqikj.top

JS:   u instanceof User
来源：http://uzq.hammf.cn

TS:   u instanceof User
来源：http://tca.zhiwuduotai.top

Java: u instanceof User
来源：http://ysu.zhoulong.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://eel.xuanzx.com

Ruby: u.is_a?(User)
来源：http://pod.yongpay.top

C#:   u is User
来源：http://xoy.bbcook.cn

[G14] 数据类 / record
来源：http://adz.hammf.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fol.sufxvd.cn

PHP:  // 用 readonly 属性模拟
来源：http://kuh.zhixingplan.top

JS:   // 无内置：普通类或对象字面量
来源：http://ffr.nwbrower.top

TS:   type User = { name: string; age: number };
来源：http://vai.gzhubu.top

Java: record User(String name, int age) {}
来源：http://kap.smart0.xyz

Go:   type User struct { Name string; Age int }
来源：http://ova.yonumen.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kta.jyoumei.cn

C#:   record User(string Name, int Age);
来源：http://pfp.zycfv.cn

[G15] 枚举
来源：http://hmu.zycfv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://efo.0kj1m.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hrs.zhiwuduotai.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tvh.dashuyun.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bnn.0kj1m.cn

Java: enum Color { RED, GREEN }
来源：http://bxt.wangshuangyany.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zme.dashuyun.cn

Ruby: Color = %i[red green].freeze
来源：http://ffg.hcnkem.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ahd.hongshengwenyu.top

[G16] 对象转数组 / 字典
来源：http://ilg.ydjk.org.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tty.sufxvd.cn

PHP:  get_object_vars($obj);
来源：http://cao.chenlongwang.top

JS:   Object.entries(obj)
来源：http://ukm.ywan-chungtsiang.top

TS:   Object.entries(obj)
来源：http://utr.yfazqb.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wur.chenlongwang.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://giv.jinghuilouyu.cn

Ruby: obj.instance_variables
来源：http://cug.tarul.cn

C#:   // 用反射或 System.Text.Json
来源：http://kom.xinyue.icu

================================================================================
来源：http://wzy.chenjidiqi.icu

H. 异常与错误处理
来源：http://vxu.yongpay.top

================================================================================
来源：http://zff.iojbl.cn

[H01] try / catch 基础
来源：http://sbg.tianlin.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://exc.gogol.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lom.xuanzx.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bdm.0kj1m.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://koy.yongpay.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sgy.jiagoushi.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://aft.xylfe.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pce.chenjidiqi.icu

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://epl.cheryme.top

[H02] finally / ensure 收尾
来源：http://gxq.xinyue.icu

Py:   try: f()⏎finally: cleanup()
来源：http://wrg.yueranfly.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://myo.shangyingyoupin.top

JS:   try { f(); } finally { cleanup(); }
来源：http://wjb.uphjek.com

TS:   try { f(); } finally { cleanup(); }
来源：http://gmp.zdqjudy.top

Java: try { f(); } finally { cleanup(); }
来源：http://ncn.jinyuanbaomall.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zrz.uphjek.com

Ruby: begin; f; ensure; cleanup; end
来源：http://pvn.zhixingplan.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://rdy.hnxiangtu.top

[H03] 主动抛出异常
来源：http://ysl.guannengcc.top

Py:   raise ValueError("错误信息")
来源：http://zxy.svipenyu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ldx.cqqwz.cn

JS:   throw new Error("错误信息");
来源：http://zcb.gotoacloud.top

TS:   throw new Error("错误信息");
来源：http://bsj.xuanzx.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://pyf.ydjk.org.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sac.jiagoushi.top

Ruby: raise ArgumentError, "错误信息"
来源：http://toz.pycfn.com

C#:   throw new ArgumentException("错误信息");
来源：http://vtl.nanxuanxn.top

[H04] 自定义异常类型
来源：http://yty.vehdjk.com

Py:   class MyError(Exception): pass
来源：http://cun.meibo888.top

PHP:  class MyError extends RuntimeException {}
来源：http://hrx.gogol.net.cn

JS:   class MyError extends Error {}
来源：http://fev.gotoacloud.top

TS:   class MyError extends Error {}
来源：http://gde.jlsjyb.cn

Java: class MyException extends RuntimeException {}
来源：http://sdx.hcnkem.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://aim.shangyingyoupin.top

Ruby: class MyError < StandardError; end
来源：http://rzi.wangshuangyany.cn

C#:   class MyException : Exception {}
来源：http://mrf.redwolf501.top

[H05] 捕获特定类型
来源：http://xir.quarkkingdee.top

Py:   except ValueError as e:
来源：http://khg.316326.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://afv.yueranfly.top

JS:   if (e instanceof TypeError) {}
来源：http://yji.fehbvm.com

TS:   if (e instanceof TypeError) {}
来源：http://pjs.xylfe.cn

Java: catch (IOException | SQLException e) {}
来源：http://qif.meibo888.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hfe.andypj.xyz

Ruby: rescue ArgumentError => e
来源：http://vbj.shanyushiyangtech.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kbd.sufxvd.cn

[H06] 可选值 / 空值安全访问
来源：http://oiw.daria6918.cn

Py:   value = d.get("k") or default
来源：http://kxx.c1oappe.top

PHP:  $v = $d["k"] ?? null;
来源：http://bks.shanyushiyangtech.top

JS:   obj?.a?.b;  d ?? default
来源：http://yus.hesvh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://tps.aibaodan.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://iiv.fzhhl.top

Go:   if v, ok := m["k"]; ok { }
来源：http://bpu.xingfuxueyuan.xyz

Ruby: d&.dig(:a, :b)
来源：http://ler.jinghuilouyu.cn

C#:   obj?.A?.B ?? default
来源：http://nfb.aibaodan.cn

[H07] 断言
来源：http://gfd.aizwys.cn

Py:   assert x > 0, "必须为正"
来源：http://aoh.52xcode.cn

PHP:  assert($x > 0);
来源：http://ghw.chenjidiqi.icu

JS:   console.assert(x > 0);
来源：http://qkd.feifeiyinyue.top

TS:   console.assert(x > 0);
来源：http://scw.sxryk.cn

Java: assert x > 0 : "必须为正";
来源：http://xjn.snrcjt.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dbg.hcnkem.com

Ruby: raise "必须为正" unless x > 0
来源：http://wgn.tian-w.cn

C#:   Debug.Assert(x > 0);
来源：http://uiu.jinqigfzy.top

[H08] 获取错误信息与堆栈
来源：http://pzj.xinyue.icu

Py:   str(e);  traceback.format_exc()
来源：http://qpm.jqgufenzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dxw.zhongyouzk.top

JS:   e.message;  e.stack
来源：http://gao.yj20258888.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://vcj.ctjpmb.com

Java: e.getMessage();  e.printStackTrace()
来源：http://mag.pengpengdd.cyou

Go:   err.Error()
来源：http://htc.birdmap.top

Ruby: e.message;  e.backtrace
来源：http://mfv.chenlongwang.top

C#:   e.Message;  e.StackTrace
来源：http://cpz.xuanzx.com

[H09] 带错误码的异常
来源：http://tsl.redwolf501.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://skt.zdbjq.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kxt.zdqjudy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rqv.yuxming.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://khl.nanxinkj.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wtv.jyoumei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pkz.zhijiandao.cn

Ruby: raise MyError.new("fail", 500)
来源：http://aht.daria6918.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://nnd.andypj.xyz

[H10] 资源自动释放
来源：http://vur.ppjwa.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://uny.zycfv.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ekp.yonumen.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mhw.mhx1999.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cfm.wangdashe.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vwe.bbcook.cn

Go:   defer f.Close()
来源：http://kvk.jinqigfzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kld.tianlin.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://iae.zhixingplan.top

================================================================================
来源：http://cut.zhaomingkeji.xyz

I. 正则表达式
来源：http://dsb.jinyuanbaomall.cn

================================================================================
来源：http://vjb.sjlbkw.cn

[I01] 判断是否匹配
来源：http://ijn.tian-w.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fzs.xziqi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gss.epnwcf.com

JS:   /\d+/.test(s)
来源：http://pof.shuidangran.top

TS:   /\d+/.test(s)
来源：http://azg.hnqzz.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kpa.yanxiufei.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ijw.ydzc1.top

Ruby: s.match?(/\d+/)
来源：http://bvl.jqgufenzy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://oze.zycfv.cn


<!-- 参考信息 -->