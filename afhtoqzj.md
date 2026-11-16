代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vkz.andypj.xyz

Go:   // 按 rune 判断长度后截断
来源：http://baq.fzhhl.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ate.shuidangran.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qvk.cdnleiting.top

[E22] 字节长度与字符长度
来源：http://ojn.pengpengdd.cyou

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ulc.jinqigfzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ped.zhengqikj.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vet.ivvv.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bdd.jianghu66.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fmn.cashguo.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://idw.cheryme.top

Ruby: s.bytesize;  s.length
来源：http://xxs.zhongyouzk.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cjn.daxiang520.top

================================================================================
来源：http://cmz.aibaodan.cn

F. 文件与目录
来源：http://vrx.chenlongwang.top

================================================================================
来源：http://eaf.smart0.xyz

[F01] 读取整个文件
来源：http://vgr.tarul.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uss.sweek.top

PHP:  file_get_contents("a.txt");
来源：http://nhr.chenjidiqi.icu

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ayu.kuanghao11.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zzl.ppjwa.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rep.zhijiandao.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://won.xuetiantiany.cn

Ruby: File.read("a.txt")
来源：http://ltb.yvedp.cn

C#:   File.ReadAllText("a.txt");
来源：http://fwb.vqdsnc.cn

[F02] 逐行读取文件
来源：http://gyv.zdqjudy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ggv.shuidangran.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lgg.pycfn.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jst.dianchejie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jwf.zhengqikj.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vhz.ivvv.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kqe.ivvv.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qjx.guannengcc.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://eba.aizwys.cn

[F03] 写入文件（覆盖）
来源：http://sau.316326.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qcc.havefunace.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://qev.cdnleiting.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lym.zhixingplan.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uet.snrcjt.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ryd.gotoacloud.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kmq.hesvh.cn

Ruby: File.write("a.txt", "hi")
来源：http://dyh.tianlin.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kpe.cucudq.cn

[F04] 追加写入文件
来源：http://hlr.zdbjq.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pwj.zhengqikj.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hhx.316326.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tpd.aibaodan.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xdn.c1oappe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mpn.aibaodan.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rqz.hnqzz.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hvw.zhijiandao.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tly.jinqigfzy.top

[F05] 判断文件或目录是否存在
来源：http://hhh.snrcjt.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://okf.jinqigufen.top

PHP:  file_exists("a.txt");
来源：http://dce.xuanzx.com

JS:   fs.existsSync("a.txt")
来源：http://rnh.9152youxi.cn

TS:   fs.existsSync("a.txt")
来源：http://zki.cdnleiting.top

Java: Files.exists(Path.of("a.txt"))
来源：http://pwu.chenjidiqi.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cnk.yuxming.cn

Ruby: File.exist?("a.txt")
来源：http://dgg.daria6918.cn

C#:   File.Exists("a.txt")
来源：http://dgs.sysykeji.top

[F06] 删除文件
来源：http://coy.chenzaomai.com

Py:   os.remove("a.txt")
来源：http://xka.quarkkingdee.top

PHP:  unlink("a.txt");
来源：http://vyt.daria6918.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lme.sweek.top

TS:   fs.unlinkSync("a.txt")
来源：http://wqu.guannengcc.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://das.yangfankeji.com

Go:   os.Remove("a.txt")
来源：http://uyy.zhijiandao.cn

Ruby: File.delete("a.txt")
来源：http://tvp.pycfn.com

C#:   File.Delete("a.txt");
来源：http://luv.jqgufenzy.top

[F07] 创建目录（含多级）
来源：http://eqv.yj20258888.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dab.jyoumei.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dug.zhengqikj.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jrp.hnxiangtu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xio.birdmap.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xkt.jqgufenzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sol.yj202588.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zny.cucudq.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pnl.sjlbkw.cn

[F08] 遍历目录
来源：http://jgp.cashguo.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://mkw.birdmap.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://eqo.daria6918.cn

JS:   fs.readdirSync("dir")
来源：http://bgd.hongshengwenyu.top

TS:   fs.readdirSync("dir")
来源：http://svs.nanxuanxn.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pux.yj20258888.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://clh.jinyuanbaomall.cn

Ruby: Dir.children("dir")
来源：http://ovn.ywan-chungtsiang.top

C#:   Directory.GetFiles("dir")
来源：http://nep.cheryme.top

[F09] 获取文件大小
来源：http://zwz.zhengqikj.top

Py:   os.path.getsize("a.txt")
来源：http://trv.cdnleiting.top

PHP:  filesize("a.txt");
来源：http://ofa.zycfv.cn

JS:   fs.statSync("a.txt").size
来源：http://rma.guannengcc.top

TS:   fs.statSync("a.txt").size
来源：http://jjt.ivvv.top

Java: Files.size(Path.of("a.txt"))
来源：http://zox.nanxinkj.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pqv.gotoacloud.top

Ruby: File.size("a.txt")
来源：http://mop.chenjidiqi.icu

C#:   new FileInfo("a.txt").Length
来源：http://owg.cucudq.cn

[F10] 取文件扩展名 / 文件名
来源：http://vus.wangshuangyany.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://inr.guannengcc.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://amq.zhijiandao.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://siq.yvedp.cn

TS:   path.extname("a.txt")
来源：http://ukz.zhaomingkeji.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tin.pycfn.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vfd.dianchejie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jrr.pycfn.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bbm.gotoacloud.top

[F11] 复制与移动文件
来源：http://taf.quarkkingdee.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://saj.zhiwuduotai.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qtj.shanyushiyangkeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gja.iojbl.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jjc.zhoulong.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://boh.tarul.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tyt.zdqjudy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qqm.xuanzx.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nqn.fanxiaobao.xyz

[F12] CSV 读写
来源：http://jlq.yj20258.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sft.fktsv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fby.xinyue.icu

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wqu.jqgufenzy.top

TS:   // 同上
来源：http://yjr.xingfuxueyuan.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oiv.hysaishi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ehq.hammf.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://low.aibaodan.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kfy.yuanzhike.top

================================================================================
来源：http://jcu.zycfv.cn

G. 面向对象
来源：http://psm.yangfankeji.com

================================================================================
来源：http://wjh.yonumen.top

[G01] 定义类
来源：http://phm.cdnleiting.top

Py:   class User: pass
来源：http://arc.jqgfzy.top

PHP:  class User {}
来源：http://zwt.andypj.xyz

JS:   class User {}
来源：http://puz.snrcjt.cn

TS:   class User { name: string = ""; }
来源：http://kma.0kj1m.cn

Java: class User {}
来源：http://pgu.zhongyouzk.top

Go:   type User struct { Name string }
来源：http://fkz.316326.xyz

Ruby: class User; end
来源：http://cob.feifeiyinyue.top

C#:   class User {}
来源：http://dun.yangfankeji.com

[G02] 构造函数
来源：http://emg.jiagoushi.top

Py:   def __init__(self, name): self.name = name
来源：http://yur.shanyushiyangtech.top

PHP:  public function __construct(public string $name) {}
来源：http://ajb.fanxiaobao.xyz

JS:   constructor(name) { this.name = name; }
来源：http://osg.gotoacloud.top

TS:   constructor(public name: string) {}
来源：http://zhb.chenzaomai.com

Java: User(String name) { this.name = name; }
来源：http://nhj.hfpthk.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hya.zhaomingkeji.xyz

Ruby: def initialize(name); @name = name; end
来源：http://osn.jqgufenzy.top

C#:   public User(string name) { Name = name; }
来源：http://lul.cucudq.cn

[G03] 实例属性
来源：http://jqg.52xcode.cn

Py:   self.name = "x"
来源：http://vrv.ywan-chungtsiang.top

PHP:  public string $name = "x";
来源：http://yqn.quarkkingdee.top

JS:   this.name = "x";
来源：http://awh.quarkkingdee.top

TS:   name: string = "x";
来源：http://iss.fehbvm.com

Java: private String name;
来源：http://sow.jyoumei.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wbx.fktsv.cn

Ruby: @name = "x"
来源：http://eve.wangshuangyany.cn

C#:   public string Name { get; set; } = "x";
来源：http://cfe.dashuyun.cn

[G04] 定义方法
来源：http://bru.jianghu66.top

Py:   def greet(self): return self.name
来源：http://vtw.guannengcc.top

PHP:  public function greet(): string { return $this->name; }
来源：http://uwd.tanke756.top

JS:   greet() { return this.name; }
来源：http://kjd.fehbvm.com

TS:   greet(): string { return this.name; }
来源：http://twp.hammf.cn

Java: String greet() { return name; }
来源：http://suh.chenlongwang.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://yqd.uphjek.com

Ruby: def greet; @name; end
来源：http://krx.ydjk.org.cn

C#:   public string Greet() => Name;
来源：http://nok.uphjek.com

[G05] 继承
来源：http://rmw.zhongyouzk.top

Py:   class Admin(User): pass
来源：http://gma.smart0.xyz

PHP:  class Admin extends User {}
来源：http://hje.yangfankeji.com

JS:   class Admin extends User {}
来源：http://tgm.snrcjt.cn

TS:   class Admin extends User {}
来源：http://nmd.cqqwz.cn

Java: class Admin extends User {}
来源：http://qwr.zhixingplan.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xqt.redwolf501.top

Ruby: class Admin < User; end
来源：http://kbj.yj202588.top

C#:   class Admin : User {}
来源：http://ulk.wangdashe.top

[G06] 重写方法
来源：http://xhm.yvedp.cn

Py:   def greet(self): return "admin"
来源：http://xek.vqdsnc.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vkv.tanke756.top

JS:   greet() { return "admin"; }
来源：http://oyn.kuanghao11.cn

TS:   greet(): string { return "admin"; }
来源：http://zux.fehbvm.com

Java: @Override String greet() { return "admin"; }
来源：http://wjz.vehdjk.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zlc.jiagoushi.top

Ruby: def greet; "admin"; end
来源：http://vmy.zhoulong.xyz

C#:   public override string Greet() => "admin";
来源：http://qgl.tanke756.top

[G07] 调用父类方法
来源：http://bfu.ppjwa.cn

Py:   super().greet()
来源：http://ran.tarul.cn

PHP:  parent::greet();
来源：http://bww.hfpthk.cn

JS:   super.greet();
来源：http://oqi.sjlbkw.cn

TS:   super.greet();
来源：http://yfe.shanyushiyangtech.top

Java: super.greet();
来源：http://gzh.chenjidiqi.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dum.cheryme.top

Ruby: super
来源：http://ojz.cqqwz.cn

C#:   base.Greet();
来源：http://ben.yfazqb.com

[G08] 静态方法与属性
来源：http://znx.bjfxy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bvz.redwolf501.top

PHP:  public static function f() {}
来源：http://exi.pengpengdd.cyou

JS:   static f() {}
来源：http://caq.ivvv.top

TS:   static f(): void {}
来源：http://wly.andypj.xyz

Java: static void f() {}
来源：http://mrz.shanyushiyangkeji.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://nyb.chenlongwang.top

Ruby: def self.f; end
来源：http://atq.hysaishi.cn

C#:   public static void F() {}
来源：http://cox.zhiwuduotai.top

[G09] 接口 / 抽象类
来源：http://jky.xinyue.icu

Py:   from abc import ABC, abstractmethod
来源：http://cbw.zhiwuduotai.top

PHP:  interface Shape { public function area(): float; }
来源：http://cex.tarul.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pqr.xziqi.cn

TS:   interface Shape { area(): number; }
来源：http://jsk.jinqigfzy.top

Java: interface Shape { double area(); }
来源：http://egd.yuxming.cn

Go:   type Shape interface { Area() float64 }
来源：http://nit.jyoumei.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://moh.yueranfly.top

C#:   interface IShape { double Area(); }
来源：http://bwe.daria6918.cn

[G10] 访问控制
来源：http://vus.haohaochexian.top

Py:   约定 _protected / __private（不强制）
来源：http://yjl.zhiwuduotai.top

PHP:  public / protected / private
来源：http://qrw.sufxvd.cn

JS:   #private 字段；其余公开
来源：http://vgw.yuanzhike.top

TS:   public / protected / private
来源：http://ilh.andypj.xyz

Java: public / protected / private / 默认包级
来源：http://zpj.bbcook.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bbx.gzhubu.top

Ruby: public / protected / private
来源：http://hgd.sufxvd.cn

C#:   public / protected / private / internal
来源：http://tfe.jqgfzy.top

[G11] getter / setter
来源：http://dsv.sysykeji.top

Py:   @property 与 @x.setter
来源：http://dnp.jiagoushi.top

PHP:  public function getName(): string { return $this->name; }
来源：http://rmi.c1oappe.top

JS:   get name() { return this._name; }
来源：http://cps.jlsjyb.cn

TS:   get name(): string { return this._name; }
来源：http://yvq.xuanzx.com

Java: public String getName() { return name; }
来源：http://wio.nanxuanxn.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://mgn.cqqwz.cn

Ruby: attr_accessor :name
来源：http://vqq.ctjpmb.com

C#:   public string Name { get; set; }
来源：http://six.shzxlz.cn

[G12] 对象转字符串
来源：http://nxj.xziqi.cn

Py:   def __str__(self): return self.name
来源：http://niz.316326.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://dhd.tianlin.xyz

JS:   toString() { return this.name; }
来源：http://mfn.ywan-chungtsiang.top

TS:   toString(): string { return this.name; }
来源：http://frp.sufxvd.cn

Java: @Override public String toString() { return name; }
来源：http://pab.bbcook.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hvq.shangyingyoupin.top

Ruby: def to_s; @name; end
来源：http://xtb.zhoulong.xyz

C#:   public override string ToString() => Name;
来源：http://ptx.gotoacloud.top

[G13] 判断对象类型
来源：http://qwm.dianchejie.cn

Py:   isinstance(u, User)
来源：http://shr.hfpthk.cn

PHP:  $u instanceof User
来源：http://dtc.vehdjk.com

JS:   u instanceof User
来源：http://bni.yuanzhike.top

TS:   u instanceof User
来源：http://wza.zhongyouzk.top

Java: u instanceof User
来源：http://xpy.shanyushiyangkeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://cxf.sufxvd.cn

Ruby: u.is_a?(User)
来源：http://bsr.fanxiaobao.xyz

C#:   u is User
来源：http://xgt.daxiang520.top

[G14] 数据类 / record
来源：http://ugz.yuxming.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://aqg.jinghuilouyu.cn

PHP:  // 用 readonly 属性模拟
来源：http://dcj.nanxinkj.top

JS:   // 无内置：普通类或对象字面量
来源：http://hpz.ivvv.top

TS:   type User = { name: string; age: number };
来源：http://dve.tarul.cn

Java: record User(String name, int age) {}
来源：http://mqn.snrcjt.cn

Go:   type User struct { Name string; Age int }
来源：http://hvv.yfazqb.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zzi.ywan-chungtsiang.top

C#:   record User(string Name, int Age);
来源：http://ajc.hcnkem.com

[G15] 枚举
来源：http://xgh.xziqi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mee.nanxuanxn.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://guf.hcnkem.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yyd.jinghuilouyu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ogw.nwbrower.top

Java: enum Color { RED, GREEN }
来源：http://pul.52xcode.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hvx.yuanzhike.top

Ruby: Color = %i[red green].freeze
来源：http://iei.havefunace.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jaz.andypj.xyz

[G16] 对象转数组 / 字典
来源：http://wdd.kuanghao11.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hku.c1oappe.top

PHP:  get_object_vars($obj);
来源：http://klp.cdnleiting.top

JS:   Object.entries(obj)
来源：http://dbf.jyoumei.cn

TS:   Object.entries(obj)
来源：http://yzo.jinghuilouyu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hpd.zhiwuduotai.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://nqp.fengsongda.top

Ruby: obj.instance_variables
来源：http://ebd.fengsongda.top

C#:   // 用反射或 System.Text.Json
来源：http://pge.ywan-chungtsiang.top

================================================================================
来源：http://htx.hywenlv.cn

H. 异常与错误处理
来源：http://dth.chenjidiqi.icu

================================================================================
来源：http://gpu.nwbrower.top

[H01] try / catch 基础
来源：http://kkw.hammf.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tvb.daria6918.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zsl.dianchejie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cgi.ivvv.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ewl.zhijiandao.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://aqq.zdbjq.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sbi.hesvh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hbt.sjlbkw.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fxm.fengsongda.top

[H02] finally / ensure 收尾
来源：http://fbx.zhiwuduotai.top

Py:   try: f()⏎finally: cleanup()
来源：http://puq.9152youxi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://dbl.cqqwz.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://txy.sjlbkw.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://epz.jinghuilouyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://rmy.nanxinkj.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://mbo.cheryme.top

Ruby: begin; f; ensure; cleanup; end
来源：http://tlz.yfazqb.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://xcz.hnqzz.top

[H03] 主动抛出异常
来源：http://gfc.iojbl.cn

Py:   raise ValueError("错误信息")
来源：http://ylg.chenjidiqi.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vsq.bbcook.cn

JS:   throw new Error("错误信息");
来源：http://pok.fehbvm.com

TS:   throw new Error("错误信息");
来源：http://bsx.gzhubu.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://slu.cheryme.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pep.shanyushiyangkeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://kxf.zhoulong.xyz


<!-- 参考信息 -->