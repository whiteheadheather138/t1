代发 wailian999

[F01] 读取整个文件
来源：http://dgo.hesvh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bqm.zhiwuduotai.top

PHP:  file_get_contents("a.txt");
来源：http://hxa.aizwys.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dgy.daria6918.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xme.tarul.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mhw.aizwys.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rae.tian-w.cn

Ruby: File.read("a.txt")
来源：http://agu.haohaochexian.top

C#:   File.ReadAllText("a.txt");
来源：http://ebz.xinyue.icu

[F02] 逐行读取文件
来源：http://ith.zhengqikj.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://klx.quarkkingdee.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lwj.yangfankeji.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hcc.vehdjk.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lvi.gotoacloud.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mqv.jinghuilouyu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mec.yuanzhike.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mig.fzhhl.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fzs.fktsv.cn

[F03] 写入文件（覆盖）
来源：http://yzn.yj20258888.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ycf.hywenlv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://deh.feifeiyinyue.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uao.yj202588.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tfb.jyoumei.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vwm.birdmap.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://oxt.xingfuxueyuan.xyz

Ruby: File.write("a.txt", "hi")
来源：http://maf.gaohongyu789.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dfz.jqgufenzy.top

[F04] 追加写入文件
来源：http://ucy.wangshuangyany.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vtu.daria6918.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://eyo.yj20258.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xmo.dianchejie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mun.fanxiaobao.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dqa.zhixingplan.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://quu.jqgufenzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qpi.ivvv.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kwb.bjfxy.top

[F05] 判断文件或目录是否存在
来源：http://nzj.bjfxy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rvp.zhongyouzk.top

PHP:  file_exists("a.txt");
来源：http://uwb.havefunace.top

JS:   fs.existsSync("a.txt")
来源：http://cem.xuanzx.com

TS:   fs.existsSync("a.txt")
来源：http://nqe.316326.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://eed.gaohongyu789.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tui.9152youxi.cn

Ruby: File.exist?("a.txt")
来源：http://hww.epnwcf.com

C#:   File.Exists("a.txt")
来源：http://pju.mhx1999.top

[F06] 删除文件
来源：http://eeh.birdmap.top

Py:   os.remove("a.txt")
来源：http://lix.zhijiandao.cn

PHP:  unlink("a.txt");
来源：http://dki.cheryme.top

JS:   fs.unlinkSync("a.txt")
来源：http://mmx.zhiwuduotai.top

TS:   fs.unlinkSync("a.txt")
来源：http://ele.ctjpmb.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://und.gaohongyu789.top

Go:   os.Remove("a.txt")
来源：http://axw.nwbrower.top

Ruby: File.delete("a.txt")
来源：http://yen.svipenyu.cn

C#:   File.Delete("a.txt");
来源：http://voa.9152youxi.cn

[F07] 创建目录（含多级）
来源：http://dje.xylfe.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nmv.jqgufenzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lgr.sufxvd.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pnb.zhengqikj.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eug.xziqi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fkx.kuanghao11.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ayl.xingfuxueyuan.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rgn.yongpay.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ddk.ppjwa.cn

[F08] 遍历目录
来源：http://llp.ydjk.org.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cuo.cqqwz.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jej.zdbjq.cn

JS:   fs.readdirSync("dir")
来源：http://sdp.snrcjt.cn

TS:   fs.readdirSync("dir")
来源：http://edz.nanxuanxn.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://npq.gogol.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vvi.cashguo.top

Ruby: Dir.children("dir")
来源：http://mmy.sweek.top

C#:   Directory.GetFiles("dir")
来源：http://rfe.andypj.xyz

[F09] 获取文件大小
来源：http://fxd.shzxlz.cn

Py:   os.path.getsize("a.txt")
来源：http://bjh.wangdashe.top

PHP:  filesize("a.txt");
来源：http://mpy.yj202588.top

JS:   fs.statSync("a.txt").size
来源：http://umy.zhengqikj.top

TS:   fs.statSync("a.txt").size
来源：http://ebv.52xcode.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fce.shangyingyoupin.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tzn.ppjwa.cn

Ruby: File.size("a.txt")
来源：http://xvb.jiagoushi.top

C#:   new FileInfo("a.txt").Length
来源：http://fcr.aizwys.cn

[F10] 取文件扩展名 / 文件名
来源：http://dxe.yuxming.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tlo.aibaodan.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lnp.haohaochexian.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dqy.jqgufenzy.top

TS:   path.extname("a.txt")
来源：http://koh.hfpthk.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blh.tian-w.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rna.yj20258.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hnc.kuanghao11.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://azc.c1oappe.top

[F11] 复制与移动文件
来源：http://kjz.52xcode.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hzm.vehdjk.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yyt.cashguo.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vue.hongshengwenyu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vyk.fengsongda.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ewt.sysykeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bfu.daxiang520.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bco.chenjidiqi.icu

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dxg.pengpengdd.cyou

[F12] CSV 读写
来源：http://mdb.ywan-chungtsiang.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jwe.sysykeji.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ger.sweek.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gml.0kj1m.cn

TS:   // 同上
来源：http://byy.tianlin.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ppg.cheryme.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xmd.cqqwz.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pis.bjfxy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://qtu.birdmap.top

================================================================================
来源：http://nsr.fehbvm.com

G. 面向对象
来源：http://sim.tian-w.cn

================================================================================
来源：http://lye.bbcook.cn

[G01] 定义类
来源：http://fsf.smart0.xyz

Py:   class User: pass
来源：http://kkb.sufxvd.cn

PHP:  class User {}
来源：http://gyz.zhengqikj.top

JS:   class User {}
来源：http://zvt.yongpay.top

TS:   class User { name: string = ""; }
来源：http://wie.ehwqpu.com

Java: class User {}
来源：http://kxq.snrcjt.cn

Go:   type User struct { Name string }
来源：http://hqa.iojbl.cn

Ruby: class User; end
来源：http://ssp.hnqzz.top

C#:   class User {}
来源：http://pva.gogol.net.cn

[G02] 构造函数
来源：http://dqs.fehbvm.com

Py:   def __init__(self, name): self.name = name
来源：http://xmp.cashguo.top

PHP:  public function __construct(public string $name) {}
来源：http://reo.pycfn.com

JS:   constructor(name) { this.name = name; }
来源：http://ubj.0kj1m.cn

TS:   constructor(public name: string) {}
来源：http://cpx.dianchejie.cn

Java: User(String name) { this.name = name; }
来源：http://sig.gaohongyu789.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://whf.nanxinkj.top

Ruby: def initialize(name); @name = name; end
来源：http://zhx.fengsongda.top

C#:   public User(string name) { Name = name; }
来源：http://cgi.gaohongyu789.top

[G03] 实例属性
来源：http://hcs.dashuyun.cn

Py:   self.name = "x"
来源：http://vkk.vqdsnc.cn

PHP:  public string $name = "x";
来源：http://psr.epnwcf.com

JS:   this.name = "x";
来源：http://dxn.dianchejie.cn

TS:   name: string = "x";
来源：http://fqm.vqdsnc.cn

Java: private String name;
来源：http://wtr.aibaodan.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fkp.cashguo.top

Ruby: @name = "x"
来源：http://mad.yonumen.top

C#:   public string Name { get; set; } = "x";
来源：http://giv.kuanghao11.cn

[G04] 定义方法
来源：http://hzd.hywenlv.cn

Py:   def greet(self): return self.name
来源：http://hbt.shanyushiyangkeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://bih.chenlongwang.top

JS:   greet() { return this.name; }
来源：http://eyx.xinyue.icu

TS:   greet(): string { return this.name; }
来源：http://rpl.sjlbkw.cn

Java: String greet() { return name; }
来源：http://kxb.sweek.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://rjw.xuanzx.com

Ruby: def greet; @name; end
来源：http://eed.fzhhl.top

C#:   public string Greet() => Name;
来源：http://vsg.zycfv.cn

[G05] 继承
来源：http://pvf.9152youxi.cn

Py:   class Admin(User): pass
来源：http://qcy.yuanzhike.top

PHP:  class Admin extends User {}
来源：http://zso.tianlin.xyz

JS:   class Admin extends User {}
来源：http://nsm.nanxuanxn.top

TS:   class Admin extends User {}
来源：http://bnc.bjfxy.top

Java: class Admin extends User {}
来源：http://kdq.feifeiyinyue.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://auh.yfazqb.com

Ruby: class Admin < User; end
来源：http://cfo.hnqzz.top

C#:   class Admin : User {}
来源：http://hei.fanxiaobao.xyz

[G06] 重写方法
来源：http://eze.fengsongda.top

Py:   def greet(self): return "admin"
来源：http://cwr.pycfn.com

PHP:  public function greet(): string { return "admin"; }
来源：http://bcp.bbcook.cn

JS:   greet() { return "admin"; }
来源：http://num.c1oappe.top

TS:   greet(): string { return "admin"; }
来源：http://pum.dashuyun.cn

Java: @Override String greet() { return "admin"; }
来源：http://kyn.9152youxi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kqf.jqgfzy.top

Ruby: def greet; "admin"; end
来源：http://aps.xinyue.icu

C#:   public override string Greet() => "admin";
来源：http://dhs.uphjek.com

[G07] 调用父类方法
来源：http://vpn.fanxiaobao.xyz

Py:   super().greet()
来源：http://zei.shzxlz.cn

PHP:  parent::greet();
来源：http://bce.dianchejie.cn

JS:   super.greet();
来源：http://jhh.cqqwz.cn

TS:   super.greet();
来源：http://adx.gotoacloud.top

Java: super.greet();
来源：http://whb.hesvh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yvf.ywan-chungtsiang.top

Ruby: super
来源：http://ybm.bjfxy.top

C#:   base.Greet();
来源：http://mbd.zhaomingkeji.xyz

[G08] 静态方法与属性
来源：http://ler.ehwqpu.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yiw.fanxiaobao.xyz

PHP:  public static function f() {}
来源：http://wwg.zhaomingkeji.xyz

JS:   static f() {}
来源：http://buy.cashguo.top

TS:   static f(): void {}
来源：http://wwq.xuetiantiany.cn

Java: static void f() {}
来源：http://wbs.sweek.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://bfw.ywan-chungtsiang.top

Ruby: def self.f; end
来源：http://ygx.pengpengdd.cyou

C#:   public static void F() {}
来源：http://jhl.gzhubu.top

[G09] 接口 / 抽象类
来源：http://zrj.yuanzhike.top

Py:   from abc import ABC, abstractmethod
来源：http://pzl.svipenyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://koc.ydzc1.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://yrt.birdmap.top

TS:   interface Shape { area(): number; }
来源：http://vsf.bbcook.cn

Java: interface Shape { double area(); }
来源：http://udn.birdmap.top

Go:   type Shape interface { Area() float64 }
来源：http://alg.fzhhl.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vat.havefunace.top

C#:   interface IShape { double Area(); }
来源：http://gef.ywan-chungtsiang.top

[G10] 访问控制
来源：http://vrq.cqqwz.cn

Py:   约定 _protected / __private（不强制）
来源：http://lfk.xuanzx.com

PHP:  public / protected / private
来源：http://dts.aibaodan.cn

JS:   #private 字段；其余公开
来源：http://ujm.jqgufenzy.top

TS:   public / protected / private
来源：http://odh.wangdashe.top

Java: public / protected / private / 默认包级
来源：http://pbh.hammf.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mca.tian-w.cn

Ruby: public / protected / private
来源：http://jyd.ehwqpu.com

C#:   public / protected / private / internal
来源：http://ugu.aibaodan.cn

[G11] getter / setter
来源：http://nwd.nanxinkj.top

Py:   @property 与 @x.setter
来源：http://dti.ybcxt.top

PHP:  public function getName(): string { return $this->name; }
来源：http://wns.chenjidiqi.icu

JS:   get name() { return this._name; }
来源：http://nku.sxryk.cn

TS:   get name(): string { return this._name; }
来源：http://zdn.sjlbkw.cn

Java: public String getName() { return name; }
来源：http://nvw.cucudq.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jpe.0kj1m.cn

Ruby: attr_accessor :name
来源：http://sab.zhengqikj.top

C#:   public string Name { get; set; }
来源：http://fud.nanxuanxn.top

[G12] 对象转字符串
来源：http://jln.ivvv.top

Py:   def __str__(self): return self.name
来源：http://daa.9152youxi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ung.xuetiantiany.cn

JS:   toString() { return this.name; }
来源：http://qin.iojbl.cn

TS:   toString(): string { return this.name; }
来源：http://ijb.hesvh.cn

Java: @Override public String toString() { return name; }
来源：http://enk.xinyue.icu

Go:   func (u User) String() string { return u.Name }
来源：http://vzj.aizwys.cn

Ruby: def to_s; @name; end
来源：http://spg.316326.xyz

C#:   public override string ToString() => Name;
来源：http://ayn.xinyue.icu

[G13] 判断对象类型
来源：http://tzm.xinyue.icu

Py:   isinstance(u, User)
来源：http://ugk.cucudq.cn

PHP:  $u instanceof User
来源：http://hql.zycfv.cn

JS:   u instanceof User
来源：http://odd.birdmap.top

TS:   u instanceof User
来源：http://aoe.gogol.net.cn

Java: u instanceof User
来源：http://udr.fzhhl.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://cie.jyoumei.cn

Ruby: u.is_a?(User)
来源：http://kqi.yonumen.top

C#:   u is User
来源：http://akk.gotoacloud.top

[G14] 数据类 / record
来源：http://ajk.hcnkem.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wgl.nanxinkj.top

PHP:  // 用 readonly 属性模拟
来源：http://fdk.ppjwa.cn

JS:   // 无内置：普通类或对象字面量
来源：http://uku.shuidangran.top

TS:   type User = { name: string; age: number };
来源：http://eqy.zhongyouzk.top

Java: record User(String name, int age) {}
来源：http://yzd.sweek.top

Go:   type User struct { Name string; Age int }
来源：http://ncr.xylfe.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vwj.ybcxt.top

C#:   record User(string Name, int Age);
来源：http://ktv.dashuyun.cn

[G15] 枚举
来源：http://slo.shanyushiyangtech.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fvl.wangshuangyany.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qwt.zhongyouzk.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dbg.bjfxy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mgl.tian-w.cn

Java: enum Color { RED, GREEN }
来源：http://krn.zdqjudy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ndw.yfazqb.com

Ruby: Color = %i[red green].freeze
来源：http://ofz.vehdjk.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wur.jyoumei.cn

[G16] 对象转数组 / 字典
来源：http://buy.ehwqpu.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ymk.xuanzx.com

PHP:  get_object_vars($obj);
来源：http://wxg.cqqwz.cn

JS:   Object.entries(obj)
来源：http://iuc.52xcode.cn

TS:   Object.entries(obj)
来源：http://uqc.ctjpmb.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://htn.shanyushiyangkeji.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://aku.gogol.net.cn

Ruby: obj.instance_variables
来源：http://lfs.wangdashe.top

C#:   // 用反射或 System.Text.Json
来源：http://rwz.gzhubu.top

================================================================================
来源：http://woo.c1oappe.top

H. 异常与错误处理
来源：http://nck.zhongyouzk.top

================================================================================
来源：http://vre.jiagoushi.top

[H01] try / catch 基础
来源：http://bwg.chenlongwang.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zdj.shuidangran.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ojj.guannengcc.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://asa.fengsongda.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ubc.redwolf501.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rqq.haohaochexian.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://njm.yj202588.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jvs.vqdsnc.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vis.iojbl.cn

[H02] finally / ensure 收尾
来源：http://nem.pengpengdd.cyou

Py:   try: f()⏎finally: cleanup()
来源：http://hso.jqgufenzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ztc.0kj1m.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wnq.yongpay.top

TS:   try { f(); } finally { cleanup(); }
来源：http://kkt.haohaochexian.top

Java: try { f(); } finally { cleanup(); }
来源：http://psl.sweek.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://pis.tarul.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rpw.hnqzz.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://yfz.bbcook.cn

[H03] 主动抛出异常
来源：http://cnz.zhongyouzk.top

Py:   raise ValueError("错误信息")
来源：http://aur.kuanghao11.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hqy.dianchejie.cn

JS:   throw new Error("错误信息");
来源：http://vqr.cdnleiting.top

TS:   throw new Error("错误信息");
来源：http://jtw.yvedp.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pkg.xinyue.icu

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jgs.shanyushiyangkeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://jch.mhx1999.top

C#:   throw new ArgumentException("错误信息");
来源：http://abu.dianchejie.cn

[H04] 自定义异常类型
来源：http://gtf.yanxiufei.cn

Py:   class MyError(Exception): pass
来源：http://dzy.nwbrower.top

PHP:  class MyError extends RuntimeException {}
来源：http://fay.9152youxi.cn

JS:   class MyError extends Error {}
来源：http://btd.zhoulong.xyz

TS:   class MyError extends Error {}
来源：http://kqd.shangyingyoupin.top

Java: class MyException extends RuntimeException {}
来源：http://cmi.ydjk.org.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://for.feifeiyinyue.top

Ruby: class MyError < StandardError; end
来源：http://psc.hnxiangtu.top

C#:   class MyException : Exception {}
来源：http://kql.yfazqb.com

[H05] 捕获特定类型
来源：http://rbh.meibo888.top

Py:   except ValueError as e:
来源：http://djh.zdqjudy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hmd.smart0.xyz

JS:   if (e instanceof TypeError) {}
来源：http://uhm.iojbl.cn

TS:   if (e instanceof TypeError) {}
来源：http://xlq.xylfe.cn

Java: catch (IOException | SQLException e) {}
来源：http://qeq.fanxiaobao.xyz


<!-- 参考信息 -->