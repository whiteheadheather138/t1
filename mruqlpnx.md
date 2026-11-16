代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gmj.zycfv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gnk.xuanzx.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pgl.xuetiantiany.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ctp.daria6918.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nfv.316326.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://drj.wangdashe.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qrq.redwolf501.top

[F08] 遍历目录
来源：http://fdf.yfazqb.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://yev.feifeiyinyue.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sgl.guannengcc.top

JS:   fs.readdirSync("dir")
来源：http://hyi.meibo888.top

TS:   fs.readdirSync("dir")
来源：http://exy.jqgufenzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ilj.yonumen.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://qmz.xinyue.icu

Ruby: Dir.children("dir")
来源：http://dre.zhiwuduotai.top

C#:   Directory.GetFiles("dir")
来源：http://iyp.wangdashe.top

[F09] 获取文件大小
来源：http://xaj.zhiwuduotai.top

Py:   os.path.getsize("a.txt")
来源：http://opp.smart0.xyz

PHP:  filesize("a.txt");
来源：http://lnz.havefunace.top

JS:   fs.statSync("a.txt").size
来源：http://kev.tian-w.cn

TS:   fs.statSync("a.txt").size
来源：http://chk.zhaomingkeji.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://hqz.ehwqpu.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wnu.bbcook.cn

Ruby: File.size("a.txt")
来源：http://rit.cdnleiting.top

C#:   new FileInfo("a.txt").Length
来源：http://ckc.52xcode.cn

[F10] 取文件扩展名 / 文件名
来源：http://kiy.gaohongyu789.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ubq.yfazqb.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xge.jianghu66.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://apq.gotoacloud.top

TS:   path.extname("a.txt")
来源：http://ffw.vehdjk.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pxj.xuanzx.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://olu.cdnleiting.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cdr.hysaishi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bqd.chenjidiqi.icu

[F11] 复制与移动文件
来源：http://caq.guannengcc.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mho.wangdashe.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wjz.yj20258.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kmk.hcnkem.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bpo.nanxuanxn.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://maf.daxiang520.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ptk.cucudq.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://agh.snrcjt.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jum.feifeiyinyue.top

[F12] CSV 读写
来源：http://htc.ehwqpu.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://iov.ywan-chungtsiang.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dtu.ppjwa.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://llw.meibo888.top

TS:   // 同上
来源：http://rcg.jqgufenzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ysn.52xcode.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lyz.hesvh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pml.cucudq.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://axo.smart0.xyz

================================================================================
来源：http://njo.xziqi.cn

G. 面向对象
来源：http://xtx.xuanzx.com

================================================================================
来源：http://lca.xuetiantiany.cn

[G01] 定义类
来源：http://yeq.uphjek.com

Py:   class User: pass
来源：http://qrj.yanxiufei.cn

PHP:  class User {}
来源：http://eey.guowangkeji.top

JS:   class User {}
来源：http://bll.daria6918.cn

TS:   class User { name: string = ""; }
来源：http://jfg.yuxming.cn

Java: class User {}
来源：http://gis.cucudq.cn

Go:   type User struct { Name string }
来源：http://enl.fengsongda.top

Ruby: class User; end
来源：http://ueq.cqqwz.cn

C#:   class User {}
来源：http://ttw.yj202588.top

[G02] 构造函数
来源：http://gpq.sweek.top

Py:   def __init__(self, name): self.name = name
来源：http://ktp.nwbrower.top

PHP:  public function __construct(public string $name) {}
来源：http://rlf.sysykeji.top

JS:   constructor(name) { this.name = name; }
来源：http://fkx.0kj1m.cn

TS:   constructor(public name: string) {}
来源：http://npd.xingfuxueyuan.xyz

Java: User(String name) { this.name = name; }
来源：http://erv.shangyingyoupin.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://owp.dianchejie.cn

Ruby: def initialize(name); @name = name; end
来源：http://upi.zhixingplan.top

C#:   public User(string name) { Name = name; }
来源：http://xzk.nanxuanxn.top

[G03] 实例属性
来源：http://thi.zhengqikj.top

Py:   self.name = "x"
来源：http://ahz.tanke756.top

PHP:  public string $name = "x";
来源：http://ybo.chenzaomai.com

JS:   this.name = "x";
来源：http://ejm.iojbl.cn

TS:   name: string = "x";
来源：http://hkz.cashguo.top

Java: private String name;
来源：http://ffw.smart0.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://trk.ybcxt.top

Ruby: @name = "x"
来源：http://zfs.epnwcf.com

C#:   public string Name { get; set; } = "x";
来源：http://lny.hnqzz.top

[G04] 定义方法
来源：http://zvv.tianlin.xyz

Py:   def greet(self): return self.name
来源：http://whv.cdnleiting.top

PHP:  public function greet(): string { return $this->name; }
来源：http://mpx.zhiwuduotai.top

JS:   greet() { return this.name; }
来源：http://bgb.zhoulong.xyz

TS:   greet(): string { return this.name; }
来源：http://amc.guannengcc.top

Java: String greet() { return name; }
来源：http://udd.iojbl.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://anp.chenlongwang.top

Ruby: def greet; @name; end
来源：http://bqq.redwolf501.top

C#:   public string Greet() => Name;
来源：http://qil.chenlongwang.top

[G05] 继承
来源：http://hoy.redwolf501.top

Py:   class Admin(User): pass
来源：http://lao.zhixingplan.top

PHP:  class Admin extends User {}
来源：http://nzf.kuanghao11.cn

JS:   class Admin extends User {}
来源：http://jac.fengsongda.top

TS:   class Admin extends User {}
来源：http://whn.uphjek.com

Java: class Admin extends User {}
来源：http://shu.jqgufenzy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lhe.yonumen.top

Ruby: class Admin < User; end
来源：http://kzl.shanyushiyangtech.top

C#:   class Admin : User {}
来源：http://trf.smart0.xyz

[G06] 重写方法
来源：http://ura.jianghu66.top

Py:   def greet(self): return "admin"
来源：http://uwj.sysykeji.top

PHP:  public function greet(): string { return "admin"; }
来源：http://hkc.sufxvd.cn

JS:   greet() { return "admin"; }
来源：http://umg.aibaodan.cn

TS:   greet(): string { return "admin"; }
来源：http://phj.feifeiyinyue.top

Java: @Override String greet() { return "admin"; }
来源：http://eha.shzxlz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zly.guannengcc.top

Ruby: def greet; "admin"; end
来源：http://vug.shzxlz.cn

C#:   public override string Greet() => "admin";
来源：http://sxe.hfpthk.cn

[G07] 调用父类方法
来源：http://okb.zdqjudy.top

Py:   super().greet()
来源：http://bgb.ivvv.top

PHP:  parent::greet();
来源：http://ckv.ivvv.top

JS:   super.greet();
来源：http://ftd.sysykeji.top

TS:   super.greet();
来源：http://gom.sweek.top

Java: super.greet();
来源：http://hfd.zhengqikj.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sji.zhengqikj.top

Ruby: super
来源：http://ikr.snrcjt.cn

C#:   base.Greet();
来源：http://qqv.vehdjk.com

[G08] 静态方法与属性
来源：http://npn.cqqwz.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mzz.sufxvd.cn

PHP:  public static function f() {}
来源：http://nfh.quarkkingdee.top

JS:   static f() {}
来源：http://swh.cdnleiting.top

TS:   static f(): void {}
来源：http://qey.nanxuanxn.top

Java: static void f() {}
来源：http://ldr.yj202588.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://sny.zhijiandao.cn

Ruby: def self.f; end
来源：http://ahm.zhixingplan.top

C#:   public static void F() {}
来源：http://yec.fktsv.cn

[G09] 接口 / 抽象类
来源：http://uhw.wangshuangyany.cn

Py:   from abc import ABC, abstractmethod
来源：http://kga.c1oappe.top

PHP:  interface Shape { public function area(): float; }
来源：http://xdc.jinyuanbaomall.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ijv.yj20258.top

TS:   interface Shape { area(): number; }
来源：http://prp.yueranfly.top

Java: interface Shape { double area(); }
来源：http://qyh.chenlongwang.top

Go:   type Shape interface { Area() float64 }
来源：http://aby.zdbjq.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://axo.zhaomingkeji.xyz

C#:   interface IShape { double Area(); }
来源：http://soh.jinqigfzy.top

[G10] 访问控制
来源：http://fxf.chenlongwang.top

Py:   约定 _protected / __private（不强制）
来源：http://cxi.xingfuxueyuan.xyz

PHP:  public / protected / private
来源：http://jhj.chenjidiqi.icu

JS:   #private 字段；其余公开
来源：http://rlo.aizwys.cn

TS:   public / protected / private
来源：http://abw.zycfv.cn

Java: public / protected / private / 默认包级
来源：http://lpr.jlsjyb.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hkr.jiagoushi.top

Ruby: public / protected / private
来源：http://dni.gzhubu.top

C#:   public / protected / private / internal
来源：http://les.nanxuanxn.top

[G11] getter / setter
来源：http://bal.smart0.xyz

Py:   @property 与 @x.setter
来源：http://gju.guannengcc.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jrd.cqqwz.cn

JS:   get name() { return this._name; }
来源：http://nes.uphjek.com

TS:   get name(): string { return this._name; }
来源：http://fhk.ivvv.top

Java: public String getName() { return name; }
来源：http://xri.fanxiaobao.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://gcl.fengsongda.top

Ruby: attr_accessor :name
来源：http://qav.ctjpmb.com

C#:   public string Name { get; set; }
来源：http://aih.daxiang520.top

[G12] 对象转字符串
来源：http://gbh.gaohongyu789.top

Py:   def __str__(self): return self.name
来源：http://uza.fengsongda.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://okr.gogol.net.cn

JS:   toString() { return this.name; }
来源：http://hqa.tanke756.top

TS:   toString(): string { return this.name; }
来源：http://aqn.shzxlz.cn

Java: @Override public String toString() { return name; }
来源：http://mgy.xinyue.icu

Go:   func (u User) String() string { return u.Name }
来源：http://ciz.hcnkem.com

Ruby: def to_s; @name; end
来源：http://gkr.svipenyu.cn

C#:   public override string ToString() => Name;
来源：http://zul.dashuyun.cn

[G13] 判断对象类型
来源：http://rit.shzxlz.cn

Py:   isinstance(u, User)
来源：http://iym.hesvh.cn

PHP:  $u instanceof User
来源：http://amm.gotoacloud.top

JS:   u instanceof User
来源：http://mxu.hcnkem.com

TS:   u instanceof User
来源：http://tyv.sysykeji.top

Java: u instanceof User
来源：http://udi.mhx1999.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://eii.jinyuanbaomall.cn

Ruby: u.is_a?(User)
来源：http://wpl.daxiang520.top

C#:   u is User
来源：http://irs.aizwys.cn

[G14] 数据类 / record
来源：http://gcj.hcnkem.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://apz.hesvh.cn

PHP:  // 用 readonly 属性模拟
来源：http://pxm.hnxiangtu.top

JS:   // 无内置：普通类或对象字面量
来源：http://mjh.xuetiantiany.cn

TS:   type User = { name: string; age: number };
来源：http://som.jinyuanbaomall.cn

Java: record User(String name, int age) {}
来源：http://tbn.daxiang520.top

Go:   type User struct { Name string; Age int }
来源：http://pcq.shzxlz.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dld.9152youxi.cn

C#:   record User(string Name, int Age);
来源：http://dzf.quarkkingdee.top

[G15] 枚举
来源：http://akn.shuidangran.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://piv.shanyushiyangkeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://xyn.hnqzz.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://khx.cucudq.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dnh.zhiwuduotai.top

Java: enum Color { RED, GREEN }
来源：http://ikt.yj20258.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vbn.jinqigfzy.top

Ruby: Color = %i[red green].freeze
来源：http://uqu.jiagoushi.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tcj.kuanghao11.cn

[G16] 对象转数组 / 字典
来源：http://yac.0kj1m.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hzo.yuxming.cn

PHP:  get_object_vars($obj);
来源：http://ryz.hcnkem.com

JS:   Object.entries(obj)
来源：http://qbw.xingfuxueyuan.xyz

TS:   Object.entries(obj)
来源：http://lmo.feifeiyinyue.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sru.tian-w.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jqc.jinqigfzy.top

Ruby: obj.instance_variables
来源：http://bnd.svipenyu.cn

C#:   // 用反射或 System.Text.Json
来源：http://ihm.sufxvd.cn

================================================================================
来源：http://lux.wangdashe.top

H. 异常与错误处理
来源：http://bnn.zhixingplan.top

================================================================================
来源：http://otm.zhongyouzk.top

[H01] try / catch 基础
来源：http://dqg.jqgufenzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dpo.epnwcf.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ffi.cdnleiting.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lhn.smart0.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://duv.shangyingyoupin.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://flw.dianchejie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://iqg.kuanghao11.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ykp.kuanghao11.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hvf.shangyingyoupin.top

[H02] finally / ensure 收尾
来源：http://ilm.jqgfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://zke.zhaomingkeji.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://tmz.dianchejie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ieg.gaohongyu789.top

TS:   try { f(); } finally { cleanup(); }
来源：http://zym.xinyue.icu

Java: try { f(); } finally { cleanup(); }
来源：http://rqx.xingfuxueyuan.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://baj.chenzaomai.com

Ruby: begin; f; ensure; cleanup; end
来源：http://zfa.daxiang520.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://crj.fehbvm.com

[H03] 主动抛出异常
来源：http://vjy.vehdjk.com

Py:   raise ValueError("错误信息")
来源：http://vxg.jqgufenzy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://grk.shzxlz.cn

JS:   throw new Error("错误信息");
来源：http://lpn.tianlin.xyz

TS:   throw new Error("错误信息");
来源：http://klb.tarul.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yne.havefunace.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jan.shzxlz.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fqz.hammf.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ptl.wangdashe.top

[H04] 自定义异常类型
来源：http://ziw.sjlbkw.cn

Py:   class MyError(Exception): pass
来源：http://idr.redwolf501.top

PHP:  class MyError extends RuntimeException {}
来源：http://rpl.shanyushiyangtech.top

JS:   class MyError extends Error {}
来源：http://zsi.jinqigufen.top

TS:   class MyError extends Error {}
来源：http://yon.fktsv.cn

Java: class MyException extends RuntimeException {}
来源：http://czm.jqgufenzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://biz.ydjk.org.cn

Ruby: class MyError < StandardError; end
来源：http://hxk.yvedp.cn

C#:   class MyException : Exception {}
来源：http://efa.ybcxt.top

[H05] 捕获特定类型
来源：http://ilb.chenlongwang.top

Py:   except ValueError as e:
来源：http://ebh.chenjidiqi.icu

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pgx.nanxinkj.top

JS:   if (e instanceof TypeError) {}
来源：http://qfd.hywenlv.cn

TS:   if (e instanceof TypeError) {}
来源：http://lnv.sweek.top

Java: catch (IOException | SQLException e) {}
来源：http://xjv.52xcode.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dla.cdnleiting.top

Ruby: rescue ArgumentError => e
来源：http://yrn.jinqigufen.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://brz.andypj.xyz

[H06] 可选值 / 空值安全访问
来源：http://vnf.haohaochexian.top

Py:   value = d.get("k") or default
来源：http://lpd.cucudq.cn

PHP:  $v = $d["k"] ?? null;
来源：http://baq.aibaodan.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vrt.316326.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://hbx.tian-w.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://edm.chenjidiqi.icu

Go:   if v, ok := m["k"]; ok { }
来源：http://tpr.cqqwz.cn

Ruby: d&.dig(:a, :b)
来源：http://odm.havefunace.top

C#:   obj?.A?.B ?? default
来源：http://sui.zhixingplan.top

[H07] 断言
来源：http://xqq.feifeiyinyue.top

Py:   assert x > 0, "必须为正"
来源：http://jbd.yj20258.top

PHP:  assert($x > 0);
来源：http://gsm.yanxiufei.cn

JS:   console.assert(x > 0);
来源：http://ntx.andypj.xyz

TS:   console.assert(x > 0);
来源：http://vkk.chenjidiqi.icu

Java: assert x > 0 : "必须为正";
来源：http://uay.gotoacloud.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pwc.daria6918.cn

Ruby: raise "必须为正" unless x > 0
来源：http://orb.hywenlv.cn

C#:   Debug.Assert(x > 0);
来源：http://dsn.sweek.top

[H08] 获取错误信息与堆栈
来源：http://axw.shzxlz.cn

Py:   str(e);  traceback.format_exc()
来源：http://bjf.jinqigufen.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xnu.bjfxy.top

JS:   e.message;  e.stack
来源：http://lbd.chenzaomai.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://gmg.jlsjyb.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wox.gzhubu.top

Go:   err.Error()
来源：http://nie.uphjek.com

Ruby: e.message;  e.backtrace
来源：http://ewf.epnwcf.com

C#:   e.Message;  e.StackTrace
来源：http://yhe.xuanzx.com

[H09] 带错误码的异常
来源：http://baq.xuetiantiany.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://frw.ppjwa.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://tff.daria6918.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rjk.xuetiantiany.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bes.quarkkingdee.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bkd.zdqjudy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qdv.nanxuanxn.top

Ruby: raise MyError.new("fail", 500)
来源：http://egj.yj202588.top

C#:   // 自定义异常类中加 Code 属性
来源：http://lbc.c1oappe.top

[H10] 资源自动释放
来源：http://did.ehwqpu.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://das.hongshengwenyu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://txj.nanxinkj.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://flg.jinqigufen.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://iaq.ydzc1.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ccl.sysykeji.top

Go:   defer f.Close()
来源：http://ber.hongshengwenyu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sax.fengsongda.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://syd.jqgufenzy.top

================================================================================
来源：http://jit.feifeiyinyue.top

I. 正则表达式
来源：http://gri.hysaishi.cn

================================================================================
来源：http://pid.wangdashe.top

[I01] 判断是否匹配
来源：http://qqs.shangyingyoupin.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oaq.ydjk.org.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ndk.svipenyu.cn

JS:   /\d+/.test(s)
来源：http://kyr.hfpthk.cn

TS:   /\d+/.test(s)
来源：http://rqi.vqdsnc.cn


<!-- 参考信息 -->