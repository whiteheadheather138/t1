代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://wvd.tarul.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yuo.yj202588.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://iug.feifeiyinyue.top

Go:   os.Remove("a.txt")
来源：http://ffd.pengpengdd.cyou

Ruby: File.delete("a.txt")
来源：http://nkf.dashuyun.cn

C#:   File.Delete("a.txt");
来源：http://mtq.tanke756.top

[F07] 创建目录（含多级）
来源：http://duj.sysykeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nlm.guannengcc.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uwi.jinyuanbaomall.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pdy.andypj.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rid.shangyingyoupin.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dun.shzxlz.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vfg.yj202588.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hfg.vehdjk.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ccg.smart0.xyz

[F08] 遍历目录
来源：http://mft.pycfn.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://ife.gotoacloud.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ubw.pycfn.com

JS:   fs.readdirSync("dir")
来源：http://uvz.fanxiaobao.xyz

TS:   fs.readdirSync("dir")
来源：http://ube.shzxlz.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qqi.yueranfly.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://tpa.zhoulong.xyz

Ruby: Dir.children("dir")
来源：http://tgw.quarkkingdee.top

C#:   Directory.GetFiles("dir")
来源：http://qto.daxiang520.top

[F09] 获取文件大小
来源：http://qne.yongpay.top

Py:   os.path.getsize("a.txt")
来源：http://ayg.ivvv.top

PHP:  filesize("a.txt");
来源：http://hvr.sjlbkw.cn

JS:   fs.statSync("a.txt").size
来源：http://xyy.tian-w.cn

TS:   fs.statSync("a.txt").size
来源：http://ssg.birdmap.top

Java: Files.size(Path.of("a.txt"))
来源：http://qar.tian-w.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pub.yuanzhike.top

Ruby: File.size("a.txt")
来源：http://myz.tarul.cn

C#:   new FileInfo("a.txt").Length
来源：http://kpf.sweek.top

[F10] 取文件扩展名 / 文件名
来源：http://dti.shzxlz.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://srn.guowangkeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rqk.xziqi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uci.mhx1999.top

TS:   path.extname("a.txt")
来源：http://mua.xingfuxueyuan.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mrn.yuanzhike.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fgb.aibaodan.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tor.hysaishi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ejd.fanxiaobao.xyz

[F11] 复制与移动文件
来源：http://zdr.feifeiyinyue.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://elc.yonumen.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://okf.ivvv.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://syj.zhiwuduotai.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gbe.yfazqb.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ggk.xuetiantiany.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tfx.fanxiaobao.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pbk.wangdashe.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xdd.shuidangran.top

[F12] CSV 读写
来源：http://seu.bjfxy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hhc.jiagoushi.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ayi.cqqwz.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ysd.svipenyu.cn

TS:   // 同上
来源：http://gev.uphjek.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://txe.aibaodan.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://urr.fehbvm.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ztj.hnqzz.top

C#:   // 无内置：用 CsvHelper 库
来源：http://myi.wangshuangyany.cn

================================================================================
来源：http://mhq.tian-w.cn

G. 面向对象
来源：http://bzu.meibo888.top

================================================================================
来源：http://axx.yanxiufei.cn

[G01] 定义类
来源：http://tbo.gaohongyu789.top

Py:   class User: pass
来源：http://ath.zhoulong.xyz

PHP:  class User {}
来源：http://dcb.cdnleiting.top

JS:   class User {}
来源：http://bmn.yuanzhike.top

TS:   class User { name: string = ""; }
来源：http://kcl.ehwqpu.com

Java: class User {}
来源：http://mjk.hywenlv.cn

Go:   type User struct { Name string }
来源：http://lds.fanxiaobao.xyz

Ruby: class User; end
来源：http://cpo.epnwcf.com

C#:   class User {}
来源：http://lic.yueranfly.top

[G02] 构造函数
来源：http://yur.nanxinkj.top

Py:   def __init__(self, name): self.name = name
来源：http://mbw.sweek.top

PHP:  public function __construct(public string $name) {}
来源：http://vbo.gotoacloud.top

JS:   constructor(name) { this.name = name; }
来源：http://qls.feifeiyinyue.top

TS:   constructor(public name: string) {}
来源：http://par.yuxming.cn

Java: User(String name) { this.name = name; }
来源：http://gnh.tanke756.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://syn.hesvh.cn

Ruby: def initialize(name); @name = name; end
来源：http://vvl.sufxvd.cn

C#:   public User(string name) { Name = name; }
来源：http://rit.ivvv.top

[G03] 实例属性
来源：http://jxp.chenlongwang.top

Py:   self.name = "x"
来源：http://dcv.sweek.top

PHP:  public string $name = "x";
来源：http://axt.redwolf501.top

JS:   this.name = "x";
来源：http://xvw.xinyue.icu

TS:   name: string = "x";
来源：http://qyu.yfazqb.com

Java: private String name;
来源：http://ygo.gzhubu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mlz.uphjek.com

Ruby: @name = "x"
来源：http://hfv.sweek.top

C#:   public string Name { get; set; } = "x";
来源：http://ity.wangshuangyany.cn

[G04] 定义方法
来源：http://zgv.jqgufenzy.top

Py:   def greet(self): return self.name
来源：http://ebn.cashguo.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ynz.cqqwz.cn

JS:   greet() { return this.name; }
来源：http://vtr.zdbjq.cn

TS:   greet(): string { return this.name; }
来源：http://gtw.zhoulong.xyz

Java: String greet() { return name; }
来源：http://lsb.daria6918.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wno.fanxiaobao.xyz

Ruby: def greet; @name; end
来源：http://dyr.xinyue.icu

C#:   public string Greet() => Name;
来源：http://bdm.cashguo.top

[G05] 继承
来源：http://akd.quarkkingdee.top

Py:   class Admin(User): pass
来源：http://vqo.hysaishi.cn

PHP:  class Admin extends User {}
来源：http://bwj.zhiwuduotai.top

JS:   class Admin extends User {}
来源：http://yiq.kuanghao11.cn

TS:   class Admin extends User {}
来源：http://hbj.hywenlv.cn

Java: class Admin extends User {}
来源：http://zfl.yvedp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://iea.xingfuxueyuan.xyz

Ruby: class Admin < User; end
来源：http://suk.hcnkem.com

C#:   class Admin : User {}
来源：http://nvh.shuidangran.top

[G06] 重写方法
来源：http://slt.ydzc1.top

Py:   def greet(self): return "admin"
来源：http://uxi.sysykeji.top

PHP:  public function greet(): string { return "admin"; }
来源：http://fhe.yj20258888.top

JS:   greet() { return "admin"; }
来源：http://xgw.sxryk.cn

TS:   greet(): string { return "admin"; }
来源：http://eak.52xcode.cn

Java: @Override String greet() { return "admin"; }
来源：http://eno.zhixingplan.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hhe.quarkkingdee.top

Ruby: def greet; "admin"; end
来源：http://vyp.gogol.net.cn

C#:   public override string Greet() => "admin";
来源：http://gtp.9152youxi.cn

[G07] 调用父类方法
来源：http://dvp.tarul.cn

Py:   super().greet()
来源：http://ayy.ydjk.org.cn

PHP:  parent::greet();
来源：http://bnl.shangyingyoupin.top

JS:   super.greet();
来源：http://oyi.ydzc1.top

TS:   super.greet();
来源：http://fdo.epnwcf.com

Java: super.greet();
来源：http://kij.hongshengwenyu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ofc.nwbrower.top

Ruby: super
来源：http://ehi.52xcode.cn

C#:   base.Greet();
来源：http://mre.ydjk.org.cn

[G08] 静态方法与属性
来源：http://ptp.sweek.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pbl.9152youxi.cn

PHP:  public static function f() {}
来源：http://npu.gotoacloud.top

JS:   static f() {}
来源：http://iky.zycfv.cn

TS:   static f(): void {}
来源：http://ftu.epnwcf.com

Java: static void f() {}
来源：http://edh.haohaochexian.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://uar.yonumen.top

Ruby: def self.f; end
来源：http://ffu.xuanzx.com

C#:   public static void F() {}
来源：http://hgs.guannengcc.top

[G09] 接口 / 抽象类
来源：http://yld.yj202588.top

Py:   from abc import ABC, abstractmethod
来源：http://oep.bjfxy.top

PHP:  interface Shape { public function area(): float; }
来源：http://prk.zhiwuduotai.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ggx.gogol.net.cn

TS:   interface Shape { area(): number; }
来源：http://nyf.zhaomingkeji.xyz

Java: interface Shape { double area(); }
来源：http://dtt.yangfankeji.com

Go:   type Shape interface { Area() float64 }
来源：http://vsy.52xcode.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xtv.cheryme.top

C#:   interface IShape { double Area(); }
来源：http://fvx.yanxiufei.cn

[G10] 访问控制
来源：http://jiv.hywenlv.cn

Py:   约定 _protected / __private（不强制）
来源：http://mjp.dashuyun.cn

PHP:  public / protected / private
来源：http://nik.zhixingplan.top

JS:   #private 字段；其余公开
来源：http://tsk.tian-w.cn

TS:   public / protected / private
来源：http://tnu.ppjwa.cn

Java: public / protected / private / 默认包级
来源：http://ghn.shanyushiyangtech.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://pmt.gotoacloud.top

Ruby: public / protected / private
来源：http://vto.xinyue.icu

C#:   public / protected / private / internal
来源：http://gne.zhijiandao.cn

[G11] getter / setter
来源：http://mpr.hnqzz.top

Py:   @property 与 @x.setter
来源：http://qfg.meibo888.top

PHP:  public function getName(): string { return $this->name; }
来源：http://gjo.sjlbkw.cn

JS:   get name() { return this._name; }
来源：http://lov.wangdashe.top

TS:   get name(): string { return this._name; }
来源：http://ono.cqqwz.cn

Java: public String getName() { return name; }
来源：http://rbv.yfazqb.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://okn.jyoumei.cn

Ruby: attr_accessor :name
来源：http://nvu.haohaochexian.top

C#:   public string Name { get; set; }
来源：http://mce.zhengqikj.top

[G12] 对象转字符串
来源：http://hlg.zhijiandao.cn

Py:   def __str__(self): return self.name
来源：http://aib.tianlin.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://fii.zhiwuduotai.top

JS:   toString() { return this.name; }
来源：http://xnf.yuxming.cn

TS:   toString(): string { return this.name; }
来源：http://eya.zhijiandao.cn

Java: @Override public String toString() { return name; }
来源：http://lhn.fengsongda.top

Go:   func (u User) String() string { return u.Name }
来源：http://gnx.mhx1999.top

Ruby: def to_s; @name; end
来源：http://kpk.pycfn.com

C#:   public override string ToString() => Name;
来源：http://rbu.hfpthk.cn

[G13] 判断对象类型
来源：http://hrb.wangshuangyany.cn

Py:   isinstance(u, User)
来源：http://wde.52xcode.cn

PHP:  $u instanceof User
来源：http://okp.bbcook.cn

JS:   u instanceof User
来源：http://jjk.zhengqikj.top

TS:   u instanceof User
来源：http://qkz.hnqzz.top

Java: u instanceof User
来源：http://cmz.ywan-chungtsiang.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://eay.vehdjk.com

Ruby: u.is_a?(User)
来源：http://ahn.redwolf501.top

C#:   u is User
来源：http://ajf.zhaomingkeji.xyz

[G14] 数据类 / record
来源：http://krt.sufxvd.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uxc.tian-w.cn

PHP:  // 用 readonly 属性模拟
来源：http://rsj.fzhhl.top

JS:   // 无内置：普通类或对象字面量
来源：http://qdl.zdqjudy.top

TS:   type User = { name: string; age: number };
来源：http://lyo.dashuyun.cn

Java: record User(String name, int age) {}
来源：http://uma.snrcjt.cn

Go:   type User struct { Name string; Age int }
来源：http://wif.bjfxy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xup.yuxming.cn

C#:   record User(string Name, int Age);
来源：http://bxj.hammf.cn

[G15] 枚举
来源：http://qsj.yj20258.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tym.jqgfzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://sgf.zycfv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xns.jinqigufen.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sdo.cdnleiting.top

Java: enum Color { RED, GREEN }
来源：http://qul.ydzc1.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lit.quarkkingdee.top

Ruby: Color = %i[red green].freeze
来源：http://nlv.ybcxt.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xhm.shangyingyoupin.top

[G16] 对象转数组 / 字典
来源：http://hlp.zhoulong.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jib.xylfe.cn

PHP:  get_object_vars($obj);
来源：http://gwu.daria6918.cn

JS:   Object.entries(obj)
来源：http://irr.yj20258.top

TS:   Object.entries(obj)
来源：http://dps.zhoulong.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hvt.yuanzhike.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://rpq.cashguo.top

Ruby: obj.instance_variables
来源：http://kne.smart0.xyz

C#:   // 用反射或 System.Text.Json
来源：http://flh.zdqjudy.top

================================================================================
来源：http://znh.0kj1m.cn

H. 异常与错误处理
来源：http://kht.yj202588.top

================================================================================
来源：http://tcg.tian-w.cn

[H01] try / catch 基础
来源：http://siu.havefunace.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hzy.yj202588.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bop.nanxinkj.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://twi.shzxlz.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ske.fzhhl.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gky.mhx1999.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vsd.meibo888.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://oea.meibo888.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xkn.jinghuilouyu.cn

[H02] finally / ensure 收尾
来源：http://ppe.redwolf501.top

Py:   try: f()⏎finally: cleanup()
来源：http://obm.epnwcf.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://wki.ydjk.org.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://vqf.zhongyouzk.top

TS:   try { f(); } finally { cleanup(); }
来源：http://wwe.wangshuangyany.cn

Java: try { f(); } finally { cleanup(); }
来源：http://uym.jqgfzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://gre.wangdashe.top

Ruby: begin; f; ensure; cleanup; end
来源：http://xrn.meibo888.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://sxn.zdbjq.cn

[H03] 主动抛出异常
来源：http://bdp.yuxming.cn

Py:   raise ValueError("错误信息")
来源：http://vkc.gogol.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hig.ctjpmb.com

JS:   throw new Error("错误信息");
来源：http://kgb.shzxlz.cn

TS:   throw new Error("错误信息");
来源：http://znx.zhixingplan.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://tax.jqgufenzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pbu.hammf.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ane.yj20258.top

C#:   throw new ArgumentException("错误信息");
来源：http://sfs.sysykeji.top

[H04] 自定义异常类型
来源：http://qgg.cqqwz.cn

Py:   class MyError(Exception): pass
来源：http://ons.ehwqpu.com

PHP:  class MyError extends RuntimeException {}
来源：http://ioq.kuanghao11.cn

JS:   class MyError extends Error {}
来源：http://pma.nanxuanxn.top

TS:   class MyError extends Error {}
来源：http://nsz.yueranfly.top

Java: class MyException extends RuntimeException {}
来源：http://cuh.hnxiangtu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ejq.zhoulong.xyz

Ruby: class MyError < StandardError; end
来源：http://akv.iojbl.cn

C#:   class MyException : Exception {}
来源：http://edz.sxryk.cn

[H05] 捕获特定类型
来源：http://llg.jinqigfzy.top

Py:   except ValueError as e:
来源：http://srt.iojbl.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xck.zycfv.cn

JS:   if (e instanceof TypeError) {}
来源：http://wwj.zhiwuduotai.top

TS:   if (e instanceof TypeError) {}
来源：http://juu.shuidangran.top

Java: catch (IOException | SQLException e) {}
来源：http://mer.vehdjk.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://edq.mhx1999.top

Ruby: rescue ArgumentError => e
来源：http://wia.xuanzx.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://few.yangfankeji.com

[H06] 可选值 / 空值安全访问
来源：http://dbp.yj20258.top

Py:   value = d.get("k") or default
来源：http://mma.hongshengwenyu.top

PHP:  $v = $d["k"] ?? null;
来源：http://qag.ctjpmb.com

JS:   obj?.a?.b;  d ?? default
来源：http://vnw.tarul.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ycs.gzhubu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mvz.xuetiantiany.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vzq.zhaomingkeji.xyz

Ruby: d&.dig(:a, :b)
来源：http://xuk.vehdjk.com

C#:   obj?.A?.B ?? default
来源：http://xst.yanxiufei.cn

[H07] 断言
来源：http://ovw.zhiwuduotai.top

Py:   assert x > 0, "必须为正"
来源：http://ovo.jiagoushi.top

PHP:  assert($x > 0);
来源：http://qfj.yueranfly.top

JS:   console.assert(x > 0);
来源：http://xde.zhengqikj.top

TS:   console.assert(x > 0);
来源：http://hsr.c1oappe.top

Java: assert x > 0 : "必须为正";
来源：http://eqc.sysykeji.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lzt.yvedp.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ldu.zhaomingkeji.xyz

C#:   Debug.Assert(x > 0);
来源：http://ord.jqgfzy.top

[H08] 获取错误信息与堆栈
来源：http://mkq.ctjpmb.com

Py:   str(e);  traceback.format_exc()
来源：http://bos.shzxlz.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dqd.yuanzhike.top

JS:   e.message;  e.stack
来源：http://afr.quarkkingdee.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://qtc.nanxinkj.top

Java: e.getMessage();  e.printStackTrace()
来源：http://sic.jlsjyb.cn

Go:   err.Error()
来源：http://reg.shangyingyoupin.top

Ruby: e.message;  e.backtrace
来源：http://tls.feifeiyinyue.top

C#:   e.Message;  e.StackTrace
来源：http://bkw.zhixingplan.top

[H09] 带错误码的异常
来源：http://tkc.zhixingplan.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://iic.316326.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://kpt.jianghu66.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hgr.gaohongyu789.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zzx.meibo888.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tdt.chenjidiqi.icu

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zrz.fengsongda.top

Ruby: raise MyError.new("fail", 500)
来源：http://hkt.sufxvd.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://okh.zhoulong.xyz

[H10] 资源自动释放
来源：http://uyt.cashguo.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://nny.nanxuanxn.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qtn.yfazqb.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xye.tianlin.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://urp.316326.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qla.ywan-chungtsiang.top

Go:   defer f.Close()
来源：http://uev.hywenlv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://obk.chenlongwang.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jyb.tian-w.cn


<!-- 参考信息 -->