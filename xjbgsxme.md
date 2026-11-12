代发 wailian999

[F01] 读取整个文件
来源：http://gcl.aibaodan.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://enp.hnxiangtu.top

PHP:  file_get_contents("a.txt");
来源：http://jyo.yfazqb.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zlv.zhixingplan.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://had.redwolf501.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ila.guannengcc.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uqd.feifeiyinyue.top

Ruby: File.read("a.txt")
来源：http://hxe.jiagoushi.top

C#:   File.ReadAllText("a.txt");
来源：http://eak.9152youxi.cn

[F02] 逐行读取文件
来源：http://mkd.yuanzhike.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gpb.sufxvd.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gai.zdbjq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aca.iojbl.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://syr.feifeiyinyue.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://axz.sysykeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hbe.shangyingyoupin.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xoe.sjlbkw.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ogc.aizwys.cn

[F03] 写入文件（覆盖）
来源：http://byc.kuanghao11.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://djp.kuanghao11.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hdw.tian-w.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lbo.meibo888.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://snx.bjfxy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xib.snrcjt.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sno.dianchejie.cn

Ruby: File.write("a.txt", "hi")
来源：http://nza.meibo888.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tzb.redwolf501.top

[F04] 追加写入文件
来源：http://mdz.meibo888.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wcw.vehdjk.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ahv.aibaodan.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hmx.uphjek.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rdc.aizwys.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kge.svipenyu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uyx.ydjk.org.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hoq.fktsv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jpq.wangshuangyany.cn

[F05] 判断文件或目录是否存在
来源：http://qqn.zhengqikj.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sjf.sweek.top

PHP:  file_exists("a.txt");
来源：http://pnl.hesvh.cn

JS:   fs.existsSync("a.txt")
来源：http://xol.pycfn.com

TS:   fs.existsSync("a.txt")
来源：http://dro.gzhubu.top

Java: Files.exists(Path.of("a.txt"))
来源：http://dtt.cdnleiting.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ers.uphjek.com

Ruby: File.exist?("a.txt")
来源：http://fty.yuanzhike.top

C#:   File.Exists("a.txt")
来源：http://fww.zycfv.cn

[F06] 删除文件
来源：http://xal.zhoulong.xyz

Py:   os.remove("a.txt")
来源：http://vlb.hysaishi.cn

PHP:  unlink("a.txt");
来源：http://xdc.hcnkem.com

JS:   fs.unlinkSync("a.txt")
来源：http://pax.ehwqpu.com

TS:   fs.unlinkSync("a.txt")
来源：http://trv.ehwqpu.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jzb.yj20258.top

Go:   os.Remove("a.txt")
来源：http://qho.tanke756.top

Ruby: File.delete("a.txt")
来源：http://mjv.zhoulong.xyz

C#:   File.Delete("a.txt");
来源：http://tes.snrcjt.cn

[F07] 创建目录（含多级）
来源：http://tsi.sweek.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://iro.ybcxt.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mgr.ybcxt.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xlp.ybcxt.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lux.xylfe.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://foe.hnxiangtu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wwc.shangyingyoupin.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lls.ctjpmb.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xso.sjlbkw.cn

[F08] 遍历目录
来源：http://dxh.9152youxi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wam.nwbrower.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pyj.tian-w.cn

JS:   fs.readdirSync("dir")
来源：http://ieb.ctjpmb.com

TS:   fs.readdirSync("dir")
来源：http://wxa.cheryme.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oik.9152youxi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ymy.jlsjyb.cn

Ruby: Dir.children("dir")
来源：http://tvc.smart0.xyz

C#:   Directory.GetFiles("dir")
来源：http://fvu.ctjpmb.com

[F09] 获取文件大小
来源：http://wmc.zhengqikj.top

Py:   os.path.getsize("a.txt")
来源：http://gfq.hcnkem.com

PHP:  filesize("a.txt");
来源：http://qmw.zhixingplan.top

JS:   fs.statSync("a.txt").size
来源：http://qjq.pycfn.com

TS:   fs.statSync("a.txt").size
来源：http://qqi.cqqwz.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lya.cheryme.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://csi.bjfxy.top

Ruby: File.size("a.txt")
来源：http://bhq.0kj1m.cn

C#:   new FileInfo("a.txt").Length
来源：http://ueh.jinghuilouyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://aqt.zhixingplan.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nyk.hammf.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jds.hongshengwenyu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bwo.hesvh.cn

TS:   path.extname("a.txt")
来源：http://vfr.guannengcc.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hao.sufxvd.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://btd.ppjwa.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tlg.yangfankeji.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jsl.aizwys.cn

[F11] 复制与移动文件
来源：http://oho.zdbjq.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://eup.redwolf501.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wvt.jinyuanbaomall.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zii.chenlongwang.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fcg.shanyushiyangtech.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fzl.jinghuilouyu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zis.hnqzz.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hjg.sysykeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://brq.hnxiangtu.top

[F12] CSV 读写
来源：http://zfa.smart0.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gfk.hnxiangtu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ver.hesvh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zqq.shuidangran.top

TS:   // 同上
来源：http://hwq.yanxiufei.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ejf.xuanzx.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dma.quarkkingdee.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ntj.fktsv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cvk.yongpay.top

================================================================================
来源：http://xjo.xuanzx.com

G. 面向对象
来源：http://afp.tianlin.xyz

================================================================================
来源：http://nob.snrcjt.cn

[G01] 定义类
来源：http://toe.shuidangran.top

Py:   class User: pass
来源：http://odc.pengpengdd.cyou

PHP:  class User {}
来源：http://cpr.guannengcc.top

JS:   class User {}
来源：http://alw.meibo888.top

TS:   class User { name: string = ""; }
来源：http://wyx.ydzc1.top

Java: class User {}
来源：http://bjf.ivvv.top

Go:   type User struct { Name string }
来源：http://ici.xylfe.cn

Ruby: class User; end
来源：http://ush.hywenlv.cn

C#:   class User {}
来源：http://pqp.wangshuangyany.cn

[G02] 构造函数
来源：http://afn.chenzaomai.com

Py:   def __init__(self, name): self.name = name
来源：http://yyo.yvedp.cn

PHP:  public function __construct(public string $name) {}
来源：http://rps.jianghu66.top

JS:   constructor(name) { this.name = name; }
来源：http://tze.jinghuilouyu.cn

TS:   constructor(public name: string) {}
来源：http://ghj.vehdjk.com

Java: User(String name) { this.name = name; }
来源：http://lqu.ybcxt.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rvi.shuidangran.top

Ruby: def initialize(name); @name = name; end
来源：http://acf.vqdsnc.cn

C#:   public User(string name) { Name = name; }
来源：http://bmi.zhijiandao.cn

[G03] 实例属性
来源：http://iuj.zdbjq.cn

Py:   self.name = "x"
来源：http://vyr.sweek.top

PHP:  public string $name = "x";
来源：http://mib.quarkkingdee.top

JS:   this.name = "x";
来源：http://oox.xuetiantiany.cn

TS:   name: string = "x";
来源：http://pku.wangshuangyany.cn

Java: private String name;
来源：http://ncu.yonumen.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vgn.iojbl.cn

Ruby: @name = "x"
来源：http://scy.zhengqikj.top

C#:   public string Name { get; set; } = "x";
来源：http://ucx.9152youxi.cn

[G04] 定义方法
来源：http://lzp.quarkkingdee.top

Py:   def greet(self): return self.name
来源：http://thk.ydzc1.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hzc.dianchejie.cn

JS:   greet() { return this.name; }
来源：http://kbc.epnwcf.com

TS:   greet(): string { return this.name; }
来源：http://ujs.yj20258888.top

Java: String greet() { return name; }
来源：http://ywo.hammf.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qmv.zhijiandao.cn

Ruby: def greet; @name; end
来源：http://jqh.xziqi.cn

C#:   public string Greet() => Name;
来源：http://mjh.chenzaomai.com

[G05] 继承
来源：http://unt.nwbrower.top

Py:   class Admin(User): pass
来源：http://dmf.guowangkeji.top

PHP:  class Admin extends User {}
来源：http://dgs.yuanzhike.top

JS:   class Admin extends User {}
来源：http://wvh.cdnleiting.top

TS:   class Admin extends User {}
来源：http://pzv.yangfankeji.com

Java: class Admin extends User {}
来源：http://ufw.hesvh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kur.fengsongda.top

Ruby: class Admin < User; end
来源：http://hrh.shuidangran.top

C#:   class Admin : User {}
来源：http://vat.zhaomingkeji.xyz

[G06] 重写方法
来源：http://srx.haohaochexian.top

Py:   def greet(self): return "admin"
来源：http://pxx.tianlin.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://ejb.aizwys.cn

JS:   greet() { return "admin"; }
来源：http://juz.cqqwz.cn

TS:   greet(): string { return "admin"; }
来源：http://swk.ydzc1.top

Java: @Override String greet() { return "admin"; }
来源：http://zlk.aizwys.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tfo.hfpthk.cn

Ruby: def greet; "admin"; end
来源：http://okn.ehwqpu.com

C#:   public override string Greet() => "admin";
来源：http://bxq.sysykeji.top

[G07] 调用父类方法
来源：http://jcj.zhaomingkeji.xyz

Py:   super().greet()
来源：http://tiq.nwbrower.top

PHP:  parent::greet();
来源：http://fdn.mhx1999.top

JS:   super.greet();
来源：http://env.yanxiufei.cn

TS:   super.greet();
来源：http://xvn.zhixingplan.top

Java: super.greet();
来源：http://ltt.sufxvd.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nzv.bbcook.cn

Ruby: super
来源：http://nvf.zhixingplan.top

C#:   base.Greet();
来源：http://mty.gotoacloud.top

[G08] 静态方法与属性
来源：http://gnb.gzhubu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uft.316326.xyz

PHP:  public static function f() {}
来源：http://zuj.guannengcc.top

JS:   static f() {}
来源：http://bev.hammf.cn

TS:   static f(): void {}
来源：http://lwc.meibo888.top

Java: static void f() {}
来源：http://gvq.cashguo.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://dpf.zycfv.cn

Ruby: def self.f; end
来源：http://ege.hesvh.cn

C#:   public static void F() {}
来源：http://mrq.yvedp.cn

[G09] 接口 / 抽象类
来源：http://gsn.hywenlv.cn

Py:   from abc import ABC, abstractmethod
来源：http://shv.xuetiantiany.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ngi.c1oappe.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://lbv.jlsjyb.cn

TS:   interface Shape { area(): number; }
来源：http://vhf.hongshengwenyu.top

Java: interface Shape { double area(); }
来源：http://qtf.fehbvm.com

Go:   type Shape interface { Area() float64 }
来源：http://pzc.hongshengwenyu.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tkn.jqgfzy.top

C#:   interface IShape { double Area(); }
来源：http://glc.yuanzhike.top

[G10] 访问控制
来源：http://uxq.wangdashe.top

Py:   约定 _protected / __private（不强制）
来源：http://efo.chenzaomai.com

PHP:  public / protected / private
来源：http://rjl.cqqwz.cn

JS:   #private 字段；其余公开
来源：http://ygb.snrcjt.cn

TS:   public / protected / private
来源：http://vyl.sjlbkw.cn

Java: public / protected / private / 默认包级
来源：http://eop.meibo888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://yly.jqgufenzy.top

Ruby: public / protected / private
来源：http://szx.jiagoushi.top

C#:   public / protected / private / internal
来源：http://axd.jqgfzy.top

[G11] getter / setter
来源：http://cmm.wangdashe.top

Py:   @property 与 @x.setter
来源：http://bat.jqgfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ioh.yonumen.top

JS:   get name() { return this._name; }
来源：http://jkp.yj20258.top

TS:   get name(): string { return this._name; }
来源：http://zhv.yuanzhike.top

Java: public String getName() { return name; }
来源：http://eoy.fehbvm.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://tln.cucudq.cn

Ruby: attr_accessor :name
来源：http://vdx.hnqzz.top

C#:   public string Name { get; set; }
来源：http://rbl.yongpay.top

[G12] 对象转字符串
来源：http://pbl.fanxiaobao.xyz

Py:   def __str__(self): return self.name
来源：http://wfz.zycfv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lbm.fktsv.cn

JS:   toString() { return this.name; }
来源：http://rke.yueranfly.top

TS:   toString(): string { return this.name; }
来源：http://qlk.shangyingyoupin.top

Java: @Override public String toString() { return name; }
来源：http://cdm.zhijiandao.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xru.tanke756.top

Ruby: def to_s; @name; end
来源：http://ybe.yj20258.top

C#:   public override string ToString() => Name;
来源：http://dsr.svipenyu.cn

[G13] 判断对象类型
来源：http://sdj.xziqi.cn

Py:   isinstance(u, User)
来源：http://awn.ppjwa.cn

PHP:  $u instanceof User
来源：http://qrw.hcnkem.com

JS:   u instanceof User
来源：http://aig.fktsv.cn

TS:   u instanceof User
来源：http://nxe.chenjidiqi.icu

Java: u instanceof User
来源：http://vxt.jqgufenzy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://faz.jinqigfzy.top

Ruby: u.is_a?(User)
来源：http://uuq.zhoulong.xyz

C#:   u is User
来源：http://drv.gzhubu.top

[G14] 数据类 / record
来源：http://hki.aizwys.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nmk.birdmap.top

PHP:  // 用 readonly 属性模拟
来源：http://sfq.smart0.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://yaf.ehwqpu.com

TS:   type User = { name: string; age: number };
来源：http://syo.yangfankeji.com

Java: record User(String name, int age) {}
来源：http://bsh.daxiang520.top

Go:   type User struct { Name string; Age int }
来源：http://bfn.9152youxi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wjc.jinqigfzy.top

C#:   record User(string Name, int Age);
来源：http://jfv.chenlongwang.top

[G15] 枚举
来源：http://bwo.hfpthk.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yad.ivvv.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://wtn.yuxming.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gba.yfazqb.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hky.zhoulong.xyz

Java: enum Color { RED, GREEN }
来源：http://tyy.quarkkingdee.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lzb.cucudq.cn

Ruby: Color = %i[red green].freeze
来源：http://zjg.bbcook.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bvt.hammf.cn

[G16] 对象转数组 / 字典
来源：http://gvg.guannengcc.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yty.ppjwa.cn

PHP:  get_object_vars($obj);
来源：http://esi.cdnleiting.top

JS:   Object.entries(obj)
来源：http://gvf.sxryk.cn

TS:   Object.entries(obj)
来源：http://mxp.shanyushiyangkeji.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jqb.yueranfly.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://yxe.yvedp.cn

Ruby: obj.instance_variables
来源：http://nga.mhx1999.top

C#:   // 用反射或 System.Text.Json
来源：http://ple.xingfuxueyuan.xyz

================================================================================
来源：http://yiq.yuanzhike.top

H. 异常与错误处理
来源：http://sto.jlsjyb.cn

================================================================================
来源：http://sco.zycfv.cn

[H01] try / catch 基础
来源：http://nop.haohaochexian.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zmy.jinyuanbaomall.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qlc.jyoumei.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cyf.hongshengwenyu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://far.hnxiangtu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dry.svipenyu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://eun.sysykeji.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pbv.0kj1m.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ffb.yongpay.top

[H02] finally / ensure 收尾
来源：http://dsz.yj20258888.top

Py:   try: f()⏎finally: cleanup()
来源：http://por.yangfankeji.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://sqo.sjlbkw.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yuj.9152youxi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fvb.316326.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://mav.cdnleiting.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://qey.havefunace.top

Ruby: begin; f; ensure; cleanup; end
来源：http://owz.chenlongwang.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://dyh.jyoumei.cn

[H03] 主动抛出异常
来源：http://mlh.zhijiandao.cn

Py:   raise ValueError("错误信息")
来源：http://kwx.tarul.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xnn.zhaomingkeji.xyz

JS:   throw new Error("错误信息");
来源：http://gao.wangdashe.top

TS:   throw new Error("错误信息");
来源：http://lqb.sysykeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://rex.yueranfly.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gpd.sxryk.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wld.chenzaomai.com

C#:   throw new ArgumentException("错误信息");
来源：http://vwe.vqdsnc.cn

[H04] 自定义异常类型
来源：http://enw.shzxlz.cn

Py:   class MyError(Exception): pass
来源：http://fkj.yj202588.top

PHP:  class MyError extends RuntimeException {}
来源：http://olp.haohaochexian.top

JS:   class MyError extends Error {}
来源：http://vxz.hnqzz.top

TS:   class MyError extends Error {}
来源：http://jzp.ybcxt.top

Java: class MyException extends RuntimeException {}
来源：http://ftw.gzhubu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://frp.guowangkeji.top

Ruby: class MyError < StandardError; end
来源：http://hmi.hongshengwenyu.top

C#:   class MyException : Exception {}
来源：http://iyq.hesvh.cn

[H05] 捕获特定类型
来源：http://cuq.dashuyun.cn

Py:   except ValueError as e:
来源：http://hzr.smart0.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ktr.yonumen.top

JS:   if (e instanceof TypeError) {}
来源：http://fjg.yfazqb.com

TS:   if (e instanceof TypeError) {}
来源：http://luj.52xcode.cn

Java: catch (IOException | SQLException e) {}
来源：http://lgb.xingfuxueyuan.xyz


<!-- 参考信息 -->