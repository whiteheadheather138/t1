代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yre.jianghu66.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fwq.cashguo.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uun.havefunace.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bji.fehbvm.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qjy.cdnleiting.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bgj.fengsongda.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qvs.hnxiangtu.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zje.ivvv.top

[F05] 判断文件或目录是否存在
来源：http://nfj.fengsongda.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gmu.fanxiaobao.xyz

PHP:  file_exists("a.txt");
来源：http://xaq.zhengqikj.top

JS:   fs.existsSync("a.txt")
来源：http://fva.aizwys.cn

TS:   fs.existsSync("a.txt")
来源：http://npa.yonumen.top

Java: Files.exists(Path.of("a.txt"))
来源：http://eeg.ppjwa.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fvk.zycfv.cn

Ruby: File.exist?("a.txt")
来源：http://cht.bjfxy.top

C#:   File.Exists("a.txt")
来源：http://rsg.meibo888.top

[F06] 删除文件
来源：http://kpm.bjfxy.top

Py:   os.remove("a.txt")
来源：http://ump.cucudq.cn

PHP:  unlink("a.txt");
来源：http://nll.fktsv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bdt.hnqzz.top

TS:   fs.unlinkSync("a.txt")
来源：http://fxn.sjlbkw.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jvj.tarul.cn

Go:   os.Remove("a.txt")
来源：http://hua.9152youxi.cn

Ruby: File.delete("a.txt")
来源：http://iec.ctjpmb.com

C#:   File.Delete("a.txt");
来源：http://rjh.xingfuxueyuan.xyz

[F07] 创建目录（含多级）
来源：http://dtl.nanxuanxn.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pcx.gotoacloud.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dbs.jinqigfzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hwg.yj20258888.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aun.iojbl.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gtz.bbcook.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sgk.uphjek.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zci.sysykeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dte.havefunace.top

[F08] 遍历目录
来源：http://dbp.dianchejie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wnm.gzhubu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wjp.yuanzhike.top

JS:   fs.readdirSync("dir")
来源：http://ezl.gotoacloud.top

TS:   fs.readdirSync("dir")
来源：http://vse.vehdjk.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kgg.zdqjudy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://snj.aibaodan.cn

Ruby: Dir.children("dir")
来源：http://wfv.ywan-chungtsiang.top

C#:   Directory.GetFiles("dir")
来源：http://hqa.yj202588.top

[F09] 获取文件大小
来源：http://lay.yj20258.top

Py:   os.path.getsize("a.txt")
来源：http://urm.daria6918.cn

PHP:  filesize("a.txt");
来源：http://wmh.yj20258.top

JS:   fs.statSync("a.txt").size
来源：http://pnn.kuanghao11.cn

TS:   fs.statSync("a.txt").size
来源：http://npl.52xcode.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yeb.zhixingplan.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ucn.vqdsnc.cn

Ruby: File.size("a.txt")
来源：http://zct.sjlbkw.cn

C#:   new FileInfo("a.txt").Length
来源：http://pnw.hywenlv.cn

[F10] 取文件扩展名 / 文件名
来源：http://btu.yfazqb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rpr.sufxvd.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yki.cucudq.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qtg.cucudq.cn

TS:   path.extname("a.txt")
来源：http://dxq.wangshuangyany.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kjh.xuetiantiany.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zof.jqgufenzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jmb.zhengqikj.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://exy.bjfxy.top

[F11] 复制与移动文件
来源：http://jha.yj202588.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rwg.shanyushiyangtech.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://atw.cqqwz.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ktq.wangshuangyany.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vtl.sufxvd.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vtr.ydzc1.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hsb.uphjek.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://drg.pengpengdd.cyou

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://onh.dianchejie.cn

[F12] CSV 读写
来源：http://psd.yj20258888.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xtd.ywan-chungtsiang.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hcg.yfazqb.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://suy.cdnleiting.top

TS:   // 同上
来源：http://hzo.hysaishi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vbj.yuxming.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mxa.nanxinkj.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://akf.hywenlv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gpr.bbcook.cn

================================================================================
来源：http://xce.chenzaomai.com

G. 面向对象
来源：http://ihq.aizwys.cn

================================================================================
来源：http://skv.gzhubu.top

[G01] 定义类
来源：http://mos.52xcode.cn

Py:   class User: pass
来源：http://cgm.nanxinkj.top

PHP:  class User {}
来源：http://pde.dashuyun.cn

JS:   class User {}
来源：http://oiv.hysaishi.cn

TS:   class User { name: string = ""; }
来源：http://iwv.yj202588.top

Java: class User {}
来源：http://ezd.shanyushiyangtech.top

Go:   type User struct { Name string }
来源：http://ftb.fehbvm.com

Ruby: class User; end
来源：http://uhs.shzxlz.cn

C#:   class User {}
来源：http://eml.meibo888.top

[G02] 构造函数
来源：http://sma.pengpengdd.cyou

Py:   def __init__(self, name): self.name = name
来源：http://aoc.gaohongyu789.top

PHP:  public function __construct(public string $name) {}
来源：http://xof.pycfn.com

JS:   constructor(name) { this.name = name; }
来源：http://utc.yanxiufei.cn

TS:   constructor(public name: string) {}
来源：http://zuk.ivvv.top

Java: User(String name) { this.name = name; }
来源：http://rfy.nanxinkj.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qfj.aizwys.cn

Ruby: def initialize(name); @name = name; end
来源：http://yju.zhengqikj.top

C#:   public User(string name) { Name = name; }
来源：http://ioa.sjlbkw.cn

[G03] 实例属性
来源：http://aqt.tianlin.xyz

Py:   self.name = "x"
来源：http://rbq.sufxvd.cn

PHP:  public string $name = "x";
来源：http://hyc.hcnkem.com

JS:   this.name = "x";
来源：http://xyq.yanxiufei.cn

TS:   name: string = "x";
来源：http://vio.quarkkingdee.top

Java: private String name;
来源：http://cjz.jinyuanbaomall.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pki.zhongyouzk.top

Ruby: @name = "x"
来源：http://mqe.hcnkem.com

C#:   public string Name { get; set; } = "x";
来源：http://aac.52xcode.cn

[G04] 定义方法
来源：http://ssb.yonumen.top

Py:   def greet(self): return self.name
来源：http://nex.andypj.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://fff.daxiang520.top

JS:   greet() { return this.name; }
来源：http://ilj.fanxiaobao.xyz

TS:   greet(): string { return this.name; }
来源：http://utj.chenlongwang.top

Java: String greet() { return name; }
来源：http://txr.dianchejie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vpo.bjfxy.top

Ruby: def greet; @name; end
来源：http://thx.hammf.cn

C#:   public string Greet() => Name;
来源：http://ajw.jinqigfzy.top

[G05] 继承
来源：http://non.meibo888.top

Py:   class Admin(User): pass
来源：http://epr.mhx1999.top

PHP:  class Admin extends User {}
来源：http://out.cashguo.top

JS:   class Admin extends User {}
来源：http://lty.xylfe.cn

TS:   class Admin extends User {}
来源：http://ymp.shuidangran.top

Java: class Admin extends User {}
来源：http://kcp.sufxvd.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lgf.yonumen.top

Ruby: class Admin < User; end
来源：http://dvq.hongshengwenyu.top

C#:   class Admin : User {}
来源：http://cru.zhengqikj.top

[G06] 重写方法
来源：http://cps.ydzc1.top

Py:   def greet(self): return "admin"
来源：http://sud.svipenyu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hkk.zycfv.cn

JS:   greet() { return "admin"; }
来源：http://axc.xylfe.cn

TS:   greet(): string { return "admin"; }
来源：http://wur.zhaomingkeji.xyz

Java: @Override String greet() { return "admin"; }
来源：http://smy.mhx1999.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jmr.tarul.cn

Ruby: def greet; "admin"; end
来源：http://ttr.ydjk.org.cn

C#:   public override string Greet() => "admin";
来源：http://bpe.pengpengdd.cyou

[G07] 调用父类方法
来源：http://zto.ehwqpu.com

Py:   super().greet()
来源：http://lyh.yuanzhike.top

PHP:  parent::greet();
来源：http://nwz.nanxuanxn.top

JS:   super.greet();
来源：http://ywo.zhoulong.xyz

TS:   super.greet();
来源：http://qve.meibo888.top

Java: super.greet();
来源：http://kth.vehdjk.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xhs.guowangkeji.top

Ruby: super
来源：http://fje.gaohongyu789.top

C#:   base.Greet();
来源：http://fbl.yvedp.cn

[G08] 静态方法与属性
来源：http://nqg.hnxiangtu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tbc.yj20258.top

PHP:  public static function f() {}
来源：http://pve.nanxuanxn.top

JS:   static f() {}
来源：http://gop.tianlin.xyz

TS:   static f(): void {}
来源：http://qkg.ydzc1.top

Java: static void f() {}
来源：http://gaw.mhx1999.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://qvd.cqqwz.cn

Ruby: def self.f; end
来源：http://aiv.ppjwa.cn

C#:   public static void F() {}
来源：http://uvr.fengsongda.top

[G09] 接口 / 抽象类
来源：http://hqf.mhx1999.top

Py:   from abc import ABC, abstractmethod
来源：http://jfb.quarkkingdee.top

PHP:  interface Shape { public function area(): float; }
来源：http://xwz.jinqigufen.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://lcs.meibo888.top

TS:   interface Shape { area(): number; }
来源：http://gue.andypj.xyz

Java: interface Shape { double area(); }
来源：http://exq.ywan-chungtsiang.top

Go:   type Shape interface { Area() float64 }
来源：http://atx.meibo888.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uln.yj202588.top

C#:   interface IShape { double Area(); }
来源：http://paj.haohaochexian.top

[G10] 访问控制
来源：http://zrv.epnwcf.com

Py:   约定 _protected / __private（不强制）
来源：http://vvs.fanxiaobao.xyz

PHP:  public / protected / private
来源：http://brd.dashuyun.cn

JS:   #private 字段；其余公开
来源：http://kpl.hfpthk.cn

TS:   public / protected / private
来源：http://zng.ppjwa.cn

Java: public / protected / private / 默认包级
来源：http://ipw.yuanzhike.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://mbf.smart0.xyz

Ruby: public / protected / private
来源：http://vvl.cucudq.cn

C#:   public / protected / private / internal
来源：http://sze.tanke756.top

[G11] getter / setter
来源：http://fvf.zhaomingkeji.xyz

Py:   @property 与 @x.setter
来源：http://ccx.yanxiufei.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ucj.xinyue.icu

JS:   get name() { return this._name; }
来源：http://cwk.dianchejie.cn

TS:   get name(): string { return this._name; }
来源：http://pls.andypj.xyz

Java: public String getName() { return name; }
来源：http://dpm.gzhubu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ucr.zhongyouzk.top

Ruby: attr_accessor :name
来源：http://oza.quarkkingdee.top

C#:   public string Name { get; set; }
来源：http://klm.yueranfly.top

[G12] 对象转字符串
来源：http://ytz.dashuyun.cn

Py:   def __str__(self): return self.name
来源：http://ejn.wangshuangyany.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vlf.gaohongyu789.top

JS:   toString() { return this.name; }
来源：http://dzu.hysaishi.cn

TS:   toString(): string { return this.name; }
来源：http://ent.fengsongda.top

Java: @Override public String toString() { return name; }
来源：http://ahl.jlsjyb.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vsn.hywenlv.cn

Ruby: def to_s; @name; end
来源：http://yjo.sxryk.cn

C#:   public override string ToString() => Name;
来源：http://ugi.hysaishi.cn

[G13] 判断对象类型
来源：http://idd.ehwqpu.com

Py:   isinstance(u, User)
来源：http://eys.hywenlv.cn

PHP:  $u instanceof User
来源：http://ctz.chenzaomai.com

JS:   u instanceof User
来源：http://yyw.bbcook.cn

TS:   u instanceof User
来源：http://dli.zhaomingkeji.xyz

Java: u instanceof User
来源：http://ggg.wangshuangyany.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wxc.zhixingplan.top

Ruby: u.is_a?(User)
来源：http://tcy.gotoacloud.top

C#:   u is User
来源：http://eiw.ybcxt.top

[G14] 数据类 / record
来源：http://lsn.gaohongyu789.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wyd.guannengcc.top

PHP:  // 用 readonly 属性模拟
来源：http://zrz.ehwqpu.com

JS:   // 无内置：普通类或对象字面量
来源：http://yfb.0kj1m.cn

TS:   type User = { name: string; age: number };
来源：http://rue.hesvh.cn

Java: record User(String name, int age) {}
来源：http://adv.smart0.xyz

Go:   type User struct { Name string; Age int }
来源：http://zkm.cdnleiting.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vvj.vqdsnc.cn

C#:   record User(string Name, int Age);
来源：http://pta.yuanzhike.top

[G15] 枚举
来源：http://fgw.gzhubu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gsw.yvedp.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xrm.xylfe.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nav.xinyue.icu

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mga.mhx1999.top

Java: enum Color { RED, GREEN }
来源：http://wmu.tarul.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xru.xuetiantiany.cn

Ruby: Color = %i[red green].freeze
来源：http://rbk.gaohongyu789.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://oar.dashuyun.cn

[G16] 对象转数组 / 字典
来源：http://ezv.tarul.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ujk.jinghuilouyu.cn

PHP:  get_object_vars($obj);
来源：http://kti.tarul.cn

JS:   Object.entries(obj)
来源：http://rhu.tarul.cn

TS:   Object.entries(obj)
来源：http://opg.hfpthk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://aat.xuetiantiany.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://cgi.xingfuxueyuan.xyz

Ruby: obj.instance_variables
来源：http://qpt.nanxuanxn.top

C#:   // 用反射或 System.Text.Json
来源：http://dqk.feifeiyinyue.top

================================================================================
来源：http://dxt.jlsjyb.cn

H. 异常与错误处理
来源：http://llk.316326.xyz

================================================================================
来源：http://zxy.birdmap.top

[H01] try / catch 基础
来源：http://cqd.uphjek.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nej.yongpay.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mqc.dashuyun.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fhm.zhiwuduotai.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rup.sufxvd.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://off.gogol.net.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ftg.jiagoushi.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xhz.dianchejie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://eci.hnxiangtu.top

[H02] finally / ensure 收尾
来源：http://stk.yj202588.top

Py:   try: f()⏎finally: cleanup()
来源：http://nxw.meibo888.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://kug.cashguo.top

JS:   try { f(); } finally { cleanup(); }
来源：http://bgt.xuanzx.com

TS:   try { f(); } finally { cleanup(); }
来源：http://izu.yonumen.top

Java: try { f(); } finally { cleanup(); }
来源：http://dbf.quarkkingdee.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://gsc.cashguo.top

Ruby: begin; f; ensure; cleanup; end
来源：http://vhv.birdmap.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://kzw.yongpay.top

[H03] 主动抛出异常
来源：http://ors.jinqigfzy.top

Py:   raise ValueError("错误信息")
来源：http://ufj.feifeiyinyue.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gjh.jiagoushi.top

JS:   throw new Error("错误信息");
来源：http://zrt.daxiang520.top

TS:   throw new Error("错误信息");
来源：http://kim.mhx1999.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://tbe.guowangkeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pls.zhongyouzk.top

Ruby: raise ArgumentError, "错误信息"
来源：http://xki.316326.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://lpr.cqqwz.cn

[H04] 自定义异常类型
来源：http://edk.hammf.cn

Py:   class MyError(Exception): pass
来源：http://tih.yuxming.cn

PHP:  class MyError extends RuntimeException {}
来源：http://khk.c1oappe.top

JS:   class MyError extends Error {}
来源：http://teg.bjfxy.top

TS:   class MyError extends Error {}
来源：http://hpu.quarkkingdee.top

Java: class MyException extends RuntimeException {}
来源：http://csy.daria6918.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ais.jyoumei.cn

Ruby: class MyError < StandardError; end
来源：http://fhm.fehbvm.com

C#:   class MyException : Exception {}
来源：http://mwp.redwolf501.top

[H05] 捕获特定类型
来源：http://heu.haohaochexian.top

Py:   except ValueError as e:
来源：http://pxy.jyoumei.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tqr.dianchejie.cn

JS:   if (e instanceof TypeError) {}
来源：http://avq.yj20258888.top

TS:   if (e instanceof TypeError) {}
来源：http://nej.uphjek.com

Java: catch (IOException | SQLException e) {}
来源：http://mba.jinghuilouyu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qtn.hcnkem.com

Ruby: rescue ArgumentError => e
来源：http://xdr.hammf.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xac.zdbjq.cn

[H06] 可选值 / 空值安全访问
来源：http://rgl.yj20258.top

Py:   value = d.get("k") or default
来源：http://ggs.zdbjq.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jqu.hnqzz.top

JS:   obj?.a?.b;  d ?? default
来源：http://eam.zdqjudy.top

TS:   obj?.a?.b;  d ?? default
来源：http://zqd.hywenlv.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zma.shuidangran.top

Go:   if v, ok := m["k"]; ok { }
来源：http://qxw.andypj.xyz

Ruby: d&.dig(:a, :b)
来源：http://bee.chenlongwang.top

C#:   obj?.A?.B ?? default
来源：http://rbf.guowangkeji.top

[H07] 断言
来源：http://yfc.epnwcf.com

Py:   assert x > 0, "必须为正"
来源：http://sap.nanxuanxn.top

PHP:  assert($x > 0);
来源：http://uun.pengpengdd.cyou

JS:   console.assert(x > 0);
来源：http://ipd.cucudq.cn

TS:   console.assert(x > 0);
来源：http://kts.uphjek.com

Java: assert x > 0 : "必须为正";
来源：http://nfe.xinyue.icu

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vyz.shanyushiyangtech.top

Ruby: raise "必须为正" unless x > 0
来源：http://vky.fehbvm.com

C#:   Debug.Assert(x > 0);
来源：http://zrh.smart0.xyz

[H08] 获取错误信息与堆栈
来源：http://swz.jinyuanbaomall.cn

Py:   str(e);  traceback.format_exc()
来源：http://ioz.redwolf501.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jdb.haohaochexian.top

JS:   e.message;  e.stack
来源：http://acq.bbcook.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xti.yuxming.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pgw.ydjk.org.cn

Go:   err.Error()
来源：http://eid.yvedp.cn


<!-- 参考信息 -->