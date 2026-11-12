代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://gki.jianghu66.top

TS:   fs.unlinkSync("a.txt")
来源：http://fpa.jinyuanbaomall.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yur.kuanghao11.cn

Go:   os.Remove("a.txt")
来源：http://juc.zdbjq.cn

Ruby: File.delete("a.txt")
来源：http://nuq.quarkkingdee.top

C#:   File.Delete("a.txt");
来源：http://aaw.hammf.cn

[F07] 创建目录（含多级）
来源：http://hcd.snrcjt.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qao.nanxuanxn.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fvx.ywan-chungtsiang.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hye.zdqjudy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mky.bbcook.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cpv.zhengqikj.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://elr.hongshengwenyu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ydr.cucudq.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ctr.uphjek.com

[F08] 遍历目录
来源：http://kkk.chenzaomai.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://slb.iojbl.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fth.jianghu66.top

JS:   fs.readdirSync("dir")
来源：http://ipe.zhongyouzk.top

TS:   fs.readdirSync("dir")
来源：http://mkc.jinyuanbaomall.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://weo.nwbrower.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://pzs.yuxming.cn

Ruby: Dir.children("dir")
来源：http://nyi.xinyue.icu

C#:   Directory.GetFiles("dir")
来源：http://qyj.cqqwz.cn

[F09] 获取文件大小
来源：http://gnr.yueranfly.top

Py:   os.path.getsize("a.txt")
来源：http://eoo.cqqwz.cn

PHP:  filesize("a.txt");
来源：http://qxk.jiagoushi.top

JS:   fs.statSync("a.txt").size
来源：http://cxr.jyoumei.cn

TS:   fs.statSync("a.txt").size
来源：http://brh.dashuyun.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bnr.jinqigfzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xmf.feifeiyinyue.top

Ruby: File.size("a.txt")
来源：http://lgb.0kj1m.cn

C#:   new FileInfo("a.txt").Length
来源：http://ewg.zycfv.cn

[F10] 取文件扩展名 / 文件名
来源：http://kuj.nanxuanxn.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hdx.cqqwz.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://skh.uphjek.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xax.yj20258888.top

TS:   path.extname("a.txt")
来源：http://gmt.yj202588.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tgu.316326.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mnt.feifeiyinyue.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tlc.yueranfly.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sur.feifeiyinyue.top

[F11] 复制与移动文件
来源：http://ggu.shanyushiyangtech.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qvn.hysaishi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wuk.yangfankeji.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xxp.hammf.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hpp.svipenyu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tob.guannengcc.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://iex.9152youxi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nfe.jqgfzy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pho.ehwqpu.com

[F12] CSV 读写
来源：http://qay.pengpengdd.cyou

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ley.bjfxy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hpo.0kj1m.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xvk.tian-w.cn

TS:   // 同上
来源：http://idn.fehbvm.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zln.tanke756.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://eum.svipenyu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rad.ywan-chungtsiang.top

C#:   // 无内置：用 CsvHelper 库
来源：http://yqw.hfpthk.cn

================================================================================
来源：http://pjz.shangyingyoupin.top

G. 面向对象
来源：http://dhn.hnxiangtu.top

================================================================================
来源：http://kpi.jyoumei.cn

[G01] 定义类
来源：http://eib.fktsv.cn

Py:   class User: pass
来源：http://tnl.tianlin.xyz

PHP:  class User {}
来源：http://egp.zdqjudy.top

JS:   class User {}
来源：http://ect.jyoumei.cn

TS:   class User { name: string = ""; }
来源：http://yug.fzhhl.top

Java: class User {}
来源：http://alc.hnxiangtu.top

Go:   type User struct { Name string }
来源：http://mcz.chenlongwang.top

Ruby: class User; end
来源：http://xqz.fanxiaobao.xyz

C#:   class User {}
来源：http://qrd.iojbl.cn

[G02] 构造函数
来源：http://pup.yonumen.top

Py:   def __init__(self, name): self.name = name
来源：http://yki.jqgfzy.top

PHP:  public function __construct(public string $name) {}
来源：http://pmj.mhx1999.top

JS:   constructor(name) { this.name = name; }
来源：http://rjo.ybcxt.top

TS:   constructor(public name: string) {}
来源：http://ofz.vqdsnc.cn

Java: User(String name) { this.name = name; }
来源：http://rue.shanyushiyangtech.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ohb.hfpthk.cn

Ruby: def initialize(name); @name = name; end
来源：http://rno.ydjk.org.cn

C#:   public User(string name) { Name = name; }
来源：http://aub.hcnkem.com

[G03] 实例属性
来源：http://epi.epnwcf.com

Py:   self.name = "x"
来源：http://zvv.0kj1m.cn

PHP:  public string $name = "x";
来源：http://oyi.fktsv.cn

JS:   this.name = "x";
来源：http://roz.kuanghao11.cn

TS:   name: string = "x";
来源：http://ocj.hfpthk.cn

Java: private String name;
来源：http://zew.andypj.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qyw.cqqwz.cn

Ruby: @name = "x"
来源：http://zan.wangshuangyany.cn

C#:   public string Name { get; set; } = "x";
来源：http://qij.meibo888.top

[G04] 定义方法
来源：http://giy.nanxinkj.top

Py:   def greet(self): return self.name
来源：http://hmh.cdnleiting.top

PHP:  public function greet(): string { return $this->name; }
来源：http://vcx.yfazqb.com

JS:   greet() { return this.name; }
来源：http://ajc.snrcjt.cn

TS:   greet(): string { return this.name; }
来源：http://qvz.smart0.xyz

Java: String greet() { return name; }
来源：http://zbg.zhijiandao.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hhu.gaohongyu789.top

Ruby: def greet; @name; end
来源：http://upb.zdqjudy.top

C#:   public string Greet() => Name;
来源：http://ojb.havefunace.top

[G05] 继承
来源：http://wpt.dashuyun.cn

Py:   class Admin(User): pass
来源：http://wek.zhixingplan.top

PHP:  class Admin extends User {}
来源：http://fmu.zhixingplan.top

JS:   class Admin extends User {}
来源：http://byg.sufxvd.cn

TS:   class Admin extends User {}
来源：http://tdo.nanxuanxn.top

Java: class Admin extends User {}
来源：http://kmh.cheryme.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jkx.redwolf501.top

Ruby: class Admin < User; end
来源：http://toe.jqgfzy.top

C#:   class Admin : User {}
来源：http://gng.zhongyouzk.top

[G06] 重写方法
来源：http://zyx.hnqzz.top

Py:   def greet(self): return "admin"
来源：http://vyn.meibo888.top

PHP:  public function greet(): string { return "admin"; }
来源：http://jwo.yonumen.top

JS:   greet() { return "admin"; }
来源：http://cph.shanyushiyangtech.top

TS:   greet(): string { return "admin"; }
来源：http://sig.jqgfzy.top

Java: @Override String greet() { return "admin"; }
来源：http://xrv.chenzaomai.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fgr.zhongyouzk.top

Ruby: def greet; "admin"; end
来源：http://qyp.sweek.top

C#:   public override string Greet() => "admin";
来源：http://nvw.havefunace.top

[G07] 调用父类方法
来源：http://pyu.yonumen.top

Py:   super().greet()
来源：http://tyf.bjfxy.top

PHP:  parent::greet();
来源：http://mbi.jqgfzy.top

JS:   super.greet();
来源：http://zhf.xuanzx.com

TS:   super.greet();
来源：http://hvz.yangfankeji.com

Java: super.greet();
来源：http://sqc.hongshengwenyu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wgs.ydzc1.top

Ruby: super
来源：http://rjm.pycfn.com

C#:   base.Greet();
来源：http://omj.gotoacloud.top

[G08] 静态方法与属性
来源：http://trz.ehwqpu.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uql.hywenlv.cn

PHP:  public static function f() {}
来源：http://dnp.zhengqikj.top

JS:   static f() {}
来源：http://gsz.zhoulong.xyz

TS:   static f(): void {}
来源：http://ite.yj202588.top

Java: static void f() {}
来源：http://hjq.zhijiandao.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qdx.cqqwz.cn

Ruby: def self.f; end
来源：http://mkn.ybcxt.top

C#:   public static void F() {}
来源：http://thl.shanyushiyangtech.top

[G09] 接口 / 抽象类
来源：http://sco.snrcjt.cn

Py:   from abc import ABC, abstractmethod
来源：http://dol.jinghuilouyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qjq.tanke756.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://hwp.hammf.cn

TS:   interface Shape { area(): number; }
来源：http://vpj.gaohongyu789.top

Java: interface Shape { double area(); }
来源：http://kuh.vqdsnc.cn

Go:   type Shape interface { Area() float64 }
来源：http://qme.jinqigufen.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rpf.zhengqikj.top

C#:   interface IShape { double Area(); }
来源：http://yum.hcnkem.com

[G10] 访问控制
来源：http://pmw.dianchejie.cn

Py:   约定 _protected / __private（不强制）
来源：http://yrm.jianghu66.top

PHP:  public / protected / private
来源：http://evd.tarul.cn

JS:   #private 字段；其余公开
来源：http://rkr.c1oappe.top

TS:   public / protected / private
来源：http://njf.dianchejie.cn

Java: public / protected / private / 默认包级
来源：http://wkc.nwbrower.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://jzo.tarul.cn

Ruby: public / protected / private
来源：http://bci.fengsongda.top

C#:   public / protected / private / internal
来源：http://mxh.xylfe.cn

[G11] getter / setter
来源：http://efy.jinghuilouyu.cn

Py:   @property 与 @x.setter
来源：http://fdu.zhiwuduotai.top

PHP:  public function getName(): string { return $this->name; }
来源：http://kck.wangdashe.top

JS:   get name() { return this._name; }
来源：http://hqi.zhixingplan.top

TS:   get name(): string { return this._name; }
来源：http://ckw.zhengqikj.top

Java: public String getName() { return name; }
来源：http://jnd.9152youxi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://lwf.jyoumei.cn

Ruby: attr_accessor :name
来源：http://sdi.guowangkeji.top

C#:   public string Name { get; set; }
来源：http://vwd.ydjk.org.cn

[G12] 对象转字符串
来源：http://eze.bjfxy.top

Py:   def __str__(self): return self.name
来源：http://oyx.zhengqikj.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://vqy.tarul.cn

JS:   toString() { return this.name; }
来源：http://kfz.iojbl.cn

TS:   toString(): string { return this.name; }
来源：http://yth.yvedp.cn

Java: @Override public String toString() { return name; }
来源：http://oit.smart0.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://ouh.shanyushiyangkeji.top

Ruby: def to_s; @name; end
来源：http://ntj.yj20258.top

C#:   public override string ToString() => Name;
来源：http://sel.vehdjk.com

[G13] 判断对象类型
来源：http://fcd.feifeiyinyue.top

Py:   isinstance(u, User)
来源：http://htq.hywenlv.cn

PHP:  $u instanceof User
来源：http://xqx.fanxiaobao.xyz

JS:   u instanceof User
来源：http://odt.zhongyouzk.top

TS:   u instanceof User
来源：http://cch.zhiwuduotai.top

Java: u instanceof User
来源：http://elz.tianlin.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://usp.wangshuangyany.cn

Ruby: u.is_a?(User)
来源：http://rjs.jinyuanbaomall.cn

C#:   u is User
来源：http://kmi.fanxiaobao.xyz

[G14] 数据类 / record
来源：http://noz.jinqigufen.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fsp.fzhhl.top

PHP:  // 用 readonly 属性模拟
来源：http://clu.sufxvd.cn

JS:   // 无内置：普通类或对象字面量
来源：http://plt.fanxiaobao.xyz

TS:   type User = { name: string; age: number };
来源：http://upn.iojbl.cn

Java: record User(String name, int age) {}
来源：http://zxr.nanxuanxn.top

Go:   type User struct { Name string; Age int }
来源：http://zyl.cashguo.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vpb.ydjk.org.cn

C#:   record User(string Name, int Age);
来源：http://wxu.hongshengwenyu.top

[G15] 枚举
来源：http://jjn.yanxiufei.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vui.yangfankeji.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://fmm.hywenlv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qos.snrcjt.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fyc.sxryk.cn

Java: enum Color { RED, GREEN }
来源：http://mqs.c1oappe.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://iku.jinghuilouyu.cn

Ruby: Color = %i[red green].freeze
来源：http://krt.sweek.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vay.nwbrower.top

[G16] 对象转数组 / 字典
来源：http://cia.c1oappe.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://leh.tian-w.cn

PHP:  get_object_vars($obj);
来源：http://xgy.zhengqikj.top

JS:   Object.entries(obj)
来源：http://tgb.tarul.cn

TS:   Object.entries(obj)
来源：http://vtg.wangshuangyany.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ecv.52xcode.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://woc.snrcjt.cn

Ruby: obj.instance_variables
来源：http://lwi.pengpengdd.cyou

C#:   // 用反射或 System.Text.Json
来源：http://kjl.tanke756.top

================================================================================
来源：http://lhm.pycfn.com

H. 异常与错误处理
来源：http://bby.wangdashe.top

================================================================================
来源：http://nbf.jqgfzy.top

[H01] try / catch 基础
来源：http://oal.hysaishi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bvh.yfazqb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hhk.dashuyun.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rpq.ydzc1.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wea.hongshengwenyu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wct.nanxinkj.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bte.sxryk.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wzy.hcnkem.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bwm.ydjk.org.cn

[H02] finally / ensure 收尾
来源：http://wmd.bjfxy.top

Py:   try: f()⏎finally: cleanup()
来源：http://fwv.9152youxi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jnq.daxiang520.top

JS:   try { f(); } finally { cleanup(); }
来源：http://jxk.dashuyun.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jlj.andypj.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://oqg.gaohongyu789.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://mcy.ydjk.org.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ktv.xuetiantiany.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://eef.tianlin.xyz

[H03] 主动抛出异常
来源：http://ton.316326.xyz

Py:   raise ValueError("错误信息")
来源：http://xnx.yonumen.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nrx.316326.xyz

JS:   throw new Error("错误信息");
来源：http://pzk.jqgfzy.top

TS:   throw new Error("错误信息");
来源：http://kmi.yvedp.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vty.hfpthk.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ucs.shanyushiyangtech.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ifs.hfpthk.cn

C#:   throw new ArgumentException("错误信息");
来源：http://peq.pycfn.com

[H04] 自定义异常类型
来源：http://vky.zhixingplan.top

Py:   class MyError(Exception): pass
来源：http://uou.meibo888.top

PHP:  class MyError extends RuntimeException {}
来源：http://rmy.0kj1m.cn

JS:   class MyError extends Error {}
来源：http://fih.jlsjyb.cn

TS:   class MyError extends Error {}
来源：http://kwd.havefunace.top

Java: class MyException extends RuntimeException {}
来源：http://rwc.sysykeji.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zvc.fanxiaobao.xyz

Ruby: class MyError < StandardError; end
来源：http://ele.zhengqikj.top

C#:   class MyException : Exception {}
来源：http://fqz.ydjk.org.cn

[H05] 捕获特定类型
来源：http://ebv.yonumen.top

Py:   except ValueError as e:
来源：http://vkf.dashuyun.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://emt.shuidangran.top

JS:   if (e instanceof TypeError) {}
来源：http://zmj.sxryk.cn

TS:   if (e instanceof TypeError) {}
来源：http://fdo.hnqzz.top

Java: catch (IOException | SQLException e) {}
来源：http://caw.dianchejie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ebd.xuanzx.com

Ruby: rescue ArgumentError => e
来源：http://pja.bbcook.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gzq.yvedp.cn

[H06] 可选值 / 空值安全访问
来源：http://yws.tarul.cn

Py:   value = d.get("k") or default
来源：http://vty.zhoulong.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://aek.zhoulong.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://gzy.fengsongda.top

TS:   obj?.a?.b;  d ?? default
来源：http://uji.zhaomingkeji.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ivl.yj20258.top

Go:   if v, ok := m["k"]; ok { }
来源：http://tvg.svipenyu.cn

Ruby: d&.dig(:a, :b)
来源：http://ytg.haohaochexian.top

C#:   obj?.A?.B ?? default
来源：http://bfz.svipenyu.cn

[H07] 断言
来源：http://dyk.daxiang520.top

Py:   assert x > 0, "必须为正"
来源：http://xma.zhaomingkeji.xyz

PHP:  assert($x > 0);
来源：http://dhq.hywenlv.cn

JS:   console.assert(x > 0);
来源：http://bbb.ywan-chungtsiang.top

TS:   console.assert(x > 0);
来源：http://vwt.cashguo.top

Java: assert x > 0 : "必须为正";
来源：http://exc.kuanghao11.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rnx.pengpengdd.cyou

Ruby: raise "必须为正" unless x > 0
来源：http://bjp.shanyushiyangkeji.top

C#:   Debug.Assert(x > 0);
来源：http://ouh.ydzc1.top

[H08] 获取错误信息与堆栈
来源：http://zuv.cheryme.top

Py:   str(e);  traceback.format_exc()
来源：http://mur.havefunace.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yrk.ybcxt.top

JS:   e.message;  e.stack
来源：http://uva.hysaishi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://oym.jyoumei.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://omr.sufxvd.cn

Go:   err.Error()
来源：http://arb.jinqigufen.top

Ruby: e.message;  e.backtrace
来源：http://ysl.xingfuxueyuan.xyz

C#:   e.Message;  e.StackTrace
来源：http://ttk.smart0.xyz

[H09] 带错误码的异常
来源：http://qvp.yj20258.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://adl.fehbvm.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://bot.haohaochexian.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vhb.sweek.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zok.pengpengdd.cyou

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hqq.tanke756.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gjk.hfpthk.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ljw.tanke756.top

C#:   // 自定义异常类中加 Code 属性
来源：http://hdo.cdnleiting.top

[H10] 资源自动释放
来源：http://qna.gaohongyu789.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://vrg.shuidangran.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xqv.hysaishi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://otf.shzxlz.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://puk.kuanghao11.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pan.ybcxt.top

Go:   defer f.Close()
来源：http://xqb.c1oappe.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://oyq.yvedp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rrn.smart0.xyz


<!-- 参考信息 -->