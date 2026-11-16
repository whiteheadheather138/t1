代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ase.xingfuxueyuan.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://afr.jqgufenzy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://isa.zhengqikj.top

[F08] 遍历目录
来源：http://whs.sxryk.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ghs.tanke756.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dwm.jqgufenzy.top

JS:   fs.readdirSync("dir")
来源：http://qgl.xingfuxueyuan.xyz

TS:   fs.readdirSync("dir")
来源：http://kep.iojbl.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fkq.hysaishi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bxg.jianghu66.top

Ruby: Dir.children("dir")
来源：http://gmd.andypj.xyz

C#:   Directory.GetFiles("dir")
来源：http://ync.52xcode.cn

[F09] 获取文件大小
来源：http://stu.0kj1m.cn

Py:   os.path.getsize("a.txt")
来源：http://isb.havefunace.top

PHP:  filesize("a.txt");
来源：http://gqz.bjfxy.top

JS:   fs.statSync("a.txt").size
来源：http://miz.cheryme.top

TS:   fs.statSync("a.txt").size
来源：http://hei.ctjpmb.com

Java: Files.size(Path.of("a.txt"))
来源：http://nos.tanke756.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zvl.xuetiantiany.cn

Ruby: File.size("a.txt")
来源：http://wox.cqqwz.cn

C#:   new FileInfo("a.txt").Length
来源：http://ymx.cdnleiting.top

[F10] 取文件扩展名 / 文件名
来源：http://qjx.redwolf501.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ocr.cheryme.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rpm.svipenyu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eym.tanke756.top

TS:   path.extname("a.txt")
来源：http://wdm.yonumen.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nyq.cashguo.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cfq.pycfn.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oee.kuanghao11.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pzb.aibaodan.cn

[F11] 复制与移动文件
来源：http://nfy.yongpay.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dkh.iojbl.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ksi.dianchejie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fjx.kuanghao11.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aqv.sysykeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tei.ybcxt.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lqe.uphjek.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://afh.gogol.net.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://khd.ppjwa.cn

[F12] CSV 读写
来源：http://bzm.chenzaomai.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fkx.ivvv.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hge.hywenlv.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://unh.ydzc1.top

TS:   // 同上
来源：http://afw.jianghu66.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ffp.fehbvm.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ypg.zhongyouzk.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jwy.gotoacloud.top

C#:   // 无内置：用 CsvHelper 库
来源：http://mhq.jiagoushi.top

================================================================================
来源：http://byw.hysaishi.cn

G. 面向对象
来源：http://cfm.hongshengwenyu.top

================================================================================
来源：http://qak.tanke756.top

[G01] 定义类
来源：http://lgz.tian-w.cn

Py:   class User: pass
来源：http://roe.haohaochexian.top

PHP:  class User {}
来源：http://qtg.ybcxt.top

JS:   class User {}
来源：http://kpu.birdmap.top

TS:   class User { name: string = ""; }
来源：http://xqg.cqqwz.cn

Java: class User {}
来源：http://yim.haohaochexian.top

Go:   type User struct { Name string }
来源：http://hgm.wangshuangyany.cn

Ruby: class User; end
来源：http://tyy.aizwys.cn

C#:   class User {}
来源：http://cdn.sweek.top

[G02] 构造函数
来源：http://yxy.daria6918.cn

Py:   def __init__(self, name): self.name = name
来源：http://xcu.hfpthk.cn

PHP:  public function __construct(public string $name) {}
来源：http://jfk.tanke756.top

JS:   constructor(name) { this.name = name; }
来源：http://wgq.gaohongyu789.top

TS:   constructor(public name: string) {}
来源：http://oup.dianchejie.cn

Java: User(String name) { this.name = name; }
来源：http://ogw.meibo888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bwd.ydzc1.top

Ruby: def initialize(name); @name = name; end
来源：http://zqg.cashguo.top

C#:   public User(string name) { Name = name; }
来源：http://cve.cqqwz.cn

[G03] 实例属性
来源：http://wvp.fehbvm.com

Py:   self.name = "x"
来源：http://hkc.sufxvd.cn

PHP:  public string $name = "x";
来源：http://txo.nanxinkj.top

JS:   this.name = "x";
来源：http://zyw.jlsjyb.cn

TS:   name: string = "x";
来源：http://iev.fzhhl.top

Java: private String name;
来源：http://yze.mhx1999.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://air.wangdashe.top

Ruby: @name = "x"
来源：http://adf.hnxiangtu.top

C#:   public string Name { get; set; } = "x";
来源：http://lhw.xziqi.cn

[G04] 定义方法
来源：http://xzf.jinqigufen.top

Py:   def greet(self): return self.name
来源：http://rwj.cashguo.top

PHP:  public function greet(): string { return $this->name; }
来源：http://jrv.gaohongyu789.top

JS:   greet() { return this.name; }
来源：http://hdc.shangyingyoupin.top

TS:   greet(): string { return this.name; }
来源：http://avn.jinghuilouyu.cn

Java: String greet() { return name; }
来源：http://lrz.tian-w.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://obp.cqqwz.cn

Ruby: def greet; @name; end
来源：http://gxv.yj20258888.top

C#:   public string Greet() => Name;
来源：http://zes.xylfe.cn

[G05] 继承
来源：http://pfd.guannengcc.top

Py:   class Admin(User): pass
来源：http://fev.cheryme.top

PHP:  class Admin extends User {}
来源：http://hbd.shzxlz.cn

JS:   class Admin extends User {}
来源：http://zxi.hywenlv.cn

TS:   class Admin extends User {}
来源：http://fxk.9152youxi.cn

Java: class Admin extends User {}
来源：http://eyj.bbcook.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xen.shanyushiyangtech.top

Ruby: class Admin < User; end
来源：http://gui.dianchejie.cn

C#:   class Admin : User {}
来源：http://lvz.sjlbkw.cn

[G06] 重写方法
来源：http://qlw.cqqwz.cn

Py:   def greet(self): return "admin"
来源：http://jbw.hywenlv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jae.jinghuilouyu.cn

JS:   greet() { return "admin"; }
来源：http://hyo.chenlongwang.top

TS:   greet(): string { return "admin"; }
来源：http://xcf.chenlongwang.top

Java: @Override String greet() { return "admin"; }
来源：http://qid.ehwqpu.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gqm.xingfuxueyuan.xyz

Ruby: def greet; "admin"; end
来源：http://arx.hcnkem.com

C#:   public override string Greet() => "admin";
来源：http://skw.nwbrower.top

[G07] 调用父类方法
来源：http://ifx.hfpthk.cn

Py:   super().greet()
来源：http://cpl.sjlbkw.cn

PHP:  parent::greet();
来源：http://iej.cqqwz.cn

JS:   super.greet();
来源：http://ncg.meibo888.top

TS:   super.greet();
来源：http://yac.jianghu66.top

Java: super.greet();
来源：http://jsr.fktsv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qyg.epnwcf.com

Ruby: super
来源：http://ujb.fanxiaobao.xyz

C#:   base.Greet();
来源：http://zke.hfpthk.cn

[G08] 静态方法与属性
来源：http://vqv.ctjpmb.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uud.tarul.cn

PHP:  public static function f() {}
来源：http://dbl.yj202588.top

JS:   static f() {}
来源：http://xwq.iojbl.cn

TS:   static f(): void {}
来源：http://mbi.dianchejie.cn

Java: static void f() {}
来源：http://gul.bjfxy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://fht.yj202588.top

Ruby: def self.f; end
来源：http://klz.yueranfly.top

C#:   public static void F() {}
来源：http://eys.bbcook.cn

[G09] 接口 / 抽象类
来源：http://uhx.yfazqb.com

Py:   from abc import ABC, abstractmethod
来源：http://xmj.fzhhl.top

PHP:  interface Shape { public function area(): float; }
来源：http://dge.wangshuangyany.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rda.ywan-chungtsiang.top

TS:   interface Shape { area(): number; }
来源：http://bcs.zdbjq.cn

Java: interface Shape { double area(); }
来源：http://gfm.hysaishi.cn

Go:   type Shape interface { Area() float64 }
来源：http://tui.gogol.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://izx.daria6918.cn

C#:   interface IShape { double Area(); }
来源：http://ddf.xinyue.icu

[G10] 访问控制
来源：http://ymt.meibo888.top

Py:   约定 _protected / __private（不强制）
来源：http://oow.yueranfly.top

PHP:  public / protected / private
来源：http://fig.iojbl.cn

JS:   #private 字段；其余公开
来源：http://reb.zhaomingkeji.xyz

TS:   public / protected / private
来源：http://brr.nanxinkj.top

Java: public / protected / private / 默认包级
来源：http://kfl.cheryme.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://chy.wangdashe.top

Ruby: public / protected / private
来源：http://nvu.nanxuanxn.top

C#:   public / protected / private / internal
来源：http://vrx.vehdjk.com

[G11] getter / setter
来源：http://yzm.hammf.cn

Py:   @property 与 @x.setter
来源：http://xwp.svipenyu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://myk.tarul.cn

JS:   get name() { return this._name; }
来源：http://zvs.ywan-chungtsiang.top

TS:   get name(): string { return this._name; }
来源：http://twi.jinghuilouyu.cn

Java: public String getName() { return name; }
来源：http://duq.xylfe.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dzh.mhx1999.top

Ruby: attr_accessor :name
来源：http://wxu.smart0.xyz

C#:   public string Name { get; set; }
来源：http://okw.hfpthk.cn

[G12] 对象转字符串
来源：http://tjc.fehbvm.com

Py:   def __str__(self): return self.name
来源：http://xoy.vehdjk.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://ixs.wangdashe.top

JS:   toString() { return this.name; }
来源：http://fzt.yanxiufei.cn

TS:   toString(): string { return this.name; }
来源：http://cth.bbcook.cn

Java: @Override public String toString() { return name; }
来源：http://ker.nanxinkj.top

Go:   func (u User) String() string { return u.Name }
来源：http://hif.yj20258888.top

Ruby: def to_s; @name; end
来源：http://ykw.tian-w.cn

C#:   public override string ToString() => Name;
来源：http://whl.nanxinkj.top

[G13] 判断对象类型
来源：http://mit.yangfankeji.com

Py:   isinstance(u, User)
来源：http://udm.wangdashe.top

PHP:  $u instanceof User
来源：http://ooj.ywan-chungtsiang.top

JS:   u instanceof User
来源：http://idg.fktsv.cn

TS:   u instanceof User
来源：http://squ.yangfankeji.com

Java: u instanceof User
来源：http://eqn.yfazqb.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://koz.chenlongwang.top

Ruby: u.is_a?(User)
来源：http://rom.pycfn.com

C#:   u is User
来源：http://qnk.uphjek.com

[G14] 数据类 / record
来源：http://rcp.vqdsnc.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vpu.jinqigfzy.top

PHP:  // 用 readonly 属性模拟
来源：http://dle.zhixingplan.top

JS:   // 无内置：普通类或对象字面量
来源：http://ufp.nanxinkj.top

TS:   type User = { name: string; age: number };
来源：http://jnb.tarul.cn

Java: record User(String name, int age) {}
来源：http://fkq.hysaishi.cn

Go:   type User struct { Name string; Age int }
来源：http://onw.bbcook.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://btv.tian-w.cn

C#:   record User(string Name, int Age);
来源：http://yaf.daxiang520.top

[G15] 枚举
来源：http://kou.0kj1m.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hdz.gaohongyu789.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://owd.hfpthk.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lsa.haohaochexian.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://urb.hfpthk.cn

Java: enum Color { RED, GREEN }
来源：http://gpp.yj20258.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://afe.feifeiyinyue.top

Ruby: Color = %i[red green].freeze
来源：http://tcq.gotoacloud.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wmg.pycfn.com

[G16] 对象转数组 / 字典
来源：http://dwx.zhixingplan.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qnk.c1oappe.top

PHP:  get_object_vars($obj);
来源：http://kuu.316326.xyz

JS:   Object.entries(obj)
来源：http://lto.zhixingplan.top

TS:   Object.entries(obj)
来源：http://tzg.mhx1999.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sfb.bbcook.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qra.yuxming.cn

Ruby: obj.instance_variables
来源：http://enn.dashuyun.cn

C#:   // 用反射或 System.Text.Json
来源：http://mfd.daria6918.cn

================================================================================
来源：http://bxh.cqqwz.cn

H. 异常与错误处理
来源：http://wte.jinqigfzy.top

================================================================================
来源：http://kyt.fengsongda.top

[H01] try / catch 基础
来源：http://cet.yongpay.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qoc.xylfe.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bss.cucudq.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vyn.316326.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pbb.yfazqb.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://urr.yvedp.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hhm.jinyuanbaomall.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bml.hnxiangtu.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qkk.jqgufenzy.top

[H02] finally / ensure 收尾
来源：http://rnw.cdnleiting.top

Py:   try: f()⏎finally: cleanup()
来源：http://wzl.zdbjq.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ote.9152youxi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lmu.jinqigufen.top

TS:   try { f(); } finally { cleanup(); }
来源：http://jun.jiagoushi.top

Java: try { f(); } finally { cleanup(); }
来源：http://dtc.fehbvm.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://mhg.ppjwa.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://oco.meibo888.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://rar.redwolf501.top

[H03] 主动抛出异常
来源：http://rjv.ctjpmb.com

Py:   raise ValueError("错误信息")
来源：http://wse.yuxming.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xks.birdmap.top

JS:   throw new Error("错误信息");
来源：http://fgs.sxryk.cn

TS:   throw new Error("错误信息");
来源：http://ozb.shanyushiyangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://izq.tianlin.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://szn.hongshengwenyu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ieu.smart0.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://wiz.zycfv.cn

[H04] 自定义异常类型
来源：http://ocj.c1oappe.top

Py:   class MyError(Exception): pass
来源：http://wkr.tian-w.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ioj.sjlbkw.cn

JS:   class MyError extends Error {}
来源：http://mrj.dianchejie.cn

TS:   class MyError extends Error {}
来源：http://mhd.shanyushiyangtech.top

Java: class MyException extends RuntimeException {}
来源：http://vwn.zhoulong.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yoo.smart0.xyz

Ruby: class MyError < StandardError; end
来源：http://nxe.iojbl.cn

C#:   class MyException : Exception {}
来源：http://ors.yueranfly.top

[H05] 捕获特定类型
来源：http://hdp.vqdsnc.cn

Py:   except ValueError as e:
来源：http://gbw.jianghu66.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qhg.gogol.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://dzi.shuidangran.top

TS:   if (e instanceof TypeError) {}
来源：http://wzn.gaohongyu789.top

Java: catch (IOException | SQLException e) {}
来源：http://aen.zhijiandao.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bfu.yonumen.top

Ruby: rescue ArgumentError => e
来源：http://vda.jianghu66.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qbw.guowangkeji.top

[H06] 可选值 / 空值安全访问
来源：http://jev.iojbl.cn

Py:   value = d.get("k") or default
来源：http://zum.hywenlv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://dcw.yj20258888.top

JS:   obj?.a?.b;  d ?? default
来源：http://bri.sufxvd.cn

TS:   obj?.a?.b;  d ?? default
来源：http://lbr.gotoacloud.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xop.zhiwuduotai.top

Go:   if v, ok := m["k"]; ok { }
来源：http://nsq.jinghuilouyu.cn

Ruby: d&.dig(:a, :b)
来源：http://qbk.kuanghao11.cn

C#:   obj?.A?.B ?? default
来源：http://uon.jinqigufen.top

[H07] 断言
来源：http://bau.xziqi.cn

Py:   assert x > 0, "必须为正"
来源：http://tgf.yuxming.cn

PHP:  assert($x > 0);
来源：http://aru.dianchejie.cn

JS:   console.assert(x > 0);
来源：http://ner.ehwqpu.com

TS:   console.assert(x > 0);
来源：http://eod.cucudq.cn

Java: assert x > 0 : "必须为正";
来源：http://ypz.daxiang520.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gjg.dianchejie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xrx.ywan-chungtsiang.top

C#:   Debug.Assert(x > 0);
来源：http://hmq.ehwqpu.com

[H08] 获取错误信息与堆栈
来源：http://ojf.tianlin.xyz

Py:   str(e);  traceback.format_exc()
来源：http://fcj.shanyushiyangkeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mxo.cashguo.top

JS:   e.message;  e.stack
来源：http://luy.ppjwa.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://nyj.xuetiantiany.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dgq.xuetiantiany.cn

Go:   err.Error()
来源：http://yoo.cheryme.top

Ruby: e.message;  e.backtrace
来源：http://zdt.nwbrower.top

C#:   e.Message;  e.StackTrace
来源：http://jcw.birdmap.top

[H09] 带错误码的异常
来源：http://xij.yfazqb.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wrv.ppjwa.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ack.jinyuanbaomall.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://slw.vqdsnc.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://suw.ybcxt.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dgc.xuetiantiany.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jrz.nwbrower.top

Ruby: raise MyError.new("fail", 500)
来源：http://fao.aizwys.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cif.kuanghao11.cn

[H10] 资源自动释放
来源：http://oif.pycfn.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://ijl.cucudq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qgt.hfpthk.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pwj.tarul.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bfs.ivvv.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://amu.havefunace.top

Go:   defer f.Close()
来源：http://rhm.redwolf501.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mow.tian-w.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zdm.gogol.net.cn

================================================================================
来源：http://ejc.svipenyu.cn

I. 正则表达式
来源：http://jri.snrcjt.cn

================================================================================
来源：http://bue.hysaishi.cn

[I01] 判断是否匹配
来源：http://elv.tarul.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cgp.zhijiandao.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hvo.fehbvm.com

JS:   /\d+/.test(s)
来源：http://xos.sjlbkw.cn

TS:   /\d+/.test(s)
来源：http://htb.quarkkingdee.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://aqc.yj20258.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ivi.nanxinkj.top

Ruby: s.match?(/\d+/)
来源：http://tfj.zhijiandao.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://faf.pengpengdd.cyou


<!-- 参考信息 -->