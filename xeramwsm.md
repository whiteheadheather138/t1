代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ffz.sweek.top

Ruby: File.write("a.txt", "hi")
来源：http://rpi.zhongyouzk.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vwm.yanxiufei.cn

[F04] 追加写入文件
来源：http://jxh.yueranfly.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://eog.nwbrower.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sgp.bjfxy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pgh.gotoacloud.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tmp.jqgufenzy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uxh.hesvh.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lhs.jinghuilouyu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ibj.xylfe.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jic.0kj1m.cn

[F05] 判断文件或目录是否存在
来源：http://nxw.zhongyouzk.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qls.zhongyouzk.top

PHP:  file_exists("a.txt");
来源：http://wug.pycfn.com

JS:   fs.existsSync("a.txt")
来源：http://zfv.shangyingyoupin.top

TS:   fs.existsSync("a.txt")
来源：http://hpr.cheryme.top

Java: Files.exists(Path.of("a.txt"))
来源：http://wsv.hesvh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://epu.sxryk.cn

Ruby: File.exist?("a.txt")
来源：http://bwl.yongpay.top

C#:   File.Exists("a.txt")
来源：http://wna.sweek.top

[F06] 删除文件
来源：http://ksj.c1oappe.top

Py:   os.remove("a.txt")
来源：http://tho.cashguo.top

PHP:  unlink("a.txt");
来源：http://prg.yangfankeji.com

JS:   fs.unlinkSync("a.txt")
来源：http://ljw.hysaishi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hqj.cdnleiting.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tqh.hfpthk.cn

Go:   os.Remove("a.txt")
来源：http://ovp.sjlbkw.cn

Ruby: File.delete("a.txt")
来源：http://rvn.jinghuilouyu.cn

C#:   File.Delete("a.txt");
来源：http://sau.xuetiantiany.cn

[F07] 创建目录（含多级）
来源：http://vfh.cucudq.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hsx.fktsv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vvx.cucudq.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kwu.daria6918.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ejj.yj202588.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ukw.cashguo.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hqe.shanyushiyangkeji.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dvy.yuanzhike.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jia.hysaishi.cn

[F08] 遍历目录
来源：http://fdg.sysykeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xcx.jinghuilouyu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://otr.fktsv.cn

JS:   fs.readdirSync("dir")
来源：http://ptf.jianghu66.top

TS:   fs.readdirSync("dir")
来源：http://zgs.kuanghao11.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lff.haohaochexian.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ehd.yongpay.top

Ruby: Dir.children("dir")
来源：http://hkm.jiagoushi.top

C#:   Directory.GetFiles("dir")
来源：http://afb.hesvh.cn

[F09] 获取文件大小
来源：http://vcs.bjfxy.top

Py:   os.path.getsize("a.txt")
来源：http://zgi.guowangkeji.top

PHP:  filesize("a.txt");
来源：http://eka.ivvv.top

JS:   fs.statSync("a.txt").size
来源：http://mot.shzxlz.cn

TS:   fs.statSync("a.txt").size
来源：http://wyc.sxryk.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hwd.fktsv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pap.zycfv.cn

Ruby: File.size("a.txt")
来源：http://pta.sjlbkw.cn

C#:   new FileInfo("a.txt").Length
来源：http://fox.zdbjq.cn

[F10] 取文件扩展名 / 文件名
来源：http://cvl.nwbrower.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://orp.cheryme.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uck.birdmap.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rkq.zhaomingkeji.xyz

TS:   path.extname("a.txt")
来源：http://kyb.redwolf501.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://osj.zdqjudy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nko.mhx1999.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rox.fehbvm.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dtz.hnqzz.top

[F11] 复制与移动文件
来源：http://qgu.ctjpmb.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ihy.jyoumei.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://khw.jianghu66.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tiv.chenlongwang.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wdp.nanxinkj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rsn.xinyue.icu

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://aea.andypj.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rth.haohaochexian.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wuj.jinqigufen.top

[F12] CSV 读写
来源：http://bgm.sufxvd.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zii.daxiang520.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uql.hywenlv.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rdy.xuetiantiany.cn

TS:   // 同上
来源：http://cdj.hcnkem.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://aoo.ydjk.org.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vsc.wangdashe.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jhs.fktsv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gtr.vehdjk.com

================================================================================
来源：http://sip.guowangkeji.top

G. 面向对象
来源：http://gpa.shangyingyoupin.top

================================================================================
来源：http://hrz.fanxiaobao.xyz

[G01] 定义类
来源：http://qvt.bjfxy.top

Py:   class User: pass
来源：http://cxd.dianchejie.cn

PHP:  class User {}
来源：http://qsn.fanxiaobao.xyz

JS:   class User {}
来源：http://tbk.cucudq.cn

TS:   class User { name: string = ""; }
来源：http://qtx.jianghu66.top

Java: class User {}
来源：http://vfu.ybcxt.top

Go:   type User struct { Name string }
来源：http://rdu.xingfuxueyuan.xyz

Ruby: class User; end
来源：http://yuq.cdnleiting.top

C#:   class User {}
来源：http://wuu.gaohongyu789.top

[G02] 构造函数
来源：http://kfn.dianchejie.cn

Py:   def __init__(self, name): self.name = name
来源：http://wkn.cashguo.top

PHP:  public function __construct(public string $name) {}
来源：http://gvm.316326.xyz

JS:   constructor(name) { this.name = name; }
来源：http://hil.sjlbkw.cn

TS:   constructor(public name: string) {}
来源：http://xnl.ppjwa.cn

Java: User(String name) { this.name = name; }
来源：http://mxu.jinqigufen.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xqa.hesvh.cn

Ruby: def initialize(name); @name = name; end
来源：http://qzy.gzhubu.top

C#:   public User(string name) { Name = name; }
来源：http://kmp.nanxinkj.top

[G03] 实例属性
来源：http://jut.bjfxy.top

Py:   self.name = "x"
来源：http://qgt.ctjpmb.com

PHP:  public string $name = "x";
来源：http://eas.zdqjudy.top

JS:   this.name = "x";
来源：http://aim.jinqigfzy.top

TS:   name: string = "x";
来源：http://pru.zdbjq.cn

Java: private String name;
来源：http://qxq.gotoacloud.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kfm.dianchejie.cn

Ruby: @name = "x"
来源：http://orb.sysykeji.top

C#:   public string Name { get; set; } = "x";
来源：http://wxd.fehbvm.com

[G04] 定义方法
来源：http://mur.52xcode.cn

Py:   def greet(self): return self.name
来源：http://oed.pengpengdd.cyou

PHP:  public function greet(): string { return $this->name; }
来源：http://xgr.chenzaomai.com

JS:   greet() { return this.name; }
来源：http://ill.yj202588.top

TS:   greet(): string { return this.name; }
来源：http://ahg.yueranfly.top

Java: String greet() { return name; }
来源：http://xvh.zhongyouzk.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://djo.cdnleiting.top

Ruby: def greet; @name; end
来源：http://xbp.uphjek.com

C#:   public string Greet() => Name;
来源：http://bek.gogol.net.cn

[G05] 继承
来源：http://ndf.jinyuanbaomall.cn

Py:   class Admin(User): pass
来源：http://tps.sufxvd.cn

PHP:  class Admin extends User {}
来源：http://gli.tianlin.xyz

JS:   class Admin extends User {}
来源：http://icu.jinghuilouyu.cn

TS:   class Admin extends User {}
来源：http://vhl.0kj1m.cn

Java: class Admin extends User {}
来源：http://oln.yj20258888.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cuo.daria6918.cn

Ruby: class Admin < User; end
来源：http://sal.daxiang520.top

C#:   class Admin : User {}
来源：http://jht.ctjpmb.com

[G06] 重写方法
来源：http://azt.guowangkeji.top

Py:   def greet(self): return "admin"
来源：http://bhp.zhongyouzk.top

PHP:  public function greet(): string { return "admin"; }
来源：http://pqt.yj20258.top

JS:   greet() { return "admin"; }
来源：http://sgs.sxryk.cn

TS:   greet(): string { return "admin"; }
来源：http://tyl.zdqjudy.top

Java: @Override String greet() { return "admin"; }
来源：http://ocq.zdqjudy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://abs.zhijiandao.cn

Ruby: def greet; "admin"; end
来源：http://kny.snrcjt.cn

C#:   public override string Greet() => "admin";
来源：http://nkf.cucudq.cn

[G07] 调用父类方法
来源：http://dbz.ivvv.top

Py:   super().greet()
来源：http://nta.dashuyun.cn

PHP:  parent::greet();
来源：http://bph.nanxinkj.top

JS:   super.greet();
来源：http://buj.mhx1999.top

TS:   super.greet();
来源：http://fqn.xinyue.icu

Java: super.greet();
来源：http://rae.jianghu66.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fcb.yuanzhike.top

Ruby: super
来源：http://dzi.yueranfly.top

C#:   base.Greet();
来源：http://nhb.cdnleiting.top

[G08] 静态方法与属性
来源：http://kkb.xingfuxueyuan.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dbp.quarkkingdee.top

PHP:  public static function f() {}
来源：http://ily.zhiwuduotai.top

JS:   static f() {}
来源：http://szg.jqgfzy.top

TS:   static f(): void {}
来源：http://hqo.wangshuangyany.cn

Java: static void f() {}
来源：http://pjd.gotoacloud.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://wlc.jqgfzy.top

Ruby: def self.f; end
来源：http://xkf.vehdjk.com

C#:   public static void F() {}
来源：http://uba.yj20258.top

[G09] 接口 / 抽象类
来源：http://sko.yuxming.cn

Py:   from abc import ABC, abstractmethod
来源：http://uot.epnwcf.com

PHP:  interface Shape { public function area(): float; }
来源：http://bme.yangfankeji.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://edz.sxryk.cn

TS:   interface Shape { area(): number; }
来源：http://yxt.redwolf501.top

Java: interface Shape { double area(); }
来源：http://uow.nwbrower.top

Go:   type Shape interface { Area() float64 }
来源：http://ndo.pengpengdd.cyou

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lxv.chenzaomai.com

C#:   interface IShape { double Area(); }
来源：http://vab.jianghu66.top

[G10] 访问控制
来源：http://sfq.yuanzhike.top

Py:   约定 _protected / __private（不强制）
来源：http://uql.zycfv.cn

PHP:  public / protected / private
来源：http://end.tianlin.xyz

JS:   #private 字段；其余公开
来源：http://chf.guannengcc.top

TS:   public / protected / private
来源：http://jvi.hnqzz.top

Java: public / protected / private / 默认包级
来源：http://nho.smart0.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://zap.dashuyun.cn

Ruby: public / protected / private
来源：http://zra.epnwcf.com

C#:   public / protected / private / internal
来源：http://ezn.birdmap.top

[G11] getter / setter
来源：http://pnd.bbcook.cn

Py:   @property 与 @x.setter
来源：http://rld.shangyingyoupin.top

PHP:  public function getName(): string { return $this->name; }
来源：http://poj.haohaochexian.top

JS:   get name() { return this._name; }
来源：http://wky.pycfn.com

TS:   get name(): string { return this._name; }
来源：http://btg.cashguo.top

Java: public String getName() { return name; }
来源：http://yrm.cdnleiting.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://sao.zhengqikj.top

Ruby: attr_accessor :name
来源：http://zol.tian-w.cn

C#:   public string Name { get; set; }
来源：http://snb.yanxiufei.cn

[G12] 对象转字符串
来源：http://sge.sweek.top

Py:   def __str__(self): return self.name
来源：http://bwl.snrcjt.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hli.bjfxy.top

JS:   toString() { return this.name; }
来源：http://lwo.9152youxi.cn

TS:   toString(): string { return this.name; }
来源：http://fmo.jinghuilouyu.cn

Java: @Override public String toString() { return name; }
来源：http://peh.gogol.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://clf.sweek.top

Ruby: def to_s; @name; end
来源：http://ndm.iojbl.cn

C#:   public override string ToString() => Name;
来源：http://jth.jinyuanbaomall.cn

[G13] 判断对象类型
来源：http://kvf.jiagoushi.top

Py:   isinstance(u, User)
来源：http://qfw.snrcjt.cn

PHP:  $u instanceof User
来源：http://krm.zhiwuduotai.top

JS:   u instanceof User
来源：http://rwb.jiagoushi.top

TS:   u instanceof User
来源：http://lfb.quarkkingdee.top

Java: u instanceof User
来源：http://ndr.guowangkeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://zcg.ppjwa.cn

Ruby: u.is_a?(User)
来源：http://awk.smart0.xyz

C#:   u is User
来源：http://inm.zhengqikj.top

[G14] 数据类 / record
来源：http://lut.xinyue.icu

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gya.jqgufenzy.top

PHP:  // 用 readonly 属性模拟
来源：http://glm.jqgfzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://fur.shanyushiyangkeji.top

TS:   type User = { name: string; age: number };
来源：http://keh.hcnkem.com

Java: record User(String name, int age) {}
来源：http://bnj.jlsjyb.cn

Go:   type User struct { Name string; Age int }
来源：http://xdy.gogol.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xwr.wangshuangyany.cn

C#:   record User(string Name, int Age);
来源：http://ayd.dashuyun.cn

[G15] 枚举
来源：http://nmq.zhixingplan.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rlf.haohaochexian.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://hvd.yuanzhike.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zcp.0kj1m.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wjy.cashguo.top

Java: enum Color { RED, GREEN }
来源：http://fms.hcnkem.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jqm.shzxlz.cn

Ruby: Color = %i[red green].freeze
来源：http://bzd.pycfn.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://apx.jlsjyb.cn

[G16] 对象转数组 / 字典
来源：http://aov.nanxinkj.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ugj.yj20258.top

PHP:  get_object_vars($obj);
来源：http://buw.bjfxy.top

JS:   Object.entries(obj)
来源：http://dpx.ydjk.org.cn

TS:   Object.entries(obj)
来源：http://bpg.feifeiyinyue.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tts.gaohongyu789.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://lug.sufxvd.cn

Ruby: obj.instance_variables
来源：http://onw.yuanzhike.top

C#:   // 用反射或 System.Text.Json
来源：http://rbe.xziqi.cn

================================================================================
来源：http://phr.jlsjyb.cn

H. 异常与错误处理
来源：http://ckt.tian-w.cn

================================================================================
来源：http://goq.svipenyu.cn

[H01] try / catch 基础
来源：http://naj.fanxiaobao.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://znj.ydzc1.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wej.9152youxi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://iod.hongshengwenyu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lyw.jinqigfzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bft.epnwcf.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mup.9152youxi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pyz.bbcook.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gfx.gaohongyu789.top

[H02] finally / ensure 收尾
来源：http://zeb.wangdashe.top

Py:   try: f()⏎finally: cleanup()
来源：http://ooi.shanyushiyangtech.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://yrp.cdnleiting.top

JS:   try { f(); } finally { cleanup(); }
来源：http://puk.ydjk.org.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ire.pengpengdd.cyou

Java: try { f(); } finally { cleanup(); }
来源：http://etg.nanxuanxn.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://fpp.yj20258.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ory.wangshuangyany.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ssn.ydzc1.top

[H03] 主动抛出异常
来源：http://lms.redwolf501.top

Py:   raise ValueError("错误信息")
来源：http://naf.hcnkem.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qep.ybcxt.top

JS:   throw new Error("错误信息");
来源：http://vxr.yj20258888.top

TS:   throw new Error("错误信息");
来源：http://eki.dianchejie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://skk.guowangkeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://smv.xziqi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://oss.yuanzhike.top

C#:   throw new ArgumentException("错误信息");
来源：http://oyi.ppjwa.cn

[H04] 自定义异常类型
来源：http://rmq.hesvh.cn

Py:   class MyError(Exception): pass
来源：http://axy.zhaomingkeji.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://bmv.shanyushiyangkeji.top

JS:   class MyError extends Error {}
来源：http://vep.jianghu66.top

TS:   class MyError extends Error {}
来源：http://ohm.daria6918.cn

Java: class MyException extends RuntimeException {}
来源：http://cpg.jinyuanbaomall.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bqt.pengpengdd.cyou

Ruby: class MyError < StandardError; end
来源：http://jwq.nanxinkj.top

C#:   class MyException : Exception {}
来源：http://cuh.yangfankeji.com

[H05] 捕获特定类型
来源：http://wbj.hcnkem.com

Py:   except ValueError as e:
来源：http://imc.meibo888.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jfh.bjfxy.top

JS:   if (e instanceof TypeError) {}
来源：http://fcc.tanke756.top

TS:   if (e instanceof TypeError) {}
来源：http://tau.yanxiufei.cn

Java: catch (IOException | SQLException e) {}
来源：http://vmt.jlsjyb.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mrg.xuetiantiany.cn

Ruby: rescue ArgumentError => e
来源：http://mjy.zycfv.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cqu.jyoumei.cn

[H06] 可选值 / 空值安全访问
来源：http://elb.xziqi.cn

Py:   value = d.get("k") or default
来源：http://hzr.ppjwa.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fiq.bbcook.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xkx.dianchejie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ufc.tarul.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dyq.wangdashe.top

Go:   if v, ok := m["k"]; ok { }
来源：http://eka.sysykeji.top

Ruby: d&.dig(:a, :b)
来源：http://lvi.iojbl.cn

C#:   obj?.A?.B ?? default
来源：http://pmb.hnxiangtu.top

[H07] 断言
来源：http://mzt.316326.xyz

Py:   assert x > 0, "必须为正"
来源：http://uvf.yangfankeji.com

PHP:  assert($x > 0);
来源：http://hhw.zdbjq.cn

JS:   console.assert(x > 0);
来源：http://qdy.zhoulong.xyz

TS:   console.assert(x > 0);
来源：http://ucn.cqqwz.cn

Java: assert x > 0 : "必须为正";
来源：http://nhx.tarul.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dsm.jqgfzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://gxe.daxiang520.top

C#:   Debug.Assert(x > 0);
来源：http://rsq.aibaodan.cn

[H08] 获取错误信息与堆栈
来源：http://oig.iojbl.cn

Py:   str(e);  traceback.format_exc()
来源：http://eod.ybcxt.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jhz.fzhhl.top


<!-- 参考信息 -->