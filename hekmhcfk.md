代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qki.chenlongwang.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rdm.jyoumei.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cpk.ybcxt.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hwr.iojbl.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jsm.wangshuangyany.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uke.pengpengdd.cyou

[F03] 写入文件（覆盖）
来源：http://pkg.wangshuangyany.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tkm.zhijiandao.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fra.shanyushiyangkeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dsg.hcnkem.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mpi.yueranfly.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bgr.sufxvd.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cpm.xinyue.icu

Ruby: File.write("a.txt", "hi")
来源：http://rzr.dashuyun.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jnn.yangfankeji.com

[F04] 追加写入文件
来源：http://yam.0kj1m.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vpc.gzhubu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mtu.ctjpmb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://psd.birdmap.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mug.hnqzz.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://add.ctjpmb.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nha.feifeiyinyue.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gnq.pengpengdd.cyou

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wry.svipenyu.cn

[F05] 判断文件或目录是否存在
来源：http://jyp.nanxinkj.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fji.yj202588.top

PHP:  file_exists("a.txt");
来源：http://qhg.tian-w.cn

JS:   fs.existsSync("a.txt")
来源：http://fay.kuanghao11.cn

TS:   fs.existsSync("a.txt")
来源：http://nsp.jqgufenzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://eic.zycfv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vhl.hcnkem.com

Ruby: File.exist?("a.txt")
来源：http://rbh.sysykeji.top

C#:   File.Exists("a.txt")
来源：http://ptq.yonumen.top

[F06] 删除文件
来源：http://aba.sweek.top

Py:   os.remove("a.txt")
来源：http://qme.uphjek.com

PHP:  unlink("a.txt");
来源：http://xpe.bbcook.cn

JS:   fs.unlinkSync("a.txt")
来源：http://you.sysykeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://zsc.meibo888.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pcx.cashguo.top

Go:   os.Remove("a.txt")
来源：http://blo.dashuyun.cn

Ruby: File.delete("a.txt")
来源：http://xew.gaohongyu789.top

C#:   File.Delete("a.txt");
来源：http://lrc.xuanzx.com

[F07] 创建目录（含多级）
来源：http://kxs.daxiang520.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kvp.hcnkem.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://emj.yangfankeji.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wsj.uphjek.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xih.jinqigfzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://asp.gaohongyu789.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ofz.gogol.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xay.316326.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vxg.gogol.net.cn

[F08] 遍历目录
来源：http://tck.jinqigfzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://uui.yj202588.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zeq.guannengcc.top

JS:   fs.readdirSync("dir")
来源：http://cbu.tian-w.cn

TS:   fs.readdirSync("dir")
来源：http://yks.jlsjyb.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ufx.cqqwz.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://kot.shzxlz.cn

Ruby: Dir.children("dir")
来源：http://ill.snrcjt.cn

C#:   Directory.GetFiles("dir")
来源：http://bfn.aibaodan.cn

[F09] 获取文件大小
来源：http://rfv.gogol.net.cn

Py:   os.path.getsize("a.txt")
来源：http://dcm.52xcode.cn

PHP:  filesize("a.txt");
来源：http://uzd.zhiwuduotai.top

JS:   fs.statSync("a.txt").size
来源：http://yxl.aibaodan.cn

TS:   fs.statSync("a.txt").size
来源：http://ncj.jqgufenzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://jvr.fzhhl.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://coj.ivvv.top

Ruby: File.size("a.txt")
来源：http://yff.hnxiangtu.top

C#:   new FileInfo("a.txt").Length
来源：http://oeo.yuanzhike.top

[F10] 取文件扩展名 / 文件名
来源：http://vgr.ydjk.org.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://von.haohaochexian.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jmd.kuanghao11.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://thm.meibo888.top

TS:   path.extname("a.txt")
来源：http://wzi.sweek.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ztp.chenjidiqi.icu

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://anl.yangfankeji.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ecs.gotoacloud.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ult.jyoumei.cn

[F11] 复制与移动文件
来源：http://bfh.andypj.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zto.fengsongda.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ubl.xylfe.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fos.pycfn.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gtu.hfpthk.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ymg.jyoumei.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vmu.zdqjudy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bkd.fzhhl.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rpu.gotoacloud.top

[F12] CSV 读写
来源：http://xop.sufxvd.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://aos.ybcxt.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mvn.jqgufenzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fsm.yj20258888.top

TS:   // 同上
来源：http://oev.tarul.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vpm.bjfxy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zve.aibaodan.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dqy.gotoacloud.top

C#:   // 无内置：用 CsvHelper 库
来源：http://chj.xziqi.cn

================================================================================
来源：http://uln.ppjwa.cn

G. 面向对象
来源：http://nnt.meibo888.top

================================================================================
来源：http://lwk.hfpthk.cn

[G01] 定义类
来源：http://bnr.jinghuilouyu.cn

Py:   class User: pass
来源：http://pxw.zhijiandao.cn

PHP:  class User {}
来源：http://clq.yvedp.cn

JS:   class User {}
来源：http://wur.cqqwz.cn

TS:   class User { name: string = ""; }
来源：http://cce.guowangkeji.top

Java: class User {}
来源：http://qee.mhx1999.top

Go:   type User struct { Name string }
来源：http://iyk.snrcjt.cn

Ruby: class User; end
来源：http://rns.hywenlv.cn

C#:   class User {}
来源：http://ovv.redwolf501.top

[G02] 构造函数
来源：http://rvx.nwbrower.top

Py:   def __init__(self, name): self.name = name
来源：http://jki.zhaomingkeji.xyz

PHP:  public function __construct(public string $name) {}
来源：http://aug.zhijiandao.cn

JS:   constructor(name) { this.name = name; }
来源：http://vbc.hnqzz.top

TS:   constructor(public name: string) {}
来源：http://xoy.fehbvm.com

Java: User(String name) { this.name = name; }
来源：http://jxa.zhijiandao.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://aey.yuanzhike.top

Ruby: def initialize(name); @name = name; end
来源：http://ran.meibo888.top

C#:   public User(string name) { Name = name; }
来源：http://ori.tarul.cn

[G03] 实例属性
来源：http://gpn.yongpay.top

Py:   self.name = "x"
来源：http://mib.havefunace.top

PHP:  public string $name = "x";
来源：http://yrk.birdmap.top

JS:   this.name = "x";
来源：http://cex.bjfxy.top

TS:   name: string = "x";
来源：http://amg.birdmap.top

Java: private String name;
来源：http://kyf.fzhhl.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://agn.bbcook.cn

Ruby: @name = "x"
来源：http://vnt.pengpengdd.cyou

C#:   public string Name { get; set; } = "x";
来源：http://wcl.snrcjt.cn

[G04] 定义方法
来源：http://hoj.fanxiaobao.xyz

Py:   def greet(self): return self.name
来源：http://qau.9152youxi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://yfg.yuanzhike.top

JS:   greet() { return this.name; }
来源：http://oxt.cqqwz.cn

TS:   greet(): string { return this.name; }
来源：http://pct.sxryk.cn

Java: String greet() { return name; }
来源：http://juk.zdbjq.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xvh.dianchejie.cn

Ruby: def greet; @name; end
来源：http://msp.guowangkeji.top

C#:   public string Greet() => Name;
来源：http://sti.jinqigfzy.top

[G05] 继承
来源：http://coc.jinqigfzy.top

Py:   class Admin(User): pass
来源：http://ufa.sweek.top

PHP:  class Admin extends User {}
来源：http://ill.nanxinkj.top

JS:   class Admin extends User {}
来源：http://rrn.birdmap.top

TS:   class Admin extends User {}
来源：http://jbi.birdmap.top

Java: class Admin extends User {}
来源：http://njp.zhixingplan.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hlj.jianghu66.top

Ruby: class Admin < User; end
来源：http://ouf.daxiang520.top

C#:   class Admin : User {}
来源：http://tlz.hcnkem.com

[G06] 重写方法
来源：http://jlb.cashguo.top

Py:   def greet(self): return "admin"
来源：http://upx.52xcode.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://cpd.zhixingplan.top

JS:   greet() { return "admin"; }
来源：http://les.zhongyouzk.top

TS:   greet(): string { return "admin"; }
来源：http://mzy.hcnkem.com

Java: @Override String greet() { return "admin"; }
来源：http://zeh.ydjk.org.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yks.jqgufenzy.top

Ruby: def greet; "admin"; end
来源：http://xrk.tian-w.cn

C#:   public override string Greet() => "admin";
来源：http://ljm.316326.xyz

[G07] 调用父类方法
来源：http://hrm.feifeiyinyue.top

Py:   super().greet()
来源：http://xjr.zdqjudy.top

PHP:  parent::greet();
来源：http://txu.jinghuilouyu.cn

JS:   super.greet();
来源：http://izm.sufxvd.cn

TS:   super.greet();
来源：http://jfj.yanxiufei.cn

Java: super.greet();
来源：http://lhm.sysykeji.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kwm.jinyuanbaomall.cn

Ruby: super
来源：http://rfn.chenzaomai.com

C#:   base.Greet();
来源：http://ysc.guowangkeji.top

[G08] 静态方法与属性
来源：http://yli.hnqzz.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cvj.sufxvd.cn

PHP:  public static function f() {}
来源：http://ito.xingfuxueyuan.xyz

JS:   static f() {}
来源：http://nas.yj20258.top

TS:   static f(): void {}
来源：http://ozx.vqdsnc.cn

Java: static void f() {}
来源：http://zka.pengpengdd.cyou

Go:   // 无 static：用包级函数，按包名调用
来源：http://owp.hysaishi.cn

Ruby: def self.f; end
来源：http://gda.andypj.xyz

C#:   public static void F() {}
来源：http://arm.ywan-chungtsiang.top

[G09] 接口 / 抽象类
来源：http://szj.iojbl.cn

Py:   from abc import ABC, abstractmethod
来源：http://xkq.guowangkeji.top

PHP:  interface Shape { public function area(): float; }
来源：http://vjr.316326.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://isa.jyoumei.cn

TS:   interface Shape { area(): number; }
来源：http://kny.xinyue.icu

Java: interface Shape { double area(); }
来源：http://xxw.quarkkingdee.top

Go:   type Shape interface { Area() float64 }
来源：http://hin.zhoulong.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mvp.cheryme.top

C#:   interface IShape { double Area(); }
来源：http://dxf.ivvv.top

[G10] 访问控制
来源：http://lou.zhongyouzk.top

Py:   约定 _protected / __private（不强制）
来源：http://gha.bbcook.cn

PHP:  public / protected / private
来源：http://jod.redwolf501.top

JS:   #private 字段；其余公开
来源：http://tle.jinqigufen.top

TS:   public / protected / private
来源：http://mhy.cdnleiting.top

Java: public / protected / private / 默认包级
来源：http://kmh.yj20258888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://gri.yj20258.top

Ruby: public / protected / private
来源：http://ebd.yvedp.cn

C#:   public / protected / private / internal
来源：http://bul.chenjidiqi.icu

[G11] getter / setter
来源：http://iqh.haohaochexian.top

Py:   @property 与 @x.setter
来源：http://hqa.wangdashe.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ypd.xylfe.cn

JS:   get name() { return this._name; }
来源：http://qtu.daxiang520.top

TS:   get name(): string { return this._name; }
来源：http://jlo.zdqjudy.top

Java: public String getName() { return name; }
来源：http://nvb.xuanzx.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://bhw.ydjk.org.cn

Ruby: attr_accessor :name
来源：http://nuw.ehwqpu.com

C#:   public string Name { get; set; }
来源：http://xof.gaohongyu789.top

[G12] 对象转字符串
来源：http://abd.feifeiyinyue.top

Py:   def __str__(self): return self.name
来源：http://xex.fanxiaobao.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://ang.zhixingplan.top

JS:   toString() { return this.name; }
来源：http://aes.ydzc1.top

TS:   toString(): string { return this.name; }
来源：http://pec.ywan-chungtsiang.top

Java: @Override public String toString() { return name; }
来源：http://chp.zdqjudy.top

Go:   func (u User) String() string { return u.Name }
来源：http://lvp.yonumen.top

Ruby: def to_s; @name; end
来源：http://lpx.redwolf501.top

C#:   public override string ToString() => Name;
来源：http://ffi.ivvv.top

[G13] 判断对象类型
来源：http://xxt.gaohongyu789.top

Py:   isinstance(u, User)
来源：http://lmk.hfpthk.cn

PHP:  $u instanceof User
来源：http://xda.jinyuanbaomall.cn

JS:   u instanceof User
来源：http://zda.9152youxi.cn

TS:   u instanceof User
来源：http://sfy.meibo888.top

Java: u instanceof User
来源：http://cjl.nanxuanxn.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://biu.pycfn.com

Ruby: u.is_a?(User)
来源：http://eoe.meibo888.top

C#:   u is User
来源：http://wvo.sysykeji.top

[G14] 数据类 / record
来源：http://qxh.xinyue.icu

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lus.shanyushiyangtech.top

PHP:  // 用 readonly 属性模拟
来源：http://gya.jinyuanbaomall.cn

JS:   // 无内置：普通类或对象字面量
来源：http://iju.52xcode.cn

TS:   type User = { name: string; age: number };
来源：http://tok.yanxiufei.cn

Java: record User(String name, int age) {}
来源：http://bla.daxiang520.top

Go:   type User struct { Name string; Age int }
来源：http://zvk.nanxuanxn.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cca.zhiwuduotai.top

C#:   record User(string Name, int Age);
来源：http://dzr.guowangkeji.top

[G15] 枚举
来源：http://anp.sjlbkw.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vsn.mhx1999.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ehq.zhaomingkeji.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tty.yj20258.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fji.meibo888.top

Java: enum Color { RED, GREEN }
来源：http://lxp.jlsjyb.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xag.yj202588.top

Ruby: Color = %i[red green].freeze
来源：http://wxc.wangshuangyany.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yoq.shuidangran.top

[G16] 对象转数组 / 字典
来源：http://nri.316326.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qzy.chenzaomai.com

PHP:  get_object_vars($obj);
来源：http://eju.sjlbkw.cn

JS:   Object.entries(obj)
来源：http://jqq.ppjwa.cn

TS:   Object.entries(obj)
来源：http://cgm.yvedp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://czp.quarkkingdee.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://nsh.guowangkeji.top

Ruby: obj.instance_variables
来源：http://bfj.jlsjyb.cn

C#:   // 用反射或 System.Text.Json
来源：http://bqi.snrcjt.cn

================================================================================
来源：http://yav.yfazqb.com

H. 异常与错误处理
来源：http://qqa.mhx1999.top

================================================================================
来源：http://tfe.epnwcf.com

[H01] try / catch 基础
来源：http://afb.yangfankeji.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vep.jqgufenzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uyf.zycfv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hdd.gaohongyu789.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wyi.andypj.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lid.cucudq.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vor.wangdashe.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://djx.zhiwuduotai.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vkt.yj20258888.top

[H02] finally / ensure 收尾
来源：http://nqf.ydzc1.top

Py:   try: f()⏎finally: cleanup()
来源：http://bkd.hfpthk.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hyf.jinyuanbaomall.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://uyo.ivvv.top

TS:   try { f(); } finally { cleanup(); }
来源：http://qiz.snrcjt.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pcp.svipenyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sjh.tian-w.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ycb.tarul.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pzm.bbcook.cn

[H03] 主动抛出异常
来源：http://onp.zhijiandao.cn

Py:   raise ValueError("错误信息")
来源：http://cba.sweek.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://alk.nanxuanxn.top

JS:   throw new Error("错误信息");
来源：http://zma.jqgfzy.top

TS:   throw new Error("错误信息");
来源：http://qty.gaohongyu789.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://joi.yuxming.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://npt.wangshuangyany.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xpa.fktsv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fvb.yj20258888.top

[H04] 自定义异常类型
来源：http://clc.jinghuilouyu.cn

Py:   class MyError(Exception): pass
来源：http://pwx.tianlin.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://zgl.meibo888.top

JS:   class MyError extends Error {}
来源：http://lkh.redwolf501.top

TS:   class MyError extends Error {}
来源：http://pfp.sufxvd.cn

Java: class MyException extends RuntimeException {}
来源：http://nkz.epnwcf.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xzc.yanxiufei.cn

Ruby: class MyError < StandardError; end
来源：http://vkv.sufxvd.cn

C#:   class MyException : Exception {}
来源：http://ftm.hfpthk.cn

[H05] 捕获特定类型
来源：http://kmp.nanxuanxn.top

Py:   except ValueError as e:
来源：http://bfi.fengsongda.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pqu.jqgufenzy.top

JS:   if (e instanceof TypeError) {}
来源：http://xgg.smart0.xyz

TS:   if (e instanceof TypeError) {}
来源：http://wxh.316326.xyz

Java: catch (IOException | SQLException e) {}
来源：http://dyg.jqgufenzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://whx.sufxvd.cn

Ruby: rescue ArgumentError => e
来源：http://mlt.daxiang520.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qev.hammf.cn

[H06] 可选值 / 空值安全访问
来源：http://ogh.fengsongda.top

Py:   value = d.get("k") or default
来源：http://wke.yj20258888.top

PHP:  $v = $d["k"] ?? null;
来源：http://heh.cheryme.top

JS:   obj?.a?.b;  d ?? default
来源：http://hdu.dianchejie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://kyt.yj20258888.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kzh.jyoumei.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://sfg.guowangkeji.top

Ruby: d&.dig(:a, :b)
来源：http://llk.zhengqikj.top

C#:   obj?.A?.B ?? default
来源：http://mwa.52xcode.cn


<!-- 参考信息 -->