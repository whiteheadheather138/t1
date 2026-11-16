代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yhe.fengsongda.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dhs.ywan-chungtsiang.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zle.hesvh.cn

Ruby: s.bytesize;  s.length
来源：http://ega.xingfuxueyuan.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hpd.kuanghao11.cn

================================================================================
来源：http://gdn.jinghuilouyu.cn

F. 文件与目录
来源：http://tze.9152youxi.cn

================================================================================
来源：http://xrp.yuxming.cn

[F01] 读取整个文件
来源：http://yza.zhongyouzk.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vag.sysykeji.top

PHP:  file_get_contents("a.txt");
来源：http://kkh.feifeiyinyue.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://btj.yueranfly.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ppn.aizwys.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gkm.quarkkingdee.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nhd.epnwcf.com

Ruby: File.read("a.txt")
来源：http://ocf.shanyushiyangkeji.top

C#:   File.ReadAllText("a.txt");
来源：http://zdc.wangdashe.top

[F02] 逐行读取文件
来源：http://fgg.shuidangran.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qji.jqgufenzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ebk.redwolf501.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gdf.hongshengwenyu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eud.jqgfzy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://evv.zdqjudy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kdf.aizwys.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qhh.vehdjk.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bzn.aibaodan.cn

[F03] 写入文件（覆盖）
来源：http://hzd.0kj1m.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sol.hnxiangtu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://dre.daria6918.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://svl.wangshuangyany.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lkh.sxryk.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sqx.xuetiantiany.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zlr.fanxiaobao.xyz

Ruby: File.write("a.txt", "hi")
来源：http://zqv.smart0.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tda.ctjpmb.com

[F04] 追加写入文件
来源：http://khr.chenzaomai.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ohb.yonumen.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://aur.meibo888.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://szl.316326.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vfd.0kj1m.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ear.hcnkem.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wlp.iojbl.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://oou.zhoulong.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vgz.sufxvd.cn

[F05] 判断文件或目录是否存在
来源：http://dyu.hesvh.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wzo.ywan-chungtsiang.top

PHP:  file_exists("a.txt");
来源：http://ass.jqgfzy.top

JS:   fs.existsSync("a.txt")
来源：http://wkk.nanxinkj.top

TS:   fs.existsSync("a.txt")
来源：http://bjy.chenlongwang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://nbm.sweek.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://imw.sweek.top

Ruby: File.exist?("a.txt")
来源：http://mjh.xuanzx.com

C#:   File.Exists("a.txt")
来源：http://err.ywan-chungtsiang.top

[F06] 删除文件
来源：http://cib.zhongyouzk.top

Py:   os.remove("a.txt")
来源：http://izf.yueranfly.top

PHP:  unlink("a.txt");
来源：http://sjn.jinqigufen.top

JS:   fs.unlinkSync("a.txt")
来源：http://wdj.yonumen.top

TS:   fs.unlinkSync("a.txt")
来源：http://hwd.316326.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://udh.fengsongda.top

Go:   os.Remove("a.txt")
来源：http://ids.tianlin.xyz

Ruby: File.delete("a.txt")
来源：http://wje.nanxuanxn.top

C#:   File.Delete("a.txt");
来源：http://vkg.tian-w.cn

[F07] 创建目录（含多级）
来源：http://coj.ivvv.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://scc.redwolf501.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mvb.ybcxt.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hxr.ydjk.org.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pgk.jinqigufen.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uij.bbcook.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mpi.zhiwuduotai.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lti.cqqwz.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kqn.zhengqikj.top

[F08] 遍历目录
来源：http://rhs.shuidangran.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://twy.tarul.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jyn.c1oappe.top

JS:   fs.readdirSync("dir")
来源：http://thb.hammf.cn

TS:   fs.readdirSync("dir")
来源：http://vdj.andypj.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tvh.yj20258888.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://snp.xuetiantiany.cn

Ruby: Dir.children("dir")
来源：http://bxa.wangshuangyany.cn

C#:   Directory.GetFiles("dir")
来源：http://gvx.wangdashe.top

[F09] 获取文件大小
来源：http://zxx.zhixingplan.top

Py:   os.path.getsize("a.txt")
来源：http://grh.c1oappe.top

PHP:  filesize("a.txt");
来源：http://kth.aibaodan.cn

JS:   fs.statSync("a.txt").size
来源：http://tnd.yangfankeji.com

TS:   fs.statSync("a.txt").size
来源：http://ihc.yfazqb.com

Java: Files.size(Path.of("a.txt"))
来源：http://kmy.jinyuanbaomall.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://max.yonumen.top

Ruby: File.size("a.txt")
来源：http://wxd.tanke756.top

C#:   new FileInfo("a.txt").Length
来源：http://xtv.yfazqb.com

[F10] 取文件扩展名 / 文件名
来源：http://bop.sysykeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hjr.jyoumei.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hwd.jinqigufen.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tds.ydjk.org.cn

TS:   path.extname("a.txt")
来源：http://thm.mhx1999.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://chy.ivvv.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jmd.jinghuilouyu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yki.0kj1m.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yrc.cucudq.cn

[F11] 复制与移动文件
来源：http://iio.0kj1m.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zay.52xcode.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yjy.shangyingyoupin.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://psz.cqqwz.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rhj.sjlbkw.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ksv.guannengcc.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://igy.cucudq.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sik.shanyushiyangtech.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pty.dianchejie.cn

[F12] CSV 读写
来源：http://bnq.316326.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ukx.yanxiufei.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zcq.jiagoushi.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://keb.zhijiandao.cn

TS:   // 同上
来源：http://yhv.gzhubu.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yzb.jinqigfzy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oxc.xuetiantiany.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://crc.yanxiufei.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kjd.gotoacloud.top

================================================================================
来源：http://lpq.aibaodan.cn

G. 面向对象
来源：http://nrr.jinqigfzy.top

================================================================================
来源：http://abi.xinyue.icu

[G01] 定义类
来源：http://ial.sweek.top

Py:   class User: pass
来源：http://xvd.shanyushiyangkeji.top

PHP:  class User {}
来源：http://wdo.tian-w.cn

JS:   class User {}
来源：http://ths.wangshuangyany.cn

TS:   class User { name: string = ""; }
来源：http://msx.tanke756.top

Java: class User {}
来源：http://kaw.haohaochexian.top

Go:   type User struct { Name string }
来源：http://uuk.andypj.xyz

Ruby: class User; end
来源：http://wnk.hcnkem.com

C#:   class User {}
来源：http://eta.cheryme.top

[G02] 构造函数
来源：http://xqj.quarkkingdee.top

Py:   def __init__(self, name): self.name = name
来源：http://kqg.yonumen.top

PHP:  public function __construct(public string $name) {}
来源：http://dny.jinqigfzy.top

JS:   constructor(name) { this.name = name; }
来源：http://sus.zycfv.cn

TS:   constructor(public name: string) {}
来源：http://bho.redwolf501.top

Java: User(String name) { this.name = name; }
来源：http://qhc.0kj1m.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zka.cheryme.top

Ruby: def initialize(name); @name = name; end
来源：http://pig.andypj.xyz

C#:   public User(string name) { Name = name; }
来源：http://rrq.xingfuxueyuan.xyz

[G03] 实例属性
来源：http://pxw.sweek.top

Py:   self.name = "x"
来源：http://nqs.wangdashe.top

PHP:  public string $name = "x";
来源：http://hfo.cdnleiting.top

JS:   this.name = "x";
来源：http://lsp.andypj.xyz

TS:   name: string = "x";
来源：http://vnl.yj20258888.top

Java: private String name;
来源：http://eos.sjlbkw.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pzo.cdnleiting.top

Ruby: @name = "x"
来源：http://pwk.jinghuilouyu.cn

C#:   public string Name { get; set; } = "x";
来源：http://lng.chenzaomai.com

[G04] 定义方法
来源：http://crs.wangdashe.top

Py:   def greet(self): return self.name
来源：http://swr.nanxuanxn.top

PHP:  public function greet(): string { return $this->name; }
来源：http://nyb.hcnkem.com

JS:   greet() { return this.name; }
来源：http://ipl.vehdjk.com

TS:   greet(): string { return this.name; }
来源：http://tqq.quarkkingdee.top

Java: String greet() { return name; }
来源：http://xed.hammf.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nhs.meibo888.top

Ruby: def greet; @name; end
来源：http://oby.sxryk.cn

C#:   public string Greet() => Name;
来源：http://jpq.xinyue.icu

[G05] 继承
来源：http://fbu.aibaodan.cn

Py:   class Admin(User): pass
来源：http://rrp.andypj.xyz

PHP:  class Admin extends User {}
来源：http://yih.mhx1999.top

JS:   class Admin extends User {}
来源：http://ubf.dianchejie.cn

TS:   class Admin extends User {}
来源：http://bgv.xuetiantiany.cn

Java: class Admin extends User {}
来源：http://eui.bjfxy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://aqw.cqqwz.cn

Ruby: class Admin < User; end
来源：http://fjk.cashguo.top

C#:   class Admin : User {}
来源：http://rad.jqgfzy.top

[G06] 重写方法
来源：http://hai.sysykeji.top

Py:   def greet(self): return "admin"
来源：http://wnu.haohaochexian.top

PHP:  public function greet(): string { return "admin"; }
来源：http://pco.quarkkingdee.top

JS:   greet() { return "admin"; }
来源：http://twe.dashuyun.cn

TS:   greet(): string { return "admin"; }
来源：http://rfb.zycfv.cn

Java: @Override String greet() { return "admin"; }
来源：http://qjx.guowangkeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wxu.c1oappe.top

Ruby: def greet; "admin"; end
来源：http://yaq.birdmap.top

C#:   public override string Greet() => "admin";
来源：http://ohu.redwolf501.top

[G07] 调用父类方法
来源：http://xrq.c1oappe.top

Py:   super().greet()
来源：http://eal.dianchejie.cn

PHP:  parent::greet();
来源：http://ctm.wangshuangyany.cn

JS:   super.greet();
来源：http://txl.ehwqpu.com

TS:   super.greet();
来源：http://yyt.jyoumei.cn

Java: super.greet();
来源：http://lnf.fzhhl.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ixj.iojbl.cn

Ruby: super
来源：http://goj.havefunace.top

C#:   base.Greet();
来源：http://zfj.vqdsnc.cn

[G08] 静态方法与属性
来源：http://oru.tianlin.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jwh.cqqwz.cn

PHP:  public static function f() {}
来源：http://dib.yj20258.top

JS:   static f() {}
来源：http://tmo.guannengcc.top

TS:   static f(): void {}
来源：http://pro.svipenyu.cn

Java: static void f() {}
来源：http://qcm.jqgfzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://qbf.hongshengwenyu.top

Ruby: def self.f; end
来源：http://wfw.xylfe.cn

C#:   public static void F() {}
来源：http://nuh.yuanzhike.top

[G09] 接口 / 抽象类
来源：http://zwx.smart0.xyz

Py:   from abc import ABC, abstractmethod
来源：http://pok.gaohongyu789.top

PHP:  interface Shape { public function area(): float; }
来源：http://xem.fanxiaobao.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://per.gzhubu.top

TS:   interface Shape { area(): number; }
来源：http://zkb.tanke756.top

Java: interface Shape { double area(); }
来源：http://fqz.guowangkeji.top

Go:   type Shape interface { Area() float64 }
来源：http://bpr.aibaodan.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mpz.yuanzhike.top

C#:   interface IShape { double Area(); }
来源：http://eqa.haohaochexian.top

[G10] 访问控制
来源：http://mls.0kj1m.cn

Py:   约定 _protected / __private（不强制）
来源：http://ahq.cucudq.cn

PHP:  public / protected / private
来源：http://mmu.sufxvd.cn

JS:   #private 字段；其余公开
来源：http://feh.jinqigfzy.top

TS:   public / protected / private
来源：http://shi.wangdashe.top

Java: public / protected / private / 默认包级
来源：http://grw.chenlongwang.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://gdu.svipenyu.cn

Ruby: public / protected / private
来源：http://nxa.zhengqikj.top

C#:   public / protected / private / internal
来源：http://dia.aizwys.cn

[G11] getter / setter
来源：http://ymu.cheryme.top

Py:   @property 与 @x.setter
来源：http://skb.iojbl.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pdi.shanyushiyangkeji.top

JS:   get name() { return this._name; }
来源：http://olf.hcnkem.com

TS:   get name(): string { return this._name; }
来源：http://mzy.zycfv.cn

Java: public String getName() { return name; }
来源：http://izg.ydzc1.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://jyy.chenzaomai.com

Ruby: attr_accessor :name
来源：http://lry.smart0.xyz

C#:   public string Name { get; set; }
来源：http://nkm.redwolf501.top

[G12] 对象转字符串
来源：http://zdc.0kj1m.cn

Py:   def __str__(self): return self.name
来源：http://ykt.yuanzhike.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://jrg.xinyue.icu

JS:   toString() { return this.name; }
来源：http://vac.chenjidiqi.icu

TS:   toString(): string { return this.name; }
来源：http://lsr.zhoulong.xyz

Java: @Override public String toString() { return name; }
来源：http://mkb.ehwqpu.com

Go:   func (u User) String() string { return u.Name }
来源：http://zyr.xylfe.cn

Ruby: def to_s; @name; end
来源：http://aeq.xingfuxueyuan.xyz

C#:   public override string ToString() => Name;
来源：http://wgn.hnxiangtu.top

[G13] 判断对象类型
来源：http://qcv.ehwqpu.com

Py:   isinstance(u, User)
来源：http://kqx.shzxlz.cn

PHP:  $u instanceof User
来源：http://zja.xuetiantiany.cn

JS:   u instanceof User
来源：http://vtk.yanxiufei.cn

TS:   u instanceof User
来源：http://hxn.gogol.net.cn

Java: u instanceof User
来源：http://emp.zycfv.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://oyp.havefunace.top

Ruby: u.is_a?(User)
来源：http://rtf.yanxiufei.cn

C#:   u is User
来源：http://uze.ehwqpu.com

[G14] 数据类 / record
来源：http://gzw.hammf.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ysc.sjlbkw.cn

PHP:  // 用 readonly 属性模拟
来源：http://uby.feifeiyinyue.top

JS:   // 无内置：普通类或对象字面量
来源：http://vpq.zycfv.cn

TS:   type User = { name: string; age: number };
来源：http://xmm.zhengqikj.top

Java: record User(String name, int age) {}
来源：http://lvm.vehdjk.com

Go:   type User struct { Name string; Age int }
来源：http://xxl.aizwys.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rxs.yvedp.cn

C#:   record User(string Name, int Age);
来源：http://vim.hongshengwenyu.top

[G15] 枚举
来源：http://gbd.nanxinkj.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ceo.smart0.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://oyh.ehwqpu.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://coi.dashuyun.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nay.daria6918.cn

Java: enum Color { RED, GREEN }
来源：http://boe.haohaochexian.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zqm.zhiwuduotai.top

Ruby: Color = %i[red green].freeze
来源：http://muv.hywenlv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gmv.dashuyun.cn

[G16] 对象转数组 / 字典
来源：http://mfx.jqgufenzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dxk.fanxiaobao.xyz

PHP:  get_object_vars($obj);
来源：http://gfw.tian-w.cn

JS:   Object.entries(obj)
来源：http://zkk.zhijiandao.cn

TS:   Object.entries(obj)
来源：http://czy.nanxinkj.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lwo.zhaomingkeji.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://olt.hesvh.cn

Ruby: obj.instance_variables
来源：http://hlb.zdqjudy.top

C#:   // 用反射或 System.Text.Json
来源：http://eum.haohaochexian.top

================================================================================
来源：http://hss.hcnkem.com

H. 异常与错误处理
来源：http://ewv.chenjidiqi.icu

================================================================================
来源：http://zff.hongshengwenyu.top

[H01] try / catch 基础
来源：http://kkl.shanyushiyangkeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kgf.yuxming.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cib.fehbvm.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xgk.mhx1999.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://iyi.bbcook.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yet.ehwqpu.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cwi.tianlin.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gpi.jlsjyb.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://piv.shanyushiyangkeji.top

[H02] finally / ensure 收尾
来源：http://yfn.feifeiyinyue.top

Py:   try: f()⏎finally: cleanup()
来源：http://vbz.yongpay.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://rss.nanxuanxn.top

JS:   try { f(); } finally { cleanup(); }
来源：http://hsl.bbcook.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://emc.yj20258888.top

Java: try { f(); } finally { cleanup(); }
来源：http://bmv.quarkkingdee.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://lao.cdnleiting.top

Ruby: begin; f; ensure; cleanup; end
来源：http://txl.snrcjt.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hub.jianghu66.top

[H03] 主动抛出异常
来源：http://fkq.shzxlz.cn

Py:   raise ValueError("错误信息")
来源：http://uaw.ehwqpu.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qlq.hcnkem.com

JS:   throw new Error("错误信息");
来源：http://xwe.aibaodan.cn

TS:   throw new Error("错误信息");
来源：http://svl.shangyingyoupin.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://vkx.smart0.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mcg.cucudq.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://bau.daxiang520.top

C#:   throw new ArgumentException("错误信息");
来源：http://jdp.ehwqpu.com

[H04] 自定义异常类型
来源：http://eqs.tianlin.xyz

Py:   class MyError(Exception): pass
来源：http://ory.ctjpmb.com

PHP:  class MyError extends RuntimeException {}
来源：http://bjk.xuetiantiany.cn

JS:   class MyError extends Error {}
来源：http://lrv.hywenlv.cn

TS:   class MyError extends Error {}
来源：http://rbp.wangshuangyany.cn

Java: class MyException extends RuntimeException {}
来源：http://ijf.ivvv.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ilv.zhongyouzk.top


<!-- 参考信息 -->