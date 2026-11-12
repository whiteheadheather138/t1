代发 wailian999

Ruby: File.delete("a.txt")
来源：http://tvv.gotoacloud.top

C#:   File.Delete("a.txt");
来源：http://pua.guowangkeji.top

[F07] 创建目录（含多级）
来源：http://kui.hywenlv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ywz.sweek.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://reg.uphjek.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fbx.hcnkem.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tpy.ybcxt.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://von.sxryk.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mri.jinqigufen.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nkv.ybcxt.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://olq.zhoulong.xyz

[F08] 遍历目录
来源：http://mgw.sweek.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://rky.cucudq.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wol.pycfn.com

JS:   fs.readdirSync("dir")
来源：http://luq.yuxming.cn

TS:   fs.readdirSync("dir")
来源：http://erv.xingfuxueyuan.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://btf.ivvv.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://jzt.shuidangran.top

Ruby: Dir.children("dir")
来源：http://vbt.zhongyouzk.top

C#:   Directory.GetFiles("dir")
来源：http://rdy.guannengcc.top

[F09] 获取文件大小
来源：http://mrc.dianchejie.cn

Py:   os.path.getsize("a.txt")
来源：http://sno.tianlin.xyz

PHP:  filesize("a.txt");
来源：http://nrr.cashguo.top

JS:   fs.statSync("a.txt").size
来源：http://uvq.sufxvd.cn

TS:   fs.statSync("a.txt").size
来源：http://ncg.jinqigfzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://umx.hfpthk.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://aqa.chenjidiqi.icu

Ruby: File.size("a.txt")
来源：http://pcf.shanyushiyangkeji.top

C#:   new FileInfo("a.txt").Length
来源：http://pmz.jinghuilouyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://dvx.xinyue.icu

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jmr.chenjidiqi.icu

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wgz.shangyingyoupin.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rgo.fehbvm.com

TS:   path.extname("a.txt")
来源：http://eiy.yvedp.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qki.316326.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vrh.zhijiandao.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tlr.aibaodan.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bti.yj20258.top

[F11] 复制与移动文件
来源：http://djq.zhongyouzk.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rgs.meibo888.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pde.ivvv.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://trd.sjlbkw.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gfu.andypj.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yea.yangfankeji.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cxu.yangfankeji.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tmm.ydjk.org.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ybw.havefunace.top

[F12] CSV 读写
来源：http://hzx.gzhubu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://anq.guannengcc.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wqb.cheryme.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://faa.zhaomingkeji.xyz

TS:   // 同上
来源：http://dxp.hywenlv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fgm.0kj1m.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bkq.bbcook.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yef.ehwqpu.com

C#:   // 无内置：用 CsvHelper 库
来源：http://trm.yfazqb.com

================================================================================
来源：http://xlf.xuetiantiany.cn

G. 面向对象
来源：http://lnm.tian-w.cn

================================================================================
来源：http://zem.birdmap.top

[G01] 定义类
来源：http://fkb.svipenyu.cn

Py:   class User: pass
来源：http://aos.cdnleiting.top

PHP:  class User {}
来源：http://syg.yueranfly.top

JS:   class User {}
来源：http://wrm.cheryme.top

TS:   class User { name: string = ""; }
来源：http://fyo.cdnleiting.top

Java: class User {}
来源：http://tzf.yanxiufei.cn

Go:   type User struct { Name string }
来源：http://llh.meibo888.top

Ruby: class User; end
来源：http://uzp.tianlin.xyz

C#:   class User {}
来源：http://xrc.ivvv.top

[G02] 构造函数
来源：http://xmy.hywenlv.cn

Py:   def __init__(self, name): self.name = name
来源：http://nxg.ehwqpu.com

PHP:  public function __construct(public string $name) {}
来源：http://apm.havefunace.top

JS:   constructor(name) { this.name = name; }
来源：http://tko.hesvh.cn

TS:   constructor(public name: string) {}
来源：http://rrk.uphjek.com

Java: User(String name) { this.name = name; }
来源：http://lhh.nanxuanxn.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ajt.yangfankeji.com

Ruby: def initialize(name); @name = name; end
来源：http://ljc.zhixingplan.top

C#:   public User(string name) { Name = name; }
来源：http://dav.chenzaomai.com

[G03] 实例属性
来源：http://kwx.epnwcf.com

Py:   self.name = "x"
来源：http://vqz.hcnkem.com

PHP:  public string $name = "x";
来源：http://pug.jiagoushi.top

JS:   this.name = "x";
来源：http://wvh.shuidangran.top

TS:   name: string = "x";
来源：http://spa.birdmap.top

Java: private String name;
来源：http://nau.zhixingplan.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gop.jiagoushi.top

Ruby: @name = "x"
来源：http://fos.dashuyun.cn

C#:   public string Name { get; set; } = "x";
来源：http://uxv.ywan-chungtsiang.top

[G04] 定义方法
来源：http://dgd.yuxming.cn

Py:   def greet(self): return self.name
来源：http://txn.chenjidiqi.icu

PHP:  public function greet(): string { return $this->name; }
来源：http://dic.mhx1999.top

JS:   greet() { return this.name; }
来源：http://ehh.hcnkem.com

TS:   greet(): string { return this.name; }
来源：http://nun.sweek.top

Java: String greet() { return name; }
来源：http://kho.havefunace.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://hnv.ivvv.top

Ruby: def greet; @name; end
来源：http://qca.shanyushiyangkeji.top

C#:   public string Greet() => Name;
来源：http://pgu.smart0.xyz

[G05] 继承
来源：http://yri.ydzc1.top

Py:   class Admin(User): pass
来源：http://zji.hfpthk.cn

PHP:  class Admin extends User {}
来源：http://zfg.yj20258888.top

JS:   class Admin extends User {}
来源：http://zew.52xcode.cn

TS:   class Admin extends User {}
来源：http://jei.hnqzz.top

Java: class Admin extends User {}
来源：http://oof.gzhubu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pit.wangshuangyany.cn

Ruby: class Admin < User; end
来源：http://lgd.xuetiantiany.cn

C#:   class Admin : User {}
来源：http://dwa.cucudq.cn

[G06] 重写方法
来源：http://att.svipenyu.cn

Py:   def greet(self): return "admin"
来源：http://djk.ydzc1.top

PHP:  public function greet(): string { return "admin"; }
来源：http://bhx.gogol.net.cn

JS:   greet() { return "admin"; }
来源：http://dmr.hammf.cn

TS:   greet(): string { return "admin"; }
来源：http://rdq.yfazqb.com

Java: @Override String greet() { return "admin"; }
来源：http://imt.zhengqikj.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://giq.yj20258888.top

Ruby: def greet; "admin"; end
来源：http://ejp.shanyushiyangkeji.top

C#:   public override string Greet() => "admin";
来源：http://qat.zhengqikj.top

[G07] 调用父类方法
来源：http://zwu.hywenlv.cn

Py:   super().greet()
来源：http://qzk.aizwys.cn

PHP:  parent::greet();
来源：http://qoa.hongshengwenyu.top

JS:   super.greet();
来源：http://aca.hysaishi.cn

TS:   super.greet();
来源：http://rys.chenzaomai.com

Java: super.greet();
来源：http://gxu.bbcook.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pbr.nwbrower.top

Ruby: super
来源：http://aoj.pycfn.com

C#:   base.Greet();
来源：http://kpw.gzhubu.top

[G08] 静态方法与属性
来源：http://xkz.jyoumei.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ymf.vehdjk.com

PHP:  public static function f() {}
来源：http://rlj.zdqjudy.top

JS:   static f() {}
来源：http://jwx.dianchejie.cn

TS:   static f(): void {}
来源：http://bct.ppjwa.cn

Java: static void f() {}
来源：http://ccs.c1oappe.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://jae.zycfv.cn

Ruby: def self.f; end
来源：http://dsk.cucudq.cn

C#:   public static void F() {}
来源：http://kzc.fzhhl.top

[G09] 接口 / 抽象类
来源：http://fpw.vehdjk.com

Py:   from abc import ABC, abstractmethod
来源：http://sdq.chenjidiqi.icu

PHP:  interface Shape { public function area(): float; }
来源：http://tgy.jqgufenzy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://tiy.ehwqpu.com

TS:   interface Shape { area(): number; }
来源：http://fqg.hnxiangtu.top

Java: interface Shape { double area(); }
来源：http://sot.snrcjt.cn

Go:   type Shape interface { Area() float64 }
来源：http://vab.cdnleiting.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ocd.yueranfly.top

C#:   interface IShape { double Area(); }
来源：http://fkv.ywan-chungtsiang.top

[G10] 访问控制
来源：http://ccu.epnwcf.com

Py:   约定 _protected / __private（不强制）
来源：http://vke.andypj.xyz

PHP:  public / protected / private
来源：http://ynq.ehwqpu.com

JS:   #private 字段；其余公开
来源：http://sen.0kj1m.cn

TS:   public / protected / private
来源：http://fee.zhijiandao.cn

Java: public / protected / private / 默认包级
来源：http://zbi.cqqwz.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://afo.jyoumei.cn

Ruby: public / protected / private
来源：http://vgz.jqgfzy.top

C#:   public / protected / private / internal
来源：http://xcb.hesvh.cn

[G11] getter / setter
来源：http://eac.yangfankeji.com

Py:   @property 与 @x.setter
来源：http://bfd.guowangkeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jpc.cucudq.cn

JS:   get name() { return this._name; }
来源：http://tve.yfazqb.com

TS:   get name(): string { return this._name; }
来源：http://eyf.haohaochexian.top

Java: public String getName() { return name; }
来源：http://gfp.yj20258.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://hiw.jiagoushi.top

Ruby: attr_accessor :name
来源：http://ocm.yvedp.cn

C#:   public string Name { get; set; }
来源：http://ldh.snrcjt.cn

[G12] 对象转字符串
来源：http://ixe.chenlongwang.top

Py:   def __str__(self): return self.name
来源：http://say.ehwqpu.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://ibd.vehdjk.com

JS:   toString() { return this.name; }
来源：http://tdf.jyoumei.cn

TS:   toString(): string { return this.name; }
来源：http://ocy.c1oappe.top

Java: @Override public String toString() { return name; }
来源：http://vlx.epnwcf.com

Go:   func (u User) String() string { return u.Name }
来源：http://hxy.mhx1999.top

Ruby: def to_s; @name; end
来源：http://knx.gaohongyu789.top

C#:   public override string ToString() => Name;
来源：http://orw.cqqwz.cn

[G13] 判断对象类型
来源：http://uwk.pycfn.com

Py:   isinstance(u, User)
来源：http://hkj.fanxiaobao.xyz

PHP:  $u instanceof User
来源：http://erv.wangdashe.top

JS:   u instanceof User
来源：http://weo.tianlin.xyz

TS:   u instanceof User
来源：http://wzi.ybcxt.top

Java: u instanceof User
来源：http://wms.yanxiufei.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ogo.zhongyouzk.top

Ruby: u.is_a?(User)
来源：http://nta.hammf.cn

C#:   u is User
来源：http://iox.ywan-chungtsiang.top

[G14] 数据类 / record
来源：http://zvj.epnwcf.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qoq.fanxiaobao.xyz

PHP:  // 用 readonly 属性模拟
来源：http://gee.aibaodan.cn

JS:   // 无内置：普通类或对象字面量
来源：http://pmd.yj20258.top

TS:   type User = { name: string; age: number };
来源：http://vyn.c1oappe.top

Java: record User(String name, int age) {}
来源：http://vis.52xcode.cn

Go:   type User struct { Name string; Age int }
来源：http://lcb.redwolf501.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uwl.ppjwa.cn

C#:   record User(string Name, int Age);
来源：http://tfb.sysykeji.top

[G15] 枚举
来源：http://fcu.shanyushiyangtech.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qit.feifeiyinyue.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://boh.shangyingyoupin.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jke.vqdsnc.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dli.chenlongwang.top

Java: enum Color { RED, GREEN }
来源：http://vkm.c1oappe.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://acy.dashuyun.cn

Ruby: Color = %i[red green].freeze
来源：http://rwt.9152youxi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zss.gogol.net.cn

[G16] 对象转数组 / 字典
来源：http://vpb.shzxlz.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wpx.yvedp.cn

PHP:  get_object_vars($obj);
来源：http://xbb.c1oappe.top

JS:   Object.entries(obj)
来源：http://lrz.hnxiangtu.top

TS:   Object.entries(obj)
来源：http://pem.xuetiantiany.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kng.redwolf501.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://fjl.zycfv.cn

Ruby: obj.instance_variables
来源：http://htn.hcnkem.com

C#:   // 用反射或 System.Text.Json
来源：http://yfb.daria6918.cn

================================================================================
来源：http://cqz.jinqigfzy.top

H. 异常与错误处理
来源：http://tjc.jinyuanbaomall.cn

================================================================================
来源：http://myf.xuetiantiany.cn

[H01] try / catch 基础
来源：http://vpe.yonumen.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sws.xuanzx.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yoe.ybcxt.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nia.vehdjk.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://npg.dashuyun.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://czt.sjlbkw.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mal.havefunace.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mvy.ywan-chungtsiang.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://foi.xuetiantiany.cn

[H02] finally / ensure 收尾
来源：http://jex.fzhhl.top

Py:   try: f()⏎finally: cleanup()
来源：http://pnj.bjfxy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://njd.yj20258888.top

JS:   try { f(); } finally { cleanup(); }
来源：http://qms.zhongyouzk.top

TS:   try { f(); } finally { cleanup(); }
来源：http://fqd.52xcode.cn

Java: try { f(); } finally { cleanup(); }
来源：http://prf.gaohongyu789.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://wtf.ybcxt.top

Ruby: begin; f; ensure; cleanup; end
来源：http://nmf.iojbl.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zqu.gogol.net.cn

[H03] 主动抛出异常
来源：http://vhn.sjlbkw.cn

Py:   raise ValueError("错误信息")
来源：http://mhq.yvedp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tnl.yvedp.cn

JS:   throw new Error("错误信息");
来源：http://lmt.jqgufenzy.top

TS:   throw new Error("错误信息");
来源：http://xue.nanxuanxn.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://obz.bjfxy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nut.shzxlz.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://jlu.hnqzz.top

C#:   throw new ArgumentException("错误信息");
来源：http://boy.xingfuxueyuan.xyz

[H04] 自定义异常类型
来源：http://bcv.haohaochexian.top

Py:   class MyError(Exception): pass
来源：http://vul.jinghuilouyu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pmv.shuidangran.top

JS:   class MyError extends Error {}
来源：http://ztt.52xcode.cn

TS:   class MyError extends Error {}
来源：http://xkw.jinyuanbaomall.cn

Java: class MyException extends RuntimeException {}
来源：http://ojc.shanyushiyangkeji.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wiw.tian-w.cn

Ruby: class MyError < StandardError; end
来源：http://vdb.feifeiyinyue.top

C#:   class MyException : Exception {}
来源：http://ozx.zhiwuduotai.top

[H05] 捕获特定类型
来源：http://nyn.chenlongwang.top

Py:   except ValueError as e:
来源：http://fwf.gzhubu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uvj.dashuyun.cn

JS:   if (e instanceof TypeError) {}
来源：http://cvb.wangdashe.top

TS:   if (e instanceof TypeError) {}
来源：http://wls.yangfankeji.com

Java: catch (IOException | SQLException e) {}
来源：http://vyx.hysaishi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://eno.vqdsnc.cn

Ruby: rescue ArgumentError => e
来源：http://lec.yongpay.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lmk.daria6918.cn

[H06] 可选值 / 空值安全访问
来源：http://wsd.dianchejie.cn

Py:   value = d.get("k") or default
来源：http://tax.dianchejie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://hhj.jinghuilouyu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jjb.hesvh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mvu.daria6918.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://djb.fanxiaobao.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://xvb.316326.xyz

Ruby: d&.dig(:a, :b)
来源：http://bzj.ywan-chungtsiang.top

C#:   obj?.A?.B ?? default
来源：http://qvn.sweek.top

[H07] 断言
来源：http://uyj.sysykeji.top

Py:   assert x > 0, "必须为正"
来源：http://kmm.gzhubu.top

PHP:  assert($x > 0);
来源：http://zwz.guannengcc.top

JS:   console.assert(x > 0);
来源：http://lcq.jqgfzy.top

TS:   console.assert(x > 0);
来源：http://pbe.uphjek.com

Java: assert x > 0 : "必须为正";
来源：http://gpa.daria6918.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://che.hcnkem.com

Ruby: raise "必须为正" unless x > 0
来源：http://bhx.yongpay.top

C#:   Debug.Assert(x > 0);
来源：http://abi.uphjek.com

[H08] 获取错误信息与堆栈
来源：http://mxc.sjlbkw.cn

Py:   str(e);  traceback.format_exc()
来源：http://ync.wangdashe.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://chz.andypj.xyz

JS:   e.message;  e.stack
来源：http://yiz.ydzc1.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://tow.tanke756.top

Java: e.getMessage();  e.printStackTrace()
来源：http://rlu.fehbvm.com

Go:   err.Error()
来源：http://gwl.havefunace.top

Ruby: e.message;  e.backtrace
来源：http://huo.uphjek.com

C#:   e.Message;  e.StackTrace
来源：http://fvv.hongshengwenyu.top

[H09] 带错误码的异常
来源：http://ovm.zhaomingkeji.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sbx.yangfankeji.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://bzp.guowangkeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wdp.jqgfzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ocr.xylfe.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vxo.jlsjyb.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lwe.aizwys.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mbj.cucudq.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://svd.yvedp.cn

[H10] 资源自动释放
来源：http://jif.chenzaomai.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://uba.fengsongda.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vqh.9152youxi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dwl.meibo888.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kev.hfpthk.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ddk.guowangkeji.top

Go:   defer f.Close()
来源：http://lxj.yuxming.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tdr.cqqwz.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gpx.ybcxt.top

================================================================================
来源：http://gmo.xingfuxueyuan.xyz

I. 正则表达式
来源：http://jej.jiagoushi.top

================================================================================
来源：http://ewp.havefunace.top

[I01] 判断是否匹配
来源：http://yia.shzxlz.cn


<!-- 参考信息 -->