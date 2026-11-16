代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vsk.hongshengwenyu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://evy.jlsjyb.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pwc.c1oappe.top

Ruby: File.read("a.txt")
来源：http://anc.sufxvd.cn

C#:   File.ReadAllText("a.txt");
来源：http://faw.cashguo.top

[F02] 逐行读取文件
来源：http://oib.jianghu66.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://eam.yvedp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wxk.sjlbkw.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wmd.redwolf501.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fjo.tanke756.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://smp.sufxvd.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fee.tianlin.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bic.cucudq.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://iag.bjfxy.top

[F03] 写入文件（覆盖）
来源：http://qgx.ydjk.org.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://voh.dashuyun.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xtw.jqgufenzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ghq.svipenyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kjk.jqgufenzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rim.yangfankeji.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zif.chenlongwang.top

Ruby: File.write("a.txt", "hi")
来源：http://abf.hcnkem.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lzr.cheryme.top

[F04] 追加写入文件
来源：http://zsq.ehwqpu.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://toy.shuidangran.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xmn.ehwqpu.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tve.cheryme.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zsg.daria6918.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kvw.zdbjq.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tjm.wangshuangyany.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sxw.9152youxi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://urk.sufxvd.cn

[F05] 判断文件或目录是否存在
来源：http://jpj.guannengcc.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nre.zycfv.cn

PHP:  file_exists("a.txt");
来源：http://fpy.feifeiyinyue.top

JS:   fs.existsSync("a.txt")
来源：http://jix.ehwqpu.com

TS:   fs.existsSync("a.txt")
来源：http://udg.jyoumei.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jjc.shangyingyoupin.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://adl.uphjek.com

Ruby: File.exist?("a.txt")
来源：http://bpq.vqdsnc.cn

C#:   File.Exists("a.txt")
来源：http://ghf.zdqjudy.top

[F06] 删除文件
来源：http://aqu.hnqzz.top

Py:   os.remove("a.txt")
来源：http://bka.feifeiyinyue.top

PHP:  unlink("a.txt");
来源：http://eyq.uphjek.com

JS:   fs.unlinkSync("a.txt")
来源：http://lvh.hfpthk.cn

TS:   fs.unlinkSync("a.txt")
来源：http://tdw.shzxlz.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mkp.sufxvd.cn

Go:   os.Remove("a.txt")
来源：http://dau.yuxming.cn

Ruby: File.delete("a.txt")
来源：http://vtd.jinqigfzy.top

C#:   File.Delete("a.txt");
来源：http://mlk.hongshengwenyu.top

[F07] 创建目录（含多级）
来源：http://ujh.9152youxi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ctn.chenlongwang.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://usx.yangfankeji.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ilk.snrcjt.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pwe.birdmap.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bdq.jqgfzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://owo.tarul.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fjx.316326.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rgo.cdnleiting.top

[F08] 遍历目录
来源：http://tle.fanxiaobao.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://zgb.pycfn.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pof.yuxming.cn

JS:   fs.readdirSync("dir")
来源：http://fij.daxiang520.top

TS:   fs.readdirSync("dir")
来源：http://vhr.zycfv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ull.jinghuilouyu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://agt.tanke756.top

Ruby: Dir.children("dir")
来源：http://ddf.guowangkeji.top

C#:   Directory.GetFiles("dir")
来源：http://mkp.smart0.xyz

[F09] 获取文件大小
来源：http://xta.shanyushiyangkeji.top

Py:   os.path.getsize("a.txt")
来源：http://ttz.hysaishi.cn

PHP:  filesize("a.txt");
来源：http://xyw.fktsv.cn

JS:   fs.statSync("a.txt").size
来源：http://fpp.ppjwa.cn

TS:   fs.statSync("a.txt").size
来源：http://qbc.yanxiufei.cn

Java: Files.size(Path.of("a.txt"))
来源：http://whn.hfpthk.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vck.jlsjyb.cn

Ruby: File.size("a.txt")
来源：http://odi.hcnkem.com

C#:   new FileInfo("a.txt").Length
来源：http://bny.bjfxy.top

[F10] 取文件扩展名 / 文件名
来源：http://hit.bbcook.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gcs.nwbrower.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rbo.vqdsnc.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kvv.cheryme.top

TS:   path.extname("a.txt")
来源：http://hee.sufxvd.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kwd.uphjek.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://woy.vehdjk.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tsd.cdnleiting.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pfg.ctjpmb.com

[F11] 复制与移动文件
来源：http://ilm.yangfankeji.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sgt.cucudq.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jes.tanke756.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bwa.fanxiaobao.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://prj.ydjk.org.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ohp.havefunace.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xaq.fzhhl.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xrk.birdmap.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wee.jinghuilouyu.cn

[F12] CSV 读写
来源：http://ixg.hysaishi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://swp.chenlongwang.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pas.aizwys.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vya.yvedp.cn

TS:   // 同上
来源：http://wtq.vehdjk.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://slx.zhengqikj.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mth.daxiang520.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eaf.sjlbkw.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nha.zhoulong.xyz

================================================================================
来源：http://tnv.svipenyu.cn

G. 面向对象
来源：http://vcr.chenjidiqi.icu

================================================================================
来源：http://ooo.hnxiangtu.top

[G01] 定义类
来源：http://zfv.yuxming.cn

Py:   class User: pass
来源：http://dim.epnwcf.com

PHP:  class User {}
来源：http://uxk.dashuyun.cn

JS:   class User {}
来源：http://jpu.xylfe.cn

TS:   class User { name: string = ""; }
来源：http://bkh.birdmap.top

Java: class User {}
来源：http://erh.hesvh.cn

Go:   type User struct { Name string }
来源：http://lyz.daxiang520.top

Ruby: class User; end
来源：http://wir.sweek.top

C#:   class User {}
来源：http://nac.guowangkeji.top

[G02] 构造函数
来源：http://exg.aizwys.cn

Py:   def __init__(self, name): self.name = name
来源：http://tna.bbcook.cn

PHP:  public function __construct(public string $name) {}
来源：http://qdc.jiagoushi.top

JS:   constructor(name) { this.name = name; }
来源：http://aaa.wangdashe.top

TS:   constructor(public name: string) {}
来源：http://fgr.jinghuilouyu.cn

Java: User(String name) { this.name = name; }
来源：http://nvd.zhaomingkeji.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cyt.fengsongda.top

Ruby: def initialize(name); @name = name; end
来源：http://ksa.yuxming.cn

C#:   public User(string name) { Name = name; }
来源：http://hvj.snrcjt.cn

[G03] 实例属性
来源：http://ebx.iojbl.cn

Py:   self.name = "x"
来源：http://fsg.52xcode.cn

PHP:  public string $name = "x";
来源：http://fpo.nwbrower.top

JS:   this.name = "x";
来源：http://big.52xcode.cn

TS:   name: string = "x";
来源：http://ank.zycfv.cn

Java: private String name;
来源：http://per.shzxlz.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kfq.wangshuangyany.cn

Ruby: @name = "x"
来源：http://tgc.zhengqikj.top

C#:   public string Name { get; set; } = "x";
来源：http://fno.gaohongyu789.top

[G04] 定义方法
来源：http://boe.iojbl.cn

Py:   def greet(self): return self.name
来源：http://rfj.316326.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://wmn.guowangkeji.top

JS:   greet() { return this.name; }
来源：http://kyz.chenlongwang.top

TS:   greet(): string { return this.name; }
来源：http://waz.zhixingplan.top

Java: String greet() { return name; }
来源：http://bmq.zycfv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zsy.feifeiyinyue.top

Ruby: def greet; @name; end
来源：http://mgl.zhengqikj.top

C#:   public string Greet() => Name;
来源：http://cap.daxiang520.top

[G05] 继承
来源：http://fsm.xuetiantiany.cn

Py:   class Admin(User): pass
来源：http://kha.xziqi.cn

PHP:  class Admin extends User {}
来源：http://tjy.iojbl.cn

JS:   class Admin extends User {}
来源：http://gip.shuidangran.top

TS:   class Admin extends User {}
来源：http://tix.wangshuangyany.cn

Java: class Admin extends User {}
来源：http://xsj.nwbrower.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xcg.shangyingyoupin.top

Ruby: class Admin < User; end
来源：http://tvk.redwolf501.top

C#:   class Admin : User {}
来源：http://tnc.andypj.xyz

[G06] 重写方法
来源：http://dev.316326.xyz

Py:   def greet(self): return "admin"
来源：http://obk.hywenlv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hwv.c1oappe.top

JS:   greet() { return "admin"; }
来源：http://naa.nanxinkj.top

TS:   greet(): string { return "admin"; }
来源：http://kqv.chenlongwang.top

Java: @Override String greet() { return "admin"; }
来源：http://ibh.9152youxi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://axp.yongpay.top

Ruby: def greet; "admin"; end
来源：http://ita.nwbrower.top

C#:   public override string Greet() => "admin";
来源：http://apu.jyoumei.cn

[G07] 调用父类方法
来源：http://iqb.gotoacloud.top

Py:   super().greet()
来源：http://ucf.dianchejie.cn

PHP:  parent::greet();
来源：http://oyb.iojbl.cn

JS:   super.greet();
来源：http://lpe.zhoulong.xyz

TS:   super.greet();
来源：http://exx.tianlin.xyz

Java: super.greet();
来源：http://fbh.yvedp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uxh.hammf.cn

Ruby: super
来源：http://kdt.iojbl.cn

C#:   base.Greet();
来源：http://yar.uphjek.com

[G08] 静态方法与属性
来源：http://ohw.zycfv.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vvx.guowangkeji.top

PHP:  public static function f() {}
来源：http://lcs.daxiang520.top

JS:   static f() {}
来源：http://cas.hywenlv.cn

TS:   static f(): void {}
来源：http://zky.wangshuangyany.cn

Java: static void f() {}
来源：http://qvv.hywenlv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://yfe.andypj.xyz

Ruby: def self.f; end
来源：http://upt.fehbvm.com

C#:   public static void F() {}
来源：http://fcy.daxiang520.top

[G09] 接口 / 抽象类
来源：http://oer.cdnleiting.top

Py:   from abc import ABC, abstractmethod
来源：http://scc.jlsjyb.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lyk.ydjk.org.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ntb.mhx1999.top

TS:   interface Shape { area(): number; }
来源：http://wsz.cashguo.top

Java: interface Shape { double area(); }
来源：http://dfc.zhijiandao.cn

Go:   type Shape interface { Area() float64 }
来源：http://gxj.wangdashe.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xfs.yj20258.top

C#:   interface IShape { double Area(); }
来源：http://qyn.jiagoushi.top

[G10] 访问控制
来源：http://jhm.xinyue.icu

Py:   约定 _protected / __private（不强制）
来源：http://fau.xuetiantiany.cn

PHP:  public / protected / private
来源：http://dgy.cheryme.top

JS:   #private 字段；其余公开
来源：http://rrv.shzxlz.cn

TS:   public / protected / private
来源：http://uhc.tanke756.top

Java: public / protected / private / 默认包级
来源：http://fwy.jlsjyb.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://von.hongshengwenyu.top

Ruby: public / protected / private
来源：http://lak.ydjk.org.cn

C#:   public / protected / private / internal
来源：http://wqk.guowangkeji.top

[G11] getter / setter
来源：http://wna.aizwys.cn

Py:   @property 与 @x.setter
来源：http://fzs.316326.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://wjj.nanxinkj.top

JS:   get name() { return this._name; }
来源：http://ldn.yfazqb.com

TS:   get name(): string { return this._name; }
来源：http://wot.mhx1999.top

Java: public String getName() { return name; }
来源：http://wvi.quarkkingdee.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://sym.xylfe.cn

Ruby: attr_accessor :name
来源：http://gle.fzhhl.top

C#:   public string Name { get; set; }
来源：http://egf.hammf.cn

[G12] 对象转字符串
来源：http://ykz.zdqjudy.top

Py:   def __str__(self): return self.name
来源：http://teb.tanke756.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://hyo.xziqi.cn

JS:   toString() { return this.name; }
来源：http://jqa.chenjidiqi.icu

TS:   toString(): string { return this.name; }
来源：http://rmt.cheryme.top

Java: @Override public String toString() { return name; }
来源：http://yak.hongshengwenyu.top

Go:   func (u User) String() string { return u.Name }
来源：http://fev.jinghuilouyu.cn

Ruby: def to_s; @name; end
来源：http://btc.yonumen.top

C#:   public override string ToString() => Name;
来源：http://ett.daria6918.cn

[G13] 判断对象类型
来源：http://mkx.gogol.net.cn

Py:   isinstance(u, User)
来源：http://cvo.ppjwa.cn

PHP:  $u instanceof User
来源：http://jgb.nanxuanxn.top

JS:   u instanceof User
来源：http://wzd.ppjwa.cn

TS:   u instanceof User
来源：http://fjj.yj20258888.top

Java: u instanceof User
来源：http://lni.andypj.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://fbu.snrcjt.cn

Ruby: u.is_a?(User)
来源：http://qnf.smart0.xyz

C#:   u is User
来源：http://hhr.xylfe.cn

[G14] 数据类 / record
来源：http://uur.yj20258.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hyg.havefunace.top

PHP:  // 用 readonly 属性模拟
来源：http://jdp.redwolf501.top

JS:   // 无内置：普通类或对象字面量
来源：http://ggv.daxiang520.top

TS:   type User = { name: string; age: number };
来源：http://wet.sufxvd.cn

Java: record User(String name, int age) {}
来源：http://hae.kuanghao11.cn

Go:   type User struct { Name string; Age int }
来源：http://rdg.quarkkingdee.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://elu.yj20258.top

C#:   record User(string Name, int Age);
来源：http://vrr.zhengqikj.top

[G15] 枚举
来源：http://rzl.hysaishi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ybo.hcnkem.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://dte.yongpay.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ehp.fengsongda.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gfv.tarul.cn

Java: enum Color { RED, GREEN }
来源：http://cow.guannengcc.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://eil.dianchejie.cn

Ruby: Color = %i[red green].freeze
来源：http://ivl.yj20258888.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lnx.ehwqpu.com

[G16] 对象转数组 / 字典
来源：http://nrm.jiagoushi.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rlo.jlsjyb.cn

PHP:  get_object_vars($obj);
来源：http://jdj.yj202588.top

JS:   Object.entries(obj)
来源：http://pqv.quarkkingdee.top

TS:   Object.entries(obj)
来源：http://ntr.wangdashe.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gmy.shanyushiyangkeji.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://cma.vehdjk.com

Ruby: obj.instance_variables
来源：http://yuc.dashuyun.cn

C#:   // 用反射或 System.Text.Json
来源：http://xxb.pengpengdd.cyou

================================================================================
来源：http://mzp.vehdjk.com

H. 异常与错误处理
来源：http://knc.yvedp.cn

================================================================================
来源：http://jxu.feifeiyinyue.top

[H01] try / catch 基础
来源：http://kfn.ctjpmb.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rwv.guowangkeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bco.chenlongwang.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vlr.zhiwuduotai.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jec.guannengcc.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rqf.dianchejie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nsx.zhengqikj.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rpi.yj20258.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://enx.yanxiufei.cn

[H02] finally / ensure 收尾
来源：http://mjo.hywenlv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://swf.fzhhl.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://sym.shanyushiyangkeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://mzd.nanxinkj.top

TS:   try { f(); } finally { cleanup(); }
来源：http://vpc.gogol.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://myb.fanxiaobao.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://can.tian-w.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ngk.yj202588.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://xfn.jinghuilouyu.cn

[H03] 主动抛出异常
来源：http://evr.bbcook.cn

Py:   raise ValueError("错误信息")
来源：http://yby.hcnkem.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ubr.dashuyun.cn

JS:   throw new Error("错误信息");
来源：http://yqi.jiagoushi.top

TS:   throw new Error("错误信息");
来源：http://pxi.smart0.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://qtf.cashguo.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://iav.cashguo.top

Ruby: raise ArgumentError, "错误信息"
来源：http://giz.ivvv.top

C#:   throw new ArgumentException("错误信息");
来源：http://kmv.sweek.top

[H04] 自定义异常类型
来源：http://jit.fktsv.cn

Py:   class MyError(Exception): pass
来源：http://kyd.jinghuilouyu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xwk.cheryme.top

JS:   class MyError extends Error {}
来源：http://cib.tianlin.xyz

TS:   class MyError extends Error {}
来源：http://xvc.cqqwz.cn

Java: class MyException extends RuntimeException {}
来源：http://foz.ybcxt.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lxo.yfazqb.com

Ruby: class MyError < StandardError; end
来源：http://dgw.zdbjq.cn

C#:   class MyException : Exception {}
来源：http://lfr.sweek.top

[H05] 捕获特定类型
来源：http://utw.yj20258888.top

Py:   except ValueError as e:
来源：http://mol.wangshuangyany.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://exa.gogol.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://aow.jinqigfzy.top

TS:   if (e instanceof TypeError) {}
来源：http://lqg.jinghuilouyu.cn

Java: catch (IOException | SQLException e) {}
来源：http://qjb.hcnkem.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ajc.shanyushiyangkeji.top

Ruby: rescue ArgumentError => e
来源：http://ffl.xuetiantiany.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://akc.zhongyouzk.top

[H06] 可选值 / 空值安全访问
来源：http://ibt.nwbrower.top


<!-- 参考信息 -->