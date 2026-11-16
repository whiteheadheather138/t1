代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pvf.316326.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://rwt.yj20258888.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xjl.nwbrower.top

Ruby: File.read("a.txt")
来源：http://rzf.pycfn.com

C#:   File.ReadAllText("a.txt");
来源：http://crc.hammf.cn

[F02] 逐行读取文件
来源：http://pok.yfazqb.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jfx.cqqwz.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hqh.gotoacloud.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zwq.fanxiaobao.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dge.yj20258888.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qjw.quarkkingdee.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://utb.52xcode.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://izk.fanxiaobao.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lde.hongshengwenyu.top

[F03] 写入文件（覆盖）
来源：http://way.guowangkeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zlu.quarkkingdee.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://bif.zhijiandao.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://boy.zhoulong.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://thl.yangfankeji.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kem.yfazqb.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ela.shangyingyoupin.top

Ruby: File.write("a.txt", "hi")
来源：http://eqw.pengpengdd.cyou

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bem.ywan-chungtsiang.top

[F04] 追加写入文件
来源：http://etu.fengsongda.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://seh.birdmap.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qrw.cqqwz.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jcx.guannengcc.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://buu.yvedp.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kfu.yfazqb.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://aea.haohaochexian.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jsj.ehwqpu.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vuc.yfazqb.com

[F05] 判断文件或目录是否存在
来源：http://vab.chenjidiqi.icu

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mou.gotoacloud.top

PHP:  file_exists("a.txt");
来源：http://rls.yvedp.cn

JS:   fs.existsSync("a.txt")
来源：http://zzk.shuidangran.top

TS:   fs.existsSync("a.txt")
来源：http://mot.jinyuanbaomall.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xtm.xuanzx.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vjf.bbcook.cn

Ruby: File.exist?("a.txt")
来源：http://ymq.wangshuangyany.cn

C#:   File.Exists("a.txt")
来源：http://vqy.tanke756.top

[F06] 删除文件
来源：http://ghs.jqgfzy.top

Py:   os.remove("a.txt")
来源：http://mxl.meibo888.top

PHP:  unlink("a.txt");
来源：http://zqv.wangdashe.top

JS:   fs.unlinkSync("a.txt")
来源：http://vgg.jinqigfzy.top

TS:   fs.unlinkSync("a.txt")
来源：http://xfc.epnwcf.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zoo.yuanzhike.top

Go:   os.Remove("a.txt")
来源：http://wkx.zdqjudy.top

Ruby: File.delete("a.txt")
来源：http://oop.chenlongwang.top

C#:   File.Delete("a.txt");
来源：http://dcy.wangdashe.top

[F07] 创建目录（含多级）
来源：http://hpq.kuanghao11.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ixk.nanxuanxn.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://avw.hywenlv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://flp.uphjek.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ptt.svipenyu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://toc.dianchejie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://efy.mhx1999.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pej.vehdjk.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qha.birdmap.top

[F08] 遍历目录
来源：http://znm.xingfuxueyuan.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://nir.hysaishi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://osk.zhijiandao.cn

JS:   fs.readdirSync("dir")
来源：http://xwd.xinyue.icu

TS:   fs.readdirSync("dir")
来源：http://hdk.nanxuanxn.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hgr.dianchejie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pus.mhx1999.top

Ruby: Dir.children("dir")
来源：http://ntp.xylfe.cn

C#:   Directory.GetFiles("dir")
来源：http://okv.vehdjk.com

[F09] 获取文件大小
来源：http://oay.yfazqb.com

Py:   os.path.getsize("a.txt")
来源：http://gff.c1oappe.top

PHP:  filesize("a.txt");
来源：http://mmq.zhaomingkeji.xyz

JS:   fs.statSync("a.txt").size
来源：http://ojq.wangshuangyany.cn

TS:   fs.statSync("a.txt").size
来源：http://lnw.9152youxi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://nga.jlsjyb.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jjn.jyoumei.cn

Ruby: File.size("a.txt")
来源：http://goj.dianchejie.cn

C#:   new FileInfo("a.txt").Length
来源：http://kai.daxiang520.top

[F10] 取文件扩展名 / 文件名
来源：http://rrn.chenlongwang.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hmm.cheryme.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wgx.xinyue.icu

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://veg.316326.xyz

TS:   path.extname("a.txt")
来源：http://rqi.dianchejie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bgs.hysaishi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://scr.yongpay.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://buc.ydjk.org.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://htl.fehbvm.com

[F11] 复制与移动文件
来源：http://qnw.shzxlz.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lvn.fktsv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oro.ybcxt.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gcg.uphjek.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vbg.guowangkeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wmx.gaohongyu789.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xap.zdbjq.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vfk.9152youxi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vvz.jinqigfzy.top

[F12] CSV 读写
来源：http://kxp.epnwcf.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pcf.shangyingyoupin.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rqf.yangfankeji.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fnz.9152youxi.cn

TS:   // 同上
来源：http://euh.hywenlv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://agt.xuetiantiany.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jzd.haohaochexian.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://oyp.jyoumei.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ayv.wangdashe.top

================================================================================
来源：http://zil.sysykeji.top

G. 面向对象
来源：http://yka.jqgfzy.top

================================================================================
来源：http://are.jinqigfzy.top

[G01] 定义类
来源：http://kag.sjlbkw.cn

Py:   class User: pass
来源：http://vga.hfpthk.cn

PHP:  class User {}
来源：http://rwz.sufxvd.cn

JS:   class User {}
来源：http://zbf.daxiang520.top

TS:   class User { name: string = ""; }
来源：http://pph.hnqzz.top

Java: class User {}
来源：http://shy.pengpengdd.cyou

Go:   type User struct { Name string }
来源：http://ddf.nanxuanxn.top

Ruby: class User; end
来源：http://bov.jinqigufen.top

C#:   class User {}
来源：http://ojx.cqqwz.cn

[G02] 构造函数
来源：http://axd.yuxming.cn

Py:   def __init__(self, name): self.name = name
来源：http://dpf.gaohongyu789.top

PHP:  public function __construct(public string $name) {}
来源：http://nub.fengsongda.top

JS:   constructor(name) { this.name = name; }
来源：http://ekr.52xcode.cn

TS:   constructor(public name: string) {}
来源：http://nvg.hcnkem.com

Java: User(String name) { this.name = name; }
来源：http://ebn.ivvv.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yhs.daxiang520.top

Ruby: def initialize(name); @name = name; end
来源：http://xjp.uphjek.com

C#:   public User(string name) { Name = name; }
来源：http://ccx.chenlongwang.top

[G03] 实例属性
来源：http://vpy.gogol.net.cn

Py:   self.name = "x"
来源：http://vcu.ehwqpu.com

PHP:  public string $name = "x";
来源：http://jsv.yuxming.cn

JS:   this.name = "x";
来源：http://gak.sweek.top

TS:   name: string = "x";
来源：http://iek.jianghu66.top

Java: private String name;
来源：http://vlp.wangdashe.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://enm.0kj1m.cn

Ruby: @name = "x"
来源：http://ovn.fzhhl.top

C#:   public string Name { get; set; } = "x";
来源：http://quo.9152youxi.cn

[G04] 定义方法
来源：http://bci.chenlongwang.top

Py:   def greet(self): return self.name
来源：http://uxa.fehbvm.com

PHP:  public function greet(): string { return $this->name; }
来源：http://gxs.yanxiufei.cn

JS:   greet() { return this.name; }
来源：http://ump.c1oappe.top

TS:   greet(): string { return this.name; }
来源：http://tzs.hongshengwenyu.top

Java: String greet() { return name; }
来源：http://lyb.52xcode.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://oee.zhaomingkeji.xyz

Ruby: def greet; @name; end
来源：http://ghg.tian-w.cn

C#:   public string Greet() => Name;
来源：http://ohx.cucudq.cn

[G05] 继承
来源：http://qwf.0kj1m.cn

Py:   class Admin(User): pass
来源：http://mtu.yueranfly.top

PHP:  class Admin extends User {}
来源：http://rgr.aibaodan.cn

JS:   class Admin extends User {}
来源：http://hgb.yj20258.top

TS:   class Admin extends User {}
来源：http://cyj.fzhhl.top

Java: class Admin extends User {}
来源：http://nrl.wangdashe.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dng.fktsv.cn

Ruby: class Admin < User; end
来源：http://xzy.hongshengwenyu.top

C#:   class Admin : User {}
来源：http://use.yj20258888.top

[G06] 重写方法
来源：http://hff.tianlin.xyz

Py:   def greet(self): return "admin"
来源：http://mte.yfazqb.com

PHP:  public function greet(): string { return "admin"; }
来源：http://gvv.aizwys.cn

JS:   greet() { return "admin"; }
来源：http://ozq.sysykeji.top

TS:   greet(): string { return "admin"; }
来源：http://wdv.tanke756.top

Java: @Override String greet() { return "admin"; }
来源：http://fmp.fanxiaobao.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bmr.nanxuanxn.top

Ruby: def greet; "admin"; end
来源：http://evi.vqdsnc.cn

C#:   public override string Greet() => "admin";
来源：http://zfu.ydjk.org.cn

[G07] 调用父类方法
来源：http://vij.fanxiaobao.xyz

Py:   super().greet()
来源：http://ndk.hesvh.cn

PHP:  parent::greet();
来源：http://zcp.shuidangran.top

JS:   super.greet();
来源：http://dep.ehwqpu.com

TS:   super.greet();
来源：http://pvq.yj202588.top

Java: super.greet();
来源：http://fkh.redwolf501.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ujl.sysykeji.top

Ruby: super
来源：http://ksi.andypj.xyz

C#:   base.Greet();
来源：http://glm.ybcxt.top

[G08] 静态方法与属性
来源：http://dxh.yj20258.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kab.yanxiufei.cn

PHP:  public static function f() {}
来源：http://wcp.zhiwuduotai.top

JS:   static f() {}
来源：http://gtc.yueranfly.top

TS:   static f(): void {}
来源：http://meg.xingfuxueyuan.xyz

Java: static void f() {}
来源：http://phr.sxryk.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bzz.zhoulong.xyz

Ruby: def self.f; end
来源：http://sdf.ywan-chungtsiang.top

C#:   public static void F() {}
来源：http://osh.birdmap.top

[G09] 接口 / 抽象类
来源：http://qmn.shanyushiyangkeji.top

Py:   from abc import ABC, abstractmethod
来源：http://sso.shzxlz.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ayj.guowangkeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://vyc.cashguo.top

TS:   interface Shape { area(): number; }
来源：http://cmm.nwbrower.top

Java: interface Shape { double area(); }
来源：http://rqj.wangdashe.top

Go:   type Shape interface { Area() float64 }
来源：http://mif.bbcook.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://iwk.hesvh.cn

C#:   interface IShape { double Area(); }
来源：http://mxy.xziqi.cn

[G10] 访问控制
来源：http://ixh.sweek.top

Py:   约定 _protected / __private（不强制）
来源：http://ths.52xcode.cn

PHP:  public / protected / private
来源：http://hbb.aibaodan.cn

JS:   #private 字段；其余公开
来源：http://pui.feifeiyinyue.top

TS:   public / protected / private
来源：http://iaa.meibo888.top

Java: public / protected / private / 默认包级
来源：http://smg.shanyushiyangtech.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://tnb.shangyingyoupin.top

Ruby: public / protected / private
来源：http://wkz.xinyue.icu

C#:   public / protected / private / internal
来源：http://zyu.wangshuangyany.cn

[G11] getter / setter
来源：http://fcb.yvedp.cn

Py:   @property 与 @x.setter
来源：http://irq.meibo888.top

PHP:  public function getName(): string { return $this->name; }
来源：http://yjb.316326.xyz

JS:   get name() { return this._name; }
来源：http://roc.guannengcc.top

TS:   get name(): string { return this._name; }
来源：http://pdx.yvedp.cn

Java: public String getName() { return name; }
来源：http://ufv.vehdjk.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://jhx.gogol.net.cn

Ruby: attr_accessor :name
来源：http://llk.hnqzz.top

C#:   public string Name { get; set; }
来源：http://den.zdqjudy.top

[G12] 对象转字符串
来源：http://oex.bbcook.cn

Py:   def __str__(self): return self.name
来源：http://hqr.nwbrower.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://tog.gotoacloud.top

JS:   toString() { return this.name; }
来源：http://scc.hnqzz.top

TS:   toString(): string { return this.name; }
来源：http://jmy.hnqzz.top

Java: @Override public String toString() { return name; }
来源：http://nxz.jinyuanbaomall.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fmf.shzxlz.cn

Ruby: def to_s; @name; end
来源：http://usc.mhx1999.top

C#:   public override string ToString() => Name;
来源：http://laa.nanxinkj.top

[G13] 判断对象类型
来源：http://tyw.0kj1m.cn

Py:   isinstance(u, User)
来源：http://tep.fengsongda.top

PHP:  $u instanceof User
来源：http://bea.yongpay.top

JS:   u instanceof User
来源：http://hjk.snrcjt.cn

TS:   u instanceof User
来源：http://pvn.yj20258888.top

Java: u instanceof User
来源：http://nlz.hnqzz.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://pxx.sufxvd.cn

Ruby: u.is_a?(User)
来源：http://cpt.yj20258888.top

C#:   u is User
来源：http://cdp.gaohongyu789.top

[G14] 数据类 / record
来源：http://dgc.ivvv.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://iok.tian-w.cn

PHP:  // 用 readonly 属性模拟
来源：http://owe.bjfxy.top

JS:   // 无内置：普通类或对象字面量
来源：http://yox.cdnleiting.top

TS:   type User = { name: string; age: number };
来源：http://vpw.c1oappe.top

Java: record User(String name, int age) {}
来源：http://suw.redwolf501.top

Go:   type User struct { Name string; Age int }
来源：http://fxr.yonumen.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rys.tian-w.cn

C#:   record User(string Name, int Age);
来源：http://ecp.gaohongyu789.top

[G15] 枚举
来源：http://azq.meibo888.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wiw.yangfankeji.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://jfu.aibaodan.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zbw.guowangkeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nsd.cqqwz.cn

Java: enum Color { RED, GREEN }
来源：http://fwc.zhiwuduotai.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ces.feifeiyinyue.top

Ruby: Color = %i[red green].freeze
来源：http://ied.nanxinkj.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zco.vehdjk.com

[G16] 对象转数组 / 字典
来源：http://sux.0kj1m.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://iws.shzxlz.cn

PHP:  get_object_vars($obj);
来源：http://hqp.cucudq.cn

JS:   Object.entries(obj)
来源：http://wiy.xinyue.icu

TS:   Object.entries(obj)
来源：http://pcb.zhaomingkeji.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hhi.sxryk.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rzd.tanke756.top

Ruby: obj.instance_variables
来源：http://rfh.yuxming.cn

C#:   // 用反射或 System.Text.Json
来源：http://ilt.gotoacloud.top

================================================================================
来源：http://ikn.zhaomingkeji.xyz

H. 异常与错误处理
来源：http://bdi.jyoumei.cn

================================================================================
来源：http://bxw.zdbjq.cn

[H01] try / catch 基础
来源：http://gew.316326.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zms.aibaodan.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cwl.yueranfly.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ohf.nanxuanxn.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ocu.hnxiangtu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ker.gotoacloud.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hmh.pengpengdd.cyou

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zxz.quarkkingdee.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ylk.jlsjyb.cn

[H02] finally / ensure 收尾
来源：http://fpy.pengpengdd.cyou

Py:   try: f()⏎finally: cleanup()
来源：http://wdd.sjlbkw.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hhn.shzxlz.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xzo.snrcjt.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://aoa.zhaomingkeji.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://tiu.yj202588.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://jxb.sysykeji.top

Ruby: begin; f; ensure; cleanup; end
来源：http://gwc.yongpay.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://huy.snrcjt.cn

[H03] 主动抛出异常
来源：http://cll.fzhhl.top

Py:   raise ValueError("错误信息")
来源：http://fnq.yuxming.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ikt.zhijiandao.cn

JS:   throw new Error("错误信息");
来源：http://yli.52xcode.cn

TS:   throw new Error("错误信息");
来源：http://ozp.jinqigufen.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://szf.ppjwa.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://grh.sjlbkw.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ipj.52xcode.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hoh.yvedp.cn

[H04] 自定义异常类型
来源：http://xdm.jlsjyb.cn

Py:   class MyError(Exception): pass
来源：http://ift.fengsongda.top

PHP:  class MyError extends RuntimeException {}
来源：http://ulh.yonumen.top

JS:   class MyError extends Error {}
来源：http://lls.hfpthk.cn

TS:   class MyError extends Error {}
来源：http://wim.yangfankeji.com

Java: class MyException extends RuntimeException {}
来源：http://lrt.guowangkeji.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hzk.yongpay.top

Ruby: class MyError < StandardError; end
来源：http://isl.xuanzx.com

C#:   class MyException : Exception {}
来源：http://acf.ehwqpu.com

[H05] 捕获特定类型
来源：http://fap.nanxuanxn.top

Py:   except ValueError as e:
来源：http://kyf.jiagoushi.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vtw.ywan-chungtsiang.top

JS:   if (e instanceof TypeError) {}
来源：http://wik.c1oappe.top

TS:   if (e instanceof TypeError) {}
来源：http://bnj.sufxvd.cn

Java: catch (IOException | SQLException e) {}
来源：http://bex.jyoumei.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://etk.shanyushiyangtech.top

Ruby: rescue ArgumentError => e
来源：http://dyt.havefunace.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vxt.yj20258888.top

[H06] 可选值 / 空值安全访问
来源：http://lwq.ydzc1.top


<!-- 参考信息 -->