代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wmg.ivvv.top

================================================================================
来源：http://yka.nwbrower.top

F. 文件与目录
来源：http://vhr.havefunace.top

================================================================================
来源：http://nqb.haohaochexian.top

[F01] 读取整个文件
来源：http://jue.yvedp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zjy.zhixingplan.top

PHP:  file_get_contents("a.txt");
来源：http://pxz.birdmap.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pep.tianlin.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uvt.fzhhl.top

Java: Files.readString(Path.of("a.txt"))
来源：http://urk.jqgufenzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nyl.yj20258.top

Ruby: File.read("a.txt")
来源：http://hvo.uphjek.com

C#:   File.ReadAllText("a.txt");
来源：http://lhb.gogol.net.cn

[F02] 逐行读取文件
来源：http://axu.zhengqikj.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dkg.jinyuanbaomall.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://aed.haohaochexian.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fbf.shangyingyoupin.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://grl.zhongyouzk.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xpd.xuanzx.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://njb.ivvv.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kkj.jianghu66.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rjh.zdbjq.cn

[F03] 写入文件（覆盖）
来源：http://iba.yvedp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jdu.fanxiaobao.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://cmp.jiagoushi.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://euk.feifeiyinyue.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zmg.jiagoushi.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kdq.jqgfzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pmx.jqgufenzy.top

Ruby: File.write("a.txt", "hi")
来源：http://fbt.tianlin.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yuh.quarkkingdee.top

[F04] 追加写入文件
来源：http://gbn.jqgufenzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://das.ywan-chungtsiang.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rap.dianchejie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rtj.snrcjt.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cbj.zhoulong.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ywe.guannengcc.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jfn.hammf.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ugz.c1oappe.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ljn.hammf.cn

[F05] 判断文件或目录是否存在
来源：http://rho.hnqzz.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://srm.wangdashe.top

PHP:  file_exists("a.txt");
来源：http://tng.bjfxy.top

JS:   fs.existsSync("a.txt")
来源：http://xav.wangshuangyany.cn

TS:   fs.existsSync("a.txt")
来源：http://bcv.zycfv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jsc.fktsv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://esb.ybcxt.top

Ruby: File.exist?("a.txt")
来源：http://bkf.tianlin.xyz

C#:   File.Exists("a.txt")
来源：http://ajh.hcnkem.com

[F06] 删除文件
来源：http://ehp.jinghuilouyu.cn

Py:   os.remove("a.txt")
来源：http://por.ywan-chungtsiang.top

PHP:  unlink("a.txt");
来源：http://cno.sysykeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://eoc.hysaishi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://cjb.fengsongda.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fhy.yuxming.cn

Go:   os.Remove("a.txt")
来源：http://tpc.chenjidiqi.icu

Ruby: File.delete("a.txt")
来源：http://kik.meibo888.top

C#:   File.Delete("a.txt");
来源：http://ftj.yj202588.top

[F07] 创建目录（含多级）
来源：http://yli.fengsongda.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://epd.yonumen.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://epl.dashuyun.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ojt.gzhubu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xeo.xylfe.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nva.xinyue.icu

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bbe.hcnkem.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dwh.ywan-chungtsiang.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://llt.cucudq.cn

[F08] 遍历目录
来源：http://nom.andypj.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://lvu.quarkkingdee.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rym.cucudq.cn

JS:   fs.readdirSync("dir")
来源：http://rbe.xinyue.icu

TS:   fs.readdirSync("dir")
来源：http://uyr.nwbrower.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qzo.daxiang520.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://tnt.9152youxi.cn

Ruby: Dir.children("dir")
来源：http://jqi.guannengcc.top

C#:   Directory.GetFiles("dir")
来源：http://rau.xuetiantiany.cn

[F09] 获取文件大小
来源：http://lyz.yfazqb.com

Py:   os.path.getsize("a.txt")
来源：http://adu.yvedp.cn

PHP:  filesize("a.txt");
来源：http://khi.cheryme.top

JS:   fs.statSync("a.txt").size
来源：http://mbl.ydjk.org.cn

TS:   fs.statSync("a.txt").size
来源：http://rex.jinghuilouyu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ahv.iojbl.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pxj.yueranfly.top

Ruby: File.size("a.txt")
来源：http://oki.andypj.xyz

C#:   new FileInfo("a.txt").Length
来源：http://mwr.wangdashe.top

[F10] 取文件扩展名 / 文件名
来源：http://mpu.wangshuangyany.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ieb.aibaodan.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hrm.fanxiaobao.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vry.bbcook.cn

TS:   path.extname("a.txt")
来源：http://wth.andypj.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zrz.fanxiaobao.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://frj.dashuyun.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yhk.sweek.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yna.aibaodan.cn

[F11] 复制与移动文件
来源：http://qmo.0kj1m.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://czi.zhoulong.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rav.feifeiyinyue.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fmv.yvedp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lnt.fzhhl.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wwt.hesvh.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bwb.316326.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zqq.aibaodan.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qih.fehbvm.com

[F12] CSV 读写
来源：http://zbe.shuidangran.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hzl.hnxiangtu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zwj.yueranfly.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://azp.epnwcf.com

TS:   // 同上
来源：http://uzo.ppjwa.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dao.zycfv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vze.jinqigfzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xtg.birdmap.top

C#:   // 无内置：用 CsvHelper 库
来源：http://qoc.jinqigfzy.top

================================================================================
来源：http://vii.yfazqb.com

G. 面向对象
来源：http://ztf.aibaodan.cn

================================================================================
来源：http://ppc.xuanzx.com

[G01] 定义类
来源：http://jei.cdnleiting.top

Py:   class User: pass
来源：http://yns.feifeiyinyue.top

PHP:  class User {}
来源：http://cmv.cheryme.top

JS:   class User {}
来源：http://eoj.hesvh.cn

TS:   class User { name: string = ""; }
来源：http://aet.shuidangran.top

Java: class User {}
来源：http://vmm.sufxvd.cn

Go:   type User struct { Name string }
来源：http://iuo.andypj.xyz

Ruby: class User; end
来源：http://xcg.xziqi.cn

C#:   class User {}
来源：http://los.ehwqpu.com

[G02] 构造函数
来源：http://cqu.zdbjq.cn

Py:   def __init__(self, name): self.name = name
来源：http://nmv.316326.xyz

PHP:  public function __construct(public string $name) {}
来源：http://iir.dashuyun.cn

JS:   constructor(name) { this.name = name; }
来源：http://rtl.wangshuangyany.cn

TS:   constructor(public name: string) {}
来源：http://sed.zhijiandao.cn

Java: User(String name) { this.name = name; }
来源：http://hjw.andypj.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hoq.aibaodan.cn

Ruby: def initialize(name); @name = name; end
来源：http://erq.sufxvd.cn

C#:   public User(string name) { Name = name; }
来源：http://xkm.xinyue.icu

[G03] 实例属性
来源：http://har.shangyingyoupin.top

Py:   self.name = "x"
来源：http://elc.feifeiyinyue.top

PHP:  public string $name = "x";
来源：http://tyv.meibo888.top

JS:   this.name = "x";
来源：http://mhz.yj20258.top

TS:   name: string = "x";
来源：http://ipa.xziqi.cn

Java: private String name;
来源：http://tcx.xuanzx.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hwq.jqgufenzy.top

Ruby: @name = "x"
来源：http://hge.ydzc1.top

C#:   public string Name { get; set; } = "x";
来源：http://ifv.feifeiyinyue.top

[G04] 定义方法
来源：http://lhu.cashguo.top

Py:   def greet(self): return self.name
来源：http://mes.zhijiandao.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vwg.ppjwa.cn

JS:   greet() { return this.name; }
来源：http://bte.ppjwa.cn

TS:   greet(): string { return this.name; }
来源：http://cml.fktsv.cn

Java: String greet() { return name; }
来源：http://ske.svipenyu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://znk.ehwqpu.com

Ruby: def greet; @name; end
来源：http://xiq.smart0.xyz

C#:   public string Greet() => Name;
来源：http://hgl.ybcxt.top

[G05] 继承
来源：http://itb.dashuyun.cn

Py:   class Admin(User): pass
来源：http://oba.jinqigufen.top

PHP:  class Admin extends User {}
来源：http://stt.zhengqikj.top

JS:   class Admin extends User {}
来源：http://whi.fehbvm.com

TS:   class Admin extends User {}
来源：http://ntg.gotoacloud.top

Java: class Admin extends User {}
来源：http://rds.jinqigfzy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mga.zdqjudy.top

Ruby: class Admin < User; end
来源：http://alf.sysykeji.top

C#:   class Admin : User {}
来源：http://ffi.hfpthk.cn

[G06] 重写方法
来源：http://zot.yueranfly.top

Py:   def greet(self): return "admin"
来源：http://hoa.birdmap.top

PHP:  public function greet(): string { return "admin"; }
来源：http://dem.yueranfly.top

JS:   greet() { return "admin"; }
来源：http://xyt.cqqwz.cn

TS:   greet(): string { return "admin"; }
来源：http://hgi.fehbvm.com

Java: @Override String greet() { return "admin"; }
来源：http://oap.c1oappe.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vgt.cqqwz.cn

Ruby: def greet; "admin"; end
来源：http://rji.yanxiufei.cn

C#:   public override string Greet() => "admin";
来源：http://ksp.hammf.cn

[G07] 调用父类方法
来源：http://tih.cqqwz.cn

Py:   super().greet()
来源：http://vdb.hcnkem.com

PHP:  parent::greet();
来源：http://uxp.hfpthk.cn

JS:   super.greet();
来源：http://zmm.svipenyu.cn

TS:   super.greet();
来源：http://xxi.tarul.cn

Java: super.greet();
来源：http://enw.hcnkem.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ccm.zhiwuduotai.top

Ruby: super
来源：http://grg.hcnkem.com

C#:   base.Greet();
来源：http://iey.andypj.xyz

[G08] 静态方法与属性
来源：http://bbx.shuidangran.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qts.xuetiantiany.cn

PHP:  public static function f() {}
来源：http://cid.zhiwuduotai.top

JS:   static f() {}
来源：http://sqn.quarkkingdee.top

TS:   static f(): void {}
来源：http://vjs.zhoulong.xyz

Java: static void f() {}
来源：http://qnm.ivvv.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://wil.gzhubu.top

Ruby: def self.f; end
来源：http://gap.zhoulong.xyz

C#:   public static void F() {}
来源：http://dsz.sjlbkw.cn

[G09] 接口 / 抽象类
来源：http://nix.hcnkem.com

Py:   from abc import ABC, abstractmethod
来源：http://hfo.fehbvm.com

PHP:  interface Shape { public function area(): float; }
来源：http://ynx.snrcjt.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rfs.zhoulong.xyz

TS:   interface Shape { area(): number; }
来源：http://orw.epnwcf.com

Java: interface Shape { double area(); }
来源：http://kgx.zhiwuduotai.top

Go:   type Shape interface { Area() float64 }
来源：http://xwm.uphjek.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://evo.hnxiangtu.top

C#:   interface IShape { double Area(); }
来源：http://xpg.sweek.top

[G10] 访问控制
来源：http://xrj.zycfv.cn

Py:   约定 _protected / __private（不强制）
来源：http://ikv.ppjwa.cn

PHP:  public / protected / private
来源：http://yvy.cucudq.cn

JS:   #private 字段；其余公开
来源：http://chc.wangshuangyany.cn

TS:   public / protected / private
来源：http://ljf.xingfuxueyuan.xyz

Java: public / protected / private / 默认包级
来源：http://zbr.xinyue.icu

Go:   首字母大写可导出，小写仅包内可见
来源：http://vax.ehwqpu.com

Ruby: public / protected / private
来源：http://jfb.feifeiyinyue.top

C#:   public / protected / private / internal
来源：http://org.iojbl.cn

[G11] getter / setter
来源：http://tbf.jinqigfzy.top

Py:   @property 与 @x.setter
来源：http://tao.gaohongyu789.top

PHP:  public function getName(): string { return $this->name; }
来源：http://hyx.dashuyun.cn

JS:   get name() { return this._name; }
来源：http://mpq.yvedp.cn

TS:   get name(): string { return this._name; }
来源：http://ilb.epnwcf.com

Java: public String getName() { return name; }
来源：http://pia.snrcjt.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hcm.nanxinkj.top

Ruby: attr_accessor :name
来源：http://dzp.zdqjudy.top

C#:   public string Name { get; set; }
来源：http://ufn.chenlongwang.top

[G12] 对象转字符串
来源：http://rpx.xylfe.cn

Py:   def __str__(self): return self.name
来源：http://uqj.gogol.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vti.redwolf501.top

JS:   toString() { return this.name; }
来源：http://rmh.dianchejie.cn

TS:   toString(): string { return this.name; }
来源：http://bcl.hnxiangtu.top

Java: @Override public String toString() { return name; }
来源：http://cck.shuidangran.top

Go:   func (u User) String() string { return u.Name }
来源：http://glz.zhiwuduotai.top

Ruby: def to_s; @name; end
来源：http://alp.andypj.xyz

C#:   public override string ToString() => Name;
来源：http://uyf.gaohongyu789.top

[G13] 判断对象类型
来源：http://ghw.mhx1999.top

Py:   isinstance(u, User)
来源：http://tbp.zhengqikj.top

PHP:  $u instanceof User
来源：http://qik.snrcjt.cn

JS:   u instanceof User
来源：http://mnh.vehdjk.com

TS:   u instanceof User
来源：http://ufk.epnwcf.com

Java: u instanceof User
来源：http://myl.xuetiantiany.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jbi.yongpay.top

Ruby: u.is_a?(User)
来源：http://mou.jqgfzy.top

C#:   u is User
来源：http://mix.cdnleiting.top

[G14] 数据类 / record
来源：http://cpe.vehdjk.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dvi.bjfxy.top

PHP:  // 用 readonly 属性模拟
来源：http://wbn.sweek.top

JS:   // 无内置：普通类或对象字面量
来源：http://idx.tanke756.top

TS:   type User = { name: string; age: number };
来源：http://cbm.zdqjudy.top

Java: record User(String name, int age) {}
来源：http://soi.fzhhl.top

Go:   type User struct { Name string; Age int }
来源：http://olq.fzhhl.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ssr.ywan-chungtsiang.top

C#:   record User(string Name, int Age);
来源：http://kla.sxryk.cn

[G15] 枚举
来源：http://qmt.daria6918.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rfd.hammf.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rhk.iojbl.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bup.hysaishi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://thh.aibaodan.cn

Java: enum Color { RED, GREEN }
来源：http://fkb.fktsv.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lvn.hongshengwenyu.top

Ruby: Color = %i[red green].freeze
来源：http://apw.sweek.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hbl.andypj.xyz

[G16] 对象转数组 / 字典
来源：http://kvm.xuanzx.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lvo.cashguo.top

PHP:  get_object_vars($obj);
来源：http://llp.vehdjk.com

JS:   Object.entries(obj)
来源：http://yjf.zhijiandao.cn

TS:   Object.entries(obj)
来源：http://kmt.sxryk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tbe.gotoacloud.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://stt.ppjwa.cn

Ruby: obj.instance_variables
来源：http://ijx.uphjek.com

C#:   // 用反射或 System.Text.Json
来源：http://wuk.yongpay.top

================================================================================
来源：http://bwl.316326.xyz

H. 异常与错误处理
来源：http://hia.316326.xyz

================================================================================
来源：http://bex.cucudq.cn

[H01] try / catch 基础
来源：http://ezh.zhijiandao.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uus.yfazqb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zsa.redwolf501.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xbe.gaohongyu789.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bvz.jinghuilouyu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zwn.tianlin.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rni.shanyushiyangkeji.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pma.yongpay.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xau.gotoacloud.top

[H02] finally / ensure 收尾
来源：http://izn.jianghu66.top

Py:   try: f()⏎finally: cleanup()
来源：http://faf.xylfe.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://niz.havefunace.top

JS:   try { f(); } finally { cleanup(); }
来源：http://jdc.shuidangran.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ets.yj20258.top

Java: try { f(); } finally { cleanup(); }
来源：http://uwy.cashguo.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://pyg.zhengqikj.top

Ruby: begin; f; ensure; cleanup; end
来源：http://kps.zhixingplan.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://acr.dashuyun.cn

[H03] 主动抛出异常
来源：http://tdh.yueranfly.top

Py:   raise ValueError("错误信息")
来源：http://qna.snrcjt.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lxr.hysaishi.cn

JS:   throw new Error("错误信息");
来源：http://txz.zhoulong.xyz

TS:   throw new Error("错误信息");
来源：http://zmb.redwolf501.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://exg.zhijiandao.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ewj.ydjk.org.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://iju.9152youxi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://csa.shuidangran.top

[H04] 自定义异常类型
来源：http://atx.birdmap.top

Py:   class MyError(Exception): pass
来源：http://emr.guowangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://uzy.zhixingplan.top

JS:   class MyError extends Error {}
来源：http://fei.ywan-chungtsiang.top

TS:   class MyError extends Error {}
来源：http://wxh.jinqigufen.top

Java: class MyException extends RuntimeException {}
来源：http://ijm.ydzc1.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://eix.yj20258.top

Ruby: class MyError < StandardError; end
来源：http://okt.ydjk.org.cn

C#:   class MyException : Exception {}
来源：http://tnd.yongpay.top

[H05] 捕获特定类型
来源：http://zyd.ehwqpu.com

Py:   except ValueError as e:
来源：http://lqw.fktsv.cn


<!-- 参考信息 -->