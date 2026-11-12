代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://amx.jinghuilouyu.cn

================================================================================
来源：http://hnc.bjfxy.top

F. 文件与目录
来源：http://aqd.bbcook.cn

================================================================================
来源：http://otz.yvedp.cn

[F01] 读取整个文件
来源：http://tvp.xylfe.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://oqp.xziqi.cn

PHP:  file_get_contents("a.txt");
来源：http://bgg.daxiang520.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://slz.wangshuangyany.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ynz.xingfuxueyuan.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://ftj.jinqigufen.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zpm.fehbvm.com

Ruby: File.read("a.txt")
来源：http://lvu.316326.xyz

C#:   File.ReadAllText("a.txt");
来源：http://ctm.jlsjyb.cn

[F02] 逐行读取文件
来源：http://qfo.vqdsnc.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ocb.zycfv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rlc.wangshuangyany.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pih.sjlbkw.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ibk.jiagoushi.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ipg.xuetiantiany.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vpt.pycfn.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://imk.daria6918.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yie.yongpay.top

[F03] 写入文件（覆盖）
来源：http://vit.yongpay.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zqg.yj20258888.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://wwn.gogol.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ens.hongshengwenyu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://col.havefunace.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://csk.bbcook.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lkz.cheryme.top

Ruby: File.write("a.txt", "hi")
来源：http://mjp.hongshengwenyu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cjs.shzxlz.cn

[F04] 追加写入文件
来源：http://tuj.chenlongwang.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ues.0kj1m.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://igy.hammf.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://czb.nwbrower.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xjr.zhijiandao.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mfa.ywan-chungtsiang.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ftd.ppjwa.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wdz.zdbjq.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vpi.zhijiandao.cn

[F05] 判断文件或目录是否存在
来源：http://jfp.yanxiufei.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hnr.pengpengdd.cyou

PHP:  file_exists("a.txt");
来源：http://xpa.shanyushiyangtech.top

JS:   fs.existsSync("a.txt")
来源：http://zut.zhixingplan.top

TS:   fs.existsSync("a.txt")
来源：http://mfs.yj20258.top

Java: Files.exists(Path.of("a.txt"))
来源：http://huw.jlsjyb.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dvq.hfpthk.cn

Ruby: File.exist?("a.txt")
来源：http://tne.epnwcf.com

C#:   File.Exists("a.txt")
来源：http://hav.pycfn.com

[F06] 删除文件
来源：http://xmz.sufxvd.cn

Py:   os.remove("a.txt")
来源：http://hve.yfazqb.com

PHP:  unlink("a.txt");
来源：http://val.zdqjudy.top

JS:   fs.unlinkSync("a.txt")
来源：http://pox.hysaishi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rtd.yuxming.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://avh.yangfankeji.com

Go:   os.Remove("a.txt")
来源：http://voq.zhixingplan.top

Ruby: File.delete("a.txt")
来源：http://bjd.nwbrower.top

C#:   File.Delete("a.txt");
来源：http://nsr.uphjek.com

[F07] 创建目录（含多级）
来源：http://tls.jinqigufen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mxj.ydjk.org.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jdt.jqgfzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fxj.ppjwa.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mzr.yuanzhike.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wvm.andypj.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yfz.zdqjudy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kjc.ppjwa.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sqq.feifeiyinyue.top

[F08] 遍历目录
来源：http://dup.jinyuanbaomall.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://smj.sxryk.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gqc.jinghuilouyu.cn

JS:   fs.readdirSync("dir")
来源：http://ulz.yonumen.top

TS:   fs.readdirSync("dir")
来源：http://zwq.xuetiantiany.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://brl.wangdashe.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://aib.yvedp.cn

Ruby: Dir.children("dir")
来源：http://eay.nanxinkj.top

C#:   Directory.GetFiles("dir")
来源：http://xxg.dashuyun.cn

[F09] 获取文件大小
来源：http://rnv.epnwcf.com

Py:   os.path.getsize("a.txt")
来源：http://sth.yueranfly.top

PHP:  filesize("a.txt");
来源：http://kkv.aizwys.cn

JS:   fs.statSync("a.txt").size
来源：http://rqj.cdnleiting.top

TS:   fs.statSync("a.txt").size
来源：http://lca.cqqwz.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qhs.ywan-chungtsiang.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ipf.nwbrower.top

Ruby: File.size("a.txt")
来源：http://aeg.gotoacloud.top

C#:   new FileInfo("a.txt").Length
来源：http://sgd.andypj.xyz

[F10] 取文件扩展名 / 文件名
来源：http://qhg.yangfankeji.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://scx.haohaochexian.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nud.zhoulong.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qhg.zycfv.cn

TS:   path.extname("a.txt")
来源：http://bcb.gaohongyu789.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pwn.ydzc1.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ysr.jinghuilouyu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bbz.uphjek.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hdi.feifeiyinyue.top

[F11] 复制与移动文件
来源：http://btn.pengpengdd.cyou

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lwo.birdmap.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uvz.dashuyun.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mul.hcnkem.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iab.yongpay.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hdz.jinqigufen.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gex.kuanghao11.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mqu.hammf.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://onc.gotoacloud.top

[F12] CSV 读写
来源：http://fxw.xziqi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rbc.chenzaomai.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ojc.quarkkingdee.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mpw.yangfankeji.com

TS:   // 同上
来源：http://nxm.jqgufenzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dvl.tian-w.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hpt.gotoacloud.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jxq.bbcook.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ajb.zhixingplan.top

================================================================================
来源：http://cfz.zhongyouzk.top

G. 面向对象
来源：http://kdq.epnwcf.com

================================================================================
来源：http://ofu.yj20258.top

[G01] 定义类
来源：http://xbg.birdmap.top

Py:   class User: pass
来源：http://duu.chenzaomai.com

PHP:  class User {}
来源：http://ccv.xylfe.cn

JS:   class User {}
来源：http://olc.fehbvm.com

TS:   class User { name: string = ""; }
来源：http://fzq.yuanzhike.top

Java: class User {}
来源：http://fem.zhaomingkeji.xyz

Go:   type User struct { Name string }
来源：http://ema.52xcode.cn

Ruby: class User; end
来源：http://jbd.andypj.xyz

C#:   class User {}
来源：http://brv.snrcjt.cn

[G02] 构造函数
来源：http://pui.tian-w.cn

Py:   def __init__(self, name): self.name = name
来源：http://zez.zhengqikj.top

PHP:  public function __construct(public string $name) {}
来源：http://mdy.gaohongyu789.top

JS:   constructor(name) { this.name = name; }
来源：http://kyp.xuanzx.com

TS:   constructor(public name: string) {}
来源：http://suw.kuanghao11.cn

Java: User(String name) { this.name = name; }
来源：http://yzm.yfazqb.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pwv.ehwqpu.com

Ruby: def initialize(name); @name = name; end
来源：http://zfk.zhixingplan.top

C#:   public User(string name) { Name = name; }
来源：http://zzh.smart0.xyz

[G03] 实例属性
来源：http://qgj.cheryme.top

Py:   self.name = "x"
来源：http://yvm.hongshengwenyu.top

PHP:  public string $name = "x";
来源：http://nor.ywan-chungtsiang.top

JS:   this.name = "x";
来源：http://lvl.chenjidiqi.icu

TS:   name: string = "x";
来源：http://mlq.cucudq.cn

Java: private String name;
来源：http://yxq.chenlongwang.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://swy.yongpay.top

Ruby: @name = "x"
来源：http://zlz.kuanghao11.cn

C#:   public string Name { get; set; } = "x";
来源：http://vui.zhongyouzk.top

[G04] 定义方法
来源：http://gfj.ydjk.org.cn

Py:   def greet(self): return self.name
来源：http://gon.jyoumei.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ukx.zhoulong.xyz

JS:   greet() { return this.name; }
来源：http://vsx.wangshuangyany.cn

TS:   greet(): string { return this.name; }
来源：http://lkv.xingfuxueyuan.xyz

Java: String greet() { return name; }
来源：http://msq.bjfxy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://dcn.ybcxt.top

Ruby: def greet; @name; end
来源：http://wbh.yj20258.top

C#:   public string Greet() => Name;
来源：http://ptp.yanxiufei.cn

[G05] 继承
来源：http://txr.vqdsnc.cn

Py:   class Admin(User): pass
来源：http://gmr.epnwcf.com

PHP:  class Admin extends User {}
来源：http://trt.yj202588.top

JS:   class Admin extends User {}
来源：http://szy.birdmap.top

TS:   class Admin extends User {}
来源：http://yig.smart0.xyz

Java: class Admin extends User {}
来源：http://jlo.redwolf501.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://iig.tarul.cn

Ruby: class Admin < User; end
来源：http://sfd.sxryk.cn

C#:   class Admin : User {}
来源：http://tkw.ydjk.org.cn

[G06] 重写方法
来源：http://xmy.yj20258888.top

Py:   def greet(self): return "admin"
来源：http://kib.feifeiyinyue.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ila.xziqi.cn

JS:   greet() { return "admin"; }
来源：http://don.gogol.net.cn

TS:   greet(): string { return "admin"; }
来源：http://egx.bbcook.cn

Java: @Override String greet() { return "admin"; }
来源：http://urz.epnwcf.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://laj.xziqi.cn

Ruby: def greet; "admin"; end
来源：http://rir.316326.xyz

C#:   public override string Greet() => "admin";
来源：http://jpz.zhoulong.xyz

[G07] 调用父类方法
来源：http://mcc.nanxuanxn.top

Py:   super().greet()
来源：http://esv.wangdashe.top

PHP:  parent::greet();
来源：http://yoc.hnqzz.top

JS:   super.greet();
来源：http://pbq.birdmap.top

TS:   super.greet();
来源：http://ipv.0kj1m.cn

Java: super.greet();
来源：http://gfq.zhaomingkeji.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zvb.shzxlz.cn

Ruby: super
来源：http://uuo.ydzc1.top

C#:   base.Greet();
来源：http://pyy.hysaishi.cn

[G08] 静态方法与属性
来源：http://nei.birdmap.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rcg.gaohongyu789.top

PHP:  public static function f() {}
来源：http://owq.jinyuanbaomall.cn

JS:   static f() {}
来源：http://wjy.yvedp.cn

TS:   static f(): void {}
来源：http://hvo.vehdjk.com

Java: static void f() {}
来源：http://wrs.sweek.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://swm.jqgufenzy.top

Ruby: def self.f; end
来源：http://zak.jinghuilouyu.cn

C#:   public static void F() {}
来源：http://htc.zhiwuduotai.top

[G09] 接口 / 抽象类
来源：http://wad.kuanghao11.cn

Py:   from abc import ABC, abstractmethod
来源：http://ybu.gotoacloud.top

PHP:  interface Shape { public function area(): float; }
来源：http://ils.feifeiyinyue.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://yij.xuetiantiany.cn

TS:   interface Shape { area(): number; }
来源：http://ign.guannengcc.top

Java: interface Shape { double area(); }
来源：http://fgx.xylfe.cn

Go:   type Shape interface { Area() float64 }
来源：http://uki.guannengcc.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sdj.c1oappe.top

C#:   interface IShape { double Area(); }
来源：http://uli.xuetiantiany.cn

[G10] 访问控制
来源：http://rzr.ywan-chungtsiang.top

Py:   约定 _protected / __private（不强制）
来源：http://zvt.yvedp.cn

PHP:  public / protected / private
来源：http://ioc.haohaochexian.top

JS:   #private 字段；其余公开
来源：http://eym.ydjk.org.cn

TS:   public / protected / private
来源：http://sim.gogol.net.cn

Java: public / protected / private / 默认包级
来源：http://xor.zhijiandao.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tma.hcnkem.com

Ruby: public / protected / private
来源：http://fat.zhiwuduotai.top

C#:   public / protected / private / internal
来源：http://rrr.ywan-chungtsiang.top

[G11] getter / setter
来源：http://vma.zhongyouzk.top

Py:   @property 与 @x.setter
来源：http://zfw.jqgufenzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://nio.cqqwz.cn

JS:   get name() { return this._name; }
来源：http://yjt.jinyuanbaomall.cn

TS:   get name(): string { return this._name; }
来源：http://img.hywenlv.cn

Java: public String getName() { return name; }
来源：http://vlr.svipenyu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xsz.sufxvd.cn

Ruby: attr_accessor :name
来源：http://nsr.chenjidiqi.icu

C#:   public string Name { get; set; }
来源：http://cfz.yfazqb.com

[G12] 对象转字符串
来源：http://kzb.yueranfly.top

Py:   def __str__(self): return self.name
来源：http://vnw.yvedp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lmq.jinqigufen.top

JS:   toString() { return this.name; }
来源：http://okw.yuanzhike.top

TS:   toString(): string { return this.name; }
来源：http://cxk.xingfuxueyuan.xyz

Java: @Override public String toString() { return name; }
来源：http://cso.xinyue.icu

Go:   func (u User) String() string { return u.Name }
来源：http://qse.kuanghao11.cn

Ruby: def to_s; @name; end
来源：http://qdi.uphjek.com

C#:   public override string ToString() => Name;
来源：http://jzo.ctjpmb.com

[G13] 判断对象类型
来源：http://mnh.cashguo.top

Py:   isinstance(u, User)
来源：http://zmi.epnwcf.com

PHP:  $u instanceof User
来源：http://lni.mhx1999.top

JS:   u instanceof User
来源：http://bsx.yj20258888.top

TS:   u instanceof User
来源：http://qbo.hysaishi.cn

Java: u instanceof User
来源：http://gkk.hfpthk.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://znm.birdmap.top

Ruby: u.is_a?(User)
来源：http://qeg.xuanzx.com

C#:   u is User
来源：http://ttf.sysykeji.top

[G14] 数据类 / record
来源：http://ack.bbcook.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vst.sufxvd.cn

PHP:  // 用 readonly 属性模拟
来源：http://hlp.bbcook.cn

JS:   // 无内置：普通类或对象字面量
来源：http://txz.feifeiyinyue.top

TS:   type User = { name: string; age: number };
来源：http://ken.jinyuanbaomall.cn

Java: record User(String name, int age) {}
来源：http://ikj.hnxiangtu.top

Go:   type User struct { Name string; Age int }
来源：http://mwq.xingfuxueyuan.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kco.havefunace.top

C#:   record User(string Name, int Age);
来源：http://ohd.xylfe.cn

[G15] 枚举
来源：http://syh.andypj.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xpa.zhengqikj.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://byf.mhx1999.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pfm.cqqwz.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qvb.ydjk.org.cn

Java: enum Color { RED, GREEN }
来源：http://mrx.shzxlz.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mow.c1oappe.top

Ruby: Color = %i[red green].freeze
来源：http://yvu.gogol.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iah.wangshuangyany.cn

[G16] 对象转数组 / 字典
来源：http://spc.hnqzz.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://iyu.hesvh.cn

PHP:  get_object_vars($obj);
来源：http://pcp.tanke756.top

JS:   Object.entries(obj)
来源：http://pba.shzxlz.cn

TS:   Object.entries(obj)
来源：http://jct.nanxuanxn.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://teu.gzhubu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://sqt.9152youxi.cn

Ruby: obj.instance_variables
来源：http://bxb.dianchejie.cn

C#:   // 用反射或 System.Text.Json
来源：http://tsz.xylfe.cn

================================================================================
来源：http://hut.shzxlz.cn

H. 异常与错误处理
来源：http://tel.jinghuilouyu.cn

================================================================================
来源：http://jyz.wangdashe.top

[H01] try / catch 基础
来源：http://dnt.zhixingplan.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://unh.sufxvd.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://oqc.jinghuilouyu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://izh.ydjk.org.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yqz.xziqi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://srg.yj20258.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://iff.hywenlv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xri.316326.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wpw.hfpthk.cn

[H02] finally / ensure 收尾
来源：http://rxl.jinghuilouyu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://yfk.9152youxi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fvw.jinqigufen.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ksf.iojbl.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://llo.xingfuxueyuan.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://yqj.chenzaomai.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://rgt.xinyue.icu

Ruby: begin; f; ensure; cleanup; end
来源：http://kzw.bjfxy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ygi.nanxuanxn.top

[H03] 主动抛出异常
来源：http://rka.cheryme.top

Py:   raise ValueError("错误信息")
来源：http://fhb.svipenyu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gpm.bbcook.cn

JS:   throw new Error("错误信息");
来源：http://fqd.ydjk.org.cn

TS:   throw new Error("错误信息");
来源：http://hgb.yvedp.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mcs.snrcjt.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jpa.hammf.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lja.bbcook.cn

C#:   throw new ArgumentException("错误信息");
来源：http://eem.meibo888.top

[H04] 自定义异常类型
来源：http://ytb.hesvh.cn

Py:   class MyError(Exception): pass
来源：http://spv.haohaochexian.top

PHP:  class MyError extends RuntimeException {}
来源：http://lxf.meibo888.top

JS:   class MyError extends Error {}
来源：http://ion.nanxuanxn.top

TS:   class MyError extends Error {}
来源：http://yma.ydjk.org.cn

Java: class MyException extends RuntimeException {}
来源：http://yxy.c1oappe.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://agp.yuxming.cn

Ruby: class MyError < StandardError; end
来源：http://xkg.gotoacloud.top

C#:   class MyException : Exception {}
来源：http://gyr.shanyushiyangkeji.top

[H05] 捕获特定类型
来源：http://mgx.epnwcf.com

Py:   except ValueError as e:
来源：http://cyu.xingfuxueyuan.xyz


<!-- 参考信息 -->