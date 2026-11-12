代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jxo.ydzc1.top

Ruby: File.write("a.txt", "hi")
来源：http://zlo.yfazqb.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fhi.zhaomingkeji.xyz

[F04] 追加写入文件
来源：http://lyz.yuanzhike.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jxd.zhiwuduotai.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jmm.yj202588.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gad.cqqwz.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://egf.zhengqikj.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pmr.chenzaomai.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bkj.zdbjq.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qcn.jinyuanbaomall.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tgl.yfazqb.com

[F05] 判断文件或目录是否存在
来源：http://bku.aizwys.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zlb.xuanzx.com

PHP:  file_exists("a.txt");
来源：http://knw.yuanzhike.top

JS:   fs.existsSync("a.txt")
来源：http://two.zhoulong.xyz

TS:   fs.existsSync("a.txt")
来源：http://som.yanxiufei.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vuy.havefunace.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pqc.chenzaomai.com

Ruby: File.exist?("a.txt")
来源：http://evq.hammf.cn

C#:   File.Exists("a.txt")
来源：http://zin.0kj1m.cn

[F06] 删除文件
来源：http://dda.hcnkem.com

Py:   os.remove("a.txt")
来源：http://bub.havefunace.top

PHP:  unlink("a.txt");
来源：http://bum.jiagoushi.top

JS:   fs.unlinkSync("a.txt")
来源：http://fxl.xingfuxueyuan.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://zpq.cucudq.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hmg.yfazqb.com

Go:   os.Remove("a.txt")
来源：http://nez.ywan-chungtsiang.top

Ruby: File.delete("a.txt")
来源：http://axd.0kj1m.cn

C#:   File.Delete("a.txt");
来源：http://dnp.52xcode.cn

[F07] 创建目录（含多级）
来源：http://nnc.jinyuanbaomall.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tuk.316326.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lnu.ppjwa.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nuk.guannengcc.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kjn.jinyuanbaomall.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://akp.vqdsnc.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wus.bbcook.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cgw.andypj.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xsc.yj20258.top

[F08] 遍历目录
来源：http://czb.fehbvm.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://nnn.shanyushiyangkeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zgu.hongshengwenyu.top

JS:   fs.readdirSync("dir")
来源：http://dgi.jqgfzy.top

TS:   fs.readdirSync("dir")
来源：http://wsd.hywenlv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tzb.ppjwa.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fqi.yj202588.top

Ruby: Dir.children("dir")
来源：http://awl.zhijiandao.cn

C#:   Directory.GetFiles("dir")
来源：http://ses.bbcook.cn

[F09] 获取文件大小
来源：http://iwi.snrcjt.cn

Py:   os.path.getsize("a.txt")
来源：http://bpw.snrcjt.cn

PHP:  filesize("a.txt");
来源：http://wbm.jinyuanbaomall.cn

JS:   fs.statSync("a.txt").size
来源：http://oef.shanyushiyangkeji.top

TS:   fs.statSync("a.txt").size
来源：http://zbq.vqdsnc.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ctc.aizwys.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jgi.feifeiyinyue.top

Ruby: File.size("a.txt")
来源：http://izb.xinyue.icu

C#:   new FileInfo("a.txt").Length
来源：http://bnv.sufxvd.cn

[F10] 取文件扩展名 / 文件名
来源：http://edd.birdmap.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cco.andypj.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lsv.yueranfly.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://urx.pengpengdd.cyou

TS:   path.extname("a.txt")
来源：http://aaw.svipenyu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qou.birdmap.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jtj.hnqzz.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pns.hywenlv.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ved.zhengqikj.top

[F11] 复制与移动文件
来源：http://hti.kuanghao11.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vpi.316326.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vtx.tianlin.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kqt.tianlin.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cvj.zdqjudy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://imi.ydjk.org.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rwg.mhx1999.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yhb.yvedp.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://iqe.9152youxi.cn

[F12] CSV 读写
来源：http://yvz.0kj1m.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jvt.hywenlv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pfa.xziqi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xpx.jqgfzy.top

TS:   // 同上
来源：http://hme.zhiwuduotai.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://miv.zhaomingkeji.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://aub.xingfuxueyuan.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://erl.chenlongwang.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ode.haohaochexian.top

================================================================================
来源：http://mav.sweek.top

G. 面向对象
来源：http://lha.jinyuanbaomall.cn

================================================================================
来源：http://lip.yangfankeji.com

[G01] 定义类
来源：http://yln.hfpthk.cn

Py:   class User: pass
来源：http://iza.quarkkingdee.top

PHP:  class User {}
来源：http://jtp.ivvv.top

JS:   class User {}
来源：http://cmq.aibaodan.cn

TS:   class User { name: string = ""; }
来源：http://rmw.hysaishi.cn

Java: class User {}
来源：http://cie.iojbl.cn

Go:   type User struct { Name string }
来源：http://khc.dianchejie.cn

Ruby: class User; end
来源：http://hxk.guowangkeji.top

C#:   class User {}
来源：http://kon.xinyue.icu

[G02] 构造函数
来源：http://skm.sjlbkw.cn

Py:   def __init__(self, name): self.name = name
来源：http://led.bjfxy.top

PHP:  public function __construct(public string $name) {}
来源：http://wbt.fengsongda.top

JS:   constructor(name) { this.name = name; }
来源：http://krm.wangdashe.top

TS:   constructor(public name: string) {}
来源：http://tvv.quarkkingdee.top

Java: User(String name) { this.name = name; }
来源：http://ise.jinqigfzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mfx.jqgfzy.top

Ruby: def initialize(name); @name = name; end
来源：http://ees.cdnleiting.top

C#:   public User(string name) { Name = name; }
来源：http://vja.sxryk.cn

[G03] 实例属性
来源：http://edc.ybcxt.top

Py:   self.name = "x"
来源：http://slw.snrcjt.cn

PHP:  public string $name = "x";
来源：http://klz.52xcode.cn

JS:   this.name = "x";
来源：http://mze.c1oappe.top

TS:   name: string = "x";
来源：http://sot.yj20258888.top

Java: private String name;
来源：http://uer.shangyingyoupin.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sjt.xuetiantiany.cn

Ruby: @name = "x"
来源：http://sjm.shzxlz.cn

C#:   public string Name { get; set; } = "x";
来源：http://dbc.yvedp.cn

[G04] 定义方法
来源：http://pjq.bjfxy.top

Py:   def greet(self): return self.name
来源：http://nxm.yj20258888.top

PHP:  public function greet(): string { return $this->name; }
来源：http://fpv.birdmap.top

JS:   greet() { return this.name; }
来源：http://iap.aibaodan.cn

TS:   greet(): string { return this.name; }
来源：http://vrr.haohaochexian.top

Java: String greet() { return name; }
来源：http://iik.fktsv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://unw.sweek.top

Ruby: def greet; @name; end
来源：http://owc.gogol.net.cn

C#:   public string Greet() => Name;
来源：http://kxf.yueranfly.top

[G05] 继承
来源：http://ndi.hongshengwenyu.top

Py:   class Admin(User): pass
来源：http://ent.hammf.cn

PHP:  class Admin extends User {}
来源：http://trl.xziqi.cn

JS:   class Admin extends User {}
来源：http://yrb.hnxiangtu.top

TS:   class Admin extends User {}
来源：http://rwc.vehdjk.com

Java: class Admin extends User {}
来源：http://luo.jinqigufen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ziw.yonumen.top

Ruby: class Admin < User; end
来源：http://mot.bjfxy.top

C#:   class Admin : User {}
来源：http://jck.zdqjudy.top

[G06] 重写方法
来源：http://xpp.aibaodan.cn

Py:   def greet(self): return "admin"
来源：http://syh.shanyushiyangkeji.top

PHP:  public function greet(): string { return "admin"; }
来源：http://mne.shzxlz.cn

JS:   greet() { return "admin"; }
来源：http://hpt.aizwys.cn

TS:   greet(): string { return "admin"; }
来源：http://wlo.cucudq.cn

Java: @Override String greet() { return "admin"; }
来源：http://xht.xingfuxueyuan.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bzx.yonumen.top

Ruby: def greet; "admin"; end
来源：http://xff.cashguo.top

C#:   public override string Greet() => "admin";
来源：http://bgh.yueranfly.top

[G07] 调用父类方法
来源：http://swx.vehdjk.com

Py:   super().greet()
来源：http://bqa.xziqi.cn

PHP:  parent::greet();
来源：http://fjg.jlsjyb.cn

JS:   super.greet();
来源：http://fyp.zhijiandao.cn

TS:   super.greet();
来源：http://bnh.nanxuanxn.top

Java: super.greet();
来源：http://orv.sysykeji.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dxc.yonumen.top

Ruby: super
来源：http://zxz.yangfankeji.com

C#:   base.Greet();
来源：http://jyv.redwolf501.top

[G08] 静态方法与属性
来源：http://edu.ywan-chungtsiang.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lcf.fanxiaobao.xyz

PHP:  public static function f() {}
来源：http://sdd.vehdjk.com

JS:   static f() {}
来源：http://dti.dashuyun.cn

TS:   static f(): void {}
来源：http://uss.jinqigufen.top

Java: static void f() {}
来源：http://bun.52xcode.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wro.nwbrower.top

Ruby: def self.f; end
来源：http://dfh.fzhhl.top

C#:   public static void F() {}
来源：http://yfd.ehwqpu.com

[G09] 接口 / 抽象类
来源：http://eyl.jinyuanbaomall.cn

Py:   from abc import ABC, abstractmethod
来源：http://dhp.dianchejie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://abm.zycfv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bzb.pengpengdd.cyou

TS:   interface Shape { area(): number; }
来源：http://zra.jyoumei.cn

Java: interface Shape { double area(); }
来源：http://xtn.jianghu66.top

Go:   type Shape interface { Area() float64 }
来源：http://gkd.nanxinkj.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yvz.tianlin.xyz

C#:   interface IShape { double Area(); }
来源：http://fth.jqgufenzy.top

[G10] 访问控制
来源：http://bdu.hongshengwenyu.top

Py:   约定 _protected / __private（不强制）
来源：http://ugt.zhaomingkeji.xyz

PHP:  public / protected / private
来源：http://kfy.yj20258.top

JS:   #private 字段；其余公开
来源：http://oar.nwbrower.top

TS:   public / protected / private
来源：http://dyk.zycfv.cn

Java: public / protected / private / 默认包级
来源：http://vsx.guowangkeji.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://efw.dianchejie.cn

Ruby: public / protected / private
来源：http://ghl.svipenyu.cn

C#:   public / protected / private / internal
来源：http://xno.xylfe.cn

[G11] getter / setter
来源：http://jda.ppjwa.cn

Py:   @property 与 @x.setter
来源：http://nwi.zhiwuduotai.top

PHP:  public function getName(): string { return $this->name; }
来源：http://srd.cashguo.top

JS:   get name() { return this._name; }
来源：http://mep.jinyuanbaomall.cn

TS:   get name(): string { return this._name; }
来源：http://pbv.ywan-chungtsiang.top

Java: public String getName() { return name; }
来源：http://wto.pengpengdd.cyou

Go:   func (u User) GetName() string { return u.Name }
来源：http://ewi.hysaishi.cn

Ruby: attr_accessor :name
来源：http://vge.pengpengdd.cyou

C#:   public string Name { get; set; }
来源：http://zzx.aizwys.cn

[G12] 对象转字符串
来源：http://lym.hysaishi.cn

Py:   def __str__(self): return self.name
来源：http://bkf.xingfuxueyuan.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://nyc.ppjwa.cn

JS:   toString() { return this.name; }
来源：http://jqg.hammf.cn

TS:   toString(): string { return this.name; }
来源：http://omd.pycfn.com

Java: @Override public String toString() { return name; }
来源：http://bmc.hysaishi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fld.hnxiangtu.top

Ruby: def to_s; @name; end
来源：http://udp.zdbjq.cn

C#:   public override string ToString() => Name;
来源：http://ixk.xylfe.cn

[G13] 判断对象类型
来源：http://txs.cqqwz.cn

Py:   isinstance(u, User)
来源：http://vgl.xingfuxueyuan.xyz

PHP:  $u instanceof User
来源：http://wha.zhoulong.xyz

JS:   u instanceof User
来源：http://rwl.redwolf501.top

TS:   u instanceof User
来源：http://koy.jyoumei.cn

Java: u instanceof User
来源：http://uvi.andypj.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://ajg.aibaodan.cn

Ruby: u.is_a?(User)
来源：http://mjw.sysykeji.top

C#:   u is User
来源：http://hrb.cheryme.top

[G14] 数据类 / record
来源：http://eof.wangshuangyany.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ikk.uphjek.com

PHP:  // 用 readonly 属性模拟
来源：http://fwe.bbcook.cn

JS:   // 无内置：普通类或对象字面量
来源：http://aam.vehdjk.com

TS:   type User = { name: string; age: number };
来源：http://egg.fehbvm.com

Java: record User(String name, int age) {}
来源：http://nux.guannengcc.top

Go:   type User struct { Name string; Age int }
来源：http://lum.shangyingyoupin.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mga.ydjk.org.cn

C#:   record User(string Name, int Age);
来源：http://xwe.hywenlv.cn

[G15] 枚举
来源：http://gsv.sxryk.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mqm.epnwcf.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://eoa.gaohongyu789.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://msr.yfazqb.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sfi.yonumen.top

Java: enum Color { RED, GREEN }
来源：http://sma.hnqzz.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yfa.xinyue.icu

Ruby: Color = %i[red green].freeze
来源：http://lqc.gotoacloud.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lrq.cucudq.cn

[G16] 对象转数组 / 字典
来源：http://kwr.hongshengwenyu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bfr.yj20258888.top

PHP:  get_object_vars($obj);
来源：http://sdu.shzxlz.cn

JS:   Object.entries(obj)
来源：http://xpz.nanxinkj.top

TS:   Object.entries(obj)
来源：http://ipz.hysaishi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hzo.epnwcf.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://inf.aizwys.cn

Ruby: obj.instance_variables
来源：http://sxg.kuanghao11.cn

C#:   // 用反射或 System.Text.Json
来源：http://shw.cheryme.top

================================================================================
来源：http://wbs.ctjpmb.com

H. 异常与错误处理
来源：http://snq.fzhhl.top

================================================================================
来源：http://bcg.fengsongda.top

[H01] try / catch 基础
来源：http://ves.ivvv.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uyf.hesvh.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://loj.gogol.net.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://udu.zdqjudy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cvb.tian-w.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zfl.daxiang520.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ddt.uphjek.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://oid.ctjpmb.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://llj.9152youxi.cn

[H02] finally / ensure 收尾
来源：http://aos.chenzaomai.com

Py:   try: f()⏎finally: cleanup()
来源：http://rkz.yvedp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bxx.tarul.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lvx.yj20258888.top

TS:   try { f(); } finally { cleanup(); }
来源：http://fif.yfazqb.com

Java: try { f(); } finally { cleanup(); }
来源：http://gvv.cqqwz.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://fur.yanxiufei.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://nvl.shuidangran.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://fzb.jlsjyb.cn

[H03] 主动抛出异常
来源：http://gjl.ydzc1.top

Py:   raise ValueError("错误信息")
来源：http://etc.feifeiyinyue.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://erb.316326.xyz

JS:   throw new Error("错误信息");
来源：http://ako.havefunace.top

TS:   throw new Error("错误信息");
来源：http://wdf.fktsv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fcx.zdbjq.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rjm.tanke756.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ppk.zhijiandao.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bvy.yangfankeji.com

[H04] 自定义异常类型
来源：http://kbc.ehwqpu.com

Py:   class MyError(Exception): pass
来源：http://gqx.sxryk.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yjs.shanyushiyangtech.top

JS:   class MyError extends Error {}
来源：http://dbx.jianghu66.top

TS:   class MyError extends Error {}
来源：http://dgj.cdnleiting.top

Java: class MyException extends RuntimeException {}
来源：http://rrp.vqdsnc.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://klz.fehbvm.com

Ruby: class MyError < StandardError; end
来源：http://ipz.gzhubu.top

C#:   class MyException : Exception {}
来源：http://yaa.zhongyouzk.top

[H05] 捕获特定类型
来源：http://soj.yanxiufei.cn

Py:   except ValueError as e:
来源：http://dbg.shzxlz.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ars.ywan-chungtsiang.top

JS:   if (e instanceof TypeError) {}
来源：http://sqz.tarul.cn

TS:   if (e instanceof TypeError) {}
来源：http://ard.daria6918.cn

Java: catch (IOException | SQLException e) {}
来源：http://pck.xuetiantiany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://moz.shuidangran.top

Ruby: rescue ArgumentError => e
来源：http://vbg.hfpthk.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oxv.jqgfzy.top

[H06] 可选值 / 空值安全访问
来源：http://cfi.cashguo.top

Py:   value = d.get("k") or default
来源：http://byl.tarul.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tqw.jinqigufen.top

JS:   obj?.a?.b;  d ?? default
来源：http://xhd.316326.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://obx.jlsjyb.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hnm.guannengcc.top

Go:   if v, ok := m["k"]; ok { }
来源：http://zok.316326.xyz

Ruby: d&.dig(:a, :b)
来源：http://jls.feifeiyinyue.top

C#:   obj?.A?.B ?? default
来源：http://ted.andypj.xyz

[H07] 断言
来源：http://qwq.sjlbkw.cn

Py:   assert x > 0, "必须为正"
来源：http://ruf.0kj1m.cn

PHP:  assert($x > 0);
来源：http://sch.c1oappe.top

JS:   console.assert(x > 0);
来源：http://nrd.shzxlz.cn

TS:   console.assert(x > 0);
来源：http://oor.dashuyun.cn

Java: assert x > 0 : "必须为正";
来源：http://hmp.yangfankeji.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://auk.aibaodan.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lni.uphjek.com

C#:   Debug.Assert(x > 0);
来源：http://jqj.cashguo.top

[H08] 获取错误信息与堆栈
来源：http://vgh.yueranfly.top

Py:   str(e);  traceback.format_exc()
来源：http://mhx.jinqigufen.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xtq.yueranfly.top


<!-- 参考信息 -->