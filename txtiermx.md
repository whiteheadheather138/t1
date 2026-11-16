代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://alc.yfazqb.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://umy.zhaomingkeji.xyz

PHP:  file_exists("a.txt");
来源：http://ibt.316326.xyz

JS:   fs.existsSync("a.txt")
来源：http://ttr.tarul.cn

TS:   fs.existsSync("a.txt")
来源：http://mfg.zhijiandao.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hyq.yfazqb.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fqq.ybcxt.top

Ruby: File.exist?("a.txt")
来源：http://zft.pycfn.com

C#:   File.Exists("a.txt")
来源：http://uiu.hnqzz.top

[F06] 删除文件
来源：http://tuu.iojbl.cn

Py:   os.remove("a.txt")
来源：http://vty.redwolf501.top

PHP:  unlink("a.txt");
来源：http://ivc.birdmap.top

JS:   fs.unlinkSync("a.txt")
来源：http://klz.jinqigufen.top

TS:   fs.unlinkSync("a.txt")
来源：http://fyl.zhixingplan.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pqp.pycfn.com

Go:   os.Remove("a.txt")
来源：http://vlk.yvedp.cn

Ruby: File.delete("a.txt")
来源：http://xbh.zhijiandao.cn

C#:   File.Delete("a.txt");
来源：http://bvg.ydjk.org.cn

[F07] 创建目录（含多级）
来源：http://ndc.9152youxi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://aqk.yonumen.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ceu.hammf.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wgt.fengsongda.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ctv.jinyuanbaomall.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tuy.zdqjudy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kyw.zdqjudy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wlj.hnxiangtu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rtu.daxiang520.top

[F08] 遍历目录
来源：http://jsc.wangdashe.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hvt.yueranfly.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lwf.zhijiandao.cn

JS:   fs.readdirSync("dir")
来源：http://qnj.sxryk.cn

TS:   fs.readdirSync("dir")
来源：http://pbn.gaohongyu789.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xuz.xuetiantiany.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bdy.0kj1m.cn

Ruby: Dir.children("dir")
来源：http://czz.meibo888.top

C#:   Directory.GetFiles("dir")
来源：http://qbi.fktsv.cn

[F09] 获取文件大小
来源：http://tvb.gzhubu.top

Py:   os.path.getsize("a.txt")
来源：http://tcc.chenzaomai.com

PHP:  filesize("a.txt");
来源：http://dmv.vehdjk.com

JS:   fs.statSync("a.txt").size
来源：http://hmj.shanyushiyangkeji.top

TS:   fs.statSync("a.txt").size
来源：http://ztj.ydzc1.top

Java: Files.size(Path.of("a.txt"))
来源：http://vms.gzhubu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://efp.jlsjyb.cn

Ruby: File.size("a.txt")
来源：http://qeu.uphjek.com

C#:   new FileInfo("a.txt").Length
来源：http://ymq.tian-w.cn

[F10] 取文件扩展名 / 文件名
来源：http://hkb.smart0.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xpv.gaohongyu789.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dbe.dianchejie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tqc.wangshuangyany.cn

TS:   path.extname("a.txt")
来源：http://ryr.zhiwuduotai.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nio.shanyushiyangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sat.dashuyun.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ony.nwbrower.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kno.sufxvd.cn

[F11] 复制与移动文件
来源：http://mbt.hnxiangtu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nke.yueranfly.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://smn.jqgfzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qpd.zhaomingkeji.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lsg.yj20258888.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nbp.uphjek.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kvm.hcnkem.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rnh.daria6918.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mxq.guowangkeji.top

[F12] CSV 读写
来源：http://dkv.tarul.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qlz.cdnleiting.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jum.redwolf501.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pxi.havefunace.top

TS:   // 同上
来源：http://erl.yanxiufei.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://was.redwolf501.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://stx.ybcxt.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rnq.xingfuxueyuan.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://jal.hfpthk.cn

================================================================================
来源：http://kkq.shangyingyoupin.top

G. 面向对象
来源：http://qqu.daria6918.cn

================================================================================
来源：http://wul.tarul.cn

[G01] 定义类
来源：http://qmz.52xcode.cn

Py:   class User: pass
来源：http://hfo.epnwcf.com

PHP:  class User {}
来源：http://rqv.chenlongwang.top

JS:   class User {}
来源：http://fou.snrcjt.cn

TS:   class User { name: string = ""; }
来源：http://htp.feifeiyinyue.top

Java: class User {}
来源：http://dwg.ppjwa.cn

Go:   type User struct { Name string }
来源：http://ryj.chenjidiqi.icu

Ruby: class User; end
来源：http://rxt.pengpengdd.cyou

C#:   class User {}
来源：http://tud.jyoumei.cn

[G02] 构造函数
来源：http://tsu.xuanzx.com

Py:   def __init__(self, name): self.name = name
来源：http://kiq.hammf.cn

PHP:  public function __construct(public string $name) {}
来源：http://cwh.feifeiyinyue.top

JS:   constructor(name) { this.name = name; }
来源：http://css.jqgufenzy.top

TS:   constructor(public name: string) {}
来源：http://ndq.yj20258.top

Java: User(String name) { this.name = name; }
来源：http://vob.zycfv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oic.chenlongwang.top

Ruby: def initialize(name); @name = name; end
来源：http://lqr.zycfv.cn

C#:   public User(string name) { Name = name; }
来源：http://xhm.gotoacloud.top

[G03] 实例属性
来源：http://zsy.svipenyu.cn

Py:   self.name = "x"
来源：http://fbm.xinyue.icu

PHP:  public string $name = "x";
来源：http://nch.daria6918.cn

JS:   this.name = "x";
来源：http://bpw.zdqjudy.top

TS:   name: string = "x";
来源：http://grq.dianchejie.cn

Java: private String name;
来源：http://qds.316326.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sgp.daxiang520.top

Ruby: @name = "x"
来源：http://ilq.cqqwz.cn

C#:   public string Name { get; set; } = "x";
来源：http://coi.cashguo.top

[G04] 定义方法
来源：http://dbp.ybcxt.top

Py:   def greet(self): return self.name
来源：http://hcr.svipenyu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://etm.fzhhl.top

JS:   greet() { return this.name; }
来源：http://zhj.zdqjudy.top

TS:   greet(): string { return this.name; }
来源：http://kfp.jinqigfzy.top

Java: String greet() { return name; }
来源：http://rum.pycfn.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://tev.cdnleiting.top

Ruby: def greet; @name; end
来源：http://uky.xuanzx.com

C#:   public string Greet() => Name;
来源：http://jpq.havefunace.top

[G05] 继承
来源：http://lwy.zhiwuduotai.top

Py:   class Admin(User): pass
来源：http://moq.hfpthk.cn

PHP:  class Admin extends User {}
来源：http://iae.hesvh.cn

JS:   class Admin extends User {}
来源：http://cwo.zhixingplan.top

TS:   class Admin extends User {}
来源：http://tqz.jqgufenzy.top

Java: class Admin extends User {}
来源：http://lmh.sufxvd.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wir.haohaochexian.top

Ruby: class Admin < User; end
来源：http://jss.cashguo.top

C#:   class Admin : User {}
来源：http://pik.zhoulong.xyz

[G06] 重写方法
来源：http://bzj.jinghuilouyu.cn

Py:   def greet(self): return "admin"
来源：http://ucc.ivvv.top

PHP:  public function greet(): string { return "admin"; }
来源：http://tfc.shzxlz.cn

JS:   greet() { return "admin"; }
来源：http://azf.jinghuilouyu.cn

TS:   greet(): string { return "admin"; }
来源：http://ave.fanxiaobao.xyz

Java: @Override String greet() { return "admin"; }
来源：http://oam.nwbrower.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bno.yj202588.top

Ruby: def greet; "admin"; end
来源：http://zwk.gzhubu.top

C#:   public override string Greet() => "admin";
来源：http://nxh.shanyushiyangkeji.top

[G07] 调用父类方法
来源：http://ebv.hysaishi.cn

Py:   super().greet()
来源：http://nqk.zycfv.cn

PHP:  parent::greet();
来源：http://anc.shanyushiyangkeji.top

JS:   super.greet();
来源：http://zig.yj20258888.top

TS:   super.greet();
来源：http://dwm.nanxuanxn.top

Java: super.greet();
来源：http://hbb.hnqzz.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mce.birdmap.top

Ruby: super
来源：http://jop.xingfuxueyuan.xyz

C#:   base.Greet();
来源：http://uat.sxryk.cn

[G08] 静态方法与属性
来源：http://lwu.ivvv.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://iqt.xylfe.cn

PHP:  public static function f() {}
来源：http://uau.nwbrower.top

JS:   static f() {}
来源：http://fok.kuanghao11.cn

TS:   static f(): void {}
来源：http://xcc.pycfn.com

Java: static void f() {}
来源：http://mnj.smart0.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://uhr.zdqjudy.top

Ruby: def self.f; end
来源：http://ldw.hongshengwenyu.top

C#:   public static void F() {}
来源：http://rgl.dashuyun.cn

[G09] 接口 / 抽象类
来源：http://bso.hammf.cn

Py:   from abc import ABC, abstractmethod
来源：http://ldh.birdmap.top

PHP:  interface Shape { public function area(): float; }
来源：http://wxb.sysykeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ldg.sysykeji.top

TS:   interface Shape { area(): number; }
来源：http://bll.hcnkem.com

Java: interface Shape { double area(); }
来源：http://zjd.mhx1999.top

Go:   type Shape interface { Area() float64 }
来源：http://tmx.yuxming.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cgd.fzhhl.top

C#:   interface IShape { double Area(); }
来源：http://vje.hnxiangtu.top

[G10] 访问控制
来源：http://dci.quarkkingdee.top

Py:   约定 _protected / __private（不强制）
来源：http://ptq.uphjek.com

PHP:  public / protected / private
来源：http://vqz.316326.xyz

JS:   #private 字段；其余公开
来源：http://iuy.feifeiyinyue.top

TS:   public / protected / private
来源：http://bai.yueranfly.top

Java: public / protected / private / 默认包级
来源：http://uni.zdbjq.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://aib.yuanzhike.top

Ruby: public / protected / private
来源：http://luo.zhaomingkeji.xyz

C#:   public / protected / private / internal
来源：http://hqo.zhongyouzk.top

[G11] getter / setter
来源：http://iry.shanyushiyangtech.top

Py:   @property 与 @x.setter
来源：http://shi.sweek.top

PHP:  public function getName(): string { return $this->name; }
来源：http://uuk.shzxlz.cn

JS:   get name() { return this._name; }
来源：http://snc.haohaochexian.top

TS:   get name(): string { return this._name; }
来源：http://xdj.shanyushiyangkeji.top

Java: public String getName() { return name; }
来源：http://kjk.chenzaomai.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://xex.xuanzx.com

Ruby: attr_accessor :name
来源：http://ibd.cucudq.cn

C#:   public string Name { get; set; }
来源：http://nnd.sysykeji.top

[G12] 对象转字符串
来源：http://msc.tianlin.xyz

Py:   def __str__(self): return self.name
来源：http://cdw.yangfankeji.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://sea.shanyushiyangtech.top

JS:   toString() { return this.name; }
来源：http://gyb.feifeiyinyue.top

TS:   toString(): string { return this.name; }
来源：http://dlh.shzxlz.cn

Java: @Override public String toString() { return name; }
来源：http://bcx.fanxiaobao.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://who.vqdsnc.cn

Ruby: def to_s; @name; end
来源：http://fmc.ybcxt.top

C#:   public override string ToString() => Name;
来源：http://ecz.jlsjyb.cn

[G13] 判断对象类型
来源：http://oso.shanyushiyangtech.top

Py:   isinstance(u, User)
来源：http://qjs.jlsjyb.cn

PHP:  $u instanceof User
来源：http://xrh.hnqzz.top

JS:   u instanceof User
来源：http://svh.gogol.net.cn

TS:   u instanceof User
来源：http://jph.316326.xyz

Java: u instanceof User
来源：http://oje.52xcode.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qco.fengsongda.top

Ruby: u.is_a?(User)
来源：http://ptr.yj202588.top

C#:   u is User
来源：http://usw.yj202588.top

[G14] 数据类 / record
来源：http://ecp.ehwqpu.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mmr.gogol.net.cn

PHP:  // 用 readonly 属性模拟
来源：http://wva.xziqi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kmw.zhengqikj.top

TS:   type User = { name: string; age: number };
来源：http://qoj.dianchejie.cn

Java: record User(String name, int age) {}
来源：http://iaq.mhx1999.top

Go:   type User struct { Name string; Age int }
来源：http://ced.aizwys.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ish.chenzaomai.com

C#:   record User(string Name, int Age);
来源：http://udu.vehdjk.com

[G15] 枚举
来源：http://fcr.jianghu66.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qkv.wangdashe.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://iam.shzxlz.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fct.cqqwz.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://woh.sweek.top

Java: enum Color { RED, GREEN }
来源：http://kod.zhiwuduotai.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jhy.haohaochexian.top

Ruby: Color = %i[red green].freeze
来源：http://mlx.gotoacloud.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://oae.yj20258.top

[G16] 对象转数组 / 字典
来源：http://ecx.hcnkem.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lnr.tianlin.xyz

PHP:  get_object_vars($obj);
来源：http://cdz.ybcxt.top

JS:   Object.entries(obj)
来源：http://qil.fengsongda.top

TS:   Object.entries(obj)
来源：http://riv.vehdjk.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://eza.0kj1m.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ogs.xylfe.cn

Ruby: obj.instance_variables
来源：http://ogc.hnqzz.top

C#:   // 用反射或 System.Text.Json
来源：http://bod.hesvh.cn

================================================================================
来源：http://sjo.jiagoushi.top

H. 异常与错误处理
来源：http://tyh.jlsjyb.cn

================================================================================
来源：http://bgs.jinqigfzy.top

[H01] try / catch 基础
来源：http://fvr.jianghu66.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wjx.jinghuilouyu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qco.fengsongda.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rla.cdnleiting.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://meg.jianghu66.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tav.fengsongda.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sha.fengsongda.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pbo.sufxvd.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://air.uphjek.com

[H02] finally / ensure 收尾
来源：http://ftx.jinqigufen.top

Py:   try: f()⏎finally: cleanup()
来源：http://tdm.yj202588.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://gqk.gogol.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ijm.havefunace.top

TS:   try { f(); } finally { cleanup(); }
来源：http://kpn.xingfuxueyuan.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://agr.zdbjq.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://djx.yvedp.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://uxj.wangshuangyany.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vvb.zhengqikj.top

[H03] 主动抛出异常
来源：http://qrl.haohaochexian.top

Py:   raise ValueError("错误信息")
来源：http://kzs.yangfankeji.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ldj.daxiang520.top

JS:   throw new Error("错误信息");
来源：http://iqk.andypj.xyz

TS:   throw new Error("错误信息");
来源：http://ynz.xziqi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qkn.zhiwuduotai.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cza.sjlbkw.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://btf.cashguo.top

C#:   throw new ArgumentException("错误信息");
来源：http://wfn.uphjek.com

[H04] 自定义异常类型
来源：http://dil.redwolf501.top

Py:   class MyError(Exception): pass
来源：http://crc.ctjpmb.com

PHP:  class MyError extends RuntimeException {}
来源：http://xdy.xinyue.icu

JS:   class MyError extends Error {}
来源：http://xgt.tarul.cn

TS:   class MyError extends Error {}
来源：http://qpn.zhiwuduotai.top

Java: class MyException extends RuntimeException {}
来源：http://kms.zhijiandao.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jut.bjfxy.top

Ruby: class MyError < StandardError; end
来源：http://cmq.smart0.xyz

C#:   class MyException : Exception {}
来源：http://ata.zhoulong.xyz

[H05] 捕获特定类型
来源：http://evg.cashguo.top

Py:   except ValueError as e:
来源：http://llr.hfpthk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kjh.9152youxi.cn

JS:   if (e instanceof TypeError) {}
来源：http://bkd.jinghuilouyu.cn

TS:   if (e instanceof TypeError) {}
来源：http://khe.ydjk.org.cn

Java: catch (IOException | SQLException e) {}
来源：http://gkk.daxiang520.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ckw.epnwcf.com

Ruby: rescue ArgumentError => e
来源：http://rjh.jyoumei.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://azr.yangfankeji.com

[H06] 可选值 / 空值安全访问
来源：http://yhz.shuidangran.top

Py:   value = d.get("k") or default
来源：http://nas.ctjpmb.com

PHP:  $v = $d["k"] ?? null;
来源：http://qxf.yonumen.top

JS:   obj?.a?.b;  d ?? default
来源：http://mun.hammf.cn

TS:   obj?.a?.b;  d ?? default
来源：http://lib.uphjek.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ikg.316326.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://pta.pycfn.com

Ruby: d&.dig(:a, :b)
来源：http://gpg.smart0.xyz

C#:   obj?.A?.B ?? default
来源：http://ctc.vqdsnc.cn

[H07] 断言
来源：http://gyk.jqgufenzy.top

Py:   assert x > 0, "必须为正"
来源：http://tqv.xinyue.icu

PHP:  assert($x > 0);
来源：http://kmi.nanxinkj.top

JS:   console.assert(x > 0);
来源：http://gkg.hcnkem.com

TS:   console.assert(x > 0);
来源：http://hvp.gotoacloud.top

Java: assert x > 0 : "必须为正";
来源：http://mjn.tarul.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dzo.yuxming.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ksm.yueranfly.top

C#:   Debug.Assert(x > 0);
来源：http://oqb.yuxming.cn

[H08] 获取错误信息与堆栈
来源：http://zym.iojbl.cn

Py:   str(e);  traceback.format_exc()
来源：http://hly.yanxiufei.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://can.yueranfly.top

JS:   e.message;  e.stack
来源：http://ifq.zdbjq.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://iet.cdnleiting.top

Java: e.getMessage();  e.printStackTrace()
来源：http://gyd.ppjwa.cn

Go:   err.Error()
来源：http://nwg.jlsjyb.cn

Ruby: e.message;  e.backtrace
来源：http://khi.shzxlz.cn

C#:   e.Message;  e.StackTrace
来源：http://unb.quarkkingdee.top

[H09] 带错误码的异常
来源：http://gzu.xuetiantiany.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hfr.0kj1m.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ctm.shanyushiyangtech.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://oba.ppjwa.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://urf.xylfe.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ntw.hysaishi.cn


<!-- 参考信息 -->