代发 wailian999

Ruby: File.delete("a.txt")
来源：http://gfb.guannengcc.top

C#:   File.Delete("a.txt");
来源：http://ghd.quarkkingdee.top

[F07] 创建目录（含多级）
来源：http://vhs.shzxlz.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kwb.hnqzz.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://itq.jqgufenzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bmq.tianlin.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bxr.jyoumei.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kos.redwolf501.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sgi.jyoumei.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://leh.shzxlz.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qwe.cqqwz.cn

[F08] 遍历目录
来源：http://bfh.chenzaomai.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://ewe.hfpthk.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gns.vqdsnc.cn

JS:   fs.readdirSync("dir")
来源：http://ooz.havefunace.top

TS:   fs.readdirSync("dir")
来源：http://ytw.shuidangran.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kgl.ybcxt.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://tin.jianghu66.top

Ruby: Dir.children("dir")
来源：http://wwk.fengsongda.top

C#:   Directory.GetFiles("dir")
来源：http://goe.gotoacloud.top

[F09] 获取文件大小
来源：http://sva.xuanzx.com

Py:   os.path.getsize("a.txt")
来源：http://sbm.uphjek.com

PHP:  filesize("a.txt");
来源：http://kyf.fktsv.cn

JS:   fs.statSync("a.txt").size
来源：http://ojy.ppjwa.cn

TS:   fs.statSync("a.txt").size
来源：http://vdt.hnqzz.top

Java: Files.size(Path.of("a.txt"))
来源：http://vew.fzhhl.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cex.zhongyouzk.top

Ruby: File.size("a.txt")
来源：http://onv.cdnleiting.top

C#:   new FileInfo("a.txt").Length
来源：http://zpf.xuetiantiany.cn

[F10] 取文件扩展名 / 文件名
来源：http://ggr.9152youxi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mfa.sweek.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hvs.yanxiufei.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ect.dianchejie.cn

TS:   path.extname("a.txt")
来源：http://nbo.hongshengwenyu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vgd.wangdashe.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gje.jinqigfzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ysw.hfpthk.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dzn.zhiwuduotai.top

[F11] 复制与移动文件
来源：http://wjk.tanke756.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ljv.fengsongda.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dvb.vehdjk.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uwm.jyoumei.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tcg.yanxiufei.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gja.fktsv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kge.nanxinkj.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://egd.fengsongda.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://elc.jinyuanbaomall.cn

[F12] CSV 读写
来源：http://vky.jyoumei.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sei.tarul.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fim.tarul.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bjv.ehwqpu.com

TS:   // 同上
来源：http://ilf.cheryme.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://whw.birdmap.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kyf.bjfxy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://oji.zhengqikj.top

C#:   // 无内置：用 CsvHelper 库
来源：http://agt.0kj1m.cn

================================================================================
来源：http://xam.yueranfly.top

G. 面向对象
来源：http://ikv.ydjk.org.cn

================================================================================
来源：http://pci.pycfn.com

[G01] 定义类
来源：http://kkp.bbcook.cn

Py:   class User: pass
来源：http://tpb.guowangkeji.top

PHP:  class User {}
来源：http://zcl.daxiang520.top

JS:   class User {}
来源：http://mdb.jinyuanbaomall.cn

TS:   class User { name: string = ""; }
来源：http://ina.aibaodan.cn

Java: class User {}
来源：http://rzj.hammf.cn

Go:   type User struct { Name string }
来源：http://gww.ivvv.top

Ruby: class User; end
来源：http://qfo.hongshengwenyu.top

C#:   class User {}
来源：http://yqb.yangfankeji.com

[G02] 构造函数
来源：http://wud.cashguo.top

Py:   def __init__(self, name): self.name = name
来源：http://bys.ydzc1.top

PHP:  public function __construct(public string $name) {}
来源：http://iqc.ctjpmb.com

JS:   constructor(name) { this.name = name; }
来源：http://cqt.hesvh.cn

TS:   constructor(public name: string) {}
来源：http://glz.jinghuilouyu.cn

Java: User(String name) { this.name = name; }
来源：http://jzp.yj20258888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oyu.zhongyouzk.top

Ruby: def initialize(name); @name = name; end
来源：http://opn.jqgfzy.top

C#:   public User(string name) { Name = name; }
来源：http://hlh.yj20258.top

[G03] 实例属性
来源：http://oly.zdqjudy.top

Py:   self.name = "x"
来源：http://ied.cashguo.top

PHP:  public string $name = "x";
来源：http://aew.wangdashe.top

JS:   this.name = "x";
来源：http://emn.xziqi.cn

TS:   name: string = "x";
来源：http://xzj.zhongyouzk.top

Java: private String name;
来源：http://uzp.wangshuangyany.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ucl.yangfankeji.com

Ruby: @name = "x"
来源：http://rup.ybcxt.top

C#:   public string Name { get; set; } = "x";
来源：http://qru.fengsongda.top

[G04] 定义方法
来源：http://aul.jqgfzy.top

Py:   def greet(self): return self.name
来源：http://ian.nwbrower.top

PHP:  public function greet(): string { return $this->name; }
来源：http://jgc.jlsjyb.cn

JS:   greet() { return this.name; }
来源：http://dss.nwbrower.top

TS:   greet(): string { return this.name; }
来源：http://rzi.wangdashe.top

Java: String greet() { return name; }
来源：http://mok.vehdjk.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://jwq.snrcjt.cn

Ruby: def greet; @name; end
来源：http://jxq.cheryme.top

C#:   public string Greet() => Name;
来源：http://fat.shangyingyoupin.top

[G05] 继承
来源：http://lsu.ybcxt.top

Py:   class Admin(User): pass
来源：http://oaa.yonumen.top

PHP:  class Admin extends User {}
来源：http://txi.sxryk.cn

JS:   class Admin extends User {}
来源：http://lxq.hnxiangtu.top

TS:   class Admin extends User {}
来源：http://clr.zdbjq.cn

Java: class Admin extends User {}
来源：http://vnm.ydjk.org.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cyz.nanxuanxn.top

Ruby: class Admin < User; end
来源：http://axl.wangdashe.top

C#:   class Admin : User {}
来源：http://txw.vehdjk.com

[G06] 重写方法
来源：http://uaf.yj20258888.top

Py:   def greet(self): return "admin"
来源：http://tcm.epnwcf.com

PHP:  public function greet(): string { return "admin"; }
来源：http://emw.yuanzhike.top

JS:   greet() { return "admin"; }
来源：http://puh.fehbvm.com

TS:   greet(): string { return "admin"; }
来源：http://exj.havefunace.top

Java: @Override String greet() { return "admin"; }
来源：http://mex.tianlin.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uhk.tanke756.top

Ruby: def greet; "admin"; end
来源：http://eep.hysaishi.cn

C#:   public override string Greet() => "admin";
来源：http://eyn.hywenlv.cn

[G07] 调用父类方法
来源：http://ibw.guowangkeji.top

Py:   super().greet()
来源：http://zdo.jinqigufen.top

PHP:  parent::greet();
来源：http://ahb.mhx1999.top

JS:   super.greet();
来源：http://dlf.hnxiangtu.top

TS:   super.greet();
来源：http://xda.aibaodan.cn

Java: super.greet();
来源：http://avn.dianchejie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qfa.daria6918.cn

Ruby: super
来源：http://jen.gaohongyu789.top

C#:   base.Greet();
来源：http://jbx.zhoulong.xyz

[G08] 静态方法与属性
来源：http://eml.ydjk.org.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://shj.yanxiufei.cn

PHP:  public static function f() {}
来源：http://wkr.dashuyun.cn

JS:   static f() {}
来源：http://smd.hesvh.cn

TS:   static f(): void {}
来源：http://vby.zhoulong.xyz

Java: static void f() {}
来源：http://btt.yj202588.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://kdx.jianghu66.top

Ruby: def self.f; end
来源：http://lrw.yangfankeji.com

C#:   public static void F() {}
来源：http://fuj.yanxiufei.cn

[G09] 接口 / 抽象类
来源：http://pvy.birdmap.top

Py:   from abc import ABC, abstractmethod
来源：http://ogh.jinghuilouyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://inc.redwolf501.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://tih.c1oappe.top

TS:   interface Shape { area(): number; }
来源：http://crh.cdnleiting.top

Java: interface Shape { double area(); }
来源：http://iok.nanxinkj.top

Go:   type Shape interface { Area() float64 }
来源：http://kbs.gzhubu.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://esw.nwbrower.top

C#:   interface IShape { double Area(); }
来源：http://fvd.daxiang520.top

[G10] 访问控制
来源：http://btj.vqdsnc.cn

Py:   约定 _protected / __private（不强制）
来源：http://xts.hnxiangtu.top

PHP:  public / protected / private
来源：http://mmh.andypj.xyz

JS:   #private 字段；其余公开
来源：http://ecn.sysykeji.top

TS:   public / protected / private
来源：http://tvm.shzxlz.cn

Java: public / protected / private / 默认包级
来源：http://uls.ctjpmb.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://zey.smart0.xyz

Ruby: public / protected / private
来源：http://shy.yongpay.top

C#:   public / protected / private / internal
来源：http://ivc.tarul.cn

[G11] getter / setter
来源：http://ulz.yuanzhike.top

Py:   @property 与 @x.setter
来源：http://aeh.wangshuangyany.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pyr.vqdsnc.cn

JS:   get name() { return this._name; }
来源：http://zhz.nanxuanxn.top

TS:   get name(): string { return this._name; }
来源：http://eev.bbcook.cn

Java: public String getName() { return name; }
来源：http://oir.ydjk.org.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://blx.guannengcc.top

Ruby: attr_accessor :name
来源：http://pml.aibaodan.cn

C#:   public string Name { get; set; }
来源：http://lhq.fanxiaobao.xyz

[G12] 对象转字符串
来源：http://wmt.aibaodan.cn

Py:   def __str__(self): return self.name
来源：http://kip.kuanghao11.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://eoy.zhixingplan.top

JS:   toString() { return this.name; }
来源：http://tmf.yj202588.top

TS:   toString(): string { return this.name; }
来源：http://xww.havefunace.top

Java: @Override public String toString() { return name; }
来源：http://qcl.aibaodan.cn

Go:   func (u User) String() string { return u.Name }
来源：http://shr.jiagoushi.top

Ruby: def to_s; @name; end
来源：http://mhp.zdqjudy.top

C#:   public override string ToString() => Name;
来源：http://cpd.ybcxt.top

[G13] 判断对象类型
来源：http://upb.jinghuilouyu.cn

Py:   isinstance(u, User)
来源：http://cex.wangshuangyany.cn

PHP:  $u instanceof User
来源：http://hcj.cqqwz.cn

JS:   u instanceof User
来源：http://yxu.nanxuanxn.top

TS:   u instanceof User
来源：http://iaw.c1oappe.top

Java: u instanceof User
来源：http://vcb.hnqzz.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ijr.tian-w.cn

Ruby: u.is_a?(User)
来源：http://wvy.hnqzz.top

C#:   u is User
来源：http://nph.shanyushiyangkeji.top

[G14] 数据类 / record
来源：http://adt.fengsongda.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tjc.jiagoushi.top

PHP:  // 用 readonly 属性模拟
来源：http://vib.bbcook.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xel.zhengqikj.top

TS:   type User = { name: string; age: number };
来源：http://tji.zycfv.cn

Java: record User(String name, int age) {}
来源：http://tmo.havefunace.top

Go:   type User struct { Name string; Age int }
来源：http://guu.yangfankeji.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rez.jinghuilouyu.cn

C#:   record User(string Name, int Age);
来源：http://hiz.hysaishi.cn

[G15] 枚举
来源：http://spv.gzhubu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pbc.xinyue.icu

PHP:  enum Color: string { case Red = "red"; }
来源：http://ajk.sufxvd.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://aan.cqqwz.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rcq.sjlbkw.cn

Java: enum Color { RED, GREEN }
来源：http://gdv.bbcook.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gyo.gaohongyu789.top

Ruby: Color = %i[red green].freeze
来源：http://ikj.shzxlz.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nhv.yangfankeji.com

[G16] 对象转数组 / 字典
来源：http://pxr.hammf.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xvt.aibaodan.cn

PHP:  get_object_vars($obj);
来源：http://bvp.xuanzx.com

JS:   Object.entries(obj)
来源：http://ige.zhengqikj.top

TS:   Object.entries(obj)
来源：http://xie.pengpengdd.cyou

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://msq.cheryme.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://wya.fehbvm.com

Ruby: obj.instance_variables
来源：http://dge.zdqjudy.top

C#:   // 用反射或 System.Text.Json
来源：http://pof.hnqzz.top

================================================================================
来源：http://doh.sufxvd.cn

H. 异常与错误处理
来源：http://tmx.zhiwuduotai.top

================================================================================
来源：http://ibq.shanyushiyangkeji.top

[H01] try / catch 基础
来源：http://fff.tian-w.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://phn.zhoulong.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ooa.fktsv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mig.quarkkingdee.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yox.guannengcc.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bdd.xylfe.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jfr.pengpengdd.cyou

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zee.cdnleiting.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vuc.yueranfly.top

[H02] finally / ensure 收尾
来源：http://jag.jianghu66.top

Py:   try: f()⏎finally: cleanup()
来源：http://gdy.nwbrower.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://dpk.gaohongyu789.top

JS:   try { f(); } finally { cleanup(); }
来源：http://sgy.tian-w.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ltv.shzxlz.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ryv.hnxiangtu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://nda.0kj1m.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://paj.snrcjt.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yrv.sxryk.cn

[H03] 主动抛出异常
来源：http://slw.mhx1999.top

Py:   raise ValueError("错误信息")
来源：http://zhi.pengpengdd.cyou

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tai.hnqzz.top

JS:   throw new Error("错误信息");
来源：http://ldg.shuidangran.top

TS:   throw new Error("错误信息");
来源：http://bfu.sysykeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://dni.yuxming.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xlx.fanxiaobao.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://qxl.xinyue.icu

C#:   throw new ArgumentException("错误信息");
来源：http://pxh.yuxming.cn

[H04] 自定义异常类型
来源：http://bkl.jinqigufen.top

Py:   class MyError(Exception): pass
来源：http://koj.hcnkem.com

PHP:  class MyError extends RuntimeException {}
来源：http://hbf.tianlin.xyz

JS:   class MyError extends Error {}
来源：http://mtj.pengpengdd.cyou

TS:   class MyError extends Error {}
来源：http://yba.shanyushiyangkeji.top

Java: class MyException extends RuntimeException {}
来源：http://fzw.zhiwuduotai.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://esj.jianghu66.top

Ruby: class MyError < StandardError; end
来源：http://wiq.chenzaomai.com

C#:   class MyException : Exception {}
来源：http://fqv.shanyushiyangkeji.top

[H05] 捕获特定类型
来源：http://leh.yj20258888.top

Py:   except ValueError as e:
来源：http://lce.c1oappe.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dvx.zhengqikj.top

JS:   if (e instanceof TypeError) {}
来源：http://nhc.aibaodan.cn

TS:   if (e instanceof TypeError) {}
来源：http://ioq.kuanghao11.cn

Java: catch (IOException | SQLException e) {}
来源：http://kjn.dashuyun.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wun.hfpthk.cn

Ruby: rescue ArgumentError => e
来源：http://zes.sufxvd.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ult.zdqjudy.top

[H06] 可选值 / 空值安全访问
来源：http://ykn.feifeiyinyue.top

Py:   value = d.get("k") or default
来源：http://ixn.havefunace.top

PHP:  $v = $d["k"] ?? null;
来源：http://hjc.sysykeji.top

JS:   obj?.a?.b;  d ?? default
来源：http://zje.nanxinkj.top

TS:   obj?.a?.b;  d ?? default
来源：http://bsd.zhixingplan.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nbv.316326.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://tef.redwolf501.top

Ruby: d&.dig(:a, :b)
来源：http://ysy.gaohongyu789.top

C#:   obj?.A?.B ?? default
来源：http://afn.daria6918.cn

[H07] 断言
来源：http://xok.shangyingyoupin.top

Py:   assert x > 0, "必须为正"
来源：http://jzl.ybcxt.top

PHP:  assert($x > 0);
来源：http://teo.jqgufenzy.top

JS:   console.assert(x > 0);
来源：http://nwa.yongpay.top

TS:   console.assert(x > 0);
来源：http://ljv.epnwcf.com

Java: assert x > 0 : "必须为正";
来源：http://mib.chenjidiqi.icu

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://huh.daxiang520.top

Ruby: raise "必须为正" unless x > 0
来源：http://qdm.chenlongwang.top

C#:   Debug.Assert(x > 0);
来源：http://qan.ydjk.org.cn

[H08] 获取错误信息与堆栈
来源：http://scv.hnxiangtu.top

Py:   str(e);  traceback.format_exc()
来源：http://wgo.aibaodan.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hlk.dianchejie.cn

JS:   e.message;  e.stack
来源：http://akq.smart0.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://rmn.vqdsnc.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://lck.daxiang520.top

Go:   err.Error()
来源：http://ygo.sxryk.cn

Ruby: e.message;  e.backtrace
来源：http://ddj.bjfxy.top

C#:   e.Message;  e.StackTrace
来源：http://nmw.wangdashe.top

[H09] 带错误码的异常
来源：http://vgn.andypj.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qhn.sweek.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://jco.shanyushiyangtech.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wnj.yueranfly.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://enw.daria6918.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wjk.feifeiyinyue.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mmp.fengsongda.top

Ruby: raise MyError.new("fail", 500)
来源：http://yrm.meibo888.top

C#:   // 自定义异常类中加 Code 属性
来源：http://nlt.fktsv.cn

[H10] 资源自动释放
来源：http://gye.yj202588.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ibu.cdnleiting.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wpa.zhengqikj.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bnt.vqdsnc.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qwd.sxryk.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bmb.cashguo.top

Go:   defer f.Close()
来源：http://tcw.jqgufenzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://njb.yj20258888.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lau.chenjidiqi.icu

================================================================================
来源：http://scy.cheryme.top

I. 正则表达式
来源：http://pgm.snrcjt.cn

================================================================================
来源：http://zay.hongshengwenyu.top

[I01] 判断是否匹配
来源：http://oqv.aizwys.cn


<!-- 参考信息 -->