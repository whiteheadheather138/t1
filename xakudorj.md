代发 wailian999

Ruby: File.delete("a.txt")
来源：http://ryq.shzxlz.cn

C#:   File.Delete("a.txt");
来源：http://cle.yj20258888.top

[F07] 创建目录（含多级）
来源：http://wiq.chenjidiqi.icu

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cpp.shuidangran.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://weu.zhaomingkeji.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ntk.guowangkeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dhv.bjfxy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mrp.xuetiantiany.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rfe.vehdjk.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lxx.dashuyun.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qcr.jlsjyb.cn

[F08] 遍历目录
来源：http://iwf.hysaishi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rff.haohaochexian.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vqb.yonumen.top

JS:   fs.readdirSync("dir")
来源：http://aoe.cheryme.top

TS:   fs.readdirSync("dir")
来源：http://veu.xziqi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ara.mhx1999.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://fal.yangfankeji.com

Ruby: Dir.children("dir")
来源：http://wga.jianghu66.top

C#:   Directory.GetFiles("dir")
来源：http://rqa.aibaodan.cn

[F09] 获取文件大小
来源：http://rih.yvedp.cn

Py:   os.path.getsize("a.txt")
来源：http://pki.jianghu66.top

PHP:  filesize("a.txt");
来源：http://oie.yongpay.top

JS:   fs.statSync("a.txt").size
来源：http://nwp.jinyuanbaomall.cn

TS:   fs.statSync("a.txt").size
来源：http://yfp.fengsongda.top

Java: Files.size(Path.of("a.txt"))
来源：http://viq.cqqwz.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qdf.ivvv.top

Ruby: File.size("a.txt")
来源：http://kxw.quarkkingdee.top

C#:   new FileInfo("a.txt").Length
来源：http://tob.aizwys.cn

[F10] 取文件扩展名 / 文件名
来源：http://zop.ydzc1.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kgh.vqdsnc.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kcf.shanyushiyangtech.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://heo.gogol.net.cn

TS:   path.extname("a.txt")
来源：http://igr.ehwqpu.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bsu.mhx1999.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fcf.gogol.net.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://prz.hesvh.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kzu.jqgufenzy.top

[F11] 复制与移动文件
来源：http://csz.hnxiangtu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://its.yonumen.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wod.quarkkingdee.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yhd.chenzaomai.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nmm.zdbjq.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gzj.yuxming.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jju.52xcode.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xjm.birdmap.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cip.aibaodan.cn

[F12] CSV 读写
来源：http://qjs.hnqzz.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fnu.xziqi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lyo.nanxinkj.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xua.aizwys.cn

TS:   // 同上
来源：http://hfk.zdqjudy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zke.uphjek.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zkm.hnxiangtu.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fxo.hammf.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xom.ehwqpu.com

================================================================================
来源：http://zgu.zhoulong.xyz

G. 面向对象
来源：http://kql.vehdjk.com

================================================================================
来源：http://rme.sjlbkw.cn

[G01] 定义类
来源：http://fed.nwbrower.top

Py:   class User: pass
来源：http://bgs.chenzaomai.com

PHP:  class User {}
来源：http://kiz.tarul.cn

JS:   class User {}
来源：http://pdu.yangfankeji.com

TS:   class User { name: string = ""; }
来源：http://laf.fengsongda.top

Java: class User {}
来源：http://ydu.hnqzz.top

Go:   type User struct { Name string }
来源：http://ukf.guannengcc.top

Ruby: class User; end
来源：http://hrd.zhixingplan.top

C#:   class User {}
来源：http://ack.xinyue.icu

[G02] 构造函数
来源：http://scs.jyoumei.cn

Py:   def __init__(self, name): self.name = name
来源：http://ymy.tianlin.xyz

PHP:  public function __construct(public string $name) {}
来源：http://azc.bjfxy.top

JS:   constructor(name) { this.name = name; }
来源：http://swl.jlsjyb.cn

TS:   constructor(public name: string) {}
来源：http://xgi.hfpthk.cn

Java: User(String name) { this.name = name; }
来源：http://yql.hcnkem.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hsg.aizwys.cn

Ruby: def initialize(name); @name = name; end
来源：http://slt.vqdsnc.cn

C#:   public User(string name) { Name = name; }
来源：http://cpa.jinyuanbaomall.cn

[G03] 实例属性
来源：http://fvd.hnqzz.top

Py:   self.name = "x"
来源：http://jga.tian-w.cn

PHP:  public string $name = "x";
来源：http://eul.hnqzz.top

JS:   this.name = "x";
来源：http://vzv.yj202588.top

TS:   name: string = "x";
来源：http://amx.yongpay.top

Java: private String name;
来源：http://prb.zdbjq.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xzz.zhongyouzk.top

Ruby: @name = "x"
来源：http://zms.zhoulong.xyz

C#:   public string Name { get; set; } = "x";
来源：http://ohm.meibo888.top

[G04] 定义方法
来源：http://tep.yj20258888.top

Py:   def greet(self): return self.name
来源：http://vyz.uphjek.com

PHP:  public function greet(): string { return $this->name; }
来源：http://yfd.bjfxy.top

JS:   greet() { return this.name; }
来源：http://zwd.zdbjq.cn

TS:   greet(): string { return this.name; }
来源：http://hri.jinqigfzy.top

Java: String greet() { return name; }
来源：http://ndp.andypj.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://nlm.hnqzz.top

Ruby: def greet; @name; end
来源：http://zgg.gotoacloud.top

C#:   public string Greet() => Name;
来源：http://tgk.haohaochexian.top

[G05] 继承
来源：http://lia.chenzaomai.com

Py:   class Admin(User): pass
来源：http://dfe.aibaodan.cn

PHP:  class Admin extends User {}
来源：http://deg.sweek.top

JS:   class Admin extends User {}
来源：http://whr.zhongyouzk.top

TS:   class Admin extends User {}
来源：http://zvw.jqgufenzy.top

Java: class Admin extends User {}
来源：http://vqd.gzhubu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fcc.vqdsnc.cn

Ruby: class Admin < User; end
来源：http://hlw.shangyingyoupin.top

C#:   class Admin : User {}
来源：http://vdd.yj20258.top

[G06] 重写方法
来源：http://dzl.kuanghao11.cn

Py:   def greet(self): return "admin"
来源：http://kut.shzxlz.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qtu.cqqwz.cn

JS:   greet() { return "admin"; }
来源：http://wvz.smart0.xyz

TS:   greet(): string { return "admin"; }
来源：http://rsl.feifeiyinyue.top

Java: @Override String greet() { return "admin"; }
来源：http://vnr.hnxiangtu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nmj.zycfv.cn

Ruby: def greet; "admin"; end
来源：http://zsm.nwbrower.top

C#:   public override string Greet() => "admin";
来源：http://eff.mhx1999.top

[G07] 调用父类方法
来源：http://cua.hfpthk.cn

Py:   super().greet()
来源：http://gjx.jinghuilouyu.cn

PHP:  parent::greet();
来源：http://yaq.fzhhl.top

JS:   super.greet();
来源：http://ele.yuxming.cn

TS:   super.greet();
来源：http://ati.xylfe.cn

Java: super.greet();
来源：http://ioq.zhiwuduotai.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dbf.jqgfzy.top

Ruby: super
来源：http://taa.fengsongda.top

C#:   base.Greet();
来源：http://ztt.redwolf501.top

[G08] 静态方法与属性
来源：http://qyl.daria6918.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://row.ybcxt.top

PHP:  public static function f() {}
来源：http://dsp.jqgufenzy.top

JS:   static f() {}
来源：http://ibh.aizwys.cn

TS:   static f(): void {}
来源：http://etc.guowangkeji.top

Java: static void f() {}
来源：http://tfp.jqgufenzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://xux.nanxinkj.top

Ruby: def self.f; end
来源：http://iyx.316326.xyz

C#:   public static void F() {}
来源：http://ycb.hcnkem.com

[G09] 接口 / 抽象类
来源：http://tag.cucudq.cn

Py:   from abc import ABC, abstractmethod
来源：http://nko.snrcjt.cn

PHP:  interface Shape { public function area(): float; }
来源：http://fsd.gaohongyu789.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://jln.aizwys.cn

TS:   interface Shape { area(): number; }
来源：http://bra.shanyushiyangkeji.top

Java: interface Shape { double area(); }
来源：http://cgs.epnwcf.com

Go:   type Shape interface { Area() float64 }
来源：http://isr.jianghu66.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://buy.sweek.top

C#:   interface IShape { double Area(); }
来源：http://pge.ppjwa.cn

[G10] 访问控制
来源：http://hsy.daria6918.cn

Py:   约定 _protected / __private（不强制）
来源：http://gok.ydjk.org.cn

PHP:  public / protected / private
来源：http://qhr.vehdjk.com

JS:   #private 字段；其余公开
来源：http://fdl.zhaomingkeji.xyz

TS:   public / protected / private
来源：http://nfi.ehwqpu.com

Java: public / protected / private / 默认包级
来源：http://vsu.ppjwa.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ibi.chenzaomai.com

Ruby: public / protected / private
来源：http://igt.meibo888.top

C#:   public / protected / private / internal
来源：http://lgm.yuanzhike.top

[G11] getter / setter
来源：http://pai.redwolf501.top

Py:   @property 与 @x.setter
来源：http://afk.chenzaomai.com

PHP:  public function getName(): string { return $this->name; }
来源：http://ldf.tarul.cn

JS:   get name() { return this._name; }
来源：http://svz.pycfn.com

TS:   get name(): string { return this._name; }
来源：http://oti.hesvh.cn

Java: public String getName() { return name; }
来源：http://xrb.vehdjk.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://ier.hammf.cn

Ruby: attr_accessor :name
来源：http://iju.tianlin.xyz

C#:   public string Name { get; set; }
来源：http://gpc.vehdjk.com

[G12] 对象转字符串
来源：http://aow.hywenlv.cn

Py:   def __str__(self): return self.name
来源：http://blt.jinyuanbaomall.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mbx.gzhubu.top

JS:   toString() { return this.name; }
来源：http://yci.yongpay.top

TS:   toString(): string { return this.name; }
来源：http://ruf.sxryk.cn

Java: @Override public String toString() { return name; }
来源：http://ehu.zhaomingkeji.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://hfs.jinqigufen.top

Ruby: def to_s; @name; end
来源：http://vid.hnqzz.top

C#:   public override string ToString() => Name;
来源：http://ekl.nanxuanxn.top

[G13] 判断对象类型
来源：http://rbo.yuanzhike.top

Py:   isinstance(u, User)
来源：http://wnn.wangshuangyany.cn

PHP:  $u instanceof User
来源：http://jbz.ywan-chungtsiang.top

JS:   u instanceof User
来源：http://ztp.svipenyu.cn

TS:   u instanceof User
来源：http://eqv.yfazqb.com

Java: u instanceof User
来源：http://box.yueranfly.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://yec.tarul.cn

Ruby: u.is_a?(User)
来源：http://uzh.yanxiufei.cn

C#:   u is User
来源：http://ihm.fehbvm.com

[G14] 数据类 / record
来源：http://vxu.tian-w.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://spm.jqgufenzy.top

PHP:  // 用 readonly 属性模拟
来源：http://vag.cdnleiting.top

JS:   // 无内置：普通类或对象字面量
来源：http://rdt.yangfankeji.com

TS:   type User = { name: string; age: number };
来源：http://sil.vqdsnc.cn

Java: record User(String name, int age) {}
来源：http://pyw.haohaochexian.top

Go:   type User struct { Name string; Age int }
来源：http://yml.guowangkeji.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cky.yfazqb.com

C#:   record User(string Name, int Age);
来源：http://rrm.feifeiyinyue.top

[G15] 枚举
来源：http://cuu.zdqjudy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ago.yj202588.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ufl.zycfv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hlg.yueranfly.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dsc.yj202588.top

Java: enum Color { RED, GREEN }
来源：http://gbj.chenzaomai.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hkj.hfpthk.cn

Ruby: Color = %i[red green].freeze
来源：http://tfa.dianchejie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ksj.hysaishi.cn

[G16] 对象转数组 / 字典
来源：http://jhu.guowangkeji.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ufv.gogol.net.cn

PHP:  get_object_vars($obj);
来源：http://ysw.gotoacloud.top

JS:   Object.entries(obj)
来源：http://yhp.fktsv.cn

TS:   Object.entries(obj)
来源：http://vmi.fzhhl.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qmp.pycfn.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://asg.xylfe.cn

Ruby: obj.instance_variables
来源：http://ffw.zhiwuduotai.top

C#:   // 用反射或 System.Text.Json
来源：http://qvs.nanxinkj.top

================================================================================
来源：http://zjy.nanxuanxn.top

H. 异常与错误处理
来源：http://ezz.smart0.xyz

================================================================================
来源：http://mnz.zdbjq.cn

[H01] try / catch 基础
来源：http://mvx.xylfe.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gyz.zdbjq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://whx.shuidangran.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://snp.fktsv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qog.smart0.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://syl.chenzaomai.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dzx.0kj1m.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dyv.birdmap.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mdi.shzxlz.cn

[H02] finally / ensure 收尾
来源：http://igw.guowangkeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://xgp.fktsv.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://sgc.tarul.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://txr.zhengqikj.top

TS:   try { f(); } finally { cleanup(); }
来源：http://kfb.fehbvm.com

Java: try { f(); } finally { cleanup(); }
来源：http://tyr.daria6918.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rvb.zhengqikj.top

Ruby: begin; f; ensure; cleanup; end
来源：http://gve.zhengqikj.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ryr.jyoumei.cn

[H03] 主动抛出异常
来源：http://uim.zhengqikj.top

Py:   raise ValueError("错误信息")
来源：http://oif.sufxvd.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qfe.uphjek.com

JS:   throw new Error("错误信息");
来源：http://evs.zhixingplan.top

TS:   throw new Error("错误信息");
来源：http://mpr.sweek.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ind.nanxuanxn.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hwv.bjfxy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ulh.fzhhl.top

C#:   throw new ArgumentException("错误信息");
来源：http://vxx.xuanzx.com

[H04] 自定义异常类型
来源：http://dte.jinqigufen.top

Py:   class MyError(Exception): pass
来源：http://itb.jiagoushi.top

PHP:  class MyError extends RuntimeException {}
来源：http://fqm.c1oappe.top

JS:   class MyError extends Error {}
来源：http://pef.epnwcf.com

TS:   class MyError extends Error {}
来源：http://lxo.daria6918.cn

Java: class MyException extends RuntimeException {}
来源：http://oxj.bbcook.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ogi.9152youxi.cn

Ruby: class MyError < StandardError; end
来源：http://axo.guowangkeji.top

C#:   class MyException : Exception {}
来源：http://agy.xuanzx.com

[H05] 捕获特定类型
来源：http://utz.snrcjt.cn

Py:   except ValueError as e:
来源：http://tfn.bbcook.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vpg.dianchejie.cn

JS:   if (e instanceof TypeError) {}
来源：http://frq.hywenlv.cn

TS:   if (e instanceof TypeError) {}
来源：http://yvu.ppjwa.cn

Java: catch (IOException | SQLException e) {}
来源：http://dom.svipenyu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://boc.jinqigufen.top

Ruby: rescue ArgumentError => e
来源：http://pmb.tian-w.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pkq.hcnkem.com

[H06] 可选值 / 空值安全访问
来源：http://nvz.hnxiangtu.top

Py:   value = d.get("k") or default
来源：http://oho.dianchejie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cqh.zdbjq.cn

JS:   obj?.a?.b;  d ?? default
来源：http://uzl.quarkkingdee.top

TS:   obj?.a?.b;  d ?? default
来源：http://gdo.shanyushiyangtech.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dbg.yj202588.top

Go:   if v, ok := m["k"]; ok { }
来源：http://pnp.cucudq.cn

Ruby: d&.dig(:a, :b)
来源：http://tgq.yvedp.cn

C#:   obj?.A?.B ?? default
来源：http://jgr.wangshuangyany.cn

[H07] 断言
来源：http://rry.fehbvm.com

Py:   assert x > 0, "必须为正"
来源：http://xic.cashguo.top

PHP:  assert($x > 0);
来源：http://vys.shzxlz.cn

JS:   console.assert(x > 0);
来源：http://yrv.guannengcc.top

TS:   console.assert(x > 0);
来源：http://cbl.shangyingyoupin.top

Java: assert x > 0 : "必须为正";
来源：http://kkj.ywan-chungtsiang.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uyv.yfazqb.com

Ruby: raise "必须为正" unless x > 0
来源：http://dtp.ivvv.top

C#:   Debug.Assert(x > 0);
来源：http://fup.snrcjt.cn

[H08] 获取错误信息与堆栈
来源：http://kmw.ydzc1.top

Py:   str(e);  traceback.format_exc()
来源：http://kcy.pengpengdd.cyou

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gpu.nanxinkj.top

JS:   e.message;  e.stack
来源：http://vnv.hammf.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xaf.fanxiaobao.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://rro.bjfxy.top

Go:   err.Error()
来源：http://ncv.9152youxi.cn

Ruby: e.message;  e.backtrace
来源：http://mqs.uphjek.com

C#:   e.Message;  e.StackTrace
来源：http://qal.tian-w.cn

[H09] 带错误码的异常
来源：http://prp.smart0.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vqe.wangshuangyany.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jpu.gzhubu.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ivm.snrcjt.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nnr.sweek.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tjk.0kj1m.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nwl.ybcxt.top

Ruby: raise MyError.new("fail", 500)
来源：http://zts.guannengcc.top

C#:   // 自定义异常类中加 Code 属性
来源：http://pee.tarul.cn

[H10] 资源自动释放
来源：http://amc.bbcook.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jph.aizwys.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cvj.sufxvd.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ehs.yonumen.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mbu.birdmap.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://aip.zhongyouzk.top

Go:   defer f.Close()
来源：http://ndm.gaohongyu789.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fxz.gaohongyu789.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://spx.yueranfly.top

================================================================================
来源：http://jcn.jyoumei.cn

I. 正则表达式
来源：http://nws.shuidangran.top

================================================================================
来源：http://dnz.hnqzz.top

[I01] 判断是否匹配
来源：http://wjj.zhongyouzk.top


<!-- 参考信息 -->