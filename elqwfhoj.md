代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://kva.jqgfzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://wos.tianlin.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://okb.hnxiangtu.top

Ruby: File.exist?("a.txt")
来源：http://ahr.sweek.top

C#:   File.Exists("a.txt")
来源：http://dlt.zhaomingkeji.xyz

[F06] 删除文件
来源：http://eaq.fanxiaobao.xyz

Py:   os.remove("a.txt")
来源：http://cum.hesvh.cn

PHP:  unlink("a.txt");
来源：http://drb.ehwqpu.com

JS:   fs.unlinkSync("a.txt")
来源：http://qgf.sufxvd.cn

TS:   fs.unlinkSync("a.txt")
来源：http://sms.yj20258.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rzq.xziqi.cn

Go:   os.Remove("a.txt")
来源：http://xdk.nanxuanxn.top

Ruby: File.delete("a.txt")
来源：http://dre.redwolf501.top

C#:   File.Delete("a.txt");
来源：http://uxw.yongpay.top

[F07] 创建目录（含多级）
来源：http://bog.cqqwz.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mhs.gogol.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fdv.guannengcc.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wlu.sufxvd.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://svk.hongshengwenyu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rnh.tian-w.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cok.zhengqikj.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://iyv.jinqigufen.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bzs.ehwqpu.com

[F08] 遍历目录
来源：http://gbi.hfpthk.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ico.fanxiaobao.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gkf.chenjidiqi.icu

JS:   fs.readdirSync("dir")
来源：http://csm.hfpthk.cn

TS:   fs.readdirSync("dir")
来源：http://qnt.chenjidiqi.icu

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qwf.xziqi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pzw.zhoulong.xyz

Ruby: Dir.children("dir")
来源：http://eht.shzxlz.cn

C#:   Directory.GetFiles("dir")
来源：http://psb.zhongyouzk.top

[F09] 获取文件大小
来源：http://wwv.yj202588.top

Py:   os.path.getsize("a.txt")
来源：http://dlm.fehbvm.com

PHP:  filesize("a.txt");
来源：http://dvk.aizwys.cn

JS:   fs.statSync("a.txt").size
来源：http://qms.havefunace.top

TS:   fs.statSync("a.txt").size
来源：http://jyh.nanxuanxn.top

Java: Files.size(Path.of("a.txt"))
来源：http://shc.smart0.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wmg.hcnkem.com

Ruby: File.size("a.txt")
来源：http://tcn.feifeiyinyue.top

C#:   new FileInfo("a.txt").Length
来源：http://zfg.316326.xyz

[F10] 取文件扩展名 / 文件名
来源：http://vrv.shzxlz.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yiy.52xcode.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vpt.cqqwz.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xfd.iojbl.cn

TS:   path.extname("a.txt")
来源：http://otq.quarkkingdee.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zdg.vqdsnc.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vpr.xinyue.icu

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gwc.tarul.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uxv.pycfn.com

[F11] 复制与移动文件
来源：http://mzt.zhaomingkeji.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cmt.zhiwuduotai.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tog.feifeiyinyue.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://typ.daxiang520.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lvi.zhaomingkeji.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://obo.ctjpmb.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lpy.fehbvm.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fjq.yangfankeji.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sko.zycfv.cn

[F12] CSV 读写
来源：http://brz.jinyuanbaomall.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zve.fehbvm.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://atd.pycfn.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bhs.cqqwz.cn

TS:   // 同上
来源：http://tgg.yj20258.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nzk.hnqzz.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wle.hnqzz.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lci.xuetiantiany.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tqz.guannengcc.top

================================================================================
来源：http://nwn.nanxuanxn.top

G. 面向对象
来源：http://kwh.xinyue.icu

================================================================================
来源：http://kjt.hammf.cn

[G01] 定义类
来源：http://fav.fktsv.cn

Py:   class User: pass
来源：http://lcl.tarul.cn

PHP:  class User {}
来源：http://jax.ydzc1.top

JS:   class User {}
来源：http://fnm.hywenlv.cn

TS:   class User { name: string = ""; }
来源：http://ftj.shanyushiyangtech.top

Java: class User {}
来源：http://rnt.nanxuanxn.top

Go:   type User struct { Name string }
来源：http://dgb.zdqjudy.top

Ruby: class User; end
来源：http://hrs.cdnleiting.top

C#:   class User {}
来源：http://kbu.quarkkingdee.top

[G02] 构造函数
来源：http://wxe.daxiang520.top

Py:   def __init__(self, name): self.name = name
来源：http://acz.jinghuilouyu.cn

PHP:  public function __construct(public string $name) {}
来源：http://byc.kuanghao11.cn

JS:   constructor(name) { this.name = name; }
来源：http://xyy.zhengqikj.top

TS:   constructor(public name: string) {}
来源：http://iyj.bbcook.cn

Java: User(String name) { this.name = name; }
来源：http://xjx.sweek.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zfc.vehdjk.com

Ruby: def initialize(name); @name = name; end
来源：http://xdr.quarkkingdee.top

C#:   public User(string name) { Name = name; }
来源：http://hmz.ctjpmb.com

[G03] 实例属性
来源：http://hgy.xinyue.icu

Py:   self.name = "x"
来源：http://iga.guowangkeji.top

PHP:  public string $name = "x";
来源：http://une.meibo888.top

JS:   this.name = "x";
来源：http://cdm.wangshuangyany.cn

TS:   name: string = "x";
来源：http://rap.cdnleiting.top

Java: private String name;
来源：http://jww.wangdashe.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vgc.zhengqikj.top

Ruby: @name = "x"
来源：http://odl.yueranfly.top

C#:   public string Name { get; set; } = "x";
来源：http://vnq.xinyue.icu

[G04] 定义方法
来源：http://ibx.ehwqpu.com

Py:   def greet(self): return self.name
来源：http://cgj.316326.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://xlf.yonumen.top

JS:   greet() { return this.name; }
来源：http://tbs.sysykeji.top

TS:   greet(): string { return this.name; }
来源：http://qyw.nwbrower.top

Java: String greet() { return name; }
来源：http://mnk.wangshuangyany.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wkb.shangyingyoupin.top

Ruby: def greet; @name; end
来源：http://kow.zhiwuduotai.top

C#:   public string Greet() => Name;
来源：http://kdz.nanxuanxn.top

[G05] 继承
来源：http://wbh.gzhubu.top

Py:   class Admin(User): pass
来源：http://wqw.gzhubu.top

PHP:  class Admin extends User {}
来源：http://hca.jiagoushi.top

JS:   class Admin extends User {}
来源：http://jey.gzhubu.top

TS:   class Admin extends User {}
来源：http://wpn.hcnkem.com

Java: class Admin extends User {}
来源：http://jap.yueranfly.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ric.yangfankeji.com

Ruby: class Admin < User; end
来源：http://qeh.ctjpmb.com

C#:   class Admin : User {}
来源：http://zbv.zdqjudy.top

[G06] 重写方法
来源：http://dvp.ppjwa.cn

Py:   def greet(self): return "admin"
来源：http://ptf.jqgufenzy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://hmq.yj20258888.top

JS:   greet() { return "admin"; }
来源：http://muj.jianghu66.top

TS:   greet(): string { return "admin"; }
来源：http://uns.yueranfly.top

Java: @Override String greet() { return "admin"; }
来源：http://etp.ybcxt.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vhf.smart0.xyz

Ruby: def greet; "admin"; end
来源：http://ezr.xylfe.cn

C#:   public override string Greet() => "admin";
来源：http://ejq.daria6918.cn

[G07] 调用父类方法
来源：http://udv.ehwqpu.com

Py:   super().greet()
来源：http://tds.jyoumei.cn

PHP:  parent::greet();
来源：http://ptt.haohaochexian.top

JS:   super.greet();
来源：http://jsl.ppjwa.cn

TS:   super.greet();
来源：http://yuf.zhaomingkeji.xyz

Java: super.greet();
来源：http://blm.aibaodan.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yfk.cqqwz.cn

Ruby: super
来源：http://afe.gogol.net.cn

C#:   base.Greet();
来源：http://ikr.sysykeji.top

[G08] 静态方法与属性
来源：http://qak.zhaomingkeji.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xxe.yueranfly.top

PHP:  public static function f() {}
来源：http://lcu.jqgfzy.top

JS:   static f() {}
来源：http://jbn.nanxuanxn.top

TS:   static f(): void {}
来源：http://ara.zhiwuduotai.top

Java: static void f() {}
来源：http://qtb.aizwys.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://lip.kuanghao11.cn

Ruby: def self.f; end
来源：http://nzy.fzhhl.top

C#:   public static void F() {}
来源：http://zho.dianchejie.cn

[G09] 接口 / 抽象类
来源：http://uce.jianghu66.top

Py:   from abc import ABC, abstractmethod
来源：http://uww.hammf.cn

PHP:  interface Shape { public function area(): float; }
来源：http://chp.chenlongwang.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://iyb.dianchejie.cn

TS:   interface Shape { area(): number; }
来源：http://afn.xuetiantiany.cn

Java: interface Shape { double area(); }
来源：http://fxh.snrcjt.cn

Go:   type Shape interface { Area() float64 }
来源：http://fht.jinghuilouyu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gnw.jiagoushi.top

C#:   interface IShape { double Area(); }
来源：http://bcv.xziqi.cn

[G10] 访问控制
来源：http://xrt.andypj.xyz

Py:   约定 _protected / __private（不强制）
来源：http://pgi.sjlbkw.cn

PHP:  public / protected / private
来源：http://qnh.gaohongyu789.top

JS:   #private 字段；其余公开
来源：http://kuq.cucudq.cn

TS:   public / protected / private
来源：http://cux.aizwys.cn

Java: public / protected / private / 默认包级
来源：http://nxh.zhiwuduotai.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://mif.sjlbkw.cn

Ruby: public / protected / private
来源：http://mwr.jlsjyb.cn

C#:   public / protected / private / internal
来源：http://vid.fehbvm.com

[G11] getter / setter
来源：http://wsq.havefunace.top

Py:   @property 与 @x.setter
来源：http://fup.cdnleiting.top

PHP:  public function getName(): string { return $this->name; }
来源：http://gtl.hysaishi.cn

JS:   get name() { return this._name; }
来源：http://tnt.sweek.top

TS:   get name(): string { return this._name; }
来源：http://min.jlsjyb.cn

Java: public String getName() { return name; }
来源：http://cjp.feifeiyinyue.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://qsq.gotoacloud.top

Ruby: attr_accessor :name
来源：http://vti.zdbjq.cn

C#:   public string Name { get; set; }
来源：http://lfj.haohaochexian.top

[G12] 对象转字符串
来源：http://eiq.gzhubu.top

Py:   def __str__(self): return self.name
来源：http://lpo.tian-w.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://uyh.hywenlv.cn

JS:   toString() { return this.name; }
来源：http://dfj.zhaomingkeji.xyz

TS:   toString(): string { return this.name; }
来源：http://jsm.gzhubu.top

Java: @Override public String toString() { return name; }
来源：http://lbw.wangshuangyany.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vdg.hysaishi.cn

Ruby: def to_s; @name; end
来源：http://grx.zhijiandao.cn

C#:   public override string ToString() => Name;
来源：http://ejo.sufxvd.cn

[G13] 判断对象类型
来源：http://ufg.cashguo.top

Py:   isinstance(u, User)
来源：http://wfe.pengpengdd.cyou

PHP:  $u instanceof User
来源：http://zbz.nanxuanxn.top

JS:   u instanceof User
来源：http://syl.haohaochexian.top

TS:   u instanceof User
来源：http://irb.gogol.net.cn

Java: u instanceof User
来源：http://uux.smart0.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://zhn.yuxming.cn

Ruby: u.is_a?(User)
来源：http://gpc.havefunace.top

C#:   u is User
来源：http://aqx.zhongyouzk.top

[G14] 数据类 / record
来源：http://thg.jianghu66.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://njo.ctjpmb.com

PHP:  // 用 readonly 属性模拟
来源：http://plz.hysaishi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://erd.bjfxy.top

TS:   type User = { name: string; age: number };
来源：http://wqq.jiagoushi.top

Java: record User(String name, int age) {}
来源：http://zez.yongpay.top

Go:   type User struct { Name string; Age int }
来源：http://dib.sjlbkw.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xxw.yj202588.top

C#:   record User(string Name, int Age);
来源：http://jch.jqgfzy.top

[G15] 枚举
来源：http://vuj.uphjek.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://slr.fzhhl.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://bza.guowangkeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uxe.316326.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pyl.guannengcc.top

Java: enum Color { RED, GREEN }
来源：http://uub.nwbrower.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ixa.tarul.cn

Ruby: Color = %i[red green].freeze
来源：http://ohd.sjlbkw.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bkc.ywan-chungtsiang.top

[G16] 对象转数组 / 字典
来源：http://xej.gzhubu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://weq.svipenyu.cn

PHP:  get_object_vars($obj);
来源：http://mpe.hnqzz.top

JS:   Object.entries(obj)
来源：http://rhi.aizwys.cn

TS:   Object.entries(obj)
来源：http://fgc.ywan-chungtsiang.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jca.iojbl.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xeo.cqqwz.cn

Ruby: obj.instance_variables
来源：http://cxd.zhongyouzk.top

C#:   // 用反射或 System.Text.Json
来源：http://qij.gogol.net.cn

================================================================================
来源：http://cok.hammf.cn

H. 异常与错误处理
来源：http://nqp.kuanghao11.cn

================================================================================
来源：http://eic.nanxuanxn.top

[H01] try / catch 基础
来源：http://fpe.316326.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uoc.yanxiufei.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wlt.zhoulong.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://iyn.yvedp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://aia.iojbl.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pif.fehbvm.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ufa.shanyushiyangkeji.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ojm.guowangkeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kze.9152youxi.cn

[H02] finally / ensure 收尾
来源：http://vyq.jianghu66.top

Py:   try: f()⏎finally: cleanup()
来源：http://wvv.redwolf501.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ewu.yuanzhike.top

JS:   try { f(); } finally { cleanup(); }
来源：http://pwh.vehdjk.com

TS:   try { f(); } finally { cleanup(); }
来源：http://abp.yj20258888.top

Java: try { f(); } finally { cleanup(); }
来源：http://ywq.yj20258.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://amg.zhaomingkeji.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://lik.vqdsnc.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jst.yj202588.top

[H03] 主动抛出异常
来源：http://wfr.sxryk.cn

Py:   raise ValueError("错误信息")
来源：http://msf.sysykeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qbj.nanxuanxn.top

JS:   throw new Error("错误信息");
来源：http://otb.ydzc1.top

TS:   throw new Error("错误信息");
来源：http://ttr.xuetiantiany.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gvu.0kj1m.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://grm.sjlbkw.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://nhy.zycfv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qql.vqdsnc.cn

[H04] 自定义异常类型
来源：http://gxo.yj20258.top

Py:   class MyError(Exception): pass
来源：http://srd.hysaishi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://kck.cdnleiting.top

JS:   class MyError extends Error {}
来源：http://zpj.c1oappe.top

TS:   class MyError extends Error {}
来源：http://ump.shzxlz.cn

Java: class MyException extends RuntimeException {}
来源：http://lqx.guannengcc.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lnm.daxiang520.top

Ruby: class MyError < StandardError; end
来源：http://vcy.yuanzhike.top

C#:   class MyException : Exception {}
来源：http://kiz.yuanzhike.top

[H05] 捕获特定类型
来源：http://wwi.tianlin.xyz

Py:   except ValueError as e:
来源：http://nrj.jyoumei.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jjt.yongpay.top

JS:   if (e instanceof TypeError) {}
来源：http://ihd.wangdashe.top

TS:   if (e instanceof TypeError) {}
来源：http://dny.yj20258888.top

Java: catch (IOException | SQLException e) {}
来源：http://ufy.ivvv.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://joy.xingfuxueyuan.xyz

Ruby: rescue ArgumentError => e
来源：http://rii.gotoacloud.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zwu.nanxuanxn.top

[H06] 可选值 / 空值安全访问
来源：http://twg.kuanghao11.cn

Py:   value = d.get("k") or default
来源：http://bet.fzhhl.top

PHP:  $v = $d["k"] ?? null;
来源：http://sfs.hesvh.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jnw.jianghu66.top

TS:   obj?.a?.b;  d ?? default
来源：http://uxj.uphjek.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wix.ivvv.top

Go:   if v, ok := m["k"]; ok { }
来源：http://phx.jianghu66.top

Ruby: d&.dig(:a, :b)
来源：http://ltt.yj202588.top

C#:   obj?.A?.B ?? default
来源：http://yxa.feifeiyinyue.top

[H07] 断言
来源：http://nrz.sxryk.cn

Py:   assert x > 0, "必须为正"
来源：http://mlc.aibaodan.cn

PHP:  assert($x > 0);
来源：http://ocg.sufxvd.cn

JS:   console.assert(x > 0);
来源：http://dow.gzhubu.top

TS:   console.assert(x > 0);
来源：http://ugr.jinqigufen.top

Java: assert x > 0 : "必须为正";
来源：http://umd.tian-w.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rrr.yj202588.top

Ruby: raise "必须为正" unless x > 0
来源：http://fnq.316326.xyz

C#:   Debug.Assert(x > 0);
来源：http://pkz.shangyingyoupin.top

[H08] 获取错误信息与堆栈
来源：http://bzh.ydjk.org.cn

Py:   str(e);  traceback.format_exc()
来源：http://ktc.bjfxy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bna.wangdashe.top

JS:   e.message;  e.stack
来源：http://ycf.nwbrower.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://kot.jiagoushi.top

Java: e.getMessage();  e.printStackTrace()
来源：http://hjy.bjfxy.top

Go:   err.Error()
来源：http://syk.tianlin.xyz

Ruby: e.message;  e.backtrace
来源：http://dog.sjlbkw.cn

C#:   e.Message;  e.StackTrace
来源：http://abc.zdqjudy.top

[H09] 带错误码的异常
来源：http://cet.cucudq.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tuc.kuanghao11.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ddq.xziqi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jdt.shangyingyoupin.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://riw.meibo888.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lqk.jyoumei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ude.xylfe.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qpi.snrcjt.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vqx.vehdjk.com

[H10] 资源自动释放
来源：http://ssl.shuidangran.top


<!-- 参考信息 -->