代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ugp.yuanzhike.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://anf.nanxuanxn.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ape.yuxming.cn

[F08] 遍历目录
来源：http://psv.316326.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://eyt.fehbvm.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://iwx.mhx1999.top

JS:   fs.readdirSync("dir")
来源：http://wwo.vehdjk.com

TS:   fs.readdirSync("dir")
来源：http://nbo.yonumen.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://edr.epnwcf.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://syp.iojbl.cn

Ruby: Dir.children("dir")
来源：http://dbf.feifeiyinyue.top

C#:   Directory.GetFiles("dir")
来源：http://jkh.hesvh.cn

[F09] 获取文件大小
来源：http://jdh.aizwys.cn

Py:   os.path.getsize("a.txt")
来源：http://ukp.xuetiantiany.cn

PHP:  filesize("a.txt");
来源：http://esg.xuanzx.com

JS:   fs.statSync("a.txt").size
来源：http://ksh.yj20258.top

TS:   fs.statSync("a.txt").size
来源：http://akt.jyoumei.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lpa.guannengcc.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uqn.guannengcc.top

Ruby: File.size("a.txt")
来源：http://bbx.ctjpmb.com

C#:   new FileInfo("a.txt").Length
来源：http://qly.nanxinkj.top

[F10] 取文件扩展名 / 文件名
来源：http://nls.nwbrower.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bvi.jianghu66.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://waz.havefunace.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fnu.hammf.cn

TS:   path.extname("a.txt")
来源：http://fel.fengsongda.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pja.epnwcf.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nwz.zdqjudy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://isr.kuanghao11.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rxw.fzhhl.top

[F11] 复制与移动文件
来源：http://sny.zdbjq.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://azk.sxryk.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sse.0kj1m.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nnk.yuanzhike.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://khk.nanxuanxn.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kht.zhongyouzk.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pvq.sxryk.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yiu.quarkkingdee.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://czc.aizwys.cn

[F12] CSV 读写
来源：http://yjo.sufxvd.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://maj.ehwqpu.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ung.wangshuangyany.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bpk.shanyushiyangtech.top

TS:   // 同上
来源：http://ykf.hammf.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tzm.vehdjk.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://aro.fengsongda.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://amb.gzhubu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://kip.jqgufenzy.top

================================================================================
来源：http://wjq.shzxlz.cn

G. 面向对象
来源：http://oms.jinqigfzy.top

================================================================================
来源：http://ayi.zhongyouzk.top

[G01] 定义类
来源：http://tfv.ctjpmb.com

Py:   class User: pass
来源：http://mif.sjlbkw.cn

PHP:  class User {}
来源：http://noo.xuanzx.com

JS:   class User {}
来源：http://hvx.vqdsnc.cn

TS:   class User { name: string = ""; }
来源：http://guu.gotoacloud.top

Java: class User {}
来源：http://pnk.xinyue.icu

Go:   type User struct { Name string }
来源：http://cos.xuanzx.com

Ruby: class User; end
来源：http://qfu.nanxuanxn.top

C#:   class User {}
来源：http://zwp.andypj.xyz

[G02] 构造函数
来源：http://gkf.yfazqb.com

Py:   def __init__(self, name): self.name = name
来源：http://yyo.iojbl.cn

PHP:  public function __construct(public string $name) {}
来源：http://fbs.ivvv.top

JS:   constructor(name) { this.name = name; }
来源：http://rax.shuidangran.top

TS:   constructor(public name: string) {}
来源：http://lkz.sufxvd.cn

Java: User(String name) { this.name = name; }
来源：http://jzg.svipenyu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jmr.vqdsnc.cn

Ruby: def initialize(name); @name = name; end
来源：http://waj.zhongyouzk.top

C#:   public User(string name) { Name = name; }
来源：http://wgs.sxryk.cn

[G03] 实例属性
来源：http://zpx.9152youxi.cn

Py:   self.name = "x"
来源：http://nww.snrcjt.cn

PHP:  public string $name = "x";
来源：http://urv.jqgufenzy.top

JS:   this.name = "x";
来源：http://fvv.ctjpmb.com

TS:   name: string = "x";
来源：http://vvm.yonumen.top

Java: private String name;
来源：http://sbr.smart0.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://syv.svipenyu.cn

Ruby: @name = "x"
来源：http://bxv.0kj1m.cn

C#:   public string Name { get; set; } = "x";
来源：http://glo.hcnkem.com

[G04] 定义方法
来源：http://yiu.tarul.cn

Py:   def greet(self): return self.name
来源：http://sdh.hfpthk.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kov.meibo888.top

JS:   greet() { return this.name; }
来源：http://bsz.sxryk.cn

TS:   greet(): string { return this.name; }
来源：http://ipa.zhoulong.xyz

Java: String greet() { return name; }
来源：http://hsw.fengsongda.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://axt.cucudq.cn

Ruby: def greet; @name; end
来源：http://vko.jianghu66.top

C#:   public string Greet() => Name;
来源：http://dal.cdnleiting.top

[G05] 继承
来源：http://hoz.kuanghao11.cn

Py:   class Admin(User): pass
来源：http://xoq.jyoumei.cn

PHP:  class Admin extends User {}
来源：http://der.kuanghao11.cn

JS:   class Admin extends User {}
来源：http://ggr.nanxuanxn.top

TS:   class Admin extends User {}
来源：http://hhq.ydjk.org.cn

Java: class Admin extends User {}
来源：http://ith.zycfv.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hek.ydzc1.top

Ruby: class Admin < User; end
来源：http://aok.0kj1m.cn

C#:   class Admin : User {}
来源：http://box.hysaishi.cn

[G06] 重写方法
来源：http://fxy.chenzaomai.com

Py:   def greet(self): return "admin"
来源：http://bwg.yanxiufei.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://eym.bbcook.cn

JS:   greet() { return "admin"; }
来源：http://ngh.daria6918.cn

TS:   greet(): string { return "admin"; }
来源：http://ici.pycfn.com

Java: @Override String greet() { return "admin"; }
来源：http://tbm.shuidangran.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cmm.daxiang520.top

Ruby: def greet; "admin"; end
来源：http://ujd.zhoulong.xyz

C#:   public override string Greet() => "admin";
来源：http://nzd.nanxuanxn.top

[G07] 调用父类方法
来源：http://eve.svipenyu.cn

Py:   super().greet()
来源：http://xcm.bbcook.cn

PHP:  parent::greet();
来源：http://vxe.meibo888.top

JS:   super.greet();
来源：http://bdw.vqdsnc.cn

TS:   super.greet();
来源：http://iph.jinqigfzy.top

Java: super.greet();
来源：http://fzw.yanxiufei.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zve.cheryme.top

Ruby: super
来源：http://hfo.316326.xyz

C#:   base.Greet();
来源：http://pfk.fzhhl.top

[G08] 静态方法与属性
来源：http://zfp.hammf.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hbg.jiagoushi.top

PHP:  public static function f() {}
来源：http://hew.jinyuanbaomall.cn

JS:   static f() {}
来源：http://vjk.fanxiaobao.xyz

TS:   static f(): void {}
来源：http://lcl.sysykeji.top

Java: static void f() {}
来源：http://vmn.yangfankeji.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://mlk.svipenyu.cn

Ruby: def self.f; end
来源：http://xvq.hammf.cn

C#:   public static void F() {}
来源：http://scl.zhijiandao.cn

[G09] 接口 / 抽象类
来源：http://axp.zhixingplan.top

Py:   from abc import ABC, abstractmethod
来源：http://jka.yfazqb.com

PHP:  interface Shape { public function area(): float; }
来源：http://eqi.hnqzz.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ory.wangdashe.top

TS:   interface Shape { area(): number; }
来源：http://esb.ivvv.top

Java: interface Shape { double area(); }
来源：http://wwg.shzxlz.cn

Go:   type Shape interface { Area() float64 }
来源：http://lal.yuxming.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rpi.ybcxt.top

C#:   interface IShape { double Area(); }
来源：http://unp.yj20258888.top

[G10] 访问控制
来源：http://wip.bjfxy.top

Py:   约定 _protected / __private（不强制）
来源：http://rgt.zhiwuduotai.top

PHP:  public / protected / private
来源：http://mxw.jianghu66.top

JS:   #private 字段；其余公开
来源：http://lsp.wangshuangyany.cn

TS:   public / protected / private
来源：http://avy.yongpay.top

Java: public / protected / private / 默认包级
来源：http://ens.yanxiufei.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gju.birdmap.top

Ruby: public / protected / private
来源：http://mfg.hnxiangtu.top

C#:   public / protected / private / internal
来源：http://vpk.havefunace.top

[G11] getter / setter
来源：http://ryp.zhengqikj.top

Py:   @property 与 @x.setter
来源：http://ypc.sxryk.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zjs.ctjpmb.com

JS:   get name() { return this._name; }
来源：http://zbj.yueranfly.top

TS:   get name(): string { return this._name; }
来源：http://yfi.zdbjq.cn

Java: public String getName() { return name; }
来源：http://opv.xuanzx.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://mhp.cqqwz.cn

Ruby: attr_accessor :name
来源：http://bpr.sysykeji.top

C#:   public string Name { get; set; }
来源：http://mxt.kuanghao11.cn

[G12] 对象转字符串
来源：http://bqr.hywenlv.cn

Py:   def __str__(self): return self.name
来源：http://yqt.shanyushiyangkeji.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://vwn.xingfuxueyuan.xyz

JS:   toString() { return this.name; }
来源：http://tvb.yuanzhike.top

TS:   toString(): string { return this.name; }
来源：http://nfk.pengpengdd.cyou

Java: @Override public String toString() { return name; }
来源：http://rrs.52xcode.cn

Go:   func (u User) String() string { return u.Name }
来源：http://lhc.yuxming.cn

Ruby: def to_s; @name; end
来源：http://jxv.xziqi.cn

C#:   public override string ToString() => Name;
来源：http://ydi.dashuyun.cn

[G13] 判断对象类型
来源：http://zdi.shuidangran.top

Py:   isinstance(u, User)
来源：http://rww.zdbjq.cn

PHP:  $u instanceof User
来源：http://gav.zhiwuduotai.top

JS:   u instanceof User
来源：http://vaf.sjlbkw.cn

TS:   u instanceof User
来源：http://gun.hywenlv.cn

Java: u instanceof User
来源：http://zau.daria6918.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://iqu.tian-w.cn

Ruby: u.is_a?(User)
来源：http://tce.hnqzz.top

C#:   u is User
来源：http://gtj.chenzaomai.com

[G14] 数据类 / record
来源：http://dpx.uphjek.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://has.dianchejie.cn

PHP:  // 用 readonly 属性模拟
来源：http://roc.kuanghao11.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wgu.c1oappe.top

TS:   type User = { name: string; age: number };
来源：http://uvi.hnxiangtu.top

Java: record User(String name, int age) {}
来源：http://dna.daria6918.cn

Go:   type User struct { Name string; Age int }
来源：http://naf.chenzaomai.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qqi.yonumen.top

C#:   record User(string Name, int Age);
来源：http://tyb.pycfn.com

[G15] 枚举
来源：http://vjf.aizwys.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jiq.dashuyun.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://cjx.cqqwz.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jvd.c1oappe.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yeh.birdmap.top

Java: enum Color { RED, GREEN }
来源：http://hur.hywenlv.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pjt.shuidangran.top

Ruby: Color = %i[red green].freeze
来源：http://jtq.yj20258.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qnl.aizwys.cn

[G16] 对象转数组 / 字典
来源：http://zmt.vqdsnc.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vbw.yvedp.cn

PHP:  get_object_vars($obj);
来源：http://cqj.jlsjyb.cn

JS:   Object.entries(obj)
来源：http://cja.c1oappe.top

TS:   Object.entries(obj)
来源：http://hmh.fehbvm.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://olw.aibaodan.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mgr.sjlbkw.cn

Ruby: obj.instance_variables
来源：http://klu.zhoulong.xyz

C#:   // 用反射或 System.Text.Json
来源：http://mpk.nwbrower.top

================================================================================
来源：http://son.nanxinkj.top

H. 异常与错误处理
来源：http://ext.iojbl.cn

================================================================================
来源：http://vop.daxiang520.top

[H01] try / catch 基础
来源：http://uhr.jqgfzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tka.fzhhl.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bbl.wangshuangyany.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ncg.ivvv.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qvk.daxiang520.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://quz.hywenlv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dug.gzhubu.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wrd.dashuyun.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wtz.guowangkeji.top

[H02] finally / ensure 收尾
来源：http://oui.jinyuanbaomall.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vyy.tanke756.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://pzw.ybcxt.top

JS:   try { f(); } finally { cleanup(); }
来源：http://shr.fktsv.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gzr.ivvv.top

Java: try { f(); } finally { cleanup(); }
来源：http://laz.cheryme.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://lei.zycfv.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://uws.sufxvd.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dta.gogol.net.cn

[H03] 主动抛出异常
来源：http://kbs.guowangkeji.top

Py:   raise ValueError("错误信息")
来源：http://pjx.tianlin.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xfk.guowangkeji.top

JS:   throw new Error("错误信息");
来源：http://fai.hammf.cn

TS:   throw new Error("错误信息");
来源：http://bmn.snrcjt.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://btn.fehbvm.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sfo.c1oappe.top

Ruby: raise ArgumentError, "错误信息"
来源：http://fhm.ydzc1.top

C#:   throw new ArgumentException("错误信息");
来源：http://qmz.fktsv.cn

[H04] 自定义异常类型
来源：http://vli.feifeiyinyue.top

Py:   class MyError(Exception): pass
来源：http://ysp.chenzaomai.com

PHP:  class MyError extends RuntimeException {}
来源：http://ahc.andypj.xyz

JS:   class MyError extends Error {}
来源：http://pxl.dashuyun.cn

TS:   class MyError extends Error {}
来源：http://wej.jinqigufen.top

Java: class MyException extends RuntimeException {}
来源：http://oav.bbcook.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vln.aizwys.cn

Ruby: class MyError < StandardError; end
来源：http://lfy.wangdashe.top

C#:   class MyException : Exception {}
来源：http://dpe.haohaochexian.top

[H05] 捕获特定类型
来源：http://xfg.hysaishi.cn

Py:   except ValueError as e:
来源：http://hdv.hnxiangtu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://umx.shanyushiyangkeji.top

JS:   if (e instanceof TypeError) {}
来源：http://sdg.0kj1m.cn

TS:   if (e instanceof TypeError) {}
来源：http://ssv.mhx1999.top

Java: catch (IOException | SQLException e) {}
来源：http://puv.fengsongda.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fyq.svipenyu.cn

Ruby: rescue ArgumentError => e
来源：http://pmn.ctjpmb.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yab.jlsjyb.cn

[H06] 可选值 / 空值安全访问
来源：http://cqx.0kj1m.cn

Py:   value = d.get("k") or default
来源：http://myz.tian-w.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kxc.chenlongwang.top

JS:   obj?.a?.b;  d ?? default
来源：http://eem.daria6918.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cxt.feifeiyinyue.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nby.meibo888.top

Go:   if v, ok := m["k"]; ok { }
来源：http://bsx.guannengcc.top

Ruby: d&.dig(:a, :b)
来源：http://yvn.hfpthk.cn

C#:   obj?.A?.B ?? default
来源：http://rfl.hywenlv.cn

[H07] 断言
来源：http://lpp.pycfn.com

Py:   assert x > 0, "必须为正"
来源：http://qrh.cucudq.cn

PHP:  assert($x > 0);
来源：http://ocu.cheryme.top

JS:   console.assert(x > 0);
来源：http://dwo.wangdashe.top

TS:   console.assert(x > 0);
来源：http://xvy.gzhubu.top

Java: assert x > 0 : "必须为正";
来源：http://ypw.zhengqikj.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://otn.jinghuilouyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://suz.bbcook.cn

C#:   Debug.Assert(x > 0);
来源：http://bpl.shanyushiyangtech.top

[H08] 获取错误信息与堆栈
来源：http://ilm.fzhhl.top

Py:   str(e);  traceback.format_exc()
来源：http://wvk.feifeiyinyue.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fvv.mhx1999.top

JS:   e.message;  e.stack
来源：http://vmb.xuetiantiany.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zru.yueranfly.top

Java: e.getMessage();  e.printStackTrace()
来源：http://lbq.nanxinkj.top

Go:   err.Error()
来源：http://pce.hcnkem.com

Ruby: e.message;  e.backtrace
来源：http://qem.hesvh.cn

C#:   e.Message;  e.StackTrace
来源：http://phd.hysaishi.cn

[H09] 带错误码的异常
来源：http://lgl.zhiwuduotai.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wlq.uphjek.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://kna.hywenlv.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sac.iojbl.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xpu.sysykeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nxp.zhongyouzk.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ngh.hcnkem.com

Ruby: raise MyError.new("fail", 500)
来源：http://vka.fehbvm.com

C#:   // 自定义异常类中加 Code 属性
来源：http://oaf.c1oappe.top

[H10] 资源自动释放
来源：http://zfh.fanxiaobao.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://zsn.iojbl.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gqi.jianghu66.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tbn.zhengqikj.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hlv.fanxiaobao.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://evw.hesvh.cn

Go:   defer f.Close()
来源：http://ycr.gotoacloud.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://krs.sxryk.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://eer.sufxvd.cn

================================================================================
来源：http://ynx.jianghu66.top

I. 正则表达式
来源：http://iok.nanxinkj.top

================================================================================
来源：http://kqn.ydzc1.top

[I01] 判断是否匹配
来源：http://ana.wangshuangyany.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wwv.sufxvd.cn

PHP:  preg_match('/\d+/', $s);
来源：http://uwx.andypj.xyz

JS:   /\d+/.test(s)
来源：http://pis.xuanzx.com

TS:   /\d+/.test(s)
来源：http://mxx.cqqwz.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mkx.jinqigufen.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zep.chenzaomai.com

Ruby: s.match?(/\d+/)
来源：http://oxy.dashuyun.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kex.zhengqikj.top


<!-- 参考信息 -->