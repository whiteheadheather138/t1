代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://soz.fengsongda.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mgc.shuidangran.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mms.hongshengwenyu.top

Ruby: s.bytesize;  s.length
来源：http://qlo.jinqigufen.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dbr.mhx1999.top

================================================================================
来源：http://mww.vqdsnc.cn

F. 文件与目录
来源：http://tlm.bjfxy.top

================================================================================
来源：http://iuz.jlsjyb.cn

[F01] 读取整个文件
来源：http://lxu.ybcxt.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cja.snrcjt.cn

PHP:  file_get_contents("a.txt");
来源：http://srk.zhongyouzk.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mxh.bjfxy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sqo.fehbvm.com

Java: Files.readString(Path.of("a.txt"))
来源：http://pee.yj202588.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tqa.hfpthk.cn

Ruby: File.read("a.txt")
来源：http://jjf.jiagoushi.top

C#:   File.ReadAllText("a.txt");
来源：http://hcm.nanxinkj.top

[F02] 逐行读取文件
来源：http://qof.ppjwa.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qka.shangyingyoupin.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://czy.jinghuilouyu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wvm.hywenlv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://npb.wangshuangyany.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ofb.nwbrower.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lpm.nanxuanxn.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mur.ydjk.org.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ogc.xingfuxueyuan.xyz

[F03] 写入文件（覆盖）
来源：http://icr.jianghu66.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mrs.ivvv.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://sgv.shzxlz.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dml.gaohongyu789.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xaz.sweek.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ifq.yuxming.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gbo.meibo888.top

Ruby: File.write("a.txt", "hi")
来源：http://nse.hfpthk.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rnm.smart0.xyz

[F04] 追加写入文件
来源：http://ppc.zycfv.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uem.ctjpmb.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://etn.hnxiangtu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://doj.yj202588.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jmv.jinyuanbaomall.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xhk.yuxming.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rtf.smart0.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vwh.redwolf501.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://obf.jinghuilouyu.cn

[F05] 判断文件或目录是否存在
来源：http://nbq.cdnleiting.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://iyz.zhongyouzk.top

PHP:  file_exists("a.txt");
来源：http://frv.zhiwuduotai.top

JS:   fs.existsSync("a.txt")
来源：http://tpb.0kj1m.cn

TS:   fs.existsSync("a.txt")
来源：http://sbb.9152youxi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gpn.birdmap.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cju.zhongyouzk.top

Ruby: File.exist?("a.txt")
来源：http://uib.zhijiandao.cn

C#:   File.Exists("a.txt")
来源：http://ojk.gogol.net.cn

[F06] 删除文件
来源：http://pza.guowangkeji.top

Py:   os.remove("a.txt")
来源：http://ctz.daxiang520.top

PHP:  unlink("a.txt");
来源：http://enx.chenjidiqi.icu

JS:   fs.unlinkSync("a.txt")
来源：http://the.yj20258888.top

TS:   fs.unlinkSync("a.txt")
来源：http://rew.c1oappe.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zav.jqgufenzy.top

Go:   os.Remove("a.txt")
来源：http://sqa.gaohongyu789.top

Ruby: File.delete("a.txt")
来源：http://efu.zhengqikj.top

C#:   File.Delete("a.txt");
来源：http://txd.hywenlv.cn

[F07] 创建目录（含多级）
来源：http://rhx.fzhhl.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qfi.zhijiandao.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hjl.chenzaomai.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://din.9152youxi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wcs.0kj1m.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kuo.hywenlv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://loj.fengsongda.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qxd.shanyushiyangkeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lmm.guannengcc.top

[F08] 遍历目录
来源：http://uxu.wangdashe.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xbr.nanxuanxn.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qma.cdnleiting.top

JS:   fs.readdirSync("dir")
来源：http://wtc.hammf.cn

TS:   fs.readdirSync("dir")
来源：http://zvf.yonumen.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vnv.zhoulong.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://fka.fengsongda.top

Ruby: Dir.children("dir")
来源：http://kjz.yanxiufei.cn

C#:   Directory.GetFiles("dir")
来源：http://mjq.yangfankeji.com

[F09] 获取文件大小
来源：http://zvr.guowangkeji.top

Py:   os.path.getsize("a.txt")
来源：http://sht.hnqzz.top

PHP:  filesize("a.txt");
来源：http://ihq.iojbl.cn

JS:   fs.statSync("a.txt").size
来源：http://rkm.tian-w.cn

TS:   fs.statSync("a.txt").size
来源：http://vrm.xingfuxueyuan.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://hbt.mhx1999.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ijo.sjlbkw.cn

Ruby: File.size("a.txt")
来源：http://bwq.ydzc1.top

C#:   new FileInfo("a.txt").Length
来源：http://ror.ivvv.top

[F10] 取文件扩展名 / 文件名
来源：http://bzg.yfazqb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ong.epnwcf.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://eid.c1oappe.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qpx.cashguo.top

TS:   path.extname("a.txt")
来源：http://vjn.cheryme.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://klr.quarkkingdee.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ikp.cqqwz.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cxb.ppjwa.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mye.havefunace.top

[F11] 复制与移动文件
来源：http://rzz.cdnleiting.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yya.ivvv.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hjs.yuxming.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fkr.hesvh.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tzv.nanxuanxn.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://abz.pengpengdd.cyou

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://aho.cheryme.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cfv.yj202588.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bdz.yanxiufei.cn

[F12] CSV 读写
来源：http://ljp.hfpthk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://smr.redwolf501.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ist.jiagoushi.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ira.hammf.cn

TS:   // 同上
来源：http://dya.ehwqpu.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://izv.uphjek.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rdr.xinyue.icu

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pra.yanxiufei.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gmx.yonumen.top

================================================================================
来源：http://hte.fktsv.cn

G. 面向对象
来源：http://rkj.dashuyun.cn

================================================================================
来源：http://off.jiagoushi.top

[G01] 定义类
来源：http://ejg.feifeiyinyue.top

Py:   class User: pass
来源：http://fni.sweek.top

PHP:  class User {}
来源：http://tpt.jinghuilouyu.cn

JS:   class User {}
来源：http://jzv.wangshuangyany.cn

TS:   class User { name: string = ""; }
来源：http://rnv.fehbvm.com

Java: class User {}
来源：http://rxl.nanxinkj.top

Go:   type User struct { Name string }
来源：http://yon.ybcxt.top

Ruby: class User; end
来源：http://kzb.cheryme.top

C#:   class User {}
来源：http://gsl.cucudq.cn

[G02] 构造函数
来源：http://ywr.zhaomingkeji.xyz

Py:   def __init__(self, name): self.name = name
来源：http://ham.bbcook.cn

PHP:  public function __construct(public string $name) {}
来源：http://cal.xylfe.cn

JS:   constructor(name) { this.name = name; }
来源：http://bpy.hammf.cn

TS:   constructor(public name: string) {}
来源：http://avy.xylfe.cn

Java: User(String name) { this.name = name; }
来源：http://sia.aizwys.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cex.shanyushiyangkeji.top

Ruby: def initialize(name); @name = name; end
来源：http://oab.tanke756.top

C#:   public User(string name) { Name = name; }
来源：http://kci.gzhubu.top

[G03] 实例属性
来源：http://gip.cucudq.cn

Py:   self.name = "x"
来源：http://bjj.wangdashe.top

PHP:  public string $name = "x";
来源：http://hma.zdbjq.cn

JS:   this.name = "x";
来源：http://dfu.mhx1999.top

TS:   name: string = "x";
来源：http://cgs.ydjk.org.cn

Java: private String name;
来源：http://ydn.meibo888.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wol.pycfn.com

Ruby: @name = "x"
来源：http://rdx.shanyushiyangtech.top

C#:   public string Name { get; set; } = "x";
来源：http://dqc.0kj1m.cn

[G04] 定义方法
来源：http://iym.sxryk.cn

Py:   def greet(self): return self.name
来源：http://vtd.ydzc1.top

PHP:  public function greet(): string { return $this->name; }
来源：http://evg.epnwcf.com

JS:   greet() { return this.name; }
来源：http://kah.jqgfzy.top

TS:   greet(): string { return this.name; }
来源：http://nlp.yj202588.top

Java: String greet() { return name; }
来源：http://xsz.gogol.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://kul.yj20258.top

Ruby: def greet; @name; end
来源：http://ezy.zhaomingkeji.xyz

C#:   public string Greet() => Name;
来源：http://vgn.xylfe.cn

[G05] 继承
来源：http://wdj.meibo888.top

Py:   class Admin(User): pass
来源：http://rkn.guannengcc.top

PHP:  class Admin extends User {}
来源：http://qvf.chenzaomai.com

JS:   class Admin extends User {}
来源：http://vms.xuanzx.com

TS:   class Admin extends User {}
来源：http://ntz.yj20258888.top

Java: class Admin extends User {}
来源：http://ccu.zdqjudy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rds.dashuyun.cn

Ruby: class Admin < User; end
来源：http://jeg.ybcxt.top

C#:   class Admin : User {}
来源：http://lnz.hammf.cn

[G06] 重写方法
来源：http://dvc.yongpay.top

Py:   def greet(self): return "admin"
来源：http://hnk.hysaishi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://alh.vehdjk.com

JS:   greet() { return "admin"; }
来源：http://pxx.sjlbkw.cn

TS:   greet(): string { return "admin"; }
来源：http://jka.gotoacloud.top

Java: @Override String greet() { return "admin"; }
来源：http://nze.zdqjudy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fvi.ydzc1.top

Ruby: def greet; "admin"; end
来源：http://kkf.pengpengdd.cyou

C#:   public override string Greet() => "admin";
来源：http://gnj.uphjek.com

[G07] 调用父类方法
来源：http://icn.chenzaomai.com

Py:   super().greet()
来源：http://rdw.316326.xyz

PHP:  parent::greet();
来源：http://tfw.smart0.xyz

JS:   super.greet();
来源：http://yen.shangyingyoupin.top

TS:   super.greet();
来源：http://wfq.zdqjudy.top

Java: super.greet();
来源：http://rel.xinyue.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mdm.zhiwuduotai.top

Ruby: super
来源：http://nlx.52xcode.cn

C#:   base.Greet();
来源：http://eqk.hysaishi.cn

[G08] 静态方法与属性
来源：http://tnm.hnqzz.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ore.hcnkem.com

PHP:  public static function f() {}
来源：http://pns.hfpthk.cn

JS:   static f() {}
来源：http://izf.fanxiaobao.xyz

TS:   static f(): void {}
来源：http://fez.shzxlz.cn

Java: static void f() {}
来源：http://auy.sjlbkw.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://tec.redwolf501.top

Ruby: def self.f; end
来源：http://wwe.xziqi.cn

C#:   public static void F() {}
来源：http://odi.jinqigfzy.top

[G09] 接口 / 抽象类
来源：http://uuj.nanxinkj.top

Py:   from abc import ABC, abstractmethod
来源：http://lit.yj20258.top

PHP:  interface Shape { public function area(): float; }
来源：http://fpj.tianlin.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://rmz.bjfxy.top

TS:   interface Shape { area(): number; }
来源：http://ybe.sufxvd.cn

Java: interface Shape { double area(); }
来源：http://ghg.nanxuanxn.top

Go:   type Shape interface { Area() float64 }
来源：http://gmm.316326.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ejs.jqgfzy.top

C#:   interface IShape { double Area(); }
来源：http://wil.pengpengdd.cyou

[G10] 访问控制
来源：http://mgb.vehdjk.com

Py:   约定 _protected / __private（不强制）
来源：http://eds.mhx1999.top

PHP:  public / protected / private
来源：http://ngo.yanxiufei.cn

JS:   #private 字段；其余公开
来源：http://xpo.aizwys.cn

TS:   public / protected / private
来源：http://wla.wangdashe.top

Java: public / protected / private / 默认包级
来源：http://kxb.tianlin.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://rnh.xuanzx.com

Ruby: public / protected / private
来源：http://xhy.zhaomingkeji.xyz

C#:   public / protected / private / internal
来源：http://jgh.zhongyouzk.top

[G11] getter / setter
来源：http://nim.ehwqpu.com

Py:   @property 与 @x.setter
来源：http://url.cheryme.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ury.9152youxi.cn

JS:   get name() { return this._name; }
来源：http://uvl.birdmap.top

TS:   get name(): string { return this._name; }
来源：http://nlz.jiagoushi.top

Java: public String getName() { return name; }
来源：http://aot.birdmap.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://dct.hfpthk.cn

Ruby: attr_accessor :name
来源：http://dym.sjlbkw.cn

C#:   public string Name { get; set; }
来源：http://pwv.jinqigfzy.top

[G12] 对象转字符串
来源：http://rni.yuanzhike.top

Py:   def __str__(self): return self.name
来源：http://jqm.jianghu66.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://cvm.gzhubu.top

JS:   toString() { return this.name; }
来源：http://jbi.316326.xyz

TS:   toString(): string { return this.name; }
来源：http://mtf.iojbl.cn

Java: @Override public String toString() { return name; }
来源：http://wmc.zhoulong.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://xkt.ctjpmb.com

Ruby: def to_s; @name; end
来源：http://owk.vqdsnc.cn

C#:   public override string ToString() => Name;
来源：http://hhb.yongpay.top

[G13] 判断对象类型
来源：http://bud.snrcjt.cn

Py:   isinstance(u, User)
来源：http://rkc.nanxinkj.top

PHP:  $u instanceof User
来源：http://fnr.quarkkingdee.top

JS:   u instanceof User
来源：http://zln.ydzc1.top

TS:   u instanceof User
来源：http://gro.tarul.cn

Java: u instanceof User
来源：http://kry.xylfe.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mrq.c1oappe.top

Ruby: u.is_a?(User)
来源：http://jkd.hcnkem.com

C#:   u is User
来源：http://syg.yj20258888.top

[G14] 数据类 / record
来源：http://tle.vehdjk.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hti.c1oappe.top

PHP:  // 用 readonly 属性模拟
来源：http://btp.yanxiufei.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fvs.gogol.net.cn

TS:   type User = { name: string; age: number };
来源：http://awd.andypj.xyz

Java: record User(String name, int age) {}
来源：http://xuh.c1oappe.top

Go:   type User struct { Name string; Age int }
来源：http://jzf.ppjwa.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mye.aizwys.cn

C#:   record User(string Name, int Age);
来源：http://fqu.vqdsnc.cn

[G15] 枚举
来源：http://ibd.zdbjq.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lmh.meibo888.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://kyi.fzhhl.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://avz.birdmap.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bbc.shangyingyoupin.top

Java: enum Color { RED, GREEN }
来源：http://zdi.snrcjt.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nxo.hysaishi.cn

Ruby: Color = %i[red green].freeze
来源：http://qgh.aizwys.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sva.jinghuilouyu.cn

[G16] 对象转数组 / 字典
来源：http://gqo.sysykeji.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vms.gaohongyu789.top

PHP:  get_object_vars($obj);
来源：http://rlq.haohaochexian.top

JS:   Object.entries(obj)
来源：http://caj.yangfankeji.com

TS:   Object.entries(obj)
来源：http://crl.gaohongyu789.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://abf.cashguo.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://cxt.sufxvd.cn

Ruby: obj.instance_variables
来源：http://ioe.meibo888.top

C#:   // 用反射或 System.Text.Json
来源：http://jgr.yangfankeji.com

================================================================================
来源：http://ftb.yuanzhike.top

H. 异常与错误处理
来源：http://meo.xuanzx.com

================================================================================
来源：http://abk.shanyushiyangtech.top

[H01] try / catch 基础
来源：http://amw.fehbvm.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bpt.yongpay.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tmi.cdnleiting.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nrq.vehdjk.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ujf.hcnkem.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pac.chenjidiqi.icu

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://oza.birdmap.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://exx.shangyingyoupin.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cin.smart0.xyz

[H02] finally / ensure 收尾
来源：http://eco.jinghuilouyu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ier.dianchejie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zmx.birdmap.top

JS:   try { f(); } finally { cleanup(); }
来源：http://sem.c1oappe.top

TS:   try { f(); } finally { cleanup(); }
来源：http://rvc.hfpthk.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xel.gotoacloud.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://nai.yueranfly.top

Ruby: begin; f; ensure; cleanup; end
来源：http://wmj.bbcook.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://keo.sysykeji.top

[H03] 主动抛出异常
来源：http://elq.meibo888.top

Py:   raise ValueError("错误信息")
来源：http://yzn.yonumen.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mvo.hysaishi.cn

JS:   throw new Error("错误信息");
来源：http://imc.gaohongyu789.top

TS:   throw new Error("错误信息");
来源：http://qtw.chenzaomai.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://pnb.cashguo.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wne.vqdsnc.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ary.xziqi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hte.shangyingyoupin.top

[H04] 自定义异常类型
来源：http://whx.yuxming.cn

Py:   class MyError(Exception): pass
来源：http://ihq.yonumen.top

PHP:  class MyError extends RuntimeException {}
来源：http://ywa.chenlongwang.top

JS:   class MyError extends Error {}
来源：http://pxx.fengsongda.top

TS:   class MyError extends Error {}
来源：http://jal.zhengqikj.top

Java: class MyException extends RuntimeException {}
来源：http://xdq.shanyushiyangtech.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://efj.aizwys.cn


<!-- 参考信息 -->