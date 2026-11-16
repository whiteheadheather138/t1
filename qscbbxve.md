代发 wailian999

C#:   File.Exists("a.txt")
来源：http://oei.sysykeji.top

[F06] 删除文件
来源：http://muj.yangfankeji.com

Py:   os.remove("a.txt")
来源：http://fgd.yongpay.top

PHP:  unlink("a.txt");
来源：http://xeg.fehbvm.com

JS:   fs.unlinkSync("a.txt")
来源：http://prp.9152youxi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://oaz.snrcjt.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ldl.nanxuanxn.top

Go:   os.Remove("a.txt")
来源：http://fhm.tanke756.top

Ruby: File.delete("a.txt")
来源：http://nxe.daxiang520.top

C#:   File.Delete("a.txt");
来源：http://pfu.shanyushiyangtech.top

[F07] 创建目录（含多级）
来源：http://yuc.yueranfly.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://efu.aizwys.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lvr.zhijiandao.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qpm.hfpthk.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nea.daxiang520.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ohl.shanyushiyangkeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kxp.uphjek.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rtw.zdbjq.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ztb.yvedp.cn

[F08] 遍历目录
来源：http://xqd.haohaochexian.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ntj.sxryk.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://upo.jyoumei.cn

JS:   fs.readdirSync("dir")
来源：http://xtd.dashuyun.cn

TS:   fs.readdirSync("dir")
来源：http://mub.zycfv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qat.c1oappe.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://uib.ywan-chungtsiang.top

Ruby: Dir.children("dir")
来源：http://yhw.haohaochexian.top

C#:   Directory.GetFiles("dir")
来源：http://zbz.sweek.top

[F09] 获取文件大小
来源：http://fsc.fzhhl.top

Py:   os.path.getsize("a.txt")
来源：http://pvc.gotoacloud.top

PHP:  filesize("a.txt");
来源：http://ggr.chenzaomai.com

JS:   fs.statSync("a.txt").size
来源：http://zut.zhongyouzk.top

TS:   fs.statSync("a.txt").size
来源：http://gfn.ctjpmb.com

Java: Files.size(Path.of("a.txt"))
来源：http://bpr.dianchejie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fza.zhaomingkeji.xyz

Ruby: File.size("a.txt")
来源：http://kko.ydzc1.top

C#:   new FileInfo("a.txt").Length
来源：http://jnt.epnwcf.com

[F10] 取文件扩展名 / 文件名
来源：http://dsy.cucudq.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xki.fanxiaobao.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gmo.jinqigfzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://msp.shanyushiyangtech.top

TS:   path.extname("a.txt")
来源：http://hyx.pengpengdd.cyou

Java: // 手动 substring(lastIndexOf('.'))
来源：http://uaf.yj20258888.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://och.0kj1m.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nbj.ppjwa.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xrw.ctjpmb.com

[F11] 复制与移动文件
来源：http://ptb.yonumen.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kom.ydzc1.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://imh.jiagoushi.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nbf.zdqjudy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jqz.gzhubu.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bgs.ybcxt.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yaa.yuxming.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bio.daxiang520.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pqi.cucudq.cn

[F12] CSV 读写
来源：http://shk.yongpay.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zlf.cashguo.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://umm.tian-w.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mnw.yvedp.cn

TS:   // 同上
来源：http://ypg.xuanzx.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ijp.iojbl.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://awq.yangfankeji.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://atx.yj20258888.top

C#:   // 无内置：用 CsvHelper 库
来源：http://bop.pycfn.com

================================================================================
来源：http://eyu.meibo888.top

G. 面向对象
来源：http://riw.fktsv.cn

================================================================================
来源：http://rkm.xylfe.cn

[G01] 定义类
来源：http://qmw.xziqi.cn

Py:   class User: pass
来源：http://nvg.zhengqikj.top

PHP:  class User {}
来源：http://zlm.jinqigufen.top

JS:   class User {}
来源：http://sey.cashguo.top

TS:   class User { name: string = ""; }
来源：http://iyf.zdbjq.cn

Java: class User {}
来源：http://kgn.pycfn.com

Go:   type User struct { Name string }
来源：http://tvy.fzhhl.top

Ruby: class User; end
来源：http://caf.havefunace.top

C#:   class User {}
来源：http://kjy.shangyingyoupin.top

[G02] 构造函数
来源：http://pdv.sweek.top

Py:   def __init__(self, name): self.name = name
来源：http://cuc.0kj1m.cn

PHP:  public function __construct(public string $name) {}
来源：http://ykb.sysykeji.top

JS:   constructor(name) { this.name = name; }
来源：http://mps.hcnkem.com

TS:   constructor(public name: string) {}
来源：http://rzh.snrcjt.cn

Java: User(String name) { this.name = name; }
来源：http://apl.ivvv.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://poq.dashuyun.cn

Ruby: def initialize(name); @name = name; end
来源：http://kxj.svipenyu.cn

C#:   public User(string name) { Name = name; }
来源：http://evo.redwolf501.top

[G03] 实例属性
来源：http://jwo.fengsongda.top

Py:   self.name = "x"
来源：http://hfa.nanxinkj.top

PHP:  public string $name = "x";
来源：http://ypr.andypj.xyz

JS:   this.name = "x";
来源：http://rkm.cdnleiting.top

TS:   name: string = "x";
来源：http://esf.hywenlv.cn

Java: private String name;
来源：http://xuf.ydzc1.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hlq.hfpthk.cn

Ruby: @name = "x"
来源：http://fqe.shanyushiyangkeji.top

C#:   public string Name { get; set; } = "x";
来源：http://qpw.nwbrower.top

[G04] 定义方法
来源：http://bci.yuxming.cn

Py:   def greet(self): return self.name
来源：http://sib.tarul.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zwk.jinyuanbaomall.cn

JS:   greet() { return this.name; }
来源：http://zgh.cucudq.cn

TS:   greet(): string { return this.name; }
来源：http://ycb.cashguo.top

Java: String greet() { return name; }
来源：http://ryw.jinyuanbaomall.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rhw.gogol.net.cn

Ruby: def greet; @name; end
来源：http://mhf.tian-w.cn

C#:   public string Greet() => Name;
来源：http://moi.yj20258.top

[G05] 继承
来源：http://jha.tanke756.top

Py:   class Admin(User): pass
来源：http://iou.nwbrower.top

PHP:  class Admin extends User {}
来源：http://kag.tanke756.top

JS:   class Admin extends User {}
来源：http://ivt.jinqigufen.top

TS:   class Admin extends User {}
来源：http://mgi.fehbvm.com

Java: class Admin extends User {}
来源：http://hov.zhengqikj.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hpb.epnwcf.com

Ruby: class Admin < User; end
来源：http://oaf.316326.xyz

C#:   class Admin : User {}
来源：http://kzz.jinghuilouyu.cn

[G06] 重写方法
来源：http://wlw.jqgfzy.top

Py:   def greet(self): return "admin"
来源：http://udg.cheryme.top

PHP:  public function greet(): string { return "admin"; }
来源：http://jbj.jianghu66.top

JS:   greet() { return "admin"; }
来源：http://vck.feifeiyinyue.top

TS:   greet(): string { return "admin"; }
来源：http://jos.yj20258888.top

Java: @Override String greet() { return "admin"; }
来源：http://ejj.havefunace.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mvo.pengpengdd.cyou

Ruby: def greet; "admin"; end
来源：http://lqj.c1oappe.top

C#:   public override string Greet() => "admin";
来源：http://ikl.ctjpmb.com

[G07] 调用父类方法
来源：http://rsg.xziqi.cn

Py:   super().greet()
来源：http://iwj.pengpengdd.cyou

PHP:  parent::greet();
来源：http://rek.jianghu66.top

JS:   super.greet();
来源：http://yzw.hfpthk.cn

TS:   super.greet();
来源：http://tgu.zhijiandao.cn

Java: super.greet();
来源：http://kkv.xuetiantiany.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://adk.tianlin.xyz

Ruby: super
来源：http://nkt.pengpengdd.cyou

C#:   base.Greet();
来源：http://yem.aibaodan.cn

[G08] 静态方法与属性
来源：http://vzi.yangfankeji.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://iam.yj202588.top

PHP:  public static function f() {}
来源：http://xdm.yuanzhike.top

JS:   static f() {}
来源：http://owx.ydzc1.top

TS:   static f(): void {}
来源：http://tdz.zhaomingkeji.xyz

Java: static void f() {}
来源：http://kiz.iojbl.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://non.aizwys.cn

Ruby: def self.f; end
来源：http://lhf.yvedp.cn

C#:   public static void F() {}
来源：http://sta.gzhubu.top

[G09] 接口 / 抽象类
来源：http://pbj.hnxiangtu.top

Py:   from abc import ABC, abstractmethod
来源：http://ibn.feifeiyinyue.top

PHP:  interface Shape { public function area(): float; }
来源：http://vvs.zhiwuduotai.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://tpi.jqgfzy.top

TS:   interface Shape { area(): number; }
来源：http://rgn.shanyushiyangtech.top

Java: interface Shape { double area(); }
来源：http://pmu.hywenlv.cn

Go:   type Shape interface { Area() float64 }
来源：http://qyt.xziqi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://asy.xuetiantiany.cn

C#:   interface IShape { double Area(); }
来源：http://ima.tanke756.top

[G10] 访问控制
来源：http://fbs.chenlongwang.top

Py:   约定 _protected / __private（不强制）
来源：http://qvo.xylfe.cn

PHP:  public / protected / private
来源：http://kut.mhx1999.top

JS:   #private 字段；其余公开
来源：http://iuv.birdmap.top

TS:   public / protected / private
来源：http://opz.shzxlz.cn

Java: public / protected / private / 默认包级
来源：http://gco.guannengcc.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://suz.xylfe.cn

Ruby: public / protected / private
来源：http://ugu.sjlbkw.cn

C#:   public / protected / private / internal
来源：http://roj.jlsjyb.cn

[G11] getter / setter
来源：http://bxa.shanyushiyangtech.top

Py:   @property 与 @x.setter
来源：http://zyc.zhengqikj.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ssx.meibo888.top

JS:   get name() { return this._name; }
来源：http://vhd.nwbrower.top

TS:   get name(): string { return this._name; }
来源：http://uvg.redwolf501.top

Java: public String getName() { return name; }
来源：http://vop.gotoacloud.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://tel.bjfxy.top

Ruby: attr_accessor :name
来源：http://aul.c1oappe.top

C#:   public string Name { get; set; }
来源：http://pms.cashguo.top

[G12] 对象转字符串
来源：http://otw.hywenlv.cn

Py:   def __str__(self): return self.name
来源：http://bnx.yj20258.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://evr.bbcook.cn

JS:   toString() { return this.name; }
来源：http://koy.hongshengwenyu.top

TS:   toString(): string { return this.name; }
来源：http://zex.jqgfzy.top

Java: @Override public String toString() { return name; }
来源：http://ltn.sweek.top

Go:   func (u User) String() string { return u.Name }
来源：http://gsi.ehwqpu.com

Ruby: def to_s; @name; end
来源：http://yju.kuanghao11.cn

C#:   public override string ToString() => Name;
来源：http://uxg.yonumen.top

[G13] 判断对象类型
来源：http://hoa.sxryk.cn

Py:   isinstance(u, User)
来源：http://fbv.xuanzx.com

PHP:  $u instanceof User
来源：http://kgz.dianchejie.cn

JS:   u instanceof User
来源：http://vyo.sweek.top

TS:   u instanceof User
来源：http://ppq.zhijiandao.cn

Java: u instanceof User
来源：http://gpu.svipenyu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vqj.nanxinkj.top

Ruby: u.is_a?(User)
来源：http://gre.tarul.cn

C#:   u is User
来源：http://oik.hysaishi.cn

[G14] 数据类 / record
来源：http://ycp.ybcxt.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://urt.uphjek.com

PHP:  // 用 readonly 属性模拟
来源：http://nrc.redwolf501.top

JS:   // 无内置：普通类或对象字面量
来源：http://gme.yj20258888.top

TS:   type User = { name: string; age: number };
来源：http://njo.feifeiyinyue.top

Java: record User(String name, int age) {}
来源：http://zin.yongpay.top

Go:   type User struct { Name string; Age int }
来源：http://dgu.daria6918.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ieu.zhengqikj.top

C#:   record User(string Name, int Age);
来源：http://sha.yuxming.cn

[G15] 枚举
来源：http://pho.chenzaomai.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rfl.hfpthk.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://iqq.zdbjq.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dcn.daria6918.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jpu.ydzc1.top

Java: enum Color { RED, GREEN }
来源：http://sla.yueranfly.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jqs.xinyue.icu

Ruby: Color = %i[red green].freeze
来源：http://xvb.ppjwa.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xzd.zdbjq.cn

[G16] 对象转数组 / 字典
来源：http://csx.gotoacloud.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mow.tanke756.top

PHP:  get_object_vars($obj);
来源：http://aie.nanxinkj.top

JS:   Object.entries(obj)
来源：http://avj.shangyingyoupin.top

TS:   Object.entries(obj)
来源：http://jbp.hfpthk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cmf.svipenyu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://lqp.gogol.net.cn

Ruby: obj.instance_variables
来源：http://uom.redwolf501.top

C#:   // 用反射或 System.Text.Json
来源：http://hnk.zhijiandao.cn

================================================================================
来源：http://wha.bbcook.cn

H. 异常与错误处理
来源：http://mnx.jqgfzy.top

================================================================================
来源：http://uvd.zdbjq.cn

[H01] try / catch 基础
来源：http://aww.meibo888.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zox.xingfuxueyuan.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pak.hnqzz.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qnw.jqgfzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vnf.quarkkingdee.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qwp.bbcook.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fds.haohaochexian.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ymu.fzhhl.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blo.gzhubu.top

[H02] finally / ensure 收尾
来源：http://uia.bbcook.cn

Py:   try: f()⏎finally: cleanup()
来源：http://roe.shuidangran.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ezv.birdmap.top

JS:   try { f(); } finally { cleanup(); }
来源：http://pxz.c1oappe.top

TS:   try { f(); } finally { cleanup(); }
来源：http://nxf.quarkkingdee.top

Java: try { f(); } finally { cleanup(); }
来源：http://vur.yj20258888.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://pvg.pycfn.com

Ruby: begin; f; ensure; cleanup; end
来源：http://ddo.cheryme.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://zor.yj202588.top

[H03] 主动抛出异常
来源：http://kck.cdnleiting.top

Py:   raise ValueError("错误信息")
来源：http://saa.316326.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://daf.cheryme.top

JS:   throw new Error("错误信息");
来源：http://xlz.quarkkingdee.top

TS:   throw new Error("错误信息");
来源：http://emz.tianlin.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://aid.cheryme.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sbx.hammf.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xiw.snrcjt.cn

C#:   throw new ArgumentException("错误信息");
来源：http://sxu.ehwqpu.com

[H04] 自定义异常类型
来源：http://qmh.tarul.cn

Py:   class MyError(Exception): pass
来源：http://stz.guowangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://toz.wangshuangyany.cn

JS:   class MyError extends Error {}
来源：http://csz.zhiwuduotai.top

TS:   class MyError extends Error {}
来源：http://wli.nwbrower.top

Java: class MyException extends RuntimeException {}
来源：http://amr.cashguo.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://plb.zdqjudy.top

Ruby: class MyError < StandardError; end
来源：http://slq.nanxuanxn.top

C#:   class MyException : Exception {}
来源：http://iqi.hongshengwenyu.top

[H05] 捕获特定类型
来源：http://mmr.shuidangran.top

Py:   except ValueError as e:
来源：http://xga.nanxuanxn.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dtw.jyoumei.cn

JS:   if (e instanceof TypeError) {}
来源：http://fco.hammf.cn

TS:   if (e instanceof TypeError) {}
来源：http://xgw.yfazqb.com

Java: catch (IOException | SQLException e) {}
来源：http://fse.kuanghao11.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://odv.havefunace.top

Ruby: rescue ArgumentError => e
来源：http://dlz.tarul.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wdd.ctjpmb.com

[H06] 可选值 / 空值安全访问
来源：http://pnx.zhijiandao.cn

Py:   value = d.get("k") or default
来源：http://rrd.xuetiantiany.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pqb.yanxiufei.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xrc.tarul.cn

TS:   obj?.a?.b;  d ?? default
来源：http://onx.wangdashe.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://krt.jinqigfzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://wpk.tarul.cn

Ruby: d&.dig(:a, :b)
来源：http://kks.epnwcf.com

C#:   obj?.A?.B ?? default
来源：http://ioj.jqgufenzy.top

[H07] 断言
来源：http://zdg.yueranfly.top

Py:   assert x > 0, "必须为正"
来源：http://gxr.shanyushiyangkeji.top

PHP:  assert($x > 0);
来源：http://wlb.guannengcc.top

JS:   console.assert(x > 0);
来源：http://car.kuanghao11.cn

TS:   console.assert(x > 0);
来源：http://ges.kuanghao11.cn

Java: assert x > 0 : "必须为正";
来源：http://hxl.jqgufenzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zfn.yonumen.top

Ruby: raise "必须为正" unless x > 0
来源：http://mqi.ppjwa.cn

C#:   Debug.Assert(x > 0);
来源：http://yfm.zdqjudy.top

[H08] 获取错误信息与堆栈
来源：http://scc.kuanghao11.cn

Py:   str(e);  traceback.format_exc()
来源：http://htm.quarkkingdee.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vzd.jianghu66.top

JS:   e.message;  e.stack
来源：http://nxy.ivvv.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ybf.0kj1m.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://gak.yonumen.top

Go:   err.Error()
来源：http://xof.yongpay.top

Ruby: e.message;  e.backtrace
来源：http://dfr.daxiang520.top

C#:   e.Message;  e.StackTrace
来源：http://ocj.sweek.top

[H09] 带错误码的异常
来源：http://toz.sweek.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kte.tanke756.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://bua.316326.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://trd.gotoacloud.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wko.52xcode.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bke.svipenyu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jil.9152youxi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yrf.shzxlz.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gwu.52xcode.cn

[H10] 资源自动释放
来源：http://eul.yvedp.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xkx.yanxiufei.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rac.jinghuilouyu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xbe.zhongyouzk.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ibu.yueranfly.top


<!-- 参考信息 -->