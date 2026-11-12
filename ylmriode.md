代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yit.hfpthk.cn

Ruby: File.write("a.txt", "hi")
来源：http://ygz.sysykeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://iag.jinyuanbaomall.cn

[F04] 追加写入文件
来源：http://hct.zhengqikj.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://aap.mhx1999.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://snb.birdmap.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hfh.52xcode.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ltv.vqdsnc.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rtm.xuetiantiany.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wvk.chenlongwang.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://asy.haohaochexian.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jlw.yvedp.cn

[F05] 判断文件或目录是否存在
来源：http://qgg.wangshuangyany.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://khl.xziqi.cn

PHP:  file_exists("a.txt");
来源：http://pqe.pengpengdd.cyou

JS:   fs.existsSync("a.txt")
来源：http://jmh.zycfv.cn

TS:   fs.existsSync("a.txt")
来源：http://jsn.zhaomingkeji.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://oqh.chenjidiqi.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://inf.hnqzz.top

Ruby: File.exist?("a.txt")
来源：http://hdq.hesvh.cn

C#:   File.Exists("a.txt")
来源：http://woy.yanxiufei.cn

[F06] 删除文件
来源：http://lsd.xuetiantiany.cn

Py:   os.remove("a.txt")
来源：http://uot.gotoacloud.top

PHP:  unlink("a.txt");
来源：http://mwe.316326.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://fuy.chenzaomai.com

TS:   fs.unlinkSync("a.txt")
来源：http://lrz.fktsv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gkp.sysykeji.top

Go:   os.Remove("a.txt")
来源：http://vqb.hesvh.cn

Ruby: File.delete("a.txt")
来源：http://iaq.chenlongwang.top

C#:   File.Delete("a.txt");
来源：http://anp.quarkkingdee.top

[F07] 创建目录（含多级）
来源：http://dkn.feifeiyinyue.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://oyq.guannengcc.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cwr.xziqi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jui.sxryk.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mfc.redwolf501.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bjz.quarkkingdee.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://quz.gaohongyu789.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zuq.bbcook.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kel.hysaishi.cn

[F08] 遍历目录
来源：http://ups.xuanzx.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://ezr.fengsongda.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://faf.9152youxi.cn

JS:   fs.readdirSync("dir")
来源：http://hza.jianghu66.top

TS:   fs.readdirSync("dir")
来源：http://jtt.yuanzhike.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fjc.gotoacloud.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://iqu.sxryk.cn

Ruby: Dir.children("dir")
来源：http://hcs.yfazqb.com

C#:   Directory.GetFiles("dir")
来源：http://mak.nwbrower.top

[F09] 获取文件大小
来源：http://ogk.hammf.cn

Py:   os.path.getsize("a.txt")
来源：http://jyi.dashuyun.cn

PHP:  filesize("a.txt");
来源：http://mae.kuanghao11.cn

JS:   fs.statSync("a.txt").size
来源：http://bqq.jiagoushi.top

TS:   fs.statSync("a.txt").size
来源：http://ckv.shanyushiyangkeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://kzi.c1oappe.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sui.zhixingplan.top

Ruby: File.size("a.txt")
来源：http://ouv.smart0.xyz

C#:   new FileInfo("a.txt").Length
来源：http://uad.chenjidiqi.icu

[F10] 取文件扩展名 / 文件名
来源：http://olk.chenzaomai.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xro.yongpay.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uch.hywenlv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pzi.jiagoushi.top

TS:   path.extname("a.txt")
来源：http://esi.jinyuanbaomall.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jja.birdmap.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bzv.kuanghao11.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://aaq.9152youxi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://roi.tianlin.xyz

[F11] 复制与移动文件
来源：http://eaf.vqdsnc.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hzk.yj20258.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tiu.hysaishi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cin.meibo888.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cnb.yonumen.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kdh.zhoulong.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ecx.cdnleiting.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jlr.jinyuanbaomall.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vda.vehdjk.com

[F12] CSV 读写
来源：http://cms.haohaochexian.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tuw.yj20258888.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qec.nanxuanxn.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ekn.yonumen.top

TS:   // 同上
来源：http://qmh.nanxuanxn.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dxq.sxryk.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rpk.zycfv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hzd.uphjek.com

C#:   // 无内置：用 CsvHelper 库
来源：http://npp.kuanghao11.cn

================================================================================
来源：http://ovo.svipenyu.cn

G. 面向对象
来源：http://irl.gaohongyu789.top

================================================================================
来源：http://wdi.aibaodan.cn

[G01] 定义类
来源：http://ims.zhiwuduotai.top

Py:   class User: pass
来源：http://ose.shzxlz.cn

PHP:  class User {}
来源：http://rpa.yvedp.cn

JS:   class User {}
来源：http://feq.9152youxi.cn

TS:   class User { name: string = ""; }
来源：http://niu.tanke756.top

Java: class User {}
来源：http://msy.jqgufenzy.top

Go:   type User struct { Name string }
来源：http://iwh.zhiwuduotai.top

Ruby: class User; end
来源：http://zrl.kuanghao11.cn

C#:   class User {}
来源：http://rrc.andypj.xyz

[G02] 构造函数
来源：http://xgt.daxiang520.top

Py:   def __init__(self, name): self.name = name
来源：http://fim.dianchejie.cn

PHP:  public function __construct(public string $name) {}
来源：http://oyp.fengsongda.top

JS:   constructor(name) { this.name = name; }
来源：http://dcw.shuidangran.top

TS:   constructor(public name: string) {}
来源：http://jue.zdqjudy.top

Java: User(String name) { this.name = name; }
来源：http://dgp.hfpthk.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zjv.cdnleiting.top

Ruby: def initialize(name); @name = name; end
来源：http://lio.9152youxi.cn

C#:   public User(string name) { Name = name; }
来源：http://amp.jinyuanbaomall.cn

[G03] 实例属性
来源：http://kxw.yanxiufei.cn

Py:   self.name = "x"
来源：http://qxx.gotoacloud.top

PHP:  public string $name = "x";
来源：http://uht.uphjek.com

JS:   this.name = "x";
来源：http://ndz.hnqzz.top

TS:   name: string = "x";
来源：http://hrg.daria6918.cn

Java: private String name;
来源：http://chm.shanyushiyangtech.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vpe.sweek.top

Ruby: @name = "x"
来源：http://lfv.ivvv.top

C#:   public string Name { get; set; } = "x";
来源：http://lst.jiagoushi.top

[G04] 定义方法
来源：http://ymn.yongpay.top

Py:   def greet(self): return self.name
来源：http://gid.sjlbkw.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nog.yanxiufei.cn

JS:   greet() { return this.name; }
来源：http://gof.c1oappe.top

TS:   greet(): string { return this.name; }
来源：http://oiv.vqdsnc.cn

Java: String greet() { return name; }
来源：http://hca.andypj.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://aeo.yuxming.cn

Ruby: def greet; @name; end
来源：http://uqz.shanyushiyangkeji.top

C#:   public string Greet() => Name;
来源：http://ygr.0kj1m.cn

[G05] 继承
来源：http://aby.wangshuangyany.cn

Py:   class Admin(User): pass
来源：http://rnj.hesvh.cn

PHP:  class Admin extends User {}
来源：http://yls.hfpthk.cn

JS:   class Admin extends User {}
来源：http://qnm.mhx1999.top

TS:   class Admin extends User {}
来源：http://qjs.yj20258888.top

Java: class Admin extends User {}
来源：http://xvq.ctjpmb.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fhr.yfazqb.com

Ruby: class Admin < User; end
来源：http://xoj.zdqjudy.top

C#:   class Admin : User {}
来源：http://sqh.hcnkem.com

[G06] 重写方法
来源：http://amq.mhx1999.top

Py:   def greet(self): return "admin"
来源：http://zrz.sweek.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ppz.zdbjq.cn

JS:   greet() { return "admin"; }
来源：http://ypz.hnqzz.top

TS:   greet(): string { return "admin"; }
来源：http://ria.yuxming.cn

Java: @Override String greet() { return "admin"; }
来源：http://mwj.cdnleiting.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sns.zdbjq.cn

Ruby: def greet; "admin"; end
来源：http://mbs.ctjpmb.com

C#:   public override string Greet() => "admin";
来源：http://rbc.sufxvd.cn

[G07] 调用父类方法
来源：http://lsm.ydzc1.top

Py:   super().greet()
来源：http://hix.shanyushiyangkeji.top

PHP:  parent::greet();
来源：http://bnz.zdqjudy.top

JS:   super.greet();
来源：http://qmf.sjlbkw.cn

TS:   super.greet();
来源：http://gey.mhx1999.top

Java: super.greet();
来源：http://vtc.quarkkingdee.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://aus.hfpthk.cn

Ruby: super
来源：http://zsg.yongpay.top

C#:   base.Greet();
来源：http://kjb.ehwqpu.com

[G08] 静态方法与属性
来源：http://tfn.yangfankeji.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rfk.feifeiyinyue.top

PHP:  public static function f() {}
来源：http://arc.yangfankeji.com

JS:   static f() {}
来源：http://hvx.zhongyouzk.top

TS:   static f(): void {}
来源：http://zze.0kj1m.cn

Java: static void f() {}
来源：http://xfn.cqqwz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xvj.shanyushiyangtech.top

Ruby: def self.f; end
来源：http://fuo.daria6918.cn

C#:   public static void F() {}
来源：http://mii.yuxming.cn

[G09] 接口 / 抽象类
来源：http://vua.9152youxi.cn

Py:   from abc import ABC, abstractmethod
来源：http://ejf.ctjpmb.com

PHP:  interface Shape { public function area(): float; }
来源：http://cpl.sysykeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://zyh.guannengcc.top

TS:   interface Shape { area(): number; }
来源：http://xlu.mhx1999.top

Java: interface Shape { double area(); }
来源：http://uqv.zhixingplan.top

Go:   type Shape interface { Area() float64 }
来源：http://swu.hfpthk.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gqw.zhaomingkeji.xyz

C#:   interface IShape { double Area(); }
来源：http://pwi.wangshuangyany.cn

[G10] 访问控制
来源：http://rtg.dianchejie.cn

Py:   约定 _protected / __private（不强制）
来源：http://kqh.zhoulong.xyz

PHP:  public / protected / private
来源：http://iql.chenjidiqi.icu

JS:   #private 字段；其余公开
来源：http://lnf.52xcode.cn

TS:   public / protected / private
来源：http://qvr.hnxiangtu.top

Java: public / protected / private / 默认包级
来源：http://gqz.jinqigufen.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://bje.fanxiaobao.xyz

Ruby: public / protected / private
来源：http://gvf.xingfuxueyuan.xyz

C#:   public / protected / private / internal
来源：http://yil.meibo888.top

[G11] getter / setter
来源：http://kkh.ivvv.top

Py:   @property 与 @x.setter
来源：http://uad.hesvh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fsy.dianchejie.cn

JS:   get name() { return this._name; }
来源：http://dln.sweek.top

TS:   get name(): string { return this._name; }
来源：http://vwg.ybcxt.top

Java: public String getName() { return name; }
来源：http://aqv.ivvv.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://vmt.ydjk.org.cn

Ruby: attr_accessor :name
来源：http://wqf.cheryme.top

C#:   public string Name { get; set; }
来源：http://vep.cashguo.top

[G12] 对象转字符串
来源：http://zyt.xziqi.cn

Py:   def __str__(self): return self.name
来源：http://uca.quarkkingdee.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://afo.jinyuanbaomall.cn

JS:   toString() { return this.name; }
来源：http://tym.daria6918.cn

TS:   toString(): string { return this.name; }
来源：http://mrc.zhoulong.xyz

Java: @Override public String toString() { return name; }
来源：http://dkm.hammf.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xfq.gotoacloud.top

Ruby: def to_s; @name; end
来源：http://jts.hfpthk.cn

C#:   public override string ToString() => Name;
来源：http://rfa.dianchejie.cn

[G13] 判断对象类型
来源：http://qpl.zhijiandao.cn

Py:   isinstance(u, User)
来源：http://zre.dianchejie.cn

PHP:  $u instanceof User
来源：http://lvw.shanyushiyangkeji.top

JS:   u instanceof User
来源：http://wdt.jinghuilouyu.cn

TS:   u instanceof User
来源：http://ymi.ctjpmb.com

Java: u instanceof User
来源：http://krp.guowangkeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://dec.fanxiaobao.xyz

Ruby: u.is_a?(User)
来源：http://flk.nwbrower.top

C#:   u is User
来源：http://vlp.ehwqpu.com

[G14] 数据类 / record
来源：http://jrt.0kj1m.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mkb.jianghu66.top

PHP:  // 用 readonly 属性模拟
来源：http://tql.guowangkeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://ioq.jinyuanbaomall.cn

TS:   type User = { name: string; age: number };
来源：http://edn.cucudq.cn

Java: record User(String name, int age) {}
来源：http://jfm.jqgufenzy.top

Go:   type User struct { Name string; Age int }
来源：http://gsf.zhongyouzk.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pyv.havefunace.top

C#:   record User(string Name, int Age);
来源：http://wkw.gzhubu.top

[G15] 枚举
来源：http://ygz.ivvv.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jsx.ppjwa.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gfz.ehwqpu.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wxa.sjlbkw.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://krr.nanxuanxn.top

Java: enum Color { RED, GREEN }
来源：http://atz.hcnkem.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://byi.shuidangran.top

Ruby: Color = %i[red green].freeze
来源：http://mxe.jinyuanbaomall.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mhd.zdqjudy.top

[G16] 对象转数组 / 字典
来源：http://bub.fengsongda.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://guy.yuanzhike.top

PHP:  get_object_vars($obj);
来源：http://lub.zhiwuduotai.top

JS:   Object.entries(obj)
来源：http://zsk.jinghuilouyu.cn

TS:   Object.entries(obj)
来源：http://lmc.ctjpmb.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yvw.feifeiyinyue.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://vnj.gogol.net.cn

Ruby: obj.instance_variables
来源：http://pmo.xinyue.icu

C#:   // 用反射或 System.Text.Json
来源：http://zkx.zhongyouzk.top

================================================================================
来源：http://gyd.ydzc1.top

H. 异常与错误处理
来源：http://vor.0kj1m.cn

================================================================================
来源：http://gtw.zhixingplan.top

[H01] try / catch 基础
来源：http://gme.ydzc1.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mgo.cqqwz.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lqs.jinqigfzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gte.yueranfly.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nyw.yanxiufei.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xdb.ppjwa.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://eoz.sufxvd.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mtf.daria6918.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tah.fzhhl.top

[H02] finally / ensure 收尾
来源：http://ylq.zdqjudy.top

Py:   try: f()⏎finally: cleanup()
来源：http://faw.cqqwz.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jof.hammf.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pfo.feifeiyinyue.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ewk.yj20258.top

Java: try { f(); } finally { cleanup(); }
来源：http://uej.xingfuxueyuan.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://taj.aizwys.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://tuv.cashguo.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ebg.xinyue.icu

[H03] 主动抛出异常
来源：http://ohq.fengsongda.top

Py:   raise ValueError("错误信息")
来源：http://vtl.c1oappe.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qvy.snrcjt.cn

JS:   throw new Error("错误信息");
来源：http://waw.smart0.xyz

TS:   throw new Error("错误信息");
来源：http://keq.yueranfly.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://mjc.ybcxt.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cyq.yongpay.top

Ruby: raise ArgumentError, "错误信息"
来源：http://gcc.hnqzz.top

C#:   throw new ArgumentException("错误信息");
来源：http://hyi.dianchejie.cn

[H04] 自定义异常类型
来源：http://dho.hongshengwenyu.top

Py:   class MyError(Exception): pass
来源：http://dnk.fanxiaobao.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://nvq.gzhubu.top

JS:   class MyError extends Error {}
来源：http://dcl.sufxvd.cn

TS:   class MyError extends Error {}
来源：http://iee.c1oappe.top

Java: class MyException extends RuntimeException {}
来源：http://zaj.ydzc1.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rcl.sjlbkw.cn

Ruby: class MyError < StandardError; end
来源：http://uhj.iojbl.cn

C#:   class MyException : Exception {}
来源：http://dbz.zhoulong.xyz

[H05] 捕获特定类型
来源：http://kjj.cheryme.top

Py:   except ValueError as e:
来源：http://jsf.xziqi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zvg.cucudq.cn

JS:   if (e instanceof TypeError) {}
来源：http://jrb.jqgfzy.top

TS:   if (e instanceof TypeError) {}
来源：http://pbp.jinqigfzy.top

Java: catch (IOException | SQLException e) {}
来源：http://asp.jinghuilouyu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://edu.cucudq.cn

Ruby: rescue ArgumentError => e
来源：http://wix.xingfuxueyuan.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ion.shangyingyoupin.top

[H06] 可选值 / 空值安全访问
来源：http://phs.chenzaomai.com

Py:   value = d.get("k") or default
来源：http://nvv.hcnkem.com

PHP:  $v = $d["k"] ?? null;
来源：http://uvx.cqqwz.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jme.shangyingyoupin.top

TS:   obj?.a?.b;  d ?? default
来源：http://eqj.epnwcf.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kee.yj202588.top

Go:   if v, ok := m["k"]; ok { }
来源：http://mdi.hcnkem.com

Ruby: d&.dig(:a, :b)
来源：http://ofk.zhiwuduotai.top

C#:   obj?.A?.B ?? default
来源：http://ixy.shzxlz.cn

[H07] 断言
来源：http://ffh.ehwqpu.com

Py:   assert x > 0, "必须为正"
来源：http://ftb.0kj1m.cn

PHP:  assert($x > 0);
来源：http://llx.tarul.cn

JS:   console.assert(x > 0);
来源：http://zcq.pengpengdd.cyou

TS:   console.assert(x > 0);
来源：http://nko.daria6918.cn

Java: assert x > 0 : "必须为正";
来源：http://fuu.zhoulong.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jdv.pycfn.com

Ruby: raise "必须为正" unless x > 0
来源：http://twh.quarkkingdee.top

C#:   Debug.Assert(x > 0);
来源：http://msz.xuetiantiany.cn

[H08] 获取错误信息与堆栈
来源：http://vbp.sxryk.cn

Py:   str(e);  traceback.format_exc()
来源：http://gin.sysykeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://inb.zhongyouzk.top


<!-- 参考信息 -->