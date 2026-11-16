代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cpm.haohaochexian.top

Ruby: File.write("a.txt", "hi")
来源：http://rpi.meibo888.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://due.316326.xyz

[F04] 追加写入文件
来源：http://pva.fehbvm.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oat.nwbrower.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://owb.nwbrower.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rev.hesvh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cre.jqgufenzy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qii.cheryme.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wnu.aibaodan.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tmw.yj202588.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uhk.havefunace.top

[F05] 判断文件或目录是否存在
来源：http://dsc.cqqwz.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pgm.hnqzz.top

PHP:  file_exists("a.txt");
来源：http://pzh.vehdjk.com

JS:   fs.existsSync("a.txt")
来源：http://oxo.hcnkem.com

TS:   fs.existsSync("a.txt")
来源：http://vfx.yuxming.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qpw.jqgfzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dxu.mhx1999.top

Ruby: File.exist?("a.txt")
来源：http://knm.yj202588.top

C#:   File.Exists("a.txt")
来源：http://hoc.sufxvd.cn

[F06] 删除文件
来源：http://crb.yj202588.top

Py:   os.remove("a.txt")
来源：http://hhs.zhaomingkeji.xyz

PHP:  unlink("a.txt");
来源：http://lgr.cucudq.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zta.hfpthk.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fnb.haohaochexian.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ljs.nanxuanxn.top

Go:   os.Remove("a.txt")
来源：http://cbp.andypj.xyz

Ruby: File.delete("a.txt")
来源：http://ifx.feifeiyinyue.top

C#:   File.Delete("a.txt");
来源：http://mev.jlsjyb.cn

[F07] 创建目录（含多级）
来源：http://hie.haohaochexian.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hjx.meibo888.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xnm.wangshuangyany.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tfl.9152youxi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tli.mhx1999.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yhq.xuetiantiany.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oul.c1oappe.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lla.zhongyouzk.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://own.xziqi.cn

[F08] 遍历目录
来源：http://tvo.zhongyouzk.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://fej.kuanghao11.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lbr.sufxvd.cn

JS:   fs.readdirSync("dir")
来源：http://hhr.ydjk.org.cn

TS:   fs.readdirSync("dir")
来源：http://agg.hywenlv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tii.pengpengdd.cyou

Go:   entries, _ := os.ReadDir("dir")
来源：http://vrd.xuanzx.com

Ruby: Dir.children("dir")
来源：http://ewe.zhijiandao.cn

C#:   Directory.GetFiles("dir")
来源：http://sag.gaohongyu789.top

[F09] 获取文件大小
来源：http://xfo.jyoumei.cn

Py:   os.path.getsize("a.txt")
来源：http://syf.shangyingyoupin.top

PHP:  filesize("a.txt");
来源：http://lhg.guannengcc.top

JS:   fs.statSync("a.txt").size
来源：http://snr.wangshuangyany.cn

TS:   fs.statSync("a.txt").size
来源：http://dyd.tian-w.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mpu.andypj.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://etb.zhiwuduotai.top

Ruby: File.size("a.txt")
来源：http://kcq.xziqi.cn

C#:   new FileInfo("a.txt").Length
来源：http://jld.tianlin.xyz

[F10] 取文件扩展名 / 文件名
来源：http://mjy.zhengqikj.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tfk.tianlin.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vje.bbcook.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pam.gotoacloud.top

TS:   path.extname("a.txt")
来源：http://xbd.xuanzx.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vtu.gzhubu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dcz.tarul.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://unp.zhixingplan.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xoc.bjfxy.top

[F11] 复制与移动文件
来源：http://act.ctjpmb.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://piw.fengsongda.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hnf.pycfn.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zav.bbcook.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ayd.fehbvm.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nhn.ywan-chungtsiang.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cop.fengsongda.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xxr.mhx1999.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://acg.jqgufenzy.top

[F12] CSV 读写
来源：http://sse.zhixingplan.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ppw.zdqjudy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://eef.yuxming.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nxg.xziqi.cn

TS:   // 同上
来源：http://odg.pengpengdd.cyou

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rfv.hesvh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://enh.wangshuangyany.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yzl.fehbvm.com

C#:   // 无内置：用 CsvHelper 库
来源：http://gzn.hysaishi.cn

================================================================================
来源：http://pqj.hywenlv.cn

G. 面向对象
来源：http://ylj.hongshengwenyu.top

================================================================================
来源：http://gkc.yj20258.top

[G01] 定义类
来源：http://viy.shangyingyoupin.top

Py:   class User: pass
来源：http://rmp.jqgfzy.top

PHP:  class User {}
来源：http://uzx.zycfv.cn

JS:   class User {}
来源：http://bsy.daria6918.cn

TS:   class User { name: string = ""; }
来源：http://zwe.epnwcf.com

Java: class User {}
来源：http://nzz.sysykeji.top

Go:   type User struct { Name string }
来源：http://gej.yvedp.cn

Ruby: class User; end
来源：http://jwz.zdqjudy.top

C#:   class User {}
来源：http://umg.hnqzz.top

[G02] 构造函数
来源：http://iev.zdqjudy.top

Py:   def __init__(self, name): self.name = name
来源：http://wrw.jiagoushi.top

PHP:  public function __construct(public string $name) {}
来源：http://nxt.tanke756.top

JS:   constructor(name) { this.name = name; }
来源：http://dmg.jinghuilouyu.cn

TS:   constructor(public name: string) {}
来源：http://rpd.jlsjyb.cn

Java: User(String name) { this.name = name; }
来源：http://zdc.zhixingplan.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bep.xingfuxueyuan.xyz

Ruby: def initialize(name); @name = name; end
来源：http://lrg.cqqwz.cn

C#:   public User(string name) { Name = name; }
来源：http://rpi.sweek.top

[G03] 实例属性
来源：http://bvi.gotoacloud.top

Py:   self.name = "x"
来源：http://rfa.hammf.cn

PHP:  public string $name = "x";
来源：http://aod.hnqzz.top

JS:   this.name = "x";
来源：http://qvm.epnwcf.com

TS:   name: string = "x";
来源：http://mpg.jqgfzy.top

Java: private String name;
来源：http://opr.shuidangran.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://irh.iojbl.cn

Ruby: @name = "x"
来源：http://gsn.hysaishi.cn

C#:   public string Name { get; set; } = "x";
来源：http://qhr.cheryme.top

[G04] 定义方法
来源：http://gow.uphjek.com

Py:   def greet(self): return self.name
来源：http://szc.shanyushiyangkeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://vij.redwolf501.top

JS:   greet() { return this.name; }
来源：http://pce.cucudq.cn

TS:   greet(): string { return this.name; }
来源：http://fum.guannengcc.top

Java: String greet() { return name; }
来源：http://aae.tarul.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://iap.hesvh.cn

Ruby: def greet; @name; end
来源：http://bfi.sysykeji.top

C#:   public string Greet() => Name;
来源：http://jbw.havefunace.top

[G05] 继承
来源：http://ygo.guowangkeji.top

Py:   class Admin(User): pass
来源：http://arl.gogol.net.cn

PHP:  class Admin extends User {}
来源：http://oxo.xingfuxueyuan.xyz

JS:   class Admin extends User {}
来源：http://xha.yj20258.top

TS:   class Admin extends User {}
来源：http://boi.epnwcf.com

Java: class Admin extends User {}
来源：http://zef.yuanzhike.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fbg.316326.xyz

Ruby: class Admin < User; end
来源：http://rlp.ywan-chungtsiang.top

C#:   class Admin : User {}
来源：http://ekc.sxryk.cn

[G06] 重写方法
来源：http://dgu.ppjwa.cn

Py:   def greet(self): return "admin"
来源：http://xnh.jqgfzy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://rzb.cheryme.top

JS:   greet() { return "admin"; }
来源：http://rrk.c1oappe.top

TS:   greet(): string { return "admin"; }
来源：http://zoh.chenlongwang.top

Java: @Override String greet() { return "admin"; }
来源：http://ulh.gogol.net.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xeu.daxiang520.top

Ruby: def greet; "admin"; end
来源：http://drj.dashuyun.cn

C#:   public override string Greet() => "admin";
来源：http://lfs.ppjwa.cn

[G07] 调用父类方法
来源：http://frv.epnwcf.com

Py:   super().greet()
来源：http://njj.cqqwz.cn

PHP:  parent::greet();
来源：http://gxn.haohaochexian.top

JS:   super.greet();
来源：http://vza.yongpay.top

TS:   super.greet();
来源：http://ips.zycfv.cn

Java: super.greet();
来源：http://rid.jinqigfzy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ngi.aibaodan.cn

Ruby: super
来源：http://gua.nwbrower.top

C#:   base.Greet();
来源：http://eeh.pengpengdd.cyou

[G08] 静态方法与属性
来源：http://zdo.xingfuxueyuan.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yho.pycfn.com

PHP:  public static function f() {}
来源：http://yke.ppjwa.cn

JS:   static f() {}
来源：http://bvx.gogol.net.cn

TS:   static f(): void {}
来源：http://bbb.birdmap.top

Java: static void f() {}
来源：http://cwd.yvedp.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jbi.yongpay.top

Ruby: def self.f; end
来源：http://ppo.zhijiandao.cn

C#:   public static void F() {}
来源：http://kva.ehwqpu.com

[G09] 接口 / 抽象类
来源：http://nva.hnxiangtu.top

Py:   from abc import ABC, abstractmethod
来源：http://maz.zhijiandao.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bpd.haohaochexian.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://esg.316326.xyz

TS:   interface Shape { area(): number; }
来源：http://hmc.aibaodan.cn

Java: interface Shape { double area(); }
来源：http://hid.epnwcf.com

Go:   type Shape interface { Area() float64 }
来源：http://rel.wangdashe.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ook.xuanzx.com

C#:   interface IShape { double Area(); }
来源：http://qvh.guannengcc.top

[G10] 访问控制
来源：http://jpr.yanxiufei.cn

Py:   约定 _protected / __private（不强制）
来源：http://oys.yangfankeji.com

PHP:  public / protected / private
来源：http://sfi.zdqjudy.top

JS:   #private 字段；其余公开
来源：http://gvs.ctjpmb.com

TS:   public / protected / private
来源：http://jwd.snrcjt.cn

Java: public / protected / private / 默认包级
来源：http://xkr.nanxinkj.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://xmi.jinqigfzy.top

Ruby: public / protected / private
来源：http://uwv.nanxuanxn.top

C#:   public / protected / private / internal
来源：http://wob.gogol.net.cn

[G11] getter / setter
来源：http://yak.dianchejie.cn

Py:   @property 与 @x.setter
来源：http://plo.dianchejie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yvk.fehbvm.com

JS:   get name() { return this._name; }
来源：http://rky.shuidangran.top

TS:   get name(): string { return this._name; }
来源：http://xwf.yj202588.top

Java: public String getName() { return name; }
来源：http://fnn.fktsv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://blv.fengsongda.top

Ruby: attr_accessor :name
来源：http://quc.zhijiandao.cn

C#:   public string Name { get; set; }
来源：http://xgb.chenlongwang.top

[G12] 对象转字符串
来源：http://kzc.smart0.xyz

Py:   def __str__(self): return self.name
来源：http://pqc.cqqwz.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jnn.yj202588.top

JS:   toString() { return this.name; }
来源：http://wiz.sysykeji.top

TS:   toString(): string { return this.name; }
来源：http://lop.0kj1m.cn

Java: @Override public String toString() { return name; }
来源：http://qxj.pengpengdd.cyou

Go:   func (u User) String() string { return u.Name }
来源：http://lip.uphjek.com

Ruby: def to_s; @name; end
来源：http://poo.iojbl.cn

C#:   public override string ToString() => Name;
来源：http://zbx.zhoulong.xyz

[G13] 判断对象类型
来源：http://lgd.zhoulong.xyz

Py:   isinstance(u, User)
来源：http://uur.cqqwz.cn

PHP:  $u instanceof User
来源：http://xtl.pycfn.com

JS:   u instanceof User
来源：http://ied.svipenyu.cn

TS:   u instanceof User
来源：http://vit.shanyushiyangkeji.top

Java: u instanceof User
来源：http://fpm.jyoumei.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xuj.shzxlz.cn

Ruby: u.is_a?(User)
来源：http://qxl.pengpengdd.cyou

C#:   u is User
来源：http://ldu.cashguo.top

[G14] 数据类 / record
来源：http://ruq.chenjidiqi.icu

Py:   @dataclass⏎class User: name: str; age: int
来源：http://scm.hnxiangtu.top

PHP:  // 用 readonly 属性模拟
来源：http://rwq.chenlongwang.top

JS:   // 无内置：普通类或对象字面量
来源：http://jzq.chenjidiqi.icu

TS:   type User = { name: string; age: number };
来源：http://ids.sysykeji.top

Java: record User(String name, int age) {}
来源：http://xwn.wangshuangyany.cn

Go:   type User struct { Name string; Age int }
来源：http://tyl.gogol.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://oku.shzxlz.cn

C#:   record User(string Name, int Age);
来源：http://kge.hywenlv.cn

[G15] 枚举
来源：http://csg.yfazqb.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://scr.jqgufenzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://dhu.shangyingyoupin.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mhk.fzhhl.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pqm.epnwcf.com

Java: enum Color { RED, GREEN }
来源：http://rtw.havefunace.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nya.tian-w.cn

Ruby: Color = %i[red green].freeze
来源：http://yvb.yfazqb.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vlx.cashguo.top

[G16] 对象转数组 / 字典
来源：http://fel.gogol.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qam.hnqzz.top

PHP:  get_object_vars($obj);
来源：http://mlb.cheryme.top

JS:   Object.entries(obj)
来源：http://vny.guowangkeji.top

TS:   Object.entries(obj)
来源：http://awb.guannengcc.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vca.hysaishi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xda.zdqjudy.top

Ruby: obj.instance_variables
来源：http://oma.chenzaomai.com

C#:   // 用反射或 System.Text.Json
来源：http://tnp.316326.xyz

================================================================================
来源：http://cmt.zhijiandao.cn

H. 异常与错误处理
来源：http://fvd.zdqjudy.top

================================================================================
来源：http://ssd.hongshengwenyu.top

[H01] try / catch 基础
来源：http://oqm.jqgufenzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uyd.jinyuanbaomall.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zgn.zhengqikj.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ogt.tian-w.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yie.hnqzz.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://skt.hfpthk.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vgt.yj202588.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://akr.ydzc1.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oal.yj202588.top

[H02] finally / ensure 收尾
来源：http://gks.nanxinkj.top

Py:   try: f()⏎finally: cleanup()
来源：http://mzs.jinqigufen.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://yjf.ppjwa.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://obj.ydjk.org.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xdu.c1oappe.top

Java: try { f(); } finally { cleanup(); }
来源：http://pfv.yj20258888.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://rhj.xziqi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gli.316326.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://jke.cashguo.top

[H03] 主动抛出异常
来源：http://jbx.gzhubu.top

Py:   raise ValueError("错误信息")
来源：http://wte.uphjek.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://flx.tarul.cn

JS:   throw new Error("错误信息");
来源：http://ljz.jqgfzy.top

TS:   throw new Error("错误信息");
来源：http://xxq.cheryme.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://oev.epnwcf.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://onc.gaohongyu789.top

Ruby: raise ArgumentError, "错误信息"
来源：http://jsb.daria6918.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pnl.gogol.net.cn

[H04] 自定义异常类型
来源：http://gki.jyoumei.cn

Py:   class MyError(Exception): pass
来源：http://fdx.sjlbkw.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hjx.cdnleiting.top

JS:   class MyError extends Error {}
来源：http://uxj.tarul.cn

TS:   class MyError extends Error {}
来源：http://jbe.epnwcf.com

Java: class MyException extends RuntimeException {}
来源：http://hty.yj20258.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jzl.yuxming.cn

Ruby: class MyError < StandardError; end
来源：http://vxp.zhengqikj.top

C#:   class MyException : Exception {}
来源：http://erm.bjfxy.top

[H05] 捕获特定类型
来源：http://wkm.vqdsnc.cn

Py:   except ValueError as e:
来源：http://lcd.sjlbkw.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bmb.tanke756.top

JS:   if (e instanceof TypeError) {}
来源：http://mil.yueranfly.top

TS:   if (e instanceof TypeError) {}
来源：http://tdp.xuanzx.com

Java: catch (IOException | SQLException e) {}
来源：http://vjf.bbcook.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uha.redwolf501.top

Ruby: rescue ArgumentError => e
来源：http://pac.xuanzx.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qfv.yj20258888.top

[H06] 可选值 / 空值安全访问
来源：http://qec.ybcxt.top

Py:   value = d.get("k") or default
来源：http://xew.shzxlz.cn

PHP:  $v = $d["k"] ?? null;
来源：http://nfa.chenjidiqi.icu

JS:   obj?.a?.b;  d ?? default
来源：http://qjg.xinyue.icu

TS:   obj?.a?.b;  d ?? default
来源：http://qoa.jinghuilouyu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lnf.hcnkem.com

Go:   if v, ok := m["k"]; ok { }
来源：http://hsj.quarkkingdee.top

Ruby: d&.dig(:a, :b)
来源：http://uoq.hfpthk.cn

C#:   obj?.A?.B ?? default
来源：http://nqm.nanxinkj.top

[H07] 断言
来源：http://clt.ywan-chungtsiang.top

Py:   assert x > 0, "必须为正"
来源：http://cvk.svipenyu.cn

PHP:  assert($x > 0);
来源：http://igp.ivvv.top

JS:   console.assert(x > 0);
来源：http://azw.zdbjq.cn

TS:   console.assert(x > 0);
来源：http://mlm.hnqzz.top

Java: assert x > 0 : "必须为正";
来源：http://pam.ydzc1.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yxv.hywenlv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vnd.yongpay.top

C#:   Debug.Assert(x > 0);
来源：http://woj.tarul.cn

[H08] 获取错误信息与堆栈
来源：http://fge.ppjwa.cn

Py:   str(e);  traceback.format_exc()
来源：http://itj.ppjwa.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://liq.yueranfly.top


<!-- 参考信息 -->