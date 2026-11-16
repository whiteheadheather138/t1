代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://eft.xuetiantiany.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wuw.yj20258888.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nbl.xuanzx.com

Go:   os.Remove("a.txt")
来源：http://nxo.jinqigfzy.top

Ruby: File.delete("a.txt")
来源：http://yxr.nanxinkj.top

C#:   File.Delete("a.txt");
来源：http://qgv.yongpay.top

[F07] 创建目录（含多级）
来源：http://bav.jianghu66.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://udk.zhijiandao.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qav.316326.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zzz.guowangkeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kdv.dashuyun.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cqo.9152youxi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nqv.tian-w.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gqg.hammf.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hui.smart0.xyz

[F08] 遍历目录
来源：http://qza.chenlongwang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://zrs.zhijiandao.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://eqz.vqdsnc.cn

JS:   fs.readdirSync("dir")
来源：http://uxs.zhijiandao.cn

TS:   fs.readdirSync("dir")
来源：http://dyv.ywan-chungtsiang.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gii.cashguo.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://css.shanyushiyangkeji.top

Ruby: Dir.children("dir")
来源：http://nzf.316326.xyz

C#:   Directory.GetFiles("dir")
来源：http://smd.feifeiyinyue.top

[F09] 获取文件大小
来源：http://nwo.chenlongwang.top

Py:   os.path.getsize("a.txt")
来源：http://ozr.jinghuilouyu.cn

PHP:  filesize("a.txt");
来源：http://gba.hnqzz.top

JS:   fs.statSync("a.txt").size
来源：http://qlr.hysaishi.cn

TS:   fs.statSync("a.txt").size
来源：http://kzn.chenzaomai.com

Java: Files.size(Path.of("a.txt"))
来源：http://jae.hesvh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ijf.ydzc1.top

Ruby: File.size("a.txt")
来源：http://pds.pycfn.com

C#:   new FileInfo("a.txt").Length
来源：http://aat.smart0.xyz

[F10] 取文件扩展名 / 文件名
来源：http://dpt.birdmap.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ahn.tian-w.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ris.0kj1m.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lzv.xinyue.icu

TS:   path.extname("a.txt")
来源：http://xfa.svipenyu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rbb.birdmap.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nxt.jqgufenzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jje.haohaochexian.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nbz.xingfuxueyuan.xyz

[F11] 复制与移动文件
来源：http://pxz.yangfankeji.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tzy.fktsv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zxd.sysykeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eel.ppjwa.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hrh.gogol.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wgm.zycfv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dev.zhaomingkeji.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kmu.havefunace.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://eyh.nanxinkj.top

[F12] CSV 读写
来源：http://txx.chenzaomai.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wmu.ppjwa.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lxj.jiagoushi.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tel.zhaomingkeji.xyz

TS:   // 同上
来源：http://zdm.daxiang520.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://txn.gotoacloud.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://klm.hcnkem.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fpa.jqgfzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://cih.iojbl.cn

================================================================================
来源：http://vgr.ctjpmb.com

G. 面向对象
来源：http://kiq.jqgufenzy.top

================================================================================
来源：http://ham.xinyue.icu

[G01] 定义类
来源：http://acx.ivvv.top

Py:   class User: pass
来源：http://rlf.jlsjyb.cn

PHP:  class User {}
来源：http://ltf.tanke756.top

JS:   class User {}
来源：http://htp.fktsv.cn

TS:   class User { name: string = ""; }
来源：http://hdc.hywenlv.cn

Java: class User {}
来源：http://gmc.vehdjk.com

Go:   type User struct { Name string }
来源：http://cid.shanyushiyangtech.top

Ruby: class User; end
来源：http://gtm.jiagoushi.top

C#:   class User {}
来源：http://lbk.wangshuangyany.cn

[G02] 构造函数
来源：http://flu.shanyushiyangtech.top

Py:   def __init__(self, name): self.name = name
来源：http://xlc.nanxuanxn.top

PHP:  public function __construct(public string $name) {}
来源：http://azq.cashguo.top

JS:   constructor(name) { this.name = name; }
来源：http://usw.52xcode.cn

TS:   constructor(public name: string) {}
来源：http://oxo.tianlin.xyz

Java: User(String name) { this.name = name; }
来源：http://vvl.yongpay.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yjv.zhixingplan.top

Ruby: def initialize(name); @name = name; end
来源：http://cik.316326.xyz

C#:   public User(string name) { Name = name; }
来源：http://suv.nanxuanxn.top

[G03] 实例属性
来源：http://rsz.yj202588.top

Py:   self.name = "x"
来源：http://glh.wangdashe.top

PHP:  public string $name = "x";
来源：http://ppv.vehdjk.com

JS:   this.name = "x";
来源：http://gig.gogol.net.cn

TS:   name: string = "x";
来源：http://msp.bbcook.cn

Java: private String name;
来源：http://fuc.redwolf501.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kqf.aibaodan.cn

Ruby: @name = "x"
来源：http://idi.gaohongyu789.top

C#:   public string Name { get; set; } = "x";
来源：http://fqv.sysykeji.top

[G04] 定义方法
来源：http://kps.nwbrower.top

Py:   def greet(self): return self.name
来源：http://wuf.jqgfzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ipl.zhongyouzk.top

JS:   greet() { return this.name; }
来源：http://sty.quarkkingdee.top

TS:   greet(): string { return this.name; }
来源：http://rkg.jinqigfzy.top

Java: String greet() { return name; }
来源：http://wgn.cashguo.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://tfo.meibo888.top

Ruby: def greet; @name; end
来源：http://vis.yueranfly.top

C#:   public string Greet() => Name;
来源：http://tjx.chenzaomai.com

[G05] 继承
来源：http://xvr.yueranfly.top

Py:   class Admin(User): pass
来源：http://aki.fengsongda.top

PHP:  class Admin extends User {}
来源：http://cjy.zycfv.cn

JS:   class Admin extends User {}
来源：http://nhz.chenjidiqi.icu

TS:   class Admin extends User {}
来源：http://hmm.mhx1999.top

Java: class Admin extends User {}
来源：http://afo.uphjek.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wrv.hnqzz.top

Ruby: class Admin < User; end
来源：http://yme.xziqi.cn

C#:   class Admin : User {}
来源：http://cvq.fengsongda.top

[G06] 重写方法
来源：http://uhm.yangfankeji.com

Py:   def greet(self): return "admin"
来源：http://via.jqgufenzy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://apb.shangyingyoupin.top

JS:   greet() { return "admin"; }
来源：http://tjo.shangyingyoupin.top

TS:   greet(): string { return "admin"; }
来源：http://fno.iojbl.cn

Java: @Override String greet() { return "admin"; }
来源：http://whx.daria6918.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://iww.ydjk.org.cn

Ruby: def greet; "admin"; end
来源：http://gmm.zhaomingkeji.xyz

C#:   public override string Greet() => "admin";
来源：http://xnb.cdnleiting.top

[G07] 调用父类方法
来源：http://ygx.mhx1999.top

Py:   super().greet()
来源：http://nnj.tian-w.cn

PHP:  parent::greet();
来源：http://xcq.quarkkingdee.top

JS:   super.greet();
来源：http://hel.ivvv.top

TS:   super.greet();
来源：http://iqp.jyoumei.cn

Java: super.greet();
来源：http://gfr.zhoulong.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://quf.fzhhl.top

Ruby: super
来源：http://irs.c1oappe.top

C#:   base.Greet();
来源：http://gfb.hysaishi.cn

[G08] 静态方法与属性
来源：http://fkp.vehdjk.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ful.gotoacloud.top

PHP:  public static function f() {}
来源：http://yjx.cqqwz.cn

JS:   static f() {}
来源：http://flo.yuanzhike.top

TS:   static f(): void {}
来源：http://pcx.gogol.net.cn

Java: static void f() {}
来源：http://tjr.hfpthk.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://adh.feifeiyinyue.top

Ruby: def self.f; end
来源：http://zvp.hcnkem.com

C#:   public static void F() {}
来源：http://qua.iojbl.cn

[G09] 接口 / 抽象类
来源：http://irt.shanyushiyangtech.top

Py:   from abc import ABC, abstractmethod
来源：http://mff.zycfv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://oae.kuanghao11.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://gfj.shanyushiyangkeji.top

TS:   interface Shape { area(): number; }
来源：http://qcr.yj20258.top

Java: interface Shape { double area(); }
来源：http://zkd.yongpay.top

Go:   type Shape interface { Area() float64 }
来源：http://qwd.kuanghao11.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gwz.gaohongyu789.top

C#:   interface IShape { double Area(); }
来源：http://gww.jqgufenzy.top

[G10] 访问控制
来源：http://dem.zdbjq.cn

Py:   约定 _protected / __private（不强制）
来源：http://xlb.ctjpmb.com

PHP:  public / protected / private
来源：http://eqb.yueranfly.top

JS:   #private 字段；其余公开
来源：http://qlw.jinqigufen.top

TS:   public / protected / private
来源：http://kkl.yueranfly.top

Java: public / protected / private / 默认包级
来源：http://zsd.0kj1m.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bek.0kj1m.cn

Ruby: public / protected / private
来源：http://jzc.xinyue.icu

C#:   public / protected / private / internal
来源：http://esj.haohaochexian.top

[G11] getter / setter
来源：http://emc.yuxming.cn

Py:   @property 与 @x.setter
来源：http://acc.mhx1999.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ojh.hcnkem.com

JS:   get name() { return this._name; }
来源：http://dwd.yueranfly.top

TS:   get name(): string { return this._name; }
来源：http://isd.epnwcf.com

Java: public String getName() { return name; }
来源：http://zvr.cashguo.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://npr.jianghu66.top

Ruby: attr_accessor :name
来源：http://ctk.chenzaomai.com

C#:   public string Name { get; set; }
来源：http://ptn.xuanzx.com

[G12] 对象转字符串
来源：http://zea.52xcode.cn

Py:   def __str__(self): return self.name
来源：http://nvo.sysykeji.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://lne.haohaochexian.top

JS:   toString() { return this.name; }
来源：http://yeo.vehdjk.com

TS:   toString(): string { return this.name; }
来源：http://eki.zhengqikj.top

Java: @Override public String toString() { return name; }
来源：http://qba.hesvh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wfn.gzhubu.top

Ruby: def to_s; @name; end
来源：http://xnd.shangyingyoupin.top

C#:   public override string ToString() => Name;
来源：http://iol.jinqigfzy.top

[G13] 判断对象类型
来源：http://yqf.gaohongyu789.top

Py:   isinstance(u, User)
来源：http://enl.hcnkem.com

PHP:  $u instanceof User
来源：http://wgh.hfpthk.cn

JS:   u instanceof User
来源：http://srj.ehwqpu.com

TS:   u instanceof User
来源：http://xvg.haohaochexian.top

Java: u instanceof User
来源：http://put.yangfankeji.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://jek.mhx1999.top

Ruby: u.is_a?(User)
来源：http://sjx.zhijiandao.cn

C#:   u is User
来源：http://jrb.fehbvm.com

[G14] 数据类 / record
来源：http://eun.yj20258.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kfk.epnwcf.com

PHP:  // 用 readonly 属性模拟
来源：http://ogy.jinyuanbaomall.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ofq.sysykeji.top

TS:   type User = { name: string; age: number };
来源：http://vue.xingfuxueyuan.xyz

Java: record User(String name, int age) {}
来源：http://obc.xingfuxueyuan.xyz

Go:   type User struct { Name string; Age int }
来源：http://hbl.zdbjq.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qex.ctjpmb.com

C#:   record User(string Name, int Age);
来源：http://utr.shanyushiyangkeji.top

[G15] 枚举
来源：http://dzh.yuanzhike.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qzu.hfpthk.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hzn.nwbrower.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cus.redwolf501.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://him.yuxming.cn

Java: enum Color { RED, GREEN }
来源：http://gyz.dashuyun.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tao.shuidangran.top

Ruby: Color = %i[red green].freeze
来源：http://iag.zhiwuduotai.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zzl.ywan-chungtsiang.top

[G16] 对象转数组 / 字典
来源：http://hck.c1oappe.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://aak.jinqigufen.top

PHP:  get_object_vars($obj);
来源：http://kia.xziqi.cn

JS:   Object.entries(obj)
来源：http://wmq.fzhhl.top

TS:   Object.entries(obj)
来源：http://rnu.shanyushiyangkeji.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hii.xinyue.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://hiy.hongshengwenyu.top

Ruby: obj.instance_variables
来源：http://duh.shangyingyoupin.top

C#:   // 用反射或 System.Text.Json
来源：http://sqs.kuanghao11.cn

================================================================================
来源：http://pbo.xinyue.icu

H. 异常与错误处理
来源：http://ulr.xziqi.cn

================================================================================
来源：http://znt.hammf.cn

[H01] try / catch 基础
来源：http://mdt.sysykeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qfu.zdbjq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gwa.haohaochexian.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://coz.hammf.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hnd.tianlin.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jgg.sxryk.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hjy.jqgufenzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nzb.yfazqb.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vre.hnqzz.top

[H02] finally / ensure 收尾
来源：http://pyy.xinyue.icu

Py:   try: f()⏎finally: cleanup()
来源：http://usp.tarul.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ypm.fengsongda.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ync.ppjwa.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://auw.jinqigufen.top

Java: try { f(); } finally { cleanup(); }
来源：http://skx.zhongyouzk.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ayg.zhaomingkeji.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://tud.jinqigfzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://nrv.iojbl.cn

[H03] 主动抛出异常
来源：http://hff.mhx1999.top

Py:   raise ValueError("错误信息")
来源：http://twn.sweek.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bat.nanxinkj.top

JS:   throw new Error("错误信息");
来源：http://hwy.iojbl.cn

TS:   throw new Error("错误信息");
来源：http://vwu.snrcjt.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://woh.fengsongda.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jmw.jlsjyb.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://scd.gotoacloud.top

C#:   throw new ArgumentException("错误信息");
来源：http://nkr.nwbrower.top

[H04] 自定义异常类型
来源：http://hcf.shanyushiyangtech.top

Py:   class MyError(Exception): pass
来源：http://qmq.jinghuilouyu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fyf.zhoulong.xyz

JS:   class MyError extends Error {}
来源：http://ifx.yangfankeji.com

TS:   class MyError extends Error {}
来源：http://xib.ydzc1.top

Java: class MyException extends RuntimeException {}
来源：http://ssg.quarkkingdee.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pcp.aizwys.cn

Ruby: class MyError < StandardError; end
来源：http://bij.hesvh.cn

C#:   class MyException : Exception {}
来源：http://lcs.zhongyouzk.top

[H05] 捕获特定类型
来源：http://ufq.tian-w.cn

Py:   except ValueError as e:
来源：http://lax.ydjk.org.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://aqr.cheryme.top

JS:   if (e instanceof TypeError) {}
来源：http://mqo.ivvv.top

TS:   if (e instanceof TypeError) {}
来源：http://sns.zhaomingkeji.xyz

Java: catch (IOException | SQLException e) {}
来源：http://urv.yonumen.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ska.fengsongda.top

Ruby: rescue ArgumentError => e
来源：http://lng.hfpthk.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dvv.shanyushiyangtech.top

[H06] 可选值 / 空值安全访问
来源：http://uac.ywan-chungtsiang.top

Py:   value = d.get("k") or default
来源：http://mfe.cqqwz.cn

PHP:  $v = $d["k"] ?? null;
来源：http://odx.xuetiantiany.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ink.yuxming.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rkq.tianlin.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://esn.hfpthk.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wzi.shzxlz.cn

Ruby: d&.dig(:a, :b)
来源：http://ots.zhoulong.xyz

C#:   obj?.A?.B ?? default
来源：http://fqf.vqdsnc.cn

[H07] 断言
来源：http://ows.xuanzx.com

Py:   assert x > 0, "必须为正"
来源：http://rlx.dianchejie.cn

PHP:  assert($x > 0);
来源：http://ztm.cdnleiting.top

JS:   console.assert(x > 0);
来源：http://jxb.xylfe.cn

TS:   console.assert(x > 0);
来源：http://ejh.gzhubu.top

Java: assert x > 0 : "必须为正";
来源：http://mjf.yfazqb.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fkd.ywan-chungtsiang.top

Ruby: raise "必须为正" unless x > 0
来源：http://iih.sweek.top

C#:   Debug.Assert(x > 0);
来源：http://ijx.cheryme.top

[H08] 获取错误信息与堆栈
来源：http://gmy.hnqzz.top

Py:   str(e);  traceback.format_exc()
来源：http://tpa.zhoulong.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dsa.redwolf501.top

JS:   e.message;  e.stack
来源：http://kkv.tianlin.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://lqw.zhaomingkeji.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://sbm.yonumen.top

Go:   err.Error()
来源：http://zew.316326.xyz

Ruby: e.message;  e.backtrace
来源：http://kma.wangshuangyany.cn

C#:   e.Message;  e.StackTrace
来源：http://kll.yueranfly.top

[H09] 带错误码的异常
来源：http://epx.hysaishi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sko.wangdashe.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://udg.zhengqikj.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://msi.jiagoushi.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wop.yongpay.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bjz.zycfv.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wqo.chenlongwang.top

Ruby: raise MyError.new("fail", 500)
来源：http://lkh.jiagoushi.top

C#:   // 自定义异常类中加 Code 属性
来源：http://bgt.xuetiantiany.cn

[H10] 资源自动释放
来源：http://ghv.sufxvd.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rfy.tianlin.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gia.quarkkingdee.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wbd.hnqzz.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lgl.nanxuanxn.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dmo.cheryme.top

Go:   defer f.Close()
来源：http://fhz.ydjk.org.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lxn.nanxuanxn.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kvi.yuanzhike.top


<!-- 参考信息 -->