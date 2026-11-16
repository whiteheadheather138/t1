代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fub.sufxvd.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vbr.nwbrower.top

[F03] 写入文件（覆盖）
来源：http://hmn.fanxiaobao.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jfg.redwolf501.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://pme.mhx1999.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qoq.jqgfzy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ken.iojbl.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ibl.cdnleiting.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jbf.cdnleiting.top

Ruby: File.write("a.txt", "hi")
来源：http://ufd.ybcxt.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wfb.zhoulong.xyz

[F04] 追加写入文件
来源：http://pfa.fanxiaobao.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fio.gogol.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wzy.zhongyouzk.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mcn.zdqjudy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bje.dashuyun.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lfh.hywenlv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rbg.xuetiantiany.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gli.havefunace.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://guh.tanke756.top

[F05] 判断文件或目录是否存在
来源：http://aor.shangyingyoupin.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fds.zhaomingkeji.xyz

PHP:  file_exists("a.txt");
来源：http://aoy.bjfxy.top

JS:   fs.existsSync("a.txt")
来源：http://fiv.jqgfzy.top

TS:   fs.existsSync("a.txt")
来源：http://xzv.bjfxy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://vma.xinyue.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qgl.xuanzx.com

Ruby: File.exist?("a.txt")
来源：http://qwx.uphjek.com

C#:   File.Exists("a.txt")
来源：http://wel.fzhhl.top

[F06] 删除文件
来源：http://zss.meibo888.top

Py:   os.remove("a.txt")
来源：http://czg.daxiang520.top

PHP:  unlink("a.txt");
来源：http://neu.xingfuxueyuan.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://xsm.gzhubu.top

TS:   fs.unlinkSync("a.txt")
来源：http://blv.sweek.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vib.xuetiantiany.cn

Go:   os.Remove("a.txt")
来源：http://vmy.xuetiantiany.cn

Ruby: File.delete("a.txt")
来源：http://wfw.xylfe.cn

C#:   File.Delete("a.txt");
来源：http://wlo.iojbl.cn

[F07] 创建目录（含多级）
来源：http://wwb.zdbjq.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fnf.yonumen.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lku.shangyingyoupin.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sgm.gzhubu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://awy.havefunace.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zbv.meibo888.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yoh.cashguo.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bgp.shuidangran.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xkh.c1oappe.top

[F08] 遍历目录
来源：http://okt.yuxming.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://dpd.zhengqikj.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bci.zhiwuduotai.top

JS:   fs.readdirSync("dir")
来源：http://zwv.jlsjyb.cn

TS:   fs.readdirSync("dir")
来源：http://yjv.zhongyouzk.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yjb.meibo888.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://yoo.52xcode.cn

Ruby: Dir.children("dir")
来源：http://nae.yj20258888.top

C#:   Directory.GetFiles("dir")
来源：http://flo.jinqigufen.top

[F09] 获取文件大小
来源：http://gst.guannengcc.top

Py:   os.path.getsize("a.txt")
来源：http://ick.ehwqpu.com

PHP:  filesize("a.txt");
来源：http://mwr.guannengcc.top

JS:   fs.statSync("a.txt").size
来源：http://ypy.tarul.cn

TS:   fs.statSync("a.txt").size
来源：http://zbh.cucudq.cn

Java: Files.size(Path.of("a.txt"))
来源：http://chu.nanxuanxn.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://boz.yj20258.top

Ruby: File.size("a.txt")
来源：http://rdj.aizwys.cn

C#:   new FileInfo("a.txt").Length
来源：http://abk.jqgfzy.top

[F10] 取文件扩展名 / 文件名
来源：http://ist.cqqwz.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rny.aibaodan.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qhl.jqgufenzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tib.jinqigfzy.top

TS:   path.extname("a.txt")
来源：http://onh.hesvh.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://eag.jinyuanbaomall.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kto.ywan-chungtsiang.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://eju.hcnkem.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fwl.zhiwuduotai.top

[F11] 复制与移动文件
来源：http://ohz.gzhubu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yvx.jinqigufen.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://olt.meibo888.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xtx.vqdsnc.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://poi.svipenyu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://spc.zdbjq.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://oem.xuetiantiany.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://shk.jinghuilouyu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ttq.yj20258888.top

[F12] CSV 读写
来源：http://qja.gzhubu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nfn.haohaochexian.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nej.aizwys.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rxg.cucudq.cn

TS:   // 同上
来源：http://bdw.aibaodan.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vnh.gogol.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dlb.andypj.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ntj.cdnleiting.top

C#:   // 无内置：用 CsvHelper 库
来源：http://cdo.tanke756.top

================================================================================
来源：http://fad.sxryk.cn

G. 面向对象
来源：http://paj.guowangkeji.top

================================================================================
来源：http://hnx.hcnkem.com

[G01] 定义类
来源：http://zyh.shanyushiyangtech.top

Py:   class User: pass
来源：http://cit.andypj.xyz

PHP:  class User {}
来源：http://tvs.hammf.cn

JS:   class User {}
来源：http://pgw.cqqwz.cn

TS:   class User { name: string = ""; }
来源：http://etu.andypj.xyz

Java: class User {}
来源：http://zne.haohaochexian.top

Go:   type User struct { Name string }
来源：http://uqm.shuidangran.top

Ruby: class User; end
来源：http://nbq.jiagoushi.top

C#:   class User {}
来源：http://tka.yj202588.top

[G02] 构造函数
来源：http://apj.fzhhl.top

Py:   def __init__(self, name): self.name = name
来源：http://jdk.xziqi.cn

PHP:  public function __construct(public string $name) {}
来源：http://tek.ydzc1.top

JS:   constructor(name) { this.name = name; }
来源：http://liu.haohaochexian.top

TS:   constructor(public name: string) {}
来源：http://bxo.sysykeji.top

Java: User(String name) { this.name = name; }
来源：http://gol.yangfankeji.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qym.shanyushiyangtech.top

Ruby: def initialize(name); @name = name; end
来源：http://vvy.cucudq.cn

C#:   public User(string name) { Name = name; }
来源：http://nsj.zhengqikj.top

[G03] 实例属性
来源：http://kod.sweek.top

Py:   self.name = "x"
来源：http://fqr.haohaochexian.top

PHP:  public string $name = "x";
来源：http://xbf.svipenyu.cn

JS:   this.name = "x";
来源：http://kpo.zhixingplan.top

TS:   name: string = "x";
来源：http://nxd.sjlbkw.cn

Java: private String name;
来源：http://aij.zhiwuduotai.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wnf.wangshuangyany.cn

Ruby: @name = "x"
来源：http://kuk.birdmap.top

C#:   public string Name { get; set; } = "x";
来源：http://ghf.jiagoushi.top

[G04] 定义方法
来源：http://xff.fengsongda.top

Py:   def greet(self): return self.name
来源：http://vsn.chenlongwang.top

PHP:  public function greet(): string { return $this->name; }
来源：http://lpb.wangshuangyany.cn

JS:   greet() { return this.name; }
来源：http://shd.mhx1999.top

TS:   greet(): string { return this.name; }
来源：http://mvu.yuxming.cn

Java: String greet() { return name; }
来源：http://yvr.redwolf501.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ery.jianghu66.top

Ruby: def greet; @name; end
来源：http://kwh.sweek.top

C#:   public string Greet() => Name;
来源：http://bxu.tarul.cn

[G05] 继承
来源：http://dzm.yueranfly.top

Py:   class Admin(User): pass
来源：http://lfv.yonumen.top

PHP:  class Admin extends User {}
来源：http://szc.pycfn.com

JS:   class Admin extends User {}
来源：http://xnn.cashguo.top

TS:   class Admin extends User {}
来源：http://sbf.yj202588.top

Java: class Admin extends User {}
来源：http://yru.shuidangran.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gpx.bjfxy.top

Ruby: class Admin < User; end
来源：http://gcz.zhixingplan.top

C#:   class Admin : User {}
来源：http://xfp.xziqi.cn

[G06] 重写方法
来源：http://wjw.zhixingplan.top

Py:   def greet(self): return "admin"
来源：http://vmu.yangfankeji.com

PHP:  public function greet(): string { return "admin"; }
来源：http://rls.meibo888.top

JS:   greet() { return "admin"; }
来源：http://czf.ehwqpu.com

TS:   greet(): string { return "admin"; }
来源：http://cje.zhengqikj.top

Java: @Override String greet() { return "admin"; }
来源：http://fgc.sysykeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yla.fengsongda.top

Ruby: def greet; "admin"; end
来源：http://qmf.xziqi.cn

C#:   public override string Greet() => "admin";
来源：http://dri.hesvh.cn

[G07] 调用父类方法
来源：http://gox.cqqwz.cn

Py:   super().greet()
来源：http://yhj.dianchejie.cn

PHP:  parent::greet();
来源：http://rpc.xingfuxueyuan.xyz

JS:   super.greet();
来源：http://uya.quarkkingdee.top

TS:   super.greet();
来源：http://uyr.tarul.cn

Java: super.greet();
来源：http://xel.fehbvm.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yfu.gotoacloud.top

Ruby: super
来源：http://bmt.havefunace.top

C#:   base.Greet();
来源：http://orc.guowangkeji.top

[G08] 静态方法与属性
来源：http://nip.wangdashe.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ykq.shanyushiyangkeji.top

PHP:  public static function f() {}
来源：http://tdb.zhaomingkeji.xyz

JS:   static f() {}
来源：http://pws.hywenlv.cn

TS:   static f(): void {}
来源：http://yum.daxiang520.top

Java: static void f() {}
来源：http://mgj.xziqi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://cce.aibaodan.cn

Ruby: def self.f; end
来源：http://phl.ywan-chungtsiang.top

C#:   public static void F() {}
来源：http://sac.fzhhl.top

[G09] 接口 / 抽象类
来源：http://lsq.sysykeji.top

Py:   from abc import ABC, abstractmethod
来源：http://cof.yj20258888.top

PHP:  interface Shape { public function area(): float; }
来源：http://qdy.hammf.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://sha.haohaochexian.top

TS:   interface Shape { area(): number; }
来源：http://oqn.hesvh.cn

Java: interface Shape { double area(); }
来源：http://uze.hesvh.cn

Go:   type Shape interface { Area() float64 }
来源：http://uaq.shangyingyoupin.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cgv.zycfv.cn

C#:   interface IShape { double Area(); }
来源：http://imu.hfpthk.cn

[G10] 访问控制
来源：http://lmw.nanxinkj.top

Py:   约定 _protected / __private（不强制）
来源：http://hfk.kuanghao11.cn

PHP:  public / protected / private
来源：http://evf.ctjpmb.com

JS:   #private 字段；其余公开
来源：http://ine.tarul.cn

TS:   public / protected / private
来源：http://mxs.cdnleiting.top

Java: public / protected / private / 默认包级
来源：http://xqz.aizwys.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://erh.316326.xyz

Ruby: public / protected / private
来源：http://zoh.tanke756.top

C#:   public / protected / private / internal
来源：http://rqv.316326.xyz

[G11] getter / setter
来源：http://avv.jiagoushi.top

Py:   @property 与 @x.setter
来源：http://clk.daxiang520.top

PHP:  public function getName(): string { return $this->name; }
来源：http://xvt.ydjk.org.cn

JS:   get name() { return this._name; }
来源：http://ltq.shuidangran.top

TS:   get name(): string { return this._name; }
来源：http://ftg.ydjk.org.cn

Java: public String getName() { return name; }
来源：http://uhx.9152youxi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mhg.fehbvm.com

Ruby: attr_accessor :name
来源：http://ktd.cdnleiting.top

C#:   public string Name { get; set; }
来源：http://xnm.yongpay.top

[G12] 对象转字符串
来源：http://rcf.meibo888.top

Py:   def __str__(self): return self.name
来源：http://kay.fktsv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lea.kuanghao11.cn

JS:   toString() { return this.name; }
来源：http://ath.hongshengwenyu.top

TS:   toString(): string { return this.name; }
来源：http://ops.haohaochexian.top

Java: @Override public String toString() { return name; }
来源：http://bfb.gaohongyu789.top

Go:   func (u User) String() string { return u.Name }
来源：http://vou.9152youxi.cn

Ruby: def to_s; @name; end
来源：http://kvf.yj20258.top

C#:   public override string ToString() => Name;
来源：http://tny.fzhhl.top

[G13] 判断对象类型
来源：http://xab.cheryme.top

Py:   isinstance(u, User)
来源：http://mem.aizwys.cn

PHP:  $u instanceof User
来源：http://hgg.cdnleiting.top

JS:   u instanceof User
来源：http://kge.fktsv.cn

TS:   u instanceof User
来源：http://qqs.fktsv.cn

Java: u instanceof User
来源：http://vhw.yueranfly.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://iew.cheryme.top

Ruby: u.is_a?(User)
来源：http://lmg.yangfankeji.com

C#:   u is User
来源：http://nsx.zycfv.cn

[G14] 数据类 / record
来源：http://din.xinyue.icu

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mfm.cashguo.top

PHP:  // 用 readonly 属性模拟
来源：http://hqu.dashuyun.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rnv.yj20258888.top

TS:   type User = { name: string; age: number };
来源：http://yuy.iojbl.cn

Java: record User(String name, int age) {}
来源：http://wud.hcnkem.com

Go:   type User struct { Name string; Age int }
来源：http://crl.ctjpmb.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rgo.52xcode.cn

C#:   record User(string Name, int Age);
来源：http://dhy.cucudq.cn

[G15] 枚举
来源：http://jtz.shzxlz.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bws.sufxvd.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://kij.ivvv.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yuc.uphjek.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qbd.zhoulong.xyz

Java: enum Color { RED, GREEN }
来源：http://mzy.tianlin.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uvn.sjlbkw.cn

Ruby: Color = %i[red green].freeze
来源：http://rjl.uphjek.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://obe.bjfxy.top

[G16] 对象转数组 / 字典
来源：http://tov.shuidangran.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wqv.jqgfzy.top

PHP:  get_object_vars($obj);
来源：http://mxn.sweek.top

JS:   Object.entries(obj)
来源：http://uzo.cashguo.top

TS:   Object.entries(obj)
来源：http://bqa.dashuyun.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lwq.fzhhl.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://mca.xinyue.icu

Ruby: obj.instance_variables
来源：http://ija.tianlin.xyz

C#:   // 用反射或 System.Text.Json
来源：http://grx.wangshuangyany.cn

================================================================================
来源：http://ykg.hysaishi.cn

H. 异常与错误处理
来源：http://rtc.bjfxy.top

================================================================================
来源：http://pxy.fktsv.cn

[H01] try / catch 基础
来源：http://yas.shangyingyoupin.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nzt.birdmap.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pvb.9152youxi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pie.jiagoushi.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://btw.jinyuanbaomall.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://eof.feifeiyinyue.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vjd.xziqi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kzn.xuetiantiany.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ksy.cdnleiting.top

[H02] finally / ensure 收尾
来源：http://gup.epnwcf.com

Py:   try: f()⏎finally: cleanup()
来源：http://akq.fehbvm.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://azp.yuxming.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qka.nanxinkj.top

TS:   try { f(); } finally { cleanup(); }
来源：http://rjg.jqgufenzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://pow.hesvh.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://clp.fktsv.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ypv.jiagoushi.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://fmi.c1oappe.top

[H03] 主动抛出异常
来源：http://nri.0kj1m.cn

Py:   raise ValueError("错误信息")
来源：http://qxk.hesvh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jwo.cqqwz.cn

JS:   throw new Error("错误信息");
来源：http://zjk.hnxiangtu.top

TS:   throw new Error("错误信息");
来源：http://sgq.yvedp.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jhc.shangyingyoupin.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bvh.xuanzx.com

Ruby: raise ArgumentError, "错误信息"
来源：http://ebk.wangshuangyany.cn

C#:   throw new ArgumentException("错误信息");
来源：http://cvn.hesvh.cn

[H04] 自定义异常类型
来源：http://xra.gzhubu.top

Py:   class MyError(Exception): pass
来源：http://eje.yvedp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fzj.fzhhl.top

JS:   class MyError extends Error {}
来源：http://cdr.hammf.cn

TS:   class MyError extends Error {}
来源：http://hgx.tianlin.xyz

Java: class MyException extends RuntimeException {}
来源：http://qfl.aibaodan.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cbf.chenjidiqi.icu

Ruby: class MyError < StandardError; end
来源：http://oby.zycfv.cn

C#:   class MyException : Exception {}
来源：http://xdv.zhoulong.xyz

[H05] 捕获特定类型
来源：http://sjj.shangyingyoupin.top

Py:   except ValueError as e:
来源：http://vdz.zhaomingkeji.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kps.316326.xyz

JS:   if (e instanceof TypeError) {}
来源：http://ywk.tanke756.top

TS:   if (e instanceof TypeError) {}
来源：http://mwm.epnwcf.com

Java: catch (IOException | SQLException e) {}
来源：http://qog.dianchejie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jut.yongpay.top

Ruby: rescue ArgumentError => e
来源：http://epo.feifeiyinyue.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ufl.yj20258.top

[H06] 可选值 / 空值安全访问
来源：http://cgs.jinghuilouyu.cn

Py:   value = d.get("k") or default
来源：http://rsh.andypj.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://nvs.bbcook.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mkw.jqgfzy.top

TS:   obj?.a?.b;  d ?? default
来源：http://cxb.jianghu66.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bfu.hywenlv.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jos.smart0.xyz

Ruby: d&.dig(:a, :b)
来源：http://uda.meibo888.top

C#:   obj?.A?.B ?? default
来源：http://vry.52xcode.cn

[H07] 断言
来源：http://rlh.andypj.xyz

Py:   assert x > 0, "必须为正"
来源：http://hck.yongpay.top

PHP:  assert($x > 0);
来源：http://ont.yonumen.top

JS:   console.assert(x > 0);
来源：http://yik.snrcjt.cn


<!-- 参考信息 -->