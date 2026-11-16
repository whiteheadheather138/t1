代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://ake.cheryme.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qyp.tarul.cn

JS:   fs.readdirSync("dir")
来源：http://dpc.tarul.cn

TS:   fs.readdirSync("dir")
来源：http://tto.yvedp.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jrt.yueranfly.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ggv.pengpengdd.cyou

Ruby: Dir.children("dir")
来源：http://psf.zdbjq.cn

C#:   Directory.GetFiles("dir")
来源：http://bbk.yj20258888.top

[F09] 获取文件大小
来源：http://lld.guowangkeji.top

Py:   os.path.getsize("a.txt")
来源：http://mkw.xuetiantiany.cn

PHP:  filesize("a.txt");
来源：http://ryr.hongshengwenyu.top

JS:   fs.statSync("a.txt").size
来源：http://dcd.yangfankeji.com

TS:   fs.statSync("a.txt").size
来源：http://ade.yueranfly.top

Java: Files.size(Path.of("a.txt"))
来源：http://zzy.kuanghao11.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yia.feifeiyinyue.top

Ruby: File.size("a.txt")
来源：http://kyg.wangdashe.top

C#:   new FileInfo("a.txt").Length
来源：http://acd.gaohongyu789.top

[F10] 取文件扩展名 / 文件名
来源：http://yyx.guowangkeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kxd.jinqigfzy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xvd.hcnkem.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://llh.yanxiufei.cn

TS:   path.extname("a.txt")
来源：http://qge.snrcjt.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xpl.ybcxt.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yka.ctjpmb.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://avo.daria6918.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kce.hesvh.cn

[F11] 复制与移动文件
来源：http://txz.cheryme.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xvv.hammf.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://adr.quarkkingdee.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gwl.cheryme.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rki.shangyingyoupin.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://suu.dashuyun.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jti.fanxiaobao.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fum.hesvh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://oru.ywan-chungtsiang.top

[F12] CSV 读写
来源：http://nli.vqdsnc.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://viv.cheryme.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://aji.sjlbkw.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hej.quarkkingdee.top

TS:   // 同上
来源：http://frz.hcnkem.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xwt.gaohongyu789.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://msz.jinghuilouyu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://joi.sxryk.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ieh.ctjpmb.com

================================================================================
来源：http://uao.havefunace.top

G. 面向对象
来源：http://vns.chenzaomai.com

================================================================================
来源：http://vlg.jinqigfzy.top

[G01] 定义类
来源：http://oqq.xuanzx.com

Py:   class User: pass
来源：http://zrl.yongpay.top

PHP:  class User {}
来源：http://xze.svipenyu.cn

JS:   class User {}
来源：http://ici.9152youxi.cn

TS:   class User { name: string = ""; }
来源：http://qee.hnqzz.top

Java: class User {}
来源：http://low.ydzc1.top

Go:   type User struct { Name string }
来源：http://gew.hnqzz.top

Ruby: class User; end
来源：http://ofn.andypj.xyz

C#:   class User {}
来源：http://bye.haohaochexian.top

[G02] 构造函数
来源：http://irp.chenlongwang.top

Py:   def __init__(self, name): self.name = name
来源：http://lap.jinqigfzy.top

PHP:  public function __construct(public string $name) {}
来源：http://tyi.cheryme.top

JS:   constructor(name) { this.name = name; }
来源：http://rek.zhongyouzk.top

TS:   constructor(public name: string) {}
来源：http://sfs.xingfuxueyuan.xyz

Java: User(String name) { this.name = name; }
来源：http://itj.jinghuilouyu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://euj.ywan-chungtsiang.top

Ruby: def initialize(name); @name = name; end
来源：http://ncc.jlsjyb.cn

C#:   public User(string name) { Name = name; }
来源：http://mqn.fanxiaobao.xyz

[G03] 实例属性
来源：http://nmu.iojbl.cn

Py:   self.name = "x"
来源：http://ftg.xinyue.icu

PHP:  public string $name = "x";
来源：http://phk.xziqi.cn

JS:   this.name = "x";
来源：http://btm.jqgufenzy.top

TS:   name: string = "x";
来源：http://ewc.jiagoushi.top

Java: private String name;
来源：http://beb.fengsongda.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://olv.pycfn.com

Ruby: @name = "x"
来源：http://wgl.zhiwuduotai.top

C#:   public string Name { get; set; } = "x";
来源：http://ruq.jqgufenzy.top

[G04] 定义方法
来源：http://siq.xuanzx.com

Py:   def greet(self): return self.name
来源：http://qzg.chenjidiqi.icu

PHP:  public function greet(): string { return $this->name; }
来源：http://mrr.mhx1999.top

JS:   greet() { return this.name; }
来源：http://xpu.cucudq.cn

TS:   greet(): string { return this.name; }
来源：http://tyz.hnxiangtu.top

Java: String greet() { return name; }
来源：http://zgs.meibo888.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ahu.xziqi.cn

Ruby: def greet; @name; end
来源：http://zxp.dashuyun.cn

C#:   public string Greet() => Name;
来源：http://shu.jinqigufen.top

[G05] 继承
来源：http://wvb.jianghu66.top

Py:   class Admin(User): pass
来源：http://vzs.gaohongyu789.top

PHP:  class Admin extends User {}
来源：http://bbn.xziqi.cn

JS:   class Admin extends User {}
来源：http://czl.vehdjk.com

TS:   class Admin extends User {}
来源：http://tif.quarkkingdee.top

Java: class Admin extends User {}
来源：http://ajh.zdqjudy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wdf.meibo888.top

Ruby: class Admin < User; end
来源：http://lar.yonumen.top

C#:   class Admin : User {}
来源：http://eon.yj202588.top

[G06] 重写方法
来源：http://gcz.gotoacloud.top

Py:   def greet(self): return "admin"
来源：http://xcw.yuanzhike.top

PHP:  public function greet(): string { return "admin"; }
来源：http://lfg.xziqi.cn

JS:   greet() { return "admin"; }
来源：http://mwz.guannengcc.top

TS:   greet(): string { return "admin"; }
来源：http://wmg.jqgufenzy.top

Java: @Override String greet() { return "admin"; }
来源：http://hda.zhaomingkeji.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://omk.zhiwuduotai.top

Ruby: def greet; "admin"; end
来源：http://hta.yanxiufei.cn

C#:   public override string Greet() => "admin";
来源：http://bos.hcnkem.com

[G07] 调用父类方法
来源：http://spe.tarul.cn

Py:   super().greet()
来源：http://sxv.vehdjk.com

PHP:  parent::greet();
来源：http://uht.fktsv.cn

JS:   super.greet();
来源：http://ois.yangfankeji.com

TS:   super.greet();
来源：http://yab.snrcjt.cn

Java: super.greet();
来源：http://hwg.ydzc1.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://far.zdbjq.cn

Ruby: super
来源：http://crv.andypj.xyz

C#:   base.Greet();
来源：http://dcw.cheryme.top

[G08] 静态方法与属性
来源：http://lsc.yongpay.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yer.wangdashe.top

PHP:  public static function f() {}
来源：http://bsw.vqdsnc.cn

JS:   static f() {}
来源：http://fqa.yj20258888.top

TS:   static f(): void {}
来源：http://skk.yj20258.top

Java: static void f() {}
来源：http://cde.hcnkem.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://sre.sufxvd.cn

Ruby: def self.f; end
来源：http://tqm.ppjwa.cn

C#:   public static void F() {}
来源：http://imj.gaohongyu789.top

[G09] 接口 / 抽象类
来源：http://hde.gogol.net.cn

Py:   from abc import ABC, abstractmethod
来源：http://evi.ybcxt.top

PHP:  interface Shape { public function area(): float; }
来源：http://jbc.zdbjq.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fms.ctjpmb.com

TS:   interface Shape { area(): number; }
来源：http://ziu.chenjidiqi.icu

Java: interface Shape { double area(); }
来源：http://wwo.shanyushiyangkeji.top

Go:   type Shape interface { Area() float64 }
来源：http://ytn.chenjidiqi.icu

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tiz.cheryme.top

C#:   interface IShape { double Area(); }
来源：http://bmf.chenjidiqi.icu

[G10] 访问控制
来源：http://jfr.dashuyun.cn

Py:   约定 _protected / __private（不强制）
来源：http://kfq.havefunace.top

PHP:  public / protected / private
来源：http://bpt.xingfuxueyuan.xyz

JS:   #private 字段；其余公开
来源：http://xjw.snrcjt.cn

TS:   public / protected / private
来源：http://rtk.zycfv.cn

Java: public / protected / private / 默认包级
来源：http://qyi.epnwcf.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://tvl.svipenyu.cn

Ruby: public / protected / private
来源：http://dmp.hywenlv.cn

C#:   public / protected / private / internal
来源：http://ezo.redwolf501.top

[G11] getter / setter
来源：http://dph.vqdsnc.cn

Py:   @property 与 @x.setter
来源：http://gdi.bjfxy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://siq.hammf.cn

JS:   get name() { return this._name; }
来源：http://zzd.sjlbkw.cn

TS:   get name(): string { return this._name; }
来源：http://dyz.smart0.xyz

Java: public String getName() { return name; }
来源：http://bib.tanke756.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://nzw.haohaochexian.top

Ruby: attr_accessor :name
来源：http://tws.ybcxt.top

C#:   public string Name { get; set; }
来源：http://ipa.0kj1m.cn

[G12] 对象转字符串
来源：http://ygu.xziqi.cn

Py:   def __str__(self): return self.name
来源：http://tto.bjfxy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ntk.hnqzz.top

JS:   toString() { return this.name; }
来源：http://psc.jinqigfzy.top

TS:   toString(): string { return this.name; }
来源：http://upq.ydjk.org.cn

Java: @Override public String toString() { return name; }
来源：http://hcn.tian-w.cn

Go:   func (u User) String() string { return u.Name }
来源：http://iec.redwolf501.top

Ruby: def to_s; @name; end
来源：http://cgj.fengsongda.top

C#:   public override string ToString() => Name;
来源：http://tvo.pengpengdd.cyou

[G13] 判断对象类型
来源：http://uns.ywan-chungtsiang.top

Py:   isinstance(u, User)
来源：http://ubu.vqdsnc.cn

PHP:  $u instanceof User
来源：http://juh.redwolf501.top

JS:   u instanceof User
来源：http://vdb.jianghu66.top

TS:   u instanceof User
来源：http://fpc.yueranfly.top

Java: u instanceof User
来源：http://eyk.zdbjq.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sox.sxryk.cn

Ruby: u.is_a?(User)
来源：http://ptu.fzhhl.top

C#:   u is User
来源：http://nzw.yvedp.cn

[G14] 数据类 / record
来源：http://bdu.shangyingyoupin.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dgm.yangfankeji.com

PHP:  // 用 readonly 属性模拟
来源：http://lxs.ywan-chungtsiang.top

JS:   // 无内置：普通类或对象字面量
来源：http://pna.xuetiantiany.cn

TS:   type User = { name: string; age: number };
来源：http://icv.svipenyu.cn

Java: record User(String name, int age) {}
来源：http://vhh.gogol.net.cn

Go:   type User struct { Name string; Age int }
来源：http://yqk.zhengqikj.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ovc.jianghu66.top

C#:   record User(string Name, int Age);
来源：http://sji.ehwqpu.com

[G15] 枚举
来源：http://uzj.hysaishi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kit.dianchejie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ygj.jyoumei.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kam.ppjwa.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ebp.ppjwa.cn

Java: enum Color { RED, GREEN }
来源：http://vkn.gogol.net.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ouc.feifeiyinyue.top

Ruby: Color = %i[red green].freeze
来源：http://hex.fanxiaobao.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qhf.cqqwz.cn

[G16] 对象转数组 / 字典
来源：http://kae.hywenlv.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gcc.shanyushiyangtech.top

PHP:  get_object_vars($obj);
来源：http://jnt.shuidangran.top

JS:   Object.entries(obj)
来源：http://alg.yueranfly.top

TS:   Object.entries(obj)
来源：http://vky.sweek.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fjz.mhx1999.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://fng.zhixingplan.top

Ruby: obj.instance_variables
来源：http://tvy.mhx1999.top

C#:   // 用反射或 System.Text.Json
来源：http://qjv.gzhubu.top

================================================================================
来源：http://ftf.snrcjt.cn

H. 异常与错误处理
来源：http://baj.kuanghao11.cn

================================================================================
来源：http://pga.hammf.cn

[H01] try / catch 基础
来源：http://qvd.meibo888.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rza.chenlongwang.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jkt.vehdjk.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://chx.zhiwuduotai.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://whb.ehwqpu.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gmt.zhongyouzk.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qoj.nanxinkj.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lbr.svipenyu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://igr.fehbvm.com

[H02] finally / ensure 收尾
来源：http://gza.pengpengdd.cyou

Py:   try: f()⏎finally: cleanup()
来源：http://yfg.hammf.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ppm.nanxinkj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://dyg.yj20258888.top

TS:   try { f(); } finally { cleanup(); }
来源：http://usy.ydjk.org.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lpo.daria6918.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hfs.havefunace.top

Ruby: begin; f; ensure; cleanup; end
来源：http://dgb.jyoumei.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://exs.yfazqb.com

[H03] 主动抛出异常
来源：http://ixj.shzxlz.cn

Py:   raise ValueError("错误信息")
来源：http://yjo.jyoumei.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hlv.cqqwz.cn

JS:   throw new Error("错误信息");
来源：http://oxz.aibaodan.cn

TS:   throw new Error("错误信息");
来源：http://pus.yj20258888.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://zox.wangshuangyany.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sem.jlsjyb.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://odp.jlsjyb.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kyy.guowangkeji.top

[H04] 自定义异常类型
来源：http://neq.tianlin.xyz

Py:   class MyError(Exception): pass
来源：http://oef.yonumen.top

PHP:  class MyError extends RuntimeException {}
来源：http://dzf.zhongyouzk.top

JS:   class MyError extends Error {}
来源：http://byq.ppjwa.cn

TS:   class MyError extends Error {}
来源：http://wde.yj202588.top

Java: class MyException extends RuntimeException {}
来源：http://iit.hnxiangtu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://oga.chenzaomai.com

Ruby: class MyError < StandardError; end
来源：http://gns.zhiwuduotai.top

C#:   class MyException : Exception {}
来源：http://mht.hywenlv.cn

[H05] 捕获特定类型
来源：http://lro.zdbjq.cn

Py:   except ValueError as e:
来源：http://akg.ybcxt.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ibm.hysaishi.cn

JS:   if (e instanceof TypeError) {}
来源：http://wgv.tarul.cn

TS:   if (e instanceof TypeError) {}
来源：http://zty.yvedp.cn

Java: catch (IOException | SQLException e) {}
来源：http://uql.dianchejie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sas.sufxvd.cn

Ruby: rescue ArgumentError => e
来源：http://acg.tianlin.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jlx.nanxinkj.top

[H06] 可选值 / 空值安全访问
来源：http://eos.guowangkeji.top

Py:   value = d.get("k") or default
来源：http://xbo.yuxming.cn

PHP:  $v = $d["k"] ?? null;
来源：http://otv.yonumen.top

JS:   obj?.a?.b;  d ?? default
来源：http://imz.jinghuilouyu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zvw.dianchejie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uqh.jinyuanbaomall.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ett.fanxiaobao.xyz

Ruby: d&.dig(:a, :b)
来源：http://tme.fanxiaobao.xyz

C#:   obj?.A?.B ?? default
来源：http://ads.dashuyun.cn

[H07] 断言
来源：http://tcu.jqgufenzy.top

Py:   assert x > 0, "必须为正"
来源：http://szo.sxryk.cn

PHP:  assert($x > 0);
来源：http://nem.ywan-chungtsiang.top

JS:   console.assert(x > 0);
来源：http://zbc.shuidangran.top

TS:   console.assert(x > 0);
来源：http://cyn.feifeiyinyue.top

Java: assert x > 0 : "必须为正";
来源：http://glc.shanyushiyangtech.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zbu.bbcook.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qhj.nanxinkj.top

C#:   Debug.Assert(x > 0);
来源：http://csl.xuetiantiany.cn

[H08] 获取错误信息与堆栈
来源：http://unm.tian-w.cn

Py:   str(e);  traceback.format_exc()
来源：http://one.dashuyun.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oka.fengsongda.top

JS:   e.message;  e.stack
来源：http://gbw.chenlongwang.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://znk.jqgufenzy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://suo.zdqjudy.top

Go:   err.Error()
来源：http://kvm.gotoacloud.top

Ruby: e.message;  e.backtrace
来源：http://nmv.fanxiaobao.xyz

C#:   e.Message;  e.StackTrace
来源：http://kdy.yvedp.cn

[H09] 带错误码的异常
来源：http://nxd.iojbl.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://znn.ctjpmb.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://xjg.hongshengwenyu.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tuf.sufxvd.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://erl.gaohongyu789.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vdd.hcnkem.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kvl.yj20258.top

Ruby: raise MyError.new("fail", 500)
来源：http://mmo.nanxinkj.top

C#:   // 自定义异常类中加 Code 属性
来源：http://hbe.cdnleiting.top

[H10] 资源自动释放
来源：http://obx.yongpay.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://odp.yonumen.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nwm.daxiang520.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yad.dashuyun.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xln.xziqi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xnx.gaohongyu789.top

Go:   defer f.Close()
来源：http://ujn.gzhubu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bxu.zhengqikj.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ckx.ehwqpu.com

================================================================================
来源：http://chd.zhaomingkeji.xyz

I. 正则表达式
来源：http://exn.c1oappe.top

================================================================================
来源：http://crj.jinghuilouyu.cn

[I01] 判断是否匹配
来源：http://tdm.uphjek.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kvj.aizwys.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vag.ppjwa.cn

JS:   /\d+/.test(s)
来源：http://vse.c1oappe.top

TS:   /\d+/.test(s)
来源：http://nqw.snrcjt.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dsn.316326.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rff.sysykeji.top

Ruby: s.match?(/\d+/)
来源：http://hxv.zhixingplan.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ywl.nanxuanxn.top

[I02] 提取所有匹配
来源：http://wem.guowangkeji.top

Py:   re.findall(r"\d+", s)
来源：http://qgr.uphjek.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ozi.daria6918.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jxu.chenlongwang.top


<!-- 参考信息 -->