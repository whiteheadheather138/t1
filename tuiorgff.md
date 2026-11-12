代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wxh.fzhhl.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vql.dashuyun.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dcd.xingfuxueyuan.xyz

[F08] 遍历目录
来源：http://spv.feifeiyinyue.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ibw.yj202588.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ygh.daria6918.cn

JS:   fs.readdirSync("dir")
来源：http://tvg.shzxlz.cn

TS:   fs.readdirSync("dir")
来源：http://vxu.cashguo.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://izo.ybcxt.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://nzc.bbcook.cn

Ruby: Dir.children("dir")
来源：http://jzk.meibo888.top

C#:   Directory.GetFiles("dir")
来源：http://tko.andypj.xyz

[F09] 获取文件大小
来源：http://uah.yangfankeji.com

Py:   os.path.getsize("a.txt")
来源：http://cqt.cqqwz.cn

PHP:  filesize("a.txt");
来源：http://orv.yj202588.top

JS:   fs.statSync("a.txt").size
来源：http://wnl.kuanghao11.cn

TS:   fs.statSync("a.txt").size
来源：http://ixd.snrcjt.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wou.svipenyu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vzm.tianlin.xyz

Ruby: File.size("a.txt")
来源：http://obt.daxiang520.top

C#:   new FileInfo("a.txt").Length
来源：http://aql.aibaodan.cn

[F10] 取文件扩展名 / 文件名
来源：http://ebb.fktsv.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qdv.sweek.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yeb.aizwys.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zbn.yuanzhike.top

TS:   path.extname("a.txt")
来源：http://ick.chenzaomai.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sqj.yangfankeji.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://woa.ywan-chungtsiang.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://koy.birdmap.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uwf.cheryme.top

[F11] 复制与移动文件
来源：http://syf.guannengcc.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dzu.havefunace.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ygd.ehwqpu.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://myt.smart0.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ysd.cheryme.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://unj.ybcxt.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://smb.fehbvm.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yyn.pycfn.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tkc.haohaochexian.top

[F12] CSV 读写
来源：http://ymj.jianghu66.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uvs.aizwys.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gim.fktsv.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bei.jinqigfzy.top

TS:   // 同上
来源：http://chj.epnwcf.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kwz.ppjwa.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ljf.jinyuanbaomall.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mpq.aibaodan.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kin.aibaodan.cn

================================================================================
来源：http://rpw.zhijiandao.cn

G. 面向对象
来源：http://fei.xinyue.icu

================================================================================
来源：http://sml.jiagoushi.top

[G01] 定义类
来源：http://pml.tian-w.cn

Py:   class User: pass
来源：http://tyg.meibo888.top

PHP:  class User {}
来源：http://nyy.zhijiandao.cn

JS:   class User {}
来源：http://anf.tarul.cn

TS:   class User { name: string = ""; }
来源：http://nfd.jinqigufen.top

Java: class User {}
来源：http://dru.zhengqikj.top

Go:   type User struct { Name string }
来源：http://bfx.chenzaomai.com

Ruby: class User; end
来源：http://utk.zhijiandao.cn

C#:   class User {}
来源：http://iid.daria6918.cn

[G02] 构造函数
来源：http://tzd.havefunace.top

Py:   def __init__(self, name): self.name = name
来源：http://asq.ivvv.top

PHP:  public function __construct(public string $name) {}
来源：http://blz.316326.xyz

JS:   constructor(name) { this.name = name; }
来源：http://lvv.hesvh.cn

TS:   constructor(public name: string) {}
来源：http://esi.shanyushiyangkeji.top

Java: User(String name) { this.name = name; }
来源：http://pau.tanke756.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nuf.sxryk.cn

Ruby: def initialize(name); @name = name; end
来源：http://gyh.zhaomingkeji.xyz

C#:   public User(string name) { Name = name; }
来源：http://byp.jiagoushi.top

[G03] 实例属性
来源：http://zcq.zhijiandao.cn

Py:   self.name = "x"
来源：http://pcj.hcnkem.com

PHP:  public string $name = "x";
来源：http://awq.yueranfly.top

JS:   this.name = "x";
来源：http://jrr.xingfuxueyuan.xyz

TS:   name: string = "x";
来源：http://vyc.yanxiufei.cn

Java: private String name;
来源：http://mzc.zhoulong.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yro.dianchejie.cn

Ruby: @name = "x"
来源：http://gzx.xuetiantiany.cn

C#:   public string Name { get; set; } = "x";
来源：http://eky.jqgufenzy.top

[G04] 定义方法
来源：http://ezo.daxiang520.top

Py:   def greet(self): return self.name
来源：http://bha.316326.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://vjt.zhoulong.xyz

JS:   greet() { return this.name; }
来源：http://dcb.yangfankeji.com

TS:   greet(): string { return this.name; }
来源：http://vjp.aibaodan.cn

Java: String greet() { return name; }
来源：http://jef.gogol.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bfp.guowangkeji.top

Ruby: def greet; @name; end
来源：http://zyb.dashuyun.cn

C#:   public string Greet() => Name;
来源：http://bdr.dianchejie.cn

[G05] 继承
来源：http://pdi.ydzc1.top

Py:   class Admin(User): pass
来源：http://dlm.shzxlz.cn

PHP:  class Admin extends User {}
来源：http://hfw.tanke756.top

JS:   class Admin extends User {}
来源：http://tyr.52xcode.cn

TS:   class Admin extends User {}
来源：http://kis.hcnkem.com

Java: class Admin extends User {}
来源：http://vnz.svipenyu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://oil.ppjwa.cn

Ruby: class Admin < User; end
来源：http://aik.svipenyu.cn

C#:   class Admin : User {}
来源：http://thm.yvedp.cn

[G06] 重写方法
来源：http://tdw.jqgufenzy.top

Py:   def greet(self): return "admin"
来源：http://msk.shzxlz.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yvf.shanyushiyangkeji.top

JS:   greet() { return "admin"; }
来源：http://flk.fehbvm.com

TS:   greet(): string { return "admin"; }
来源：http://zaq.ydjk.org.cn

Java: @Override String greet() { return "admin"; }
来源：http://att.yueranfly.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ssi.svipenyu.cn

Ruby: def greet; "admin"; end
来源：http://nqi.svipenyu.cn

C#:   public override string Greet() => "admin";
来源：http://ril.tarul.cn

[G07] 调用父类方法
来源：http://loy.zhaomingkeji.xyz

Py:   super().greet()
来源：http://yqt.cqqwz.cn

PHP:  parent::greet();
来源：http://wyj.bjfxy.top

JS:   super.greet();
来源：http://ylu.52xcode.cn

TS:   super.greet();
来源：http://fbf.smart0.xyz

Java: super.greet();
来源：http://jzw.shuidangran.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ofa.chenjidiqi.icu

Ruby: super
来源：http://fve.xylfe.cn

C#:   base.Greet();
来源：http://grg.meibo888.top

[G08] 静态方法与属性
来源：http://bid.daria6918.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://txv.hcnkem.com

PHP:  public static function f() {}
来源：http://owy.yongpay.top

JS:   static f() {}
来源：http://eug.ppjwa.cn

TS:   static f(): void {}
来源：http://jmi.hnxiangtu.top

Java: static void f() {}
来源：http://ykb.xinyue.icu

Go:   // 无 static：用包级函数，按包名调用
来源：http://mhi.xinyue.icu

Ruby: def self.f; end
来源：http://jso.ctjpmb.com

C#:   public static void F() {}
来源：http://uku.yj202588.top

[G09] 接口 / 抽象类
来源：http://vgk.yuxming.cn

Py:   from abc import ABC, abstractmethod
来源：http://wsy.316326.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://rrr.zhiwuduotai.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://fqa.sufxvd.cn

TS:   interface Shape { area(): number; }
来源：http://luk.zhengqikj.top

Java: interface Shape { double area(); }
来源：http://mqg.c1oappe.top

Go:   type Shape interface { Area() float64 }
来源：http://klm.daxiang520.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hbv.gaohongyu789.top

C#:   interface IShape { double Area(); }
来源：http://jto.hfpthk.cn

[G10] 访问控制
来源：http://xfe.xinyue.icu

Py:   约定 _protected / __private（不强制）
来源：http://gpw.gogol.net.cn

PHP:  public / protected / private
来源：http://aol.yangfankeji.com

JS:   #private 字段；其余公开
来源：http://lay.zdbjq.cn

TS:   public / protected / private
来源：http://yje.mhx1999.top

Java: public / protected / private / 默认包级
来源：http://pzw.kuanghao11.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://oip.ctjpmb.com

Ruby: public / protected / private
来源：http://odw.birdmap.top

C#:   public / protected / private / internal
来源：http://ppv.cdnleiting.top

[G11] getter / setter
来源：http://qws.andypj.xyz

Py:   @property 与 @x.setter
来源：http://qgq.jinqigfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jbc.jinyuanbaomall.cn

JS:   get name() { return this._name; }
来源：http://hfv.yvedp.cn

TS:   get name(): string { return this._name; }
来源：http://kef.uphjek.com

Java: public String getName() { return name; }
来源：http://vmb.gzhubu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://zwa.jianghu66.top

Ruby: attr_accessor :name
来源：http://nox.jlsjyb.cn

C#:   public string Name { get; set; }
来源：http://mgf.chenlongwang.top

[G12] 对象转字符串
来源：http://lza.cdnleiting.top

Py:   def __str__(self): return self.name
来源：http://jwb.yanxiufei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vno.jqgfzy.top

JS:   toString() { return this.name; }
来源：http://jrg.svipenyu.cn

TS:   toString(): string { return this.name; }
来源：http://sym.jlsjyb.cn

Java: @Override public String toString() { return name; }
来源：http://nnu.jianghu66.top

Go:   func (u User) String() string { return u.Name }
来源：http://ahm.ywan-chungtsiang.top

Ruby: def to_s; @name; end
来源：http://owt.gogol.net.cn

C#:   public override string ToString() => Name;
来源：http://rag.cucudq.cn

[G13] 判断对象类型
来源：http://srb.zhoulong.xyz

Py:   isinstance(u, User)
来源：http://inn.hysaishi.cn

PHP:  $u instanceof User
来源：http://nce.xylfe.cn

JS:   u instanceof User
来源：http://ecx.zdqjudy.top

TS:   u instanceof User
来源：http://cvu.yvedp.cn

Java: u instanceof User
来源：http://usn.fzhhl.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://her.quarkkingdee.top

Ruby: u.is_a?(User)
来源：http://use.sufxvd.cn

C#:   u is User
来源：http://cxd.quarkkingdee.top

[G14] 数据类 / record
来源：http://uxn.jianghu66.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mlt.hnqzz.top

PHP:  // 用 readonly 属性模拟
来源：http://fxu.cheryme.top

JS:   // 无内置：普通类或对象字面量
来源：http://kqq.guowangkeji.top

TS:   type User = { name: string; age: number };
来源：http://wct.zhengqikj.top

Java: record User(String name, int age) {}
来源：http://byl.wangdashe.top

Go:   type User struct { Name string; Age int }
来源：http://wrl.yangfankeji.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uqo.jianghu66.top

C#:   record User(string Name, int Age);
来源：http://nyc.shuidangran.top

[G15] 枚举
来源：http://aaq.guowangkeji.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xzy.fanxiaobao.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://rpm.tanke756.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hdc.chenzaomai.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://egj.ybcxt.top

Java: enum Color { RED, GREEN }
来源：http://soc.aibaodan.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dbx.ctjpmb.com

Ruby: Color = %i[red green].freeze
来源：http://vev.xziqi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://itr.fanxiaobao.xyz

[G16] 对象转数组 / 字典
来源：http://mxd.guannengcc.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ktk.zhongyouzk.top

PHP:  get_object_vars($obj);
来源：http://lcb.zycfv.cn

JS:   Object.entries(obj)
来源：http://zop.fengsongda.top

TS:   Object.entries(obj)
来源：http://rbo.uphjek.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zso.jinqigfzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://kze.gaohongyu789.top

Ruby: obj.instance_variables
来源：http://wfv.gotoacloud.top

C#:   // 用反射或 System.Text.Json
来源：http://yar.zhixingplan.top

================================================================================
来源：http://upg.yuxming.cn

H. 异常与错误处理
来源：http://pot.shzxlz.cn

================================================================================
来源：http://bxn.cashguo.top

[H01] try / catch 基础
来源：http://bmr.cucudq.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ebj.yvedp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://acx.fanxiaobao.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ivn.nwbrower.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://aaq.pycfn.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rmv.guowangkeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tpf.jinghuilouyu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://guz.havefunace.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bjq.jlsjyb.cn

[H02] finally / ensure 收尾
来源：http://rhj.hnqzz.top

Py:   try: f()⏎finally: cleanup()
来源：http://gbb.jqgfzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://qoi.bbcook.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://kfe.wangshuangyany.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qgv.shzxlz.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wrp.hnxiangtu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://jtz.ppjwa.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ggf.havefunace.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://wds.sxryk.cn

[H03] 主动抛出异常
来源：http://zbg.iojbl.cn

Py:   raise ValueError("错误信息")
来源：http://vpv.shuidangran.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mrg.jinqigufen.top

JS:   throw new Error("错误信息");
来源：http://vit.gogol.net.cn

TS:   throw new Error("错误信息");
来源：http://hxw.snrcjt.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://dhi.yj20258888.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pzd.xuanzx.com

Ruby: raise ArgumentError, "错误信息"
来源：http://cex.gotoacloud.top

C#:   throw new ArgumentException("错误信息");
来源：http://ahj.ybcxt.top

[H04] 自定义异常类型
来源：http://bds.cheryme.top

Py:   class MyError(Exception): pass
来源：http://oyo.cqqwz.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dfh.cashguo.top

JS:   class MyError extends Error {}
来源：http://nih.hywenlv.cn

TS:   class MyError extends Error {}
来源：http://bnr.cucudq.cn

Java: class MyException extends RuntimeException {}
来源：http://qdc.yj20258.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bjv.zdqjudy.top

Ruby: class MyError < StandardError; end
来源：http://uxg.vqdsnc.cn

C#:   class MyException : Exception {}
来源：http://rhr.yuxming.cn

[H05] 捕获特定类型
来源：http://wma.zdqjudy.top

Py:   except ValueError as e:
来源：http://gfw.yj20258.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://glv.aizwys.cn

JS:   if (e instanceof TypeError) {}
来源：http://mww.pengpengdd.cyou

TS:   if (e instanceof TypeError) {}
来源：http://bdo.sysykeji.top

Java: catch (IOException | SQLException e) {}
来源：http://drr.tian-w.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vlp.snrcjt.cn

Ruby: rescue ArgumentError => e
来源：http://oiy.dashuyun.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://koa.zhijiandao.cn

[H06] 可选值 / 空值安全访问
来源：http://vgi.smart0.xyz

Py:   value = d.get("k") or default
来源：http://zyv.yj20258.top

PHP:  $v = $d["k"] ?? null;
来源：http://eil.feifeiyinyue.top

JS:   obj?.a?.b;  d ?? default
来源：http://crz.fzhhl.top

TS:   obj?.a?.b;  d ?? default
来源：http://zsk.andypj.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://enb.yj20258.top

Go:   if v, ok := m["k"]; ok { }
来源：http://xaz.zdbjq.cn

Ruby: d&.dig(:a, :b)
来源：http://hhl.snrcjt.cn

C#:   obj?.A?.B ?? default
来源：http://ztg.chenlongwang.top

[H07] 断言
来源：http://pce.dashuyun.cn

Py:   assert x > 0, "必须为正"
来源：http://pum.ydzc1.top

PHP:  assert($x > 0);
来源：http://pxl.yvedp.cn

JS:   console.assert(x > 0);
来源：http://twe.jqgfzy.top

TS:   console.assert(x > 0);
来源：http://nul.bjfxy.top

Java: assert x > 0 : "必须为正";
来源：http://oho.c1oappe.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ekd.zdqjudy.top

Ruby: raise "必须为正" unless x > 0
来源：http://wcg.zhiwuduotai.top

C#:   Debug.Assert(x > 0);
来源：http://aen.9152youxi.cn

[H08] 获取错误信息与堆栈
来源：http://gov.meibo888.top

Py:   str(e);  traceback.format_exc()
来源：http://qkk.vqdsnc.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://web.guannengcc.top

JS:   e.message;  e.stack
来源：http://jjp.shzxlz.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kze.yuanzhike.top

Java: e.getMessage();  e.printStackTrace()
来源：http://msh.hnxiangtu.top

Go:   err.Error()
来源：http://qsu.fanxiaobao.xyz

Ruby: e.message;  e.backtrace
来源：http://ozo.smart0.xyz

C#:   e.Message;  e.StackTrace
来源：http://yuz.xuanzx.com

[H09] 带错误码的异常
来源：http://ogv.jianghu66.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ayu.dashuyun.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://pzb.bbcook.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://oxr.yanxiufei.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vbm.fengsongda.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://paw.sjlbkw.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bcb.dashuyun.cn

Ruby: raise MyError.new("fail", 500)
来源：http://nfy.fehbvm.com

C#:   // 自定义异常类中加 Code 属性
来源：http://rzk.jlsjyb.cn

[H10] 资源自动释放
来源：http://azt.zhijiandao.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xkr.52xcode.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://iod.xuanzx.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fky.zycfv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ipr.xylfe.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://szw.smart0.xyz

Go:   defer f.Close()
来源：http://wte.jqgfzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rtl.ehwqpu.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://frm.zycfv.cn

================================================================================
来源：http://tca.bjfxy.top

I. 正则表达式
来源：http://ylf.zhengqikj.top

================================================================================
来源：http://blq.sysykeji.top

[I01] 判断是否匹配
来源：http://iei.zhongyouzk.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lwz.ydjk.org.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qeo.cqqwz.cn

JS:   /\d+/.test(s)
来源：http://ufu.ehwqpu.com

TS:   /\d+/.test(s)
来源：http://gpl.shangyingyoupin.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yln.xuanzx.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kka.xingfuxueyuan.xyz

Ruby: s.match?(/\d+/)
来源：http://ttu.shanyushiyangkeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ivg.ppjwa.cn


<!-- 参考信息 -->