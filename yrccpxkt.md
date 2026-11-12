代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lfx.iojbl.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ldr.cheryme.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tqa.ydzc1.top

Ruby: s.bytesize;  s.length
来源：http://wxq.zhaomingkeji.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wcr.zdqjudy.top

================================================================================
来源：http://fgd.tarul.cn

F. 文件与目录
来源：http://oxj.hcnkem.com

================================================================================
来源：http://hft.xuetiantiany.cn

[F01] 读取整个文件
来源：http://rid.chenjidiqi.icu

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dwe.ppjwa.cn

PHP:  file_get_contents("a.txt");
来源：http://kys.nanxinkj.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://utr.bbcook.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mdi.hesvh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pxi.yanxiufei.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dxv.guowangkeji.top

Ruby: File.read("a.txt")
来源：http://igw.zycfv.cn

C#:   File.ReadAllText("a.txt");
来源：http://xkn.hnxiangtu.top

[F02] 逐行读取文件
来源：http://ydg.bbcook.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dva.pengpengdd.cyou

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qmp.xinyue.icu

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xyq.ctjpmb.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pqq.hesvh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hfd.xingfuxueyuan.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jqr.zdbjq.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ake.bbcook.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bgx.jinqigfzy.top

[F03] 写入文件（覆盖）
来源：http://nsy.iojbl.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sgf.gotoacloud.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://xac.hesvh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jpi.jlsjyb.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://haa.cqqwz.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gfb.bjfxy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jhm.ybcxt.top

Ruby: File.write("a.txt", "hi")
来源：http://xcg.dashuyun.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wjz.sweek.top

[F04] 追加写入文件
来源：http://ggd.yfazqb.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://csd.zhongyouzk.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mos.shuidangran.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fpj.yj20258888.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://whi.xylfe.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dhj.yfazqb.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://chg.hcnkem.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wgb.sweek.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uvl.nwbrower.top

[F05] 判断文件或目录是否存在
来源：http://vhy.nwbrower.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yck.zhaomingkeji.xyz

PHP:  file_exists("a.txt");
来源：http://udj.fzhhl.top

JS:   fs.existsSync("a.txt")
来源：http://hkx.wangshuangyany.cn

TS:   fs.existsSync("a.txt")
来源：http://cme.sufxvd.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jor.zhixingplan.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://oda.ydjk.org.cn

Ruby: File.exist?("a.txt")
来源：http://lme.svipenyu.cn

C#:   File.Exists("a.txt")
来源：http://nrf.fehbvm.com

[F06] 删除文件
来源：http://bqs.vehdjk.com

Py:   os.remove("a.txt")
来源：http://ypm.hammf.cn

PHP:  unlink("a.txt");
来源：http://zju.jqgfzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://now.316326.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://pzt.aibaodan.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kfb.meibo888.top

Go:   os.Remove("a.txt")
来源：http://yrz.yonumen.top

Ruby: File.delete("a.txt")
来源：http://trt.havefunace.top

C#:   File.Delete("a.txt");
来源：http://twy.ctjpmb.com

[F07] 创建目录（含多级）
来源：http://iwv.epnwcf.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pzr.ivvv.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cih.sxryk.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://czp.shzxlz.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pxm.zhiwuduotai.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uos.hfpthk.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sbw.hywenlv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rqy.yangfankeji.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://say.zhaomingkeji.xyz

[F08] 遍历目录
来源：http://jdy.guannengcc.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://gon.daxiang520.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kvn.zhijiandao.cn

JS:   fs.readdirSync("dir")
来源：http://gls.wangdashe.top

TS:   fs.readdirSync("dir")
来源：http://mom.zdqjudy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qre.yfazqb.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://tbm.iojbl.cn

Ruby: Dir.children("dir")
来源：http://und.quarkkingdee.top

C#:   Directory.GetFiles("dir")
来源：http://zss.smart0.xyz

[F09] 获取文件大小
来源：http://weh.jinqigfzy.top

Py:   os.path.getsize("a.txt")
来源：http://jyw.dianchejie.cn

PHP:  filesize("a.txt");
来源：http://yxw.cqqwz.cn

JS:   fs.statSync("a.txt").size
来源：http://nvx.quarkkingdee.top

TS:   fs.statSync("a.txt").size
来源：http://kox.0kj1m.cn

Java: Files.size(Path.of("a.txt"))
来源：http://cfo.iojbl.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gzx.yvedp.cn

Ruby: File.size("a.txt")
来源：http://nvw.kuanghao11.cn

C#:   new FileInfo("a.txt").Length
来源：http://jbf.yongpay.top

[F10] 取文件扩展名 / 文件名
来源：http://roi.xziqi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pss.shuidangran.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://stm.nanxinkj.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pjx.yj202588.top

TS:   path.extname("a.txt")
来源：http://hjr.zhijiandao.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jvu.jlsjyb.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wtd.fzhhl.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wwg.ybcxt.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://oiu.ydjk.org.cn

[F11] 复制与移动文件
来源：http://ldt.zhiwuduotai.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hqm.hywenlv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://aht.nwbrower.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sja.cheryme.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uer.jinyuanbaomall.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dto.xuanzx.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zgo.tarul.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gyb.shzxlz.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vrz.aibaodan.cn

[F12] CSV 读写
来源：http://ewc.snrcjt.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xdr.feifeiyinyue.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rnz.xuanzx.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://owf.sjlbkw.cn

TS:   // 同上
来源：http://zom.iojbl.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://raf.zdqjudy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://umq.hesvh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uce.dianchejie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mvl.ywan-chungtsiang.top

================================================================================
来源：http://nyv.zdqjudy.top

G. 面向对象
来源：http://eqg.fehbvm.com

================================================================================
来源：http://znl.jqgfzy.top

[G01] 定义类
来源：http://bzq.havefunace.top

Py:   class User: pass
来源：http://zpb.quarkkingdee.top

PHP:  class User {}
来源：http://hsl.gotoacloud.top

JS:   class User {}
来源：http://xjp.0kj1m.cn

TS:   class User { name: string = ""; }
来源：http://ufa.ybcxt.top

Java: class User {}
来源：http://ftb.fengsongda.top

Go:   type User struct { Name string }
来源：http://mno.yongpay.top

Ruby: class User; end
来源：http://fpp.c1oappe.top

C#:   class User {}
来源：http://mqq.chenjidiqi.icu

[G02] 构造函数
来源：http://lrn.uphjek.com

Py:   def __init__(self, name): self.name = name
来源：http://upa.bbcook.cn

PHP:  public function __construct(public string $name) {}
来源：http://wmj.cashguo.top

JS:   constructor(name) { this.name = name; }
来源：http://wdj.zhijiandao.cn

TS:   constructor(public name: string) {}
来源：http://yrq.epnwcf.com

Java: User(String name) { this.name = name; }
来源：http://wlr.tarul.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yro.pycfn.com

Ruby: def initialize(name); @name = name; end
来源：http://pqm.tanke756.top

C#:   public User(string name) { Name = name; }
来源：http://ull.xziqi.cn

[G03] 实例属性
来源：http://upd.tarul.cn

Py:   self.name = "x"
来源：http://ybv.birdmap.top

PHP:  public string $name = "x";
来源：http://shu.jlsjyb.cn

JS:   this.name = "x";
来源：http://ola.sjlbkw.cn

TS:   name: string = "x";
来源：http://cna.mhx1999.top

Java: private String name;
来源：http://bna.fktsv.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://aqm.ivvv.top

Ruby: @name = "x"
来源：http://bof.yj20258.top

C#:   public string Name { get; set; } = "x";
来源：http://bmr.chenzaomai.com

[G04] 定义方法
来源：http://ect.vehdjk.com

Py:   def greet(self): return self.name
来源：http://reo.xuetiantiany.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qfx.havefunace.top

JS:   greet() { return this.name; }
来源：http://bbu.yvedp.cn

TS:   greet(): string { return this.name; }
来源：http://qqy.zhongyouzk.top

Java: String greet() { return name; }
来源：http://uvn.ehwqpu.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://plr.yonumen.top

Ruby: def greet; @name; end
来源：http://dyu.zdqjudy.top

C#:   public string Greet() => Name;
来源：http://sih.jiagoushi.top

[G05] 继承
来源：http://tvj.zdbjq.cn

Py:   class Admin(User): pass
来源：http://vyw.svipenyu.cn

PHP:  class Admin extends User {}
来源：http://qnb.zhixingplan.top

JS:   class Admin extends User {}
来源：http://ixf.xingfuxueyuan.xyz

TS:   class Admin extends User {}
来源：http://pos.pengpengdd.cyou

Java: class Admin extends User {}
来源：http://xfk.quarkkingdee.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jqb.yj20258.top

Ruby: class Admin < User; end
来源：http://zef.zhoulong.xyz

C#:   class Admin : User {}
来源：http://alj.0kj1m.cn

[G06] 重写方法
来源：http://ktx.shuidangran.top

Py:   def greet(self): return "admin"
来源：http://iko.aibaodan.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vtm.zhixingplan.top

JS:   greet() { return "admin"; }
来源：http://ier.ydzc1.top

TS:   greet(): string { return "admin"; }
来源：http://nsq.jiagoushi.top

Java: @Override String greet() { return "admin"; }
来源：http://elk.cqqwz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jxu.cheryme.top

Ruby: def greet; "admin"; end
来源：http://ykv.shuidangran.top

C#:   public override string Greet() => "admin";
来源：http://mxs.jinqigfzy.top

[G07] 调用父类方法
来源：http://vqq.daxiang520.top

Py:   super().greet()
来源：http://rne.yonumen.top

PHP:  parent::greet();
来源：http://mqz.pengpengdd.cyou

JS:   super.greet();
来源：http://kxz.xylfe.cn

TS:   super.greet();
来源：http://xlj.daria6918.cn

Java: super.greet();
来源：http://vot.cashguo.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ywf.yuanzhike.top

Ruby: super
来源：http://qwk.yj20258888.top

C#:   base.Greet();
来源：http://pyg.sysykeji.top

[G08] 静态方法与属性
来源：http://rkn.zdbjq.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zhv.yvedp.cn

PHP:  public static function f() {}
来源：http://jfx.chenjidiqi.icu

JS:   static f() {}
来源：http://obt.meibo888.top

TS:   static f(): void {}
来源：http://swu.andypj.xyz

Java: static void f() {}
来源：http://bqs.wangdashe.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://fjf.shanyushiyangtech.top

Ruby: def self.f; end
来源：http://cst.ydjk.org.cn

C#:   public static void F() {}
来源：http://qih.vehdjk.com

[G09] 接口 / 抽象类
来源：http://ztv.vehdjk.com

Py:   from abc import ABC, abstractmethod
来源：http://soe.shzxlz.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nds.svipenyu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rzs.jlsjyb.cn

TS:   interface Shape { area(): number; }
来源：http://dzt.wangshuangyany.cn

Java: interface Shape { double area(); }
来源：http://hjf.jqgufenzy.top

Go:   type Shape interface { Area() float64 }
来源：http://rdn.vqdsnc.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://szh.ydzc1.top

C#:   interface IShape { double Area(); }
来源：http://hth.tarul.cn

[G10] 访问控制
来源：http://zob.xuetiantiany.cn

Py:   约定 _protected / __private（不强制）
来源：http://mfi.wangdashe.top

PHP:  public / protected / private
来源：http://djz.zycfv.cn

JS:   #private 字段；其余公开
来源：http://lpc.yuxming.cn

TS:   public / protected / private
来源：http://zqy.fzhhl.top

Java: public / protected / private / 默认包级
来源：http://uaf.zhoulong.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://iys.fengsongda.top

Ruby: public / protected / private
来源：http://mkp.0kj1m.cn

C#:   public / protected / private / internal
来源：http://fne.guowangkeji.top

[G11] getter / setter
来源：http://ign.dashuyun.cn

Py:   @property 与 @x.setter
来源：http://tnu.yj202588.top

PHP:  public function getName(): string { return $this->name; }
来源：http://irq.jlsjyb.cn

JS:   get name() { return this._name; }
来源：http://gyf.cucudq.cn

TS:   get name(): string { return this._name; }
来源：http://pko.zhaomingkeji.xyz

Java: public String getName() { return name; }
来源：http://epj.zhoulong.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://fnq.aizwys.cn

Ruby: attr_accessor :name
来源：http://fqy.yfazqb.com

C#:   public string Name { get; set; }
来源：http://kgy.cheryme.top

[G12] 对象转字符串
来源：http://awr.fanxiaobao.xyz

Py:   def __str__(self): return self.name
来源：http://upx.vqdsnc.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://cqa.zdqjudy.top

JS:   toString() { return this.name; }
来源：http://fiq.daxiang520.top

TS:   toString(): string { return this.name; }
来源：http://cwp.shanyushiyangkeji.top

Java: @Override public String toString() { return name; }
来源：http://rsc.ydjk.org.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cbh.smart0.xyz

Ruby: def to_s; @name; end
来源：http://bfc.jinqigfzy.top

C#:   public override string ToString() => Name;
来源：http://eec.gaohongyu789.top

[G13] 判断对象类型
来源：http://whi.shangyingyoupin.top

Py:   isinstance(u, User)
来源：http://pnn.xylfe.cn

PHP:  $u instanceof User
来源：http://rbe.sjlbkw.cn

JS:   u instanceof User
来源：http://ooq.yanxiufei.cn

TS:   u instanceof User
来源：http://vwo.hnqzz.top

Java: u instanceof User
来源：http://yhz.zhongyouzk.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://tjs.cqqwz.cn

Ruby: u.is_a?(User)
来源：http://frz.cqqwz.cn

C#:   u is User
来源：http://vst.yuanzhike.top

[G14] 数据类 / record
来源：http://qmt.sweek.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jsb.shanyushiyangkeji.top

PHP:  // 用 readonly 属性模拟
来源：http://twf.yongpay.top

JS:   // 无内置：普通类或对象字面量
来源：http://xcl.dianchejie.cn

TS:   type User = { name: string; age: number };
来源：http://gee.yueranfly.top

Java: record User(String name, int age) {}
来源：http://tkh.fehbvm.com

Go:   type User struct { Name string; Age int }
来源：http://sso.zhiwuduotai.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tld.jinghuilouyu.cn

C#:   record User(string Name, int Age);
来源：http://anj.sxryk.cn

[G15] 枚举
来源：http://dmi.ivvv.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kst.shuidangran.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ved.yuanzhike.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tiq.pycfn.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pma.jinqigfzy.top

Java: enum Color { RED, GREEN }
来源：http://loi.yueranfly.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hpv.hysaishi.cn

Ruby: Color = %i[red green].freeze
来源：http://vsq.ydjk.org.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rpd.ybcxt.top

[G16] 对象转数组 / 字典
来源：http://dxs.fengsongda.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mfq.tian-w.cn

PHP:  get_object_vars($obj);
来源：http://nxm.shanyushiyangkeji.top

JS:   Object.entries(obj)
来源：http://heu.epnwcf.com

TS:   Object.entries(obj)
来源：http://ryf.feifeiyinyue.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://poh.xylfe.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hxr.fanxiaobao.xyz

Ruby: obj.instance_variables
来源：http://rju.aibaodan.cn

C#:   // 用反射或 System.Text.Json
来源：http://lgx.zdbjq.cn

================================================================================
来源：http://tgb.zhixingplan.top

H. 异常与错误处理
来源：http://xrr.iojbl.cn

================================================================================
来源：http://ktf.uphjek.com

[H01] try / catch 基础
来源：http://nbw.shangyingyoupin.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jyx.zhoulong.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vzv.hesvh.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://aoi.haohaochexian.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ixr.dianchejie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nmd.wangdashe.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://deu.andypj.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ctb.cheryme.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xej.xziqi.cn

[H02] finally / ensure 收尾
来源：http://ciy.ivvv.top

Py:   try: f()⏎finally: cleanup()
来源：http://ucu.shuidangran.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://nmw.aibaodan.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hux.yonumen.top

TS:   try { f(); } finally { cleanup(); }
来源：http://pki.pengpengdd.cyou

Java: try { f(); } finally { cleanup(); }
来源：http://tev.ppjwa.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jbe.xziqi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://iwm.jinyuanbaomall.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pah.gzhubu.top

[H03] 主动抛出异常
来源：http://kfr.jinyuanbaomall.cn

Py:   raise ValueError("错误信息")
来源：http://uya.ydzc1.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ilv.ydjk.org.cn

JS:   throw new Error("错误信息");
来源：http://qnw.hongshengwenyu.top

TS:   throw new Error("错误信息");
来源：http://ycg.ehwqpu.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://xpj.jinghuilouyu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://prv.jinghuilouyu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://frn.cucudq.cn

C#:   throw new ArgumentException("错误信息");
来源：http://cqg.zhoulong.xyz

[H04] 自定义异常类型
来源：http://ejn.ppjwa.cn

Py:   class MyError(Exception): pass
来源：http://axj.cdnleiting.top

PHP:  class MyError extends RuntimeException {}
来源：http://nog.zhixingplan.top

JS:   class MyError extends Error {}
来源：http://boe.ydjk.org.cn

TS:   class MyError extends Error {}
来源：http://icx.jqgufenzy.top

Java: class MyException extends RuntimeException {}
来源：http://rux.sysykeji.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ffq.sufxvd.cn


<!-- 参考信息 -->