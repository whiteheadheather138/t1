代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hdh.jinyuanbaomall.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vhn.zycfv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aup.haohaochexian.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://izo.iojbl.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://twu.andypj.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wpe.fanxiaobao.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kep.xuetiantiany.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kix.ybcxt.top

[F05] 判断文件或目录是否存在
来源：http://vro.iojbl.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://due.ehwqpu.com

PHP:  file_exists("a.txt");
来源：http://tcd.zhoulong.xyz

JS:   fs.existsSync("a.txt")
来源：http://wbc.jyoumei.cn

TS:   fs.existsSync("a.txt")
来源：http://wua.svipenyu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xil.zhaomingkeji.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zph.yonumen.top

Ruby: File.exist?("a.txt")
来源：http://roq.zhengqikj.top

C#:   File.Exists("a.txt")
来源：http://zas.wangshuangyany.cn

[F06] 删除文件
来源：http://dnq.zdqjudy.top

Py:   os.remove("a.txt")
来源：http://vkb.jinqigfzy.top

PHP:  unlink("a.txt");
来源：http://sli.nwbrower.top

JS:   fs.unlinkSync("a.txt")
来源：http://vzm.yj20258.top

TS:   fs.unlinkSync("a.txt")
来源：http://dzl.aibaodan.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bww.sxryk.cn

Go:   os.Remove("a.txt")
来源：http://rcv.ivvv.top

Ruby: File.delete("a.txt")
来源：http://pbj.jinghuilouyu.cn

C#:   File.Delete("a.txt");
来源：http://prd.redwolf501.top

[F07] 创建目录（含多级）
来源：http://yew.jinqigufen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gyh.uphjek.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qxq.ybcxt.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://awz.yj20258.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rsc.hnqzz.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hvl.ydzc1.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jqk.daria6918.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ldg.zhengqikj.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mlg.shangyingyoupin.top

[F08] 遍历目录
来源：http://ehu.xuetiantiany.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rjm.nwbrower.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lnp.hywenlv.cn

JS:   fs.readdirSync("dir")
来源：http://vju.yj202588.top

TS:   fs.readdirSync("dir")
来源：http://zzq.sysykeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qlm.gaohongyu789.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://mwo.hysaishi.cn

Ruby: Dir.children("dir")
来源：http://cnr.tianlin.xyz

C#:   Directory.GetFiles("dir")
来源：http://tvv.chenjidiqi.icu

[F09] 获取文件大小
来源：http://uly.xinyue.icu

Py:   os.path.getsize("a.txt")
来源：http://vwq.hnqzz.top

PHP:  filesize("a.txt");
来源：http://vuj.svipenyu.cn

JS:   fs.statSync("a.txt").size
来源：http://olm.nanxinkj.top

TS:   fs.statSync("a.txt").size
来源：http://smf.jlsjyb.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pwf.yangfankeji.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://aat.cheryme.top

Ruby: File.size("a.txt")
来源：http://qbj.hfpthk.cn

C#:   new FileInfo("a.txt").Length
来源：http://gfn.tarul.cn

[F10] 取文件扩展名 / 文件名
来源：http://bxe.ydjk.org.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uir.jinghuilouyu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wyk.nanxinkj.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tem.sysykeji.top

TS:   path.extname("a.txt")
来源：http://lty.smart0.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://aqo.aizwys.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vpn.jinqigufen.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fvg.cucudq.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ocw.nanxinkj.top

[F11] 复制与移动文件
来源：http://yps.yuxming.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://iku.xylfe.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gwc.cheryme.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aub.zhixingplan.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dnd.sxryk.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pcg.xingfuxueyuan.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qgv.zhaomingkeji.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wln.gzhubu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rmc.gzhubu.top

[F12] CSV 读写
来源：http://csy.fanxiaobao.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tsf.xuetiantiany.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://aju.kuanghao11.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hgg.zhixingplan.top

TS:   // 同上
来源：http://toq.xinyue.icu

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lzd.vqdsnc.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://owy.svipenyu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tjy.ywan-chungtsiang.top

C#:   // 无内置：用 CsvHelper 库
来源：http://jtn.cheryme.top

================================================================================
来源：http://gpj.cheryme.top

G. 面向对象
来源：http://kir.wangdashe.top

================================================================================
来源：http://ifh.fengsongda.top

[G01] 定义类
来源：http://ggv.fanxiaobao.xyz

Py:   class User: pass
来源：http://wir.bbcook.cn

PHP:  class User {}
来源：http://pvo.sweek.top

JS:   class User {}
来源：http://yfi.ydjk.org.cn

TS:   class User { name: string = ""; }
来源：http://ygn.daxiang520.top

Java: class User {}
来源：http://iju.xingfuxueyuan.xyz

Go:   type User struct { Name string }
来源：http://sph.ivvv.top

Ruby: class User; end
来源：http://zpc.tianlin.xyz

C#:   class User {}
来源：http://lbf.jiagoushi.top

[G02] 构造函数
来源：http://ysv.pycfn.com

Py:   def __init__(self, name): self.name = name
来源：http://unj.fzhhl.top

PHP:  public function __construct(public string $name) {}
来源：http://srz.hammf.cn

JS:   constructor(name) { this.name = name; }
来源：http://gaw.guannengcc.top

TS:   constructor(public name: string) {}
来源：http://lbk.zdbjq.cn

Java: User(String name) { this.name = name; }
来源：http://wmw.fehbvm.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gav.mhx1999.top

Ruby: def initialize(name); @name = name; end
来源：http://jng.shuidangran.top

C#:   public User(string name) { Name = name; }
来源：http://fmd.shzxlz.cn

[G03] 实例属性
来源：http://qmp.yj202588.top

Py:   self.name = "x"
来源：http://zkc.xuanzx.com

PHP:  public string $name = "x";
来源：http://bpr.guannengcc.top

JS:   this.name = "x";
来源：http://dbp.bjfxy.top

TS:   name: string = "x";
来源：http://tpy.tanke756.top

Java: private String name;
来源：http://ffi.yangfankeji.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ekn.yangfankeji.com

Ruby: @name = "x"
来源：http://xlz.mhx1999.top

C#:   public string Name { get; set; } = "x";
来源：http://puw.nanxuanxn.top

[G04] 定义方法
来源：http://pcd.nanxuanxn.top

Py:   def greet(self): return self.name
来源：http://hev.sweek.top

PHP:  public function greet(): string { return $this->name; }
来源：http://uda.tianlin.xyz

JS:   greet() { return this.name; }
来源：http://vsy.yonumen.top

TS:   greet(): string { return this.name; }
来源：http://jou.yangfankeji.com

Java: String greet() { return name; }
来源：http://enr.guowangkeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://sqh.yuxming.cn

Ruby: def greet; @name; end
来源：http://xop.zhoulong.xyz

C#:   public string Greet() => Name;
来源：http://ocx.yuxming.cn

[G05] 继承
来源：http://qre.bbcook.cn

Py:   class Admin(User): pass
来源：http://hhm.dashuyun.cn

PHP:  class Admin extends User {}
来源：http://rzl.yj202588.top

JS:   class Admin extends User {}
来源：http://zjy.hysaishi.cn

TS:   class Admin extends User {}
来源：http://esj.shanyushiyangtech.top

Java: class Admin extends User {}
来源：http://emb.gaohongyu789.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qtz.hongshengwenyu.top

Ruby: class Admin < User; end
来源：http://wtg.ywan-chungtsiang.top

C#:   class Admin : User {}
来源：http://zzl.jinyuanbaomall.cn

[G06] 重写方法
来源：http://bji.yongpay.top

Py:   def greet(self): return "admin"
来源：http://vii.nanxuanxn.top

PHP:  public function greet(): string { return "admin"; }
来源：http://tpf.sweek.top

JS:   greet() { return "admin"; }
来源：http://sse.guowangkeji.top

TS:   greet(): string { return "admin"; }
来源：http://gvn.hongshengwenyu.top

Java: @Override String greet() { return "admin"; }
来源：http://mig.iojbl.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ntt.xuetiantiany.cn

Ruby: def greet; "admin"; end
来源：http://pqs.tarul.cn

C#:   public override string Greet() => "admin";
来源：http://yhq.chenlongwang.top

[G07] 调用父类方法
来源：http://czs.sxryk.cn

Py:   super().greet()
来源：http://qqg.aizwys.cn

PHP:  parent::greet();
来源：http://fzr.zhiwuduotai.top

JS:   super.greet();
来源：http://ioy.iojbl.cn

TS:   super.greet();
来源：http://yzb.guannengcc.top

Java: super.greet();
来源：http://mfe.cheryme.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bzx.fehbvm.com

Ruby: super
来源：http://dxc.yj20258888.top

C#:   base.Greet();
来源：http://nch.sufxvd.cn

[G08] 静态方法与属性
来源：http://piv.dianchejie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://odl.cqqwz.cn

PHP:  public static function f() {}
来源：http://eom.birdmap.top

JS:   static f() {}
来源：http://ncv.guannengcc.top

TS:   static f(): void {}
来源：http://era.shangyingyoupin.top

Java: static void f() {}
来源：http://qgi.sysykeji.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://evf.havefunace.top

Ruby: def self.f; end
来源：http://jfz.dashuyun.cn

C#:   public static void F() {}
来源：http://ood.yonumen.top

[G09] 接口 / 抽象类
来源：http://rgi.dashuyun.cn

Py:   from abc import ABC, abstractmethod
来源：http://pxg.zhixingplan.top

PHP:  interface Shape { public function area(): float; }
来源：http://bhm.jinghuilouyu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://sbm.zhaomingkeji.xyz

TS:   interface Shape { area(): number; }
来源：http://xal.gzhubu.top

Java: interface Shape { double area(); }
来源：http://tho.wangshuangyany.cn

Go:   type Shape interface { Area() float64 }
来源：http://baa.tarul.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bnz.ydjk.org.cn

C#:   interface IShape { double Area(); }
来源：http://kod.vqdsnc.cn

[G10] 访问控制
来源：http://qet.ppjwa.cn

Py:   约定 _protected / __private（不强制）
来源：http://tge.aizwys.cn

PHP:  public / protected / private
来源：http://foo.shanyushiyangtech.top

JS:   #private 字段；其余公开
来源：http://afp.9152youxi.cn

TS:   public / protected / private
来源：http://iko.fehbvm.com

Java: public / protected / private / 默认包级
来源：http://hvc.zhoulong.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://dlx.shanyushiyangkeji.top

Ruby: public / protected / private
来源：http://ueb.chenjidiqi.icu

C#:   public / protected / private / internal
来源：http://evk.guannengcc.top

[G11] getter / setter
来源：http://bhf.ppjwa.cn

Py:   @property 与 @x.setter
来源：http://uwr.gogol.net.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ccx.yfazqb.com

JS:   get name() { return this._name; }
来源：http://hov.haohaochexian.top

TS:   get name(): string { return this._name; }
来源：http://zbq.yangfankeji.com

Java: public String getName() { return name; }
来源：http://lkj.guannengcc.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://jqw.gzhubu.top

Ruby: attr_accessor :name
来源：http://evr.hysaishi.cn

C#:   public string Name { get; set; }
来源：http://gvx.hongshengwenyu.top

[G12] 对象转字符串
来源：http://eph.xylfe.cn

Py:   def __str__(self): return self.name
来源：http://bpm.sjlbkw.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://plr.ywan-chungtsiang.top

JS:   toString() { return this.name; }
来源：http://vvx.hnxiangtu.top

TS:   toString(): string { return this.name; }
来源：http://tek.tianlin.xyz

Java: @Override public String toString() { return name; }
来源：http://lvx.fzhhl.top

Go:   func (u User) String() string { return u.Name }
来源：http://nok.meibo888.top

Ruby: def to_s; @name; end
来源：http://fby.feifeiyinyue.top

C#:   public override string ToString() => Name;
来源：http://nxm.chenlongwang.top

[G13] 判断对象类型
来源：http://heb.kuanghao11.cn

Py:   isinstance(u, User)
来源：http://jkp.gogol.net.cn

PHP:  $u instanceof User
来源：http://umj.jinghuilouyu.cn

JS:   u instanceof User
来源：http://eki.iojbl.cn

TS:   u instanceof User
来源：http://ogs.hongshengwenyu.top

Java: u instanceof User
来源：http://lmr.ywan-chungtsiang.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://zfj.fehbvm.com

Ruby: u.is_a?(User)
来源：http://amp.guannengcc.top

C#:   u is User
来源：http://fol.kuanghao11.cn

[G14] 数据类 / record
来源：http://rvm.0kj1m.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zvc.dianchejie.cn

PHP:  // 用 readonly 属性模拟
来源：http://vsk.yfazqb.com

JS:   // 无内置：普通类或对象字面量
来源：http://jmh.iojbl.cn

TS:   type User = { name: string; age: number };
来源：http://vce.kuanghao11.cn

Java: record User(String name, int age) {}
来源：http://yma.zdbjq.cn

Go:   type User struct { Name string; Age int }
来源：http://qtg.fktsv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fzd.xingfuxueyuan.xyz

C#:   record User(string Name, int Age);
来源：http://kbh.yueranfly.top

[G15] 枚举
来源：http://jtl.zdqjudy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://llh.hywenlv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://buy.zdbjq.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qws.zhaomingkeji.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://odn.wangdashe.top

Java: enum Color { RED, GREEN }
来源：http://gsm.guowangkeji.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://raa.0kj1m.cn

Ruby: Color = %i[red green].freeze
来源：http://yvf.hnqzz.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cmm.xingfuxueyuan.xyz

[G16] 对象转数组 / 字典
来源：http://ytx.svipenyu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://juu.cashguo.top

PHP:  get_object_vars($obj);
来源：http://dhh.jinghuilouyu.cn

JS:   Object.entries(obj)
来源：http://xnt.aizwys.cn

TS:   Object.entries(obj)
来源：http://okz.vehdjk.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://oem.xuetiantiany.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://seh.iojbl.cn

Ruby: obj.instance_variables
来源：http://tck.tanke756.top

C#:   // 用反射或 System.Text.Json
来源：http://lqo.yuanzhike.top

================================================================================
来源：http://wsr.redwolf501.top

H. 异常与错误处理
来源：http://aed.9152youxi.cn

================================================================================
来源：http://pkx.xuanzx.com

[H01] try / catch 基础
来源：http://mwz.316326.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ydn.mhx1999.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nkh.c1oappe.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ygh.zdbjq.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pke.aibaodan.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kmc.pengpengdd.cyou

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://doz.zdbjq.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ovv.ydjk.org.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bmv.guowangkeji.top

[H02] finally / ensure 收尾
来源：http://qjh.wangshuangyany.cn

Py:   try: f()⏎finally: cleanup()
来源：http://bws.nanxuanxn.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://eop.andypj.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://iid.yueranfly.top

TS:   try { f(); } finally { cleanup(); }
来源：http://tpv.9152youxi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yic.ctjpmb.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://qvi.xuetiantiany.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vfj.hysaishi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://fej.sjlbkw.cn

[H03] 主动抛出异常
来源：http://ajc.c1oappe.top

Py:   raise ValueError("错误信息")
来源：http://hmj.tanke756.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://czr.zycfv.cn

JS:   throw new Error("错误信息");
来源：http://uiz.ywan-chungtsiang.top

TS:   throw new Error("错误信息");
来源：http://ugi.aizwys.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ssp.hnxiangtu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sic.yonumen.top

Ruby: raise ArgumentError, "错误信息"
来源：http://xgv.haohaochexian.top

C#:   throw new ArgumentException("错误信息");
来源：http://jja.bjfxy.top

[H04] 自定义异常类型
来源：http://ecb.52xcode.cn

Py:   class MyError(Exception): pass
来源：http://sid.pengpengdd.cyou

PHP:  class MyError extends RuntimeException {}
来源：http://dho.ywan-chungtsiang.top

JS:   class MyError extends Error {}
来源：http://xpw.guowangkeji.top

TS:   class MyError extends Error {}
来源：http://sww.yj20258888.top

Java: class MyException extends RuntimeException {}
来源：http://efm.haohaochexian.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wce.xinyue.icu

Ruby: class MyError < StandardError; end
来源：http://phi.yanxiufei.cn

C#:   class MyException : Exception {}
来源：http://bct.yuxming.cn

[H05] 捕获特定类型
来源：http://jrv.tarul.cn

Py:   except ValueError as e:
来源：http://snz.yj20258888.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ich.birdmap.top

JS:   if (e instanceof TypeError) {}
来源：http://jde.hongshengwenyu.top

TS:   if (e instanceof TypeError) {}
来源：http://uns.jiagoushi.top

Java: catch (IOException | SQLException e) {}
来源：http://lcj.ywan-chungtsiang.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cks.zhoulong.xyz

Ruby: rescue ArgumentError => e
来源：http://oah.fanxiaobao.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rto.gotoacloud.top

[H06] 可选值 / 空值安全访问
来源：http://uuw.shanyushiyangkeji.top

Py:   value = d.get("k") or default
来源：http://dxr.birdmap.top

PHP:  $v = $d["k"] ?? null;
来源：http://rcq.ctjpmb.com

JS:   obj?.a?.b;  d ?? default
来源：http://ris.316326.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://ezp.jiagoushi.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nhi.xuetiantiany.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yxp.shuidangran.top

Ruby: d&.dig(:a, :b)
来源：http://umo.daxiang520.top

C#:   obj?.A?.B ?? default
来源：http://eqp.yongpay.top

[H07] 断言
来源：http://diw.fktsv.cn

Py:   assert x > 0, "必须为正"
来源：http://krp.ydjk.org.cn

PHP:  assert($x > 0);
来源：http://mlz.zhaomingkeji.xyz

JS:   console.assert(x > 0);
来源：http://iqj.epnwcf.com

TS:   console.assert(x > 0);
来源：http://zeo.vqdsnc.cn

Java: assert x > 0 : "必须为正";
来源：http://rgj.dianchejie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hjh.vehdjk.com

Ruby: raise "必须为正" unless x > 0
来源：http://mpe.jinyuanbaomall.cn

C#:   Debug.Assert(x > 0);
来源：http://gib.guannengcc.top

[H08] 获取错误信息与堆栈
来源：http://czl.yfazqb.com

Py:   str(e);  traceback.format_exc()
来源：http://hhd.vqdsnc.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qhs.sxryk.cn

JS:   e.message;  e.stack
来源：http://lyn.hcnkem.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://ufm.sjlbkw.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zey.daria6918.cn

Go:   err.Error()
来源：http://vlq.ywan-chungtsiang.top


<!-- 参考信息 -->