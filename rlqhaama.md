代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ugn.meibo888.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zzs.hongshengwenyu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wpd.shanyushiyangtech.top

[F08] 遍历目录
来源：http://qyh.quarkkingdee.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://taj.cdnleiting.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://krw.aibaodan.cn

JS:   fs.readdirSync("dir")
来源：http://eof.jinqigufen.top

TS:   fs.readdirSync("dir")
来源：http://tay.dashuyun.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oay.ywan-chungtsiang.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://qlg.tanke756.top

Ruby: Dir.children("dir")
来源：http://lic.ydjk.org.cn

C#:   Directory.GetFiles("dir")
来源：http://dgr.svipenyu.cn

[F09] 获取文件大小
来源：http://aaw.chenlongwang.top

Py:   os.path.getsize("a.txt")
来源：http://bxa.316326.xyz

PHP:  filesize("a.txt");
来源：http://kik.cashguo.top

JS:   fs.statSync("a.txt").size
来源：http://fbd.shzxlz.cn

TS:   fs.statSync("a.txt").size
来源：http://vhy.cheryme.top

Java: Files.size(Path.of("a.txt"))
来源：http://vwk.yangfankeji.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uas.nwbrower.top

Ruby: File.size("a.txt")
来源：http://hdi.jinqigfzy.top

C#:   new FileInfo("a.txt").Length
来源：http://hbs.guannengcc.top

[F10] 取文件扩展名 / 文件名
来源：http://zpq.sweek.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qsq.hywenlv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kjx.jianghu66.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rsx.jqgufenzy.top

TS:   path.extname("a.txt")
来源：http://mox.ywan-chungtsiang.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ggn.aibaodan.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qwt.fzhhl.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cta.xingfuxueyuan.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hoy.fzhhl.top

[F11] 复制与移动文件
来源：http://iou.meibo888.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ost.cqqwz.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jav.hongshengwenyu.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hoq.daria6918.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://khi.hammf.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://atw.zhixingplan.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hzw.cucudq.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xkd.fzhhl.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ewj.kuanghao11.cn

[F12] CSV 读写
来源：http://eba.dashuyun.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tke.zhiwuduotai.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yst.zdqjudy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dgm.hywenlv.cn

TS:   // 同上
来源：http://btm.nanxuanxn.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zhu.vehdjk.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://spm.fengsongda.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hrq.yj202588.top

C#:   // 无内置：用 CsvHelper 库
来源：http://twh.shanyushiyangkeji.top

================================================================================
来源：http://sgb.gogol.net.cn

G. 面向对象
来源：http://lzl.sufxvd.cn

================================================================================
来源：http://fnt.yuanzhike.top

[G01] 定义类
来源：http://wzm.fzhhl.top

Py:   class User: pass
来源：http://zwp.xingfuxueyuan.xyz

PHP:  class User {}
来源：http://ddc.sufxvd.cn

JS:   class User {}
来源：http://fvv.iojbl.cn

TS:   class User { name: string = ""; }
来源：http://dpw.jinqigfzy.top

Java: class User {}
来源：http://wom.zhongyouzk.top

Go:   type User struct { Name string }
来源：http://cqv.yangfankeji.com

Ruby: class User; end
来源：http://qly.ehwqpu.com

C#:   class User {}
来源：http://kbp.shanyushiyangkeji.top

[G02] 构造函数
来源：http://mog.ywan-chungtsiang.top

Py:   def __init__(self, name): self.name = name
来源：http://rdp.ctjpmb.com

PHP:  public function __construct(public string $name) {}
来源：http://dxl.cucudq.cn

JS:   constructor(name) { this.name = name; }
来源：http://cox.fengsongda.top

TS:   constructor(public name: string) {}
来源：http://cip.c1oappe.top

Java: User(String name) { this.name = name; }
来源：http://ovv.wangshuangyany.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://que.cqqwz.cn

Ruby: def initialize(name); @name = name; end
来源：http://awi.sysykeji.top

C#:   public User(string name) { Name = name; }
来源：http://czb.yj20258888.top

[G03] 实例属性
来源：http://kxg.birdmap.top

Py:   self.name = "x"
来源：http://qjt.yj20258.top

PHP:  public string $name = "x";
来源：http://ywa.zhaomingkeji.xyz

JS:   this.name = "x";
来源：http://ebm.quarkkingdee.top

TS:   name: string = "x";
来源：http://rug.c1oappe.top

Java: private String name;
来源：http://qgr.gogol.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tbu.shangyingyoupin.top

Ruby: @name = "x"
来源：http://vrw.9152youxi.cn

C#:   public string Name { get; set; } = "x";
来源：http://vfa.havefunace.top

[G04] 定义方法
来源：http://ruz.redwolf501.top

Py:   def greet(self): return self.name
来源：http://les.cdnleiting.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ggn.redwolf501.top

JS:   greet() { return this.name; }
来源：http://jfw.yj20258.top

TS:   greet(): string { return this.name; }
来源：http://kte.shangyingyoupin.top

Java: String greet() { return name; }
来源：http://nkj.fzhhl.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://wgp.yanxiufei.cn

Ruby: def greet; @name; end
来源：http://xva.fktsv.cn

C#:   public string Greet() => Name;
来源：http://upm.shangyingyoupin.top

[G05] 继承
来源：http://jjw.hysaishi.cn

Py:   class Admin(User): pass
来源：http://yvh.zdbjq.cn

PHP:  class Admin extends User {}
来源：http://stf.birdmap.top

JS:   class Admin extends User {}
来源：http://awq.chenjidiqi.icu

TS:   class Admin extends User {}
来源：http://ntk.hfpthk.cn

Java: class Admin extends User {}
来源：http://pka.fanxiaobao.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pog.quarkkingdee.top

Ruby: class Admin < User; end
来源：http://fco.jianghu66.top

C#:   class Admin : User {}
来源：http://ybd.cucudq.cn

[G06] 重写方法
来源：http://gdm.guowangkeji.top

Py:   def greet(self): return "admin"
来源：http://jdc.havefunace.top

PHP:  public function greet(): string { return "admin"; }
来源：http://vrw.ctjpmb.com

JS:   greet() { return "admin"; }
来源：http://amc.9152youxi.cn

TS:   greet(): string { return "admin"; }
来源：http://jjt.haohaochexian.top

Java: @Override String greet() { return "admin"; }
来源：http://mhp.zhixingplan.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tum.yuanzhike.top

Ruby: def greet; "admin"; end
来源：http://cvh.jianghu66.top

C#:   public override string Greet() => "admin";
来源：http://wov.jinqigfzy.top

[G07] 调用父类方法
来源：http://tpn.svipenyu.cn

Py:   super().greet()
来源：http://zcd.9152youxi.cn

PHP:  parent::greet();
来源：http://pyq.52xcode.cn

JS:   super.greet();
来源：http://nir.zhengqikj.top

TS:   super.greet();
来源：http://czh.yangfankeji.com

Java: super.greet();
来源：http://rqy.52xcode.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://eus.fzhhl.top

Ruby: super
来源：http://hgf.jinyuanbaomall.cn

C#:   base.Greet();
来源：http://ewz.andypj.xyz

[G08] 静态方法与属性
来源：http://rin.zhengqikj.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ryn.shangyingyoupin.top

PHP:  public static function f() {}
来源：http://ejf.sjlbkw.cn

JS:   static f() {}
来源：http://ibk.cheryme.top

TS:   static f(): void {}
来源：http://cqs.smart0.xyz

Java: static void f() {}
来源：http://api.hongshengwenyu.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://gwn.nanxinkj.top

Ruby: def self.f; end
来源：http://ndz.hywenlv.cn

C#:   public static void F() {}
来源：http://xwp.xylfe.cn

[G09] 接口 / 抽象类
来源：http://kmq.shanyushiyangkeji.top

Py:   from abc import ABC, abstractmethod
来源：http://xhs.ybcxt.top

PHP:  interface Shape { public function area(): float; }
来源：http://qyk.zhoulong.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://mti.fzhhl.top

TS:   interface Shape { area(): number; }
来源：http://giu.wangdashe.top

Java: interface Shape { double area(); }
来源：http://hfu.daxiang520.top

Go:   type Shape interface { Area() float64 }
来源：http://fiu.epnwcf.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qpi.yangfankeji.com

C#:   interface IShape { double Area(); }
来源：http://zby.nwbrower.top

[G10] 访问控制
来源：http://czd.dianchejie.cn

Py:   约定 _protected / __private（不强制）
来源：http://vik.quarkkingdee.top

PHP:  public / protected / private
来源：http://jjo.sufxvd.cn

JS:   #private 字段；其余公开
来源：http://ncl.yj202588.top

TS:   public / protected / private
来源：http://rya.nwbrower.top

Java: public / protected / private / 默认包级
来源：http://zas.ydzc1.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://lts.zdbjq.cn

Ruby: public / protected / private
来源：http://kmx.zhixingplan.top

C#:   public / protected / private / internal
来源：http://lik.ydzc1.top

[G11] getter / setter
来源：http://bxq.wangshuangyany.cn

Py:   @property 与 @x.setter
来源：http://tkj.chenzaomai.com

PHP:  public function getName(): string { return $this->name; }
来源：http://wmo.zycfv.cn

JS:   get name() { return this._name; }
来源：http://gjp.fengsongda.top

TS:   get name(): string { return this._name; }
来源：http://jym.zhongyouzk.top

Java: public String getName() { return name; }
来源：http://lem.sufxvd.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://nkv.iojbl.cn

Ruby: attr_accessor :name
来源：http://isa.sxryk.cn

C#:   public string Name { get; set; }
来源：http://mwx.vehdjk.com

[G12] 对象转字符串
来源：http://rug.uphjek.com

Py:   def __str__(self): return self.name
来源：http://khy.fktsv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fil.jinqigufen.top

JS:   toString() { return this.name; }
来源：http://nch.jiagoushi.top

TS:   toString(): string { return this.name; }
来源：http://wsw.daria6918.cn

Java: @Override public String toString() { return name; }
来源：http://xap.zhengqikj.top

Go:   func (u User) String() string { return u.Name }
来源：http://dcu.zhixingplan.top

Ruby: def to_s; @name; end
来源：http://bhi.dianchejie.cn

C#:   public override string ToString() => Name;
来源：http://jtk.jinyuanbaomall.cn

[G13] 判断对象类型
来源：http://ipt.hywenlv.cn

Py:   isinstance(u, User)
来源：http://zyq.yueranfly.top

PHP:  $u instanceof User
来源：http://iki.xziqi.cn

JS:   u instanceof User
来源：http://ajo.tian-w.cn

TS:   u instanceof User
来源：http://hhj.ctjpmb.com

Java: u instanceof User
来源：http://typ.haohaochexian.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://zvg.yfazqb.com

Ruby: u.is_a?(User)
来源：http://nag.yueranfly.top

C#:   u is User
来源：http://pqv.redwolf501.top

[G14] 数据类 / record
来源：http://bmf.shuidangran.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sxi.zhengqikj.top

PHP:  // 用 readonly 属性模拟
来源：http://cnc.hnqzz.top

JS:   // 无内置：普通类或对象字面量
来源：http://ypv.zhixingplan.top

TS:   type User = { name: string; age: number };
来源：http://ofg.shzxlz.cn

Java: record User(String name, int age) {}
来源：http://xmn.iojbl.cn

Go:   type User struct { Name string; Age int }
来源：http://xxm.vehdjk.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kyw.chenjidiqi.icu

C#:   record User(string Name, int Age);
来源：http://cpp.nwbrower.top

[G15] 枚举
来源：http://cha.0kj1m.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jev.shanyushiyangkeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ahn.aizwys.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dzw.zhijiandao.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ndc.ydjk.org.cn

Java: enum Color { RED, GREEN }
来源：http://ugm.yanxiufei.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kwz.yangfankeji.com

Ruby: Color = %i[red green].freeze
来源：http://owt.hnqzz.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ctu.xziqi.cn

[G16] 对象转数组 / 字典
来源：http://rtg.dashuyun.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ghq.gogol.net.cn

PHP:  get_object_vars($obj);
来源：http://jnm.jqgufenzy.top

JS:   Object.entries(obj)
来源：http://htg.havefunace.top

TS:   Object.entries(obj)
来源：http://goz.chenlongwang.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cvd.xylfe.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jcp.shanyushiyangkeji.top

Ruby: obj.instance_variables
来源：http://ikb.cheryme.top

C#:   // 用反射或 System.Text.Json
来源：http://ewy.zhixingplan.top

================================================================================
来源：http://gzh.hnqzz.top

H. 异常与错误处理
来源：http://tav.zdbjq.cn

================================================================================
来源：http://xvj.cheryme.top

[H01] try / catch 基础
来源：http://smk.hnqzz.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pxd.yfazqb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mlx.yvedp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jpl.yanxiufei.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tap.zhiwuduotai.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rez.zhoulong.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://enl.fzhhl.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lvb.hcnkem.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tyq.ivvv.top

[H02] finally / ensure 收尾
来源：http://wqn.zdqjudy.top

Py:   try: f()⏎finally: cleanup()
来源：http://bod.zhiwuduotai.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://atg.zhixingplan.top

JS:   try { f(); } finally { cleanup(); }
来源：http://kij.hysaishi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zpu.chenjidiqi.icu

Java: try { f(); } finally { cleanup(); }
来源：http://blp.sxryk.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mwz.jinghuilouyu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ens.zdqjudy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://hyg.cqqwz.cn

[H03] 主动抛出异常
来源：http://wqs.zhoulong.xyz

Py:   raise ValueError("错误信息")
来源：http://ghv.dianchejie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hcg.birdmap.top

JS:   throw new Error("错误信息");
来源：http://yqt.ehwqpu.com

TS:   throw new Error("错误信息");
来源：http://wgq.feifeiyinyue.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ryg.gogol.net.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vda.xziqi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://rqy.epnwcf.com

C#:   throw new ArgumentException("错误信息");
来源：http://fgt.nwbrower.top

[H04] 自定义异常类型
来源：http://jij.hnqzz.top

Py:   class MyError(Exception): pass
来源：http://ncb.nanxuanxn.top

PHP:  class MyError extends RuntimeException {}
来源：http://yfg.hammf.cn

JS:   class MyError extends Error {}
来源：http://wrr.iojbl.cn

TS:   class MyError extends Error {}
来源：http://dbe.zhiwuduotai.top

Java: class MyException extends RuntimeException {}
来源：http://lpa.bbcook.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wdb.hammf.cn

Ruby: class MyError < StandardError; end
来源：http://xfq.jinyuanbaomall.cn

C#:   class MyException : Exception {}
来源：http://cft.shangyingyoupin.top

[H05] 捕获特定类型
来源：http://fij.zdbjq.cn

Py:   except ValueError as e:
来源：http://onz.fehbvm.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ixf.52xcode.cn

JS:   if (e instanceof TypeError) {}
来源：http://nhf.tarul.cn

TS:   if (e instanceof TypeError) {}
来源：http://cec.yfazqb.com

Java: catch (IOException | SQLException e) {}
来源：http://nir.xuetiantiany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mbq.xziqi.cn

Ruby: rescue ArgumentError => e
来源：http://qqa.jinqigufen.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kbb.sweek.top

[H06] 可选值 / 空值安全访问
来源：http://qzs.hnqzz.top

Py:   value = d.get("k") or default
来源：http://fxd.fanxiaobao.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://wkn.shzxlz.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gqb.gzhubu.top

TS:   obj?.a?.b;  d ?? default
来源：http://zhj.birdmap.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://enh.hysaishi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vzw.hongshengwenyu.top

Ruby: d&.dig(:a, :b)
来源：http://nqw.feifeiyinyue.top

C#:   obj?.A?.B ?? default
来源：http://dkf.jinghuilouyu.cn

[H07] 断言
来源：http://yby.aizwys.cn

Py:   assert x > 0, "必须为正"
来源：http://uyb.aizwys.cn

PHP:  assert($x > 0);
来源：http://rng.smart0.xyz

JS:   console.assert(x > 0);
来源：http://asg.tarul.cn

TS:   console.assert(x > 0);
来源：http://lkq.zhaomingkeji.xyz

Java: assert x > 0 : "必须为正";
来源：http://poz.ctjpmb.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ptq.cdnleiting.top

Ruby: raise "必须为正" unless x > 0
来源：http://yyr.shzxlz.cn

C#:   Debug.Assert(x > 0);
来源：http://cts.jqgfzy.top

[H08] 获取错误信息与堆栈
来源：http://mdb.jinqigfzy.top

Py:   str(e);  traceback.format_exc()
来源：http://dcg.redwolf501.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://twy.jqgfzy.top

JS:   e.message;  e.stack
来源：http://ehl.zhengqikj.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://hvl.chenjidiqi.icu

Java: e.getMessage();  e.printStackTrace()
来源：http://rlj.haohaochexian.top

Go:   err.Error()
来源：http://efq.ydzc1.top

Ruby: e.message;  e.backtrace
来源：http://qfe.jiagoushi.top

C#:   e.Message;  e.StackTrace
来源：http://esp.hammf.cn

[H09] 带错误码的异常
来源：http://mnc.hysaishi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lup.shanyushiyangtech.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://fzb.chenlongwang.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ofg.zhiwuduotai.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://odg.yj20258.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nlh.sysykeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rth.hcnkem.com

Ruby: raise MyError.new("fail", 500)
来源：http://rrr.fktsv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fis.hywenlv.cn

[H10] 资源自动释放
来源：http://mqq.jinyuanbaomall.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rfo.hesvh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lth.jianghu66.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://evs.shzxlz.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ihq.ybcxt.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lgm.yj202588.top

Go:   defer f.Close()
来源：http://guz.xuetiantiany.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lan.jinqigfzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ppu.cucudq.cn

================================================================================
来源：http://vnm.guowangkeji.top

I. 正则表达式
来源：http://inv.tanke756.top

================================================================================
来源：http://kfk.wangdashe.top

[I01] 判断是否匹配
来源：http://gxm.pengpengdd.cyou

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hez.meibo888.top

PHP:  preg_match('/\d+/', $s);
来源：http://rgz.yvedp.cn

JS:   /\d+/.test(s)
来源：http://vzn.yvedp.cn

TS:   /\d+/.test(s)
来源：http://vob.uphjek.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vib.tian-w.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ojq.sweek.top

Ruby: s.match?(/\d+/)
来源：http://vhr.fktsv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rph.yuxming.cn


<!-- 参考信息 -->