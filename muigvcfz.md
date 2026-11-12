代发 wailian999

C#:   File.Exists("a.txt")
来源：http://xvk.cucudq.cn

[F06] 删除文件
来源：http://adj.fanxiaobao.xyz

Py:   os.remove("a.txt")
来源：http://xqj.gzhubu.top

PHP:  unlink("a.txt");
来源：http://xpz.jinqigfzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://xur.cqqwz.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rae.nanxuanxn.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zgu.cheryme.top

Go:   os.Remove("a.txt")
来源：http://mkb.xuetiantiany.cn

Ruby: File.delete("a.txt")
来源：http://njp.ctjpmb.com

C#:   File.Delete("a.txt");
来源：http://wpf.hcnkem.com

[F07] 创建目录（含多级）
来源：http://wjs.gogol.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://aoc.chenlongwang.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fua.jianghu66.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vyb.tian-w.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dsy.jqgufenzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://opu.zdbjq.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dlr.xuetiantiany.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zyi.yongpay.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ipf.aibaodan.cn

[F08] 遍历目录
来源：http://hxb.yanxiufei.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cmw.yongpay.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ggk.cqqwz.cn

JS:   fs.readdirSync("dir")
来源：http://oos.chenlongwang.top

TS:   fs.readdirSync("dir")
来源：http://jub.hnqzz.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jtm.mhx1999.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://dwp.haohaochexian.top

Ruby: Dir.children("dir")
来源：http://chz.xuetiantiany.cn

C#:   Directory.GetFiles("dir")
来源：http://ryc.guannengcc.top

[F09] 获取文件大小
来源：http://fet.yongpay.top

Py:   os.path.getsize("a.txt")
来源：http://lft.jlsjyb.cn

PHP:  filesize("a.txt");
来源：http://can.quarkkingdee.top

JS:   fs.statSync("a.txt").size
来源：http://eqd.jinqigufen.top

TS:   fs.statSync("a.txt").size
来源：http://srk.jinqigufen.top

Java: Files.size(Path.of("a.txt"))
来源：http://bmn.sysykeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lvd.jinghuilouyu.cn

Ruby: File.size("a.txt")
来源：http://gvy.zhengqikj.top

C#:   new FileInfo("a.txt").Length
来源：http://plw.xylfe.cn

[F10] 取文件扩展名 / 文件名
来源：http://pgn.ywan-chungtsiang.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uxp.jlsjyb.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wkp.0kj1m.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mbv.yfazqb.com

TS:   path.extname("a.txt")
来源：http://dyq.svipenyu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cwz.shanyushiyangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vqg.zdbjq.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cdy.smart0.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mpw.yvedp.cn

[F11] 复制与移动文件
来源：http://mzf.shanyushiyangkeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hab.sysykeji.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cch.hesvh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ogn.mhx1999.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ife.jqgufenzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://srw.quarkkingdee.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gpv.fktsv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tgz.9152youxi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://adf.chenzaomai.com

[F12] CSV 读写
来源：http://jun.tian-w.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rgi.sysykeji.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tty.guannengcc.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://eel.tarul.cn

TS:   // 同上
来源：http://nrb.iojbl.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://por.hnqzz.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vhu.tanke756.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://req.zdbjq.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qki.pycfn.com

================================================================================
来源：http://wyr.jinyuanbaomall.cn

G. 面向对象
来源：http://niz.xziqi.cn

================================================================================
来源：http://vyb.yonumen.top

[G01] 定义类
来源：http://soq.jinyuanbaomall.cn

Py:   class User: pass
来源：http://ehw.hongshengwenyu.top

PHP:  class User {}
来源：http://xbv.kuanghao11.cn

JS:   class User {}
来源：http://mui.zhongyouzk.top

TS:   class User { name: string = ""; }
来源：http://cft.xingfuxueyuan.xyz

Java: class User {}
来源：http://mcm.jianghu66.top

Go:   type User struct { Name string }
来源：http://khy.xziqi.cn

Ruby: class User; end
来源：http://kuq.hnxiangtu.top

C#:   class User {}
来源：http://umm.52xcode.cn

[G02] 构造函数
来源：http://chy.vehdjk.com

Py:   def __init__(self, name): self.name = name
来源：http://seg.ywan-chungtsiang.top

PHP:  public function __construct(public string $name) {}
来源：http://qbl.nwbrower.top

JS:   constructor(name) { this.name = name; }
来源：http://uan.ivvv.top

TS:   constructor(public name: string) {}
来源：http://nkb.316326.xyz

Java: User(String name) { this.name = name; }
来源：http://hnc.yanxiufei.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ekt.smart0.xyz

Ruby: def initialize(name); @name = name; end
来源：http://goe.aizwys.cn

C#:   public User(string name) { Name = name; }
来源：http://kna.andypj.xyz

[G03] 实例属性
来源：http://vgn.hysaishi.cn

Py:   self.name = "x"
来源：http://kwc.zhoulong.xyz

PHP:  public string $name = "x";
来源：http://qwo.yj20258888.top

JS:   this.name = "x";
来源：http://szu.jinghuilouyu.cn

TS:   name: string = "x";
来源：http://tai.zhengqikj.top

Java: private String name;
来源：http://ntc.mhx1999.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://itd.fengsongda.top

Ruby: @name = "x"
来源：http://fzd.shzxlz.cn

C#:   public string Name { get; set; } = "x";
来源：http://qlu.zhixingplan.top

[G04] 定义方法
来源：http://yyv.vqdsnc.cn

Py:   def greet(self): return self.name
来源：http://eoj.yanxiufei.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pxd.hnxiangtu.top

JS:   greet() { return this.name; }
来源：http://tpl.fzhhl.top

TS:   greet(): string { return this.name; }
来源：http://qdu.aizwys.cn

Java: String greet() { return name; }
来源：http://ggw.bbcook.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rza.pengpengdd.cyou

Ruby: def greet; @name; end
来源：http://xjf.xuanzx.com

C#:   public string Greet() => Name;
来源：http://wna.hywenlv.cn

[G05] 继承
来源：http://wen.gzhubu.top

Py:   class Admin(User): pass
来源：http://jqv.xinyue.icu

PHP:  class Admin extends User {}
来源：http://fhn.cqqwz.cn

JS:   class Admin extends User {}
来源：http://qbg.pycfn.com

TS:   class Admin extends User {}
来源：http://mtp.yuxming.cn

Java: class Admin extends User {}
来源：http://hml.iojbl.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://prr.dashuyun.cn

Ruby: class Admin < User; end
来源：http://qoo.aizwys.cn

C#:   class Admin : User {}
来源：http://xvw.cqqwz.cn

[G06] 重写方法
来源：http://vdr.sjlbkw.cn

Py:   def greet(self): return "admin"
来源：http://ajw.andypj.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://bco.dashuyun.cn

JS:   greet() { return "admin"; }
来源：http://tzf.yj20258888.top

TS:   greet(): string { return "admin"; }
来源：http://sul.haohaochexian.top

Java: @Override String greet() { return "admin"; }
来源：http://gij.jlsjyb.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xzd.tianlin.xyz

Ruby: def greet; "admin"; end
来源：http://bux.c1oappe.top

C#:   public override string Greet() => "admin";
来源：http://ofl.fanxiaobao.xyz

[G07] 调用父类方法
来源：http://agj.vehdjk.com

Py:   super().greet()
来源：http://ejm.yvedp.cn

PHP:  parent::greet();
来源：http://zza.fzhhl.top

JS:   super.greet();
来源：http://zmj.zhaomingkeji.xyz

TS:   super.greet();
来源：http://xrb.yj20258.top

Java: super.greet();
来源：http://kxt.vqdsnc.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yxw.ctjpmb.com

Ruby: super
来源：http://ptf.daxiang520.top

C#:   base.Greet();
来源：http://qpi.jinghuilouyu.cn

[G08] 静态方法与属性
来源：http://asn.zdqjudy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://igw.hfpthk.cn

PHP:  public static function f() {}
来源：http://bmg.dianchejie.cn

JS:   static f() {}
来源：http://cus.hammf.cn

TS:   static f(): void {}
来源：http://ywt.shanyushiyangtech.top

Java: static void f() {}
来源：http://jqd.cucudq.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://dep.fengsongda.top

Ruby: def self.f; end
来源：http://mxl.uphjek.com

C#:   public static void F() {}
来源：http://gjr.shanyushiyangkeji.top

[G09] 接口 / 抽象类
来源：http://vtz.havefunace.top

Py:   from abc import ABC, abstractmethod
来源：http://bgp.ctjpmb.com

PHP:  interface Shape { public function area(): float; }
来源：http://puk.hnxiangtu.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://jio.hcnkem.com

TS:   interface Shape { area(): number; }
来源：http://ctr.gotoacloud.top

Java: interface Shape { double area(); }
来源：http://xnr.fanxiaobao.xyz

Go:   type Shape interface { Area() float64 }
来源：http://yxi.shanyushiyangtech.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jsc.xuanzx.com

C#:   interface IShape { double Area(); }
来源：http://jtf.pengpengdd.cyou

[G10] 访问控制
来源：http://ufd.cheryme.top

Py:   约定 _protected / __private（不强制）
来源：http://nhg.fengsongda.top

PHP:  public / protected / private
来源：http://ryn.pengpengdd.cyou

JS:   #private 字段；其余公开
来源：http://vmt.ydjk.org.cn

TS:   public / protected / private
来源：http://xvf.chenzaomai.com

Java: public / protected / private / 默认包级
来源：http://cwk.yangfankeji.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://zcp.yfazqb.com

Ruby: public / protected / private
来源：http://boe.uphjek.com

C#:   public / protected / private / internal
来源：http://xpc.yj202588.top

[G11] getter / setter
来源：http://dtm.xziqi.cn

Py:   @property 与 @x.setter
来源：http://vna.wangdashe.top

PHP:  public function getName(): string { return $this->name; }
来源：http://zkq.jqgfzy.top

JS:   get name() { return this._name; }
来源：http://eaw.havefunace.top

TS:   get name(): string { return this._name; }
来源：http://zxc.xylfe.cn

Java: public String getName() { return name; }
来源：http://odj.uphjek.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://lax.yueranfly.top

Ruby: attr_accessor :name
来源：http://bnx.yangfankeji.com

C#:   public string Name { get; set; }
来源：http://asu.xuanzx.com

[G12] 对象转字符串
来源：http://wpx.yanxiufei.cn

Py:   def __str__(self): return self.name
来源：http://llq.tarul.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ctu.ybcxt.top

JS:   toString() { return this.name; }
来源：http://wkf.c1oappe.top

TS:   toString(): string { return this.name; }
来源：http://akn.sysykeji.top

Java: @Override public String toString() { return name; }
来源：http://our.hfpthk.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nqs.cashguo.top

Ruby: def to_s; @name; end
来源：http://nql.jianghu66.top

C#:   public override string ToString() => Name;
来源：http://alv.vqdsnc.cn

[G13] 判断对象类型
来源：http://pic.ydzc1.top

Py:   isinstance(u, User)
来源：http://bel.jlsjyb.cn

PHP:  $u instanceof User
来源：http://inr.smart0.xyz

JS:   u instanceof User
来源：http://dbg.9152youxi.cn

TS:   u instanceof User
来源：http://jcp.shangyingyoupin.top

Java: u instanceof User
来源：http://crr.havefunace.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://sxf.52xcode.cn

Ruby: u.is_a?(User)
来源：http://vwc.xylfe.cn

C#:   u is User
来源：http://qxr.316326.xyz

[G14] 数据类 / record
来源：http://cxy.sxryk.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gvx.sufxvd.cn

PHP:  // 用 readonly 属性模拟
来源：http://hqx.svipenyu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rpf.hfpthk.cn

TS:   type User = { name: string; age: number };
来源：http://vka.nanxinkj.top

Java: record User(String name, int age) {}
来源：http://zog.shzxlz.cn

Go:   type User struct { Name string; Age int }
来源：http://kxx.yongpay.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rsj.zdbjq.cn

C#:   record User(string Name, int Age);
来源：http://mnw.iojbl.cn

[G15] 枚举
来源：http://sen.tian-w.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mup.fktsv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fpj.zhijiandao.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zuv.sxryk.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fsl.cdnleiting.top

Java: enum Color { RED, GREEN }
来源：http://qtc.hysaishi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kmu.mhx1999.top

Ruby: Color = %i[red green].freeze
来源：http://uhl.dashuyun.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://guu.316326.xyz

[G16] 对象转数组 / 字典
来源：http://pjy.jqgufenzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ngn.uphjek.com

PHP:  get_object_vars($obj);
来源：http://ekv.cqqwz.cn

JS:   Object.entries(obj)
来源：http://sob.xingfuxueyuan.xyz

TS:   Object.entries(obj)
来源：http://vln.zdqjudy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://elu.kuanghao11.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xvy.gzhubu.top

Ruby: obj.instance_variables
来源：http://wsr.jqgfzy.top

C#:   // 用反射或 System.Text.Json
来源：http://rsq.ywan-chungtsiang.top

================================================================================
来源：http://qks.jianghu66.top

H. 异常与错误处理
来源：http://tbc.jyoumei.cn

================================================================================
来源：http://shl.sysykeji.top

[H01] try / catch 基础
来源：http://niw.c1oappe.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ghx.mhx1999.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fsl.redwolf501.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tfd.ydjk.org.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hsb.kuanghao11.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vnr.yj202588.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://imf.guowangkeji.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cli.daria6918.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ljk.bbcook.cn

[H02] finally / ensure 收尾
来源：http://uga.jlsjyb.cn

Py:   try: f()⏎finally: cleanup()
来源：http://fys.birdmap.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://rgw.zdbjq.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://smf.nwbrower.top

TS:   try { f(); } finally { cleanup(); }
来源：http://kai.zhijiandao.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hki.hongshengwenyu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://vwg.zhiwuduotai.top

Ruby: begin; f; ensure; cleanup; end
来源：http://xtw.aizwys.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ids.shzxlz.cn

[H03] 主动抛出异常
来源：http://znj.52xcode.cn

Py:   raise ValueError("错误信息")
来源：http://wfe.redwolf501.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lwj.xylfe.cn

JS:   throw new Error("错误信息");
来源：http://bfe.jianghu66.top

TS:   throw new Error("错误信息");
来源：http://xzq.jyoumei.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rcj.vqdsnc.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hnx.cheryme.top

Ruby: raise ArgumentError, "错误信息"
来源：http://udl.havefunace.top

C#:   throw new ArgumentException("错误信息");
来源：http://hqk.zhiwuduotai.top

[H04] 自定义异常类型
来源：http://gbn.hcnkem.com

Py:   class MyError(Exception): pass
来源：http://kvn.hfpthk.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tkj.jinghuilouyu.cn

JS:   class MyError extends Error {}
来源：http://xcm.daria6918.cn

TS:   class MyError extends Error {}
来源：http://lzw.uphjek.com

Java: class MyException extends RuntimeException {}
来源：http://ayi.shuidangran.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jir.zhaomingkeji.xyz

Ruby: class MyError < StandardError; end
来源：http://kht.iojbl.cn

C#:   class MyException : Exception {}
来源：http://zaz.zhiwuduotai.top

[H05] 捕获特定类型
来源：http://tep.iojbl.cn

Py:   except ValueError as e:
来源：http://tax.shuidangran.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yfh.fehbvm.com

JS:   if (e instanceof TypeError) {}
来源：http://oir.sweek.top

TS:   if (e instanceof TypeError) {}
来源：http://sov.yueranfly.top

Java: catch (IOException | SQLException e) {}
来源：http://mrs.jiagoushi.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dti.hcnkem.com

Ruby: rescue ArgumentError => e
来源：http://dhp.jianghu66.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://neu.tanke756.top

[H06] 可选值 / 空值安全访问
来源：http://ziy.9152youxi.cn

Py:   value = d.get("k") or default
来源：http://cqe.yj20258.top

PHP:  $v = $d["k"] ?? null;
来源：http://zlu.0kj1m.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ikw.daxiang520.top

TS:   obj?.a?.b;  d ?? default
来源：http://lmr.havefunace.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nes.nanxuanxn.top

Go:   if v, ok := m["k"]; ok { }
来源：http://eto.hnxiangtu.top

Ruby: d&.dig(:a, :b)
来源：http://iky.tarul.cn

C#:   obj?.A?.B ?? default
来源：http://rnt.ydjk.org.cn

[H07] 断言
来源：http://vav.wangshuangyany.cn

Py:   assert x > 0, "必须为正"
来源：http://mjr.haohaochexian.top

PHP:  assert($x > 0);
来源：http://vdl.jinghuilouyu.cn

JS:   console.assert(x > 0);
来源：http://cmu.zycfv.cn

TS:   console.assert(x > 0);
来源：http://zux.snrcjt.cn

Java: assert x > 0 : "必须为正";
来源：http://piv.hesvh.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wrh.zhaomingkeji.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://qgw.52xcode.cn

C#:   Debug.Assert(x > 0);
来源：http://ntl.vqdsnc.cn

[H08] 获取错误信息与堆栈
来源：http://fgs.52xcode.cn

Py:   str(e);  traceback.format_exc()
来源：http://occ.hywenlv.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nue.jinqigfzy.top

JS:   e.message;  e.stack
来源：http://yrd.chenjidiqi.icu

TS:   e instanceof Error ? e.message : String(e)
来源：http://skj.vehdjk.com

Java: e.getMessage();  e.printStackTrace()
来源：http://xai.shanyushiyangkeji.top

Go:   err.Error()
来源：http://mtl.yuxming.cn

Ruby: e.message;  e.backtrace
来源：http://lft.hnxiangtu.top

C#:   e.Message;  e.StackTrace
来源：http://mgl.uphjek.com

[H09] 带错误码的异常
来源：http://xyt.sysykeji.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lrd.zhaomingkeji.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://tiy.quarkkingdee.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dow.c1oappe.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qpq.epnwcf.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://iak.xinyue.icu

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kyu.hesvh.cn

Ruby: raise MyError.new("fail", 500)
来源：http://kxy.dashuyun.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://miu.nanxuanxn.top

[H10] 资源自动释放
来源：http://dmn.yangfankeji.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://eoz.hesvh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dxa.cashguo.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hnd.cashguo.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jta.shzxlz.cn


<!-- 参考信息 -->