代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://vkn.guannengcc.top

TS:   fs.unlinkSync("a.txt")
来源：http://nyo.tian-w.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qhk.vehdjk.com

Go:   os.Remove("a.txt")
来源：http://bvw.fanxiaobao.xyz

Ruby: File.delete("a.txt")
来源：http://ggv.smart0.xyz

C#:   File.Delete("a.txt");
来源：http://fzr.0kj1m.cn

[F07] 创建目录（含多级）
来源：http://uqx.yongpay.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pjl.0kj1m.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ngn.jqgfzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mir.xziqi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hrq.bbcook.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ibv.zdbjq.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pig.yongpay.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cyj.yonumen.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rle.yvedp.cn

[F08] 遍历目录
来源：http://icz.andypj.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://wfp.jyoumei.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dsk.gogol.net.cn

JS:   fs.readdirSync("dir")
来源：http://qcp.ehwqpu.com

TS:   fs.readdirSync("dir")
来源：http://ezp.zhoulong.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nhl.ydzc1.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://rvf.pengpengdd.cyou

Ruby: Dir.children("dir")
来源：http://saw.yj20258888.top

C#:   Directory.GetFiles("dir")
来源：http://zzc.havefunace.top

[F09] 获取文件大小
来源：http://xzp.fanxiaobao.xyz

Py:   os.path.getsize("a.txt")
来源：http://gim.jiagoushi.top

PHP:  filesize("a.txt");
来源：http://ptm.ydzc1.top

JS:   fs.statSync("a.txt").size
来源：http://lsm.c1oappe.top

TS:   fs.statSync("a.txt").size
来源：http://xlt.haohaochexian.top

Java: Files.size(Path.of("a.txt"))
来源：http://wyn.gogol.net.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lkf.c1oappe.top

Ruby: File.size("a.txt")
来源：http://wig.xingfuxueyuan.xyz

C#:   new FileInfo("a.txt").Length
来源：http://mzk.fanxiaobao.xyz

[F10] 取文件扩展名 / 文件名
来源：http://awb.gaohongyu789.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qot.ybcxt.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vcz.meibo888.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sqp.chenjidiqi.icu

TS:   path.extname("a.txt")
来源：http://qrb.zhengqikj.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zap.aibaodan.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mlc.tianlin.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://utt.fengsongda.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vem.chenzaomai.com

[F11] 复制与移动文件
来源：http://iix.hammf.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dim.tian-w.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lng.cheryme.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ueg.shzxlz.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fia.dashuyun.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ccm.dianchejie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ane.dianchejie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gel.guowangkeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zyt.yueranfly.top

[F12] CSV 读写
来源：http://ajr.shanyushiyangtech.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kwt.nanxinkj.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pkj.shanyushiyangtech.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dug.smart0.xyz

TS:   // 同上
来源：http://oug.daria6918.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cvd.zhongyouzk.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xvx.ybcxt.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dwo.zdbjq.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://yje.fzhhl.top

================================================================================
来源：http://rjj.52xcode.cn

G. 面向对象
来源：http://vef.nanxuanxn.top

================================================================================
来源：http://bvx.jianghu66.top

[G01] 定义类
来源：http://tgm.yj20258.top

Py:   class User: pass
来源：http://ctl.gaohongyu789.top

PHP:  class User {}
来源：http://pzk.redwolf501.top

JS:   class User {}
来源：http://xst.smart0.xyz

TS:   class User { name: string = ""; }
来源：http://try.shuidangran.top

Java: class User {}
来源：http://zmg.shzxlz.cn

Go:   type User struct { Name string }
来源：http://yyo.meibo888.top

Ruby: class User; end
来源：http://wnl.dianchejie.cn

C#:   class User {}
来源：http://rlr.0kj1m.cn

[G02] 构造函数
来源：http://jqr.jqgfzy.top

Py:   def __init__(self, name): self.name = name
来源：http://ael.jlsjyb.cn

PHP:  public function __construct(public string $name) {}
来源：http://oer.hammf.cn

JS:   constructor(name) { this.name = name; }
来源：http://jbd.c1oappe.top

TS:   constructor(public name: string) {}
来源：http://vsa.birdmap.top

Java: User(String name) { this.name = name; }
来源：http://fnr.cucudq.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fpq.xylfe.cn

Ruby: def initialize(name); @name = name; end
来源：http://vpc.zhijiandao.cn

C#:   public User(string name) { Name = name; }
来源：http://jft.zhijiandao.cn

[G03] 实例属性
来源：http://nba.smart0.xyz

Py:   self.name = "x"
来源：http://hbg.yuanzhike.top

PHP:  public string $name = "x";
来源：http://tnd.quarkkingdee.top

JS:   this.name = "x";
来源：http://nkx.fanxiaobao.xyz

TS:   name: string = "x";
来源：http://cbg.zhongyouzk.top

Java: private String name;
来源：http://ooo.0kj1m.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dku.jinghuilouyu.cn

Ruby: @name = "x"
来源：http://kho.sjlbkw.cn

C#:   public string Name { get; set; } = "x";
来源：http://nnm.birdmap.top

[G04] 定义方法
来源：http://fxm.dashuyun.cn

Py:   def greet(self): return self.name
来源：http://mdt.guannengcc.top

PHP:  public function greet(): string { return $this->name; }
来源：http://xbe.yonumen.top

JS:   greet() { return this.name; }
来源：http://uue.vehdjk.com

TS:   greet(): string { return this.name; }
来源：http://rgh.wangdashe.top

Java: String greet() { return name; }
来源：http://coe.jinyuanbaomall.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qyk.mhx1999.top

Ruby: def greet; @name; end
来源：http://ews.jinqigfzy.top

C#:   public string Greet() => Name;
来源：http://sfw.hesvh.cn

[G05] 继承
来源：http://uxj.meibo888.top

Py:   class Admin(User): pass
来源：http://vaq.ivvv.top

PHP:  class Admin extends User {}
来源：http://rkm.ctjpmb.com

JS:   class Admin extends User {}
来源：http://ncl.bbcook.cn

TS:   class Admin extends User {}
来源：http://lgw.guowangkeji.top

Java: class Admin extends User {}
来源：http://swi.tarul.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rcb.tarul.cn

Ruby: class Admin < User; end
来源：http://dzl.xuetiantiany.cn

C#:   class Admin : User {}
来源：http://nbw.ydjk.org.cn

[G06] 重写方法
来源：http://ftt.chenlongwang.top

Py:   def greet(self): return "admin"
来源：http://hnd.yangfankeji.com

PHP:  public function greet(): string { return "admin"; }
来源：http://wfd.gzhubu.top

JS:   greet() { return "admin"; }
来源：http://wsf.316326.xyz

TS:   greet(): string { return "admin"; }
来源：http://mzi.nwbrower.top

Java: @Override String greet() { return "admin"; }
来源：http://syq.zdqjudy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://csu.birdmap.top

Ruby: def greet; "admin"; end
来源：http://ezh.epnwcf.com

C#:   public override string Greet() => "admin";
来源：http://rsp.uphjek.com

[G07] 调用父类方法
来源：http://vrb.shzxlz.cn

Py:   super().greet()
来源：http://wnt.pycfn.com

PHP:  parent::greet();
来源：http://nkb.birdmap.top

JS:   super.greet();
来源：http://bhf.zdqjudy.top

TS:   super.greet();
来源：http://fms.svipenyu.cn

Java: super.greet();
来源：http://qza.nwbrower.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tpl.zhoulong.xyz

Ruby: super
来源：http://tej.9152youxi.cn

C#:   base.Greet();
来源：http://nyj.sufxvd.cn

[G08] 静态方法与属性
来源：http://rdo.zhixingplan.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yjm.fanxiaobao.xyz

PHP:  public static function f() {}
来源：http://qes.sweek.top

JS:   static f() {}
来源：http://vtm.xuanzx.com

TS:   static f(): void {}
来源：http://ovw.nanxuanxn.top

Java: static void f() {}
来源：http://sqk.shzxlz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ybc.zhengqikj.top

Ruby: def self.f; end
来源：http://nyg.yuxming.cn

C#:   public static void F() {}
来源：http://bly.daxiang520.top

[G09] 接口 / 抽象类
来源：http://lxk.hesvh.cn

Py:   from abc import ABC, abstractmethod
来源：http://mlf.gogol.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nrq.jinghuilouyu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vrn.wangdashe.top

TS:   interface Shape { area(): number; }
来源：http://kxp.nwbrower.top

Java: interface Shape { double area(); }
来源：http://kgt.tanke756.top

Go:   type Shape interface { Area() float64 }
来源：http://vhu.yj202588.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rzy.sufxvd.cn

C#:   interface IShape { double Area(); }
来源：http://eut.gogol.net.cn

[G10] 访问控制
来源：http://kjd.tarul.cn

Py:   约定 _protected / __private（不强制）
来源：http://gcc.yj20258888.top

PHP:  public / protected / private
来源：http://inx.jinqigufen.top

JS:   #private 字段；其余公开
来源：http://jwn.birdmap.top

TS:   public / protected / private
来源：http://edx.xuanzx.com

Java: public / protected / private / 默认包级
来源：http://mqp.jinghuilouyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://wzr.redwolf501.top

Ruby: public / protected / private
来源：http://ljz.zdbjq.cn

C#:   public / protected / private / internal
来源：http://vcu.xziqi.cn

[G11] getter / setter
来源：http://zrz.iojbl.cn

Py:   @property 与 @x.setter
来源：http://vua.quarkkingdee.top

PHP:  public function getName(): string { return $this->name; }
来源：http://exk.cashguo.top

JS:   get name() { return this._name; }
来源：http://zpw.daxiang520.top

TS:   get name(): string { return this._name; }
来源：http://pzh.ybcxt.top

Java: public String getName() { return name; }
来源：http://thv.ivvv.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://hft.jianghu66.top

Ruby: attr_accessor :name
来源：http://nkt.hfpthk.cn

C#:   public string Name { get; set; }
来源：http://gbb.vqdsnc.cn

[G12] 对象转字符串
来源：http://alx.fktsv.cn

Py:   def __str__(self): return self.name
来源：http://lpy.hfpthk.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://uvp.cheryme.top

JS:   toString() { return this.name; }
来源：http://knq.yongpay.top

TS:   toString(): string { return this.name; }
来源：http://ggy.ehwqpu.com

Java: @Override public String toString() { return name; }
来源：http://cuf.gaohongyu789.top

Go:   func (u User) String() string { return u.Name }
来源：http://ndg.hongshengwenyu.top

Ruby: def to_s; @name; end
来源：http://sda.sufxvd.cn

C#:   public override string ToString() => Name;
来源：http://acy.cucudq.cn

[G13] 判断对象类型
来源：http://jxq.xuanzx.com

Py:   isinstance(u, User)
来源：http://wxi.xingfuxueyuan.xyz

PHP:  $u instanceof User
来源：http://oex.wangdashe.top

JS:   u instanceof User
来源：http://qdo.bbcook.cn

TS:   u instanceof User
来源：http://xvf.epnwcf.com

Java: u instanceof User
来源：http://cza.hesvh.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pcj.ctjpmb.com

Ruby: u.is_a?(User)
来源：http://ods.ehwqpu.com

C#:   u is User
来源：http://ewn.sufxvd.cn

[G14] 数据类 / record
来源：http://tdj.tian-w.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xjr.shanyushiyangtech.top

PHP:  // 用 readonly 属性模拟
来源：http://oll.yj20258888.top

JS:   // 无内置：普通类或对象字面量
来源：http://pvw.quarkkingdee.top

TS:   type User = { name: string; age: number };
来源：http://bgc.aibaodan.cn

Java: record User(String name, int age) {}
来源：http://zis.zhiwuduotai.top

Go:   type User struct { Name string; Age int }
来源：http://wuc.mhx1999.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://scc.pengpengdd.cyou

C#:   record User(string Name, int Age);
来源：http://rfa.hfpthk.cn

[G15] 枚举
来源：http://zly.jyoumei.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dgp.jqgfzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ztd.xinyue.icu

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pnp.cucudq.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sor.ehwqpu.com

Java: enum Color { RED, GREEN }
来源：http://bxu.bjfxy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ydk.tarul.cn

Ruby: Color = %i[red green].freeze
来源：http://but.shanyushiyangtech.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kjo.sysykeji.top

[G16] 对象转数组 / 字典
来源：http://dwo.gaohongyu789.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dvh.aizwys.cn

PHP:  get_object_vars($obj);
来源：http://ltj.cdnleiting.top

JS:   Object.entries(obj)
来源：http://kgd.snrcjt.cn

TS:   Object.entries(obj)
来源：http://mpg.chenzaomai.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://teo.gaohongyu789.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://scf.shangyingyoupin.top

Ruby: obj.instance_variables
来源：http://mhf.feifeiyinyue.top

C#:   // 用反射或 System.Text.Json
来源：http://brz.kuanghao11.cn

================================================================================
来源：http://lgg.epnwcf.com

H. 异常与错误处理
来源：http://dtq.feifeiyinyue.top

================================================================================
来源：http://zwk.pycfn.com

[H01] try / catch 基础
来源：http://thm.316326.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nws.aizwys.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yup.tian-w.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ofw.birdmap.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://imd.cheryme.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://igl.ppjwa.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://glg.bbcook.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ogg.jinqigfzy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gne.sufxvd.cn

[H02] finally / ensure 收尾
来源：http://umk.yj20258888.top

Py:   try: f()⏎finally: cleanup()
来源：http://rxr.bjfxy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://qhc.gaohongyu789.top

JS:   try { f(); } finally { cleanup(); }
来源：http://lff.nwbrower.top

TS:   try { f(); } finally { cleanup(); }
来源：http://pzy.tanke756.top

Java: try { f(); } finally { cleanup(); }
来源：http://sqs.yonumen.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://blb.gotoacloud.top

Ruby: begin; f; ensure; cleanup; end
来源：http://gvx.shanyushiyangkeji.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://xrz.hcnkem.com

[H03] 主动抛出异常
来源：http://pvo.tarul.cn

Py:   raise ValueError("错误信息")
来源：http://dmv.yonumen.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://neq.hcnkem.com

JS:   throw new Error("错误信息");
来源：http://zea.mhx1999.top

TS:   throw new Error("错误信息");
来源：http://rey.zdqjudy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://flx.jinyuanbaomall.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nfc.fzhhl.top

Ruby: raise ArgumentError, "错误信息"
来源：http://icj.shzxlz.cn

C#:   throw new ArgumentException("错误信息");
来源：http://plc.tianlin.xyz

[H04] 自定义异常类型
来源：http://jnp.wangdashe.top

Py:   class MyError(Exception): pass
来源：http://sdm.daxiang520.top

PHP:  class MyError extends RuntimeException {}
来源：http://sax.guowangkeji.top

JS:   class MyError extends Error {}
来源：http://erw.shzxlz.cn

TS:   class MyError extends Error {}
来源：http://hxj.fzhhl.top

Java: class MyException extends RuntimeException {}
来源：http://jht.9152youxi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uzi.shzxlz.cn

Ruby: class MyError < StandardError; end
来源：http://mwd.aibaodan.cn

C#:   class MyException : Exception {}
来源：http://ntx.nwbrower.top

[H05] 捕获特定类型
来源：http://mwk.jqgufenzy.top

Py:   except ValueError as e:
来源：http://lht.uphjek.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nfl.yonumen.top

JS:   if (e instanceof TypeError) {}
来源：http://uen.jinghuilouyu.cn

TS:   if (e instanceof TypeError) {}
来源：http://ojt.hcnkem.com

Java: catch (IOException | SQLException e) {}
来源：http://lmu.jinghuilouyu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uzk.ehwqpu.com

Ruby: rescue ArgumentError => e
来源：http://nic.cheryme.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ezh.zhengqikj.top

[H06] 可选值 / 空值安全访问
来源：http://dau.nanxuanxn.top

Py:   value = d.get("k") or default
来源：http://byw.xuanzx.com

PHP:  $v = $d["k"] ?? null;
来源：http://eoc.guannengcc.top

JS:   obj?.a?.b;  d ?? default
来源：http://goo.jianghu66.top

TS:   obj?.a?.b;  d ?? default
来源：http://ngu.fehbvm.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://eqh.jiagoushi.top

Go:   if v, ok := m["k"]; ok { }
来源：http://pgt.pengpengdd.cyou

Ruby: d&.dig(:a, :b)
来源：http://nic.mhx1999.top

C#:   obj?.A?.B ?? default
来源：http://yor.bbcook.cn

[H07] 断言
来源：http://iqh.birdmap.top

Py:   assert x > 0, "必须为正"
来源：http://jmp.redwolf501.top

PHP:  assert($x > 0);
来源：http://wpw.chenzaomai.com

JS:   console.assert(x > 0);
来源：http://zpz.daxiang520.top

TS:   console.assert(x > 0);
来源：http://hkc.jqgfzy.top

Java: assert x > 0 : "必须为正";
来源：http://nwx.cashguo.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jii.guannengcc.top

Ruby: raise "必须为正" unless x > 0
来源：http://onk.chenzaomai.com

C#:   Debug.Assert(x > 0);
来源：http://ppc.dianchejie.cn

[H08] 获取错误信息与堆栈
来源：http://kmu.snrcjt.cn

Py:   str(e);  traceback.format_exc()
来源：http://yzg.ehwqpu.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sea.vqdsnc.cn

JS:   e.message;  e.stack
来源：http://rcx.52xcode.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mkx.ehwqpu.com

Java: e.getMessage();  e.printStackTrace()
来源：http://pif.sjlbkw.cn

Go:   err.Error()
来源：http://kgc.hnqzz.top

Ruby: e.message;  e.backtrace
来源：http://yeq.kuanghao11.cn

C#:   e.Message;  e.StackTrace
来源：http://teq.zdbjq.cn

[H09] 带错误码的异常
来源：http://ngw.jianghu66.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zce.yanxiufei.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ghw.xinyue.icu

JS:   const err = new Error("fail");  err.code = 500;
来源：http://htc.aizwys.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xge.ctjpmb.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wha.yj20258.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cmh.hammf.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vjl.vehdjk.com

C#:   // 自定义异常类中加 Code 属性
来源：http://sey.nanxuanxn.top

[H10] 资源自动释放
来源：http://fln.snrcjt.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://cru.shuidangran.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cmb.meibo888.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://meo.gaohongyu789.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mna.guowangkeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zbi.zhengqikj.top

Go:   defer f.Close()
来源：http://sor.gaohongyu789.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://svd.nanxuanxn.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qeo.chenjidiqi.icu


<!-- 参考信息 -->