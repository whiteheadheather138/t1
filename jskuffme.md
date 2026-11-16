代发 wailian999

Ruby: File.delete("a.txt")
来源：http://qkm.hywenlv.cn

C#:   File.Delete("a.txt");
来源：http://lcv.yuanzhike.top

[F07] 创建目录（含多级）
来源：http://qpy.shanyushiyangtech.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cig.shuidangran.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://eyf.xinyue.icu

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eco.shangyingyoupin.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rtr.chenjidiqi.icu

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zte.hysaishi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zpf.yuanzhike.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://iiz.guannengcc.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kwq.iojbl.cn

[F08] 遍历目录
来源：http://kgp.yangfankeji.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://eqm.hfpthk.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://von.gzhubu.top

JS:   fs.readdirSync("dir")
来源：http://jwf.shanyushiyangkeji.top

TS:   fs.readdirSync("dir")
来源：http://euc.shanyushiyangkeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oxk.316326.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://axh.52xcode.cn

Ruby: Dir.children("dir")
来源：http://yrr.gotoacloud.top

C#:   Directory.GetFiles("dir")
来源：http://mfq.sxryk.cn

[F09] 获取文件大小
来源：http://uuu.sxryk.cn

Py:   os.path.getsize("a.txt")
来源：http://dkh.zhengqikj.top

PHP:  filesize("a.txt");
来源：http://svc.cqqwz.cn

JS:   fs.statSync("a.txt").size
来源：http://fti.aizwys.cn

TS:   fs.statSync("a.txt").size
来源：http://xla.kuanghao11.cn

Java: Files.size(Path.of("a.txt"))
来源：http://aio.pycfn.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dyv.yfazqb.com

Ruby: File.size("a.txt")
来源：http://tfg.hysaishi.cn

C#:   new FileInfo("a.txt").Length
来源：http://zzl.chenlongwang.top

[F10] 取文件扩展名 / 文件名
来源：http://bdy.nwbrower.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://csf.gogol.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ykm.ivvv.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://icu.ybcxt.top

TS:   path.extname("a.txt")
来源：http://hsw.chenzaomai.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://obp.sweek.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ojl.svipenyu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qfx.jyoumei.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lxn.andypj.xyz

[F11] 复制与移动文件
来源：http://ota.yj20258888.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wgs.shuidangran.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ulo.yangfankeji.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gou.jyoumei.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bps.yfazqb.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qia.uphjek.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vzf.zhengqikj.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mae.cqqwz.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yhr.fanxiaobao.xyz

[F12] CSV 读写
来源：http://stv.dashuyun.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://utl.hywenlv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://akm.zdbjq.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hrm.uphjek.com

TS:   // 同上
来源：http://ffm.zhaomingkeji.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wku.zdqjudy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fsm.sxryk.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wre.zhongyouzk.top

C#:   // 无内置：用 CsvHelper 库
来源：http://die.yj20258888.top

================================================================================
来源：http://qpo.hywenlv.cn

G. 面向对象
来源：http://wlb.chenlongwang.top

================================================================================
来源：http://xtr.fengsongda.top

[G01] 定义类
来源：http://ofp.pengpengdd.cyou

Py:   class User: pass
来源：http://bjs.jiagoushi.top

PHP:  class User {}
来源：http://duj.hywenlv.cn

JS:   class User {}
来源：http://vdw.ehwqpu.com

TS:   class User { name: string = ""; }
来源：http://var.wangshuangyany.cn

Java: class User {}
来源：http://ojg.ydzc1.top

Go:   type User struct { Name string }
来源：http://kdg.kuanghao11.cn

Ruby: class User; end
来源：http://yyq.ivvv.top

C#:   class User {}
来源：http://vjx.vqdsnc.cn

[G02] 构造函数
来源：http://wvf.sufxvd.cn

Py:   def __init__(self, name): self.name = name
来源：http://zkp.chenlongwang.top

PHP:  public function __construct(public string $name) {}
来源：http://nbf.guannengcc.top

JS:   constructor(name) { this.name = name; }
来源：http://qfb.hammf.cn

TS:   constructor(public name: string) {}
来源：http://hhh.hnxiangtu.top

Java: User(String name) { this.name = name; }
来源：http://zwn.0kj1m.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wfn.jlsjyb.cn

Ruby: def initialize(name); @name = name; end
来源：http://zxn.sxryk.cn

C#:   public User(string name) { Name = name; }
来源：http://vvr.wangshuangyany.cn

[G03] 实例属性
来源：http://vca.hfpthk.cn

Py:   self.name = "x"
来源：http://tcg.epnwcf.com

PHP:  public string $name = "x";
来源：http://hbp.sufxvd.cn

JS:   this.name = "x";
来源：http://zrz.cqqwz.cn

TS:   name: string = "x";
来源：http://akx.yj20258888.top

Java: private String name;
来源：http://wev.jinqigufen.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zdn.xinyue.icu

Ruby: @name = "x"
来源：http://hky.iojbl.cn

C#:   public string Name { get; set; } = "x";
来源：http://kbl.dashuyun.cn

[G04] 定义方法
来源：http://ujd.yj20258.top

Py:   def greet(self): return self.name
来源：http://azd.cheryme.top

PHP:  public function greet(): string { return $this->name; }
来源：http://apw.hysaishi.cn

JS:   greet() { return this.name; }
来源：http://xan.cdnleiting.top

TS:   greet(): string { return this.name; }
来源：http://qbg.dashuyun.cn

Java: String greet() { return name; }
来源：http://pss.tian-w.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pjs.zdbjq.cn

Ruby: def greet; @name; end
来源：http://emd.fanxiaobao.xyz

C#:   public string Greet() => Name;
来源：http://fqt.yfazqb.com

[G05] 继承
来源：http://utq.fktsv.cn

Py:   class Admin(User): pass
来源：http://xay.xuanzx.com

PHP:  class Admin extends User {}
来源：http://zmp.zhaomingkeji.xyz

JS:   class Admin extends User {}
来源：http://tcr.zycfv.cn

TS:   class Admin extends User {}
来源：http://xwh.gogol.net.cn

Java: class Admin extends User {}
来源：http://qwo.daria6918.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://czl.zycfv.cn

Ruby: class Admin < User; end
来源：http://mev.snrcjt.cn

C#:   class Admin : User {}
来源：http://thk.shangyingyoupin.top

[G06] 重写方法
来源：http://qer.xuetiantiany.cn

Py:   def greet(self): return "admin"
来源：http://evg.fengsongda.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ilv.tianlin.xyz

JS:   greet() { return "admin"; }
来源：http://sal.epnwcf.com

TS:   greet(): string { return "admin"; }
来源：http://pku.cashguo.top

Java: @Override String greet() { return "admin"; }
来源：http://npt.xuanzx.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ikt.fanxiaobao.xyz

Ruby: def greet; "admin"; end
来源：http://ogg.daxiang520.top

C#:   public override string Greet() => "admin";
来源：http://ihh.dashuyun.cn

[G07] 调用父类方法
来源：http://wpf.jinqigfzy.top

Py:   super().greet()
来源：http://vdp.zhixingplan.top

PHP:  parent::greet();
来源：http://ely.xuetiantiany.cn

JS:   super.greet();
来源：http://adb.yueranfly.top

TS:   super.greet();
来源：http://vst.sufxvd.cn

Java: super.greet();
来源：http://esh.cheryme.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bfh.hesvh.cn

Ruby: super
来源：http://ypz.yonumen.top

C#:   base.Greet();
来源：http://wnc.sysykeji.top

[G08] 静态方法与属性
来源：http://tcc.haohaochexian.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hld.shanyushiyangkeji.top

PHP:  public static function f() {}
来源：http://fxu.xuanzx.com

JS:   static f() {}
来源：http://etq.dashuyun.cn

TS:   static f(): void {}
来源：http://nly.zhongyouzk.top

Java: static void f() {}
来源：http://pct.zhoulong.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://etr.hongshengwenyu.top

Ruby: def self.f; end
来源：http://xjz.zhoulong.xyz

C#:   public static void F() {}
来源：http://oea.bbcook.cn

[G09] 接口 / 抽象类
来源：http://ftd.chenzaomai.com

Py:   from abc import ABC, abstractmethod
来源：http://fmh.9152youxi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wph.yj20258.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://suw.zycfv.cn

TS:   interface Shape { area(): number; }
来源：http://nln.wangshuangyany.cn

Java: interface Shape { double area(); }
来源：http://bdt.zdqjudy.top

Go:   type Shape interface { Area() float64 }
来源：http://qsd.sufxvd.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ypl.nwbrower.top

C#:   interface IShape { double Area(); }
来源：http://xyu.dianchejie.cn

[G10] 访问控制
来源：http://ttv.vqdsnc.cn

Py:   约定 _protected / __private（不强制）
来源：http://hhe.jqgufenzy.top

PHP:  public / protected / private
来源：http://lgg.fengsongda.top

JS:   #private 字段；其余公开
来源：http://yyh.ydzc1.top

TS:   public / protected / private
来源：http://kiw.hnxiangtu.top

Java: public / protected / private / 默认包级
来源：http://udy.fktsv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://usy.jqgfzy.top

Ruby: public / protected / private
来源：http://kai.cheryme.top

C#:   public / protected / private / internal
来源：http://cdh.svipenyu.cn

[G11] getter / setter
来源：http://mpr.uphjek.com

Py:   @property 与 @x.setter
来源：http://nii.fengsongda.top

PHP:  public function getName(): string { return $this->name; }
来源：http://xfo.jinqigufen.top

JS:   get name() { return this._name; }
来源：http://gmn.ctjpmb.com

TS:   get name(): string { return this._name; }
来源：http://kva.feifeiyinyue.top

Java: public String getName() { return name; }
来源：http://mtl.sufxvd.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://eyt.fzhhl.top

Ruby: attr_accessor :name
来源：http://uhi.wangshuangyany.cn

C#:   public string Name { get; set; }
来源：http://ich.fzhhl.top

[G12] 对象转字符串
来源：http://six.jinqigfzy.top

Py:   def __str__(self): return self.name
来源：http://gqs.hnxiangtu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://qoa.jqgufenzy.top

JS:   toString() { return this.name; }
来源：http://aia.nanxuanxn.top

TS:   toString(): string { return this.name; }
来源：http://dpb.316326.xyz

Java: @Override public String toString() { return name; }
来源：http://nya.gotoacloud.top

Go:   func (u User) String() string { return u.Name }
来源：http://buk.jlsjyb.cn

Ruby: def to_s; @name; end
来源：http://woo.sweek.top

C#:   public override string ToString() => Name;
来源：http://dco.svipenyu.cn

[G13] 判断对象类型
来源：http://yca.ywan-chungtsiang.top

Py:   isinstance(u, User)
来源：http://lwd.zhengqikj.top

PHP:  $u instanceof User
来源：http://omv.hfpthk.cn

JS:   u instanceof User
来源：http://iwz.xuetiantiany.cn

TS:   u instanceof User
来源：http://sdx.cashguo.top

Java: u instanceof User
来源：http://cpa.yvedp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ggb.sufxvd.cn

Ruby: u.is_a?(User)
来源：http://nwa.hywenlv.cn

C#:   u is User
来源：http://stw.sysykeji.top

[G14] 数据类 / record
来源：http://aro.snrcjt.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ext.snrcjt.cn

PHP:  // 用 readonly 属性模拟
来源：http://fiy.haohaochexian.top

JS:   // 无内置：普通类或对象字面量
来源：http://cid.gaohongyu789.top

TS:   type User = { name: string; age: number };
来源：http://kgi.redwolf501.top

Java: record User(String name, int age) {}
来源：http://nqo.sysykeji.top

Go:   type User struct { Name string; Age int }
来源：http://eob.yvedp.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qdj.wangshuangyany.cn

C#:   record User(string Name, int Age);
来源：http://mri.zhaomingkeji.xyz

[G15] 枚举
来源：http://kvy.bjfxy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pwo.yj202588.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://gst.jqgufenzy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kfh.nwbrower.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bov.vehdjk.com

Java: enum Color { RED, GREEN }
来源：http://qsp.nanxuanxn.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fex.yj202588.top

Ruby: Color = %i[red green].freeze
来源：http://nmi.yj20258888.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jqa.xingfuxueyuan.xyz

[G16] 对象转数组 / 字典
来源：http://xcr.yangfankeji.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jlv.quarkkingdee.top

PHP:  get_object_vars($obj);
来源：http://itk.dianchejie.cn

JS:   Object.entries(obj)
来源：http://umz.nanxinkj.top

TS:   Object.entries(obj)
来源：http://uli.jianghu66.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cie.vqdsnc.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wql.snrcjt.cn

Ruby: obj.instance_variables
来源：http://hfh.gaohongyu789.top

C#:   // 用反射或 System.Text.Json
来源：http://iix.quarkkingdee.top

================================================================================
来源：http://rmm.gotoacloud.top

H. 异常与错误处理
来源：http://nxw.jinyuanbaomall.cn

================================================================================
来源：http://lxy.shanyushiyangkeji.top

[H01] try / catch 基础
来源：http://mty.chenzaomai.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fgq.sweek.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vrc.9152youxi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fke.bbcook.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sdq.pycfn.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wzb.gzhubu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jtk.andypj.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cic.chenlongwang.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sfu.haohaochexian.top

[H02] finally / ensure 收尾
来源：http://lxd.nwbrower.top

Py:   try: f()⏎finally: cleanup()
来源：http://nxd.hongshengwenyu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://fgi.havefunace.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ylm.iojbl.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gxy.hnqzz.top

Java: try { f(); } finally { cleanup(); }
来源：http://qzc.chenlongwang.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://osq.sxryk.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bob.ywan-chungtsiang.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://gja.zycfv.cn

[H03] 主动抛出异常
来源：http://wtw.yangfankeji.com

Py:   raise ValueError("错误信息")
来源：http://xge.zdqjudy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vkw.quarkkingdee.top

JS:   throw new Error("错误信息");
来源：http://vhg.gotoacloud.top

TS:   throw new Error("错误信息");
来源：http://nnx.jinqigfzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://wsk.fzhhl.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://msn.yanxiufei.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fws.quarkkingdee.top

C#:   throw new ArgumentException("错误信息");
来源：http://hcn.hywenlv.cn

[H04] 自定义异常类型
来源：http://utv.yonumen.top

Py:   class MyError(Exception): pass
来源：http://oui.svipenyu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wvb.shangyingyoupin.top

JS:   class MyError extends Error {}
来源：http://tut.gzhubu.top

TS:   class MyError extends Error {}
来源：http://szw.yj20258.top

Java: class MyException extends RuntimeException {}
来源：http://igl.ybcxt.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ooh.yj20258.top

Ruby: class MyError < StandardError; end
来源：http://xav.nanxinkj.top

C#:   class MyException : Exception {}
来源：http://lsy.hfpthk.cn

[H05] 捕获特定类型
来源：http://zel.tarul.cn

Py:   except ValueError as e:
来源：http://qta.jiagoushi.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cip.ywan-chungtsiang.top

JS:   if (e instanceof TypeError) {}
来源：http://ijx.hongshengwenyu.top

TS:   if (e instanceof TypeError) {}
来源：http://jbf.xylfe.cn

Java: catch (IOException | SQLException e) {}
来源：http://yki.dashuyun.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dvr.svipenyu.cn

Ruby: rescue ArgumentError => e
来源：http://ddd.hnxiangtu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ioy.ctjpmb.com

[H06] 可选值 / 空值安全访问
来源：http://fep.ybcxt.top

Py:   value = d.get("k") or default
来源：http://tco.smart0.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://ffv.jianghu66.top

JS:   obj?.a?.b;  d ?? default
来源：http://ynk.xuetiantiany.cn

TS:   obj?.a?.b;  d ?? default
来源：http://akm.smart0.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pvf.ehwqpu.com

Go:   if v, ok := m["k"]; ok { }
来源：http://tna.xylfe.cn

Ruby: d&.dig(:a, :b)
来源：http://hox.zhoulong.xyz

C#:   obj?.A?.B ?? default
来源：http://ddz.hnqzz.top

[H07] 断言
来源：http://tyt.epnwcf.com

Py:   assert x > 0, "必须为正"
来源：http://rqc.jianghu66.top

PHP:  assert($x > 0);
来源：http://hmh.vqdsnc.cn

JS:   console.assert(x > 0);
来源：http://otc.epnwcf.com

TS:   console.assert(x > 0);
来源：http://iwm.yanxiufei.cn

Java: assert x > 0 : "必须为正";
来源：http://sid.ydjk.org.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dzd.bjfxy.top

Ruby: raise "必须为正" unless x > 0
来源：http://xoo.shuidangran.top

C#:   Debug.Assert(x > 0);
来源：http://rvw.zhiwuduotai.top

[H08] 获取错误信息与堆栈
来源：http://gud.uphjek.com

Py:   str(e);  traceback.format_exc()
来源：http://sme.ctjpmb.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qee.redwolf501.top

JS:   e.message;  e.stack
来源：http://upb.cheryme.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://jph.sxryk.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cva.yuanzhike.top

Go:   err.Error()
来源：http://tmf.mhx1999.top

Ruby: e.message;  e.backtrace
来源：http://fco.aizwys.cn

C#:   e.Message;  e.StackTrace
来源：http://xqt.ywan-chungtsiang.top

[H09] 带错误码的异常
来源：http://ypa.jinqigufen.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rkx.svipenyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xjn.jiagoushi.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ecd.hesvh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rbu.shanyushiyangtech.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yav.feifeiyinyue.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lpl.shuidangran.top

Ruby: raise MyError.new("fail", 500)
来源：http://svw.jinqigfzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://jjk.yfazqb.com

[H10] 资源自动释放
来源：http://ccu.andypj.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://efv.0kj1m.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sll.chenzaomai.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mfj.fehbvm.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lty.fktsv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ief.tanke756.top

Go:   defer f.Close()
来源：http://ihe.redwolf501.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lmd.52xcode.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tit.fanxiaobao.xyz

================================================================================
来源：http://zuo.ydjk.org.cn

I. 正则表达式
来源：http://qvq.redwolf501.top

================================================================================
来源：http://qaj.sxryk.cn

[I01] 判断是否匹配
来源：http://ygk.xingfuxueyuan.xyz


<!-- 参考信息 -->