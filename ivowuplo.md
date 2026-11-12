代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://oye.cashguo.top

Ruby: File.write("a.txt", "hi")
来源：http://rrz.gaohongyu789.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lyp.gaohongyu789.top

[F04] 追加写入文件
来源：http://jls.chenjidiqi.icu

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wjd.aibaodan.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://aoo.quarkkingdee.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qoo.hfpthk.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xkt.zhixingplan.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hif.xingfuxueyuan.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://srb.smart0.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://igq.xylfe.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dtg.dianchejie.cn

[F05] 判断文件或目录是否存在
来源：http://plt.gotoacloud.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vfv.hfpthk.cn

PHP:  file_exists("a.txt");
来源：http://dkv.jinghuilouyu.cn

JS:   fs.existsSync("a.txt")
来源：http://mfo.ehwqpu.com

TS:   fs.existsSync("a.txt")
来源：http://qfe.hywenlv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tkx.gaohongyu789.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kxa.vehdjk.com

Ruby: File.exist?("a.txt")
来源：http://zkb.pycfn.com

C#:   File.Exists("a.txt")
来源：http://dsh.hysaishi.cn

[F06] 删除文件
来源：http://qzd.nanxuanxn.top

Py:   os.remove("a.txt")
来源：http://wol.pycfn.com

PHP:  unlink("a.txt");
来源：http://viq.uphjek.com

JS:   fs.unlinkSync("a.txt")
来源：http://wqk.chenlongwang.top

TS:   fs.unlinkSync("a.txt")
来源：http://gid.gotoacloud.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yuu.daria6918.cn

Go:   os.Remove("a.txt")
来源：http://ctd.yongpay.top

Ruby: File.delete("a.txt")
来源：http://qit.jinqigfzy.top

C#:   File.Delete("a.txt");
来源：http://jph.tanke756.top

[F07] 创建目录（含多级）
来源：http://ixx.jiagoushi.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://uit.svipenyu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xtn.shanyushiyangkeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rjy.daxiang520.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ijv.cucudq.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mrp.tianlin.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ddi.chenlongwang.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cyr.zhoulong.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ydd.zhijiandao.cn

[F08] 遍历目录
来源：http://ctn.wangshuangyany.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://kwt.zhiwuduotai.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nkw.fanxiaobao.xyz

JS:   fs.readdirSync("dir")
来源：http://xrv.ivvv.top

TS:   fs.readdirSync("dir")
来源：http://rkp.jinghuilouyu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ldl.sweek.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://pop.xylfe.cn

Ruby: Dir.children("dir")
来源：http://gcz.snrcjt.cn

C#:   Directory.GetFiles("dir")
来源：http://mex.c1oappe.top

[F09] 获取文件大小
来源：http://msq.wangshuangyany.cn

Py:   os.path.getsize("a.txt")
来源：http://zza.cheryme.top

PHP:  filesize("a.txt");
来源：http://lqv.shzxlz.cn

JS:   fs.statSync("a.txt").size
来源：http://len.hnqzz.top

TS:   fs.statSync("a.txt").size
来源：http://tvu.yangfankeji.com

Java: Files.size(Path.of("a.txt"))
来源：http://opo.yj20258888.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qrb.chenjidiqi.icu

Ruby: File.size("a.txt")
来源：http://xeg.xinyue.icu

C#:   new FileInfo("a.txt").Length
来源：http://vrg.chenjidiqi.icu

[F10] 取文件扩展名 / 文件名
来源：http://kof.zhixingplan.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fdm.cheryme.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lpc.wangdashe.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dkc.zdbjq.cn

TS:   path.extname("a.txt")
来源：http://mpj.meibo888.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://whx.cqqwz.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uch.yueranfly.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ncl.zycfv.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ckm.jlsjyb.cn

[F11] 复制与移动文件
来源：http://phc.vehdjk.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qsk.kuanghao11.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tgj.sufxvd.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rtn.zhiwuduotai.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bru.shanyushiyangtech.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://osr.gotoacloud.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ddg.0kj1m.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ihr.quarkkingdee.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wog.hfpthk.cn

[F12] CSV 读写
来源：http://dwf.bjfxy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jgh.dianchejie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wjk.kuanghao11.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vjf.hongshengwenyu.top

TS:   // 同上
来源：http://jed.316326.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cyu.tarul.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yuv.pycfn.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kcw.hnqzz.top

C#:   // 无内置：用 CsvHelper 库
来源：http://wjf.yongpay.top

================================================================================
来源：http://kwh.haohaochexian.top

G. 面向对象
来源：http://tyv.hesvh.cn

================================================================================
来源：http://fao.fehbvm.com

[G01] 定义类
来源：http://pok.sweek.top

Py:   class User: pass
来源：http://shh.fehbvm.com

PHP:  class User {}
来源：http://wsy.gzhubu.top

JS:   class User {}
来源：http://uqh.hnxiangtu.top

TS:   class User { name: string = ""; }
来源：http://ikb.sysykeji.top

Java: class User {}
来源：http://xmc.meibo888.top

Go:   type User struct { Name string }
来源：http://mtg.fktsv.cn

Ruby: class User; end
来源：http://ocy.tanke756.top

C#:   class User {}
来源：http://srk.fktsv.cn

[G02] 构造函数
来源：http://vjm.daxiang520.top

Py:   def __init__(self, name): self.name = name
来源：http://dcp.iojbl.cn

PHP:  public function __construct(public string $name) {}
来源：http://dqt.shanyushiyangkeji.top

JS:   constructor(name) { this.name = name; }
来源：http://mkc.vqdsnc.cn

TS:   constructor(public name: string) {}
来源：http://axc.chenjidiqi.icu

Java: User(String name) { this.name = name; }
来源：http://zls.sufxvd.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://muv.yueranfly.top

Ruby: def initialize(name); @name = name; end
来源：http://lui.pengpengdd.cyou

C#:   public User(string name) { Name = name; }
来源：http://ncu.pycfn.com

[G03] 实例属性
来源：http://wax.sufxvd.cn

Py:   self.name = "x"
来源：http://lgr.hammf.cn

PHP:  public string $name = "x";
来源：http://jhk.chenlongwang.top

JS:   this.name = "x";
来源：http://kgg.uphjek.com

TS:   name: string = "x";
来源：http://zrr.feifeiyinyue.top

Java: private String name;
来源：http://isq.9152youxi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kuw.ydzc1.top

Ruby: @name = "x"
来源：http://vkq.hammf.cn

C#:   public string Name { get; set; } = "x";
来源：http://daj.kuanghao11.cn

[G04] 定义方法
来源：http://jyr.uphjek.com

Py:   def greet(self): return self.name
来源：http://veo.birdmap.top

PHP:  public function greet(): string { return $this->name; }
来源：http://diw.hcnkem.com

JS:   greet() { return this.name; }
来源：http://qzg.feifeiyinyue.top

TS:   greet(): string { return this.name; }
来源：http://mpt.xuanzx.com

Java: String greet() { return name; }
来源：http://tdz.yj20258.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://wjs.zhixingplan.top

Ruby: def greet; @name; end
来源：http://vmz.zhoulong.xyz

C#:   public string Greet() => Name;
来源：http://gxi.shzxlz.cn

[G05] 继承
来源：http://rou.hcnkem.com

Py:   class Admin(User): pass
来源：http://wyr.sxryk.cn

PHP:  class Admin extends User {}
来源：http://sxi.fzhhl.top

JS:   class Admin extends User {}
来源：http://ein.guowangkeji.top

TS:   class Admin extends User {}
来源：http://zxx.jiagoushi.top

Java: class Admin extends User {}
来源：http://clr.guowangkeji.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lef.fzhhl.top

Ruby: class Admin < User; end
来源：http://ign.pycfn.com

C#:   class Admin : User {}
来源：http://gvz.yfazqb.com

[G06] 重写方法
来源：http://ngg.chenjidiqi.icu

Py:   def greet(self): return "admin"
来源：http://chz.cqqwz.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yvh.fehbvm.com

JS:   greet() { return "admin"; }
来源：http://bcc.tian-w.cn

TS:   greet(): string { return "admin"; }
来源：http://boz.uphjek.com

Java: @Override String greet() { return "admin"; }
来源：http://vfc.yuanzhike.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ags.haohaochexian.top

Ruby: def greet; "admin"; end
来源：http://nkh.shzxlz.cn

C#:   public override string Greet() => "admin";
来源：http://qle.jiagoushi.top

[G07] 调用父类方法
来源：http://kfz.chenjidiqi.icu

Py:   super().greet()
来源：http://osk.ybcxt.top

PHP:  parent::greet();
来源：http://vwz.tarul.cn

JS:   super.greet();
来源：http://qei.nwbrower.top

TS:   super.greet();
来源：http://udw.fzhhl.top

Java: super.greet();
来源：http://mor.birdmap.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dnm.daria6918.cn

Ruby: super
来源：http://bqa.quarkkingdee.top

C#:   base.Greet();
来源：http://qcq.shanyushiyangkeji.top

[G08] 静态方法与属性
来源：http://wew.tanke756.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rjs.meibo888.top

PHP:  public static function f() {}
来源：http://dsx.zdqjudy.top

JS:   static f() {}
来源：http://fdh.yangfankeji.com

TS:   static f(): void {}
来源：http://smj.sxryk.cn

Java: static void f() {}
来源：http://zia.zdbjq.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://inv.ivvv.top

Ruby: def self.f; end
来源：http://tzg.birdmap.top

C#:   public static void F() {}
来源：http://owk.xinyue.icu

[G09] 接口 / 抽象类
来源：http://oja.jinqigfzy.top

Py:   from abc import ABC, abstractmethod
来源：http://qif.jinqigufen.top

PHP:  interface Shape { public function area(): float; }
来源：http://tcg.zhiwuduotai.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://rfk.nanxinkj.top

TS:   interface Shape { area(): number; }
来源：http://qoq.dashuyun.cn

Java: interface Shape { double area(); }
来源：http://vcv.zhiwuduotai.top

Go:   type Shape interface { Area() float64 }
来源：http://amb.sweek.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uqx.wangdashe.top

C#:   interface IShape { double Area(); }
来源：http://ide.wangdashe.top

[G10] 访问控制
来源：http://rph.chenzaomai.com

Py:   约定 _protected / __private（不强制）
来源：http://lno.dashuyun.cn

PHP:  public / protected / private
来源：http://fpy.xziqi.cn

JS:   #private 字段；其余公开
来源：http://rvn.cashguo.top

TS:   public / protected / private
来源：http://ria.fengsongda.top

Java: public / protected / private / 默认包级
来源：http://jkl.jinyuanbaomall.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ewm.9152youxi.cn

Ruby: public / protected / private
来源：http://zow.jyoumei.cn

C#:   public / protected / private / internal
来源：http://rza.yanxiufei.cn

[G11] getter / setter
来源：http://pcv.hysaishi.cn

Py:   @property 与 @x.setter
来源：http://ybn.jiagoushi.top

PHP:  public function getName(): string { return $this->name; }
来源：http://kys.sjlbkw.cn

JS:   get name() { return this._name; }
来源：http://cct.zhengqikj.top

TS:   get name(): string { return this._name; }
来源：http://kim.cheryme.top

Java: public String getName() { return name; }
来源：http://nhp.shanyushiyangkeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ucd.chenjidiqi.icu

Ruby: attr_accessor :name
来源：http://zod.nwbrower.top

C#:   public string Name { get; set; }
来源：http://ksq.yanxiufei.cn

[G12] 对象转字符串
来源：http://kgr.xylfe.cn

Py:   def __str__(self): return self.name
来源：http://ldt.quarkkingdee.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://icl.jyoumei.cn

JS:   toString() { return this.name; }
来源：http://fef.cdnleiting.top

TS:   toString(): string { return this.name; }
来源：http://ymn.xinyue.icu

Java: @Override public String toString() { return name; }
来源：http://jcw.fzhhl.top

Go:   func (u User) String() string { return u.Name }
来源：http://eka.yj202588.top

Ruby: def to_s; @name; end
来源：http://aqa.hysaishi.cn

C#:   public override string ToString() => Name;
来源：http://okz.jinqigfzy.top

[G13] 判断对象类型
来源：http://qdd.andypj.xyz

Py:   isinstance(u, User)
来源：http://ien.zhixingplan.top

PHP:  $u instanceof User
来源：http://ibl.zhengqikj.top

JS:   u instanceof User
来源：http://rui.cdnleiting.top

TS:   u instanceof User
来源：http://oiw.uphjek.com

Java: u instanceof User
来源：http://vrc.xinyue.icu

Go:   u, ok := v.(User)            // 类型断言
来源：http://zto.jlsjyb.cn

Ruby: u.is_a?(User)
来源：http://ipy.shangyingyoupin.top

C#:   u is User
来源：http://nff.yueranfly.top

[G14] 数据类 / record
来源：http://nsc.shuidangran.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ggk.havefunace.top

PHP:  // 用 readonly 属性模拟
来源：http://rha.shuidangran.top

JS:   // 无内置：普通类或对象字面量
来源：http://ymg.ctjpmb.com

TS:   type User = { name: string; age: number };
来源：http://elt.hysaishi.cn

Java: record User(String name, int age) {}
来源：http://dwa.wangshuangyany.cn

Go:   type User struct { Name string; Age int }
来源：http://xns.chenjidiqi.icu

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tqx.daria6918.cn

C#:   record User(string Name, int Age);
来源：http://tco.feifeiyinyue.top

[G15] 枚举
来源：http://abd.aizwys.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ezn.bjfxy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://tvy.chenzaomai.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cww.hfpthk.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uns.fanxiaobao.xyz

Java: enum Color { RED, GREEN }
来源：http://xuv.hywenlv.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oho.yj20258888.top

Ruby: Color = %i[red green].freeze
来源：http://znn.sweek.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://set.yonumen.top

[G16] 对象转数组 / 字典
来源：http://ryt.vehdjk.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://isy.tanke756.top

PHP:  get_object_vars($obj);
来源：http://fck.yvedp.cn

JS:   Object.entries(obj)
来源：http://sdz.ydzc1.top

TS:   Object.entries(obj)
来源：http://xvu.pengpengdd.cyou

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://amf.c1oappe.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://due.shanyushiyangkeji.top

Ruby: obj.instance_variables
来源：http://xzg.gzhubu.top

C#:   // 用反射或 System.Text.Json
来源：http://npt.xingfuxueyuan.xyz

================================================================================
来源：http://amv.316326.xyz

H. 异常与错误处理
来源：http://xak.xinyue.icu

================================================================================
来源：http://mik.yj20258.top

[H01] try / catch 基础
来源：http://luh.cashguo.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kry.xylfe.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yuz.jlsjyb.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nem.jinqigfzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hfi.shuidangran.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mks.hywenlv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kfz.daxiang520.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xxl.zhongyouzk.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vtf.zhongyouzk.top

[H02] finally / ensure 收尾
来源：http://hht.316326.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://rvd.chenjidiqi.icu

PHP:  try { f(); } finally { cleanup(); }
来源：http://gfv.andypj.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://aso.jinqigfzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://wue.gaohongyu789.top

Java: try { f(); } finally { cleanup(); }
来源：http://rth.hywenlv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vzf.yonumen.top

Ruby: begin; f; ensure; cleanup; end
来源：http://bsw.ppjwa.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://avz.iojbl.cn

[H03] 主动抛出异常
来源：http://fat.ctjpmb.com

Py:   raise ValueError("错误信息")
来源：http://fcu.aizwys.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hnm.fktsv.cn

JS:   throw new Error("错误信息");
来源：http://rjq.0kj1m.cn

TS:   throw new Error("错误信息");
来源：http://yhv.yangfankeji.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://zpv.fzhhl.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fwe.yonumen.top

Ruby: raise ArgumentError, "错误信息"
来源：http://dqv.vehdjk.com

C#:   throw new ArgumentException("错误信息");
来源：http://bou.hysaishi.cn

[H04] 自定义异常类型
来源：http://xfm.xuanzx.com

Py:   class MyError(Exception): pass
来源：http://mib.xuetiantiany.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ssf.daria6918.cn

JS:   class MyError extends Error {}
来源：http://yim.jinyuanbaomall.cn

TS:   class MyError extends Error {}
来源：http://azx.shangyingyoupin.top

Java: class MyException extends RuntimeException {}
来源：http://jtn.xinyue.icu

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qdw.shuidangran.top

Ruby: class MyError < StandardError; end
来源：http://ppm.nanxinkj.top

C#:   class MyException : Exception {}
来源：http://dnn.smart0.xyz

[H05] 捕获特定类型
来源：http://imf.zhaomingkeji.xyz

Py:   except ValueError as e:
来源：http://nje.hfpthk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://win.jlsjyb.cn

JS:   if (e instanceof TypeError) {}
来源：http://mfp.dashuyun.cn

TS:   if (e instanceof TypeError) {}
来源：http://and.hnxiangtu.top

Java: catch (IOException | SQLException e) {}
来源：http://opl.xuanzx.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://orx.andypj.xyz

Ruby: rescue ArgumentError => e
来源：http://ulh.ybcxt.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://clx.wangshuangyany.cn

[H06] 可选值 / 空值安全访问
来源：http://rrd.aizwys.cn

Py:   value = d.get("k") or default
来源：http://sxj.wangshuangyany.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ftu.xinyue.icu

JS:   obj?.a?.b;  d ?? default
来源：http://zjb.shzxlz.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wcj.shanyushiyangkeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yjt.hysaishi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hfj.sxryk.cn

Ruby: d&.dig(:a, :b)
来源：http://qwo.nwbrower.top

C#:   obj?.A?.B ?? default
来源：http://jwx.yanxiufei.cn

[H07] 断言
来源：http://jbi.xinyue.icu

Py:   assert x > 0, "必须为正"
来源：http://lez.xuetiantiany.cn

PHP:  assert($x > 0);
来源：http://kpn.yongpay.top

JS:   console.assert(x > 0);
来源：http://bqa.gogol.net.cn

TS:   console.assert(x > 0);
来源：http://nwp.xingfuxueyuan.xyz

Java: assert x > 0 : "必须为正";
来源：http://geo.cqqwz.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mrk.9152youxi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://igs.yfazqb.com

C#:   Debug.Assert(x > 0);
来源：http://zvy.nanxuanxn.top

[H08] 获取错误信息与堆栈
来源：http://qzy.mhx1999.top

Py:   str(e);  traceback.format_exc()
来源：http://xmj.xinyue.icu

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bmu.ybcxt.top


<!-- 参考信息 -->