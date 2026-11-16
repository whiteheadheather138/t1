代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://qqr.316326.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://can.sjlbkw.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://puw.fehbvm.com

Go:   os.Remove("a.txt")
来源：http://ebg.chenzaomai.com

Ruby: File.delete("a.txt")
来源：http://kwz.bbcook.cn

C#:   File.Delete("a.txt");
来源：http://nwn.hysaishi.cn

[F07] 创建目录（含多级）
来源：http://rbs.yuanzhike.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zxf.yfazqb.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://neh.yanxiufei.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zbu.fktsv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ksf.zycfv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lhc.sufxvd.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fpi.hammf.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ebn.zycfv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yph.zycfv.cn

[F08] 遍历目录
来源：http://qrh.tarul.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wtb.aibaodan.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://eab.yuanzhike.top

JS:   fs.readdirSync("dir")
来源：http://ywt.redwolf501.top

TS:   fs.readdirSync("dir")
来源：http://jwj.ywan-chungtsiang.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vox.chenzaomai.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://loy.redwolf501.top

Ruby: Dir.children("dir")
来源：http://hwv.snrcjt.cn

C#:   Directory.GetFiles("dir")
来源：http://gqn.shzxlz.cn

[F09] 获取文件大小
来源：http://qof.sjlbkw.cn

Py:   os.path.getsize("a.txt")
来源：http://dbg.yonumen.top

PHP:  filesize("a.txt");
来源：http://iev.zhengqikj.top

JS:   fs.statSync("a.txt").size
来源：http://ppa.nanxinkj.top

TS:   fs.statSync("a.txt").size
来源：http://yqz.xingfuxueyuan.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://eua.c1oappe.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ltp.jinghuilouyu.cn

Ruby: File.size("a.txt")
来源：http://gfk.chenzaomai.com

C#:   new FileInfo("a.txt").Length
来源：http://wfb.jinqigufen.top

[F10] 取文件扩展名 / 文件名
来源：http://stn.jinqigufen.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ukx.chenzaomai.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gdv.xylfe.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ryy.gaohongyu789.top

TS:   path.extname("a.txt")
来源：http://ieb.yvedp.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pan.yj202588.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://aat.iojbl.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yei.jyoumei.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fej.jinyuanbaomall.cn

[F11] 复制与移动文件
来源：http://edl.cheryme.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uzz.ctjpmb.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zjy.svipenyu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://frf.gaohongyu789.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xdz.tarul.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://shx.gogol.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vwd.hywenlv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://djc.pycfn.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yrl.jiagoushi.top

[F12] CSV 读写
来源：http://jxd.hammf.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rpg.tanke756.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bzn.zhiwuduotai.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ieb.jlsjyb.cn

TS:   // 同上
来源：http://hzq.aibaodan.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ipp.daxiang520.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://idy.chenlongwang.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xtn.cucudq.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bym.sysykeji.top

================================================================================
来源：http://lqj.cqqwz.cn

G. 面向对象
来源：http://lwn.zhengqikj.top

================================================================================
来源：http://pny.zhengqikj.top

[G01] 定义类
来源：http://ijp.gogol.net.cn

Py:   class User: pass
来源：http://lko.hcnkem.com

PHP:  class User {}
来源：http://etr.yj202588.top

JS:   class User {}
来源：http://fhb.zhijiandao.cn

TS:   class User { name: string = ""; }
来源：http://iab.jinqigufen.top

Java: class User {}
来源：http://isn.jinqigfzy.top

Go:   type User struct { Name string }
来源：http://qgw.jlsjyb.cn

Ruby: class User; end
来源：http://ots.jqgfzy.top

C#:   class User {}
来源：http://dvk.316326.xyz

[G02] 构造函数
来源：http://mir.ehwqpu.com

Py:   def __init__(self, name): self.name = name
来源：http://zse.ydjk.org.cn

PHP:  public function __construct(public string $name) {}
来源：http://mzo.sweek.top

JS:   constructor(name) { this.name = name; }
来源：http://ofv.cheryme.top

TS:   constructor(public name: string) {}
来源：http://asl.iojbl.cn

Java: User(String name) { this.name = name; }
来源：http://zcz.birdmap.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fke.xuetiantiany.cn

Ruby: def initialize(name); @name = name; end
来源：http://ioh.jqgfzy.top

C#:   public User(string name) { Name = name; }
来源：http://yyw.aibaodan.cn

[G03] 实例属性
来源：http://fit.jqgufenzy.top

Py:   self.name = "x"
来源：http://umb.hnqzz.top

PHP:  public string $name = "x";
来源：http://uic.xziqi.cn

JS:   this.name = "x";
来源：http://hqd.yvedp.cn

TS:   name: string = "x";
来源：http://suc.mhx1999.top

Java: private String name;
来源：http://uil.yuanzhike.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ibk.hammf.cn

Ruby: @name = "x"
来源：http://ram.ehwqpu.com

C#:   public string Name { get; set; } = "x";
来源：http://erk.zhixingplan.top

[G04] 定义方法
来源：http://eyd.fengsongda.top

Py:   def greet(self): return self.name
来源：http://tnr.yonumen.top

PHP:  public function greet(): string { return $this->name; }
来源：http://xvw.mhx1999.top

JS:   greet() { return this.name; }
来源：http://ewt.xinyue.icu

TS:   greet(): string { return this.name; }
来源：http://hvs.jinyuanbaomall.cn

Java: String greet() { return name; }
来源：http://ubt.fehbvm.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://oqy.iojbl.cn

Ruby: def greet; @name; end
来源：http://tqs.ehwqpu.com

C#:   public string Greet() => Name;
来源：http://lnc.tianlin.xyz

[G05] 继承
来源：http://aca.feifeiyinyue.top

Py:   class Admin(User): pass
来源：http://ycp.hesvh.cn

PHP:  class Admin extends User {}
来源：http://smq.dashuyun.cn

JS:   class Admin extends User {}
来源：http://gnw.vehdjk.com

TS:   class Admin extends User {}
来源：http://wqm.zhijiandao.cn

Java: class Admin extends User {}
来源：http://vfn.quarkkingdee.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mak.feifeiyinyue.top

Ruby: class Admin < User; end
来源：http://buz.vehdjk.com

C#:   class Admin : User {}
来源：http://cms.mhx1999.top

[G06] 重写方法
来源：http://idg.hfpthk.cn

Py:   def greet(self): return "admin"
来源：http://ewu.uphjek.com

PHP:  public function greet(): string { return "admin"; }
来源：http://lcg.xinyue.icu

JS:   greet() { return "admin"; }
来源：http://ast.nanxuanxn.top

TS:   greet(): string { return "admin"; }
来源：http://mpe.cdnleiting.top

Java: @Override String greet() { return "admin"; }
来源：http://ujl.zhijiandao.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sif.redwolf501.top

Ruby: def greet; "admin"; end
来源：http://lgg.hywenlv.cn

C#:   public override string Greet() => "admin";
来源：http://fsm.gzhubu.top

[G07] 调用父类方法
来源：http://tsb.pycfn.com

Py:   super().greet()
来源：http://ztr.ybcxt.top

PHP:  parent::greet();
来源：http://ewr.tianlin.xyz

JS:   super.greet();
来源：http://vsp.zhixingplan.top

TS:   super.greet();
来源：http://vdg.sjlbkw.cn

Java: super.greet();
来源：http://maz.aibaodan.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lkf.ivvv.top

Ruby: super
来源：http://bgo.zhiwuduotai.top

C#:   base.Greet();
来源：http://aqx.gogol.net.cn

[G08] 静态方法与属性
来源：http://vod.hfpthk.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://esh.c1oappe.top

PHP:  public static function f() {}
来源：http://hnj.shanyushiyangkeji.top

JS:   static f() {}
来源：http://unn.redwolf501.top

TS:   static f(): void {}
来源：http://lrz.hywenlv.cn

Java: static void f() {}
来源：http://vni.xziqi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://teg.wangshuangyany.cn

Ruby: def self.f; end
来源：http://ytu.yj20258888.top

C#:   public static void F() {}
来源：http://gyg.hammf.cn

[G09] 接口 / 抽象类
来源：http://hwt.xylfe.cn

Py:   from abc import ABC, abstractmethod
来源：http://xqa.cqqwz.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mhk.yj20258.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://hvj.shanyushiyangtech.top

TS:   interface Shape { area(): number; }
来源：http://kvn.tanke756.top

Java: interface Shape { double area(); }
来源：http://dri.gzhubu.top

Go:   type Shape interface { Area() float64 }
来源：http://fto.sxryk.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://iss.svipenyu.cn

C#:   interface IShape { double Area(); }
来源：http://bwg.cheryme.top

[G10] 访问控制
来源：http://aqn.wangdashe.top

Py:   约定 _protected / __private（不强制）
来源：http://nka.daria6918.cn

PHP:  public / protected / private
来源：http://uvy.jlsjyb.cn

JS:   #private 字段；其余公开
来源：http://fuy.zhijiandao.cn

TS:   public / protected / private
来源：http://pcs.jinghuilouyu.cn

Java: public / protected / private / 默认包级
来源：http://nad.ybcxt.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://sil.jinghuilouyu.cn

Ruby: public / protected / private
来源：http://lvm.zhongyouzk.top

C#:   public / protected / private / internal
来源：http://oof.guannengcc.top

[G11] getter / setter
来源：http://rco.yj20258.top

Py:   @property 与 @x.setter
来源：http://lre.guannengcc.top

PHP:  public function getName(): string { return $this->name; }
来源：http://whh.vehdjk.com

JS:   get name() { return this._name; }
来源：http://otf.xuanzx.com

TS:   get name(): string { return this._name; }
来源：http://xzc.shanyushiyangkeji.top

Java: public String getName() { return name; }
来源：http://whx.guannengcc.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://jcl.jlsjyb.cn

Ruby: attr_accessor :name
来源：http://vkc.shzxlz.cn

C#:   public string Name { get; set; }
来源：http://jym.birdmap.top

[G12] 对象转字符串
来源：http://ozx.shangyingyoupin.top

Py:   def __str__(self): return self.name
来源：http://les.jinqigfzy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://uom.wangdashe.top

JS:   toString() { return this.name; }
来源：http://aeh.chenjidiqi.icu

TS:   toString(): string { return this.name; }
来源：http://cgp.sysykeji.top

Java: @Override public String toString() { return name; }
来源：http://uaq.jinyuanbaomall.cn

Go:   func (u User) String() string { return u.Name }
来源：http://eeo.hongshengwenyu.top

Ruby: def to_s; @name; end
来源：http://hio.daria6918.cn

C#:   public override string ToString() => Name;
来源：http://vec.daria6918.cn

[G13] 判断对象类型
来源：http://ccx.guowangkeji.top

Py:   isinstance(u, User)
来源：http://fep.shanyushiyangtech.top

PHP:  $u instanceof User
来源：http://kvz.yonumen.top

JS:   u instanceof User
来源：http://kjw.jyoumei.cn

TS:   u instanceof User
来源：http://hyg.birdmap.top

Java: u instanceof User
来源：http://nnx.mhx1999.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ufn.bbcook.cn

Ruby: u.is_a?(User)
来源：http://usq.dashuyun.cn

C#:   u is User
来源：http://unk.hywenlv.cn

[G14] 数据类 / record
来源：http://uvr.wangdashe.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jsn.zhaomingkeji.xyz

PHP:  // 用 readonly 属性模拟
来源：http://fik.havefunace.top

JS:   // 无内置：普通类或对象字面量
来源：http://qnm.yj20258.top

TS:   type User = { name: string; age: number };
来源：http://ejc.aizwys.cn

Java: record User(String name, int age) {}
来源：http://zsq.sxryk.cn

Go:   type User struct { Name string; Age int }
来源：http://nqm.snrcjt.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zju.dashuyun.cn

C#:   record User(string Name, int Age);
来源：http://guq.xuetiantiany.cn

[G15] 枚举
来源：http://wda.yuxming.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vcy.svipenyu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mia.aizwys.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ipr.hnxiangtu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zoq.hysaishi.cn

Java: enum Color { RED, GREEN }
来源：http://wtb.hcnkem.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lcp.sjlbkw.cn

Ruby: Color = %i[red green].freeze
来源：http://roz.zycfv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rgz.yj202588.top

[G16] 对象转数组 / 字典
来源：http://hez.shzxlz.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jis.aibaodan.cn

PHP:  get_object_vars($obj);
来源：http://yze.cashguo.top

JS:   Object.entries(obj)
来源：http://jdi.mhx1999.top

TS:   Object.entries(obj)
来源：http://pfj.zhaomingkeji.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mmr.ydjk.org.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dsg.yanxiufei.cn

Ruby: obj.instance_variables
来源：http://bqp.ydjk.org.cn

C#:   // 用反射或 System.Text.Json
来源：http://oal.hnqzz.top

================================================================================
来源：http://mdn.uphjek.com

H. 异常与错误处理
来源：http://uxu.xingfuxueyuan.xyz

================================================================================
来源：http://irh.xuetiantiany.cn

[H01] try / catch 基础
来源：http://kbi.birdmap.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ghy.cheryme.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cmf.yj20258888.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tsp.cheryme.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hco.fengsongda.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://iwx.guowangkeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dnc.xuanzx.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rue.zycfv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jwx.52xcode.cn

[H02] finally / ensure 收尾
来源：http://psk.xinyue.icu

Py:   try: f()⏎finally: cleanup()
来源：http://rbq.smart0.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://hog.chenzaomai.com

JS:   try { f(); } finally { cleanup(); }
来源：http://wmm.nwbrower.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ghw.yj202588.top

Java: try { f(); } finally { cleanup(); }
来源：http://nwk.hammf.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zjs.andypj.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://qrw.meibo888.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ssv.zhijiandao.cn

[H03] 主动抛出异常
来源：http://pcn.jyoumei.cn

Py:   raise ValueError("错误信息")
来源：http://tal.kuanghao11.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uxm.yonumen.top

JS:   throw new Error("错误信息");
来源：http://rwe.cucudq.cn

TS:   throw new Error("错误信息");
来源：http://suf.ivvv.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://sbv.yuanzhike.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pyp.yuanzhike.top

Ruby: raise ArgumentError, "错误信息"
来源：http://xpo.ehwqpu.com

C#:   throw new ArgumentException("错误信息");
来源：http://qmy.fengsongda.top

[H04] 自定义异常类型
来源：http://rwt.iojbl.cn

Py:   class MyError(Exception): pass
来源：http://zxe.xylfe.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jez.ywan-chungtsiang.top

JS:   class MyError extends Error {}
来源：http://wjv.yanxiufei.cn

TS:   class MyError extends Error {}
来源：http://cby.xuanzx.com

Java: class MyException extends RuntimeException {}
来源：http://bgp.jinqigufen.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yzs.ppjwa.cn

Ruby: class MyError < StandardError; end
来源：http://clx.vqdsnc.cn

C#:   class MyException : Exception {}
来源：http://gvo.fzhhl.top

[H05] 捕获特定类型
来源：http://nvx.aizwys.cn

Py:   except ValueError as e:
来源：http://afn.mhx1999.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://byx.xuanzx.com

JS:   if (e instanceof TypeError) {}
来源：http://nid.zhaomingkeji.xyz

TS:   if (e instanceof TypeError) {}
来源：http://cho.chenlongwang.top

Java: catch (IOException | SQLException e) {}
来源：http://xhj.52xcode.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ksi.gotoacloud.top

Ruby: rescue ArgumentError => e
来源：http://ljr.xziqi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jty.shuidangran.top

[H06] 可选值 / 空值安全访问
来源：http://owt.hywenlv.cn

Py:   value = d.get("k") or default
来源：http://czi.zhengqikj.top

PHP:  $v = $d["k"] ?? null;
来源：http://kfv.zhiwuduotai.top

JS:   obj?.a?.b;  d ?? default
来源：http://igb.zhijiandao.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jio.jqgufenzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tzp.ppjwa.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mpb.bbcook.cn

Ruby: d&.dig(:a, :b)
来源：http://hat.pengpengdd.cyou

C#:   obj?.A?.B ?? default
来源：http://cel.hongshengwenyu.top

[H07] 断言
来源：http://pli.birdmap.top

Py:   assert x > 0, "必须为正"
来源：http://pth.yanxiufei.cn

PHP:  assert($x > 0);
来源：http://mdd.316326.xyz

JS:   console.assert(x > 0);
来源：http://atn.gaohongyu789.top

TS:   console.assert(x > 0);
来源：http://wwc.jinyuanbaomall.cn

Java: assert x > 0 : "必须为正";
来源：http://ype.hongshengwenyu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dtm.guannengcc.top

Ruby: raise "必须为正" unless x > 0
来源：http://qyx.yj20258888.top

C#:   Debug.Assert(x > 0);
来源：http://kaf.hfpthk.cn

[H08] 获取错误信息与堆栈
来源：http://xqx.xingfuxueyuan.xyz

Py:   str(e);  traceback.format_exc()
来源：http://kmd.iojbl.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zld.xinyue.icu

JS:   e.message;  e.stack
来源：http://laa.jianghu66.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://qcy.9152youxi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ale.fehbvm.com

Go:   err.Error()
来源：http://tmm.shuidangran.top

Ruby: e.message;  e.backtrace
来源：http://hvh.cashguo.top

C#:   e.Message;  e.StackTrace
来源：http://dcy.meibo888.top

[H09] 带错误码的异常
来源：http://mrs.vqdsnc.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gxl.yangfankeji.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://eqj.zhijiandao.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kju.jinqigfzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dcu.birdmap.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ogi.zhiwuduotai.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mzn.dianchejie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pua.cucudq.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gjy.guowangkeji.top

[H10] 资源自动释放
来源：http://esr.fzhhl.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://dnc.mhx1999.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://por.hcnkem.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jyp.kuanghao11.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hzz.daria6918.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bvo.yfazqb.com

Go:   defer f.Close()
来源：http://vdi.zhongyouzk.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wzp.birdmap.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dtt.nanxuanxn.top


<!-- 参考信息 -->