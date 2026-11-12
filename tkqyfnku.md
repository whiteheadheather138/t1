代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://tpp.iojbl.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kly.aizwys.cn

JS:   fs.readdirSync("dir")
来源：http://ezj.tarul.cn

TS:   fs.readdirSync("dir")
来源：http://hyz.kuanghao11.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fib.havefunace.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://pgg.snrcjt.cn

Ruby: Dir.children("dir")
来源：http://fjd.jinghuilouyu.cn

C#:   Directory.GetFiles("dir")
来源：http://vkh.fanxiaobao.xyz

[F09] 获取文件大小
来源：http://new.jqgufenzy.top

Py:   os.path.getsize("a.txt")
来源：http://jin.cdnleiting.top

PHP:  filesize("a.txt");
来源：http://jxf.hfpthk.cn

JS:   fs.statSync("a.txt").size
来源：http://rjy.vqdsnc.cn

TS:   fs.statSync("a.txt").size
来源：http://ivy.cucudq.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fot.52xcode.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://aks.jyoumei.cn

Ruby: File.size("a.txt")
来源：http://rmh.dianchejie.cn

C#:   new FileInfo("a.txt").Length
来源：http://sup.yanxiufei.cn

[F10] 取文件扩展名 / 文件名
来源：http://jyl.pengpengdd.cyou

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://seu.cashguo.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pvw.tarul.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yet.gaohongyu789.top

TS:   path.extname("a.txt")
来源：http://bmk.chenjidiqi.icu

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jlq.jiagoushi.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dmb.9152youxi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vjo.jianghu66.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xdg.uphjek.com

[F11] 复制与移动文件
来源：http://heo.fengsongda.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qax.jinqigfzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pjf.zhijiandao.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aow.cucudq.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rgf.c1oappe.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uil.vehdjk.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qld.sxryk.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://svg.fzhhl.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rts.chenjidiqi.icu

[F12] CSV 读写
来源：http://kyx.kuanghao11.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fjy.tian-w.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://otm.hnqzz.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mei.0kj1m.cn

TS:   // 同上
来源：http://wbk.zhijiandao.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mls.fehbvm.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cmp.jinyuanbaomall.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ptt.tianlin.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://srt.jlsjyb.cn

================================================================================
来源：http://blm.yj20258.top

G. 面向对象
来源：http://rzh.hysaishi.cn

================================================================================
来源：http://jem.yuanzhike.top

[G01] 定义类
来源：http://rwe.chenzaomai.com

Py:   class User: pass
来源：http://kbx.hysaishi.cn

PHP:  class User {}
来源：http://rlq.gotoacloud.top

JS:   class User {}
来源：http://uuh.c1oappe.top

TS:   class User { name: string = ""; }
来源：http://ktm.jqgfzy.top

Java: class User {}
来源：http://hxv.cashguo.top

Go:   type User struct { Name string }
来源：http://ixu.ybcxt.top

Ruby: class User; end
来源：http://fzj.xingfuxueyuan.xyz

C#:   class User {}
来源：http://bcl.wangshuangyany.cn

[G02] 构造函数
来源：http://wro.jianghu66.top

Py:   def __init__(self, name): self.name = name
来源：http://mee.hfpthk.cn

PHP:  public function __construct(public string $name) {}
来源：http://cuc.ydzc1.top

JS:   constructor(name) { this.name = name; }
来源：http://ihy.52xcode.cn

TS:   constructor(public name: string) {}
来源：http://oez.chenjidiqi.icu

Java: User(String name) { this.name = name; }
来源：http://adn.zhengqikj.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rvg.tanke756.top

Ruby: def initialize(name); @name = name; end
来源：http://vln.fktsv.cn

C#:   public User(string name) { Name = name; }
来源：http://wbv.tian-w.cn

[G03] 实例属性
来源：http://ndd.ydjk.org.cn

Py:   self.name = "x"
来源：http://gwe.hysaishi.cn

PHP:  public string $name = "x";
来源：http://hss.ivvv.top

JS:   this.name = "x";
来源：http://wpt.shanyushiyangtech.top

TS:   name: string = "x";
来源：http://oqq.shanyushiyangkeji.top

Java: private String name;
来源：http://hlt.fanxiaobao.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://unj.zhiwuduotai.top

Ruby: @name = "x"
来源：http://fyu.cqqwz.cn

C#:   public string Name { get; set; } = "x";
来源：http://blr.tianlin.xyz

[G04] 定义方法
来源：http://dug.yuanzhike.top

Py:   def greet(self): return self.name
来源：http://vau.yuxming.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hyh.cucudq.cn

JS:   greet() { return this.name; }
来源：http://bdz.yuanzhike.top

TS:   greet(): string { return this.name; }
来源：http://dtd.ydzc1.top

Java: String greet() { return name; }
来源：http://lhu.fehbvm.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://dzu.hnqzz.top

Ruby: def greet; @name; end
来源：http://ufo.gogol.net.cn

C#:   public string Greet() => Name;
来源：http://mzp.fehbvm.com

[G05] 继承
来源：http://yly.hammf.cn

Py:   class Admin(User): pass
来源：http://joy.yanxiufei.cn

PHP:  class Admin extends User {}
来源：http://iya.cashguo.top

JS:   class Admin extends User {}
来源：http://sqs.hfpthk.cn

TS:   class Admin extends User {}
来源：http://lqu.haohaochexian.top

Java: class Admin extends User {}
来源：http://dat.xuanzx.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tsk.nanxuanxn.top

Ruby: class Admin < User; end
来源：http://ruh.ydzc1.top

C#:   class Admin : User {}
来源：http://thz.sxryk.cn

[G06] 重写方法
来源：http://rpd.andypj.xyz

Py:   def greet(self): return "admin"
来源：http://plx.birdmap.top

PHP:  public function greet(): string { return "admin"; }
来源：http://twq.shanyushiyangtech.top

JS:   greet() { return "admin"; }
来源：http://iii.uphjek.com

TS:   greet(): string { return "admin"; }
来源：http://fth.gogol.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://fpq.jlsjyb.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fzo.cashguo.top

Ruby: def greet; "admin"; end
来源：http://khe.yj20258888.top

C#:   public override string Greet() => "admin";
来源：http://ykb.vqdsnc.cn

[G07] 调用父类方法
来源：http://zvz.yfazqb.com

Py:   super().greet()
来源：http://rku.tian-w.cn

PHP:  parent::greet();
来源：http://tsc.yvedp.cn

JS:   super.greet();
来源：http://myh.andypj.xyz

TS:   super.greet();
来源：http://rss.zhengqikj.top

Java: super.greet();
来源：http://ytd.chenzaomai.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cuq.jiagoushi.top

Ruby: super
来源：http://vsi.daxiang520.top

C#:   base.Greet();
来源：http://fuk.snrcjt.cn

[G08] 静态方法与属性
来源：http://ieh.jqgufenzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blv.yj202588.top

PHP:  public static function f() {}
来源：http://odt.vehdjk.com

JS:   static f() {}
来源：http://dny.gogol.net.cn

TS:   static f(): void {}
来源：http://ell.daria6918.cn

Java: static void f() {}
来源：http://hjs.yueranfly.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ufy.chenzaomai.com

Ruby: def self.f; end
来源：http://oan.jianghu66.top

C#:   public static void F() {}
来源：http://ywg.zdqjudy.top

[G09] 接口 / 抽象类
来源：http://exq.yonumen.top

Py:   from abc import ABC, abstractmethod
来源：http://fhb.yuanzhike.top

PHP:  interface Shape { public function area(): float; }
来源：http://gav.xinyue.icu

JS:   // 无接口：靠约定或 JSDoc
来源：http://igz.jinqigufen.top

TS:   interface Shape { area(): number; }
来源：http://uzx.0kj1m.cn

Java: interface Shape { double area(); }
来源：http://kro.wangdashe.top

Go:   type Shape interface { Area() float64 }
来源：http://igr.zhixingplan.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wix.tianlin.xyz

C#:   interface IShape { double Area(); }
来源：http://odz.dianchejie.cn

[G10] 访问控制
来源：http://zyg.zhiwuduotai.top

Py:   约定 _protected / __private（不强制）
来源：http://dll.zhongyouzk.top

PHP:  public / protected / private
来源：http://iuy.yueranfly.top

JS:   #private 字段；其余公开
来源：http://jut.0kj1m.cn

TS:   public / protected / private
来源：http://ffh.wangshuangyany.cn

Java: public / protected / private / 默认包级
来源：http://ryc.shzxlz.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://sjr.xuanzx.com

Ruby: public / protected / private
来源：http://ybq.redwolf501.top

C#:   public / protected / private / internal
来源：http://dav.cucudq.cn

[G11] getter / setter
来源：http://ggt.jianghu66.top

Py:   @property 与 @x.setter
来源：http://agv.andypj.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://bih.fanxiaobao.xyz

JS:   get name() { return this._name; }
来源：http://dvj.xuanzx.com

TS:   get name(): string { return this._name; }
来源：http://xyu.hysaishi.cn

Java: public String getName() { return name; }
来源：http://zrn.cdnleiting.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://nzr.yangfankeji.com

Ruby: attr_accessor :name
来源：http://jkq.nanxinkj.top

C#:   public string Name { get; set; }
来源：http://umc.fzhhl.top

[G12] 对象转字符串
来源：http://jqe.hnxiangtu.top

Py:   def __str__(self): return self.name
来源：http://suz.jqgufenzy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://pfn.ybcxt.top

JS:   toString() { return this.name; }
来源：http://esz.shzxlz.cn

TS:   toString(): string { return this.name; }
来源：http://kvq.yvedp.cn

Java: @Override public String toString() { return name; }
来源：http://vyn.yj20258.top

Go:   func (u User) String() string { return u.Name }
来源：http://aly.chenzaomai.com

Ruby: def to_s; @name; end
来源：http://mxs.tianlin.xyz

C#:   public override string ToString() => Name;
来源：http://bay.yuxming.cn

[G13] 判断对象类型
来源：http://yzt.tianlin.xyz

Py:   isinstance(u, User)
来源：http://hfy.yonumen.top

PHP:  $u instanceof User
来源：http://dne.zhoulong.xyz

JS:   u instanceof User
来源：http://ien.hysaishi.cn

TS:   u instanceof User
来源：http://wcq.zhijiandao.cn

Java: u instanceof User
来源：http://ffr.ywan-chungtsiang.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://uwp.52xcode.cn

Ruby: u.is_a?(User)
来源：http://tmi.sxryk.cn

C#:   u is User
来源：http://kim.aizwys.cn

[G14] 数据类 / record
来源：http://yyv.kuanghao11.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mpe.chenzaomai.com

PHP:  // 用 readonly 属性模拟
来源：http://fli.yj20258888.top

JS:   // 无内置：普通类或对象字面量
来源：http://urc.hnxiangtu.top

TS:   type User = { name: string; age: number };
来源：http://dtb.cashguo.top

Java: record User(String name, int age) {}
来源：http://kln.yanxiufei.cn

Go:   type User struct { Name string; Age int }
来源：http://jce.9152youxi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wkn.gaohongyu789.top

C#:   record User(string Name, int Age);
来源：http://opc.sufxvd.cn

[G15] 枚举
来源：http://qrd.yanxiufei.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qol.zycfv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://yog.9152youxi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hcu.shanyushiyangtech.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tjj.hnqzz.top

Java: enum Color { RED, GREEN }
来源：http://gph.daxiang520.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ywe.9152youxi.cn

Ruby: Color = %i[red green].freeze
来源：http://lxn.epnwcf.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jbf.yueranfly.top

[G16] 对象转数组 / 字典
来源：http://ebi.gzhubu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sxp.haohaochexian.top

PHP:  get_object_vars($obj);
来源：http://wnj.quarkkingdee.top

JS:   Object.entries(obj)
来源：http://ekq.zycfv.cn

TS:   Object.entries(obj)
来源：http://vwl.ybcxt.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://emv.xuetiantiany.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ced.hcnkem.com

Ruby: obj.instance_variables
来源：http://cqb.iojbl.cn

C#:   // 用反射或 System.Text.Json
来源：http://fsv.tian-w.cn

================================================================================
来源：http://cmm.zycfv.cn

H. 异常与错误处理
来源：http://jbu.jiagoushi.top

================================================================================
来源：http://oqx.shzxlz.cn

[H01] try / catch 基础
来源：http://hrq.tian-w.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qia.smart0.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qzj.zhiwuduotai.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kdm.ydjk.org.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lbq.pengpengdd.cyou

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nqx.fktsv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uxp.havefunace.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lvk.hesvh.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kdg.zhongyouzk.top

[H02] finally / ensure 收尾
来源：http://mny.tanke756.top

Py:   try: f()⏎finally: cleanup()
来源：http://tax.smart0.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://cpu.mhx1999.top

JS:   try { f(); } finally { cleanup(); }
来源：http://swh.birdmap.top

TS:   try { f(); } finally { cleanup(); }
来源：http://cfk.shanyushiyangtech.top

Java: try { f(); } finally { cleanup(); }
来源：http://vft.gotoacloud.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://izl.yonumen.top

Ruby: begin; f; ensure; cleanup; end
来源：http://zic.yangfankeji.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://dbw.nanxinkj.top

[H03] 主动抛出异常
来源：http://hkf.xingfuxueyuan.xyz

Py:   raise ValueError("错误信息")
来源：http://xvz.snrcjt.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vll.snrcjt.cn

JS:   throw new Error("错误信息");
来源：http://jnn.yanxiufei.cn

TS:   throw new Error("错误信息");
来源：http://wea.tarul.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yyd.sufxvd.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tml.vehdjk.com

Ruby: raise ArgumentError, "错误信息"
来源：http://lnb.52xcode.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fbg.jyoumei.cn

[H04] 自定义异常类型
来源：http://hjb.xziqi.cn

Py:   class MyError(Exception): pass
来源：http://ibk.kuanghao11.cn

PHP:  class MyError extends RuntimeException {}
来源：http://lsr.fktsv.cn

JS:   class MyError extends Error {}
来源：http://lry.ivvv.top

TS:   class MyError extends Error {}
来源：http://dfk.cheryme.top

Java: class MyException extends RuntimeException {}
来源：http://met.shuidangran.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wbv.ctjpmb.com

Ruby: class MyError < StandardError; end
来源：http://tpr.xziqi.cn

C#:   class MyException : Exception {}
来源：http://yvc.52xcode.cn

[H05] 捕获特定类型
来源：http://brg.iojbl.cn

Py:   except ValueError as e:
来源：http://bjb.yuxming.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kue.jinghuilouyu.cn

JS:   if (e instanceof TypeError) {}
来源：http://gth.zhijiandao.cn

TS:   if (e instanceof TypeError) {}
来源：http://wyk.jinghuilouyu.cn

Java: catch (IOException | SQLException e) {}
来源：http://jgq.xuetiantiany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vyp.pengpengdd.cyou

Ruby: rescue ArgumentError => e
来源：http://ksj.andypj.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bcf.fengsongda.top

[H06] 可选值 / 空值安全访问
来源：http://fxp.ydjk.org.cn

Py:   value = d.get("k") or default
来源：http://low.jqgufenzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://zlu.52xcode.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zzu.zdbjq.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cxm.zycfv.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vgq.sysykeji.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ylx.shangyingyoupin.top

Ruby: d&.dig(:a, :b)
来源：http://cbi.epnwcf.com

C#:   obj?.A?.B ?? default
来源：http://mhz.meibo888.top

[H07] 断言
来源：http://mbu.ehwqpu.com

Py:   assert x > 0, "必须为正"
来源：http://xqt.jyoumei.cn

PHP:  assert($x > 0);
来源：http://kis.yonumen.top

JS:   console.assert(x > 0);
来源：http://sgw.yfazqb.com

TS:   console.assert(x > 0);
来源：http://ffa.yanxiufei.cn

Java: assert x > 0 : "必须为正";
来源：http://etd.gotoacloud.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ovr.zhengqikj.top

Ruby: raise "必须为正" unless x > 0
来源：http://yxr.shuidangran.top

C#:   Debug.Assert(x > 0);
来源：http://oef.ehwqpu.com

[H08] 获取错误信息与堆栈
来源：http://rpg.sjlbkw.cn

Py:   str(e);  traceback.format_exc()
来源：http://toj.jqgfzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cdh.zhaomingkeji.xyz

JS:   e.message;  e.stack
来源：http://dpc.sweek.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://iwt.hfpthk.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hbl.gaohongyu789.top

Go:   err.Error()
来源：http://jkh.jlsjyb.cn

Ruby: e.message;  e.backtrace
来源：http://syc.sxryk.cn

C#:   e.Message;  e.StackTrace
来源：http://uxv.hnxiangtu.top

[H09] 带错误码的异常
来源：http://lsf.shangyingyoupin.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ghw.dianchejie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://tur.tarul.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ioz.sufxvd.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://iar.mhx1999.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dmh.sweek.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kds.aizwys.cn

Ruby: raise MyError.new("fail", 500)
来源：http://aok.xylfe.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hcr.havefunace.top

[H10] 资源自动释放
来源：http://ubp.shangyingyoupin.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ksc.xylfe.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ute.pengpengdd.cyou

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kpb.zhiwuduotai.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tsu.gaohongyu789.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dgt.zhengqikj.top

Go:   defer f.Close()
来源：http://mkc.yonumen.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tzg.ywan-chungtsiang.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ktk.hnqzz.top

================================================================================
来源：http://hbj.tianlin.xyz

I. 正则表达式
来源：http://qyn.fktsv.cn

================================================================================
来源：http://aoh.jinyuanbaomall.cn

[I01] 判断是否匹配
来源：http://fbk.cashguo.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dpk.xingfuxueyuan.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://fjv.yvedp.cn

JS:   /\d+/.test(s)
来源：http://mlq.c1oappe.top

TS:   /\d+/.test(s)
来源：http://zwd.xylfe.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ffs.316326.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uzb.jinghuilouyu.cn

Ruby: s.match?(/\d+/)
来源：http://usc.xuanzx.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://imk.jinghuilouyu.cn

[I02] 提取所有匹配
来源：http://mym.shanyushiyangtech.top

Py:   re.findall(r"\d+", s)
来源：http://xoe.meibo888.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://aue.jinghuilouyu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ehm.meibo888.top


<!-- 参考信息 -->