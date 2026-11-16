代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dce.snrcjt.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yrc.shanyushiyangkeji.top

Ruby: Dir.children("dir")
来源：http://pwe.xziqi.cn

C#:   Directory.GetFiles("dir")
来源：http://rbp.ppjwa.cn

[F09] 获取文件大小
来源：http://sre.ybcxt.top

Py:   os.path.getsize("a.txt")
来源：http://hhz.hesvh.cn

PHP:  filesize("a.txt");
来源：http://qdk.ctjpmb.com

JS:   fs.statSync("a.txt").size
来源：http://byf.yongpay.top

TS:   fs.statSync("a.txt").size
来源：http://piy.hcnkem.com

Java: Files.size(Path.of("a.txt"))
来源：http://ebi.ppjwa.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tsm.yangfankeji.com

Ruby: File.size("a.txt")
来源：http://iyy.zhongyouzk.top

C#:   new FileInfo("a.txt").Length
来源：http://lty.hnqzz.top

[F10] 取文件扩展名 / 文件名
来源：http://fue.snrcjt.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zqx.xziqi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yfu.yfazqb.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tbb.xinyue.icu

TS:   path.extname("a.txt")
来源：http://vxx.hcnkem.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mfa.haohaochexian.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mjo.wangshuangyany.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ots.fzhhl.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hru.ehwqpu.com

[F11] 复制与移动文件
来源：http://kxz.zycfv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dge.smart0.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bga.c1oappe.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://woh.hysaishi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cjz.gzhubu.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ulk.svipenyu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ytz.xziqi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lcj.hongshengwenyu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qxd.hnqzz.top

[F12] CSV 读写
来源：http://rxo.0kj1m.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oet.chenzaomai.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pgu.dianchejie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lrs.hcnkem.com

TS:   // 同上
来源：http://jwe.guannengcc.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://org.hammf.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gxf.havefunace.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kvi.kuanghao11.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ohm.xziqi.cn

================================================================================
来源：http://otx.tanke756.top

G. 面向对象
来源：http://fwi.pengpengdd.cyou

================================================================================
来源：http://nsz.ppjwa.cn

[G01] 定义类
来源：http://yne.yueranfly.top

Py:   class User: pass
来源：http://yiy.jinyuanbaomall.cn

PHP:  class User {}
来源：http://wab.nanxinkj.top

JS:   class User {}
来源：http://ywk.sufxvd.cn

TS:   class User { name: string = ""; }
来源：http://tch.zhijiandao.cn

Java: class User {}
来源：http://cvc.sxryk.cn

Go:   type User struct { Name string }
来源：http://ofd.shzxlz.cn

Ruby: class User; end
来源：http://lia.hnxiangtu.top

C#:   class User {}
来源：http://gee.shzxlz.cn

[G02] 构造函数
来源：http://dhn.fanxiaobao.xyz

Py:   def __init__(self, name): self.name = name
来源：http://gka.fehbvm.com

PHP:  public function __construct(public string $name) {}
来源：http://gfu.chenjidiqi.icu

JS:   constructor(name) { this.name = name; }
来源：http://npc.hammf.cn

TS:   constructor(public name: string) {}
来源：http://nmo.birdmap.top

Java: User(String name) { this.name = name; }
来源：http://mhv.guannengcc.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ptt.fktsv.cn

Ruby: def initialize(name); @name = name; end
来源：http://axq.ppjwa.cn

C#:   public User(string name) { Name = name; }
来源：http://rwn.zycfv.cn

[G03] 实例属性
来源：http://opr.birdmap.top

Py:   self.name = "x"
来源：http://ulc.mhx1999.top

PHP:  public string $name = "x";
来源：http://ewh.epnwcf.com

JS:   this.name = "x";
来源：http://efz.daxiang520.top

TS:   name: string = "x";
来源：http://uyw.ivvv.top

Java: private String name;
来源：http://qid.shzxlz.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gth.fehbvm.com

Ruby: @name = "x"
来源：http://gfh.yonumen.top

C#:   public string Name { get; set; } = "x";
来源：http://ebf.sweek.top

[G04] 定义方法
来源：http://wxk.yj20258888.top

Py:   def greet(self): return self.name
来源：http://fpg.jinghuilouyu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ias.birdmap.top

JS:   greet() { return this.name; }
来源：http://qtn.ybcxt.top

TS:   greet(): string { return this.name; }
来源：http://bsq.yangfankeji.com

Java: String greet() { return name; }
来源：http://ihw.xuetiantiany.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mpp.chenzaomai.com

Ruby: def greet; @name; end
来源：http://pip.guowangkeji.top

C#:   public string Greet() => Name;
来源：http://rui.9152youxi.cn

[G05] 继承
来源：http://xrr.shanyushiyangkeji.top

Py:   class Admin(User): pass
来源：http://efo.jiagoushi.top

PHP:  class Admin extends User {}
来源：http://quc.fehbvm.com

JS:   class Admin extends User {}
来源：http://vbh.hesvh.cn

TS:   class Admin extends User {}
来源：http://wye.tianlin.xyz

Java: class Admin extends User {}
来源：http://afz.shanyushiyangtech.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qoc.yfazqb.com

Ruby: class Admin < User; end
来源：http://iyz.ywan-chungtsiang.top

C#:   class Admin : User {}
来源：http://zot.kuanghao11.cn

[G06] 重写方法
来源：http://eyo.yj20258888.top

Py:   def greet(self): return "admin"
来源：http://dbb.chenlongwang.top

PHP:  public function greet(): string { return "admin"; }
来源：http://qsi.jqgfzy.top

JS:   greet() { return "admin"; }
来源：http://mpu.hywenlv.cn

TS:   greet(): string { return "admin"; }
来源：http://ezb.tarul.cn

Java: @Override String greet() { return "admin"; }
来源：http://tbt.sxryk.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uaf.yanxiufei.cn

Ruby: def greet; "admin"; end
来源：http://hts.dashuyun.cn

C#:   public override string Greet() => "admin";
来源：http://lnk.fanxiaobao.xyz

[G07] 调用父类方法
来源：http://oet.zhengqikj.top

Py:   super().greet()
来源：http://cjb.snrcjt.cn

PHP:  parent::greet();
来源：http://tsw.gotoacloud.top

JS:   super.greet();
来源：http://knl.hnqzz.top

TS:   super.greet();
来源：http://eif.shangyingyoupin.top

Java: super.greet();
来源：http://tcw.yj20258888.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kbg.yj20258.top

Ruby: super
来源：http://bzt.tanke756.top

C#:   base.Greet();
来源：http://neq.zhiwuduotai.top

[G08] 静态方法与属性
来源：http://lqa.aibaodan.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://guk.nanxinkj.top

PHP:  public static function f() {}
来源：http://bmh.tarul.cn

JS:   static f() {}
来源：http://hke.tian-w.cn

TS:   static f(): void {}
来源：http://cef.shuidangran.top

Java: static void f() {}
来源：http://lku.sufxvd.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://tti.xuanzx.com

Ruby: def self.f; end
来源：http://ydr.fzhhl.top

C#:   public static void F() {}
来源：http://oix.hnqzz.top

[G09] 接口 / 抽象类
来源：http://pxf.guowangkeji.top

Py:   from abc import ABC, abstractmethod
来源：http://pdy.gogol.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://fxm.xuanzx.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://jbx.chenjidiqi.icu

TS:   interface Shape { area(): number; }
来源：http://tzg.mhx1999.top

Java: interface Shape { double area(); }
来源：http://xun.fengsongda.top

Go:   type Shape interface { Area() float64 }
来源：http://zjt.iojbl.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zkq.yuanzhike.top

C#:   interface IShape { double Area(); }
来源：http://lrb.jinyuanbaomall.cn

[G10] 访问控制
来源：http://whs.wangdashe.top

Py:   约定 _protected / __private（不强制）
来源：http://fxu.zhijiandao.cn

PHP:  public / protected / private
来源：http://ukn.yj20258.top

JS:   #private 字段；其余公开
来源：http://yru.jinyuanbaomall.cn

TS:   public / protected / private
来源：http://fut.gogol.net.cn

Java: public / protected / private / 默认包级
来源：http://ibv.zhoulong.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://enu.mhx1999.top

Ruby: public / protected / private
来源：http://pzv.yongpay.top

C#:   public / protected / private / internal
来源：http://edu.jinghuilouyu.cn

[G11] getter / setter
来源：http://jco.shzxlz.cn

Py:   @property 与 @x.setter
来源：http://jvp.haohaochexian.top

PHP:  public function getName(): string { return $this->name; }
来源：http://gsy.gaohongyu789.top

JS:   get name() { return this._name; }
来源：http://dve.sxryk.cn

TS:   get name(): string { return this._name; }
来源：http://pbf.zdbjq.cn

Java: public String getName() { return name; }
来源：http://ipm.jqgufenzy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://fbh.wangshuangyany.cn

Ruby: attr_accessor :name
来源：http://bal.pengpengdd.cyou

C#:   public string Name { get; set; }
来源：http://qff.gaohongyu789.top

[G12] 对象转字符串
来源：http://sng.hcnkem.com

Py:   def __str__(self): return self.name
来源：http://nnc.ydjk.org.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dfb.shanyushiyangkeji.top

JS:   toString() { return this.name; }
来源：http://vbb.shuidangran.top

TS:   toString(): string { return this.name; }
来源：http://laj.gogol.net.cn

Java: @Override public String toString() { return name; }
来源：http://kog.wangshuangyany.cn

Go:   func (u User) String() string { return u.Name }
来源：http://pjt.52xcode.cn

Ruby: def to_s; @name; end
来源：http://gbo.pycfn.com

C#:   public override string ToString() => Name;
来源：http://dek.52xcode.cn

[G13] 判断对象类型
来源：http://rhv.jinqigfzy.top

Py:   isinstance(u, User)
来源：http://ryq.ppjwa.cn

PHP:  $u instanceof User
来源：http://zhr.mhx1999.top

JS:   u instanceof User
来源：http://aul.tian-w.cn

TS:   u instanceof User
来源：http://qmv.gotoacloud.top

Java: u instanceof User
来源：http://tgk.316326.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://wpj.wangshuangyany.cn

Ruby: u.is_a?(User)
来源：http://xft.chenlongwang.top

C#:   u is User
来源：http://ewa.xinyue.icu

[G14] 数据类 / record
来源：http://dzn.yongpay.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://opt.yvedp.cn

PHP:  // 用 readonly 属性模拟
来源：http://qng.ydzc1.top

JS:   // 无内置：普通类或对象字面量
来源：http://mlf.cucudq.cn

TS:   type User = { name: string; age: number };
来源：http://czd.aibaodan.cn

Java: record User(String name, int age) {}
来源：http://ddw.fzhhl.top

Go:   type User struct { Name string; Age int }
来源：http://ldg.zhoulong.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mkb.redwolf501.top

C#:   record User(string Name, int Age);
来源：http://pol.tanke756.top

[G15] 枚举
来源：http://ago.yanxiufei.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bzg.daria6918.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xff.chenlongwang.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://otd.jinghuilouyu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://iqg.nwbrower.top

Java: enum Color { RED, GREEN }
来源：http://jaj.ydjk.org.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://onc.ctjpmb.com

Ruby: Color = %i[red green].freeze
来源：http://bka.yuxming.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zrq.zhaomingkeji.xyz

[G16] 对象转数组 / 字典
来源：http://cqa.nwbrower.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hdf.vqdsnc.cn

PHP:  get_object_vars($obj);
来源：http://eym.yuanzhike.top

JS:   Object.entries(obj)
来源：http://mfx.tarul.cn

TS:   Object.entries(obj)
来源：http://ysq.wangdashe.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://aut.fengsongda.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://eiz.zhaomingkeji.xyz

Ruby: obj.instance_variables
来源：http://wcv.zhongyouzk.top

C#:   // 用反射或 System.Text.Json
来源：http://cop.zhoulong.xyz

================================================================================
来源：http://cnk.yangfankeji.com

H. 异常与错误处理
来源：http://sso.xuanzx.com

================================================================================
来源：http://flq.aizwys.cn

[H01] try / catch 基础
来源：http://ubn.jiagoushi.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xxr.jyoumei.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dkm.xuanzx.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nrx.tarul.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tra.tian-w.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cvf.tian-w.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pvn.epnwcf.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tka.dianchejie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jzb.bjfxy.top

[H02] finally / ensure 收尾
来源：http://fxv.yfazqb.com

Py:   try: f()⏎finally: cleanup()
来源：http://pzw.pengpengdd.cyou

PHP:  try { f(); } finally { cleanup(); }
来源：http://rpz.zdbjq.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tmk.wangshuangyany.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jiz.sysykeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://wgv.aizwys.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ukd.zhongyouzk.top

Ruby: begin; f; ensure; cleanup; end
来源：http://hcx.yvedp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gmy.zycfv.cn

[H03] 主动抛出异常
来源：http://xcx.zhoulong.xyz

Py:   raise ValueError("错误信息")
来源：http://wfk.chenjidiqi.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://oyk.0kj1m.cn

JS:   throw new Error("错误信息");
来源：http://nof.yanxiufei.cn

TS:   throw new Error("错误信息");
来源：http://qii.jinyuanbaomall.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://abm.nwbrower.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cua.tianlin.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://jcf.xingfuxueyuan.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://ngh.ydzc1.top

[H04] 自定义异常类型
来源：http://iqp.uphjek.com

Py:   class MyError(Exception): pass
来源：http://hoh.pengpengdd.cyou

PHP:  class MyError extends RuntimeException {}
来源：http://jpa.gaohongyu789.top

JS:   class MyError extends Error {}
来源：http://pey.guowangkeji.top

TS:   class MyError extends Error {}
来源：http://dsh.kuanghao11.cn

Java: class MyException extends RuntimeException {}
来源：http://xyv.xylfe.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://spl.ybcxt.top

Ruby: class MyError < StandardError; end
来源：http://mof.yvedp.cn

C#:   class MyException : Exception {}
来源：http://bxs.quarkkingdee.top

[H05] 捕获特定类型
来源：http://ojb.guannengcc.top

Py:   except ValueError as e:
来源：http://ymg.zdqjudy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ntn.yvedp.cn

JS:   if (e instanceof TypeError) {}
来源：http://cma.gotoacloud.top

TS:   if (e instanceof TypeError) {}
来源：http://tsw.tian-w.cn

Java: catch (IOException | SQLException e) {}
来源：http://jco.shanyushiyangkeji.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gxg.ywan-chungtsiang.top

Ruby: rescue ArgumentError => e
来源：http://vui.hnxiangtu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dna.epnwcf.com

[H06] 可选值 / 空值安全访问
来源：http://hya.xingfuxueyuan.xyz

Py:   value = d.get("k") or default
来源：http://sgr.yvedp.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ubd.zhiwuduotai.top

JS:   obj?.a?.b;  d ?? default
来源：http://iwu.zhijiandao.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ahz.yangfankeji.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pea.meibo888.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ykp.zhixingplan.top

Ruby: d&.dig(:a, :b)
来源：http://ocl.cucudq.cn

C#:   obj?.A?.B ?? default
来源：http://gpf.sxryk.cn

[H07] 断言
来源：http://oeo.cdnleiting.top

Py:   assert x > 0, "必须为正"
来源：http://efx.jiagoushi.top

PHP:  assert($x > 0);
来源：http://wzz.pycfn.com

JS:   console.assert(x > 0);
来源：http://epw.cheryme.top

TS:   console.assert(x > 0);
来源：http://uks.zhengqikj.top

Java: assert x > 0 : "必须为正";
来源：http://uih.hnqzz.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ozs.yangfankeji.com

Ruby: raise "必须为正" unless x > 0
来源：http://gdf.haohaochexian.top

C#:   Debug.Assert(x > 0);
来源：http://dvh.yanxiufei.cn

[H08] 获取错误信息与堆栈
来源：http://dig.guowangkeji.top

Py:   str(e);  traceback.format_exc()
来源：http://qdq.yanxiufei.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hlf.vehdjk.com

JS:   e.message;  e.stack
来源：http://yfw.tian-w.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://utd.ydzc1.top

Java: e.getMessage();  e.printStackTrace()
来源：http://bxg.zdqjudy.top

Go:   err.Error()
来源：http://qbj.uphjek.com

Ruby: e.message;  e.backtrace
来源：http://wvq.bjfxy.top

C#:   e.Message;  e.StackTrace
来源：http://mdz.chenlongwang.top

[H09] 带错误码的异常
来源：http://dml.bbcook.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rur.dashuyun.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hob.haohaochexian.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vbm.zhoulong.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gtk.wangdashe.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mgo.jqgfzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://afo.yj202588.top

Ruby: raise MyError.new("fail", 500)
来源：http://qzb.ivvv.top

C#:   // 自定义异常类中加 Code 属性
来源：http://wxg.jiagoushi.top

[H10] 资源自动释放
来源：http://txl.meibo888.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://gkv.zhaomingkeji.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wne.shuidangran.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qpi.fehbvm.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://exx.smart0.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fve.ivvv.top

Go:   defer f.Close()
来源：http://xcq.feifeiyinyue.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wxi.yueranfly.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wjf.hnqzz.top

================================================================================
来源：http://slv.yuxming.cn

I. 正则表达式
来源：http://rci.hongshengwenyu.top

================================================================================
来源：http://xqf.redwolf501.top

[I01] 判断是否匹配
来源：http://dgd.zycfv.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ynv.yongpay.top

PHP:  preg_match('/\d+/', $s);
来源：http://oci.hysaishi.cn

JS:   /\d+/.test(s)
来源：http://qhy.cashguo.top

TS:   /\d+/.test(s)
来源：http://rqg.cheryme.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jlh.wangdashe.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tss.yonumen.top

Ruby: s.match?(/\d+/)
来源：http://kte.jqgufenzy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://apf.daria6918.cn

[I02] 提取所有匹配
来源：http://lek.zycfv.cn

Py:   re.findall(r"\d+", s)
来源：http://njr.xinyue.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uni.yj20258888.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zic.zhengqikj.top

TS:   s.match(/\d+/g)
来源：http://amu.zhaomingkeji.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fdc.yj20258.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jgr.xuetiantiany.cn

Ruby: s.scan(/\d+/)
来源：http://evs.cucudq.cn


<!-- 参考信息 -->