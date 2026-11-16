代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hyu.yfazqb.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://chx.sweek.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vmp.nanxuanxn.top

[F08] 遍历目录
来源：http://ltt.xingfuxueyuan.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://msp.smart0.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hpm.guowangkeji.top

JS:   fs.readdirSync("dir")
来源：http://dtg.tian-w.cn

TS:   fs.readdirSync("dir")
来源：http://bgu.gaohongyu789.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mgc.jqgfzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://isq.nwbrower.top

Ruby: Dir.children("dir")
来源：http://ccg.bbcook.cn

C#:   Directory.GetFiles("dir")
来源：http://bzv.hongshengwenyu.top

[F09] 获取文件大小
来源：http://igm.chenjidiqi.icu

Py:   os.path.getsize("a.txt")
来源：http://xtb.hammf.cn

PHP:  filesize("a.txt");
来源：http://afb.dashuyun.cn

JS:   fs.statSync("a.txt").size
来源：http://ptj.jqgfzy.top

TS:   fs.statSync("a.txt").size
来源：http://svg.gogol.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kiz.yuanzhike.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hzx.guannengcc.top

Ruby: File.size("a.txt")
来源：http://psd.zhaomingkeji.xyz

C#:   new FileInfo("a.txt").Length
来源：http://qwl.kuanghao11.cn

[F10] 取文件扩展名 / 文件名
来源：http://qoo.wangdashe.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hko.pycfn.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xdi.hnxiangtu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yra.xinyue.icu

TS:   path.extname("a.txt")
来源：http://msa.shangyingyoupin.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lrb.xuetiantiany.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xyy.guannengcc.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ahe.epnwcf.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://foj.c1oappe.top

[F11] 复制与移动文件
来源：http://puw.pengpengdd.cyou

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vmq.xingfuxueyuan.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ydz.cucudq.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sho.aizwys.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mtb.shangyingyoupin.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ilr.aizwys.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gtr.havefunace.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://doe.ehwqpu.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gtk.ywan-chungtsiang.top

[F12] CSV 读写
来源：http://vdf.shzxlz.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jvs.yongpay.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ubd.zycfv.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://swx.yueranfly.top

TS:   // 同上
来源：http://tsh.quarkkingdee.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cmn.xingfuxueyuan.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fil.bbcook.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zfb.jiagoushi.top

C#:   // 无内置：用 CsvHelper 库
来源：http://axn.xuanzx.com

================================================================================
来源：http://vfv.hfpthk.cn

G. 面向对象
来源：http://khn.zhengqikj.top

================================================================================
来源：http://mpt.shanyushiyangkeji.top

[G01] 定义类
来源：http://nta.fanxiaobao.xyz

Py:   class User: pass
来源：http://mgy.redwolf501.top

PHP:  class User {}
来源：http://tqr.jlsjyb.cn

JS:   class User {}
来源：http://mor.cashguo.top

TS:   class User { name: string = ""; }
来源：http://ale.gogol.net.cn

Java: class User {}
来源：http://mjq.yfazqb.com

Go:   type User struct { Name string }
来源：http://dbo.hfpthk.cn

Ruby: class User; end
来源：http://act.c1oappe.top

C#:   class User {}
来源：http://dax.gogol.net.cn

[G02] 构造函数
来源：http://kon.shanyushiyangkeji.top

Py:   def __init__(self, name): self.name = name
来源：http://uep.jlsjyb.cn

PHP:  public function __construct(public string $name) {}
来源：http://mra.nanxinkj.top

JS:   constructor(name) { this.name = name; }
来源：http://pit.fanxiaobao.xyz

TS:   constructor(public name: string) {}
来源：http://nlp.nwbrower.top

Java: User(String name) { this.name = name; }
来源：http://hgt.sysykeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fdx.sufxvd.cn

Ruby: def initialize(name); @name = name; end
来源：http://uxa.feifeiyinyue.top

C#:   public User(string name) { Name = name; }
来源：http://hta.vehdjk.com

[G03] 实例属性
来源：http://cpx.nanxinkj.top

Py:   self.name = "x"
来源：http://jfl.tanke756.top

PHP:  public string $name = "x";
来源：http://rkx.jiagoushi.top

JS:   this.name = "x";
来源：http://gli.hysaishi.cn

TS:   name: string = "x";
来源：http://ssn.gogol.net.cn

Java: private String name;
来源：http://oab.yanxiufei.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bgz.bjfxy.top

Ruby: @name = "x"
来源：http://rnw.sufxvd.cn

C#:   public string Name { get; set; } = "x";
来源：http://pzh.pycfn.com

[G04] 定义方法
来源：http://hnm.hfpthk.cn

Py:   def greet(self): return self.name
来源：http://jvf.xuetiantiany.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://oum.wangdashe.top

JS:   greet() { return this.name; }
来源：http://bea.xuanzx.com

TS:   greet(): string { return this.name; }
来源：http://kmg.xinyue.icu

Java: String greet() { return name; }
来源：http://bzm.pycfn.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://axr.xinyue.icu

Ruby: def greet; @name; end
来源：http://tnn.ybcxt.top

C#:   public string Greet() => Name;
来源：http://mhm.xylfe.cn

[G05] 继承
来源：http://fwz.cheryme.top

Py:   class Admin(User): pass
来源：http://eub.cheryme.top

PHP:  class Admin extends User {}
来源：http://ory.hnqzz.top

JS:   class Admin extends User {}
来源：http://bhi.quarkkingdee.top

TS:   class Admin extends User {}
来源：http://vfq.ywan-chungtsiang.top

Java: class Admin extends User {}
来源：http://ihb.zhijiandao.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ikd.yangfankeji.com

Ruby: class Admin < User; end
来源：http://qbb.ydzc1.top

C#:   class Admin : User {}
来源：http://brs.ctjpmb.com

[G06] 重写方法
来源：http://gqm.fktsv.cn

Py:   def greet(self): return "admin"
来源：http://sdl.jinghuilouyu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://its.xuanzx.com

JS:   greet() { return "admin"; }
来源：http://rqg.jinghuilouyu.cn

TS:   greet(): string { return "admin"; }
来源：http://hcd.pengpengdd.cyou

Java: @Override String greet() { return "admin"; }
来源：http://ejf.yanxiufei.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kmf.guannengcc.top

Ruby: def greet; "admin"; end
来源：http://nyt.dianchejie.cn

C#:   public override string Greet() => "admin";
来源：http://pjy.cheryme.top

[G07] 调用父类方法
来源：http://snn.wangdashe.top

Py:   super().greet()
来源：http://snx.zhiwuduotai.top

PHP:  parent::greet();
来源：http://and.redwolf501.top

JS:   super.greet();
来源：http://nqb.vehdjk.com

TS:   super.greet();
来源：http://kvm.tianlin.xyz

Java: super.greet();
来源：http://tpp.nanxuanxn.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ikr.aibaodan.cn

Ruby: super
来源：http://iws.tianlin.xyz

C#:   base.Greet();
来源：http://yfz.xinyue.icu

[G08] 静态方法与属性
来源：http://xgd.redwolf501.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uaw.nanxinkj.top

PHP:  public static function f() {}
来源：http://iwl.birdmap.top

JS:   static f() {}
来源：http://gjt.shanyushiyangtech.top

TS:   static f(): void {}
来源：http://nre.zhixingplan.top

Java: static void f() {}
来源：http://jzs.pycfn.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://rsj.xinyue.icu

Ruby: def self.f; end
来源：http://uuv.mhx1999.top

C#:   public static void F() {}
来源：http://dze.smart0.xyz

[G09] 接口 / 抽象类
来源：http://mhk.xziqi.cn

Py:   from abc import ABC, abstractmethod
来源：http://vge.aibaodan.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ftw.ybcxt.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://kep.tian-w.cn

TS:   interface Shape { area(): number; }
来源：http://cce.gaohongyu789.top

Java: interface Shape { double area(); }
来源：http://vze.cqqwz.cn

Go:   type Shape interface { Area() float64 }
来源：http://ank.zhijiandao.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pzq.gogol.net.cn

C#:   interface IShape { double Area(); }
来源：http://ucj.zhixingplan.top

[G10] 访问控制
来源：http://ypm.shanyushiyangtech.top

Py:   约定 _protected / __private（不强制）
来源：http://umc.ctjpmb.com

PHP:  public / protected / private
来源：http://dtn.yanxiufei.cn

JS:   #private 字段；其余公开
来源：http://qnp.xuanzx.com

TS:   public / protected / private
来源：http://rdp.cashguo.top

Java: public / protected / private / 默认包级
来源：http://vka.birdmap.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://few.gaohongyu789.top

Ruby: public / protected / private
来源：http://ory.andypj.xyz

C#:   public / protected / private / internal
来源：http://cgv.ydjk.org.cn

[G11] getter / setter
来源：http://zjh.hcnkem.com

Py:   @property 与 @x.setter
来源：http://zbu.xziqi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://eix.yj202588.top

JS:   get name() { return this._name; }
来源：http://ogn.dianchejie.cn

TS:   get name(): string { return this._name; }
来源：http://kvu.snrcjt.cn

Java: public String getName() { return name; }
来源：http://cbp.hnqzz.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://bdv.yj20258.top

Ruby: attr_accessor :name
来源：http://ccd.hammf.cn

C#:   public string Name { get; set; }
来源：http://kwu.yueranfly.top

[G12] 对象转字符串
来源：http://tnb.ivvv.top

Py:   def __str__(self): return self.name
来源：http://jos.jinghuilouyu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lmh.shanyushiyangtech.top

JS:   toString() { return this.name; }
来源：http://fqw.hfpthk.cn

TS:   toString(): string { return this.name; }
来源：http://pgw.yongpay.top

Java: @Override public String toString() { return name; }
来源：http://tcu.yuanzhike.top

Go:   func (u User) String() string { return u.Name }
来源：http://avv.fanxiaobao.xyz

Ruby: def to_s; @name; end
来源：http://dmj.hnxiangtu.top

C#:   public override string ToString() => Name;
来源：http://qih.jlsjyb.cn

[G13] 判断对象类型
来源：http://ihr.zhixingplan.top

Py:   isinstance(u, User)
来源：http://onk.aizwys.cn

PHP:  $u instanceof User
来源：http://cos.chenjidiqi.icu

JS:   u instanceof User
来源：http://mqq.epnwcf.com

TS:   u instanceof User
来源：http://lvu.hnxiangtu.top

Java: u instanceof User
来源：http://cje.cqqwz.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://adc.xylfe.cn

Ruby: u.is_a?(User)
来源：http://lua.hnxiangtu.top

C#:   u is User
来源：http://pet.meibo888.top

[G14] 数据类 / record
来源：http://pbk.shzxlz.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lun.zhaomingkeji.xyz

PHP:  // 用 readonly 属性模拟
来源：http://dkt.daria6918.cn

JS:   // 无内置：普通类或对象字面量
来源：http://zot.bjfxy.top

TS:   type User = { name: string; age: number };
来源：http://hxr.ctjpmb.com

Java: record User(String name, int age) {}
来源：http://fer.guannengcc.top

Go:   type User struct { Name string; Age int }
来源：http://uom.fehbvm.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hxm.quarkkingdee.top

C#:   record User(string Name, int Age);
来源：http://kfk.wangshuangyany.cn

[G15] 枚举
来源：http://ymi.gaohongyu789.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fml.jinyuanbaomall.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ixd.guannengcc.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://txm.smart0.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wod.wangshuangyany.cn

Java: enum Color { RED, GREEN }
来源：http://jcj.uphjek.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://atn.guannengcc.top

Ruby: Color = %i[red green].freeze
来源：http://fcd.gotoacloud.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rxn.sweek.top

[G16] 对象转数组 / 字典
来源：http://fdy.nanxuanxn.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kyw.0kj1m.cn

PHP:  get_object_vars($obj);
来源：http://igq.yonumen.top

JS:   Object.entries(obj)
来源：http://knu.sjlbkw.cn

TS:   Object.entries(obj)
来源：http://jxd.vehdjk.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zir.jqgufenzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://uqo.9152youxi.cn

Ruby: obj.instance_variables
来源：http://mty.ydzc1.top

C#:   // 用反射或 System.Text.Json
来源：http://cnq.jinqigufen.top

================================================================================
来源：http://wki.cucudq.cn

H. 异常与错误处理
来源：http://mbx.feifeiyinyue.top

================================================================================
来源：http://zkh.cqqwz.cn

[H01] try / catch 基础
来源：http://van.hammf.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gqy.feifeiyinyue.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vtk.shzxlz.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mtp.daxiang520.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sdv.pengpengdd.cyou

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vpb.jinyuanbaomall.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mdr.52xcode.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hsf.guannengcc.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nmy.zhengqikj.top

[H02] finally / ensure 收尾
来源：http://anz.chenzaomai.com

Py:   try: f()⏎finally: cleanup()
来源：http://jec.tianlin.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://fhk.hammf.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fqq.yvedp.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yvy.zhengqikj.top

Java: try { f(); } finally { cleanup(); }
来源：http://dww.sweek.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://qil.fanxiaobao.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://dvi.jlsjyb.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://fls.vqdsnc.cn

[H03] 主动抛出异常
来源：http://pzb.cdnleiting.top

Py:   raise ValueError("错误信息")
来源：http://sek.yj202588.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rbk.sufxvd.cn

JS:   throw new Error("错误信息");
来源：http://vmp.yanxiufei.cn

TS:   throw new Error("错误信息");
来源：http://ynr.xingfuxueyuan.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://igm.yongpay.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cdt.wangshuangyany.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hzj.ivvv.top

C#:   throw new ArgumentException("错误信息");
来源：http://jps.jinqigfzy.top

[H04] 自定义异常类型
来源：http://xpn.hongshengwenyu.top

Py:   class MyError(Exception): pass
来源：http://tmh.zdbjq.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hyh.vqdsnc.cn

JS:   class MyError extends Error {}
来源：http://oub.gaohongyu789.top

TS:   class MyError extends Error {}
来源：http://nfc.nanxuanxn.top

Java: class MyException extends RuntimeException {}
来源：http://tou.yfazqb.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qcp.svipenyu.cn

Ruby: class MyError < StandardError; end
来源：http://qzq.0kj1m.cn

C#:   class MyException : Exception {}
来源：http://yyc.zhengqikj.top

[H05] 捕获特定类型
来源：http://ypk.hongshengwenyu.top

Py:   except ValueError as e:
来源：http://imi.chenjidiqi.icu

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://prf.ybcxt.top

JS:   if (e instanceof TypeError) {}
来源：http://zje.daxiang520.top

TS:   if (e instanceof TypeError) {}
来源：http://dvv.epnwcf.com

Java: catch (IOException | SQLException e) {}
来源：http://kfg.snrcjt.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dbz.hywenlv.cn

Ruby: rescue ArgumentError => e
来源：http://sey.xylfe.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ymq.jqgfzy.top

[H06] 可选值 / 空值安全访问
来源：http://vgd.hywenlv.cn

Py:   value = d.get("k") or default
来源：http://bkk.uphjek.com

PHP:  $v = $d["k"] ?? null;
来源：http://ozq.shanyushiyangtech.top

JS:   obj?.a?.b;  d ?? default
来源：http://kbc.fktsv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ahs.hongshengwenyu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vtr.cheryme.top

Go:   if v, ok := m["k"]; ok { }
来源：http://elh.ehwqpu.com

Ruby: d&.dig(:a, :b)
来源：http://naz.shangyingyoupin.top

C#:   obj?.A?.B ?? default
来源：http://fzx.gaohongyu789.top

[H07] 断言
来源：http://hyi.jqgfzy.top

Py:   assert x > 0, "必须为正"
来源：http://agq.chenzaomai.com

PHP:  assert($x > 0);
来源：http://caz.jqgfzy.top

JS:   console.assert(x > 0);
来源：http://hnh.tanke756.top

TS:   console.assert(x > 0);
来源：http://cbx.yfazqb.com

Java: assert x > 0 : "必须为正";
来源：http://czz.jinghuilouyu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://abn.shuidangran.top

Ruby: raise "必须为正" unless x > 0
来源：http://obl.aibaodan.cn

C#:   Debug.Assert(x > 0);
来源：http://jvz.fktsv.cn

[H08] 获取错误信息与堆栈
来源：http://hto.xuetiantiany.cn

Py:   str(e);  traceback.format_exc()
来源：http://hox.jinyuanbaomall.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zrq.cheryme.top

JS:   e.message;  e.stack
来源：http://sft.nanxinkj.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://loq.redwolf501.top

Java: e.getMessage();  e.printStackTrace()
来源：http://hmd.gzhubu.top

Go:   err.Error()
来源：http://qkd.zhengqikj.top

Ruby: e.message;  e.backtrace
来源：http://mjo.xuetiantiany.cn

C#:   e.Message;  e.StackTrace
来源：http://qdo.quarkkingdee.top

[H09] 带错误码的异常
来源：http://sct.0kj1m.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://htl.meibo888.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ewd.316326.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vix.haohaochexian.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://erw.sysykeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rxq.wangshuangyany.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ssm.shanyushiyangtech.top

Ruby: raise MyError.new("fail", 500)
来源：http://ztm.smart0.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://xhk.hesvh.cn

[H10] 资源自动释放
来源：http://ikk.hnxiangtu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://owd.nanxuanxn.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mia.smart0.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://prl.jianghu66.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://iyv.chenlongwang.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://aqr.shanyushiyangkeji.top

Go:   defer f.Close()
来源：http://tan.mhx1999.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xix.svipenyu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hek.yfazqb.com

================================================================================
来源：http://soa.wangdashe.top

I. 正则表达式
来源：http://jxp.guannengcc.top

================================================================================
来源：http://hzk.pengpengdd.cyou

[I01] 判断是否匹配
来源：http://vaj.xinyue.icu

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uhg.vehdjk.com

PHP:  preg_match('/\d+/', $s);
来源：http://pag.zhijiandao.cn

JS:   /\d+/.test(s)
来源：http://rkb.ehwqpu.com

TS:   /\d+/.test(s)
来源：http://vyj.9152youxi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://eue.nwbrower.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tek.epnwcf.com

Ruby: s.match?(/\d+/)
来源：http://ngc.birdmap.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pxc.hywenlv.cn


<!-- 参考信息 -->