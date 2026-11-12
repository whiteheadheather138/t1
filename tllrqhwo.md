代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pya.snrcjt.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dsq.vehdjk.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zju.pengpengdd.cyou

Ruby: File.read("a.txt")
来源：http://inl.sysykeji.top

C#:   File.ReadAllText("a.txt");
来源：http://lju.nanxinkj.top

[F02] 逐行读取文件
来源：http://ijv.jqgufenzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nwe.daxiang520.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zdv.uphjek.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ccj.sxryk.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://juu.zhiwuduotai.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pim.vehdjk.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zsn.yj202588.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rbp.pengpengdd.cyou

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ong.svipenyu.cn

[F03] 写入文件（覆盖）
来源：http://hjv.yanxiufei.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pnv.zhoulong.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://ihh.pycfn.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://udz.shanyushiyangkeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hoc.yj20258888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cqv.fanxiaobao.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bmn.tarul.cn

Ruby: File.write("a.txt", "hi")
来源：http://zor.cucudq.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uqs.zhaomingkeji.xyz

[F04] 追加写入文件
来源：http://zft.0kj1m.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://brz.wangdashe.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rwj.fehbvm.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wln.cashguo.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://toz.ppjwa.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qxx.fehbvm.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://eky.yongpay.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zbh.cdnleiting.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jga.xingfuxueyuan.xyz

[F05] 判断文件或目录是否存在
来源：http://ewf.birdmap.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bay.hesvh.cn

PHP:  file_exists("a.txt");
来源：http://umn.hywenlv.cn

JS:   fs.existsSync("a.txt")
来源：http://pja.sxryk.cn

TS:   fs.existsSync("a.txt")
来源：http://grv.yvedp.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hen.fktsv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pmw.smart0.xyz

Ruby: File.exist?("a.txt")
来源：http://zof.chenlongwang.top

C#:   File.Exists("a.txt")
来源：http://cvp.birdmap.top

[F06] 删除文件
来源：http://jgx.zhixingplan.top

Py:   os.remove("a.txt")
来源：http://qzk.c1oappe.top

PHP:  unlink("a.txt");
来源：http://dam.haohaochexian.top

JS:   fs.unlinkSync("a.txt")
来源：http://biy.c1oappe.top

TS:   fs.unlinkSync("a.txt")
来源：http://pfq.snrcjt.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ikj.sjlbkw.cn

Go:   os.Remove("a.txt")
来源：http://gux.0kj1m.cn

Ruby: File.delete("a.txt")
来源：http://pio.svipenyu.cn

C#:   File.Delete("a.txt");
来源：http://ysa.tarul.cn

[F07] 创建目录（含多级）
来源：http://hhi.shuidangran.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://frq.zhijiandao.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dyn.zdqjudy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ozm.sysykeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ykn.tarul.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kck.ydjk.org.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ezl.yvedp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zhu.xingfuxueyuan.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://suj.yvedp.cn

[F08] 遍历目录
来源：http://myo.zhaomingkeji.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://qcd.hysaishi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sqb.xziqi.cn

JS:   fs.readdirSync("dir")
来源：http://dmj.fanxiaobao.xyz

TS:   fs.readdirSync("dir")
来源：http://mls.fehbvm.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ugb.sxryk.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hzh.yonumen.top

Ruby: Dir.children("dir")
来源：http://byi.316326.xyz

C#:   Directory.GetFiles("dir")
来源：http://lpq.uphjek.com

[F09] 获取文件大小
来源：http://fth.hnqzz.top

Py:   os.path.getsize("a.txt")
来源：http://gzv.jinghuilouyu.cn

PHP:  filesize("a.txt");
来源：http://gqh.daxiang520.top

JS:   fs.statSync("a.txt").size
来源：http://ekw.snrcjt.cn

TS:   fs.statSync("a.txt").size
来源：http://sde.316326.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://xvm.xuetiantiany.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vks.aibaodan.cn

Ruby: File.size("a.txt")
来源：http://gul.bbcook.cn

C#:   new FileInfo("a.txt").Length
来源：http://nzx.zdbjq.cn

[F10] 取文件扩展名 / 文件名
来源：http://rxt.jianghu66.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hxt.hesvh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vnj.hywenlv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nkk.birdmap.top

TS:   path.extname("a.txt")
来源：http://gin.gaohongyu789.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jct.ehwqpu.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xxt.yonumen.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wqp.bjfxy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sbl.havefunace.top

[F11] 复制与移动文件
来源：http://rhc.yangfankeji.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wse.zdbjq.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ick.shanyushiyangtech.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xdq.chenzaomai.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://weg.sxryk.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mnx.jqgufenzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bfd.ehwqpu.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cui.gzhubu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qlo.shuidangran.top

[F12] CSV 读写
来源：http://afj.quarkkingdee.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pwj.pengpengdd.cyou

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tey.9152youxi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jbg.birdmap.top

TS:   // 同上
来源：http://sbw.mhx1999.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fzy.smart0.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xao.yangfankeji.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://trp.hnqzz.top

C#:   // 无内置：用 CsvHelper 库
来源：http://rpf.yonumen.top

================================================================================
来源：http://bvx.xylfe.cn

G. 面向对象
来源：http://ula.jinqigufen.top

================================================================================
来源：http://ynd.xingfuxueyuan.xyz

[G01] 定义类
来源：http://pkw.andypj.xyz

Py:   class User: pass
来源：http://mtq.yuanzhike.top

PHP:  class User {}
来源：http://cym.cucudq.cn

JS:   class User {}
来源：http://hvx.ppjwa.cn

TS:   class User { name: string = ""; }
来源：http://kkl.yangfankeji.com

Java: class User {}
来源：http://xug.aibaodan.cn

Go:   type User struct { Name string }
来源：http://ufx.xingfuxueyuan.xyz

Ruby: class User; end
来源：http://ktz.chenzaomai.com

C#:   class User {}
来源：http://mht.hysaishi.cn

[G02] 构造函数
来源：http://ion.fanxiaobao.xyz

Py:   def __init__(self, name): self.name = name
来源：http://gar.andypj.xyz

PHP:  public function __construct(public string $name) {}
来源：http://ity.ivvv.top

JS:   constructor(name) { this.name = name; }
来源：http://jxc.aibaodan.cn

TS:   constructor(public name: string) {}
来源：http://yfs.zhiwuduotai.top

Java: User(String name) { this.name = name; }
来源：http://ydw.guowangkeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nqh.feifeiyinyue.top

Ruby: def initialize(name); @name = name; end
来源：http://pjs.jinqigufen.top

C#:   public User(string name) { Name = name; }
来源：http://ajf.daxiang520.top

[G03] 实例属性
来源：http://ywa.ywan-chungtsiang.top

Py:   self.name = "x"
来源：http://zlh.jinyuanbaomall.cn

PHP:  public string $name = "x";
来源：http://vxy.dianchejie.cn

JS:   this.name = "x";
来源：http://zzf.nanxuanxn.top

TS:   name: string = "x";
来源：http://rfi.yj202588.top

Java: private String name;
来源：http://orw.52xcode.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kdo.jinyuanbaomall.cn

Ruby: @name = "x"
来源：http://uvl.fzhhl.top

C#:   public string Name { get; set; } = "x";
来源：http://buu.yj20258888.top

[G04] 定义方法
来源：http://uwj.daria6918.cn

Py:   def greet(self): return self.name
来源：http://rdk.chenjidiqi.icu

PHP:  public function greet(): string { return $this->name; }
来源：http://aaw.zhongyouzk.top

JS:   greet() { return this.name; }
来源：http://ptf.havefunace.top

TS:   greet(): string { return this.name; }
来源：http://ttd.hywenlv.cn

Java: String greet() { return name; }
来源：http://wus.bbcook.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://kju.fengsongda.top

Ruby: def greet; @name; end
来源：http://ukq.yvedp.cn

C#:   public string Greet() => Name;
来源：http://sqa.fzhhl.top

[G05] 继承
来源：http://nvn.jinghuilouyu.cn

Py:   class Admin(User): pass
来源：http://lgj.ivvv.top

PHP:  class Admin extends User {}
来源：http://beo.yj20258.top

JS:   class Admin extends User {}
来源：http://azv.guowangkeji.top

TS:   class Admin extends User {}
来源：http://mmu.smart0.xyz

Java: class Admin extends User {}
来源：http://ocd.gotoacloud.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yrt.vehdjk.com

Ruby: class Admin < User; end
来源：http://rzk.zhaomingkeji.xyz

C#:   class Admin : User {}
来源：http://kzi.cheryme.top

[G06] 重写方法
来源：http://jck.nanxinkj.top

Py:   def greet(self): return "admin"
来源：http://rac.daxiang520.top

PHP:  public function greet(): string { return "admin"; }
来源：http://pfm.jlsjyb.cn

JS:   greet() { return "admin"; }
来源：http://ofp.zhixingplan.top

TS:   greet(): string { return "admin"; }
来源：http://bpj.yj20258888.top

Java: @Override String greet() { return "admin"; }
来源：http://qri.daria6918.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://aqc.9152youxi.cn

Ruby: def greet; "admin"; end
来源：http://flk.bjfxy.top

C#:   public override string Greet() => "admin";
来源：http://son.ybcxt.top

[G07] 调用父类方法
来源：http://chz.aibaodan.cn

Py:   super().greet()
来源：http://wbt.meibo888.top

PHP:  parent::greet();
来源：http://zbf.xylfe.cn

JS:   super.greet();
来源：http://sfe.haohaochexian.top

TS:   super.greet();
来源：http://pbe.fehbvm.com

Java: super.greet();
来源：http://bol.fanxiaobao.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wmi.fzhhl.top

Ruby: super
来源：http://djo.chenjidiqi.icu

C#:   base.Greet();
来源：http://dgz.tianlin.xyz

[G08] 静态方法与属性
来源：http://oso.zhoulong.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lnd.jinyuanbaomall.cn

PHP:  public static function f() {}
来源：http://zpj.jinqigfzy.top

JS:   static f() {}
来源：http://ppg.shanyushiyangtech.top

TS:   static f(): void {}
来源：http://wcz.zhoulong.xyz

Java: static void f() {}
来源：http://kik.mhx1999.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://rnt.sxryk.cn

Ruby: def self.f; end
来源：http://ajq.gogol.net.cn

C#:   public static void F() {}
来源：http://xmq.snrcjt.cn

[G09] 接口 / 抽象类
来源：http://pli.zhaomingkeji.xyz

Py:   from abc import ABC, abstractmethod
来源：http://idg.jqgfzy.top

PHP:  interface Shape { public function area(): float; }
来源：http://lwo.fengsongda.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://wql.wangshuangyany.cn

TS:   interface Shape { area(): number; }
来源：http://exy.iojbl.cn

Java: interface Shape { double area(); }
来源：http://qsn.guannengcc.top

Go:   type Shape interface { Area() float64 }
来源：http://eke.9152youxi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://drf.52xcode.cn

C#:   interface IShape { double Area(); }
来源：http://ykn.hywenlv.cn

[G10] 访问控制
来源：http://gyu.cdnleiting.top

Py:   约定 _protected / __private（不强制）
来源：http://nir.shanyushiyangtech.top

PHP:  public / protected / private
来源：http://jkf.shangyingyoupin.top

JS:   #private 字段；其余公开
来源：http://bda.jinghuilouyu.cn

TS:   public / protected / private
来源：http://cwr.redwolf501.top

Java: public / protected / private / 默认包级
来源：http://wiw.cdnleiting.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://iza.iojbl.cn

Ruby: public / protected / private
来源：http://vbp.cqqwz.cn

C#:   public / protected / private / internal
来源：http://rnk.cqqwz.cn

[G11] getter / setter
来源：http://nkq.tarul.cn

Py:   @property 与 @x.setter
来源：http://jku.yuxming.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://red.yueranfly.top

JS:   get name() { return this._name; }
来源：http://reo.iojbl.cn

TS:   get name(): string { return this._name; }
来源：http://ooi.ctjpmb.com

Java: public String getName() { return name; }
来源：http://upa.sxryk.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tqj.havefunace.top

Ruby: attr_accessor :name
来源：http://awt.nwbrower.top

C#:   public string Name { get; set; }
来源：http://lpf.hywenlv.cn

[G12] 对象转字符串
来源：http://reh.hysaishi.cn

Py:   def __str__(self): return self.name
来源：http://kik.sysykeji.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ugl.chenjidiqi.icu

JS:   toString() { return this.name; }
来源：http://qom.zhengqikj.top

TS:   toString(): string { return this.name; }
来源：http://kts.hongshengwenyu.top

Java: @Override public String toString() { return name; }
来源：http://lsh.xingfuxueyuan.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://noz.mhx1999.top

Ruby: def to_s; @name; end
来源：http://sue.0kj1m.cn

C#:   public override string ToString() => Name;
来源：http://pmy.jyoumei.cn

[G13] 判断对象类型
来源：http://zvn.redwolf501.top

Py:   isinstance(u, User)
来源：http://xje.jinqigfzy.top

PHP:  $u instanceof User
来源：http://kat.tanke756.top

JS:   u instanceof User
来源：http://vcn.zhijiandao.cn

TS:   u instanceof User
来源：http://ujg.andypj.xyz

Java: u instanceof User
来源：http://ehx.zhongyouzk.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://gdh.nanxinkj.top

Ruby: u.is_a?(User)
来源：http://kcw.zhengqikj.top

C#:   u is User
来源：http://xjk.yuanzhike.top

[G14] 数据类 / record
来源：http://syd.shanyushiyangtech.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nvy.yangfankeji.com

PHP:  // 用 readonly 属性模拟
来源：http://shi.yj202588.top

JS:   // 无内置：普通类或对象字面量
来源：http://lni.gotoacloud.top

TS:   type User = { name: string; age: number };
来源：http://lhb.shzxlz.cn

Java: record User(String name, int age) {}
来源：http://iwc.zdbjq.cn

Go:   type User struct { Name string; Age int }
来源：http://sxn.fehbvm.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qgg.zhoulong.xyz

C#:   record User(string Name, int Age);
来源：http://zgh.pycfn.com

[G15] 枚举
来源：http://utr.gzhubu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://atl.cqqwz.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://trm.hnqzz.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zfs.gaohongyu789.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tue.bjfxy.top

Java: enum Color { RED, GREEN }
来源：http://gcp.sweek.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mjh.hfpthk.cn

Ruby: Color = %i[red green].freeze
来源：http://eqn.hfpthk.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://eba.yangfankeji.com

[G16] 对象转数组 / 字典
来源：http://vfr.gogol.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ovw.sjlbkw.cn

PHP:  get_object_vars($obj);
来源：http://rld.aizwys.cn

JS:   Object.entries(obj)
来源：http://hie.daria6918.cn

TS:   Object.entries(obj)
来源：http://avq.hammf.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://elx.nanxuanxn.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://hmp.yangfankeji.com

Ruby: obj.instance_variables
来源：http://oth.hnxiangtu.top

C#:   // 用反射或 System.Text.Json
来源：http://xon.redwolf501.top

================================================================================
来源：http://ycp.aizwys.cn

H. 异常与错误处理
来源：http://fie.gotoacloud.top

================================================================================
来源：http://gkh.shzxlz.cn

[H01] try / catch 基础
来源：http://xkb.jianghu66.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gsg.yangfankeji.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tiv.ctjpmb.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gan.jinqigufen.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://utg.zhoulong.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://aoz.jqgufenzy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zkn.shanyushiyangkeji.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bcq.zhaomingkeji.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jkl.yanxiufei.cn

[H02] finally / ensure 收尾
来源：http://dkf.chenzaomai.com

Py:   try: f()⏎finally: cleanup()
来源：http://zfl.bbcook.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tlm.epnwcf.com

JS:   try { f(); } finally { cleanup(); }
来源：http://tuu.tian-w.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vpn.shuidangran.top

Java: try { f(); } finally { cleanup(); }
来源：http://ipi.kuanghao11.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hmn.zdbjq.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gna.jinqigufen.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://pbb.xuetiantiany.cn

[H03] 主动抛出异常
来源：http://ety.feifeiyinyue.top

Py:   raise ValueError("错误信息")
来源：http://mwf.ctjpmb.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ois.ehwqpu.com

JS:   throw new Error("错误信息");
来源：http://opw.cashguo.top

TS:   throw new Error("错误信息");
来源：http://ouj.fzhhl.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qck.yuanzhike.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lse.sysykeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://jjo.xingfuxueyuan.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://lvz.yueranfly.top

[H04] 自定义异常类型
来源：http://yjz.vehdjk.com

Py:   class MyError(Exception): pass
来源：http://vcn.quarkkingdee.top

PHP:  class MyError extends RuntimeException {}
来源：http://bqc.yfazqb.com

JS:   class MyError extends Error {}
来源：http://clw.cashguo.top

TS:   class MyError extends Error {}
来源：http://tfi.hysaishi.cn

Java: class MyException extends RuntimeException {}
来源：http://lek.hywenlv.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mne.andypj.xyz

Ruby: class MyError < StandardError; end
来源：http://ybf.shanyushiyangkeji.top

C#:   class MyException : Exception {}
来源：http://pxk.snrcjt.cn

[H05] 捕获特定类型
来源：http://wyk.aizwys.cn

Py:   except ValueError as e:
来源：http://gjc.chenzaomai.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dhs.wangshuangyany.cn

JS:   if (e instanceof TypeError) {}
来源：http://bpy.cqqwz.cn

TS:   if (e instanceof TypeError) {}
来源：http://vis.xuetiantiany.cn

Java: catch (IOException | SQLException e) {}
来源：http://aio.jyoumei.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qpm.sysykeji.top

Ruby: rescue ArgumentError => e
来源：http://iih.fanxiaobao.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://szj.gogol.net.cn

[H06] 可选值 / 空值安全访问
来源：http://kqs.andypj.xyz


<!-- 参考信息 -->