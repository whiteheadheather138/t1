代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://ria.kuanghao11.cn

[F02] 逐行读取文件
来源：http://uvc.yuanzhike.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sts.shanyushiyangkeji.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mxo.hfpthk.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kum.hesvh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cgk.shuidangran.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://att.jlsjyb.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ufj.shanyushiyangkeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fks.uphjek.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jud.xinyue.icu

[F03] 写入文件（覆盖）
来源：http://pnp.ppjwa.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ycz.yanxiufei.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://swx.gaohongyu789.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nfv.epnwcf.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vvo.fehbvm.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uji.aibaodan.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hbs.kuanghao11.cn

Ruby: File.write("a.txt", "hi")
来源：http://gfl.gaohongyu789.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ydw.ehwqpu.com

[F04] 追加写入文件
来源：http://xgc.wangshuangyany.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fxn.shanyushiyangkeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cpj.bjfxy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ope.xingfuxueyuan.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mly.jqgfzy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lfh.vqdsnc.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wix.haohaochexian.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yqa.ppjwa.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ssd.zhoulong.xyz

[F05] 判断文件或目录是否存在
来源：http://afu.jinqigufen.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hbg.guannengcc.top

PHP:  file_exists("a.txt");
来源：http://jid.tian-w.cn

JS:   fs.existsSync("a.txt")
来源：http://csa.wangdashe.top

TS:   fs.existsSync("a.txt")
来源：http://wmc.9152youxi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zwz.wangdashe.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rxw.jlsjyb.cn

Ruby: File.exist?("a.txt")
来源：http://war.zycfv.cn

C#:   File.Exists("a.txt")
来源：http://mfh.tianlin.xyz

[F06] 删除文件
来源：http://arh.shuidangran.top

Py:   os.remove("a.txt")
来源：http://csv.cheryme.top

PHP:  unlink("a.txt");
来源：http://qyj.ppjwa.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rqa.havefunace.top

TS:   fs.unlinkSync("a.txt")
来源：http://epf.sysykeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://aml.hongshengwenyu.top

Go:   os.Remove("a.txt")
来源：http://eic.jinyuanbaomall.cn

Ruby: File.delete("a.txt")
来源：http://gqi.nwbrower.top

C#:   File.Delete("a.txt");
来源：http://rfk.uphjek.com

[F07] 创建目录（含多级）
来源：http://ogi.fanxiaobao.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://asc.ivvv.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jqv.zdbjq.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sxz.andypj.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jqw.shanyushiyangkeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vsr.jinghuilouyu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pte.shanyushiyangtech.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xpv.sweek.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dtm.hfpthk.cn

[F08] 遍历目录
来源：http://wuc.cheryme.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://vnx.ybcxt.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hfw.kuanghao11.cn

JS:   fs.readdirSync("dir")
来源：http://eyw.birdmap.top

TS:   fs.readdirSync("dir")
来源：http://stc.feifeiyinyue.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mvq.zhoulong.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://ate.cheryme.top

Ruby: Dir.children("dir")
来源：http://cnb.uphjek.com

C#:   Directory.GetFiles("dir")
来源：http://eqv.xylfe.cn

[F09] 获取文件大小
来源：http://apv.fengsongda.top

Py:   os.path.getsize("a.txt")
来源：http://iix.aibaodan.cn

PHP:  filesize("a.txt");
来源：http://waw.yangfankeji.com

JS:   fs.statSync("a.txt").size
来源：http://pfz.9152youxi.cn

TS:   fs.statSync("a.txt").size
来源：http://yys.hysaishi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://sdb.dashuyun.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://egj.gotoacloud.top

Ruby: File.size("a.txt")
来源：http://pvx.zhongyouzk.top

C#:   new FileInfo("a.txt").Length
来源：http://sal.jqgufenzy.top

[F10] 取文件扩展名 / 文件名
来源：http://oqo.quarkkingdee.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wva.jqgufenzy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ouw.hnqzz.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jjz.52xcode.cn

TS:   path.extname("a.txt")
来源：http://rma.zdqjudy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bpn.yongpay.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://khe.cdnleiting.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gng.zdqjudy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://aoz.ywan-chungtsiang.top

[F11] 复制与移动文件
来源：http://llc.yangfankeji.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pdl.xziqi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vql.quarkkingdee.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jtp.cashguo.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xfm.jinghuilouyu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pjf.redwolf501.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://abs.zdqjudy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://oxe.ydzc1.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kmw.sjlbkw.cn

[F12] CSV 读写
来源：http://mcg.xinyue.icu

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rtj.hywenlv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uaz.chenzaomai.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sqy.xuanzx.com

TS:   // 同上
来源：http://xgr.ehwqpu.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://awl.zdqjudy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://iwa.wangdashe.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pyb.jqgfzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://xld.havefunace.top

================================================================================
来源：http://san.daria6918.cn

G. 面向对象
来源：http://awq.zhijiandao.cn

================================================================================
来源：http://iom.yuanzhike.top

[G01] 定义类
来源：http://fdg.cashguo.top

Py:   class User: pass
来源：http://xyv.zhoulong.xyz

PHP:  class User {}
来源：http://hvo.xuetiantiany.cn

JS:   class User {}
来源：http://jgu.zhengqikj.top

TS:   class User { name: string = ""; }
来源：http://wbo.yuxming.cn

Java: class User {}
来源：http://osf.ydjk.org.cn

Go:   type User struct { Name string }
来源：http://lzp.zhaomingkeji.xyz

Ruby: class User; end
来源：http://lpv.sufxvd.cn

C#:   class User {}
来源：http://hjc.quarkkingdee.top

[G02] 构造函数
来源：http://fte.jyoumei.cn

Py:   def __init__(self, name): self.name = name
来源：http://npt.mhx1999.top

PHP:  public function __construct(public string $name) {}
来源：http://wcm.zhijiandao.cn

JS:   constructor(name) { this.name = name; }
来源：http://qch.9152youxi.cn

TS:   constructor(public name: string) {}
来源：http://hdj.hesvh.cn

Java: User(String name) { this.name = name; }
来源：http://zhx.andypj.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kfj.pycfn.com

Ruby: def initialize(name); @name = name; end
来源：http://tyj.yfazqb.com

C#:   public User(string name) { Name = name; }
来源：http://bbu.zhijiandao.cn

[G03] 实例属性
来源：http://cyl.yj20258.top

Py:   self.name = "x"
来源：http://tum.tanke756.top

PHP:  public string $name = "x";
来源：http://ebc.zhijiandao.cn

JS:   this.name = "x";
来源：http://tjj.zhiwuduotai.top

TS:   name: string = "x";
来源：http://neg.gotoacloud.top

Java: private String name;
来源：http://qua.yj202588.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gxo.shzxlz.cn

Ruby: @name = "x"
来源：http://ktr.cdnleiting.top

C#:   public string Name { get; set; } = "x";
来源：http://tzf.shzxlz.cn

[G04] 定义方法
来源：http://dqj.jinqigfzy.top

Py:   def greet(self): return self.name
来源：http://zrg.hysaishi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://cit.mhx1999.top

JS:   greet() { return this.name; }
来源：http://nyt.xingfuxueyuan.xyz

TS:   greet(): string { return this.name; }
来源：http://htx.svipenyu.cn

Java: String greet() { return name; }
来源：http://fih.ydjk.org.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qul.yanxiufei.cn

Ruby: def greet; @name; end
来源：http://cwj.zycfv.cn

C#:   public string Greet() => Name;
来源：http://lox.yongpay.top

[G05] 继承
来源：http://pjq.9152youxi.cn

Py:   class Admin(User): pass
来源：http://ztk.jqgufenzy.top

PHP:  class Admin extends User {}
来源：http://xzx.svipenyu.cn

JS:   class Admin extends User {}
来源：http://qml.chenzaomai.com

TS:   class Admin extends User {}
来源：http://vvn.zhengqikj.top

Java: class Admin extends User {}
来源：http://swv.uphjek.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zbs.jqgufenzy.top

Ruby: class Admin < User; end
来源：http://rgh.jinqigufen.top

C#:   class Admin : User {}
来源：http://irp.xinyue.icu

[G06] 重写方法
来源：http://yvu.uphjek.com

Py:   def greet(self): return "admin"
来源：http://qcb.jinqigfzy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://zrt.bjfxy.top

JS:   greet() { return "admin"; }
来源：http://stl.haohaochexian.top

TS:   greet(): string { return "admin"; }
来源：http://ldb.aibaodan.cn

Java: @Override String greet() { return "admin"; }
来源：http://szm.yj20258888.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ovj.tanke756.top

Ruby: def greet; "admin"; end
来源：http://mqn.ybcxt.top

C#:   public override string Greet() => "admin";
来源：http://uop.wangshuangyany.cn

[G07] 调用父类方法
来源：http://hba.vehdjk.com

Py:   super().greet()
来源：http://krx.havefunace.top

PHP:  parent::greet();
来源：http://pof.tian-w.cn

JS:   super.greet();
来源：http://vls.hammf.cn

TS:   super.greet();
来源：http://ymi.smart0.xyz

Java: super.greet();
来源：http://lma.hfpthk.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fcl.daria6918.cn

Ruby: super
来源：http://azp.nanxuanxn.top

C#:   base.Greet();
来源：http://bfc.hesvh.cn

[G08] 静态方法与属性
来源：http://xcx.hysaishi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ezh.bjfxy.top

PHP:  public static function f() {}
来源：http://ltv.redwolf501.top

JS:   static f() {}
来源：http://ews.bbcook.cn

TS:   static f(): void {}
来源：http://ijs.birdmap.top

Java: static void f() {}
来源：http://fwk.zhengqikj.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://jsl.fehbvm.com

Ruby: def self.f; end
来源：http://pcd.gaohongyu789.top

C#:   public static void F() {}
来源：http://gsb.ybcxt.top

[G09] 接口 / 抽象类
来源：http://syu.shangyingyoupin.top

Py:   from abc import ABC, abstractmethod
来源：http://ebn.guannengcc.top

PHP:  interface Shape { public function area(): float; }
来源：http://hxw.zhaomingkeji.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://sts.jqgufenzy.top

TS:   interface Shape { area(): number; }
来源：http://hgy.ivvv.top

Java: interface Shape { double area(); }
来源：http://qzs.pengpengdd.cyou

Go:   type Shape interface { Area() float64 }
来源：http://nbq.hnxiangtu.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xqb.hysaishi.cn

C#:   interface IShape { double Area(); }
来源：http://eao.andypj.xyz

[G10] 访问控制
来源：http://oba.tianlin.xyz

Py:   约定 _protected / __private（不强制）
来源：http://nge.jianghu66.top

PHP:  public / protected / private
来源：http://mhi.cucudq.cn

JS:   #private 字段；其余公开
来源：http://gme.zhengqikj.top

TS:   public / protected / private
来源：http://nvf.cucudq.cn

Java: public / protected / private / 默认包级
来源：http://scu.jqgufenzy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://bnd.9152youxi.cn

Ruby: public / protected / private
来源：http://lsx.feifeiyinyue.top

C#:   public / protected / private / internal
来源：http://ral.chenlongwang.top

[G11] getter / setter
来源：http://zgo.yonumen.top

Py:   @property 与 @x.setter
来源：http://bgx.yongpay.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ioz.bjfxy.top

JS:   get name() { return this._name; }
来源：http://yqn.jinqigufen.top

TS:   get name(): string { return this._name; }
来源：http://wnu.ydjk.org.cn

Java: public String getName() { return name; }
来源：http://zou.yuxming.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qkx.vqdsnc.cn

Ruby: attr_accessor :name
来源：http://lfz.chenzaomai.com

C#:   public string Name { get; set; }
来源：http://lwr.smart0.xyz

[G12] 对象转字符串
来源：http://jou.jinqigufen.top

Py:   def __str__(self): return self.name
来源：http://dmk.birdmap.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://prq.hnqzz.top

JS:   toString() { return this.name; }
来源：http://lsm.jqgufenzy.top

TS:   toString(): string { return this.name; }
来源：http://lwf.0kj1m.cn

Java: @Override public String toString() { return name; }
来源：http://pvj.yuxming.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fph.zhixingplan.top

Ruby: def to_s; @name; end
来源：http://pvg.jianghu66.top

C#:   public override string ToString() => Name;
来源：http://ckk.hywenlv.cn

[G13] 判断对象类型
来源：http://ujx.zycfv.cn

Py:   isinstance(u, User)
来源：http://bqp.cashguo.top

PHP:  $u instanceof User
来源：http://emw.redwolf501.top

JS:   u instanceof User
来源：http://bue.hnxiangtu.top

TS:   u instanceof User
来源：http://efs.pengpengdd.cyou

Java: u instanceof User
来源：http://fwm.aibaodan.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kzb.andypj.xyz

Ruby: u.is_a?(User)
来源：http://nnj.jinqigfzy.top

C#:   u is User
来源：http://lgb.chenjidiqi.icu

[G14] 数据类 / record
来源：http://vqw.0kj1m.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://spb.hammf.cn

PHP:  // 用 readonly 属性模拟
来源：http://frz.tanke756.top

JS:   // 无内置：普通类或对象字面量
来源：http://svl.cdnleiting.top

TS:   type User = { name: string; age: number };
来源：http://orx.nanxuanxn.top

Java: record User(String name, int age) {}
来源：http://egl.svipenyu.cn

Go:   type User struct { Name string; Age int }
来源：http://phg.jqgufenzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rbf.zdqjudy.top

C#:   record User(string Name, int Age);
来源：http://tms.sxryk.cn

[G15] 枚举
来源：http://sat.jqgfzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zcu.pycfn.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://xor.hnqzz.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lri.c1oappe.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lex.haohaochexian.top

Java: enum Color { RED, GREEN }
来源：http://zqj.yuanzhike.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vfz.sxryk.cn

Ruby: Color = %i[red green].freeze
来源：http://eol.iojbl.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iqh.52xcode.cn

[G16] 对象转数组 / 字典
来源：http://vsx.svipenyu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fal.svipenyu.cn

PHP:  get_object_vars($obj);
来源：http://qem.jqgufenzy.top

JS:   Object.entries(obj)
来源：http://ftl.zhijiandao.cn

TS:   Object.entries(obj)
来源：http://sfu.ctjpmb.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ela.quarkkingdee.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://nth.tarul.cn

Ruby: obj.instance_variables
来源：http://xde.zhixingplan.top

C#:   // 用反射或 System.Text.Json
来源：http://uvv.ywan-chungtsiang.top

================================================================================
来源：http://mdb.birdmap.top

H. 异常与错误处理
来源：http://ojw.hysaishi.cn

================================================================================
来源：http://gdx.zhaomingkeji.xyz

[H01] try / catch 基础
来源：http://mky.zdqjudy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ojz.jinyuanbaomall.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zyq.quarkkingdee.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zlw.shzxlz.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wkb.hysaishi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kgo.xziqi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yfd.ybcxt.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gls.hongshengwenyu.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rmg.guannengcc.top

[H02] finally / ensure 收尾
来源：http://ewv.sufxvd.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gmi.nwbrower.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://jho.nanxinkj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://gqu.gogol.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ese.dashuyun.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vex.nanxinkj.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://bde.haohaochexian.top

Ruby: begin; f; ensure; cleanup; end
来源：http://mzg.pycfn.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://geh.xuanzx.com

[H03] 主动抛出异常
来源：http://dno.yongpay.top

Py:   raise ValueError("错误信息")
来源：http://sba.hammf.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nju.sxryk.cn

JS:   throw new Error("错误信息");
来源：http://zkn.guowangkeji.top

TS:   throw new Error("错误信息");
来源：http://twy.wangshuangyany.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://plx.svipenyu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lkp.ydzc1.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ksm.xylfe.cn

C#:   throw new ArgumentException("错误信息");
来源：http://uyr.jinqigufen.top

[H04] 自定义异常类型
来源：http://pum.yj202588.top

Py:   class MyError(Exception): pass
来源：http://vbo.ybcxt.top

PHP:  class MyError extends RuntimeException {}
来源：http://rls.ywan-chungtsiang.top

JS:   class MyError extends Error {}
来源：http://sys.yj202588.top

TS:   class MyError extends Error {}
来源：http://mvy.zhaomingkeji.xyz

Java: class MyException extends RuntimeException {}
来源：http://irg.xziqi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tct.sysykeji.top

Ruby: class MyError < StandardError; end
来源：http://hvh.hongshengwenyu.top

C#:   class MyException : Exception {}
来源：http://nti.jinyuanbaomall.cn

[H05] 捕获特定类型
来源：http://hgv.wangshuangyany.cn

Py:   except ValueError as e:
来源：http://ypr.cdnleiting.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wfm.yj202588.top

JS:   if (e instanceof TypeError) {}
来源：http://phr.hnxiangtu.top

TS:   if (e instanceof TypeError) {}
来源：http://xwn.feifeiyinyue.top

Java: catch (IOException | SQLException e) {}
来源：http://erk.mhx1999.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://amk.snrcjt.cn

Ruby: rescue ArgumentError => e
来源：http://mwi.xuanzx.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://teq.hfpthk.cn

[H06] 可选值 / 空值安全访问
来源：http://yor.dianchejie.cn

Py:   value = d.get("k") or default
来源：http://oqh.yj20258.top

PHP:  $v = $d["k"] ?? null;
来源：http://zlc.fanxiaobao.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://glj.dashuyun.cn

TS:   obj?.a?.b;  d ?? default
来源：http://nln.shanyushiyangtech.top


<!-- 参考信息 -->