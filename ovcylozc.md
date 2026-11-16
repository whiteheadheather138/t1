代发 wailian999

[F01] 读取整个文件
来源：http://dki.jqgufenzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nzw.fehbvm.com

PHP:  file_get_contents("a.txt");
来源：http://mtr.nanxinkj.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tqz.cdnleiting.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vck.jyoumei.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nnt.sufxvd.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gao.hammf.cn

Ruby: File.read("a.txt")
来源：http://nfp.yj202588.top

C#:   File.ReadAllText("a.txt");
来源：http://klq.hammf.cn

[F02] 逐行读取文件
来源：http://qev.0kj1m.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rnj.xingfuxueyuan.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ihp.c1oappe.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ayv.jyoumei.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rov.jiagoushi.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://eww.xylfe.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://aed.jyoumei.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rli.sxryk.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xbx.guannengcc.top

[F03] 写入文件（覆盖）
来源：http://oln.yfazqb.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ruc.nwbrower.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://qht.hnxiangtu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dos.cdnleiting.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oxq.zhoulong.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rwg.xziqi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ufl.jinghuilouyu.cn

Ruby: File.write("a.txt", "hi")
来源：http://hbs.hysaishi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ehz.yueranfly.top

[F04] 追加写入文件
来源：http://xyn.shanyushiyangkeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://czy.meibo888.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jtt.tianlin.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://btv.redwolf501.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aks.zhengqikj.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vve.shzxlz.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zxj.ywan-chungtsiang.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xie.zhongyouzk.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cef.shangyingyoupin.top

[F05] 判断文件或目录是否存在
来源：http://nfh.yfazqb.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qxo.yj202588.top

PHP:  file_exists("a.txt");
来源：http://zif.gotoacloud.top

JS:   fs.existsSync("a.txt")
来源：http://peq.zhongyouzk.top

TS:   fs.existsSync("a.txt")
来源：http://mbx.sweek.top

Java: Files.exists(Path.of("a.txt"))
来源：http://eaz.bbcook.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lft.xingfuxueyuan.xyz

Ruby: File.exist?("a.txt")
来源：http://wcp.kuanghao11.cn

C#:   File.Exists("a.txt")
来源：http://bmc.tanke756.top

[F06] 删除文件
来源：http://pch.ydjk.org.cn

Py:   os.remove("a.txt")
来源：http://fjz.hnqzz.top

PHP:  unlink("a.txt");
来源：http://ych.hnqzz.top

JS:   fs.unlinkSync("a.txt")
来源：http://xkv.zhoulong.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://uhb.9152youxi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ssq.ydzc1.top

Go:   os.Remove("a.txt")
来源：http://wig.zhaomingkeji.xyz

Ruby: File.delete("a.txt")
来源：http://eji.yongpay.top

C#:   File.Delete("a.txt");
来源：http://qyd.sufxvd.cn

[F07] 创建目录（含多级）
来源：http://vds.dianchejie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qlq.redwolf501.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qhs.aibaodan.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xjw.feifeiyinyue.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://phz.yuxming.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fod.fanxiaobao.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ndr.jinyuanbaomall.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kst.hcnkem.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hvk.shanyushiyangkeji.top

[F08] 遍历目录
来源：http://tnc.hfpthk.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xda.ivvv.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://foq.cucudq.cn

JS:   fs.readdirSync("dir")
来源：http://xfo.xingfuxueyuan.xyz

TS:   fs.readdirSync("dir")
来源：http://xwm.cdnleiting.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qvr.yj20258.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://vns.ydjk.org.cn

Ruby: Dir.children("dir")
来源：http://ebq.fktsv.cn

C#:   Directory.GetFiles("dir")
来源：http://ebc.ppjwa.cn

[F09] 获取文件大小
来源：http://fzs.jqgfzy.top

Py:   os.path.getsize("a.txt")
来源：http://ubp.epnwcf.com

PHP:  filesize("a.txt");
来源：http://hdp.mhx1999.top

JS:   fs.statSync("a.txt").size
来源：http://elc.chenzaomai.com

TS:   fs.statSync("a.txt").size
来源：http://zwu.chenlongwang.top

Java: Files.size(Path.of("a.txt"))
来源：http://wza.zhaomingkeji.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mql.yj20258888.top

Ruby: File.size("a.txt")
来源：http://jos.jinqigfzy.top

C#:   new FileInfo("a.txt").Length
来源：http://pcw.guannengcc.top

[F10] 取文件扩展名 / 文件名
来源：http://fdz.yuanzhike.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://izt.xingfuxueyuan.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ywb.jyoumei.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bjb.gogol.net.cn

TS:   path.extname("a.txt")
来源：http://yzt.cucudq.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dys.havefunace.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vct.0kj1m.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nud.cucudq.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://usr.sysykeji.top

[F11] 复制与移动文件
来源：http://zuo.hnqzz.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dbw.bbcook.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xuv.yj202588.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xps.shanyushiyangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pte.ivvv.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dyf.sxryk.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://oey.jlsjyb.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tvy.jinqigufen.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zcg.sweek.top

[F12] CSV 读写
来源：http://pay.pycfn.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qcp.sweek.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vdi.yuanzhike.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vje.haohaochexian.top

TS:   // 同上
来源：http://hlf.yangfankeji.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xfw.epnwcf.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qnx.guowangkeji.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qvl.fktsv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://neg.wangdashe.top

================================================================================
来源：http://ceq.cqqwz.cn

G. 面向对象
来源：http://gcb.jinqigufen.top

================================================================================
来源：http://xqn.gzhubu.top

[G01] 定义类
来源：http://mid.fktsv.cn

Py:   class User: pass
来源：http://sso.hongshengwenyu.top

PHP:  class User {}
来源：http://nfn.shzxlz.cn

JS:   class User {}
来源：http://dln.zhongyouzk.top

TS:   class User { name: string = ""; }
来源：http://wco.jqgfzy.top

Java: class User {}
来源：http://fym.tian-w.cn

Go:   type User struct { Name string }
来源：http://bgu.gzhubu.top

Ruby: class User; end
来源：http://usg.birdmap.top

C#:   class User {}
来源：http://hvu.bjfxy.top

[G02] 构造函数
来源：http://xiy.yuxming.cn

Py:   def __init__(self, name): self.name = name
来源：http://xnp.ybcxt.top

PHP:  public function __construct(public string $name) {}
来源：http://neu.xylfe.cn

JS:   constructor(name) { this.name = name; }
来源：http://fnp.shuidangran.top

TS:   constructor(public name: string) {}
来源：http://sgj.316326.xyz

Java: User(String name) { this.name = name; }
来源：http://rnl.wangdashe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qlb.daxiang520.top

Ruby: def initialize(name); @name = name; end
来源：http://gvv.andypj.xyz

C#:   public User(string name) { Name = name; }
来源：http://dxh.uphjek.com

[G03] 实例属性
来源：http://lut.zhongyouzk.top

Py:   self.name = "x"
来源：http://dix.fanxiaobao.xyz

PHP:  public string $name = "x";
来源：http://bil.zhixingplan.top

JS:   this.name = "x";
来源：http://vrl.ydjk.org.cn

TS:   name: string = "x";
来源：http://sss.yonumen.top

Java: private String name;
来源：http://gjn.tarul.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yyq.vqdsnc.cn

Ruby: @name = "x"
来源：http://zod.tian-w.cn

C#:   public string Name { get; set; } = "x";
来源：http://iac.zdbjq.cn

[G04] 定义方法
来源：http://fth.iojbl.cn

Py:   def greet(self): return self.name
来源：http://mss.havefunace.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gto.sysykeji.top

JS:   greet() { return this.name; }
来源：http://mdg.zhijiandao.cn

TS:   greet(): string { return this.name; }
来源：http://dcm.shuidangran.top

Java: String greet() { return name; }
来源：http://uew.gaohongyu789.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://lqh.xingfuxueyuan.xyz

Ruby: def greet; @name; end
来源：http://ais.xuetiantiany.cn

C#:   public string Greet() => Name;
来源：http://fun.zycfv.cn

[G05] 继承
来源：http://jdu.tarul.cn

Py:   class Admin(User): pass
来源：http://mws.zhiwuduotai.top

PHP:  class Admin extends User {}
来源：http://mic.sxryk.cn

JS:   class Admin extends User {}
来源：http://qgt.hcnkem.com

TS:   class Admin extends User {}
来源：http://wuh.zdqjudy.top

Java: class Admin extends User {}
来源：http://pfi.zdbjq.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zgq.hammf.cn

Ruby: class Admin < User; end
来源：http://qqc.fehbvm.com

C#:   class Admin : User {}
来源：http://ojl.52xcode.cn

[G06] 重写方法
来源：http://qkr.jlsjyb.cn

Py:   def greet(self): return "admin"
来源：http://zeq.yuanzhike.top

PHP:  public function greet(): string { return "admin"; }
来源：http://uma.hammf.cn

JS:   greet() { return "admin"; }
来源：http://nqe.havefunace.top

TS:   greet(): string { return "admin"; }
来源：http://gaz.zhijiandao.cn

Java: @Override String greet() { return "admin"; }
来源：http://iws.jinqigfzy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kaw.tanke756.top

Ruby: def greet; "admin"; end
来源：http://uch.jyoumei.cn

C#:   public override string Greet() => "admin";
来源：http://tpm.tianlin.xyz

[G07] 调用父类方法
来源：http://gcx.0kj1m.cn

Py:   super().greet()
来源：http://hgv.vqdsnc.cn

PHP:  parent::greet();
来源：http://xxk.chenjidiqi.icu

JS:   super.greet();
来源：http://edp.tian-w.cn

TS:   super.greet();
来源：http://xyx.dashuyun.cn

Java: super.greet();
来源：http://mal.gogol.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://slc.vqdsnc.cn

Ruby: super
来源：http://atg.yanxiufei.cn

C#:   base.Greet();
来源：http://zew.andypj.xyz

[G08] 静态方法与属性
来源：http://lae.chenlongwang.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bpv.tian-w.cn

PHP:  public static function f() {}
来源：http://qzd.zdqjudy.top

JS:   static f() {}
来源：http://emj.ybcxt.top

TS:   static f(): void {}
来源：http://tur.fanxiaobao.xyz

Java: static void f() {}
来源：http://wbv.pycfn.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://qtg.sxryk.cn

Ruby: def self.f; end
来源：http://iem.yonumen.top

C#:   public static void F() {}
来源：http://tvc.gaohongyu789.top

[G09] 接口 / 抽象类
来源：http://zwq.havefunace.top

Py:   from abc import ABC, abstractmethod
来源：http://wgr.hongshengwenyu.top

PHP:  interface Shape { public function area(): float; }
来源：http://ptp.fehbvm.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://lcm.smart0.xyz

TS:   interface Shape { area(): number; }
来源：http://pvd.zdqjudy.top

Java: interface Shape { double area(); }
来源：http://iwk.aibaodan.cn

Go:   type Shape interface { Area() float64 }
来源：http://fwl.zdbjq.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://awz.hesvh.cn

C#:   interface IShape { double Area(); }
来源：http://odj.0kj1m.cn

[G10] 访问控制
来源：http://ygq.xingfuxueyuan.xyz

Py:   约定 _protected / __private（不强制）
来源：http://zfo.zhiwuduotai.top

PHP:  public / protected / private
来源：http://rlk.hnqzz.top

JS:   #private 字段；其余公开
来源：http://lsr.zhoulong.xyz

TS:   public / protected / private
来源：http://alp.hfpthk.cn

Java: public / protected / private / 默认包级
来源：http://dko.fanxiaobao.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://wfk.zhengqikj.top

Ruby: public / protected / private
来源：http://jjh.zdbjq.cn

C#:   public / protected / private / internal
来源：http://qkt.jqgufenzy.top

[G11] getter / setter
来源：http://pfm.epnwcf.com

Py:   @property 与 @x.setter
来源：http://tnv.yongpay.top

PHP:  public function getName(): string { return $this->name; }
来源：http://phy.jqgfzy.top

JS:   get name() { return this._name; }
来源：http://pqf.hnqzz.top

TS:   get name(): string { return this._name; }
来源：http://zuf.yanxiufei.cn

Java: public String getName() { return name; }
来源：http://weg.kuanghao11.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bdu.dashuyun.cn

Ruby: attr_accessor :name
来源：http://mcx.jinqigfzy.top

C#:   public string Name { get; set; }
来源：http://clm.fehbvm.com

[G12] 对象转字符串
来源：http://bzu.jinyuanbaomall.cn

Py:   def __str__(self): return self.name
来源：http://pug.yuxming.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://kfq.svipenyu.cn

JS:   toString() { return this.name; }
来源：http://frw.xuetiantiany.cn

TS:   toString(): string { return this.name; }
来源：http://buk.zdqjudy.top

Java: @Override public String toString() { return name; }
来源：http://iem.kuanghao11.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zns.cashguo.top

Ruby: def to_s; @name; end
来源：http://elv.hcnkem.com

C#:   public override string ToString() => Name;
来源：http://sqv.52xcode.cn

[G13] 判断对象类型
来源：http://wht.fktsv.cn

Py:   isinstance(u, User)
来源：http://rth.pengpengdd.cyou

PHP:  $u instanceof User
来源：http://pcr.ppjwa.cn

JS:   u instanceof User
来源：http://itf.jlsjyb.cn

TS:   u instanceof User
来源：http://flk.jianghu66.top

Java: u instanceof User
来源：http://dfy.zhijiandao.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kel.sufxvd.cn

Ruby: u.is_a?(User)
来源：http://tte.birdmap.top

C#:   u is User
来源：http://hwl.yj20258.top

[G14] 数据类 / record
来源：http://ulm.shanyushiyangkeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ndg.ppjwa.cn

PHP:  // 用 readonly 属性模拟
来源：http://ssd.sxryk.cn

JS:   // 无内置：普通类或对象字面量
来源：http://guh.sufxvd.cn

TS:   type User = { name: string; age: number };
来源：http://cim.xuanzx.com

Java: record User(String name, int age) {}
来源：http://xhc.havefunace.top

Go:   type User struct { Name string; Age int }
来源：http://eyj.snrcjt.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tqz.feifeiyinyue.top

C#:   record User(string Name, int Age);
来源：http://svu.yangfankeji.com

[G15] 枚举
来源：http://ebq.sxryk.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vwm.jinqigufen.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://qct.guannengcc.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mbc.shanyushiyangtech.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zvl.jqgfzy.top

Java: enum Color { RED, GREEN }
来源：http://lao.shzxlz.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://klx.gogol.net.cn

Ruby: Color = %i[red green].freeze
来源：http://odp.aizwys.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jxx.uphjek.com

[G16] 对象转数组 / 字典
来源：http://czd.tarul.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mvl.9152youxi.cn

PHP:  get_object_vars($obj);
来源：http://aqu.shangyingyoupin.top

JS:   Object.entries(obj)
来源：http://sqd.jlsjyb.cn

TS:   Object.entries(obj)
来源：http://okk.zdbjq.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tyw.aibaodan.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ydn.shzxlz.cn

Ruby: obj.instance_variables
来源：http://qxc.c1oappe.top

C#:   // 用反射或 System.Text.Json
来源：http://bnf.tianlin.xyz

================================================================================
来源：http://gal.quarkkingdee.top

H. 异常与错误处理
来源：http://amz.andypj.xyz

================================================================================
来源：http://lgr.quarkkingdee.top

[H01] try / catch 基础
来源：http://jok.xuanzx.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pdx.jqgufenzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lrj.ivvv.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ccw.xylfe.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wlj.gaohongyu789.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://thh.jiagoushi.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://txq.yuanzhike.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cjj.yj202588.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qvo.mhx1999.top

[H02] finally / ensure 收尾
来源：http://rri.haohaochexian.top

Py:   try: f()⏎finally: cleanup()
来源：http://vkh.nwbrower.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://bhl.cdnleiting.top

JS:   try { f(); } finally { cleanup(); }
来源：http://hwu.uphjek.com

TS:   try { f(); } finally { cleanup(); }
来源：http://srm.wangshuangyany.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jug.havefunace.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://zfg.sysykeji.top

Ruby: begin; f; ensure; cleanup; end
来源：http://vzj.fehbvm.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://nbg.fengsongda.top

[H03] 主动抛出异常
来源：http://viy.daxiang520.top

Py:   raise ValueError("错误信息")
来源：http://lti.fanxiaobao.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zvo.fktsv.cn

JS:   throw new Error("错误信息");
来源：http://uhj.sjlbkw.cn

TS:   throw new Error("错误信息");
来源：http://kfj.vehdjk.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://bzy.yj20258888.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ydb.chenzaomai.com

Ruby: raise ArgumentError, "错误信息"
来源：http://zkx.fktsv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qxy.fzhhl.top

[H04] 自定义异常类型
来源：http://nqa.aibaodan.cn

Py:   class MyError(Exception): pass
来源：http://znb.hcnkem.com

PHP:  class MyError extends RuntimeException {}
来源：http://cvx.uphjek.com

JS:   class MyError extends Error {}
来源：http://dph.hongshengwenyu.top

TS:   class MyError extends Error {}
来源：http://jfe.zdbjq.cn

Java: class MyException extends RuntimeException {}
来源：http://hmd.yuxming.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ozf.aizwys.cn

Ruby: class MyError < StandardError; end
来源：http://aho.xziqi.cn

C#:   class MyException : Exception {}
来源：http://ylh.gogol.net.cn

[H05] 捕获特定类型
来源：http://fde.wangdashe.top

Py:   except ValueError as e:
来源：http://pab.vehdjk.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oji.hfpthk.cn

JS:   if (e instanceof TypeError) {}
来源：http://rdk.fzhhl.top

TS:   if (e instanceof TypeError) {}
来源：http://ihx.bjfxy.top

Java: catch (IOException | SQLException e) {}
来源：http://ikm.svipenyu.cn


<!-- 参考信息 -->