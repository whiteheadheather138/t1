代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dfk.fehbvm.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yqd.ivvv.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://meg.havefunace.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fum.fanxiaobao.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yrd.yueranfly.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://igw.dashuyun.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pse.redwolf501.top

[F08] 遍历目录
来源：http://gqu.shzxlz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://hyn.guannengcc.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kvj.yvedp.cn

JS:   fs.readdirSync("dir")
来源：http://vau.fengsongda.top

TS:   fs.readdirSync("dir")
来源：http://ozc.bjfxy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qpp.sxryk.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zwd.shzxlz.cn

Ruby: Dir.children("dir")
来源：http://tvt.jinghuilouyu.cn

C#:   Directory.GetFiles("dir")
来源：http://wtv.andypj.xyz

[F09] 获取文件大小
来源：http://voi.kuanghao11.cn

Py:   os.path.getsize("a.txt")
来源：http://plc.tarul.cn

PHP:  filesize("a.txt");
来源：http://jdp.nanxuanxn.top

JS:   fs.statSync("a.txt").size
来源：http://gtp.mhx1999.top

TS:   fs.statSync("a.txt").size
来源：http://rdn.zhixingplan.top

Java: Files.size(Path.of("a.txt"))
来源：http://pvm.pycfn.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ztw.ydzc1.top

Ruby: File.size("a.txt")
来源：http://uxo.ehwqpu.com

C#:   new FileInfo("a.txt").Length
来源：http://nbd.yuanzhike.top

[F10] 取文件扩展名 / 文件名
来源：http://hca.hfpthk.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pno.9152youxi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gvp.yuanzhike.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vfo.jinqigufen.top

TS:   path.extname("a.txt")
来源：http://igl.meibo888.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rqi.tarul.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wij.shanyushiyangtech.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sfz.yj20258888.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wkz.ywan-chungtsiang.top

[F11] 复制与移动文件
来源：http://xql.gogol.net.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tmy.cdnleiting.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hlw.chenjidiqi.icu

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ooe.daxiang520.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fzc.quarkkingdee.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kts.zhengqikj.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://evn.haohaochexian.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jmg.ehwqpu.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qlm.wangshuangyany.cn

[F12] CSV 读写
来源：http://kin.cqqwz.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://euc.gotoacloud.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://urd.nanxinkj.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cib.quarkkingdee.top

TS:   // 同上
来源：http://zin.gaohongyu789.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qgx.jlsjyb.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sjv.yj20258888.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://znb.jyoumei.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tqh.ywan-chungtsiang.top

================================================================================
来源：http://hyc.sysykeji.top

G. 面向对象
来源：http://dvn.xylfe.cn

================================================================================
来源：http://jom.shanyushiyangkeji.top

[G01] 定义类
来源：http://rlt.vqdsnc.cn

Py:   class User: pass
来源：http://vdn.chenlongwang.top

PHP:  class User {}
来源：http://cfq.zhongyouzk.top

JS:   class User {}
来源：http://vxt.redwolf501.top

TS:   class User { name: string = ""; }
来源：http://xmx.redwolf501.top

Java: class User {}
来源：http://hpf.316326.xyz

Go:   type User struct { Name string }
来源：http://qpt.hnqzz.top

Ruby: class User; end
来源：http://jtw.yanxiufei.cn

C#:   class User {}
来源：http://rcn.iojbl.cn

[G02] 构造函数
来源：http://iqj.shanyushiyangtech.top

Py:   def __init__(self, name): self.name = name
来源：http://exe.zhengqikj.top

PHP:  public function __construct(public string $name) {}
来源：http://ddf.bjfxy.top

JS:   constructor(name) { this.name = name; }
来源：http://ugl.sjlbkw.cn

TS:   constructor(public name: string) {}
来源：http://fbp.zycfv.cn

Java: User(String name) { this.name = name; }
来源：http://owu.redwolf501.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://iqg.guowangkeji.top

Ruby: def initialize(name); @name = name; end
来源：http://gni.wangshuangyany.cn

C#:   public User(string name) { Name = name; }
来源：http://yrn.hammf.cn

[G03] 实例属性
来源：http://evt.hcnkem.com

Py:   self.name = "x"
来源：http://enh.jianghu66.top

PHP:  public string $name = "x";
来源：http://veg.smart0.xyz

JS:   this.name = "x";
来源：http://zqe.smart0.xyz

TS:   name: string = "x";
来源：http://nsf.wangshuangyany.cn

Java: private String name;
来源：http://fza.yj202588.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cuu.jqgufenzy.top

Ruby: @name = "x"
来源：http://jfv.52xcode.cn

C#:   public string Name { get; set; } = "x";
来源：http://jpm.gaohongyu789.top

[G04] 定义方法
来源：http://azq.hywenlv.cn

Py:   def greet(self): return self.name
来源：http://dkc.iojbl.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://cwo.ybcxt.top

JS:   greet() { return this.name; }
来源：http://gao.zhijiandao.cn

TS:   greet(): string { return this.name; }
来源：http://hpq.hongshengwenyu.top

Java: String greet() { return name; }
来源：http://ily.bjfxy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://sld.yj20258.top

Ruby: def greet; @name; end
来源：http://cue.bbcook.cn

C#:   public string Greet() => Name;
来源：http://ebd.hysaishi.cn

[G05] 继承
来源：http://zio.yvedp.cn

Py:   class Admin(User): pass
来源：http://gho.hcnkem.com

PHP:  class Admin extends User {}
来源：http://aym.wangdashe.top

JS:   class Admin extends User {}
来源：http://dmg.tanke756.top

TS:   class Admin extends User {}
来源：http://smk.ctjpmb.com

Java: class Admin extends User {}
来源：http://hvj.xingfuxueyuan.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ett.guowangkeji.top

Ruby: class Admin < User; end
来源：http://yyb.xinyue.icu

C#:   class Admin : User {}
来源：http://fed.hammf.cn

[G06] 重写方法
来源：http://fzr.guannengcc.top

Py:   def greet(self): return "admin"
来源：http://rip.vehdjk.com

PHP:  public function greet(): string { return "admin"; }
来源：http://hig.sysykeji.top

JS:   greet() { return "admin"; }
来源：http://esr.cqqwz.cn

TS:   greet(): string { return "admin"; }
来源：http://cmw.zhiwuduotai.top

Java: @Override String greet() { return "admin"; }
来源：http://vfc.yj20258888.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wew.ehwqpu.com

Ruby: def greet; "admin"; end
来源：http://qre.quarkkingdee.top

C#:   public override string Greet() => "admin";
来源：http://jwn.nwbrower.top

[G07] 调用父类方法
来源：http://yug.xinyue.icu

Py:   super().greet()
来源：http://zhv.jinyuanbaomall.cn

PHP:  parent::greet();
来源：http://ntt.chenjidiqi.icu

JS:   super.greet();
来源：http://vtg.xingfuxueyuan.xyz

TS:   super.greet();
来源：http://rhp.daxiang520.top

Java: super.greet();
来源：http://eaj.guannengcc.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ogm.hywenlv.cn

Ruby: super
来源：http://hjr.yfazqb.com

C#:   base.Greet();
来源：http://nfu.quarkkingdee.top

[G08] 静态方法与属性
来源：http://qew.sjlbkw.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://aiu.zdbjq.cn

PHP:  public static function f() {}
来源：http://vfh.shuidangran.top

JS:   static f() {}
来源：http://jzj.fehbvm.com

TS:   static f(): void {}
来源：http://ehe.meibo888.top

Java: static void f() {}
来源：http://qtt.daxiang520.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://agw.yonumen.top

Ruby: def self.f; end
来源：http://vwp.c1oappe.top

C#:   public static void F() {}
来源：http://wqt.jiagoushi.top

[G09] 接口 / 抽象类
来源：http://fqc.kuanghao11.cn

Py:   from abc import ABC, abstractmethod
来源：http://hqq.tian-w.cn

PHP:  interface Shape { public function area(): float; }
来源：http://svd.zhongyouzk.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://aeu.zhiwuduotai.top

TS:   interface Shape { area(): number; }
来源：http://qtk.jqgufenzy.top

Java: interface Shape { double area(); }
来源：http://byb.yfazqb.com

Go:   type Shape interface { Area() float64 }
来源：http://xkv.9152youxi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qig.gaohongyu789.top

C#:   interface IShape { double Area(); }
来源：http://xph.yj202588.top

[G10] 访问控制
来源：http://lvd.jianghu66.top

Py:   约定 _protected / __private（不强制）
来源：http://mqi.xuetiantiany.cn

PHP:  public / protected / private
来源：http://qee.meibo888.top

JS:   #private 字段；其余公开
来源：http://kes.dashuyun.cn

TS:   public / protected / private
来源：http://iek.sxryk.cn

Java: public / protected / private / 默认包级
来源：http://uxl.52xcode.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dzs.daxiang520.top

Ruby: public / protected / private
来源：http://ywm.yfazqb.com

C#:   public / protected / private / internal
来源：http://cde.ybcxt.top

[G11] getter / setter
来源：http://nrj.shanyushiyangkeji.top

Py:   @property 与 @x.setter
来源：http://zok.sjlbkw.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mny.birdmap.top

JS:   get name() { return this._name; }
来源：http://bpr.pycfn.com

TS:   get name(): string { return this._name; }
来源：http://bwp.yongpay.top

Java: public String getName() { return name; }
来源：http://sob.sufxvd.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qbs.316326.xyz

Ruby: attr_accessor :name
来源：http://zon.shanyushiyangtech.top

C#:   public string Name { get; set; }
来源：http://qai.hnqzz.top

[G12] 对象转字符串
来源：http://hgw.ppjwa.cn

Py:   def __str__(self): return self.name
来源：http://rai.daxiang520.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://aoy.epnwcf.com

JS:   toString() { return this.name; }
来源：http://tfc.svipenyu.cn

TS:   toString(): string { return this.name; }
来源：http://ijv.chenlongwang.top

Java: @Override public String toString() { return name; }
来源：http://jma.xuetiantiany.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fro.guannengcc.top

Ruby: def to_s; @name; end
来源：http://ocq.svipenyu.cn

C#:   public override string ToString() => Name;
来源：http://xzg.jqgfzy.top

[G13] 判断对象类型
来源：http://yyd.chenzaomai.com

Py:   isinstance(u, User)
来源：http://pyu.jyoumei.cn

PHP:  $u instanceof User
来源：http://tpq.meibo888.top

JS:   u instanceof User
来源：http://elo.nwbrower.top

TS:   u instanceof User
来源：http://bie.smart0.xyz

Java: u instanceof User
来源：http://tob.yfazqb.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://imj.xylfe.cn

Ruby: u.is_a?(User)
来源：http://cjs.hongshengwenyu.top

C#:   u is User
来源：http://dzr.tanke756.top

[G14] 数据类 / record
来源：http://yeb.xziqi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://add.jqgufenzy.top

PHP:  // 用 readonly 属性模拟
来源：http://zpr.bjfxy.top

JS:   // 无内置：普通类或对象字面量
来源：http://vtz.hcnkem.com

TS:   type User = { name: string; age: number };
来源：http://wyg.jinqigufen.top

Java: record User(String name, int age) {}
来源：http://kdt.yvedp.cn

Go:   type User struct { Name string; Age int }
来源：http://bzn.jianghu66.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bvq.jinyuanbaomall.cn

C#:   record User(string Name, int Age);
来源：http://vps.guannengcc.top

[G15] 枚举
来源：http://dfu.hnxiangtu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qqx.svipenyu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pqw.zhoulong.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zra.nanxinkj.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vvr.gaohongyu789.top

Java: enum Color { RED, GREEN }
来源：http://grs.sxryk.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vjk.cheryme.top

Ruby: Color = %i[red green].freeze
来源：http://moy.guannengcc.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hia.redwolf501.top

[G16] 对象转数组 / 字典
来源：http://rwe.yuxming.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pwc.hesvh.cn

PHP:  get_object_vars($obj);
来源：http://imv.sweek.top

JS:   Object.entries(obj)
来源：http://olc.jqgufenzy.top

TS:   Object.entries(obj)
来源：http://zyb.yuanzhike.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://usj.haohaochexian.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://xfi.sjlbkw.cn

Ruby: obj.instance_variables
来源：http://tlx.jqgufenzy.top

C#:   // 用反射或 System.Text.Json
来源：http://msj.xuetiantiany.cn

================================================================================
来源：http://weg.nanxinkj.top

H. 异常与错误处理
来源：http://evb.yonumen.top

================================================================================
来源：http://gct.meibo888.top

[H01] try / catch 基础
来源：http://uja.bbcook.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://quy.zhixingplan.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kvh.yuxming.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jby.cqqwz.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rkl.fzhhl.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://weo.yongpay.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jex.vehdjk.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dff.ybcxt.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pxl.fengsongda.top

[H02] finally / ensure 收尾
来源：http://gvs.birdmap.top

Py:   try: f()⏎finally: cleanup()
来源：http://mnm.tianlin.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://ubj.shanyushiyangtech.top

JS:   try { f(); } finally { cleanup(); }
来源：http://pvh.yuxming.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mut.chenzaomai.com

Java: try { f(); } finally { cleanup(); }
来源：http://igb.zhongyouzk.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://lbt.aibaodan.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://cys.uphjek.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://mti.daria6918.cn

[H03] 主动抛出异常
来源：http://wob.316326.xyz

Py:   raise ValueError("错误信息")
来源：http://roz.ctjpmb.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://psb.ppjwa.cn

JS:   throw new Error("错误信息");
来源：http://fxj.jinqigufen.top

TS:   throw new Error("错误信息");
来源：http://dqi.nwbrower.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://sqi.zhoulong.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qpw.yuxming.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://rzi.jinqigufen.top

C#:   throw new ArgumentException("错误信息");
来源：http://ylx.zhixingplan.top

[H04] 自定义异常类型
来源：http://bea.shzxlz.cn

Py:   class MyError(Exception): pass
来源：http://gei.vqdsnc.cn

PHP:  class MyError extends RuntimeException {}
来源：http://kdl.svipenyu.cn

JS:   class MyError extends Error {}
来源：http://xld.gotoacloud.top

TS:   class MyError extends Error {}
来源：http://vyx.jiagoushi.top

Java: class MyException extends RuntimeException {}
来源：http://rvn.tanke756.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hdu.uphjek.com

Ruby: class MyError < StandardError; end
来源：http://gng.quarkkingdee.top

C#:   class MyException : Exception {}
来源：http://fmd.yfazqb.com

[H05] 捕获特定类型
来源：http://dpa.hcnkem.com

Py:   except ValueError as e:
来源：http://kdh.sweek.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cod.ctjpmb.com

JS:   if (e instanceof TypeError) {}
来源：http://mky.ybcxt.top

TS:   if (e instanceof TypeError) {}
来源：http://ywm.dashuyun.cn

Java: catch (IOException | SQLException e) {}
来源：http://xfd.yj20258888.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kww.jlsjyb.cn

Ruby: rescue ArgumentError => e
来源：http://oem.kuanghao11.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ndc.birdmap.top

[H06] 可选值 / 空值安全访问
来源：http://pia.zhixingplan.top

Py:   value = d.get("k") or default
来源：http://rie.gaohongyu789.top

PHP:  $v = $d["k"] ?? null;
来源：http://dpz.sjlbkw.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ekx.yueranfly.top

TS:   obj?.a?.b;  d ?? default
来源：http://rkt.nanxinkj.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ewd.wangdashe.top

Go:   if v, ok := m["k"]; ok { }
来源：http://vhx.yj20258.top

Ruby: d&.dig(:a, :b)
来源：http://bbb.uphjek.com

C#:   obj?.A?.B ?? default
来源：http://lre.hywenlv.cn

[H07] 断言
来源：http://zlx.tarul.cn

Py:   assert x > 0, "必须为正"
来源：http://jud.zhongyouzk.top

PHP:  assert($x > 0);
来源：http://ptl.jianghu66.top

JS:   console.assert(x > 0);
来源：http://pav.shuidangran.top

TS:   console.assert(x > 0);
来源：http://dhc.yangfankeji.com

Java: assert x > 0 : "必须为正";
来源：http://ykw.zhoulong.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ynt.gaohongyu789.top

Ruby: raise "必须为正" unless x > 0
来源：http://pnl.meibo888.top

C#:   Debug.Assert(x > 0);
来源：http://plo.ehwqpu.com

[H08] 获取错误信息与堆栈
来源：http://plj.ppjwa.cn

Py:   str(e);  traceback.format_exc()
来源：http://bls.sweek.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hzw.vehdjk.com

JS:   e.message;  e.stack
来源：http://fna.cheryme.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://alj.0kj1m.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nom.xingfuxueyuan.xyz

Go:   err.Error()
来源：http://ljd.hywenlv.cn

Ruby: e.message;  e.backtrace
来源：http://fej.gaohongyu789.top

C#:   e.Message;  e.StackTrace
来源：http://ajo.sweek.top

[H09] 带错误码的异常
来源：http://fph.quarkkingdee.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pks.daxiang520.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://jbd.smart0.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hyy.ivvv.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://olm.gaohongyu789.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ale.mhx1999.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://eia.shzxlz.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bkr.zdbjq.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mfj.meibo888.top

[H10] 资源自动释放
来源：http://dsp.fktsv.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.dashuyun.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rxg.yongpay.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://seg.haohaochexian.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qqk.yfazqb.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lsn.svipenyu.cn

Go:   defer f.Close()
来源：http://maw.dianchejie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jax.jinghuilouyu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nem.jlsjyb.cn

================================================================================
来源：http://qnv.fanxiaobao.xyz

I. 正则表达式
来源：http://uuo.xuanzx.com

================================================================================
来源：http://urb.ydjk.org.cn

[I01] 判断是否匹配
来源：http://uvt.bbcook.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lgp.yuxming.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hvt.nwbrower.top

JS:   /\d+/.test(s)
来源：http://gnb.dashuyun.cn

TS:   /\d+/.test(s)
来源：http://wrx.jqgfzy.top


<!-- 参考信息 -->