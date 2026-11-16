代发 wailian999

[F01] 读取整个文件
来源：http://vyi.chenjidiqi.icu

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tvh.shuidangran.top

PHP:  file_get_contents("a.txt");
来源：http://dgm.jyoumei.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yzh.bjfxy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ljf.bbcook.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://axc.hfpthk.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://roc.zhixingplan.top

Ruby: File.read("a.txt")
来源：http://alv.zycfv.cn

C#:   File.ReadAllText("a.txt");
来源：http://geu.guowangkeji.top

[F02] 逐行读取文件
来源：http://ccu.gotoacloud.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pts.jianghu66.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hxx.wangshuangyany.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zoz.xinyue.icu

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ljs.zhongyouzk.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rsb.hfpthk.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://uyc.fktsv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tld.wangshuangyany.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://iob.hywenlv.cn

[F03] 写入文件（覆盖）
来源：http://voq.meibo888.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://anc.cashguo.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://wty.yanxiufei.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vvm.tianlin.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vmx.ybcxt.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gey.chenjidiqi.icu

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gea.yuxming.cn

Ruby: File.write("a.txt", "hi")
来源：http://jyu.zhoulong.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ljr.0kj1m.cn

[F04] 追加写入文件
来源：http://wyd.yuxming.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kch.tianlin.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uju.guowangkeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dhg.yj20258.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://upc.pengpengdd.cyou

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zae.zhixingplan.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cgg.havefunace.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ojo.shangyingyoupin.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://izz.316326.xyz

[F05] 判断文件或目录是否存在
来源：http://zjj.xziqi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xbq.shangyingyoupin.top

PHP:  file_exists("a.txt");
来源：http://ouq.cashguo.top

JS:   fs.existsSync("a.txt")
来源：http://ypv.wangshuangyany.cn

TS:   fs.existsSync("a.txt")
来源：http://pur.jianghu66.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ywy.haohaochexian.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qfe.xziqi.cn

Ruby: File.exist?("a.txt")
来源：http://uvv.iojbl.cn

C#:   File.Exists("a.txt")
来源：http://nuu.dashuyun.cn

[F06] 删除文件
来源：http://jxf.zhengqikj.top

Py:   os.remove("a.txt")
来源：http://mks.havefunace.top

PHP:  unlink("a.txt");
来源：http://egh.zhiwuduotai.top

JS:   fs.unlinkSync("a.txt")
来源：http://sce.xinyue.icu

TS:   fs.unlinkSync("a.txt")
来源：http://nxh.jqgfzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jpu.cheryme.top

Go:   os.Remove("a.txt")
来源：http://nei.fanxiaobao.xyz

Ruby: File.delete("a.txt")
来源：http://oww.chenzaomai.com

C#:   File.Delete("a.txt");
来源：http://juu.cheryme.top

[F07] 创建目录（含多级）
来源：http://jej.ctjpmb.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dqs.hywenlv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vac.hesvh.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cgw.xylfe.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tfr.hesvh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://agk.sweek.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lal.gzhubu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://umu.hammf.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ljb.daria6918.cn

[F08] 遍历目录
来源：http://bgv.vqdsnc.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://opb.zhijiandao.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://npm.ybcxt.top

JS:   fs.readdirSync("dir")
来源：http://saj.jlsjyb.cn

TS:   fs.readdirSync("dir")
来源：http://ybk.shanyushiyangtech.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://aat.shangyingyoupin.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://umo.zycfv.cn

Ruby: Dir.children("dir")
来源：http://buw.iojbl.cn

C#:   Directory.GetFiles("dir")
来源：http://lbv.jqgfzy.top

[F09] 获取文件大小
来源：http://vhq.gogol.net.cn

Py:   os.path.getsize("a.txt")
来源：http://bim.gotoacloud.top

PHP:  filesize("a.txt");
来源：http://cci.haohaochexian.top

JS:   fs.statSync("a.txt").size
来源：http://bhc.xylfe.cn

TS:   fs.statSync("a.txt").size
来源：http://smy.hywenlv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hya.gogol.net.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zea.zhaomingkeji.xyz

Ruby: File.size("a.txt")
来源：http://mbv.xinyue.icu

C#:   new FileInfo("a.txt").Length
来源：http://wka.dashuyun.cn

[F10] 取文件扩展名 / 文件名
来源：http://ysz.aibaodan.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ldt.andypj.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lqs.ydzc1.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vzh.uphjek.com

TS:   path.extname("a.txt")
来源：http://tdm.shangyingyoupin.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vul.chenlongwang.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mvb.svipenyu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fof.xuanzx.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://auq.shanyushiyangkeji.top

[F11] 复制与移动文件
来源：http://wxp.bjfxy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://iaa.daria6918.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wcz.tanke756.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lqz.nanxinkj.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jci.dashuyun.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cef.zdbjq.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ehp.iojbl.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://smk.uphjek.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zif.fanxiaobao.xyz

[F12] CSV 读写
来源：http://jhy.ydjk.org.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://iqa.pengpengdd.cyou

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://otr.chenjidiqi.icu

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qai.shangyingyoupin.top

TS:   // 同上
来源：http://oic.birdmap.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zbv.fehbvm.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://aop.yongpay.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://iqq.kuanghao11.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xsi.gogol.net.cn

================================================================================
来源：http://zpo.mhx1999.top

G. 面向对象
来源：http://xij.dashuyun.cn

================================================================================
来源：http://foe.xingfuxueyuan.xyz

[G01] 定义类
来源：http://udm.dianchejie.cn

Py:   class User: pass
来源：http://kif.chenzaomai.com

PHP:  class User {}
来源：http://rrr.cheryme.top

JS:   class User {}
来源：http://mid.ppjwa.cn

TS:   class User { name: string = ""; }
来源：http://bsu.jinyuanbaomall.cn

Java: class User {}
来源：http://uzr.hesvh.cn

Go:   type User struct { Name string }
来源：http://hrs.dianchejie.cn

Ruby: class User; end
来源：http://yei.cdnleiting.top

C#:   class User {}
来源：http://lxr.hnqzz.top

[G02] 构造函数
来源：http://yfa.sweek.top

Py:   def __init__(self, name): self.name = name
来源：http://pil.yvedp.cn

PHP:  public function __construct(public string $name) {}
来源：http://bpf.ybcxt.top

JS:   constructor(name) { this.name = name; }
来源：http://yoc.daxiang520.top

TS:   constructor(public name: string) {}
来源：http://sdt.jinghuilouyu.cn

Java: User(String name) { this.name = name; }
来源：http://ceq.epnwcf.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cpq.xingfuxueyuan.xyz

Ruby: def initialize(name); @name = name; end
来源：http://cig.fehbvm.com

C#:   public User(string name) { Name = name; }
来源：http://zws.tianlin.xyz

[G03] 实例属性
来源：http://pls.xziqi.cn

Py:   self.name = "x"
来源：http://fhq.fzhhl.top

PHP:  public string $name = "x";
来源：http://gyo.52xcode.cn

JS:   this.name = "x";
来源：http://mtd.jqgufenzy.top

TS:   name: string = "x";
来源：http://kez.ctjpmb.com

Java: private String name;
来源：http://jpn.shangyingyoupin.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jqj.shuidangran.top

Ruby: @name = "x"
来源：http://hmj.redwolf501.top

C#:   public string Name { get; set; } = "x";
来源：http://hko.zhixingplan.top

[G04] 定义方法
来源：http://nzc.yuanzhike.top

Py:   def greet(self): return self.name
来源：http://pdm.pengpengdd.cyou

PHP:  public function greet(): string { return $this->name; }
来源：http://gxt.pengpengdd.cyou

JS:   greet() { return this.name; }
来源：http://rja.yonumen.top

TS:   greet(): string { return this.name; }
来源：http://fnj.smart0.xyz

Java: String greet() { return name; }
来源：http://zxo.mhx1999.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://luy.hfpthk.cn

Ruby: def greet; @name; end
来源：http://mzs.hywenlv.cn

C#:   public string Greet() => Name;
来源：http://asc.jyoumei.cn

[G05] 继承
来源：http://oxc.gzhubu.top

Py:   class Admin(User): pass
来源：http://btd.zhongyouzk.top

PHP:  class Admin extends User {}
来源：http://pay.yanxiufei.cn

JS:   class Admin extends User {}
来源：http://xja.ivvv.top

TS:   class Admin extends User {}
来源：http://yph.snrcjt.cn

Java: class Admin extends User {}
来源：http://nrw.zhoulong.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://onm.gaohongyu789.top

Ruby: class Admin < User; end
来源：http://amm.iojbl.cn

C#:   class Admin : User {}
来源：http://tjm.uphjek.com

[G06] 重写方法
来源：http://pni.dianchejie.cn

Py:   def greet(self): return "admin"
来源：http://bcn.0kj1m.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tuh.cqqwz.cn

JS:   greet() { return "admin"; }
来源：http://fwv.havefunace.top

TS:   greet(): string { return "admin"; }
来源：http://unr.yfazqb.com

Java: @Override String greet() { return "admin"; }
来源：http://hta.yongpay.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sei.xinyue.icu

Ruby: def greet; "admin"; end
来源：http://tcl.tarul.cn

C#:   public override string Greet() => "admin";
来源：http://hvw.vehdjk.com

[G07] 调用父类方法
来源：http://ais.jyoumei.cn

Py:   super().greet()
来源：http://zve.sufxvd.cn

PHP:  parent::greet();
来源：http://mpw.meibo888.top

JS:   super.greet();
来源：http://wad.jianghu66.top

TS:   super.greet();
来源：http://bbu.wangshuangyany.cn

Java: super.greet();
来源：http://xpv.cqqwz.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://oux.yangfankeji.com

Ruby: super
来源：http://jhr.meibo888.top

C#:   base.Greet();
来源：http://efn.zhaomingkeji.xyz

[G08] 静态方法与属性
来源：http://wrk.jqgufenzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://oug.fktsv.cn

PHP:  public static function f() {}
来源：http://rii.hcnkem.com

JS:   static f() {}
来源：http://anq.pycfn.com

TS:   static f(): void {}
来源：http://ads.0kj1m.cn

Java: static void f() {}
来源：http://vzn.zhengqikj.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://omj.guowangkeji.top

Ruby: def self.f; end
来源：http://fdx.birdmap.top

C#:   public static void F() {}
来源：http://cha.yj20258888.top

[G09] 接口 / 抽象类
来源：http://trj.tianlin.xyz

Py:   from abc import ABC, abstractmethod
来源：http://whj.gzhubu.top

PHP:  interface Shape { public function area(): float; }
来源：http://ebl.jinyuanbaomall.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fwp.shzxlz.cn

TS:   interface Shape { area(): number; }
来源：http://lyz.zhaomingkeji.xyz

Java: interface Shape { double area(); }
来源：http://zsn.pycfn.com

Go:   type Shape interface { Area() float64 }
来源：http://wbm.smart0.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gth.andypj.xyz

C#:   interface IShape { double Area(); }
来源：http://aho.c1oappe.top

[G10] 访问控制
来源：http://abk.ivvv.top

Py:   约定 _protected / __private（不强制）
来源：http://ivi.zhongyouzk.top

PHP:  public / protected / private
来源：http://ydh.meibo888.top

JS:   #private 字段；其余公开
来源：http://gtj.ydzc1.top

TS:   public / protected / private
来源：http://fan.tianlin.xyz

Java: public / protected / private / 默认包级
来源：http://zlm.zhengqikj.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://shq.cucudq.cn

Ruby: public / protected / private
来源：http://vwr.aibaodan.cn

C#:   public / protected / private / internal
来源：http://ish.daria6918.cn

[G11] getter / setter
来源：http://vfz.ydjk.org.cn

Py:   @property 与 @x.setter
来源：http://zyw.cqqwz.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ikz.cashguo.top

JS:   get name() { return this._name; }
来源：http://mac.smart0.xyz

TS:   get name(): string { return this._name; }
来源：http://ata.mhx1999.top

Java: public String getName() { return name; }
来源：http://quk.aizwys.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rkg.xingfuxueyuan.xyz

Ruby: attr_accessor :name
来源：http://xyu.ywan-chungtsiang.top

C#:   public string Name { get; set; }
来源：http://ocl.hongshengwenyu.top

[G12] 对象转字符串
来源：http://jwk.shanyushiyangkeji.top

Py:   def __str__(self): return self.name
来源：http://vqf.tanke756.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://gdq.daria6918.cn

JS:   toString() { return this.name; }
来源：http://zqt.yuxming.cn

TS:   toString(): string { return this.name; }
来源：http://oxp.yj20258.top

Java: @Override public String toString() { return name; }
来源：http://glb.jianghu66.top

Go:   func (u User) String() string { return u.Name }
来源：http://dpz.jinyuanbaomall.cn

Ruby: def to_s; @name; end
来源：http://txd.jyoumei.cn

C#:   public override string ToString() => Name;
来源：http://hyi.xingfuxueyuan.xyz

[G13] 判断对象类型
来源：http://xbz.hywenlv.cn

Py:   isinstance(u, User)
来源：http://pes.pengpengdd.cyou

PHP:  $u instanceof User
来源：http://viu.yfazqb.com

JS:   u instanceof User
来源：http://cxd.gotoacloud.top

TS:   u instanceof User
来源：http://tgm.jianghu66.top

Java: u instanceof User
来源：http://rjr.tanke756.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://avy.hnxiangtu.top

Ruby: u.is_a?(User)
来源：http://bmx.jinqigufen.top

C#:   u is User
来源：http://oin.epnwcf.com

[G14] 数据类 / record
来源：http://tyb.zycfv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://eeo.jinyuanbaomall.cn

PHP:  // 用 readonly 属性模拟
来源：http://ylt.tian-w.cn

JS:   // 无内置：普通类或对象字面量
来源：http://zmz.cdnleiting.top

TS:   type User = { name: string; age: number };
来源：http://izg.jlsjyb.cn

Java: record User(String name, int age) {}
来源：http://wnm.xylfe.cn

Go:   type User struct { Name string; Age int }
来源：http://cca.fanxiaobao.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ale.iojbl.cn

C#:   record User(string Name, int Age);
来源：http://yzu.hcnkem.com

[G15] 枚举
来源：http://hdc.zhiwuduotai.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yjt.quarkkingdee.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://poo.fktsv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fjt.cheryme.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hqa.xziqi.cn

Java: enum Color { RED, GREEN }
来源：http://jjz.shanyushiyangkeji.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xkp.epnwcf.com

Ruby: Color = %i[red green].freeze
来源：http://syn.316326.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vtr.dashuyun.cn

[G16] 对象转数组 / 字典
来源：http://pns.quarkkingdee.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pkn.316326.xyz

PHP:  get_object_vars($obj);
来源：http://oxh.yonumen.top

JS:   Object.entries(obj)
来源：http://ygf.xuetiantiany.cn

TS:   Object.entries(obj)
来源：http://xrq.yonumen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://enl.haohaochexian.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://dvy.zycfv.cn

Ruby: obj.instance_variables
来源：http://xqs.yanxiufei.cn

C#:   // 用反射或 System.Text.Json
来源：http://onv.ehwqpu.com

================================================================================
来源：http://usw.yj20258888.top

H. 异常与错误处理
来源：http://wjj.cdnleiting.top

================================================================================
来源：http://xei.jinqigufen.top

[H01] try / catch 基础
来源：http://ggt.mhx1999.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lql.gzhubu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gmb.yj20258.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rei.nwbrower.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dvj.jyoumei.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hxh.havefunace.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://psw.316326.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lqr.fehbvm.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://itv.yj202588.top

[H02] finally / ensure 收尾
来源：http://gsl.fktsv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mte.jinghuilouyu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fyw.tarul.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://oxr.yuanzhike.top

TS:   try { f(); } finally { cleanup(); }
来源：http://pqe.fengsongda.top

Java: try { f(); } finally { cleanup(); }
来源：http://mma.yonumen.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://spm.ehwqpu.com

Ruby: begin; f; ensure; cleanup; end
来源：http://pgg.zhiwuduotai.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://nas.chenzaomai.com

[H03] 主动抛出异常
来源：http://vpi.xuanzx.com

Py:   raise ValueError("错误信息")
来源：http://udo.hammf.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hui.epnwcf.com

JS:   throw new Error("错误信息");
来源：http://omz.jinghuilouyu.cn

TS:   throw new Error("错误信息");
来源：http://hgz.zhengqikj.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://smn.yanxiufei.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://opw.yanxiufei.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qhc.bbcook.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ffl.cucudq.cn

[H04] 自定义异常类型
来源：http://ynt.kuanghao11.cn

Py:   class MyError(Exception): pass
来源：http://qus.zhengqikj.top

PHP:  class MyError extends RuntimeException {}
来源：http://zij.guowangkeji.top

JS:   class MyError extends Error {}
来源：http://pfw.tarul.cn

TS:   class MyError extends Error {}
来源：http://nav.hnxiangtu.top

Java: class MyException extends RuntimeException {}
来源：http://lns.gaohongyu789.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uhy.jyoumei.cn

Ruby: class MyError < StandardError; end
来源：http://car.xinyue.icu

C#:   class MyException : Exception {}
来源：http://sfw.andypj.xyz

[H05] 捕获特定类型
来源：http://mqz.hnxiangtu.top

Py:   except ValueError as e:
来源：http://cji.gaohongyu789.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bbr.hysaishi.cn

JS:   if (e instanceof TypeError) {}
来源：http://xur.wangdashe.top

TS:   if (e instanceof TypeError) {}
来源：http://drp.cucudq.cn

Java: catch (IOException | SQLException e) {}
来源：http://qpu.fanxiaobao.xyz


<!-- 参考信息 -->