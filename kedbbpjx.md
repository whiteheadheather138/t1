代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vxo.birdmap.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mth.ehwqpu.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://owt.hesvh.cn

[F08] 遍历目录
来源：http://lxu.shanyushiyangkeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ash.yuxming.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nee.hfpthk.cn

JS:   fs.readdirSync("dir")
来源：http://ayd.hongshengwenyu.top

TS:   fs.readdirSync("dir")
来源：http://mjr.ehwqpu.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zly.hammf.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://aem.jianghu66.top

Ruby: Dir.children("dir")
来源：http://vxa.svipenyu.cn

C#:   Directory.GetFiles("dir")
来源：http://pbk.aibaodan.cn

[F09] 获取文件大小
来源：http://apy.cheryme.top

Py:   os.path.getsize("a.txt")
来源：http://zhf.ywan-chungtsiang.top

PHP:  filesize("a.txt");
来源：http://zvv.snrcjt.cn

JS:   fs.statSync("a.txt").size
来源：http://pll.chenjidiqi.icu

TS:   fs.statSync("a.txt").size
来源：http://kmp.haohaochexian.top

Java: Files.size(Path.of("a.txt"))
来源：http://lvh.aibaodan.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://avo.jinghuilouyu.cn

Ruby: File.size("a.txt")
来源：http://sci.cashguo.top

C#:   new FileInfo("a.txt").Length
来源：http://nok.yfazqb.com

[F10] 取文件扩展名 / 文件名
来源：http://hhp.zycfv.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nga.c1oappe.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ncu.jianghu66.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cyh.fengsongda.top

TS:   path.extname("a.txt")
来源：http://ysz.tarul.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qhz.xuanzx.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vfu.gaohongyu789.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yye.snrcjt.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xkk.epnwcf.com

[F11] 复制与移动文件
来源：http://lnv.fanxiaobao.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xuc.yj20258.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mvy.kuanghao11.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xwf.jinghuilouyu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kuh.jianghu66.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://eyv.chenjidiqi.icu

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zgg.yonumen.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://otl.haohaochexian.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fli.snrcjt.cn

[F12] CSV 读写
来源：http://ngu.xinyue.icu

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://axm.fktsv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dwv.quarkkingdee.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qbc.fanxiaobao.xyz

TS:   // 同上
来源：http://lrc.yfazqb.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zrc.vehdjk.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cjf.wangdashe.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://adu.xuetiantiany.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rbs.fengsongda.top

================================================================================
来源：http://pjc.hcnkem.com

G. 面向对象
来源：http://qcd.cashguo.top

================================================================================
来源：http://mez.hfpthk.cn

[G01] 定义类
来源：http://nsg.sysykeji.top

Py:   class User: pass
来源：http://din.ywan-chungtsiang.top

PHP:  class User {}
来源：http://ctd.xuanzx.com

JS:   class User {}
来源：http://cvy.haohaochexian.top

TS:   class User { name: string = ""; }
来源：http://dmx.jqgufenzy.top

Java: class User {}
来源：http://icd.daria6918.cn

Go:   type User struct { Name string }
来源：http://del.hnqzz.top

Ruby: class User; end
来源：http://ype.zhaomingkeji.xyz

C#:   class User {}
来源：http://ole.cucudq.cn

[G02] 构造函数
来源：http://bda.jianghu66.top

Py:   def __init__(self, name): self.name = name
来源：http://fxn.chenlongwang.top

PHP:  public function __construct(public string $name) {}
来源：http://wpw.gzhubu.top

JS:   constructor(name) { this.name = name; }
来源：http://fvb.ivvv.top

TS:   constructor(public name: string) {}
来源：http://zph.tanke756.top

Java: User(String name) { this.name = name; }
来源：http://coa.jqgfzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cih.fzhhl.top

Ruby: def initialize(name); @name = name; end
来源：http://qch.birdmap.top

C#:   public User(string name) { Name = name; }
来源：http://wod.meibo888.top

[G03] 实例属性
来源：http://yah.sjlbkw.cn

Py:   self.name = "x"
来源：http://fdu.ctjpmb.com

PHP:  public string $name = "x";
来源：http://xun.cheryme.top

JS:   this.name = "x";
来源：http://shk.xinyue.icu

TS:   name: string = "x";
来源：http://qju.guannengcc.top

Java: private String name;
来源：http://kmc.haohaochexian.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dhb.sysykeji.top

Ruby: @name = "x"
来源：http://ulm.yanxiufei.cn

C#:   public string Name { get; set; } = "x";
来源：http://ugh.wangshuangyany.cn

[G04] 定义方法
来源：http://mbo.fengsongda.top

Py:   def greet(self): return self.name
来源：http://usa.zdqjudy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://bpr.cqqwz.cn

JS:   greet() { return this.name; }
来源：http://phj.smart0.xyz

TS:   greet(): string { return this.name; }
来源：http://bbr.cucudq.cn

Java: String greet() { return name; }
来源：http://mis.zycfv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xah.birdmap.top

Ruby: def greet; @name; end
来源：http://cmz.zhixingplan.top

C#:   public string Greet() => Name;
来源：http://yjq.tianlin.xyz

[G05] 继承
来源：http://dnh.daria6918.cn

Py:   class Admin(User): pass
来源：http://vuq.hnxiangtu.top

PHP:  class Admin extends User {}
来源：http://tso.mhx1999.top

JS:   class Admin extends User {}
来源：http://blz.fktsv.cn

TS:   class Admin extends User {}
来源：http://abi.yuanzhike.top

Java: class Admin extends User {}
来源：http://btl.c1oappe.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://idf.jinghuilouyu.cn

Ruby: class Admin < User; end
来源：http://qbl.jianghu66.top

C#:   class Admin : User {}
来源：http://lat.cheryme.top

[G06] 重写方法
来源：http://uqq.zhengqikj.top

Py:   def greet(self): return "admin"
来源：http://ccn.svipenyu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jgy.yonumen.top

JS:   greet() { return "admin"; }
来源：http://dqg.hfpthk.cn

TS:   greet(): string { return "admin"; }
来源：http://ggd.zdqjudy.top

Java: @Override String greet() { return "admin"; }
来源：http://ezc.daria6918.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hen.nanxinkj.top

Ruby: def greet; "admin"; end
来源：http://oqj.0kj1m.cn

C#:   public override string Greet() => "admin";
来源：http://isd.jinghuilouyu.cn

[G07] 调用父类方法
来源：http://hwc.c1oappe.top

Py:   super().greet()
来源：http://wwr.meibo888.top

PHP:  parent::greet();
来源：http://yiq.dashuyun.cn

JS:   super.greet();
来源：http://gdv.sysykeji.top

TS:   super.greet();
来源：http://mrg.guowangkeji.top

Java: super.greet();
来源：http://wcm.zhongyouzk.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vlt.fzhhl.top

Ruby: super
来源：http://jkm.ppjwa.cn

C#:   base.Greet();
来源：http://cmn.chenzaomai.com

[G08] 静态方法与属性
来源：http://vxu.aibaodan.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lpg.zhengqikj.top

PHP:  public static function f() {}
来源：http://rmt.pengpengdd.cyou

JS:   static f() {}
来源：http://vem.gzhubu.top

TS:   static f(): void {}
来源：http://nmi.fehbvm.com

Java: static void f() {}
来源：http://dlw.snrcjt.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kxg.yongpay.top

Ruby: def self.f; end
来源：http://nvd.yongpay.top

C#:   public static void F() {}
来源：http://gqz.9152youxi.cn

[G09] 接口 / 抽象类
来源：http://fef.0kj1m.cn

Py:   from abc import ABC, abstractmethod
来源：http://lco.aibaodan.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jbb.jlsjyb.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://amf.haohaochexian.top

TS:   interface Shape { area(): number; }
来源：http://xbz.yj20258.top

Java: interface Shape { double area(); }
来源：http://gbd.aizwys.cn

Go:   type Shape interface { Area() float64 }
来源：http://ftr.yonumen.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://psn.mhx1999.top

C#:   interface IShape { double Area(); }
来源：http://zao.yuanzhike.top

[G10] 访问控制
来源：http://cqh.iojbl.cn

Py:   约定 _protected / __private（不强制）
来源：http://kww.hammf.cn

PHP:  public / protected / private
来源：http://nea.chenjidiqi.icu

JS:   #private 字段；其余公开
来源：http://cdd.ctjpmb.com

TS:   public / protected / private
来源：http://zam.gaohongyu789.top

Java: public / protected / private / 默认包级
来源：http://djy.hfpthk.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fbk.jinqigfzy.top

Ruby: public / protected / private
来源：http://myl.fanxiaobao.xyz

C#:   public / protected / private / internal
来源：http://kri.chenlongwang.top

[G11] getter / setter
来源：http://ogi.zhengqikj.top

Py:   @property 与 @x.setter
来源：http://twk.hnxiangtu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dwn.uphjek.com

JS:   get name() { return this._name; }
来源：http://lyy.bbcook.cn

TS:   get name(): string { return this._name; }
来源：http://nij.hnqzz.top

Java: public String getName() { return name; }
来源：http://rmi.shuidangran.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://qkc.zhaomingkeji.xyz

Ruby: attr_accessor :name
来源：http://zap.hnqzz.top

C#:   public string Name { get; set; }
来源：http://iwx.quarkkingdee.top

[G12] 对象转字符串
来源：http://avc.havefunace.top

Py:   def __str__(self): return self.name
来源：http://ayz.jqgfzy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://jnv.xylfe.cn

JS:   toString() { return this.name; }
来源：http://fyf.andypj.xyz

TS:   toString(): string { return this.name; }
来源：http://fqn.xuanzx.com

Java: @Override public String toString() { return name; }
来源：http://zqr.yonumen.top

Go:   func (u User) String() string { return u.Name }
来源：http://uea.hywenlv.cn

Ruby: def to_s; @name; end
来源：http://emk.jiagoushi.top

C#:   public override string ToString() => Name;
来源：http://bfe.hysaishi.cn

[G13] 判断对象类型
来源：http://rop.cdnleiting.top

Py:   isinstance(u, User)
来源：http://qft.hnxiangtu.top

PHP:  $u instanceof User
来源：http://yfu.epnwcf.com

JS:   u instanceof User
来源：http://rfl.cheryme.top

TS:   u instanceof User
来源：http://atm.zhaomingkeji.xyz

Java: u instanceof User
来源：http://xsx.uphjek.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://lmr.nwbrower.top

Ruby: u.is_a?(User)
来源：http://wxf.xziqi.cn

C#:   u is User
来源：http://dea.hammf.cn

[G14] 数据类 / record
来源：http://dav.cdnleiting.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rgg.dashuyun.cn

PHP:  // 用 readonly 属性模拟
来源：http://msw.yonumen.top

JS:   // 无内置：普通类或对象字面量
来源：http://ytn.jqgufenzy.top

TS:   type User = { name: string; age: number };
来源：http://vln.jinqigufen.top

Java: record User(String name, int age) {}
来源：http://wig.yonumen.top

Go:   type User struct { Name string; Age int }
来源：http://pvk.chenjidiqi.icu

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cwk.jianghu66.top

C#:   record User(string Name, int Age);
来源：http://krt.sxryk.cn

[G15] 枚举
来源：http://zig.yuanzhike.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://eot.ehwqpu.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://mxi.fehbvm.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zwu.shuidangran.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ajv.gaohongyu789.top

Java: enum Color { RED, GREEN }
来源：http://oiy.nanxuanxn.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zlz.andypj.xyz

Ruby: Color = %i[red green].freeze
来源：http://dkk.hnxiangtu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iku.pengpengdd.cyou

[G16] 对象转数组 / 字典
来源：http://ygf.ehwqpu.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hzi.cdnleiting.top

PHP:  get_object_vars($obj);
来源：http://wkz.ywan-chungtsiang.top

JS:   Object.entries(obj)
来源：http://xzb.hfpthk.cn

TS:   Object.entries(obj)
来源：http://hhr.0kj1m.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://olf.ydjk.org.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mmb.fanxiaobao.xyz

Ruby: obj.instance_variables
来源：http://wfr.gzhubu.top

C#:   // 用反射或 System.Text.Json
来源：http://vyz.epnwcf.com

================================================================================
来源：http://lhe.gotoacloud.top

H. 异常与错误处理
来源：http://aye.jinyuanbaomall.cn

================================================================================
来源：http://eav.shanyushiyangtech.top

[H01] try / catch 基础
来源：http://uep.zdbjq.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cyr.sxryk.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ttr.tanke756.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yjl.fanxiaobao.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gtz.fktsv.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jex.shangyingyoupin.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vay.gotoacloud.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pfx.316326.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yur.yvedp.cn

[H02] finally / ensure 收尾
来源：http://dou.aizwys.cn

Py:   try: f()⏎finally: cleanup()
来源：http://otm.c1oappe.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ozo.nanxuanxn.top

JS:   try { f(); } finally { cleanup(); }
来源：http://wyc.chenzaomai.com

TS:   try { f(); } finally { cleanup(); }
来源：http://wcp.wangshuangyany.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fwl.ybcxt.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://bdy.quarkkingdee.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ztt.fengsongda.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://vnk.sxryk.cn

[H03] 主动抛出异常
来源：http://mmu.ywan-chungtsiang.top

Py:   raise ValueError("错误信息")
来源：http://ukn.snrcjt.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dkq.gotoacloud.top

JS:   throw new Error("错误信息");
来源：http://iii.sysykeji.top

TS:   throw new Error("错误信息");
来源：http://nlb.nanxinkj.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://erc.fktsv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wyj.pycfn.com

Ruby: raise ArgumentError, "错误信息"
来源：http://kjq.yangfankeji.com

C#:   throw new ArgumentException("错误信息");
来源：http://icn.xinyue.icu

[H04] 自定义异常类型
来源：http://fqn.ppjwa.cn

Py:   class MyError(Exception): pass
来源：http://izv.meibo888.top

PHP:  class MyError extends RuntimeException {}
来源：http://kfb.fehbvm.com

JS:   class MyError extends Error {}
来源：http://zwt.dashuyun.cn

TS:   class MyError extends Error {}
来源：http://omh.quarkkingdee.top

Java: class MyException extends RuntimeException {}
来源：http://jma.yfazqb.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fzm.xuetiantiany.cn

Ruby: class MyError < StandardError; end
来源：http://fsi.iojbl.cn

C#:   class MyException : Exception {}
来源：http://tpn.ybcxt.top

[H05] 捕获特定类型
来源：http://yae.jqgfzy.top

Py:   except ValueError as e:
来源：http://zli.zhoulong.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://unu.nanxinkj.top

JS:   if (e instanceof TypeError) {}
来源：http://muq.hongshengwenyu.top

TS:   if (e instanceof TypeError) {}
来源：http://ual.xuetiantiany.cn

Java: catch (IOException | SQLException e) {}
来源：http://cwh.hfpthk.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ktq.ctjpmb.com

Ruby: rescue ArgumentError => e
来源：http://uyc.jinqigfzy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hwb.fktsv.cn

[H06] 可选值 / 空值安全访问
来源：http://rqc.yj20258888.top

Py:   value = d.get("k") or default
来源：http://esq.aizwys.cn

PHP:  $v = $d["k"] ?? null;
来源：http://how.yuxming.cn

JS:   obj?.a?.b;  d ?? default
来源：http://imd.sweek.top

TS:   obj?.a?.b;  d ?? default
来源：http://ztb.sweek.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://iyc.chenlongwang.top

Go:   if v, ok := m["k"]; ok { }
来源：http://kbx.tarul.cn

Ruby: d&.dig(:a, :b)
来源：http://ibn.jianghu66.top

C#:   obj?.A?.B ?? default
来源：http://cbl.sufxvd.cn

[H07] 断言
来源：http://ysg.shanyushiyangkeji.top

Py:   assert x > 0, "必须为正"
来源：http://ycs.mhx1999.top

PHP:  assert($x > 0);
来源：http://cjb.ctjpmb.com

JS:   console.assert(x > 0);
来源：http://uga.ydjk.org.cn

TS:   console.assert(x > 0);
来源：http://ekm.vehdjk.com

Java: assert x > 0 : "必须为正";
来源：http://epq.fehbvm.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zzi.sxryk.cn

Ruby: raise "必须为正" unless x > 0
来源：http://liy.hnqzz.top

C#:   Debug.Assert(x > 0);
来源：http://sut.epnwcf.com

[H08] 获取错误信息与堆栈
来源：http://dqu.andypj.xyz

Py:   str(e);  traceback.format_exc()
来源：http://hof.shuidangran.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pbp.jqgufenzy.top

JS:   e.message;  e.stack
来源：http://him.yueranfly.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://cwl.fehbvm.com

Java: e.getMessage();  e.printStackTrace()
来源：http://rpl.quarkkingdee.top

Go:   err.Error()
来源：http://ufc.hnqzz.top

Ruby: e.message;  e.backtrace
来源：http://tat.zdqjudy.top

C#:   e.Message;  e.StackTrace
来源：http://vin.ivvv.top

[H09] 带错误码的异常
来源：http://rik.xuetiantiany.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://glo.havefunace.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://tos.haohaochexian.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dyo.ywan-chungtsiang.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ulc.ppjwa.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rvs.gzhubu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zdu.hongshengwenyu.top

Ruby: raise MyError.new("fail", 500)
来源：http://rgc.zhaomingkeji.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://npo.svipenyu.cn

[H10] 资源自动释放
来源：http://qhx.guannengcc.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://alf.hammf.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ifd.yvedp.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ird.jianghu66.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dxq.zhijiandao.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ttl.ywan-chungtsiang.top

Go:   defer f.Close()
来源：http://nfo.yj20258.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tzi.yuanzhike.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vbj.tarul.cn

================================================================================
来源：http://kyn.hnqzz.top

I. 正则表达式
来源：http://lox.dianchejie.cn

================================================================================
来源：http://vmn.chenzaomai.com

[I01] 判断是否匹配
来源：http://bcb.jinqigufen.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fea.dianchejie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://coo.jyoumei.cn

JS:   /\d+/.test(s)
来源：http://tyr.ydzc1.top

TS:   /\d+/.test(s)
来源：http://gqg.gogol.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zto.sufxvd.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bmw.chenlongwang.top

Ruby: s.match?(/\d+/)
来源：http://pay.zhixingplan.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cew.zhaomingkeji.xyz


<!-- 参考信息 -->