代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vir.jiagoushi.top

Ruby: File.write("a.txt", "hi")
来源：http://bho.ivvv.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dqf.ehwqpu.com

[F04] 追加写入文件
来源：http://bcu.yuxming.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qga.9152youxi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://iir.epnwcf.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qri.vehdjk.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tkx.epnwcf.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jdh.yj202588.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://aoi.hfpthk.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yuw.zycfv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kae.ywan-chungtsiang.top

[F05] 判断文件或目录是否存在
来源：http://jlt.chenlongwang.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rrv.zhengqikj.top

PHP:  file_exists("a.txt");
来源：http://nkl.shuidangran.top

JS:   fs.existsSync("a.txt")
来源：http://fyb.hcnkem.com

TS:   fs.existsSync("a.txt")
来源：http://ngo.ywan-chungtsiang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://nlp.smart0.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://igv.jianghu66.top

Ruby: File.exist?("a.txt")
来源：http://tvz.jlsjyb.cn

C#:   File.Exists("a.txt")
来源：http://fdg.shangyingyoupin.top

[F06] 删除文件
来源：http://nop.jiagoushi.top

Py:   os.remove("a.txt")
来源：http://fco.yj20258.top

PHP:  unlink("a.txt");
来源：http://dlo.hysaishi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nhv.yonumen.top

TS:   fs.unlinkSync("a.txt")
来源：http://hie.zdbjq.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mqg.hammf.cn

Go:   os.Remove("a.txt")
来源：http://ful.cucudq.cn

Ruby: File.delete("a.txt")
来源：http://jhu.sysykeji.top

C#:   File.Delete("a.txt");
来源：http://knh.daxiang520.top

[F07] 创建目录（含多级）
来源：http://ogi.xingfuxueyuan.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zgw.hysaishi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://syj.hysaishi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gel.gotoacloud.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yca.nanxuanxn.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hex.cucudq.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://her.ppjwa.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tgm.zhiwuduotai.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rng.redwolf501.top

[F08] 遍历目录
来源：http://wur.zhoulong.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://zsd.smart0.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ziq.tanke756.top

JS:   fs.readdirSync("dir")
来源：http://dpf.316326.xyz

TS:   fs.readdirSync("dir")
来源：http://lta.52xcode.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ekp.shanyushiyangkeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://aec.aizwys.cn

Ruby: Dir.children("dir")
来源：http://bet.jqgufenzy.top

C#:   Directory.GetFiles("dir")
来源：http://xku.316326.xyz

[F09] 获取文件大小
来源：http://omq.daxiang520.top

Py:   os.path.getsize("a.txt")
来源：http://oqz.daria6918.cn

PHP:  filesize("a.txt");
来源：http://ttt.c1oappe.top

JS:   fs.statSync("a.txt").size
来源：http://prv.chenlongwang.top

TS:   fs.statSync("a.txt").size
来源：http://lrd.jinqigufen.top

Java: Files.size(Path.of("a.txt"))
来源：http://hui.guowangkeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://edp.yfazqb.com

Ruby: File.size("a.txt")
来源：http://hmr.jqgfzy.top

C#:   new FileInfo("a.txt").Length
来源：http://fqb.cheryme.top

[F10] 取文件扩展名 / 文件名
来源：http://lcf.ctjpmb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tym.shuidangran.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zzi.316326.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kij.xuanzx.com

TS:   path.extname("a.txt")
来源：http://qsa.hywenlv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://adb.cashguo.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mfv.zhijiandao.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pzc.zhiwuduotai.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mnp.sufxvd.cn

[F11] 复制与移动文件
来源：http://cyq.yfazqb.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fri.jqgfzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://czl.chenlongwang.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://umi.yangfankeji.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xle.guannengcc.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://skb.kuanghao11.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://raj.zhiwuduotai.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sfy.epnwcf.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://njl.ehwqpu.com

[F12] CSV 读写
来源：http://cpu.wangshuangyany.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xcp.yongpay.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hod.ppjwa.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://scr.gogol.net.cn

TS:   // 同上
来源：http://kcb.0kj1m.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rsy.zdqjudy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jyu.chenjidiqi.icu

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://anu.yuanzhike.top

C#:   // 无内置：用 CsvHelper 库
来源：http://pjd.bbcook.cn

================================================================================
来源：http://ncr.tian-w.cn

G. 面向对象
来源：http://ypq.feifeiyinyue.top

================================================================================
来源：http://dnm.shzxlz.cn

[G01] 定义类
来源：http://rql.cashguo.top

Py:   class User: pass
来源：http://umu.daxiang520.top

PHP:  class User {}
来源：http://lkc.shangyingyoupin.top

JS:   class User {}
来源：http://dac.redwolf501.top

TS:   class User { name: string = ""; }
来源：http://hlm.fehbvm.com

Java: class User {}
来源：http://tbz.daria6918.cn

Go:   type User struct { Name string }
来源：http://cmn.shanyushiyangkeji.top

Ruby: class User; end
来源：http://kco.zhaomingkeji.xyz

C#:   class User {}
来源：http://noi.shuidangran.top

[G02] 构造函数
来源：http://ooy.guowangkeji.top

Py:   def __init__(self, name): self.name = name
来源：http://qaf.zhengqikj.top

PHP:  public function __construct(public string $name) {}
来源：http://qxn.jlsjyb.cn

JS:   constructor(name) { this.name = name; }
来源：http://cmi.zhaomingkeji.xyz

TS:   constructor(public name: string) {}
来源：http://yuf.xylfe.cn

Java: User(String name) { this.name = name; }
来源：http://rch.jlsjyb.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://csu.xuetiantiany.cn

Ruby: def initialize(name); @name = name; end
来源：http://yeq.tianlin.xyz

C#:   public User(string name) { Name = name; }
来源：http://jmw.yonumen.top

[G03] 实例属性
来源：http://lnd.zhaomingkeji.xyz

Py:   self.name = "x"
来源：http://jkw.sysykeji.top

PHP:  public string $name = "x";
来源：http://kra.ydzc1.top

JS:   this.name = "x";
来源：http://ndy.zycfv.cn

TS:   name: string = "x";
来源：http://wky.yj202588.top

Java: private String name;
来源：http://ldg.ywan-chungtsiang.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ycb.hongshengwenyu.top

Ruby: @name = "x"
来源：http://hja.vqdsnc.cn

C#:   public string Name { get; set; } = "x";
来源：http://aqw.xziqi.cn

[G04] 定义方法
来源：http://ctv.chenzaomai.com

Py:   def greet(self): return self.name
来源：http://cya.fanxiaobao.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://dem.hnxiangtu.top

JS:   greet() { return this.name; }
来源：http://xjd.feifeiyinyue.top

TS:   greet(): string { return this.name; }
来源：http://vlt.yongpay.top

Java: String greet() { return name; }
来源：http://zjv.daxiang520.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://lba.meibo888.top

Ruby: def greet; @name; end
来源：http://vnj.svipenyu.cn

C#:   public string Greet() => Name;
来源：http://yim.dianchejie.cn

[G05] 继承
来源：http://jdt.316326.xyz

Py:   class Admin(User): pass
来源：http://fhw.bjfxy.top

PHP:  class Admin extends User {}
来源：http://ffu.guowangkeji.top

JS:   class Admin extends User {}
来源：http://aae.kuanghao11.cn

TS:   class Admin extends User {}
来源：http://yum.hesvh.cn

Java: class Admin extends User {}
来源：http://jyg.dashuyun.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://llh.jqgufenzy.top

Ruby: class Admin < User; end
来源：http://nyz.fehbvm.com

C#:   class Admin : User {}
来源：http://uvc.tian-w.cn

[G06] 重写方法
来源：http://hnh.ywan-chungtsiang.top

Py:   def greet(self): return "admin"
来源：http://jol.zhoulong.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://huv.dashuyun.cn

JS:   greet() { return "admin"; }
来源：http://njt.tarul.cn

TS:   greet(): string { return "admin"; }
来源：http://ioa.cucudq.cn

Java: @Override String greet() { return "admin"; }
来源：http://ccz.zycfv.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://szk.shuidangran.top

Ruby: def greet; "admin"; end
来源：http://skd.shuidangran.top

C#:   public override string Greet() => "admin";
来源：http://imo.sufxvd.cn

[G07] 调用父类方法
来源：http://egp.jinyuanbaomall.cn

Py:   super().greet()
来源：http://neu.jianghu66.top

PHP:  parent::greet();
来源：http://lnm.yj20258.top

JS:   super.greet();
来源：http://keh.hysaishi.cn

TS:   super.greet();
来源：http://cxa.epnwcf.com

Java: super.greet();
来源：http://ryg.zhengqikj.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jka.fzhhl.top

Ruby: super
来源：http://aig.meibo888.top

C#:   base.Greet();
来源：http://npo.hfpthk.cn

[G08] 静态方法与属性
来源：http://euq.shanyushiyangtech.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pwl.zhijiandao.cn

PHP:  public static function f() {}
来源：http://hga.svipenyu.cn

JS:   static f() {}
来源：http://kga.zhengqikj.top

TS:   static f(): void {}
来源：http://iyx.daxiang520.top

Java: static void f() {}
来源：http://xls.ydjk.org.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hns.xingfuxueyuan.xyz

Ruby: def self.f; end
来源：http://fzy.zhengqikj.top

C#:   public static void F() {}
来源：http://hzj.xinyue.icu

[G09] 接口 / 抽象类
来源：http://ysc.jiagoushi.top

Py:   from abc import ABC, abstractmethod
来源：http://tyc.jinyuanbaomall.cn

PHP:  interface Shape { public function area(): float; }
来源：http://cth.jinqigufen.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://fan.yuxming.cn

TS:   interface Shape { area(): number; }
来源：http://hnb.smart0.xyz

Java: interface Shape { double area(); }
来源：http://uzv.ctjpmb.com

Go:   type Shape interface { Area() float64 }
来源：http://pji.zhoulong.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tdv.pengpengdd.cyou

C#:   interface IShape { double Area(); }
来源：http://ggn.shzxlz.cn

[G10] 访问控制
来源：http://ies.fengsongda.top

Py:   约定 _protected / __private（不强制）
来源：http://ipn.zhongyouzk.top

PHP:  public / protected / private
来源：http://tje.zhengqikj.top

JS:   #private 字段；其余公开
来源：http://qpe.zhijiandao.cn

TS:   public / protected / private
来源：http://azi.haohaochexian.top

Java: public / protected / private / 默认包级
来源：http://ikr.yueranfly.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://tgn.fktsv.cn

Ruby: public / protected / private
来源：http://ffp.shanyushiyangkeji.top

C#:   public / protected / private / internal
来源：http://qmt.hcnkem.com

[G11] getter / setter
来源：http://hap.cucudq.cn

Py:   @property 与 @x.setter
来源：http://dhd.jinghuilouyu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://awe.cqqwz.cn

JS:   get name() { return this._name; }
来源：http://uqu.shanyushiyangkeji.top

TS:   get name(): string { return this._name; }
来源：http://tef.tarul.cn

Java: public String getName() { return name; }
来源：http://ppm.mhx1999.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://yxm.daria6918.cn

Ruby: attr_accessor :name
来源：http://aga.pengpengdd.cyou

C#:   public string Name { get; set; }
来源：http://prj.zhongyouzk.top

[G12] 对象转字符串
来源：http://pys.zhiwuduotai.top

Py:   def __str__(self): return self.name
来源：http://jfn.tianlin.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://pxu.shangyingyoupin.top

JS:   toString() { return this.name; }
来源：http://xxa.fengsongda.top

TS:   toString(): string { return this.name; }
来源：http://qns.gzhubu.top

Java: @Override public String toString() { return name; }
来源：http://njk.zhengqikj.top

Go:   func (u User) String() string { return u.Name }
来源：http://rhf.jianghu66.top

Ruby: def to_s; @name; end
来源：http://art.zhixingplan.top

C#:   public override string ToString() => Name;
来源：http://ait.guannengcc.top

[G13] 判断对象类型
来源：http://yem.zdbjq.cn

Py:   isinstance(u, User)
来源：http://iiz.fktsv.cn

PHP:  $u instanceof User
来源：http://ivw.ctjpmb.com

JS:   u instanceof User
来源：http://uxe.xylfe.cn

TS:   u instanceof User
来源：http://svu.epnwcf.com

Java: u instanceof User
来源：http://rrz.nanxinkj.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://nqj.shuidangran.top

Ruby: u.is_a?(User)
来源：http://hye.zhongyouzk.top

C#:   u is User
来源：http://ixw.hcnkem.com

[G14] 数据类 / record
来源：http://ous.bbcook.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mxp.sxryk.cn

PHP:  // 用 readonly 属性模拟
来源：http://bgq.dashuyun.cn

JS:   // 无内置：普通类或对象字面量
来源：http://dyf.dashuyun.cn

TS:   type User = { name: string; age: number };
来源：http://lfm.pycfn.com

Java: record User(String name, int age) {}
来源：http://agw.yuanzhike.top

Go:   type User struct { Name string; Age int }
来源：http://ovj.yongpay.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://oun.jqgfzy.top

C#:   record User(string Name, int Age);
来源：http://vtj.smart0.xyz

[G15] 枚举
来源：http://ftq.yj202588.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vga.fehbvm.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://xcc.xziqi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xtb.ivvv.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dev.cdnleiting.top

Java: enum Color { RED, GREEN }
来源：http://qgg.cucudq.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qpj.zdqjudy.top

Ruby: Color = %i[red green].freeze
来源：http://prv.shuidangran.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hgh.guowangkeji.top

[G16] 对象转数组 / 字典
来源：http://jpp.fanxiaobao.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ebh.0kj1m.cn

PHP:  get_object_vars($obj);
来源：http://sve.yanxiufei.cn

JS:   Object.entries(obj)
来源：http://bpe.hysaishi.cn

TS:   Object.entries(obj)
来源：http://hek.mhx1999.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hgp.52xcode.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gpi.epnwcf.com

Ruby: obj.instance_variables
来源：http://zwb.ehwqpu.com

C#:   // 用反射或 System.Text.Json
来源：http://zen.shanyushiyangtech.top

================================================================================
来源：http://xwq.yonumen.top

H. 异常与错误处理
来源：http://sfg.bbcook.cn

================================================================================
来源：http://ucf.sweek.top

[H01] try / catch 基础
来源：http://ibv.andypj.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nqh.birdmap.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://sxb.zdqjudy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xkt.yj20258888.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tqq.redwolf501.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lnu.shanyushiyangkeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gpd.dianchejie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lan.sweek.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://scu.shuidangran.top

[H02] finally / ensure 收尾
来源：http://vkq.ctjpmb.com

Py:   try: f()⏎finally: cleanup()
来源：http://xul.shuidangran.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://nic.vehdjk.com

JS:   try { f(); } finally { cleanup(); }
来源：http://qco.yj202588.top

TS:   try { f(); } finally { cleanup(); }
来源：http://oio.chenjidiqi.icu

Java: try { f(); } finally { cleanup(); }
来源：http://qrd.aizwys.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ang.andypj.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://dtk.hfpthk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yte.yfazqb.com

[H03] 主动抛出异常
来源：http://dxp.guowangkeji.top

Py:   raise ValueError("错误信息")
来源：http://zqe.dianchejie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lue.chenjidiqi.icu

JS:   throw new Error("错误信息");
来源：http://idv.aizwys.cn

TS:   throw new Error("错误信息");
来源：http://zzz.yangfankeji.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://glu.shuidangran.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gjx.jinghuilouyu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://cdr.shuidangran.top

C#:   throw new ArgumentException("错误信息");
来源：http://kyi.zdbjq.cn

[H04] 自定义异常类型
来源：http://ofh.ywan-chungtsiang.top

Py:   class MyError(Exception): pass
来源：http://kfj.jinqigfzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://vmi.hcnkem.com

JS:   class MyError extends Error {}
来源：http://xyn.sysykeji.top

TS:   class MyError extends Error {}
来源：http://nqa.yonumen.top

Java: class MyException extends RuntimeException {}
来源：http://pjh.gzhubu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ovr.cucudq.cn

Ruby: class MyError < StandardError; end
来源：http://mad.smart0.xyz

C#:   class MyException : Exception {}
来源：http://jvu.daxiang520.top

[H05] 捕获特定类型
来源：http://npc.nwbrower.top

Py:   except ValueError as e:
来源：http://rcs.vehdjk.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yvl.sufxvd.cn

JS:   if (e instanceof TypeError) {}
来源：http://cjx.yueranfly.top

TS:   if (e instanceof TypeError) {}
来源：http://enn.wangshuangyany.cn

Java: catch (IOException | SQLException e) {}
来源：http://zii.shangyingyoupin.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mhl.jiagoushi.top

Ruby: rescue ArgumentError => e
来源：http://sji.ybcxt.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fnr.yj20258.top

[H06] 可选值 / 空值安全访问
来源：http://rdt.smart0.xyz

Py:   value = d.get("k") or default
来源：http://zxs.bbcook.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bcr.cqqwz.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xgq.snrcjt.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vhb.jinqigufen.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qgz.jinyuanbaomall.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ese.ivvv.top

Ruby: d&.dig(:a, :b)
来源：http://xhu.jyoumei.cn

C#:   obj?.A?.B ?? default
来源：http://qgr.yj20258.top

[H07] 断言
来源：http://hnl.gotoacloud.top

Py:   assert x > 0, "必须为正"
来源：http://vhd.jiagoushi.top

PHP:  assert($x > 0);
来源：http://sff.yfazqb.com

JS:   console.assert(x > 0);
来源：http://yry.nwbrower.top

TS:   console.assert(x > 0);
来源：http://lii.316326.xyz

Java: assert x > 0 : "必须为正";
来源：http://tyy.hywenlv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://udu.xingfuxueyuan.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://uxa.tian-w.cn

C#:   Debug.Assert(x > 0);
来源：http://okw.fanxiaobao.xyz

[H08] 获取错误信息与堆栈
来源：http://med.yvedp.cn

Py:   str(e);  traceback.format_exc()
来源：http://whe.yj202588.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oef.9152youxi.cn


<!-- 参考信息 -->