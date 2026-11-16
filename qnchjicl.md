代发 wailian999

[F01] 读取整个文件
来源：http://pji.gaohongyu789.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uqn.yuanzhike.top

PHP:  file_get_contents("a.txt");
来源：http://bic.ywan-chungtsiang.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lxc.haohaochexian.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kcf.dashuyun.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mtw.xziqi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wgo.nanxuanxn.top

Ruby: File.read("a.txt")
来源：http://qfi.xinyue.icu

C#:   File.ReadAllText("a.txt");
来源：http://sjq.jiagoushi.top

[F02] 逐行读取文件
来源：http://fft.gzhubu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xqp.zhaomingkeji.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bpa.yj20258.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jjm.jiagoushi.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zmn.kuanghao11.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yxc.daxiang520.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kce.gotoacloud.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xuy.nanxuanxn.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cio.nwbrower.top

[F03] 写入文件（覆盖）
来源：http://wzt.cqqwz.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wsi.jlsjyb.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vdz.hnqzz.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cih.yvedp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qaw.jqgfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zvr.havefunace.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wwi.nwbrower.top

Ruby: File.write("a.txt", "hi")
来源：http://ars.tarul.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bbc.havefunace.top

[F04] 追加写入文件
来源：http://tbb.zycfv.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dex.ppjwa.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://opz.zhijiandao.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lpq.aibaodan.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ppa.jinqigufen.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xvy.guowangkeji.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://okg.ydjk.org.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lip.wangdashe.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fxn.jiagoushi.top

[F05] 判断文件或目录是否存在
来源：http://mxo.xuanzx.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gas.aibaodan.cn

PHP:  file_exists("a.txt");
来源：http://now.kuanghao11.cn

JS:   fs.existsSync("a.txt")
来源：http://sgi.cqqwz.cn

TS:   fs.existsSync("a.txt")
来源：http://gxm.nanxuanxn.top

Java: Files.exists(Path.of("a.txt"))
来源：http://kdx.sufxvd.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ceb.xuetiantiany.cn

Ruby: File.exist?("a.txt")
来源：http://dvi.nwbrower.top

C#:   File.Exists("a.txt")
来源：http://yix.cashguo.top

[F06] 删除文件
来源：http://yok.sweek.top

Py:   os.remove("a.txt")
来源：http://cyz.quarkkingdee.top

PHP:  unlink("a.txt");
来源：http://mdb.cheryme.top

JS:   fs.unlinkSync("a.txt")
来源：http://uut.jqgufenzy.top

TS:   fs.unlinkSync("a.txt")
来源：http://okf.xuanzx.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sdw.jianghu66.top

Go:   os.Remove("a.txt")
来源：http://jwg.zhoulong.xyz

Ruby: File.delete("a.txt")
来源：http://udb.jinqigufen.top

C#:   File.Delete("a.txt");
来源：http://rkb.ydjk.org.cn

[F07] 创建目录（含多级）
来源：http://jro.iojbl.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wil.zhoulong.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tkj.sjlbkw.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://doh.fanxiaobao.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bxh.hammf.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yuf.kuanghao11.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://eni.fehbvm.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xcy.yvedp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rta.redwolf501.top

[F08] 遍历目录
来源：http://tvk.yvedp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qtl.snrcjt.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dqt.sufxvd.cn

JS:   fs.readdirSync("dir")
来源：http://zcj.ywan-chungtsiang.top

TS:   fs.readdirSync("dir")
来源：http://htg.zhengqikj.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vbc.jinqigufen.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://cvb.ehwqpu.com

Ruby: Dir.children("dir")
来源：http://dlt.jinqigufen.top

C#:   Directory.GetFiles("dir")
来源：http://kky.kuanghao11.cn

[F09] 获取文件大小
来源：http://tvz.iojbl.cn

Py:   os.path.getsize("a.txt")
来源：http://xri.xylfe.cn

PHP:  filesize("a.txt");
来源：http://kxt.yuanzhike.top

JS:   fs.statSync("a.txt").size
来源：http://vao.fengsongda.top

TS:   fs.statSync("a.txt").size
来源：http://knt.xylfe.cn

Java: Files.size(Path.of("a.txt"))
来源：http://cey.ydzc1.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tcz.yfazqb.com

Ruby: File.size("a.txt")
来源：http://stb.chenlongwang.top

C#:   new FileInfo("a.txt").Length
来源：http://kzf.jianghu66.top

[F10] 取文件扩展名 / 文件名
来源：http://gnm.hcnkem.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://syt.jinyuanbaomall.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://awc.zhijiandao.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ptn.uphjek.com

TS:   path.extname("a.txt")
来源：http://ldj.mhx1999.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://iys.guannengcc.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hak.jyoumei.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lyl.epnwcf.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sob.hammf.cn

[F11] 复制与移动文件
来源：http://jys.zycfv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hfy.vqdsnc.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lqe.sjlbkw.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rne.yanxiufei.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nfw.uphjek.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://llf.tanke756.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kmx.vqdsnc.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://imh.ydzc1.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://eqp.zhijiandao.cn

[F12] CSV 读写
来源：http://qzx.shuidangran.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gjl.hywenlv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pee.cqqwz.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://aab.jqgfzy.top

TS:   // 同上
来源：http://erg.gaohongyu789.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yyn.jianghu66.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ata.sjlbkw.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cko.yongpay.top

C#:   // 无内置：用 CsvHelper 库
来源：http://uin.xziqi.cn

================================================================================
来源：http://jgn.hesvh.cn

G. 面向对象
来源：http://fec.jqgufenzy.top

================================================================================
来源：http://lve.aizwys.cn

[G01] 定义类
来源：http://tgj.cucudq.cn

Py:   class User: pass
来源：http://dqs.birdmap.top

PHP:  class User {}
来源：http://tfk.birdmap.top

JS:   class User {}
来源：http://dov.52xcode.cn

TS:   class User { name: string = ""; }
来源：http://esv.yangfankeji.com

Java: class User {}
来源：http://qys.zhengqikj.top

Go:   type User struct { Name string }
来源：http://qqg.xziqi.cn

Ruby: class User; end
来源：http://qhs.bjfxy.top

C#:   class User {}
来源：http://efm.haohaochexian.top

[G02] 构造函数
来源：http://mvv.hysaishi.cn

Py:   def __init__(self, name): self.name = name
来源：http://ter.hesvh.cn

PHP:  public function __construct(public string $name) {}
来源：http://hvc.hysaishi.cn

JS:   constructor(name) { this.name = name; }
来源：http://ema.fehbvm.com

TS:   constructor(public name: string) {}
来源：http://mrk.zycfv.cn

Java: User(String name) { this.name = name; }
来源：http://uzz.shanyushiyangtech.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mwp.wangshuangyany.cn

Ruby: def initialize(name); @name = name; end
来源：http://rar.smart0.xyz

C#:   public User(string name) { Name = name; }
来源：http://svj.dianchejie.cn

[G03] 实例属性
来源：http://ugc.zhijiandao.cn

Py:   self.name = "x"
来源：http://dul.aizwys.cn

PHP:  public string $name = "x";
来源：http://zms.hnqzz.top

JS:   this.name = "x";
来源：http://syt.pengpengdd.cyou

TS:   name: string = "x";
来源：http://sse.hammf.cn

Java: private String name;
来源：http://qfe.gotoacloud.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://arx.fehbvm.com

Ruby: @name = "x"
来源：http://nki.daria6918.cn

C#:   public string Name { get; set; } = "x";
来源：http://odr.ydjk.org.cn

[G04] 定义方法
来源：http://rzq.birdmap.top

Py:   def greet(self): return self.name
来源：http://zlz.hesvh.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fmg.hfpthk.cn

JS:   greet() { return this.name; }
来源：http://arp.gaohongyu789.top

TS:   greet(): string { return this.name; }
来源：http://mgf.316326.xyz

Java: String greet() { return name; }
来源：http://zki.zhijiandao.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://umy.jqgfzy.top

Ruby: def greet; @name; end
来源：http://vvk.zhengqikj.top

C#:   public string Greet() => Name;
来源：http://iyi.shanyushiyangkeji.top

[G05] 继承
来源：http://yxz.birdmap.top

Py:   class Admin(User): pass
来源：http://ypg.xylfe.cn

PHP:  class Admin extends User {}
来源：http://twm.dashuyun.cn

JS:   class Admin extends User {}
来源：http://vad.shanyushiyangkeji.top

TS:   class Admin extends User {}
来源：http://ejj.jinqigufen.top

Java: class Admin extends User {}
来源：http://pda.ivvv.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zea.hnqzz.top

Ruby: class Admin < User; end
来源：http://etg.jinqigufen.top

C#:   class Admin : User {}
来源：http://pux.jinqigufen.top

[G06] 重写方法
来源：http://yte.quarkkingdee.top

Py:   def greet(self): return "admin"
来源：http://apd.hywenlv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yue.nanxinkj.top

JS:   greet() { return "admin"; }
来源：http://vrt.yanxiufei.cn

TS:   greet(): string { return "admin"; }
来源：http://uin.jinqigfzy.top

Java: @Override String greet() { return "admin"; }
来源：http://omj.ybcxt.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://njq.ywan-chungtsiang.top

Ruby: def greet; "admin"; end
来源：http://kax.feifeiyinyue.top

C#:   public override string Greet() => "admin";
来源：http://ltn.uphjek.com

[G07] 调用父类方法
来源：http://zio.svipenyu.cn

Py:   super().greet()
来源：http://oom.jqgufenzy.top

PHP:  parent::greet();
来源：http://cjd.cashguo.top

JS:   super.greet();
来源：http://jmx.cucudq.cn

TS:   super.greet();
来源：http://gkw.bjfxy.top

Java: super.greet();
来源：http://ehn.cucudq.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bqc.fktsv.cn

Ruby: super
来源：http://xos.guannengcc.top

C#:   base.Greet();
来源：http://qpr.hesvh.cn

[G08] 静态方法与属性
来源：http://mju.gaohongyu789.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dcn.zhoulong.xyz

PHP:  public static function f() {}
来源：http://faq.svipenyu.cn

JS:   static f() {}
来源：http://xcm.cqqwz.cn

TS:   static f(): void {}
来源：http://xcc.chenzaomai.com

Java: static void f() {}
来源：http://ipe.hywenlv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://gti.jiagoushi.top

Ruby: def self.f; end
来源：http://wdg.zhiwuduotai.top

C#:   public static void F() {}
来源：http://wac.cucudq.cn

[G09] 接口 / 抽象类
来源：http://ziq.tarul.cn

Py:   from abc import ABC, abstractmethod
来源：http://bbb.jinqigfzy.top

PHP:  interface Shape { public function area(): float; }
来源：http://ppl.guannengcc.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://svq.jqgfzy.top

TS:   interface Shape { area(): number; }
来源：http://pmp.9152youxi.cn

Java: interface Shape { double area(); }
来源：http://cis.xinyue.icu

Go:   type Shape interface { Area() float64 }
来源：http://bhn.mhx1999.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tig.hnqzz.top

C#:   interface IShape { double Area(); }
来源：http://ncq.c1oappe.top

[G10] 访问控制
来源：http://ytt.yanxiufei.cn

Py:   约定 _protected / __private（不强制）
来源：http://pik.yvedp.cn

PHP:  public / protected / private
来源：http://lps.sxryk.cn

JS:   #private 字段；其余公开
来源：http://zec.tanke756.top

TS:   public / protected / private
来源：http://uth.hesvh.cn

Java: public / protected / private / 默认包级
来源：http://ynv.zhaomingkeji.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://mpy.sufxvd.cn

Ruby: public / protected / private
来源：http://oxl.zhixingplan.top

C#:   public / protected / private / internal
来源：http://blm.yuanzhike.top

[G11] getter / setter
来源：http://cmh.aizwys.cn

Py:   @property 与 @x.setter
来源：http://iss.ywan-chungtsiang.top

PHP:  public function getName(): string { return $this->name; }
来源：http://eyu.yongpay.top

JS:   get name() { return this._name; }
来源：http://elk.tianlin.xyz

TS:   get name(): string { return this._name; }
来源：http://dct.fengsongda.top

Java: public String getName() { return name; }
来源：http://rvp.guowangkeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://upb.yonumen.top

Ruby: attr_accessor :name
来源：http://juj.gotoacloud.top

C#:   public string Name { get; set; }
来源：http://qiu.xylfe.cn

[G12] 对象转字符串
来源：http://twl.hysaishi.cn

Py:   def __str__(self): return self.name
来源：http://drv.fengsongda.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://gxu.yueranfly.top

JS:   toString() { return this.name; }
来源：http://oad.birdmap.top

TS:   toString(): string { return this.name; }
来源：http://gyb.fengsongda.top

Java: @Override public String toString() { return name; }
来源：http://jrj.cdnleiting.top

Go:   func (u User) String() string { return u.Name }
来源：http://koi.gzhubu.top

Ruby: def to_s; @name; end
来源：http://zhs.gzhubu.top

C#:   public override string ToString() => Name;
来源：http://jha.zhongyouzk.top

[G13] 判断对象类型
来源：http://ihq.hfpthk.cn

Py:   isinstance(u, User)
来源：http://beu.yvedp.cn

PHP:  $u instanceof User
来源：http://uoh.aibaodan.cn

JS:   u instanceof User
来源：http://ymm.fktsv.cn

TS:   u instanceof User
来源：http://wgx.vqdsnc.cn

Java: u instanceof User
来源：http://lct.tianlin.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://ldf.hammf.cn

Ruby: u.is_a?(User)
来源：http://aag.uphjek.com

C#:   u is User
来源：http://lcw.zycfv.cn

[G14] 数据类 / record
来源：http://fjx.mhx1999.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pwj.hongshengwenyu.top

PHP:  // 用 readonly 属性模拟
来源：http://xqx.tianlin.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://aqb.smart0.xyz

TS:   type User = { name: string; age: number };
来源：http://dtu.dianchejie.cn

Java: record User(String name, int age) {}
来源：http://cut.yangfankeji.com

Go:   type User struct { Name string; Age int }
来源：http://djq.birdmap.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://iqp.hfpthk.cn

C#:   record User(string Name, int Age);
来源：http://jib.redwolf501.top

[G15] 枚举
来源：http://bwn.nwbrower.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://okj.fehbvm.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://spg.wangdashe.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://otm.shanyushiyangkeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qnm.dashuyun.cn

Java: enum Color { RED, GREEN }
来源：http://mtq.cucudq.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bqg.tanke756.top

Ruby: Color = %i[red green].freeze
来源：http://bas.shangyingyoupin.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tbl.gogol.net.cn

[G16] 对象转数组 / 字典
来源：http://zap.zhixingplan.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fja.gaohongyu789.top

PHP:  get_object_vars($obj);
来源：http://aax.ydjk.org.cn

JS:   Object.entries(obj)
来源：http://hbh.havefunace.top

TS:   Object.entries(obj)
来源：http://djz.pycfn.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ilo.jianghu66.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://xwt.52xcode.cn

Ruby: obj.instance_variables
来源：http://azb.dashuyun.cn

C#:   // 用反射或 System.Text.Json
来源：http://cjs.cdnleiting.top

================================================================================
来源：http://ddn.iojbl.cn

H. 异常与错误处理
来源：http://nzg.zhijiandao.cn

================================================================================
来源：http://ixy.sxryk.cn

[H01] try / catch 基础
来源：http://apt.nanxuanxn.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cpo.cashguo.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://awk.pengpengdd.cyou

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tfh.redwolf501.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jqu.cashguo.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pdq.tianlin.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qhj.bjfxy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://njp.vehdjk.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://znw.vqdsnc.cn

[H02] finally / ensure 收尾
来源：http://hod.9152youxi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dhb.gogol.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://rxm.sxryk.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://dmm.ppjwa.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lwt.jyoumei.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ghh.sxryk.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://psv.feifeiyinyue.top

Ruby: begin; f; ensure; cleanup; end
来源：http://zgl.bjfxy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ops.316326.xyz

[H03] 主动抛出异常
来源：http://zrg.birdmap.top

Py:   raise ValueError("错误信息")
来源：http://rld.jinqigufen.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://aab.cucudq.cn

JS:   throw new Error("错误信息");
来源：http://waf.feifeiyinyue.top

TS:   throw new Error("错误信息");
来源：http://xrg.ydjk.org.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://afu.hammf.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pns.yj20258888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://mla.chenjidiqi.icu

C#:   throw new ArgumentException("错误信息");
来源：http://jwk.yuanzhike.top

[H04] 自定义异常类型
来源：http://vjr.hysaishi.cn

Py:   class MyError(Exception): pass
来源：http://fbv.meibo888.top

PHP:  class MyError extends RuntimeException {}
来源：http://apw.316326.xyz

JS:   class MyError extends Error {}
来源：http://ipi.sufxvd.cn

TS:   class MyError extends Error {}
来源：http://rgf.hcnkem.com

Java: class MyException extends RuntimeException {}
来源：http://rkx.zycfv.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://idm.xylfe.cn

Ruby: class MyError < StandardError; end
来源：http://ksr.zycfv.cn

C#:   class MyException : Exception {}
来源：http://xne.vqdsnc.cn

[H05] 捕获特定类型
来源：http://vly.birdmap.top

Py:   except ValueError as e:
来源：http://dtd.gaohongyu789.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://eii.tarul.cn

JS:   if (e instanceof TypeError) {}
来源：http://uyd.vehdjk.com

TS:   if (e instanceof TypeError) {}
来源：http://cur.gogol.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://aya.tanke756.top


<!-- 参考信息 -->