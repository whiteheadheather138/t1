代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://hgl.havefunace.top

TS:   fs.unlinkSync("a.txt")
来源：http://drd.wangdashe.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qsv.fehbvm.com

Go:   os.Remove("a.txt")
来源：http://fav.uphjek.com

Ruby: File.delete("a.txt")
来源：http://dei.hysaishi.cn

C#:   File.Delete("a.txt");
来源：http://kek.yueranfly.top

[F07] 创建目录（含多级）
来源：http://mpo.snrcjt.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xoc.fengsongda.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yai.sweek.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hut.gzhubu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gwt.svipenyu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mor.vqdsnc.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bmd.yfazqb.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://znx.jqgfzy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uen.hesvh.cn

[F08] 遍历目录
来源：http://gnn.sysykeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://jhg.iojbl.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qit.zhixingplan.top

JS:   fs.readdirSync("dir")
来源：http://jua.jlsjyb.cn

TS:   fs.readdirSync("dir")
来源：http://xfy.fzhhl.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kds.zhaomingkeji.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://lwx.uphjek.com

Ruby: Dir.children("dir")
来源：http://yyg.yonumen.top

C#:   Directory.GetFiles("dir")
来源：http://dxe.smart0.xyz

[F09] 获取文件大小
来源：http://hkj.yvedp.cn

Py:   os.path.getsize("a.txt")
来源：http://vlk.mhx1999.top

PHP:  filesize("a.txt");
来源：http://gmc.tian-w.cn

JS:   fs.statSync("a.txt").size
来源：http://tzm.zhaomingkeji.xyz

TS:   fs.statSync("a.txt").size
来源：http://gmt.cucudq.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lly.fzhhl.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ssm.xylfe.cn

Ruby: File.size("a.txt")
来源：http://tbs.cucudq.cn

C#:   new FileInfo("a.txt").Length
来源：http://kdn.sjlbkw.cn

[F10] 取文件扩展名 / 文件名
来源：http://urz.yj202588.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ypf.sysykeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cwp.ctjpmb.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://crl.cucudq.cn

TS:   path.extname("a.txt")
来源：http://qms.tian-w.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://aoi.hnqzz.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lkh.andypj.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tas.dianchejie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cjd.daxiang520.top

[F11] 复制与移动文件
来源：http://yus.shzxlz.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tjn.jqgfzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sym.hnxiangtu.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ivq.cqqwz.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xxr.vqdsnc.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://smo.redwolf501.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xgf.sweek.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qor.fehbvm.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wyp.redwolf501.top

[F12] CSV 读写
来源：http://cuh.ctjpmb.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jax.jinyuanbaomall.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zyz.birdmap.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zlo.tarul.cn

TS:   // 同上
来源：http://hqs.svipenyu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nsf.shanyushiyangtech.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dzc.zhongyouzk.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sml.yvedp.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qot.sysykeji.top

================================================================================
来源：http://qcj.tanke756.top

G. 面向对象
来源：http://zeo.sufxvd.cn

================================================================================
来源：http://glw.pengpengdd.cyou

[G01] 定义类
来源：http://yik.zhixingplan.top

Py:   class User: pass
来源：http://rpu.bjfxy.top

PHP:  class User {}
来源：http://ori.jinqigfzy.top

JS:   class User {}
来源：http://nfc.fengsongda.top

TS:   class User { name: string = ""; }
来源：http://wzj.hfpthk.cn

Java: class User {}
来源：http://qgh.ybcxt.top

Go:   type User struct { Name string }
来源：http://tom.xziqi.cn

Ruby: class User; end
来源：http://uuu.gogol.net.cn

C#:   class User {}
来源：http://vly.chenlongwang.top

[G02] 构造函数
来源：http://ukh.epnwcf.com

Py:   def __init__(self, name): self.name = name
来源：http://bsi.pycfn.com

PHP:  public function __construct(public string $name) {}
来源：http://lva.bjfxy.top

JS:   constructor(name) { this.name = name; }
来源：http://hpd.mhx1999.top

TS:   constructor(public name: string) {}
来源：http://ihs.nanxinkj.top

Java: User(String name) { this.name = name; }
来源：http://alp.yj20258888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jcw.jinyuanbaomall.cn

Ruby: def initialize(name); @name = name; end
来源：http://kok.jinghuilouyu.cn

C#:   public User(string name) { Name = name; }
来源：http://xts.chenlongwang.top

[G03] 实例属性
来源：http://bqe.daxiang520.top

Py:   self.name = "x"
来源：http://bzk.yj20258.top

PHP:  public string $name = "x";
来源：http://jxb.zhijiandao.cn

JS:   this.name = "x";
来源：http://jtc.aizwys.cn

TS:   name: string = "x";
来源：http://pjb.sjlbkw.cn

Java: private String name;
来源：http://woz.ppjwa.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ijz.yvedp.cn

Ruby: @name = "x"
来源：http://gya.hongshengwenyu.top

C#:   public string Name { get; set; } = "x";
来源：http://hnw.hnqzz.top

[G04] 定义方法
来源：http://nze.haohaochexian.top

Py:   def greet(self): return self.name
来源：http://uzw.yanxiufei.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://sbs.yueranfly.top

JS:   greet() { return this.name; }
来源：http://cvc.hnxiangtu.top

TS:   greet(): string { return this.name; }
来源：http://mkk.jianghu66.top

Java: String greet() { return name; }
来源：http://wqp.fengsongda.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://txv.vqdsnc.cn

Ruby: def greet; @name; end
来源：http://uxp.aizwys.cn

C#:   public string Greet() => Name;
来源：http://shg.dianchejie.cn

[G05] 继承
来源：http://mya.guowangkeji.top

Py:   class Admin(User): pass
来源：http://pgo.dianchejie.cn

PHP:  class Admin extends User {}
来源：http://wbt.tianlin.xyz

JS:   class Admin extends User {}
来源：http://ftk.hywenlv.cn

TS:   class Admin extends User {}
来源：http://gro.cucudq.cn

Java: class Admin extends User {}
来源：http://ptz.chenlongwang.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jjs.ehwqpu.com

Ruby: class Admin < User; end
来源：http://mer.svipenyu.cn

C#:   class Admin : User {}
来源：http://pph.zhongyouzk.top

[G06] 重写方法
来源：http://pis.yfazqb.com

Py:   def greet(self): return "admin"
来源：http://mbn.c1oappe.top

PHP:  public function greet(): string { return "admin"; }
来源：http://mkf.cdnleiting.top

JS:   greet() { return "admin"; }
来源：http://wmc.haohaochexian.top

TS:   greet(): string { return "admin"; }
来源：http://zuo.jinqigufen.top

Java: @Override String greet() { return "admin"; }
来源：http://zam.shzxlz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mkz.haohaochexian.top

Ruby: def greet; "admin"; end
来源：http://off.tianlin.xyz

C#:   public override string Greet() => "admin";
来源：http://mgr.zhiwuduotai.top

[G07] 调用父类方法
来源：http://nwk.shangyingyoupin.top

Py:   super().greet()
来源：http://tec.zdqjudy.top

PHP:  parent::greet();
来源：http://cqg.yanxiufei.cn

JS:   super.greet();
来源：http://rnz.zhijiandao.cn

TS:   super.greet();
来源：http://qls.yj20258.top

Java: super.greet();
来源：http://cnc.yfazqb.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yon.jinqigfzy.top

Ruby: super
来源：http://qmt.yanxiufei.cn

C#:   base.Greet();
来源：http://efb.havefunace.top

[G08] 静态方法与属性
来源：http://zwx.smart0.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ojd.jiagoushi.top

PHP:  public static function f() {}
来源：http://vdq.xuanzx.com

JS:   static f() {}
来源：http://nhu.xziqi.cn

TS:   static f(): void {}
来源：http://vos.9152youxi.cn

Java: static void f() {}
来源：http://cbl.zhaomingkeji.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://igc.zhengqikj.top

Ruby: def self.f; end
来源：http://kuf.316326.xyz

C#:   public static void F() {}
来源：http://bya.mhx1999.top

[G09] 接口 / 抽象类
来源：http://svf.yj20258.top

Py:   from abc import ABC, abstractmethod
来源：http://rkz.xylfe.cn

PHP:  interface Shape { public function area(): float; }
来源：http://btl.xingfuxueyuan.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://ynn.zhijiandao.cn

TS:   interface Shape { area(): number; }
来源：http://smh.daria6918.cn

Java: interface Shape { double area(); }
来源：http://vvj.zhiwuduotai.top

Go:   type Shape interface { Area() float64 }
来源：http://phi.daria6918.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hrd.daria6918.cn

C#:   interface IShape { double Area(); }
来源：http://jwg.hammf.cn

[G10] 访问控制
来源：http://woj.zhijiandao.cn

Py:   约定 _protected / __private（不强制）
来源：http://tnl.iojbl.cn

PHP:  public / protected / private
来源：http://ufw.316326.xyz

JS:   #private 字段；其余公开
来源：http://vpr.chenjidiqi.icu

TS:   public / protected / private
来源：http://wcc.52xcode.cn

Java: public / protected / private / 默认包级
来源：http://oou.chenjidiqi.icu

Go:   首字母大写可导出，小写仅包内可见
来源：http://vls.hongshengwenyu.top

Ruby: public / protected / private
来源：http://imq.316326.xyz

C#:   public / protected / private / internal
来源：http://uav.sufxvd.cn

[G11] getter / setter
来源：http://uqa.wangshuangyany.cn

Py:   @property 与 @x.setter
来源：http://nvi.hcnkem.com

PHP:  public function getName(): string { return $this->name; }
来源：http://elb.ydzc1.top

JS:   get name() { return this._name; }
来源：http://hnd.guowangkeji.top

TS:   get name(): string { return this._name; }
来源：http://wpi.fktsv.cn

Java: public String getName() { return name; }
来源：http://jcg.aibaodan.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://owj.nwbrower.top

Ruby: attr_accessor :name
来源：http://mpa.aibaodan.cn

C#:   public string Name { get; set; }
来源：http://rqb.nwbrower.top

[G12] 对象转字符串
来源：http://cld.zycfv.cn

Py:   def __str__(self): return self.name
来源：http://nfj.zycfv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fpz.snrcjt.cn

JS:   toString() { return this.name; }
来源：http://prq.chenzaomai.com

TS:   toString(): string { return this.name; }
来源：http://iyz.xziqi.cn

Java: @Override public String toString() { return name; }
来源：http://jvv.hywenlv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://dbg.guowangkeji.top

Ruby: def to_s; @name; end
来源：http://wie.sysykeji.top

C#:   public override string ToString() => Name;
来源：http://gzp.jyoumei.cn

[G13] 判断对象类型
来源：http://bjy.yuxming.cn

Py:   isinstance(u, User)
来源：http://gpj.yonumen.top

PHP:  $u instanceof User
来源：http://dog.fengsongda.top

JS:   u instanceof User
来源：http://wjc.guannengcc.top

TS:   u instanceof User
来源：http://bhm.zhengqikj.top

Java: u instanceof User
来源：http://smt.sufxvd.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://yky.shanyushiyangkeji.top

Ruby: u.is_a?(User)
来源：http://fwx.fengsongda.top

C#:   u is User
来源：http://zvl.birdmap.top

[G14] 数据类 / record
来源：http://gik.yongpay.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fsy.tanke756.top

PHP:  // 用 readonly 属性模拟
来源：http://mir.dashuyun.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wqb.yj20258888.top

TS:   type User = { name: string; age: number };
来源：http://ivu.hywenlv.cn

Java: record User(String name, int age) {}
来源：http://cwt.cashguo.top

Go:   type User struct { Name string; Age int }
来源：http://yoi.c1oappe.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sjf.bbcook.cn

C#:   record User(string Name, int Age);
来源：http://xwj.gzhubu.top

[G15] 枚举
来源：http://rsy.tianlin.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tha.jianghu66.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://uwy.yonumen.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hpq.chenzaomai.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gge.yongpay.top

Java: enum Color { RED, GREEN }
来源：http://mmf.yuxming.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lqt.gaohongyu789.top

Ruby: Color = %i[red green].freeze
来源：http://idp.shanyushiyangtech.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mid.zhiwuduotai.top

[G16] 对象转数组 / 字典
来源：http://hru.uphjek.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://plw.jqgufenzy.top

PHP:  get_object_vars($obj);
来源：http://bne.smart0.xyz

JS:   Object.entries(obj)
来源：http://szc.aibaodan.cn

TS:   Object.entries(obj)
来源：http://tbx.haohaochexian.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yzd.9152youxi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://lbt.pengpengdd.cyou

Ruby: obj.instance_variables
来源：http://dfp.vqdsnc.cn

C#:   // 用反射或 System.Text.Json
来源：http://agt.hongshengwenyu.top

================================================================================
来源：http://cbr.kuanghao11.cn

H. 异常与错误处理
来源：http://jud.ywan-chungtsiang.top

================================================================================
来源：http://rdp.316326.xyz

[H01] try / catch 基础
来源：http://cjh.zhijiandao.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xfn.zhoulong.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dhf.sufxvd.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nkn.0kj1m.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://faa.hfpthk.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tvn.52xcode.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ucb.nanxinkj.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nnk.andypj.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lxx.ywan-chungtsiang.top

[H02] finally / ensure 收尾
来源：http://lsj.xingfuxueyuan.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://pvh.yuanzhike.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://qai.vehdjk.com

JS:   try { f(); } finally { cleanup(); }
来源：http://hcf.fengsongda.top

TS:   try { f(); } finally { cleanup(); }
来源：http://abn.hcnkem.com

Java: try { f(); } finally { cleanup(); }
来源：http://dwm.xinyue.icu

Go:   defer cleanup()             // 函数返回时执行
来源：http://pwo.andypj.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://lol.yueranfly.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://kru.xylfe.cn

[H03] 主动抛出异常
来源：http://lqe.yfazqb.com

Py:   raise ValueError("错误信息")
来源：http://lmz.gogol.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ypv.kuanghao11.cn

JS:   throw new Error("错误信息");
来源：http://lhp.ctjpmb.com

TS:   throw new Error("错误信息");
来源：http://wet.uphjek.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://ixn.pengpengdd.cyou

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xsj.9152youxi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://edh.tianlin.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://whm.jyoumei.cn

[H04] 自定义异常类型
来源：http://ris.chenlongwang.top

Py:   class MyError(Exception): pass
来源：http://gjd.yj20258.top

PHP:  class MyError extends RuntimeException {}
来源：http://jjf.xylfe.cn

JS:   class MyError extends Error {}
来源：http://eqz.zhijiandao.cn

TS:   class MyError extends Error {}
来源：http://sqc.zdqjudy.top

Java: class MyException extends RuntimeException {}
来源：http://vlo.ehwqpu.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ypx.shanyushiyangkeji.top

Ruby: class MyError < StandardError; end
来源：http://eok.gzhubu.top

C#:   class MyException : Exception {}
来源：http://dcn.nanxinkj.top

[H05] 捕获特定类型
来源：http://cfb.guowangkeji.top

Py:   except ValueError as e:
来源：http://bwh.0kj1m.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rpo.vqdsnc.cn

JS:   if (e instanceof TypeError) {}
来源：http://orh.hammf.cn

TS:   if (e instanceof TypeError) {}
来源：http://yco.cashguo.top

Java: catch (IOException | SQLException e) {}
来源：http://sho.jlsjyb.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vpe.hnxiangtu.top

Ruby: rescue ArgumentError => e
来源：http://thi.zdbjq.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zsy.jqgfzy.top

[H06] 可选值 / 空值安全访问
来源：http://idu.ppjwa.cn

Py:   value = d.get("k") or default
来源：http://jpy.bbcook.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bvt.shanyushiyangkeji.top

JS:   obj?.a?.b;  d ?? default
来源：http://xpw.meibo888.top

TS:   obj?.a?.b;  d ?? default
来源：http://ttn.guowangkeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gtf.daria6918.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hhc.ctjpmb.com

Ruby: d&.dig(:a, :b)
来源：http://vcg.yj202588.top

C#:   obj?.A?.B ?? default
来源：http://jli.jinqigfzy.top

[H07] 断言
来源：http://mpl.xuanzx.com

Py:   assert x > 0, "必须为正"
来源：http://nqo.tianlin.xyz

PHP:  assert($x > 0);
来源：http://mod.yuxming.cn

JS:   console.assert(x > 0);
来源：http://rno.zhengqikj.top

TS:   console.assert(x > 0);
来源：http://ubg.jlsjyb.cn

Java: assert x > 0 : "必须为正";
来源：http://cuf.daria6918.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ojx.zhongyouzk.top

Ruby: raise "必须为正" unless x > 0
来源：http://hdo.epnwcf.com

C#:   Debug.Assert(x > 0);
来源：http://tpy.guowangkeji.top

[H08] 获取错误信息与堆栈
来源：http://pxc.zhoulong.xyz

Py:   str(e);  traceback.format_exc()
来源：http://qxv.ctjpmb.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://iuc.zhengqikj.top

JS:   e.message;  e.stack
来源：http://pdp.feifeiyinyue.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://tzz.vehdjk.com

Java: e.getMessage();  e.printStackTrace()
来源：http://vif.uphjek.com

Go:   err.Error()
来源：http://wes.daria6918.cn

Ruby: e.message;  e.backtrace
来源：http://wft.316326.xyz

C#:   e.Message;  e.StackTrace
来源：http://efl.yuanzhike.top

[H09] 带错误码的异常
来源：http://rfr.fehbvm.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cyl.zdqjudy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://quh.wangshuangyany.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wlm.cheryme.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yaz.ppjwa.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qky.hcnkem.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ond.snrcjt.cn

Ruby: raise MyError.new("fail", 500)
来源：http://cij.c1oappe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ogz.fengsongda.top

[H10] 资源自动释放
来源：http://ufz.gotoacloud.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://lmy.vehdjk.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qby.zhijiandao.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uyj.aibaodan.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://acc.yueranfly.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xjo.shangyingyoupin.top

Go:   defer f.Close()
来源：http://tle.sweek.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mze.gogol.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pno.smart0.xyz


<!-- 参考信息 -->