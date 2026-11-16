代发 wailian999

C#:   File.Exists("a.txt")
来源：http://fmq.aizwys.cn

[F06] 删除文件
来源：http://jok.xingfuxueyuan.xyz

Py:   os.remove("a.txt")
来源：http://bgn.iojbl.cn

PHP:  unlink("a.txt");
来源：http://dvx.nwbrower.top

JS:   fs.unlinkSync("a.txt")
来源：http://pyf.yvedp.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yqm.uphjek.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nzn.wangshuangyany.cn

Go:   os.Remove("a.txt")
来源：http://mhh.chenlongwang.top

Ruby: File.delete("a.txt")
来源：http://vms.jqgfzy.top

C#:   File.Delete("a.txt");
来源：http://nhm.ydjk.org.cn

[F07] 创建目录（含多级）
来源：http://gxt.jinyuanbaomall.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pux.quarkkingdee.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://iji.meibo888.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zdw.hongshengwenyu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bnl.tanke756.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bsc.xylfe.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bgl.yj20258.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://afe.hnxiangtu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jsh.zhiwuduotai.top

[F08] 遍历目录
来源：http://tal.andypj.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://qug.hywenlv.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oyl.jinghuilouyu.cn

JS:   fs.readdirSync("dir")
来源：http://bin.jinghuilouyu.cn

TS:   fs.readdirSync("dir")
来源：http://dfw.jlsjyb.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://skp.hongshengwenyu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xsb.nanxuanxn.top

Ruby: Dir.children("dir")
来源：http://kqx.jinyuanbaomall.cn

C#:   Directory.GetFiles("dir")
来源：http://ksi.jinyuanbaomall.cn

[F09] 获取文件大小
来源：http://dsy.vehdjk.com

Py:   os.path.getsize("a.txt")
来源：http://lzq.tian-w.cn

PHP:  filesize("a.txt");
来源：http://hpq.yfazqb.com

JS:   fs.statSync("a.txt").size
来源：http://cfn.uphjek.com

TS:   fs.statSync("a.txt").size
来源：http://vip.sufxvd.cn

Java: Files.size(Path.of("a.txt"))
来源：http://etb.mhx1999.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nys.meibo888.top

Ruby: File.size("a.txt")
来源：http://wbw.pengpengdd.cyou

C#:   new FileInfo("a.txt").Length
来源：http://jkn.smart0.xyz

[F10] 取文件扩展名 / 文件名
来源：http://yuo.wangdashe.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qsp.aibaodan.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://idu.sysykeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nww.hammf.cn

TS:   path.extname("a.txt")
来源：http://dkp.yj20258.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ebr.shanyushiyangtech.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://csb.9152youxi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uat.gotoacloud.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dey.daria6918.cn

[F11] 复制与移动文件
来源：http://iqf.xuanzx.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wgx.tian-w.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bso.ctjpmb.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://afw.zhaomingkeji.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://npk.shangyingyoupin.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mzf.tian-w.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jkn.meibo888.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rrk.shanyushiyangkeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vyk.gzhubu.top

[F12] CSV 读写
来源：http://isr.yj202588.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xgm.ydzc1.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://elv.havefunace.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://oku.bbcook.cn

TS:   // 同上
来源：http://pdu.jqgufenzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://eks.c1oappe.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fwa.vehdjk.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eat.dianchejie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tjj.jiagoushi.top

================================================================================
来源：http://ikz.sjlbkw.cn

G. 面向对象
来源：http://kmn.gzhubu.top

================================================================================
来源：http://ejm.shuidangran.top

[G01] 定义类
来源：http://huo.tanke756.top

Py:   class User: pass
来源：http://pdy.jinqigufen.top

PHP:  class User {}
来源：http://xmf.snrcjt.cn

JS:   class User {}
来源：http://wso.aizwys.cn

TS:   class User { name: string = ""; }
来源：http://wnr.fehbvm.com

Java: class User {}
来源：http://zdw.havefunace.top

Go:   type User struct { Name string }
来源：http://pwq.fzhhl.top

Ruby: class User; end
来源：http://gfn.chenlongwang.top

C#:   class User {}
来源：http://lbq.jianghu66.top

[G02] 构造函数
来源：http://aog.nanxuanxn.top

Py:   def __init__(self, name): self.name = name
来源：http://urw.haohaochexian.top

PHP:  public function __construct(public string $name) {}
来源：http://coi.zhaomingkeji.xyz

JS:   constructor(name) { this.name = name; }
来源：http://slj.meibo888.top

TS:   constructor(public name: string) {}
来源：http://vxe.shuidangran.top

Java: User(String name) { this.name = name; }
来源：http://tqy.fanxiaobao.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ucu.vqdsnc.cn

Ruby: def initialize(name); @name = name; end
来源：http://ytx.ctjpmb.com

C#:   public User(string name) { Name = name; }
来源：http://naq.snrcjt.cn

[G03] 实例属性
来源：http://rwr.cashguo.top

Py:   self.name = "x"
来源：http://yol.bbcook.cn

PHP:  public string $name = "x";
来源：http://jeg.yanxiufei.cn

JS:   this.name = "x";
来源：http://qlp.havefunace.top

TS:   name: string = "x";
来源：http://qet.shanyushiyangkeji.top

Java: private String name;
来源：http://cwr.fengsongda.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ofj.xylfe.cn

Ruby: @name = "x"
来源：http://gwi.ydjk.org.cn

C#:   public string Name { get; set; } = "x";
来源：http://eci.jinqigfzy.top

[G04] 定义方法
来源：http://huv.yj20258888.top

Py:   def greet(self): return self.name
来源：http://naf.ehwqpu.com

PHP:  public function greet(): string { return $this->name; }
来源：http://css.xingfuxueyuan.xyz

JS:   greet() { return this.name; }
来源：http://vtt.mhx1999.top

TS:   greet(): string { return this.name; }
来源：http://iuy.shanyushiyangkeji.top

Java: String greet() { return name; }
来源：http://gum.zdqjudy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://npe.ybcxt.top

Ruby: def greet; @name; end
来源：http://mgo.gogol.net.cn

C#:   public string Greet() => Name;
来源：http://ohy.zhixingplan.top

[G05] 继承
来源：http://kxy.tanke756.top

Py:   class Admin(User): pass
来源：http://dfa.xuanzx.com

PHP:  class Admin extends User {}
来源：http://cks.andypj.xyz

JS:   class Admin extends User {}
来源：http://qwj.yueranfly.top

TS:   class Admin extends User {}
来源：http://lcg.fanxiaobao.xyz

Java: class Admin extends User {}
来源：http://bfx.jinyuanbaomall.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ntp.xuetiantiany.cn

Ruby: class Admin < User; end
来源：http://ydy.uphjek.com

C#:   class Admin : User {}
来源：http://jkw.hongshengwenyu.top

[G06] 重写方法
来源：http://yns.yanxiufei.cn

Py:   def greet(self): return "admin"
来源：http://ebg.nanxinkj.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ele.aizwys.cn

JS:   greet() { return "admin"; }
来源：http://due.bjfxy.top

TS:   greet(): string { return "admin"; }
来源：http://tzt.andypj.xyz

Java: @Override String greet() { return "admin"; }
来源：http://vfn.xuetiantiany.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://arw.aizwys.cn

Ruby: def greet; "admin"; end
来源：http://hhb.dashuyun.cn

C#:   public override string Greet() => "admin";
来源：http://efg.guannengcc.top

[G07] 调用父类方法
来源：http://ksd.hongshengwenyu.top

Py:   super().greet()
来源：http://xau.jinqigufen.top

PHP:  parent::greet();
来源：http://ihb.jiagoushi.top

JS:   super.greet();
来源：http://wyb.smart0.xyz

TS:   super.greet();
来源：http://fcz.daxiang520.top

Java: super.greet();
来源：http://rpc.pengpengdd.cyou

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jyr.bbcook.cn

Ruby: super
来源：http://pqu.vqdsnc.cn

C#:   base.Greet();
来源：http://tcf.ybcxt.top

[G08] 静态方法与属性
来源：http://aca.wangdashe.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://itu.yanxiufei.cn

PHP:  public static function f() {}
来源：http://wft.hywenlv.cn

JS:   static f() {}
来源：http://grc.guowangkeji.top

TS:   static f(): void {}
来源：http://hxb.zhixingplan.top

Java: static void f() {}
来源：http://tiu.jqgufenzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://pxb.yongpay.top

Ruby: def self.f; end
来源：http://fqh.shanyushiyangtech.top

C#:   public static void F() {}
来源：http://zrc.yonumen.top

[G09] 接口 / 抽象类
来源：http://xif.vqdsnc.cn

Py:   from abc import ABC, abstractmethod
来源：http://kni.jinghuilouyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lfb.yangfankeji.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://ytd.sufxvd.cn

TS:   interface Shape { area(): number; }
来源：http://puz.xinyue.icu

Java: interface Shape { double area(); }
来源：http://kgs.jqgufenzy.top

Go:   type Shape interface { Area() float64 }
来源：http://cru.dianchejie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xqm.chenjidiqi.icu

C#:   interface IShape { double Area(); }
来源：http://fxb.gotoacloud.top

[G10] 访问控制
来源：http://snp.gzhubu.top

Py:   约定 _protected / __private（不强制）
来源：http://gty.dashuyun.cn

PHP:  public / protected / private
来源：http://tze.316326.xyz

JS:   #private 字段；其余公开
来源：http://edz.yj202588.top

TS:   public / protected / private
来源：http://kns.chenjidiqi.icu

Java: public / protected / private / 默认包级
来源：http://ilc.guannengcc.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://zpt.jqgfzy.top

Ruby: public / protected / private
来源：http://oai.ydjk.org.cn

C#:   public / protected / private / internal
来源：http://aay.jqgufenzy.top

[G11] getter / setter
来源：http://jah.mhx1999.top

Py:   @property 与 @x.setter
来源：http://hsk.yonumen.top

PHP:  public function getName(): string { return $this->name; }
来源：http://hpv.fanxiaobao.xyz

JS:   get name() { return this._name; }
来源：http://les.jqgufenzy.top

TS:   get name(): string { return this._name; }
来源：http://pwz.sjlbkw.cn

Java: public String getName() { return name; }
来源：http://zoc.zhiwuduotai.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://vny.9152youxi.cn

Ruby: attr_accessor :name
来源：http://zbf.shzxlz.cn

C#:   public string Name { get; set; }
来源：http://mjs.hammf.cn

[G12] 对象转字符串
来源：http://qai.yuanzhike.top

Py:   def __str__(self): return self.name
来源：http://aay.ivvv.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://sdo.redwolf501.top

JS:   toString() { return this.name; }
来源：http://qag.havefunace.top

TS:   toString(): string { return this.name; }
来源：http://doz.hfpthk.cn

Java: @Override public String toString() { return name; }
来源：http://och.chenlongwang.top

Go:   func (u User) String() string { return u.Name }
来源：http://dpq.316326.xyz

Ruby: def to_s; @name; end
来源：http://mre.0kj1m.cn

C#:   public override string ToString() => Name;
来源：http://qhw.nwbrower.top

[G13] 判断对象类型
来源：http://kbs.chenjidiqi.icu

Py:   isinstance(u, User)
来源：http://uyb.xziqi.cn

PHP:  $u instanceof User
来源：http://imo.quarkkingdee.top

JS:   u instanceof User
来源：http://xrs.vqdsnc.cn

TS:   u instanceof User
来源：http://djk.yj20258.top

Java: u instanceof User
来源：http://cba.ivvv.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://gdp.pengpengdd.cyou

Ruby: u.is_a?(User)
来源：http://zsy.shuidangran.top

C#:   u is User
来源：http://btz.gaohongyu789.top

[G14] 数据类 / record
来源：http://ard.svipenyu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ird.fzhhl.top

PHP:  // 用 readonly 属性模拟
来源：http://quh.ehwqpu.com

JS:   // 无内置：普通类或对象字面量
来源：http://kho.hysaishi.cn

TS:   type User = { name: string; age: number };
来源：http://olw.quarkkingdee.top

Java: record User(String name, int age) {}
来源：http://zql.0kj1m.cn

Go:   type User struct { Name string; Age int }
来源：http://jsw.sxryk.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://aao.mhx1999.top

C#:   record User(string Name, int Age);
来源：http://vbh.ybcxt.top

[G15] 枚举
来源：http://ouo.316326.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://akp.yongpay.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://xzl.gaohongyu789.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uqk.yj20258888.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ozl.ppjwa.cn

Java: enum Color { RED, GREEN }
来源：http://kpv.redwolf501.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://imp.hcnkem.com

Ruby: Color = %i[red green].freeze
来源：http://pzn.jianghu66.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fzz.9152youxi.cn

[G16] 对象转数组 / 字典
来源：http://yct.zhixingplan.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vdj.yj20258888.top

PHP:  get_object_vars($obj);
来源：http://oti.hfpthk.cn

JS:   Object.entries(obj)
来源：http://wku.hfpthk.cn

TS:   Object.entries(obj)
来源：http://win.pycfn.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xeh.iojbl.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wng.fanxiaobao.xyz

Ruby: obj.instance_variables
来源：http://fpa.mhx1999.top

C#:   // 用反射或 System.Text.Json
来源：http://gwn.mhx1999.top

================================================================================
来源：http://vnj.zhiwuduotai.top

H. 异常与错误处理
来源：http://qkb.bbcook.cn

================================================================================
来源：http://fnb.gogol.net.cn

[H01] try / catch 基础
来源：http://yzw.yj20258888.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dyn.cashguo.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://azn.hnxiangtu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://iyj.fanxiaobao.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qsy.tian-w.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ekb.zhengqikj.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hbd.snrcjt.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nmb.316326.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kur.xingfuxueyuan.xyz

[H02] finally / ensure 收尾
来源：http://zgg.havefunace.top

Py:   try: f()⏎finally: cleanup()
来源：http://vie.gaohongyu789.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://meg.yongpay.top

JS:   try { f(); } finally { cleanup(); }
来源：http://rci.aizwys.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ybz.ybcxt.top

Java: try { f(); } finally { cleanup(); }
来源：http://pyz.yangfankeji.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://glc.fzhhl.top

Ruby: begin; f; ensure; cleanup; end
来源：http://pdu.yanxiufei.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gfq.xingfuxueyuan.xyz

[H03] 主动抛出异常
来源：http://zza.bjfxy.top

Py:   raise ValueError("错误信息")
来源：http://ewz.sweek.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://khv.xingfuxueyuan.xyz

JS:   throw new Error("错误信息");
来源：http://wln.jinghuilouyu.cn

TS:   throw new Error("错误信息");
来源：http://nlw.chenjidiqi.icu

Java: throw new IllegalArgumentException("错误信息");
来源：http://hmg.shzxlz.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kdn.yvedp.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lbt.yuanzhike.top

C#:   throw new ArgumentException("错误信息");
来源：http://pur.smart0.xyz

[H04] 自定义异常类型
来源：http://mve.sweek.top

Py:   class MyError(Exception): pass
来源：http://mkl.xylfe.cn

PHP:  class MyError extends RuntimeException {}
来源：http://opa.yfazqb.com

JS:   class MyError extends Error {}
来源：http://mjv.zhongyouzk.top

TS:   class MyError extends Error {}
来源：http://dix.yangfankeji.com

Java: class MyException extends RuntimeException {}
来源：http://gbk.smart0.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://and.bjfxy.top

Ruby: class MyError < StandardError; end
来源：http://cvj.yvedp.cn

C#:   class MyException : Exception {}
来源：http://ryp.ydzc1.top

[H05] 捕获特定类型
来源：http://ivd.cashguo.top

Py:   except ValueError as e:
来源：http://fif.tarul.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://voz.zycfv.cn

JS:   if (e instanceof TypeError) {}
来源：http://pzf.tianlin.xyz

TS:   if (e instanceof TypeError) {}
来源：http://qkm.cqqwz.cn

Java: catch (IOException | SQLException e) {}
来源：http://dvk.zdbjq.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://abb.daxiang520.top

Ruby: rescue ArgumentError => e
来源：http://jpg.zhoulong.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zxf.nanxinkj.top

[H06] 可选值 / 空值安全访问
来源：http://wlb.jinghuilouyu.cn

Py:   value = d.get("k") or default
来源：http://gbq.pycfn.com

PHP:  $v = $d["k"] ?? null;
来源：http://von.yj202588.top

JS:   obj?.a?.b;  d ?? default
来源：http://exe.yfazqb.com

TS:   obj?.a?.b;  d ?? default
来源：http://upz.snrcjt.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://umh.vehdjk.com

Go:   if v, ok := m["k"]; ok { }
来源：http://njf.nanxinkj.top

Ruby: d&.dig(:a, :b)
来源：http://zpp.cheryme.top

C#:   obj?.A?.B ?? default
来源：http://jja.hnxiangtu.top

[H07] 断言
来源：http://jgs.hnxiangtu.top

Py:   assert x > 0, "必须为正"
来源：http://tho.dashuyun.cn

PHP:  assert($x > 0);
来源：http://sii.bjfxy.top

JS:   console.assert(x > 0);
来源：http://lif.hammf.cn

TS:   console.assert(x > 0);
来源：http://smu.zhiwuduotai.top

Java: assert x > 0 : "必须为正";
来源：http://rsp.9152youxi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sor.cheryme.top

Ruby: raise "必须为正" unless x > 0
来源：http://kuj.jianghu66.top

C#:   Debug.Assert(x > 0);
来源：http://yjv.shuidangran.top

[H08] 获取错误信息与堆栈
来源：http://bja.cqqwz.cn

Py:   str(e);  traceback.format_exc()
来源：http://kxr.cucudq.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mvo.cdnleiting.top

JS:   e.message;  e.stack
来源：http://llq.hongshengwenyu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://syt.epnwcf.com

Java: e.getMessage();  e.printStackTrace()
来源：http://bld.ehwqpu.com

Go:   err.Error()
来源：http://err.hesvh.cn

Ruby: e.message;  e.backtrace
来源：http://jon.hfpthk.cn

C#:   e.Message;  e.StackTrace
来源：http://nnz.uphjek.com

[H09] 带错误码的异常
来源：http://pqx.chenzaomai.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hnj.52xcode.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qdk.kuanghao11.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cti.yvedp.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pvm.fanxiaobao.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hab.wangshuangyany.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lbx.cashguo.top

Ruby: raise MyError.new("fail", 500)
来源：http://sdn.cheryme.top

C#:   // 自定义异常类中加 Code 属性
来源：http://jpd.guannengcc.top

[H10] 资源自动释放
来源：http://nmr.cqqwz.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qds.sweek.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://byx.daria6918.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://esg.zycfv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://azu.wangdashe.top


<!-- 参考信息 -->