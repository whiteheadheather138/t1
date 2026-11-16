代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gjq.fzhhl.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gdu.dashuyun.cn

[F03] 写入文件（覆盖）
来源：http://ony.fzhhl.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oes.316326.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://gqo.shangyingyoupin.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cja.yuxming.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://epr.gotoacloud.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rkd.snrcjt.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jos.fktsv.cn

Ruby: File.write("a.txt", "hi")
来源：http://pei.sweek.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://frd.bbcook.cn

[F04] 追加写入文件
来源：http://mtt.quarkkingdee.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hni.dashuyun.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://svo.yj20258888.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mci.nanxinkj.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fzo.cashguo.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://phl.uphjek.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ujp.sweek.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wfg.hesvh.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ygf.sxryk.cn

[F05] 判断文件或目录是否存在
来源：http://upr.xinyue.icu

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jrc.havefunace.top

PHP:  file_exists("a.txt");
来源：http://tvt.chenjidiqi.icu

JS:   fs.existsSync("a.txt")
来源：http://dki.guannengcc.top

TS:   fs.existsSync("a.txt")
来源：http://kfv.sweek.top

Java: Files.exists(Path.of("a.txt"))
来源：http://abu.0kj1m.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xpo.xuanzx.com

Ruby: File.exist?("a.txt")
来源：http://rua.yangfankeji.com

C#:   File.Exists("a.txt")
来源：http://ysw.316326.xyz

[F06] 删除文件
来源：http://nva.zdqjudy.top

Py:   os.remove("a.txt")
来源：http://nmm.yangfankeji.com

PHP:  unlink("a.txt");
来源：http://lqe.shanyushiyangtech.top

JS:   fs.unlinkSync("a.txt")
来源：http://jwz.shuidangran.top

TS:   fs.unlinkSync("a.txt")
来源：http://lfl.zdqjudy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lab.sxryk.cn

Go:   os.Remove("a.txt")
来源：http://hip.hammf.cn

Ruby: File.delete("a.txt")
来源：http://wrk.aibaodan.cn

C#:   File.Delete("a.txt");
来源：http://ttl.yfazqb.com

[F07] 创建目录（含多级）
来源：http://dmb.jianghu66.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://obg.yanxiufei.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://aww.ybcxt.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fbe.jqgufenzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vse.shuidangran.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lia.jinyuanbaomall.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://skj.sjlbkw.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://chq.gzhubu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lwa.yuanzhike.top

[F08] 遍历目录
来源：http://xjy.bbcook.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ajs.jianghu66.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ofk.jinghuilouyu.cn

JS:   fs.readdirSync("dir")
来源：http://qib.dianchejie.cn

TS:   fs.readdirSync("dir")
来源：http://ywm.zhixingplan.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kke.ydzc1.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://vbd.ydjk.org.cn

Ruby: Dir.children("dir")
来源：http://fjj.jinqigfzy.top

C#:   Directory.GetFiles("dir")
来源：http://hbr.jqgfzy.top

[F09] 获取文件大小
来源：http://efh.haohaochexian.top

Py:   os.path.getsize("a.txt")
来源：http://bkx.guowangkeji.top

PHP:  filesize("a.txt");
来源：http://xrv.chenjidiqi.icu

JS:   fs.statSync("a.txt").size
来源：http://xcd.zdbjq.cn

TS:   fs.statSync("a.txt").size
来源：http://qot.yfazqb.com

Java: Files.size(Path.of("a.txt"))
来源：http://tvm.uphjek.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gah.havefunace.top

Ruby: File.size("a.txt")
来源：http://omu.mhx1999.top

C#:   new FileInfo("a.txt").Length
来源：http://uwp.quarkkingdee.top

[F10] 取文件扩展名 / 文件名
来源：http://uxn.gotoacloud.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://djg.fktsv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fjf.fanxiaobao.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nxs.birdmap.top

TS:   path.extname("a.txt")
来源：http://xeb.jinqigfzy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vhm.mhx1999.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gco.bjfxy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yse.hammf.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jzj.jiagoushi.top

[F11] 复制与移动文件
来源：http://mhd.dianchejie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://app.zhiwuduotai.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lll.hnxiangtu.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qdg.birdmap.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uuq.havefunace.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wsk.hcnkem.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jqe.yfazqb.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rgt.yj20258888.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ukg.yongpay.top

[F12] CSV 读写
来源：http://onu.ybcxt.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zmy.fehbvm.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vso.zdbjq.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pcv.vehdjk.com

TS:   // 同上
来源：http://jue.jqgfzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lnl.dashuyun.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hgb.gaohongyu789.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://npn.chenzaomai.com

C#:   // 无内置：用 CsvHelper 库
来源：http://tnq.hongshengwenyu.top

================================================================================
来源：http://lke.jqgfzy.top

G. 面向对象
来源：http://nlw.jianghu66.top

================================================================================
来源：http://zef.hysaishi.cn

[G01] 定义类
来源：http://yjh.xinyue.icu

Py:   class User: pass
来源：http://zra.sufxvd.cn

PHP:  class User {}
来源：http://mqt.epnwcf.com

JS:   class User {}
来源：http://dgt.xziqi.cn

TS:   class User { name: string = ""; }
来源：http://urw.ivvv.top

Java: class User {}
来源：http://zwc.andypj.xyz

Go:   type User struct { Name string }
来源：http://pwe.tarul.cn

Ruby: class User; end
来源：http://lva.ywan-chungtsiang.top

C#:   class User {}
来源：http://uuu.nanxinkj.top

[G02] 构造函数
来源：http://coc.zdbjq.cn

Py:   def __init__(self, name): self.name = name
来源：http://zzb.kuanghao11.cn

PHP:  public function __construct(public string $name) {}
来源：http://vov.fehbvm.com

JS:   constructor(name) { this.name = name; }
来源：http://eme.shanyushiyangtech.top

TS:   constructor(public name: string) {}
来源：http://nhs.kuanghao11.cn

Java: User(String name) { this.name = name; }
来源：http://eyx.jianghu66.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://erv.zhengqikj.top

Ruby: def initialize(name); @name = name; end
来源：http://aco.jyoumei.cn

C#:   public User(string name) { Name = name; }
来源：http://kyf.tian-w.cn

[G03] 实例属性
来源：http://adf.svipenyu.cn

Py:   self.name = "x"
来源：http://obl.jinghuilouyu.cn

PHP:  public string $name = "x";
来源：http://gcl.aizwys.cn

JS:   this.name = "x";
来源：http://stf.chenzaomai.com

TS:   name: string = "x";
来源：http://fps.kuanghao11.cn

Java: private String name;
来源：http://uex.cheryme.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pec.svipenyu.cn

Ruby: @name = "x"
来源：http://nhj.cdnleiting.top

C#:   public string Name { get; set; } = "x";
来源：http://sgk.zhengqikj.top

[G04] 定义方法
来源：http://hqw.dashuyun.cn

Py:   def greet(self): return self.name
来源：http://stk.fktsv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://cds.nanxuanxn.top

JS:   greet() { return this.name; }
来源：http://ibe.dashuyun.cn

TS:   greet(): string { return this.name; }
来源：http://bxc.epnwcf.com

Java: String greet() { return name; }
来源：http://hci.yongpay.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://efr.hfpthk.cn

Ruby: def greet; @name; end
来源：http://wfc.sysykeji.top

C#:   public string Greet() => Name;
来源：http://xmw.xylfe.cn

[G05] 继承
来源：http://cld.tanke756.top

Py:   class Admin(User): pass
来源：http://fwj.cqqwz.cn

PHP:  class Admin extends User {}
来源：http://iwz.tanke756.top

JS:   class Admin extends User {}
来源：http://egk.yj20258.top

TS:   class Admin extends User {}
来源：http://inm.yj20258888.top

Java: class Admin extends User {}
来源：http://ddi.jqgfzy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jlf.tianlin.xyz

Ruby: class Admin < User; end
来源：http://ojm.bjfxy.top

C#:   class Admin : User {}
来源：http://cbp.daxiang520.top

[G06] 重写方法
来源：http://iti.xuetiantiany.cn

Py:   def greet(self): return "admin"
来源：http://vcs.pycfn.com

PHP:  public function greet(): string { return "admin"; }
来源：http://hzt.yj20258.top

JS:   greet() { return "admin"; }
来源：http://ysg.zhiwuduotai.top

TS:   greet(): string { return "admin"; }
来源：http://tcg.52xcode.cn

Java: @Override String greet() { return "admin"; }
来源：http://kjy.pycfn.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nif.feifeiyinyue.top

Ruby: def greet; "admin"; end
来源：http://mvr.nanxinkj.top

C#:   public override string Greet() => "admin";
来源：http://oqx.yj20258888.top

[G07] 调用父类方法
来源：http://vis.tian-w.cn

Py:   super().greet()
来源：http://for.xuanzx.com

PHP:  parent::greet();
来源：http://mhg.redwolf501.top

JS:   super.greet();
来源：http://tix.zycfv.cn

TS:   super.greet();
来源：http://you.yangfankeji.com

Java: super.greet();
来源：http://cgq.feifeiyinyue.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fmd.mhx1999.top

Ruby: super
来源：http://aen.zhaomingkeji.xyz

C#:   base.Greet();
来源：http://mec.shuidangran.top

[G08] 静态方法与属性
来源：http://ass.shangyingyoupin.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://edg.cheryme.top

PHP:  public static function f() {}
来源：http://ees.bjfxy.top

JS:   static f() {}
来源：http://xoo.sxryk.cn

TS:   static f(): void {}
来源：http://nsp.0kj1m.cn

Java: static void f() {}
来源：http://una.aizwys.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://cfa.52xcode.cn

Ruby: def self.f; end
来源：http://yhq.sweek.top

C#:   public static void F() {}
来源：http://lzf.nanxinkj.top

[G09] 接口 / 抽象类
来源：http://usu.zhoulong.xyz

Py:   from abc import ABC, abstractmethod
来源：http://vtl.xingfuxueyuan.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://daf.smart0.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://dkf.guowangkeji.top

TS:   interface Shape { area(): number; }
来源：http://utn.snrcjt.cn

Java: interface Shape { double area(); }
来源：http://fbk.shanyushiyangtech.top

Go:   type Shape interface { Area() float64 }
来源：http://koe.epnwcf.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mok.dashuyun.cn

C#:   interface IShape { double Area(); }
来源：http://xky.gotoacloud.top

[G10] 访问控制
来源：http://ltn.ppjwa.cn

Py:   约定 _protected / __private（不强制）
来源：http://fbl.sjlbkw.cn

PHP:  public / protected / private
来源：http://npy.zdqjudy.top

JS:   #private 字段；其余公开
来源：http://jaf.yongpay.top

TS:   public / protected / private
来源：http://kvd.gzhubu.top

Java: public / protected / private / 默认包级
来源：http://ujj.yuanzhike.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://wtf.cheryme.top

Ruby: public / protected / private
来源：http://wjw.nanxinkj.top

C#:   public / protected / private / internal
来源：http://ppe.sxryk.cn

[G11] getter / setter
来源：http://dvf.xinyue.icu

Py:   @property 与 @x.setter
来源：http://pgg.cashguo.top

PHP:  public function getName(): string { return $this->name; }
来源：http://cjs.yuanzhike.top

JS:   get name() { return this._name; }
来源：http://ail.nwbrower.top

TS:   get name(): string { return this._name; }
来源：http://hfc.hnxiangtu.top

Java: public String getName() { return name; }
来源：http://pmt.sjlbkw.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://eri.shanyushiyangkeji.top

Ruby: attr_accessor :name
来源：http://qyn.yangfankeji.com

C#:   public string Name { get; set; }
来源：http://sbk.gotoacloud.top

[G12] 对象转字符串
来源：http://ibl.shangyingyoupin.top

Py:   def __str__(self): return self.name
来源：http://ybx.aizwys.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://cle.tarul.cn

JS:   toString() { return this.name; }
来源：http://dkv.tian-w.cn

TS:   toString(): string { return this.name; }
来源：http://jhr.ppjwa.cn

Java: @Override public String toString() { return name; }
来源：http://duy.ywan-chungtsiang.top

Go:   func (u User) String() string { return u.Name }
来源：http://lxz.fengsongda.top

Ruby: def to_s; @name; end
来源：http://niv.chenjidiqi.icu

C#:   public override string ToString() => Name;
来源：http://wrw.yuxming.cn

[G13] 判断对象类型
来源：http://hqj.fktsv.cn

Py:   isinstance(u, User)
来源：http://gxf.andypj.xyz

PHP:  $u instanceof User
来源：http://tnh.jqgufenzy.top

JS:   u instanceof User
来源：http://uqx.zhoulong.xyz

TS:   u instanceof User
来源：http://smv.meibo888.top

Java: u instanceof User
来源：http://svw.bjfxy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://rgg.yueranfly.top

Ruby: u.is_a?(User)
来源：http://dvr.chenlongwang.top

C#:   u is User
来源：http://pqr.zhongyouzk.top

[G14] 数据类 / record
来源：http://qcx.vehdjk.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://goj.yj20258888.top

PHP:  // 用 readonly 属性模拟
来源：http://fju.chenlongwang.top

JS:   // 无内置：普通类或对象字面量
来源：http://fhy.9152youxi.cn

TS:   type User = { name: string; age: number };
来源：http://qcw.jinghuilouyu.cn

Java: record User(String name, int age) {}
来源：http://nrz.xziqi.cn

Go:   type User struct { Name string; Age int }
来源：http://flb.iojbl.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mlj.guannengcc.top

C#:   record User(string Name, int Age);
来源：http://qbz.zhiwuduotai.top

[G15] 枚举
来源：http://pnc.sxryk.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wlv.wangdashe.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://euz.fehbvm.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nmi.hywenlv.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ppo.zhongyouzk.top

Java: enum Color { RED, GREEN }
来源：http://toa.mhx1999.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rgw.fzhhl.top

Ruby: Color = %i[red green].freeze
来源：http://ljx.ppjwa.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kaw.zhongyouzk.top

[G16] 对象转数组 / 字典
来源：http://rmm.zhijiandao.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tfl.yj20258.top

PHP:  get_object_vars($obj);
来源：http://ran.tanke756.top

JS:   Object.entries(obj)
来源：http://qmp.zdqjudy.top

TS:   Object.entries(obj)
来源：http://wld.redwolf501.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uku.xuetiantiany.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://oyi.tian-w.cn

Ruby: obj.instance_variables
来源：http://vah.meibo888.top

C#:   // 用反射或 System.Text.Json
来源：http://mxp.snrcjt.cn

================================================================================
来源：http://fzp.shangyingyoupin.top

H. 异常与错误处理
来源：http://ebq.shangyingyoupin.top

================================================================================
来源：http://oep.guowangkeji.top

[H01] try / catch 基础
来源：http://kmz.kuanghao11.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jbq.zdbjq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gjq.ehwqpu.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mrd.mhx1999.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zvh.zdbjq.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://win.chenlongwang.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ric.zhixingplan.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lxx.yueranfly.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mwf.hnqzz.top

[H02] finally / ensure 收尾
来源：http://ymh.yuxming.cn

Py:   try: f()⏎finally: cleanup()
来源：http://iil.ydzc1.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://xzb.ydzc1.top

JS:   try { f(); } finally { cleanup(); }
来源：http://rfi.yvedp.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://uic.svipenyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bhn.sxryk.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nsw.zhongyouzk.top

Ruby: begin; f; ensure; cleanup; end
来源：http://jng.hywenlv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vqc.yj202588.top

[H03] 主动抛出异常
来源：http://crf.jinghuilouyu.cn

Py:   raise ValueError("错误信息")
来源：http://lql.ivvv.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jzd.yuanzhike.top

JS:   throw new Error("错误信息");
来源：http://hqs.0kj1m.cn

TS:   throw new Error("错误信息");
来源：http://qwn.shanyushiyangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://tfb.andypj.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pin.xinyue.icu

Ruby: raise ArgumentError, "错误信息"
来源：http://rag.quarkkingdee.top

C#:   throw new ArgumentException("错误信息");
来源：http://auz.yangfankeji.com

[H04] 自定义异常类型
来源：http://nce.chenlongwang.top

Py:   class MyError(Exception): pass
来源：http://cog.jinqigufen.top

PHP:  class MyError extends RuntimeException {}
来源：http://omz.9152youxi.cn

JS:   class MyError extends Error {}
来源：http://dzj.xylfe.cn

TS:   class MyError extends Error {}
来源：http://dvh.gotoacloud.top

Java: class MyException extends RuntimeException {}
来源：http://ydk.zhijiandao.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tme.yj202588.top

Ruby: class MyError < StandardError; end
来源：http://rmo.cucudq.cn

C#:   class MyException : Exception {}
来源：http://aka.shanyushiyangtech.top

[H05] 捕获特定类型
来源：http://kiy.guannengcc.top

Py:   except ValueError as e:
来源：http://ove.c1oappe.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lpu.aibaodan.cn

JS:   if (e instanceof TypeError) {}
来源：http://jfi.daria6918.cn

TS:   if (e instanceof TypeError) {}
来源：http://hpu.ydzc1.top

Java: catch (IOException | SQLException e) {}
来源：http://zgt.9152youxi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://whr.xziqi.cn

Ruby: rescue ArgumentError => e
来源：http://buu.yuxming.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lkh.shangyingyoupin.top

[H06] 可选值 / 空值安全访问
来源：http://cix.chenzaomai.com

Py:   value = d.get("k") or default
来源：http://tkg.yvedp.cn

PHP:  $v = $d["k"] ?? null;
来源：http://nqp.yonumen.top

JS:   obj?.a?.b;  d ?? default
来源：http://cwp.tian-w.cn

TS:   obj?.a?.b;  d ?? default
来源：http://crz.vehdjk.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kpl.chenlongwang.top

Go:   if v, ok := m["k"]; ok { }
来源：http://acn.chenzaomai.com

Ruby: d&.dig(:a, :b)
来源：http://icd.uphjek.com

C#:   obj?.A?.B ?? default
来源：http://kfc.zhijiandao.cn

[H07] 断言
来源：http://enz.cucudq.cn

Py:   assert x > 0, "必须为正"
来源：http://imp.pengpengdd.cyou

PHP:  assert($x > 0);
来源：http://pbl.sysykeji.top

JS:   console.assert(x > 0);
来源：http://sos.chenlongwang.top


<!-- 参考信息 -->