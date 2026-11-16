代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://iqw.daxiang520.top

Java: Files.readString(Path.of("a.txt"))
来源：http://azx.vqdsnc.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tlc.xinyue.icu

Ruby: File.read("a.txt")
来源：http://btb.ybcxt.top

C#:   File.ReadAllText("a.txt");
来源：http://snd.jinghuilouyu.cn

[F02] 逐行读取文件
来源：http://xbt.zycfv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://shd.shzxlz.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pug.jinqigfzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wtj.smart0.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ioc.jlsjyb.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wlj.sweek.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sys.hfpthk.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://phb.zhiwuduotai.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dkp.yueranfly.top

[F03] 写入文件（覆盖）
来源：http://hkg.fengsongda.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://iwe.dianchejie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yiq.fktsv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tjj.havefunace.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vxd.ctjpmb.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jfc.jinghuilouyu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hzm.ybcxt.top

Ruby: File.write("a.txt", "hi")
来源：http://pag.nwbrower.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ftk.fehbvm.com

[F04] 追加写入文件
来源：http://ykx.ctjpmb.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yrv.andypj.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xje.tianlin.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kqg.sysykeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sog.hywenlv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tnf.havefunace.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kua.0kj1m.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jjq.yonumen.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hsm.zhiwuduotai.top

[F05] 判断文件或目录是否存在
来源：http://uui.zycfv.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ysc.gzhubu.top

PHP:  file_exists("a.txt");
来源：http://izb.guowangkeji.top

JS:   fs.existsSync("a.txt")
来源：http://kig.hcnkem.com

TS:   fs.existsSync("a.txt")
来源：http://krk.cucudq.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://geo.jlsjyb.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zgw.yvedp.cn

Ruby: File.exist?("a.txt")
来源：http://nlg.shanyushiyangkeji.top

C#:   File.Exists("a.txt")
来源：http://hzz.xingfuxueyuan.xyz

[F06] 删除文件
来源：http://wqm.xingfuxueyuan.xyz

Py:   os.remove("a.txt")
来源：http://ibs.fengsongda.top

PHP:  unlink("a.txt");
来源：http://zqm.zhixingplan.top

JS:   fs.unlinkSync("a.txt")
来源：http://wii.vqdsnc.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qhw.yuxming.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ufk.wangdashe.top

Go:   os.Remove("a.txt")
来源：http://yjr.yongpay.top

Ruby: File.delete("a.txt")
来源：http://vxs.zhengqikj.top

C#:   File.Delete("a.txt");
来源：http://qec.daria6918.cn

[F07] 创建目录（含多级）
来源：http://uoy.vehdjk.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hae.svipenyu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pzo.ehwqpu.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ufp.fktsv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gce.nanxuanxn.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hdw.guowangkeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qwi.316326.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yaq.xziqi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zcd.daria6918.cn

[F08] 遍历目录
来源：http://jps.wangdashe.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://met.xinyue.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jds.jqgfzy.top

JS:   fs.readdirSync("dir")
来源：http://jfv.yanxiufei.cn

TS:   fs.readdirSync("dir")
来源：http://qhs.meibo888.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hwg.yangfankeji.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://fti.9152youxi.cn

Ruby: Dir.children("dir")
来源：http://kfr.fengsongda.top

C#:   Directory.GetFiles("dir")
来源：http://xcx.shangyingyoupin.top

[F09] 获取文件大小
来源：http://edw.zhongyouzk.top

Py:   os.path.getsize("a.txt")
来源：http://nwz.nwbrower.top

PHP:  filesize("a.txt");
来源：http://etu.jyoumei.cn

JS:   fs.statSync("a.txt").size
来源：http://ggr.cucudq.cn

TS:   fs.statSync("a.txt").size
来源：http://cox.yanxiufei.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dtp.sufxvd.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://orj.52xcode.cn

Ruby: File.size("a.txt")
来源：http://sgs.yongpay.top

C#:   new FileInfo("a.txt").Length
来源：http://sat.jiagoushi.top

[F10] 取文件扩展名 / 文件名
来源：http://cxb.ydjk.org.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://smp.yj20258888.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rfe.jqgfzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://knl.yj202588.top

TS:   path.extname("a.txt")
来源：http://nrp.tarul.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bqd.sufxvd.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://swy.birdmap.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://imv.shanyushiyangtech.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ipf.quarkkingdee.top

[F11] 复制与移动文件
来源：http://dku.pengpengdd.cyou

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pqn.0kj1m.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://krc.gzhubu.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mmv.hammf.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cnv.hywenlv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tkf.cdnleiting.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ctl.hongshengwenyu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cjt.0kj1m.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hnd.zdqjudy.top

[F12] CSV 读写
来源：http://nqc.chenlongwang.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fsz.chenzaomai.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://iwe.ctjpmb.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vrs.sjlbkw.cn

TS:   // 同上
来源：http://lxx.hesvh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://czs.smart0.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qsc.jinqigfzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vxl.nanxinkj.top

C#:   // 无内置：用 CsvHelper 库
来源：http://vim.yuxming.cn

================================================================================
来源：http://vbf.ctjpmb.com

G. 面向对象
来源：http://ove.yj202588.top

================================================================================
来源：http://afm.pycfn.com

[G01] 定义类
来源：http://cjw.fengsongda.top

Py:   class User: pass
来源：http://hky.ydzc1.top

PHP:  class User {}
来源：http://vio.yangfankeji.com

JS:   class User {}
来源：http://tmt.jiagoushi.top

TS:   class User { name: string = ""; }
来源：http://urk.jiagoushi.top

Java: class User {}
来源：http://aab.fanxiaobao.xyz

Go:   type User struct { Name string }
来源：http://hfb.pycfn.com

Ruby: class User; end
来源：http://ysf.bjfxy.top

C#:   class User {}
来源：http://hgi.cheryme.top

[G02] 构造函数
来源：http://awa.xylfe.cn

Py:   def __init__(self, name): self.name = name
来源：http://zfu.hysaishi.cn

PHP:  public function __construct(public string $name) {}
来源：http://kig.316326.xyz

JS:   constructor(name) { this.name = name; }
来源：http://ppn.fehbvm.com

TS:   constructor(public name: string) {}
来源：http://oea.zhijiandao.cn

Java: User(String name) { this.name = name; }
来源：http://hzy.chenlongwang.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wyu.epnwcf.com

Ruby: def initialize(name); @name = name; end
来源：http://kht.bbcook.cn

C#:   public User(string name) { Name = name; }
来源：http://lra.jyoumei.cn

[G03] 实例属性
来源：http://oqr.gzhubu.top

Py:   self.name = "x"
来源：http://cbz.gogol.net.cn

PHP:  public string $name = "x";
来源：http://und.smart0.xyz

JS:   this.name = "x";
来源：http://ltp.tarul.cn

TS:   name: string = "x";
来源：http://xgm.hnxiangtu.top

Java: private String name;
来源：http://cuv.chenjidiqi.icu

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wfs.hnqzz.top

Ruby: @name = "x"
来源：http://lny.yj20258888.top

C#:   public string Name { get; set; } = "x";
来源：http://ulb.redwolf501.top

[G04] 定义方法
来源：http://nav.xuanzx.com

Py:   def greet(self): return self.name
来源：http://clx.andypj.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://mba.cucudq.cn

JS:   greet() { return this.name; }
来源：http://slk.cheryme.top

TS:   greet(): string { return this.name; }
来源：http://sjv.hfpthk.cn

Java: String greet() { return name; }
来源：http://kts.yj202588.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://suo.yangfankeji.com

Ruby: def greet; @name; end
来源：http://akm.jyoumei.cn

C#:   public string Greet() => Name;
来源：http://glk.hysaishi.cn

[G05] 继承
来源：http://gne.yj202588.top

Py:   class Admin(User): pass
来源：http://wyg.fehbvm.com

PHP:  class Admin extends User {}
来源：http://spv.yanxiufei.cn

JS:   class Admin extends User {}
来源：http://veq.ydzc1.top

TS:   class Admin extends User {}
来源：http://kae.yuanzhike.top

Java: class Admin extends User {}
来源：http://zon.jinghuilouyu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://voo.pengpengdd.cyou

Ruby: class Admin < User; end
来源：http://nzo.xuetiantiany.cn

C#:   class Admin : User {}
来源：http://aul.jyoumei.cn

[G06] 重写方法
来源：http://ynj.fehbvm.com

Py:   def greet(self): return "admin"
来源：http://rtc.nanxuanxn.top

PHP:  public function greet(): string { return "admin"; }
来源：http://jvq.zhiwuduotai.top

JS:   greet() { return "admin"; }
来源：http://ieq.nwbrower.top

TS:   greet(): string { return "admin"; }
来源：http://mkd.0kj1m.cn

Java: @Override String greet() { return "admin"; }
来源：http://xam.meibo888.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lgu.yonumen.top

Ruby: def greet; "admin"; end
来源：http://yzf.hfpthk.cn

C#:   public override string Greet() => "admin";
来源：http://hmn.yanxiufei.cn

[G07] 调用父类方法
来源：http://spr.0kj1m.cn

Py:   super().greet()
来源：http://bgy.hywenlv.cn

PHP:  parent::greet();
来源：http://ywy.shangyingyoupin.top

JS:   super.greet();
来源：http://gye.daxiang520.top

TS:   super.greet();
来源：http://yiz.jinqigufen.top

Java: super.greet();
来源：http://btv.gzhubu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://abl.redwolf501.top

Ruby: super
来源：http://isx.sxryk.cn

C#:   base.Greet();
来源：http://bwm.yueranfly.top

[G08] 静态方法与属性
来源：http://did.ivvv.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xcn.yvedp.cn

PHP:  public static function f() {}
来源：http://prd.ppjwa.cn

JS:   static f() {}
来源：http://fzy.yj20258.top

TS:   static f(): void {}
来源：http://jws.guowangkeji.top

Java: static void f() {}
来源：http://sqm.vqdsnc.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://alz.bbcook.cn

Ruby: def self.f; end
来源：http://tjq.xinyue.icu

C#:   public static void F() {}
来源：http://xfe.quarkkingdee.top

[G09] 接口 / 抽象类
来源：http://fkm.yuanzhike.top

Py:   from abc import ABC, abstractmethod
来源：http://tmi.zhiwuduotai.top

PHP:  interface Shape { public function area(): float; }
来源：http://gmq.dashuyun.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://gmr.cashguo.top

TS:   interface Shape { area(): number; }
来源：http://qrx.guowangkeji.top

Java: interface Shape { double area(); }
来源：http://iia.daxiang520.top

Go:   type Shape interface { Area() float64 }
来源：http://uib.jinyuanbaomall.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nhl.sweek.top

C#:   interface IShape { double Area(); }
来源：http://hay.kuanghao11.cn

[G10] 访问控制
来源：http://mzk.haohaochexian.top

Py:   约定 _protected / __private（不强制）
来源：http://csf.hnxiangtu.top

PHP:  public / protected / private
来源：http://npg.cashguo.top

JS:   #private 字段；其余公开
来源：http://gcu.nanxinkj.top

TS:   public / protected / private
来源：http://ouu.shangyingyoupin.top

Java: public / protected / private / 默认包级
来源：http://eyy.xuanzx.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://tvj.bbcook.cn

Ruby: public / protected / private
来源：http://nom.zycfv.cn

C#:   public / protected / private / internal
来源：http://gvy.hammf.cn

[G11] getter / setter
来源：http://caz.hcnkem.com

Py:   @property 与 @x.setter
来源：http://vnf.zdqjudy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://rvi.jiagoushi.top

JS:   get name() { return this._name; }
来源：http://vzc.xinyue.icu

TS:   get name(): string { return this._name; }
来源：http://bzq.zhiwuduotai.top

Java: public String getName() { return name; }
来源：http://tsz.yj20258888.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://gch.jqgfzy.top

Ruby: attr_accessor :name
来源：http://mhy.yj20258.top

C#:   public string Name { get; set; }
来源：http://fbb.0kj1m.cn

[G12] 对象转字符串
来源：http://rdw.ctjpmb.com

Py:   def __str__(self): return self.name
来源：http://pde.ehwqpu.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://vqj.jiagoushi.top

JS:   toString() { return this.name; }
来源：http://psr.aibaodan.cn

TS:   toString(): string { return this.name; }
来源：http://cru.ydzc1.top

Java: @Override public String toString() { return name; }
来源：http://hge.yongpay.top

Go:   func (u User) String() string { return u.Name }
来源：http://nrd.smart0.xyz

Ruby: def to_s; @name; end
来源：http://wjm.hnxiangtu.top

C#:   public override string ToString() => Name;
来源：http://pzo.yuxming.cn

[G13] 判断对象类型
来源：http://dzw.zhaomingkeji.xyz

Py:   isinstance(u, User)
来源：http://civ.jyoumei.cn

PHP:  $u instanceof User
来源：http://cko.wangshuangyany.cn

JS:   u instanceof User
来源：http://gvs.ybcxt.top

TS:   u instanceof User
来源：http://rhn.jinghuilouyu.cn

Java: u instanceof User
来源：http://oit.yanxiufei.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xgh.dashuyun.cn

Ruby: u.is_a?(User)
来源：http://jvu.52xcode.cn

C#:   u is User
来源：http://owo.hammf.cn

[G14] 数据类 / record
来源：http://jbv.pycfn.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jvw.gogol.net.cn

PHP:  // 用 readonly 属性模拟
来源：http://epd.0kj1m.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vdo.jyoumei.cn

TS:   type User = { name: string; age: number };
来源：http://zfq.jlsjyb.cn

Java: record User(String name, int age) {}
来源：http://vdh.aizwys.cn

Go:   type User struct { Name string; Age int }
来源：http://jbc.gzhubu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mjn.jiagoushi.top

C#:   record User(string Name, int Age);
来源：http://xxy.zycfv.cn

[G15] 枚举
来源：http://yty.daria6918.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qhd.jinqigufen.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://dcq.yvedp.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vau.zhaomingkeji.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nxc.yueranfly.top

Java: enum Color { RED, GREEN }
来源：http://ars.9152youxi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qwg.nanxinkj.top

Ruby: Color = %i[red green].freeze
来源：http://xmt.ivvv.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jre.zhaomingkeji.xyz

[G16] 对象转数组 / 字典
来源：http://xnz.zycfv.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kdi.hysaishi.cn

PHP:  get_object_vars($obj);
来源：http://bxc.ydjk.org.cn

JS:   Object.entries(obj)
来源：http://sqf.kuanghao11.cn

TS:   Object.entries(obj)
来源：http://hjf.nanxuanxn.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://log.hysaishi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://czg.feifeiyinyue.top

Ruby: obj.instance_variables
来源：http://ffr.gotoacloud.top

C#:   // 用反射或 System.Text.Json
来源：http://psb.ywan-chungtsiang.top

================================================================================
来源：http://jnn.xuanzx.com

H. 异常与错误处理
来源：http://lwu.ehwqpu.com

================================================================================
来源：http://hwd.zhijiandao.cn

[H01] try / catch 基础
来源：http://dmw.cheryme.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bnw.gzhubu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jkl.c1oappe.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jmy.andypj.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sww.aizwys.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dfo.nanxinkj.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zxo.xuanzx.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tlm.cqqwz.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dmq.jinyuanbaomall.cn

[H02] finally / ensure 收尾
来源：http://muq.ctjpmb.com

Py:   try: f()⏎finally: cleanup()
来源：http://hor.ydjk.org.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bgw.aibaodan.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xro.pengpengdd.cyou

TS:   try { f(); } finally { cleanup(); }
来源：http://vxu.yonumen.top

Java: try { f(); } finally { cleanup(); }
来源：http://ffb.bbcook.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nls.jlsjyb.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kzv.zhiwuduotai.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://yuy.hywenlv.cn

[H03] 主动抛出异常
来源：http://zyk.shangyingyoupin.top

Py:   raise ValueError("错误信息")
来源：http://cat.sysykeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jdh.yuanzhike.top

JS:   throw new Error("错误信息");
来源：http://vso.jyoumei.cn

TS:   throw new Error("错误信息");
来源：http://wda.fanxiaobao.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://uny.nwbrower.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fdc.dashuyun.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fui.tian-w.cn

C#:   throw new ArgumentException("错误信息");
来源：http://dso.shanyushiyangkeji.top

[H04] 自定义异常类型
来源：http://nlt.tian-w.cn

Py:   class MyError(Exception): pass
来源：http://cds.gaohongyu789.top

PHP:  class MyError extends RuntimeException {}
来源：http://vlp.wangdashe.top

JS:   class MyError extends Error {}
来源：http://yks.yueranfly.top

TS:   class MyError extends Error {}
来源：http://oau.uphjek.com

Java: class MyException extends RuntimeException {}
来源：http://wqj.smart0.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bwm.hongshengwenyu.top

Ruby: class MyError < StandardError; end
来源：http://cfx.fanxiaobao.xyz

C#:   class MyException : Exception {}
来源：http://att.ctjpmb.com

[H05] 捕获特定类型
来源：http://iry.nanxinkj.top

Py:   except ValueError as e:
来源：http://rvp.feifeiyinyue.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gut.fengsongda.top

JS:   if (e instanceof TypeError) {}
来源：http://lwz.redwolf501.top

TS:   if (e instanceof TypeError) {}
来源：http://syi.dashuyun.cn

Java: catch (IOException | SQLException e) {}
来源：http://nou.aizwys.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tkn.hysaishi.cn

Ruby: rescue ArgumentError => e
来源：http://kqx.gzhubu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://khl.hammf.cn

[H06] 可选值 / 空值安全访问
来源：http://vgu.9152youxi.cn


<!-- 参考信息 -->