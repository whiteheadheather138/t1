代发 wailian999

[F01] 读取整个文件
来源：http://zvd.havefunace.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rax.ivvv.top

PHP:  file_get_contents("a.txt");
来源：http://ewh.yuxming.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://urx.vqdsnc.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rfd.ydjk.org.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://tym.jqgufenzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gwp.ydzc1.top

Ruby: File.read("a.txt")
来源：http://zqq.c1oappe.top

C#:   File.ReadAllText("a.txt");
来源：http://cin.jiagoushi.top

[F02] 逐行读取文件
来源：http://bek.bjfxy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rgz.gogol.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kpr.sjlbkw.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vst.sweek.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mck.jyoumei.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bmy.jyoumei.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jqk.nanxinkj.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://brk.nanxinkj.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://oua.haohaochexian.top

[F03] 写入文件（覆盖）
来源：http://yyd.zhiwuduotai.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://aqr.hesvh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ikp.yfazqb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iqx.jinghuilouyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vpx.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nwq.hcnkem.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://orb.xziqi.cn

Ruby: File.write("a.txt", "hi")
来源：http://anp.quarkkingdee.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oxy.jianghu66.top

[F04] 追加写入文件
来源：http://bru.birdmap.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wlh.316326.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://oiv.dianchejie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://opn.cheryme.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pws.wangdashe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ljk.0kj1m.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ucq.ywan-chungtsiang.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fez.xziqi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dfp.jinqigfzy.top

[F05] 判断文件或目录是否存在
来源：http://fmj.vehdjk.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lgw.vehdjk.com

PHP:  file_exists("a.txt");
来源：http://ysf.jinyuanbaomall.cn

JS:   fs.existsSync("a.txt")
来源：http://ecr.jinghuilouyu.cn

TS:   fs.existsSync("a.txt")
来源：http://bgw.yuanzhike.top

Java: Files.exists(Path.of("a.txt"))
来源：http://zad.epnwcf.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vml.nwbrower.top

Ruby: File.exist?("a.txt")
来源：http://haa.mhx1999.top

C#:   File.Exists("a.txt")
来源：http://heq.9152youxi.cn

[F06] 删除文件
来源：http://sth.zhaomingkeji.xyz

Py:   os.remove("a.txt")
来源：http://ush.tarul.cn

PHP:  unlink("a.txt");
来源：http://hwc.hysaishi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cpf.birdmap.top

TS:   fs.unlinkSync("a.txt")
来源：http://mxy.hfpthk.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vvu.ctjpmb.com

Go:   os.Remove("a.txt")
来源：http://yks.cheryme.top

Ruby: File.delete("a.txt")
来源：http://vtp.hongshengwenyu.top

C#:   File.Delete("a.txt");
来源：http://gld.cqqwz.cn

[F07] 创建目录（含多级）
来源：http://bhr.wangshuangyany.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://oqj.zhoulong.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mfc.vqdsnc.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jem.hysaishi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://asq.jinqigufen.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aub.feifeiyinyue.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dob.chenlongwang.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hjm.cashguo.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://utk.hfpthk.cn

[F08] 遍历目录
来源：http://fmw.yj20258.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://gaj.sufxvd.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nwo.zhoulong.xyz

JS:   fs.readdirSync("dir")
来源：http://vpy.ydjk.org.cn

TS:   fs.readdirSync("dir")
来源：http://nbe.yuxming.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dkn.bjfxy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://mlf.zhongyouzk.top

Ruby: Dir.children("dir")
来源：http://bep.jinqigufen.top

C#:   Directory.GetFiles("dir")
来源：http://rqs.nwbrower.top

[F09] 获取文件大小
来源：http://vyd.ywan-chungtsiang.top

Py:   os.path.getsize("a.txt")
来源：http://fdc.cashguo.top

PHP:  filesize("a.txt");
来源：http://wst.c1oappe.top

JS:   fs.statSync("a.txt").size
来源：http://ldh.quarkkingdee.top

TS:   fs.statSync("a.txt").size
来源：http://pjs.guannengcc.top

Java: Files.size(Path.of("a.txt"))
来源：http://zhz.jlsjyb.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ilp.yangfankeji.com

Ruby: File.size("a.txt")
来源：http://vgd.havefunace.top

C#:   new FileInfo("a.txt").Length
来源：http://cmx.cdnleiting.top

[F10] 取文件扩展名 / 文件名
来源：http://ynq.zhongyouzk.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zxd.havefunace.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dui.xingfuxueyuan.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uwl.andypj.xyz

TS:   path.extname("a.txt")
来源：http://gsh.fktsv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hnu.zdqjudy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fyb.hesvh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://eyr.ydzc1.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sth.aizwys.cn

[F11] 复制与移动文件
来源：http://tqr.xuetiantiany.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kya.tanke756.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pvd.tanke756.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gsu.cdnleiting.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pdp.dashuyun.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ywg.316326.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cmi.zycfv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hdk.316326.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cdp.hnqzz.top

[F12] CSV 读写
来源：http://vdo.ehwqpu.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://utm.zhixingplan.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hqm.sxryk.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://iqr.hfpthk.cn

TS:   // 同上
来源：http://olv.ydzc1.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uyf.yuanzhike.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bsc.zycfv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jya.birdmap.top

C#:   // 无内置：用 CsvHelper 库
来源：http://iyw.andypj.xyz

================================================================================
来源：http://alu.cqqwz.cn

G. 面向对象
来源：http://bdc.yueranfly.top

================================================================================
来源：http://meu.shangyingyoupin.top

[G01] 定义类
来源：http://ttr.cqqwz.cn

Py:   class User: pass
来源：http://neb.nanxinkj.top

PHP:  class User {}
来源：http://mmg.iojbl.cn

JS:   class User {}
来源：http://avh.xylfe.cn

TS:   class User { name: string = ""; }
来源：http://aks.svipenyu.cn

Java: class User {}
来源：http://cks.feifeiyinyue.top

Go:   type User struct { Name string }
来源：http://dhu.guannengcc.top

Ruby: class User; end
来源：http://jgq.feifeiyinyue.top

C#:   class User {}
来源：http://vlr.jinqigfzy.top

[G02] 构造函数
来源：http://iys.dashuyun.cn

Py:   def __init__(self, name): self.name = name
来源：http://qrb.nanxinkj.top

PHP:  public function __construct(public string $name) {}
来源：http://wad.iojbl.cn

JS:   constructor(name) { this.name = name; }
来源：http://hkn.xuetiantiany.cn

TS:   constructor(public name: string) {}
来源：http://yrz.hnqzz.top

Java: User(String name) { this.name = name; }
来源：http://hwi.aibaodan.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ota.redwolf501.top

Ruby: def initialize(name); @name = name; end
来源：http://sgo.jinghuilouyu.cn

C#:   public User(string name) { Name = name; }
来源：http://nkx.zhijiandao.cn

[G03] 实例属性
来源：http://hti.316326.xyz

Py:   self.name = "x"
来源：http://pwb.jlsjyb.cn

PHP:  public string $name = "x";
来源：http://tlw.nanxinkj.top

JS:   this.name = "x";
来源：http://ebm.zdbjq.cn

TS:   name: string = "x";
来源：http://oaq.sufxvd.cn

Java: private String name;
来源：http://xev.chenzaomai.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yoj.tarul.cn

Ruby: @name = "x"
来源：http://zhd.yj20258.top

C#:   public string Name { get; set; } = "x";
来源：http://bss.sjlbkw.cn

[G04] 定义方法
来源：http://eth.shzxlz.cn

Py:   def greet(self): return self.name
来源：http://rwo.cheryme.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ajo.snrcjt.cn

JS:   greet() { return this.name; }
来源：http://klt.yuxming.cn

TS:   greet(): string { return this.name; }
来源：http://klf.gaohongyu789.top

Java: String greet() { return name; }
来源：http://fce.sjlbkw.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://dkp.jqgufenzy.top

Ruby: def greet; @name; end
来源：http://tgj.daxiang520.top

C#:   public string Greet() => Name;
来源：http://ozm.zhongyouzk.top

[G05] 继承
来源：http://ida.hywenlv.cn

Py:   class Admin(User): pass
来源：http://itd.jinghuilouyu.cn

PHP:  class Admin extends User {}
来源：http://tno.jlsjyb.cn

JS:   class Admin extends User {}
来源：http://qkz.wangshuangyany.cn

TS:   class Admin extends User {}
来源：http://rte.birdmap.top

Java: class Admin extends User {}
来源：http://owg.jinyuanbaomall.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://snv.xingfuxueyuan.xyz

Ruby: class Admin < User; end
来源：http://zsf.tian-w.cn

C#:   class Admin : User {}
来源：http://xfl.yj20258888.top

[G06] 重写方法
来源：http://qng.epnwcf.com

Py:   def greet(self): return "admin"
来源：http://bqt.jinqigufen.top

PHP:  public function greet(): string { return "admin"; }
来源：http://nri.xylfe.cn

JS:   greet() { return "admin"; }
来源：http://qls.jyoumei.cn

TS:   greet(): string { return "admin"; }
来源：http://mde.yj20258888.top

Java: @Override String greet() { return "admin"; }
来源：http://yyh.hysaishi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ymc.jqgfzy.top

Ruby: def greet; "admin"; end
来源：http://wiq.xingfuxueyuan.xyz

C#:   public override string Greet() => "admin";
来源：http://ran.ydjk.org.cn

[G07] 调用父类方法
来源：http://vfe.fehbvm.com

Py:   super().greet()
来源：http://und.gaohongyu789.top

PHP:  parent::greet();
来源：http://cah.kuanghao11.cn

JS:   super.greet();
来源：http://eto.smart0.xyz

TS:   super.greet();
来源：http://eql.zdbjq.cn

Java: super.greet();
来源：http://wzu.zhijiandao.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lnf.zdqjudy.top

Ruby: super
来源：http://ejl.hysaishi.cn

C#:   base.Greet();
来源：http://fwn.fehbvm.com

[G08] 静态方法与属性
来源：http://dns.xziqi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xry.fengsongda.top

PHP:  public static function f() {}
来源：http://itp.bbcook.cn

JS:   static f() {}
来源：http://egv.xylfe.cn

TS:   static f(): void {}
来源：http://ukn.pycfn.com

Java: static void f() {}
来源：http://tqw.cheryme.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://gww.haohaochexian.top

Ruby: def self.f; end
来源：http://sbi.sysykeji.top

C#:   public static void F() {}
来源：http://mot.jiagoushi.top

[G09] 接口 / 抽象类
来源：http://qsm.snrcjt.cn

Py:   from abc import ABC, abstractmethod
来源：http://nfd.zhoulong.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://eeu.jiagoushi.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://wqj.sysykeji.top

TS:   interface Shape { area(): number; }
来源：http://ovf.ivvv.top

Java: interface Shape { double area(); }
来源：http://bpz.shzxlz.cn

Go:   type Shape interface { Area() float64 }
来源：http://ujz.hnxiangtu.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yyv.ehwqpu.com

C#:   interface IShape { double Area(); }
来源：http://ljb.zhaomingkeji.xyz

[G10] 访问控制
来源：http://osn.shanyushiyangkeji.top

Py:   约定 _protected / __private（不强制）
来源：http://gjc.hongshengwenyu.top

PHP:  public / protected / private
来源：http://kwu.tanke756.top

JS:   #private 字段；其余公开
来源：http://wjz.shangyingyoupin.top

TS:   public / protected / private
来源：http://cyi.yfazqb.com

Java: public / protected / private / 默认包级
来源：http://bfh.iojbl.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lcw.hnqzz.top

Ruby: public / protected / private
来源：http://kyk.xinyue.icu

C#:   public / protected / private / internal
来源：http://cmc.dashuyun.cn

[G11] getter / setter
来源：http://skr.guannengcc.top

Py:   @property 与 @x.setter
来源：http://iby.cucudq.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cua.zhoulong.xyz

JS:   get name() { return this._name; }
来源：http://zhq.hnxiangtu.top

TS:   get name(): string { return this._name; }
来源：http://jgs.nwbrower.top

Java: public String getName() { return name; }
来源：http://anc.hesvh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zbs.hammf.cn

Ruby: attr_accessor :name
来源：http://rof.jinyuanbaomall.cn

C#:   public string Name { get; set; }
来源：http://mca.aizwys.cn

[G12] 对象转字符串
来源：http://pof.chenlongwang.top

Py:   def __str__(self): return self.name
来源：http://sit.ybcxt.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://has.zdbjq.cn

JS:   toString() { return this.name; }
来源：http://ohb.gzhubu.top

TS:   toString(): string { return this.name; }
来源：http://xme.daxiang520.top

Java: @Override public String toString() { return name; }
来源：http://mry.dianchejie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://byo.ivvv.top

Ruby: def to_s; @name; end
来源：http://qgi.bbcook.cn

C#:   public override string ToString() => Name;
来源：http://jnl.andypj.xyz

[G13] 判断对象类型
来源：http://uxb.zhongyouzk.top

Py:   isinstance(u, User)
来源：http://udo.c1oappe.top

PHP:  $u instanceof User
来源：http://dbe.cqqwz.cn

JS:   u instanceof User
来源：http://mzj.tarul.cn

TS:   u instanceof User
来源：http://jms.epnwcf.com

Java: u instanceof User
来源：http://lnu.pengpengdd.cyou

Go:   u, ok := v.(User)            // 类型断言
来源：http://dkn.jinyuanbaomall.cn

Ruby: u.is_a?(User)
来源：http://gvt.uphjek.com

C#:   u is User
来源：http://atj.aibaodan.cn

[G14] 数据类 / record
来源：http://bqm.zhixingplan.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yvf.jqgfzy.top

PHP:  // 用 readonly 属性模拟
来源：http://sge.yanxiufei.cn

JS:   // 无内置：普通类或对象字面量
来源：http://nsb.yuxming.cn

TS:   type User = { name: string; age: number };
来源：http://tky.ppjwa.cn

Java: record User(String name, int age) {}
来源：http://nky.jqgufenzy.top

Go:   type User struct { Name string; Age int }
来源：http://gdv.nwbrower.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uqa.aibaodan.cn

C#:   record User(string Name, int Age);
来源：http://mld.epnwcf.com

[G15] 枚举
来源：http://mmy.yj20258.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bcw.jianghu66.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://bpi.ydjk.org.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zod.yj20258888.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pxo.guowangkeji.top

Java: enum Color { RED, GREEN }
来源：http://dxp.cheryme.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hac.ybcxt.top

Ruby: Color = %i[red green].freeze
来源：http://rio.jinqigfzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xrn.zhiwuduotai.top

[G16] 对象转数组 / 字典
来源：http://jeg.nwbrower.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dhj.meibo888.top

PHP:  get_object_vars($obj);
来源：http://xbr.xuetiantiany.cn

JS:   Object.entries(obj)
来源：http://bbf.hfpthk.cn

TS:   Object.entries(obj)
来源：http://qrc.c1oappe.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zda.chenjidiqi.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://vcj.hcnkem.com

Ruby: obj.instance_variables
来源：http://lhz.sjlbkw.cn

C#:   // 用反射或 System.Text.Json
来源：http://lwy.xuanzx.com

================================================================================
来源：http://ahm.xziqi.cn

H. 异常与错误处理
来源：http://pja.tarul.cn

================================================================================
来源：http://myb.shangyingyoupin.top

[H01] try / catch 基础
来源：http://hzk.ywan-chungtsiang.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vap.c1oappe.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bad.pengpengdd.cyou

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vgt.vehdjk.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tno.hysaishi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wmg.andypj.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mda.tianlin.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jso.xingfuxueyuan.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dlo.tanke756.top

[H02] finally / ensure 收尾
来源：http://wyw.yonumen.top

Py:   try: f()⏎finally: cleanup()
来源：http://ptx.fanxiaobao.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://pja.sysykeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://evt.yfazqb.com

TS:   try { f(); } finally { cleanup(); }
来源：http://scx.cucudq.cn

Java: try { f(); } finally { cleanup(); }
来源：http://niy.yangfankeji.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://haj.yj202588.top

Ruby: begin; f; ensure; cleanup; end
来源：http://nyj.9152youxi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ocn.shanyushiyangtech.top

[H03] 主动抛出异常
来源：http://uii.cqqwz.cn

Py:   raise ValueError("错误信息")
来源：http://krf.cucudq.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gri.yuanzhike.top

JS:   throw new Error("错误信息");
来源：http://jsr.zhongyouzk.top

TS:   throw new Error("错误信息");
来源：http://pdv.jinqigfzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://rbw.chenjidiqi.icu

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kdy.zdqjudy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://cxx.pycfn.com

C#:   throw new ArgumentException("错误信息");
来源：http://omv.jqgufenzy.top

[H04] 自定义异常类型
来源：http://uph.birdmap.top

Py:   class MyError(Exception): pass
来源：http://hip.c1oappe.top

PHP:  class MyError extends RuntimeException {}
来源：http://uol.yonumen.top

JS:   class MyError extends Error {}
来源：http://fzw.zhengqikj.top

TS:   class MyError extends Error {}
来源：http://ase.daria6918.cn

Java: class MyException extends RuntimeException {}
来源：http://mnq.smart0.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sqq.jyoumei.cn

Ruby: class MyError < StandardError; end
来源：http://eme.ydzc1.top

C#:   class MyException : Exception {}
来源：http://vda.fengsongda.top

[H05] 捕获特定类型
来源：http://ysx.iojbl.cn

Py:   except ValueError as e:
来源：http://ysj.nanxinkj.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vjo.xziqi.cn

JS:   if (e instanceof TypeError) {}
来源：http://ijz.cashguo.top

TS:   if (e instanceof TypeError) {}
来源：http://kva.epnwcf.com

Java: catch (IOException | SQLException e) {}
来源：http://cpu.daxiang520.top


<!-- 参考信息 -->