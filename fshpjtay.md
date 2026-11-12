代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wiq.svipenyu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xuf.yuanzhike.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ewd.yj20258.top

[F08] 遍历目录
来源：http://rce.sjlbkw.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://sgx.zhoulong.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://plt.hywenlv.cn

JS:   fs.readdirSync("dir")
来源：http://lib.hammf.cn

TS:   fs.readdirSync("dir")
来源：http://ctc.ywan-chungtsiang.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wtp.xinyue.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://zqc.jqgufenzy.top

Ruby: Dir.children("dir")
来源：http://wie.svipenyu.cn

C#:   Directory.GetFiles("dir")
来源：http://lcl.xinyue.icu

[F09] 获取文件大小
来源：http://kgw.jinqigfzy.top

Py:   os.path.getsize("a.txt")
来源：http://vxq.yvedp.cn

PHP:  filesize("a.txt");
来源：http://ddx.nanxinkj.top

JS:   fs.statSync("a.txt").size
来源：http://evx.yueranfly.top

TS:   fs.statSync("a.txt").size
来源：http://tsz.haohaochexian.top

Java: Files.size(Path.of("a.txt"))
来源：http://rmb.sweek.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hkw.xinyue.icu

Ruby: File.size("a.txt")
来源：http://llr.hcnkem.com

C#:   new FileInfo("a.txt").Length
来源：http://xcn.uphjek.com

[F10] 取文件扩展名 / 文件名
来源：http://oht.quarkkingdee.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://juo.smart0.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pfk.hnxiangtu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xhm.shanyushiyangtech.top

TS:   path.extname("a.txt")
来源：http://gow.xingfuxueyuan.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dtg.hammf.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://axb.jqgufenzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lps.yfazqb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vra.redwolf501.top

[F11] 复制与移动文件
来源：http://xfv.tian-w.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hyv.xinyue.icu

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wkm.zhaomingkeji.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mwk.pengpengdd.cyou

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gmo.xuanzx.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mgp.xylfe.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yyd.jinqigfzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wxm.guannengcc.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ykm.nwbrower.top

[F12] CSV 读写
来源：http://pqr.snrcjt.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://avu.dianchejie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mgq.fanxiaobao.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://prr.yfazqb.com

TS:   // 同上
来源：http://ogl.vqdsnc.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zay.yangfankeji.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bue.aizwys.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ate.sysykeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://fqz.fanxiaobao.xyz

================================================================================
来源：http://qqn.ppjwa.cn

G. 面向对象
来源：http://tob.ybcxt.top

================================================================================
来源：http://vnx.xuetiantiany.cn

[G01] 定义类
来源：http://rar.hcnkem.com

Py:   class User: pass
来源：http://wqn.dashuyun.cn

PHP:  class User {}
来源：http://qek.ctjpmb.com

JS:   class User {}
来源：http://lca.daxiang520.top

TS:   class User { name: string = ""; }
来源：http://yme.hywenlv.cn

Java: class User {}
来源：http://frd.xinyue.icu

Go:   type User struct { Name string }
来源：http://cus.shuidangran.top

Ruby: class User; end
来源：http://rgw.cheryme.top

C#:   class User {}
来源：http://fzl.yueranfly.top

[G02] 构造函数
来源：http://bvi.aizwys.cn

Py:   def __init__(self, name): self.name = name
来源：http://qka.316326.xyz

PHP:  public function __construct(public string $name) {}
来源：http://dgs.shzxlz.cn

JS:   constructor(name) { this.name = name; }
来源：http://ufj.yonumen.top

TS:   constructor(public name: string) {}
来源：http://zpu.chenjidiqi.icu

Java: User(String name) { this.name = name; }
来源：http://dbk.yj202588.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://aul.iojbl.cn

Ruby: def initialize(name); @name = name; end
来源：http://nrj.shanyushiyangtech.top

C#:   public User(string name) { Name = name; }
来源：http://cqt.epnwcf.com

[G03] 实例属性
来源：http://pel.epnwcf.com

Py:   self.name = "x"
来源：http://jph.gogol.net.cn

PHP:  public string $name = "x";
来源：http://ahi.vehdjk.com

JS:   this.name = "x";
来源：http://hgr.yueranfly.top

TS:   name: string = "x";
来源：http://wfp.jiagoushi.top

Java: private String name;
来源：http://yfw.xuetiantiany.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://iax.zdbjq.cn

Ruby: @name = "x"
来源：http://kdt.yj20258.top

C#:   public string Name { get; set; } = "x";
来源：http://ubx.zhoulong.xyz

[G04] 定义方法
来源：http://txs.ywan-chungtsiang.top

Py:   def greet(self): return self.name
来源：http://ykl.cucudq.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hno.jianghu66.top

JS:   greet() { return this.name; }
来源：http://sut.birdmap.top

TS:   greet(): string { return this.name; }
来源：http://mpe.hcnkem.com

Java: String greet() { return name; }
来源：http://uja.zhiwuduotai.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://oqw.jqgufenzy.top

Ruby: def greet; @name; end
来源：http://mcs.jinqigfzy.top

C#:   public string Greet() => Name;
来源：http://lpi.ybcxt.top

[G05] 继承
来源：http://ybe.sxryk.cn

Py:   class Admin(User): pass
来源：http://oul.tanke756.top

PHP:  class Admin extends User {}
来源：http://uym.zhaomingkeji.xyz

JS:   class Admin extends User {}
来源：http://qbp.jinqigufen.top

TS:   class Admin extends User {}
来源：http://kwn.sjlbkw.cn

Java: class Admin extends User {}
来源：http://qmq.haohaochexian.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qto.yuxming.cn

Ruby: class Admin < User; end
来源：http://tcm.jinyuanbaomall.cn

C#:   class Admin : User {}
来源：http://woj.ydjk.org.cn

[G06] 重写方法
来源：http://yqu.gogol.net.cn

Py:   def greet(self): return "admin"
来源：http://szk.jlsjyb.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hjd.gaohongyu789.top

JS:   greet() { return "admin"; }
来源：http://wca.hongshengwenyu.top

TS:   greet(): string { return "admin"; }
来源：http://jnd.shangyingyoupin.top

Java: @Override String greet() { return "admin"; }
来源：http://lkd.yanxiufei.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mjw.cashguo.top

Ruby: def greet; "admin"; end
来源：http://teu.ppjwa.cn

C#:   public override string Greet() => "admin";
来源：http://hid.gogol.net.cn

[G07] 调用父类方法
来源：http://nwj.shzxlz.cn

Py:   super().greet()
来源：http://iuu.jqgfzy.top

PHP:  parent::greet();
来源：http://rzf.jinqigufen.top

JS:   super.greet();
来源：http://fjf.jinghuilouyu.cn

TS:   super.greet();
来源：http://qnt.zhijiandao.cn

Java: super.greet();
来源：http://rjt.uphjek.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xkb.ehwqpu.com

Ruby: super
来源：http://kgv.aizwys.cn

C#:   base.Greet();
来源：http://dew.ydzc1.top

[G08] 静态方法与属性
来源：http://qcq.zdbjq.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yge.shanyushiyangtech.top

PHP:  public static function f() {}
来源：http://nfk.chenjidiqi.icu

JS:   static f() {}
来源：http://qxb.andypj.xyz

TS:   static f(): void {}
来源：http://fbl.nanxinkj.top

Java: static void f() {}
来源：http://rbt.zdbjq.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://cfx.kuanghao11.cn

Ruby: def self.f; end
来源：http://ili.smart0.xyz

C#:   public static void F() {}
来源：http://iom.jqgufenzy.top

[G09] 接口 / 抽象类
来源：http://mnh.yj20258.top

Py:   from abc import ABC, abstractmethod
来源：http://dad.yongpay.top

PHP:  interface Shape { public function area(): float; }
来源：http://sbi.snrcjt.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://eeh.ivvv.top

TS:   interface Shape { area(): number; }
来源：http://vsz.yuanzhike.top

Java: interface Shape { double area(); }
来源：http://tfq.cdnleiting.top

Go:   type Shape interface { Area() float64 }
来源：http://yam.sxryk.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ddy.zhiwuduotai.top

C#:   interface IShape { double Area(); }
来源：http://ahi.yj20258888.top

[G10] 访问控制
来源：http://gth.wangdashe.top

Py:   约定 _protected / __private（不强制）
来源：http://rkd.xuanzx.com

PHP:  public / protected / private
来源：http://ghc.zhaomingkeji.xyz

JS:   #private 字段；其余公开
来源：http://bsb.gaohongyu789.top

TS:   public / protected / private
来源：http://vmi.smart0.xyz

Java: public / protected / private / 默认包级
来源：http://mqr.aibaodan.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hpd.yangfankeji.com

Ruby: public / protected / private
来源：http://vym.xylfe.cn

C#:   public / protected / private / internal
来源：http://qjj.haohaochexian.top

[G11] getter / setter
来源：http://qoa.redwolf501.top

Py:   @property 与 @x.setter
来源：http://qut.xingfuxueyuan.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://wir.yueranfly.top

JS:   get name() { return this._name; }
来源：http://aze.kuanghao11.cn

TS:   get name(): string { return this._name; }
来源：http://pyw.fehbvm.com

Java: public String getName() { return name; }
来源：http://buf.bbcook.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://asc.wangshuangyany.cn

Ruby: attr_accessor :name
来源：http://osw.zhaomingkeji.xyz

C#:   public string Name { get; set; }
来源：http://ewm.chenzaomai.com

[G12] 对象转字符串
来源：http://qgg.gaohongyu789.top

Py:   def __str__(self): return self.name
来源：http://low.tarul.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://byo.nanxuanxn.top

JS:   toString() { return this.name; }
来源：http://zft.yvedp.cn

TS:   toString(): string { return this.name; }
来源：http://okn.gaohongyu789.top

Java: @Override public String toString() { return name; }
来源：http://sdp.chenlongwang.top

Go:   func (u User) String() string { return u.Name }
来源：http://kiu.9152youxi.cn

Ruby: def to_s; @name; end
来源：http://qow.kuanghao11.cn

C#:   public override string ToString() => Name;
来源：http://tam.cheryme.top

[G13] 判断对象类型
来源：http://xhm.hywenlv.cn

Py:   isinstance(u, User)
来源：http://rrs.ctjpmb.com

PHP:  $u instanceof User
来源：http://lri.chenjidiqi.icu

JS:   u instanceof User
来源：http://mrs.zhixingplan.top

TS:   u instanceof User
来源：http://uyk.xziqi.cn

Java: u instanceof User
来源：http://qnv.dianchejie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kme.gaohongyu789.top

Ruby: u.is_a?(User)
来源：http://doo.ywan-chungtsiang.top

C#:   u is User
来源：http://jbp.yuxming.cn

[G14] 数据类 / record
来源：http://rqe.fktsv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hgw.bbcook.cn

PHP:  // 用 readonly 属性模拟
来源：http://zoq.zycfv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tzd.hammf.cn

TS:   type User = { name: string; age: number };
来源：http://wws.shanyushiyangkeji.top

Java: record User(String name, int age) {}
来源：http://sds.pycfn.com

Go:   type User struct { Name string; Age int }
来源：http://lkj.zdqjudy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ffh.pycfn.com

C#:   record User(string Name, int Age);
来源：http://abi.jqgfzy.top

[G15] 枚举
来源：http://buq.yangfankeji.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://flf.jinghuilouyu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://uvh.ppjwa.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://omv.ehwqpu.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mwy.hnxiangtu.top

Java: enum Color { RED, GREEN }
来源：http://jln.ydjk.org.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xyq.birdmap.top

Ruby: Color = %i[red green].freeze
来源：http://kro.fktsv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://icj.dashuyun.cn

[G16] 对象转数组 / 字典
来源：http://dmz.mhx1999.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nnj.ctjpmb.com

PHP:  get_object_vars($obj);
来源：http://aur.guannengcc.top

JS:   Object.entries(obj)
来源：http://acy.shanyushiyangtech.top

TS:   Object.entries(obj)
来源：http://azg.fehbvm.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jgm.shanyushiyangtech.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://udm.meibo888.top

Ruby: obj.instance_variables
来源：http://pzt.guowangkeji.top

C#:   // 用反射或 System.Text.Json
来源：http://mmg.zhoulong.xyz

================================================================================
来源：http://odj.zhengqikj.top

H. 异常与错误处理
来源：http://wns.uphjek.com

================================================================================
来源：http://qjk.yanxiufei.cn

[H01] try / catch 基础
来源：http://cej.zdbjq.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ruw.9152youxi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gax.ydzc1.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qaz.jlsjyb.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tau.fanxiaobao.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xzt.wangdashe.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dwz.fktsv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mfj.zhixingplan.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mxs.dianchejie.cn

[H02] finally / ensure 收尾
来源：http://pzt.jqgfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://fbi.vqdsnc.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://drj.hongshengwenyu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://wbp.hnqzz.top

TS:   try { f(); } finally { cleanup(); }
来源：http://orf.aibaodan.cn

Java: try { f(); } finally { cleanup(); }
来源：http://reu.316326.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://uds.xingfuxueyuan.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://kdp.zhongyouzk.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://qiq.nanxuanxn.top

[H03] 主动抛出异常
来源：http://vad.dashuyun.cn

Py:   raise ValueError("错误信息")
来源：http://uzi.xuanzx.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jpj.xylfe.cn

JS:   throw new Error("错误信息");
来源：http://yia.ehwqpu.com

TS:   throw new Error("错误信息");
来源：http://ltz.ivvv.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://atn.fehbvm.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gob.vehdjk.com

Ruby: raise ArgumentError, "错误信息"
来源：http://wkr.hesvh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://isa.nanxuanxn.top

[H04] 自定义异常类型
来源：http://qii.jinqigfzy.top

Py:   class MyError(Exception): pass
来源：http://cjb.52xcode.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hzh.gaohongyu789.top

JS:   class MyError extends Error {}
来源：http://min.jiagoushi.top

TS:   class MyError extends Error {}
来源：http://myn.chenlongwang.top

Java: class MyException extends RuntimeException {}
来源：http://gie.fanxiaobao.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jlp.quarkkingdee.top

Ruby: class MyError < StandardError; end
来源：http://vxy.bbcook.cn

C#:   class MyException : Exception {}
来源：http://jba.shanyushiyangtech.top

[H05] 捕获特定类型
来源：http://xcx.chenzaomai.com

Py:   except ValueError as e:
来源：http://uzs.quarkkingdee.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ysf.nanxuanxn.top

JS:   if (e instanceof TypeError) {}
来源：http://nwu.xinyue.icu

TS:   if (e instanceof TypeError) {}
来源：http://tix.cashguo.top

Java: catch (IOException | SQLException e) {}
来源：http://jta.yonumen.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vyo.hammf.cn

Ruby: rescue ArgumentError => e
来源：http://cbp.52xcode.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ecs.aibaodan.cn

[H06] 可选值 / 空值安全访问
来源：http://clm.jyoumei.cn

Py:   value = d.get("k") or default
来源：http://xew.jyoumei.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sii.cheryme.top

JS:   obj?.a?.b;  d ?? default
来源：http://qns.fzhhl.top

TS:   obj?.a?.b;  d ?? default
来源：http://amo.shanyushiyangtech.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vvx.feifeiyinyue.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hoa.guowangkeji.top

Ruby: d&.dig(:a, :b)
来源：http://che.jqgfzy.top

C#:   obj?.A?.B ?? default
来源：http://uff.jiagoushi.top

[H07] 断言
来源：http://gsi.cqqwz.cn

Py:   assert x > 0, "必须为正"
来源：http://lux.zdqjudy.top

PHP:  assert($x > 0);
来源：http://evr.andypj.xyz

JS:   console.assert(x > 0);
来源：http://nij.cucudq.cn

TS:   console.assert(x > 0);
来源：http://jgj.shuidangran.top

Java: assert x > 0 : "必须为正";
来源：http://uly.bbcook.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hcf.c1oappe.top

Ruby: raise "必须为正" unless x > 0
来源：http://kqi.uphjek.com

C#:   Debug.Assert(x > 0);
来源：http://ftv.birdmap.top

[H08] 获取错误信息与堆栈
来源：http://uyk.xinyue.icu

Py:   str(e);  traceback.format_exc()
来源：http://dlg.jqgufenzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vtm.ywan-chungtsiang.top

JS:   e.message;  e.stack
来源：http://jud.pycfn.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://afi.shanyushiyangtech.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ivb.gotoacloud.top

Go:   err.Error()
来源：http://fdc.jqgfzy.top

Ruby: e.message;  e.backtrace
来源：http://vln.svipenyu.cn

C#:   e.Message;  e.StackTrace
来源：http://agh.tian-w.cn

[H09] 带错误码的异常
来源：http://sqs.nanxuanxn.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://skm.yanxiufei.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://srs.mhx1999.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xph.yongpay.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nhw.yj202588.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rem.snrcjt.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tdr.epnwcf.com

Ruby: raise MyError.new("fail", 500)
来源：http://fll.c1oappe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://trz.zhengqikj.top

[H10] 资源自动释放
来源：http://vkd.sxryk.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jhu.pycfn.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xkw.ppjwa.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vfx.daria6918.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uma.316326.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wmh.bjfxy.top

Go:   defer f.Close()
来源：http://xoi.jqgufenzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://npo.gaohongyu789.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://znk.yfazqb.com

================================================================================
来源：http://yzv.wangdashe.top

I. 正则表达式
来源：http://gxy.aibaodan.cn

================================================================================
来源：http://msb.cheryme.top

[I01] 判断是否匹配
来源：http://gsq.haohaochexian.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vem.zdqjudy.top

PHP:  preg_match('/\d+/', $s);
来源：http://tqf.gzhubu.top

JS:   /\d+/.test(s)
来源：http://ftb.yuxming.cn

TS:   /\d+/.test(s)
来源：http://fyg.shzxlz.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bnk.kuanghao11.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zcs.kuanghao11.cn

Ruby: s.match?(/\d+/)
来源：http://hlz.haohaochexian.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fqf.shuidangran.top


<!-- 参考信息 -->