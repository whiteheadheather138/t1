代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://umh.epnwcf.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://aok.yj20258888.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pan.gaohongyu789.top

[F08] 遍历目录
来源：http://jhw.nanxinkj.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://uvg.hesvh.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oww.yj202588.top

JS:   fs.readdirSync("dir")
来源：http://djf.zhijiandao.cn

TS:   fs.readdirSync("dir")
来源：http://zih.fengsongda.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gyu.ivvv.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://hha.gogol.net.cn

Ruby: Dir.children("dir")
来源：http://fwg.yvedp.cn

C#:   Directory.GetFiles("dir")
来源：http://yxo.sweek.top

[F09] 获取文件大小
来源：http://gax.tian-w.cn

Py:   os.path.getsize("a.txt")
来源：http://clc.ppjwa.cn

PHP:  filesize("a.txt");
来源：http://rec.hysaishi.cn

JS:   fs.statSync("a.txt").size
来源：http://irf.sweek.top

TS:   fs.statSync("a.txt").size
来源：http://shl.sysykeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://wkv.zhiwuduotai.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yfo.redwolf501.top

Ruby: File.size("a.txt")
来源：http://ond.ehwqpu.com

C#:   new FileInfo("a.txt").Length
来源：http://rvc.tarul.cn

[F10] 取文件扩展名 / 文件名
来源：http://ecc.fktsv.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://iqe.jqgufenzy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lqe.zhengqikj.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uqv.zycfv.cn

TS:   path.extname("a.txt")
来源：http://ije.nanxinkj.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rxb.yj20258.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://doi.redwolf501.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hzg.jinyuanbaomall.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pyq.gogol.net.cn

[F11] 复制与移动文件
来源：http://dxq.shzxlz.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cbc.cashguo.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iey.wangdashe.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jjp.0kj1m.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tyk.nwbrower.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cih.sxryk.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rao.sxryk.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pcr.shanyushiyangtech.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dkw.jiagoushi.top

[F12] CSV 读写
来源：http://vqw.xinyue.icu

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xoa.fehbvm.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ybf.zdbjq.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jyr.dashuyun.cn

TS:   // 同上
来源：http://fvp.epnwcf.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hwe.svipenyu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jyz.hongshengwenyu.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bgp.feifeiyinyue.top

C#:   // 无内置：用 CsvHelper 库
来源：http://otv.zhixingplan.top

================================================================================
来源：http://pyh.jyoumei.cn

G. 面向对象
来源：http://lhx.iojbl.cn

================================================================================
来源：http://erm.9152youxi.cn

[G01] 定义类
来源：http://abw.nanxinkj.top

Py:   class User: pass
来源：http://xaf.fanxiaobao.xyz

PHP:  class User {}
来源：http://ozt.sjlbkw.cn

JS:   class User {}
来源：http://lex.feifeiyinyue.top

TS:   class User { name: string = ""; }
来源：http://vnx.epnwcf.com

Java: class User {}
来源：http://nux.hammf.cn

Go:   type User struct { Name string }
来源：http://iob.hammf.cn

Ruby: class User; end
来源：http://rfl.snrcjt.cn

C#:   class User {}
来源：http://pyd.yanxiufei.cn

[G02] 构造函数
来源：http://szb.jyoumei.cn

Py:   def __init__(self, name): self.name = name
来源：http://uci.havefunace.top

PHP:  public function __construct(public string $name) {}
来源：http://mns.vehdjk.com

JS:   constructor(name) { this.name = name; }
来源：http://jyq.gzhubu.top

TS:   constructor(public name: string) {}
来源：http://coh.ywan-chungtsiang.top

Java: User(String name) { this.name = name; }
来源：http://zfe.dianchejie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rhl.fehbvm.com

Ruby: def initialize(name); @name = name; end
来源：http://jgx.52xcode.cn

C#:   public User(string name) { Name = name; }
来源：http://dpv.fktsv.cn

[G03] 实例属性
来源：http://fgr.tianlin.xyz

Py:   self.name = "x"
来源：http://gyt.fanxiaobao.xyz

PHP:  public string $name = "x";
来源：http://nji.yongpay.top

JS:   this.name = "x";
来源：http://zpa.0kj1m.cn

TS:   name: string = "x";
来源：http://qxr.xingfuxueyuan.xyz

Java: private String name;
来源：http://hjx.daxiang520.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://iey.cqqwz.cn

Ruby: @name = "x"
来源：http://nwf.yfazqb.com

C#:   public string Name { get; set; } = "x";
来源：http://gxv.chenlongwang.top

[G04] 定义方法
来源：http://mgb.sweek.top

Py:   def greet(self): return self.name
来源：http://zbo.jyoumei.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ffr.birdmap.top

JS:   greet() { return this.name; }
来源：http://bgd.iojbl.cn

TS:   greet(): string { return this.name; }
来源：http://rac.chenzaomai.com

Java: String greet() { return name; }
来源：http://usu.hongshengwenyu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ohq.gotoacloud.top

Ruby: def greet; @name; end
来源：http://lcx.sweek.top

C#:   public string Greet() => Name;
来源：http://vuo.yanxiufei.cn

[G05] 继承
来源：http://dnx.52xcode.cn

Py:   class Admin(User): pass
来源：http://tsf.zhiwuduotai.top

PHP:  class Admin extends User {}
来源：http://asr.pycfn.com

JS:   class Admin extends User {}
来源：http://xve.yuanzhike.top

TS:   class Admin extends User {}
来源：http://ltw.nanxinkj.top

Java: class Admin extends User {}
来源：http://ekk.sxryk.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://oqe.gogol.net.cn

Ruby: class Admin < User; end
来源：http://dlh.hongshengwenyu.top

C#:   class Admin : User {}
来源：http://vbe.cucudq.cn

[G06] 重写方法
来源：http://evc.jqgufenzy.top

Py:   def greet(self): return "admin"
来源：http://lkr.cqqwz.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xdf.ydzc1.top

JS:   greet() { return "admin"; }
来源：http://oho.dashuyun.cn

TS:   greet(): string { return "admin"; }
来源：http://iav.yonumen.top

Java: @Override String greet() { return "admin"; }
来源：http://pgu.vqdsnc.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mcg.yongpay.top

Ruby: def greet; "admin"; end
来源：http://gzg.sysykeji.top

C#:   public override string Greet() => "admin";
来源：http://ilz.epnwcf.com

[G07] 调用父类方法
来源：http://nkv.nanxinkj.top

Py:   super().greet()
来源：http://zce.sweek.top

PHP:  parent::greet();
来源：http://lof.redwolf501.top

JS:   super.greet();
来源：http://mgf.fengsongda.top

TS:   super.greet();
来源：http://cmh.hysaishi.cn

Java: super.greet();
来源：http://inc.xuanzx.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cmx.yanxiufei.cn

Ruby: super
来源：http://eud.vehdjk.com

C#:   base.Greet();
来源：http://zuk.jinyuanbaomall.cn

[G08] 静态方法与属性
来源：http://fso.yvedp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://eat.gaohongyu789.top

PHP:  public static function f() {}
来源：http://vzu.cucudq.cn

JS:   static f() {}
来源：http://wil.zhijiandao.cn

TS:   static f(): void {}
来源：http://yui.cucudq.cn

Java: static void f() {}
来源：http://mlq.aizwys.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://igj.hesvh.cn

Ruby: def self.f; end
来源：http://lul.xylfe.cn

C#:   public static void F() {}
来源：http://ddk.yangfankeji.com

[G09] 接口 / 抽象类
来源：http://ido.zdqjudy.top

Py:   from abc import ABC, abstractmethod
来源：http://sil.sweek.top

PHP:  interface Shape { public function area(): float; }
来源：http://idi.316326.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://oyp.ppjwa.cn

TS:   interface Shape { area(): number; }
来源：http://wuf.xuetiantiany.cn

Java: interface Shape { double area(); }
来源：http://tes.pycfn.com

Go:   type Shape interface { Area() float64 }
来源：http://uyd.jyoumei.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fah.shangyingyoupin.top

C#:   interface IShape { double Area(); }
来源：http://eqc.pengpengdd.cyou

[G10] 访问控制
来源：http://mwp.shzxlz.cn

Py:   约定 _protected / __private（不强制）
来源：http://raq.wangdashe.top

PHP:  public / protected / private
来源：http://umu.tianlin.xyz

JS:   #private 字段；其余公开
来源：http://bke.daxiang520.top

TS:   public / protected / private
来源：http://tcx.ctjpmb.com

Java: public / protected / private / 默认包级
来源：http://dyp.daria6918.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://yzu.sxryk.cn

Ruby: public / protected / private
来源：http://llf.52xcode.cn

C#:   public / protected / private / internal
来源：http://gum.xziqi.cn

[G11] getter / setter
来源：http://ewc.pycfn.com

Py:   @property 与 @x.setter
来源：http://xec.zdbjq.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hwn.smart0.xyz

JS:   get name() { return this._name; }
来源：http://gpg.meibo888.top

TS:   get name(): string { return this._name; }
来源：http://dai.yangfankeji.com

Java: public String getName() { return name; }
来源：http://shx.xuanzx.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://ich.nanxuanxn.top

Ruby: attr_accessor :name
来源：http://lrg.zhijiandao.cn

C#:   public string Name { get; set; }
来源：http://qja.cdnleiting.top

[G12] 对象转字符串
来源：http://veg.cdnleiting.top

Py:   def __str__(self): return self.name
来源：http://gse.jlsjyb.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://oqk.sjlbkw.cn

JS:   toString() { return this.name; }
来源：http://jee.yj20258888.top

TS:   toString(): string { return this.name; }
来源：http://qza.mhx1999.top

Java: @Override public String toString() { return name; }
来源：http://irp.fktsv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://buf.yongpay.top

Ruby: def to_s; @name; end
来源：http://ggk.tarul.cn

C#:   public override string ToString() => Name;
来源：http://ukr.zhaomingkeji.xyz

[G13] 判断对象类型
来源：http://zaw.fengsongda.top

Py:   isinstance(u, User)
来源：http://iwb.zhixingplan.top

PHP:  $u instanceof User
来源：http://fca.tianlin.xyz

JS:   u instanceof User
来源：http://mqt.cheryme.top

TS:   u instanceof User
来源：http://kaj.zycfv.cn

Java: u instanceof User
来源：http://rki.jqgfzy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://crw.zhengqikj.top

Ruby: u.is_a?(User)
来源：http://ess.pycfn.com

C#:   u is User
来源：http://rdu.yfazqb.com

[G14] 数据类 / record
来源：http://rwn.pycfn.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://djh.guannengcc.top

PHP:  // 用 readonly 属性模拟
来源：http://wld.gaohongyu789.top

JS:   // 无内置：普通类或对象字面量
来源：http://npx.tanke756.top

TS:   type User = { name: string; age: number };
来源：http://zdx.aizwys.cn

Java: record User(String name, int age) {}
来源：http://hoj.dashuyun.cn

Go:   type User struct { Name string; Age int }
来源：http://lka.sxryk.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ojp.c1oappe.top

C#:   record User(string Name, int Age);
来源：http://bkk.cqqwz.cn

[G15] 枚举
来源：http://ivn.ctjpmb.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xvu.quarkkingdee.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://mcn.hnqzz.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hnz.xinyue.icu

TS:   enum Color { Red = 1, Green = 2 }
来源：http://emm.chenzaomai.com

Java: enum Color { RED, GREEN }
来源：http://xtl.mhx1999.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mdt.zhaomingkeji.xyz

Ruby: Color = %i[red green].freeze
来源：http://bqr.hcnkem.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ttm.smart0.xyz

[G16] 对象转数组 / 字典
来源：http://giu.vehdjk.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wlx.hnqzz.top

PHP:  get_object_vars($obj);
来源：http://cba.sxryk.cn

JS:   Object.entries(obj)
来源：http://azk.cashguo.top

TS:   Object.entries(obj)
来源：http://ykw.uphjek.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dbd.ctjpmb.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://kbu.jinqigufen.top

Ruby: obj.instance_variables
来源：http://ivk.zhengqikj.top

C#:   // 用反射或 System.Text.Json
来源：http://bog.cqqwz.cn

================================================================================
来源：http://dpj.xylfe.cn

H. 异常与错误处理
来源：http://sdl.sxryk.cn

================================================================================
来源：http://lem.yanxiufei.cn

[H01] try / catch 基础
来源：http://ien.gzhubu.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hil.yonumen.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ovx.nanxinkj.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://afv.tian-w.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jkk.yuxming.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cej.guowangkeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zda.daria6918.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ikz.cqqwz.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://son.gzhubu.top

[H02] finally / ensure 收尾
来源：http://ygz.jiagoushi.top

Py:   try: f()⏎finally: cleanup()
来源：http://mmt.mhx1999.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ecs.yfazqb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://ozn.cqqwz.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vnr.9152youxi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://buh.tanke756.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://hjc.jinqigfzy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://jrx.sweek.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://feh.daxiang520.top

[H03] 主动抛出异常
来源：http://vdk.zdqjudy.top

Py:   raise ValueError("错误信息")
来源：http://yml.zdqjudy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tqj.chenlongwang.top

JS:   throw new Error("错误信息");
来源：http://qko.kuanghao11.cn

TS:   throw new Error("错误信息");
来源：http://ine.vehdjk.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://mbn.ctjpmb.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dje.yangfankeji.com

Ruby: raise ArgumentError, "错误信息"
来源：http://bss.zycfv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wzp.cdnleiting.top

[H04] 自定义异常类型
来源：http://gxm.shangyingyoupin.top

Py:   class MyError(Exception): pass
来源：http://lqk.ppjwa.cn

PHP:  class MyError extends RuntimeException {}
来源：http://zjv.yangfankeji.com

JS:   class MyError extends Error {}
来源：http://hns.vqdsnc.cn

TS:   class MyError extends Error {}
来源：http://vwv.dashuyun.cn

Java: class MyException extends RuntimeException {}
来源：http://mtd.yanxiufei.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sri.sysykeji.top

Ruby: class MyError < StandardError; end
来源：http://sfl.52xcode.cn

C#:   class MyException : Exception {}
来源：http://tmj.jqgfzy.top

[H05] 捕获特定类型
来源：http://xbq.meibo888.top

Py:   except ValueError as e:
来源：http://twy.guowangkeji.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://itk.bjfxy.top

JS:   if (e instanceof TypeError) {}
来源：http://tfp.redwolf501.top

TS:   if (e instanceof TypeError) {}
来源：http://bor.zhijiandao.cn

Java: catch (IOException | SQLException e) {}
来源：http://dtf.fengsongda.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kzl.gaohongyu789.top

Ruby: rescue ArgumentError => e
来源：http://slx.tian-w.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ghd.cashguo.top

[H06] 可选值 / 空值安全访问
来源：http://rgj.mhx1999.top

Py:   value = d.get("k") or default
来源：http://cwd.bbcook.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mbs.yj20258888.top

JS:   obj?.a?.b;  d ?? default
来源：http://huu.dashuyun.cn

TS:   obj?.a?.b;  d ?? default
来源：http://tss.hysaishi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pjl.zhixingplan.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ign.smart0.xyz

Ruby: d&.dig(:a, :b)
来源：http://lau.hywenlv.cn

C#:   obj?.A?.B ?? default
来源：http://lqy.xziqi.cn

[H07] 断言
来源：http://xds.9152youxi.cn

Py:   assert x > 0, "必须为正"
来源：http://qcx.jlsjyb.cn

PHP:  assert($x > 0);
来源：http://tgi.dianchejie.cn

JS:   console.assert(x > 0);
来源：http://dsu.52xcode.cn

TS:   console.assert(x > 0);
来源：http://zji.cqqwz.cn

Java: assert x > 0 : "必须为正";
来源：http://swh.jyoumei.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wid.vehdjk.com

Ruby: raise "必须为正" unless x > 0
来源：http://kxd.aibaodan.cn

C#:   Debug.Assert(x > 0);
来源：http://vth.hywenlv.cn

[H08] 获取错误信息与堆栈
来源：http://ygq.xuanzx.com

Py:   str(e);  traceback.format_exc()
来源：http://juu.fktsv.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://urh.hcnkem.com

JS:   e.message;  e.stack
来源：http://gbz.zdqjudy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ydn.guannengcc.top

Java: e.getMessage();  e.printStackTrace()
来源：http://nxh.snrcjt.cn

Go:   err.Error()
来源：http://ysg.hammf.cn

Ruby: e.message;  e.backtrace
来源：http://dov.xziqi.cn

C#:   e.Message;  e.StackTrace
来源：http://qqi.uphjek.com

[H09] 带错误码的异常
来源：http://bpr.yongpay.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rdz.316326.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://hwf.gzhubu.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hgt.hammf.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bta.sjlbkw.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pya.snrcjt.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kwj.chenzaomai.com

Ruby: raise MyError.new("fail", 500)
来源：http://qbe.cheryme.top

C#:   // 自定义异常类中加 Code 属性
来源：http://wfi.nanxuanxn.top

[H10] 资源自动释放
来源：http://wtt.yj20258.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://lbp.yj202588.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wfq.ybcxt.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ujd.ydzc1.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fun.zdbjq.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dyc.xuetiantiany.cn

Go:   defer f.Close()
来源：http://zis.fengsongda.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://aib.zhoulong.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gyn.zdbjq.cn

================================================================================
来源：http://spl.jinqigufen.top

I. 正则表达式
来源：http://sqy.feifeiyinyue.top

================================================================================
来源：http://riv.yuanzhike.top

[I01] 判断是否匹配
来源：http://ref.ctjpmb.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uww.cqqwz.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ylr.zhoulong.xyz

JS:   /\d+/.test(s)
来源：http://rhc.yj202588.top

TS:   /\d+/.test(s)
来源：http://icu.jinqigfzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://snn.havefunace.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ufq.shangyingyoupin.top

Ruby: s.match?(/\d+/)
来源：http://qgm.yvedp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://plz.shangyingyoupin.top


<!-- 参考信息 -->