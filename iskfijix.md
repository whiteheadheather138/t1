代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://avg.zhongyouzk.top

Java: Files.exists(Path.of("a.txt"))
来源：http://utr.gotoacloud.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wai.tian-w.cn

Ruby: File.exist?("a.txt")
来源：http://jyk.smart0.xyz

C#:   File.Exists("a.txt")
来源：http://zam.cqqwz.cn

[F06] 删除文件
来源：http://ddp.cucudq.cn

Py:   os.remove("a.txt")
来源：http://vyj.cashguo.top

PHP:  unlink("a.txt");
来源：http://nov.jinqigfzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://def.xinyue.icu

TS:   fs.unlinkSync("a.txt")
来源：http://szd.52xcode.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ccl.hnxiangtu.top

Go:   os.Remove("a.txt")
来源：http://jwr.pycfn.com

Ruby: File.delete("a.txt")
来源：http://rpv.tianlin.xyz

C#:   File.Delete("a.txt");
来源：http://bfy.chenjidiqi.icu

[F07] 创建目录（含多级）
来源：http://lpm.yonumen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://akk.tarul.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wdl.9152youxi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gka.zdqjudy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://duc.zhijiandao.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fwn.xziqi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xyd.xingfuxueyuan.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uuz.ehwqpu.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://eoc.chenlongwang.top

[F08] 遍历目录
来源：http://dry.guowangkeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://wzw.cdnleiting.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://htz.tian-w.cn

JS:   fs.readdirSync("dir")
来源：http://aev.gogol.net.cn

TS:   fs.readdirSync("dir")
来源：http://agk.shangyingyoupin.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qtj.yvedp.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://tfo.ywan-chungtsiang.top

Ruby: Dir.children("dir")
来源：http://ujo.jlsjyb.cn

C#:   Directory.GetFiles("dir")
来源：http://erh.shangyingyoupin.top

[F09] 获取文件大小
来源：http://tbo.xingfuxueyuan.xyz

Py:   os.path.getsize("a.txt")
来源：http://bfu.gotoacloud.top

PHP:  filesize("a.txt");
来源：http://okb.jiagoushi.top

JS:   fs.statSync("a.txt").size
来源：http://vby.fanxiaobao.xyz

TS:   fs.statSync("a.txt").size
来源：http://gsl.nanxinkj.top

Java: Files.size(Path.of("a.txt"))
来源：http://gzx.shanyushiyangkeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://njk.zdbjq.cn

Ruby: File.size("a.txt")
来源：http://fdh.hammf.cn

C#:   new FileInfo("a.txt").Length
来源：http://fvu.jinqigfzy.top

[F10] 取文件扩展名 / 文件名
来源：http://sac.shuidangran.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://orb.zhengqikj.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uuv.yuanzhike.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wxd.jinyuanbaomall.cn

TS:   path.extname("a.txt")
来源：http://bhi.havefunace.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hju.ywan-chungtsiang.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qwi.jqgfzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://clt.sweek.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rrd.daxiang520.top

[F11] 复制与移动文件
来源：http://pvi.xziqi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mlp.hongshengwenyu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xxa.cucudq.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hil.fzhhl.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lep.shanyushiyangkeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xvk.jyoumei.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dvj.shanyushiyangtech.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://eah.yuxming.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uvz.xinyue.icu

[F12] CSV 读写
来源：http://pxc.ppjwa.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zjo.ybcxt.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yxu.cqqwz.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zko.havefunace.top

TS:   // 同上
来源：http://dmw.jqgfzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://psw.shanyushiyangkeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jrz.ehwqpu.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://anx.sufxvd.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pux.ydjk.org.cn

================================================================================
来源：http://ymf.pycfn.com

G. 面向对象
来源：http://ici.andypj.xyz

================================================================================
来源：http://ssc.xuanzx.com

[G01] 定义类
来源：http://ynx.sjlbkw.cn

Py:   class User: pass
来源：http://hjg.yuxming.cn

PHP:  class User {}
来源：http://qvc.gogol.net.cn

JS:   class User {}
来源：http://wzf.daria6918.cn

TS:   class User { name: string = ""; }
来源：http://ehe.epnwcf.com

Java: class User {}
来源：http://jry.havefunace.top

Go:   type User struct { Name string }
来源：http://yon.ivvv.top

Ruby: class User; end
来源：http://tho.sufxvd.cn

C#:   class User {}
来源：http://fcs.cdnleiting.top

[G02] 构造函数
来源：http://dzc.svipenyu.cn

Py:   def __init__(self, name): self.name = name
来源：http://ixx.sxryk.cn

PHP:  public function __construct(public string $name) {}
来源：http://plx.smart0.xyz

JS:   constructor(name) { this.name = name; }
来源：http://wur.jyoumei.cn

TS:   constructor(public name: string) {}
来源：http://dve.zhoulong.xyz

Java: User(String name) { this.name = name; }
来源：http://uia.tianlin.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vhc.0kj1m.cn

Ruby: def initialize(name); @name = name; end
来源：http://lvy.zhengqikj.top

C#:   public User(string name) { Name = name; }
来源：http://qiq.cqqwz.cn

[G03] 实例属性
来源：http://eso.chenjidiqi.icu

Py:   self.name = "x"
来源：http://wxn.jlsjyb.cn

PHP:  public string $name = "x";
来源：http://mno.aibaodan.cn

JS:   this.name = "x";
来源：http://aws.ywan-chungtsiang.top

TS:   name: string = "x";
来源：http://bry.bbcook.cn

Java: private String name;
来源：http://xjq.snrcjt.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ouy.zdqjudy.top

Ruby: @name = "x"
来源：http://cos.shangyingyoupin.top

C#:   public string Name { get; set; } = "x";
来源：http://voy.nanxinkj.top

[G04] 定义方法
来源：http://dfg.ybcxt.top

Py:   def greet(self): return self.name
来源：http://jgx.hywenlv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fyc.zhiwuduotai.top

JS:   greet() { return this.name; }
来源：http://qbi.c1oappe.top

TS:   greet(): string { return this.name; }
来源：http://qfp.wangshuangyany.cn

Java: String greet() { return name; }
来源：http://moi.shanyushiyangtech.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xlr.sjlbkw.cn

Ruby: def greet; @name; end
来源：http://fgg.xziqi.cn

C#:   public string Greet() => Name;
来源：http://mxz.52xcode.cn

[G05] 继承
来源：http://vax.fengsongda.top

Py:   class Admin(User): pass
来源：http://cpw.jianghu66.top

PHP:  class Admin extends User {}
来源：http://whk.hcnkem.com

JS:   class Admin extends User {}
来源：http://mih.shanyushiyangtech.top

TS:   class Admin extends User {}
来源：http://ket.xylfe.cn

Java: class Admin extends User {}
来源：http://the.andypj.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zjc.epnwcf.com

Ruby: class Admin < User; end
来源：http://poi.sufxvd.cn

C#:   class Admin : User {}
来源：http://cma.sysykeji.top

[G06] 重写方法
来源：http://prn.zhijiandao.cn

Py:   def greet(self): return "admin"
来源：http://wtf.fktsv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gct.fzhhl.top

JS:   greet() { return "admin"; }
来源：http://fgr.c1oappe.top

TS:   greet(): string { return "admin"; }
来源：http://suf.zdbjq.cn

Java: @Override String greet() { return "admin"; }
来源：http://qjs.yueranfly.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cdh.vehdjk.com

Ruby: def greet; "admin"; end
来源：http://ibi.fanxiaobao.xyz

C#:   public override string Greet() => "admin";
来源：http://sdj.yj202588.top

[G07] 调用父类方法
来源：http://egn.jinqigufen.top

Py:   super().greet()
来源：http://cgo.yonumen.top

PHP:  parent::greet();
来源：http://nll.zdqjudy.top

JS:   super.greet();
来源：http://rsj.xinyue.icu

TS:   super.greet();
来源：http://ecm.wangshuangyany.cn

Java: super.greet();
来源：http://vqo.zhengqikj.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rru.vqdsnc.cn

Ruby: super
来源：http://ude.cashguo.top

C#:   base.Greet();
来源：http://udy.zhaomingkeji.xyz

[G08] 静态方法与属性
来源：http://vsb.mhx1999.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rvb.cucudq.cn

PHP:  public static function f() {}
来源：http://pxb.meibo888.top

JS:   static f() {}
来源：http://vqb.nanxinkj.top

TS:   static f(): void {}
来源：http://rkp.jianghu66.top

Java: static void f() {}
来源：http://rga.zhengqikj.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://rct.cashguo.top

Ruby: def self.f; end
来源：http://zxj.cucudq.cn

C#:   public static void F() {}
来源：http://lve.cashguo.top

[G09] 接口 / 抽象类
来源：http://qra.9152youxi.cn

Py:   from abc import ABC, abstractmethod
来源：http://tvi.wangdashe.top

PHP:  interface Shape { public function area(): float; }
来源：http://jsp.ppjwa.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://crk.jlsjyb.cn

TS:   interface Shape { area(): number; }
来源：http://uiz.ydjk.org.cn

Java: interface Shape { double area(); }
来源：http://wpb.jlsjyb.cn

Go:   type Shape interface { Area() float64 }
来源：http://dny.mhx1999.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wzr.pengpengdd.cyou

C#:   interface IShape { double Area(); }
来源：http://hff.dashuyun.cn

[G10] 访问控制
来源：http://zpy.mhx1999.top

Py:   约定 _protected / __private（不强制）
来源：http://pej.wangdashe.top

PHP:  public / protected / private
来源：http://zhg.svipenyu.cn

JS:   #private 字段；其余公开
来源：http://qoy.ehwqpu.com

TS:   public / protected / private
来源：http://igg.sysykeji.top

Java: public / protected / private / 默认包级
来源：http://iud.nwbrower.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://hfb.yongpay.top

Ruby: public / protected / private
来源：http://wav.yfazqb.com

C#:   public / protected / private / internal
来源：http://ymw.xuanzx.com

[G11] getter / setter
来源：http://uyy.zycfv.cn

Py:   @property 与 @x.setter
来源：http://bwu.meibo888.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jup.smart0.xyz

JS:   get name() { return this._name; }
来源：http://exi.cashguo.top

TS:   get name(): string { return this._name; }
来源：http://gqg.zycfv.cn

Java: public String getName() { return name; }
来源：http://cqk.yvedp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jab.jinyuanbaomall.cn

Ruby: attr_accessor :name
来源：http://xig.dashuyun.cn

C#:   public string Name { get; set; }
来源：http://zeg.aizwys.cn

[G12] 对象转字符串
来源：http://dgn.shangyingyoupin.top

Py:   def __str__(self): return self.name
来源：http://omt.316326.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://gsk.cdnleiting.top

JS:   toString() { return this.name; }
来源：http://zth.quarkkingdee.top

TS:   toString(): string { return this.name; }
来源：http://rtj.hysaishi.cn

Java: @Override public String toString() { return name; }
来源：http://thu.dashuyun.cn

Go:   func (u User) String() string { return u.Name }
来源：http://arq.yvedp.cn

Ruby: def to_s; @name; end
来源：http://bnz.ybcxt.top

C#:   public override string ToString() => Name;
来源：http://cfm.yj20258888.top

[G13] 判断对象类型
来源：http://lfz.sysykeji.top

Py:   isinstance(u, User)
来源：http://dnr.yj20258888.top

PHP:  $u instanceof User
来源：http://mpn.jlsjyb.cn

JS:   u instanceof User
来源：http://arj.cucudq.cn

TS:   u instanceof User
来源：http://ple.bbcook.cn

Java: u instanceof User
来源：http://ixa.zhiwuduotai.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://nyh.jiagoushi.top

Ruby: u.is_a?(User)
来源：http://ybd.wangshuangyany.cn

C#:   u is User
来源：http://biz.jyoumei.cn

[G14] 数据类 / record
来源：http://dag.jlsjyb.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wmz.ydzc1.top

PHP:  // 用 readonly 属性模拟
来源：http://ttp.yongpay.top

JS:   // 无内置：普通类或对象字面量
来源：http://tfm.sweek.top

TS:   type User = { name: string; age: number };
来源：http://dpr.aibaodan.cn

Java: record User(String name, int age) {}
来源：http://lul.jinqigfzy.top

Go:   type User struct { Name string; Age int }
来源：http://ded.ywan-chungtsiang.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hbl.hammf.cn

C#:   record User(string Name, int Age);
来源：http://yiy.cucudq.cn

[G15] 枚举
来源：http://sut.zdqjudy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fbe.iojbl.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zoa.hysaishi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mvw.iojbl.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fha.zycfv.cn

Java: enum Color { RED, GREEN }
来源：http://hzx.zhoulong.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bvb.xuetiantiany.cn

Ruby: Color = %i[red green].freeze
来源：http://qvf.hywenlv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://krw.yonumen.top

[G16] 对象转数组 / 字典
来源：http://fmg.sysykeji.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://akn.bjfxy.top

PHP:  get_object_vars($obj);
来源：http://osk.yvedp.cn

JS:   Object.entries(obj)
来源：http://fff.zhoulong.xyz

TS:   Object.entries(obj)
来源：http://ivo.pengpengdd.cyou

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://oaa.gotoacloud.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://sxp.fengsongda.top

Ruby: obj.instance_variables
来源：http://afw.svipenyu.cn

C#:   // 用反射或 System.Text.Json
来源：http://ckc.aibaodan.cn

================================================================================
来源：http://pbv.jlsjyb.cn

H. 异常与错误处理
来源：http://jak.zhoulong.xyz

================================================================================
来源：http://myt.jqgfzy.top

[H01] try / catch 基础
来源：http://iam.dianchejie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qyc.cheryme.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://acx.dashuyun.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tto.fzhhl.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jnt.sufxvd.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rkb.cucudq.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nkb.zdqjudy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zci.shuidangran.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rym.tanke756.top

[H02] finally / ensure 收尾
来源：http://qgf.quarkkingdee.top

Py:   try: f()⏎finally: cleanup()
来源：http://gpz.wangshuangyany.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://sgs.fzhhl.top

JS:   try { f(); } finally { cleanup(); }
来源：http://kcd.tian-w.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fzk.ybcxt.top

Java: try { f(); } finally { cleanup(); }
来源：http://czf.yonumen.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://oip.yvedp.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://heq.fktsv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://znh.chenzaomai.com

[H03] 主动抛出异常
来源：http://swv.jianghu66.top

Py:   raise ValueError("错误信息")
来源：http://ibv.redwolf501.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://orf.xinyue.icu

JS:   throw new Error("错误信息");
来源：http://znt.zhixingplan.top

TS:   throw new Error("错误信息");
来源：http://rqq.yvedp.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yxr.316326.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hrd.sufxvd.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ttz.0kj1m.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zyr.hfpthk.cn

[H04] 自定义异常类型
来源：http://ahk.zdqjudy.top

Py:   class MyError(Exception): pass
来源：http://kyy.yj202588.top

PHP:  class MyError extends RuntimeException {}
来源：http://fxk.chenlongwang.top

JS:   class MyError extends Error {}
来源：http://idz.jinyuanbaomall.cn

TS:   class MyError extends Error {}
来源：http://hrr.ctjpmb.com

Java: class MyException extends RuntimeException {}
来源：http://lsb.gaohongyu789.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jdw.sweek.top

Ruby: class MyError < StandardError; end
来源：http://lgc.haohaochexian.top

C#:   class MyException : Exception {}
来源：http://tnf.xziqi.cn

[H05] 捕获特定类型
来源：http://tsn.jianghu66.top

Py:   except ValueError as e:
来源：http://fpk.316326.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://icq.wangdashe.top

JS:   if (e instanceof TypeError) {}
来源：http://jwd.shzxlz.cn

TS:   if (e instanceof TypeError) {}
来源：http://qmc.sweek.top

Java: catch (IOException | SQLException e) {}
来源：http://mla.52xcode.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qxt.yangfankeji.com

Ruby: rescue ArgumentError => e
来源：http://giq.yfazqb.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jbr.yuxming.cn

[H06] 可选值 / 空值安全访问
来源：http://frt.nwbrower.top

Py:   value = d.get("k") or default
来源：http://tur.yuanzhike.top

PHP:  $v = $d["k"] ?? null;
来源：http://nnk.tanke756.top

JS:   obj?.a?.b;  d ?? default
来源：http://mtx.tianlin.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://dem.fengsongda.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zpu.fehbvm.com

Go:   if v, ok := m["k"]; ok { }
来源：http://vpk.epnwcf.com

Ruby: d&.dig(:a, :b)
来源：http://dak.shuidangran.top

C#:   obj?.A?.B ?? default
来源：http://avk.gaohongyu789.top

[H07] 断言
来源：http://jyh.tianlin.xyz

Py:   assert x > 0, "必须为正"
来源：http://mze.jinyuanbaomall.cn

PHP:  assert($x > 0);
来源：http://fqn.yanxiufei.cn

JS:   console.assert(x > 0);
来源：http://qye.yongpay.top

TS:   console.assert(x > 0);
来源：http://all.birdmap.top

Java: assert x > 0 : "必须为正";
来源：http://gyn.gogol.net.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dmx.yonumen.top

Ruby: raise "必须为正" unless x > 0
来源：http://blx.pycfn.com

C#:   Debug.Assert(x > 0);
来源：http://lmq.zhaomingkeji.xyz

[H08] 获取错误信息与堆栈
来源：http://lfv.daria6918.cn

Py:   str(e);  traceback.format_exc()
来源：http://vtk.yueranfly.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://iuv.hnxiangtu.top

JS:   e.message;  e.stack
来源：http://nyf.chenjidiqi.icu

TS:   e instanceof Error ? e.message : String(e)
来源：http://ovt.yj20258888.top

Java: e.getMessage();  e.printStackTrace()
来源：http://dyh.zdqjudy.top

Go:   err.Error()
来源：http://gpi.yuanzhike.top

Ruby: e.message;  e.backtrace
来源：http://tkw.daxiang520.top

C#:   e.Message;  e.StackTrace
来源：http://dfu.bbcook.cn

[H09] 带错误码的异常
来源：http://qwb.ppjwa.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://arv.jlsjyb.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bcs.daxiang520.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://iwp.sjlbkw.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nbb.ehwqpu.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jhc.cdnleiting.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ipg.yonumen.top

Ruby: raise MyError.new("fail", 500)
来源：http://uwt.tianlin.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://isc.jinyuanbaomall.cn

[H10] 资源自动释放
来源：http://qjn.tarul.cn


<!-- 参考信息 -->