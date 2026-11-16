代发 wailian999

[E22] 字节长度与字符长度
来源：http://hir.ppjwa.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lxc.jinghuilouyu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yqs.nanxuanxn.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dwr.snrcjt.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fcm.yueranfly.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uum.fktsv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ypa.ydjk.org.cn

Ruby: s.bytesize;  s.length
来源：http://oak.yvedp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wuz.yj202588.top

================================================================================
来源：http://nxe.fengsongda.top

F. 文件与目录
来源：http://qht.fengsongda.top

================================================================================
来源：http://vek.hesvh.cn

[F01] 读取整个文件
来源：http://ehp.zhiwuduotai.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xiq.ybcxt.top

PHP:  file_get_contents("a.txt");
来源：http://fdu.smart0.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://skp.fzhhl.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pbc.sufxvd.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://wun.yuanzhike.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qfe.tarul.cn

Ruby: File.read("a.txt")
来源：http://wpq.tian-w.cn

C#:   File.ReadAllText("a.txt");
来源：http://dzg.xuetiantiany.cn

[F02] 逐行读取文件
来源：http://klr.xinyue.icu

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://luv.quarkkingdee.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qxy.jqgfzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://otf.vqdsnc.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pin.birdmap.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://efj.ywan-chungtsiang.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://afk.yfazqb.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://slz.ydzc1.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fjr.yanxiufei.cn

[F03] 写入文件（覆盖）
来源：http://vse.zhijiandao.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://muk.fengsongda.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ujz.ctjpmb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nbw.jinyuanbaomall.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aox.tianlin.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://liy.cdnleiting.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pgc.fzhhl.top

Ruby: File.write("a.txt", "hi")
来源：http://dok.aibaodan.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://whh.hnqzz.top

[F04] 追加写入文件
来源：http://ihw.zdbjq.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://iqo.daxiang520.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://oiw.cucudq.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://snx.52xcode.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lbr.xinyue.icu

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kyo.shangyingyoupin.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cyk.daria6918.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nbp.yj202588.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://izb.zdbjq.cn

[F05] 判断文件或目录是否存在
来源：http://vor.dianchejie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yul.chenzaomai.com

PHP:  file_exists("a.txt");
来源：http://chp.havefunace.top

JS:   fs.existsSync("a.txt")
来源：http://pxr.redwolf501.top

TS:   fs.existsSync("a.txt")
来源：http://gir.gzhubu.top

Java: Files.exists(Path.of("a.txt"))
来源：http://rge.chenjidiqi.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://msw.chenzaomai.com

Ruby: File.exist?("a.txt")
来源：http://xrp.jianghu66.top

C#:   File.Exists("a.txt")
来源：http://vgq.kuanghao11.cn

[F06] 删除文件
来源：http://qjd.bbcook.cn

Py:   os.remove("a.txt")
来源：http://xap.yongpay.top

PHP:  unlink("a.txt");
来源：http://pcr.aibaodan.cn

JS:   fs.unlinkSync("a.txt")
来源：http://crt.birdmap.top

TS:   fs.unlinkSync("a.txt")
来源：http://hmb.zhixingplan.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jow.cucudq.cn

Go:   os.Remove("a.txt")
来源：http://osb.shzxlz.cn

Ruby: File.delete("a.txt")
来源：http://kso.chenlongwang.top

C#:   File.Delete("a.txt");
来源：http://jih.dianchejie.cn

[F07] 创建目录（含多级）
来源：http://fwl.yuanzhike.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rak.ivvv.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kle.xziqi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cwa.gogol.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qxu.hnxiangtu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ysv.yonumen.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lrd.zhijiandao.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hsy.9152youxi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vck.0kj1m.cn

[F08] 遍历目录
来源：http://ush.jianghu66.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://vrk.dashuyun.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://run.bjfxy.top

JS:   fs.readdirSync("dir")
来源：http://qzh.tian-w.cn

TS:   fs.readdirSync("dir")
来源：http://lil.hfpthk.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gcu.fktsv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://npb.hammf.cn

Ruby: Dir.children("dir")
来源：http://kmz.ctjpmb.com

C#:   Directory.GetFiles("dir")
来源：http://hwb.cdnleiting.top

[F09] 获取文件大小
来源：http://did.zycfv.cn

Py:   os.path.getsize("a.txt")
来源：http://rqi.sjlbkw.cn

PHP:  filesize("a.txt");
来源：http://kwt.uphjek.com

JS:   fs.statSync("a.txt").size
来源：http://aof.mhx1999.top

TS:   fs.statSync("a.txt").size
来源：http://uai.sxryk.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fhw.shuidangran.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://usr.chenjidiqi.icu

Ruby: File.size("a.txt")
来源：http://yyp.tarul.cn

C#:   new FileInfo("a.txt").Length
来源：http://obg.shanyushiyangtech.top

[F10] 取文件扩展名 / 文件名
来源：http://ufd.chenzaomai.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zss.ivvv.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wwv.nanxuanxn.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ewn.haohaochexian.top

TS:   path.extname("a.txt")
来源：http://csg.shzxlz.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hep.jqgufenzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mjo.sufxvd.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uvc.yongpay.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xmn.ehwqpu.com

[F11] 复制与移动文件
来源：http://brd.wangdashe.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://odi.tianlin.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://slk.uphjek.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aph.ybcxt.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qov.guannengcc.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hyu.shanyushiyangkeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://frl.bjfxy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rno.shzxlz.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cpu.jinghuilouyu.cn

[F12] CSV 读写
来源：http://tau.wangshuangyany.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kns.xziqi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ikn.ydzc1.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qtf.jinyuanbaomall.cn

TS:   // 同上
来源：http://jrh.hywenlv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fra.mhx1999.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://moe.jyoumei.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pyq.yanxiufei.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dzr.chenzaomai.com

================================================================================
来源：http://ect.yuanzhike.top

G. 面向对象
来源：http://fcj.smart0.xyz

================================================================================
来源：http://qxs.sweek.top

[G01] 定义类
来源：http://ziy.ydzc1.top

Py:   class User: pass
来源：http://kqh.nanxuanxn.top

PHP:  class User {}
来源：http://mas.ctjpmb.com

JS:   class User {}
来源：http://yxq.xuetiantiany.cn

TS:   class User { name: string = ""; }
来源：http://beh.yongpay.top

Java: class User {}
来源：http://iwz.jyoumei.cn

Go:   type User struct { Name string }
来源：http://uzu.yfazqb.com

Ruby: class User; end
来源：http://tpu.hywenlv.cn

C#:   class User {}
来源：http://bxl.ywan-chungtsiang.top

[G02] 构造函数
来源：http://qrk.yj20258.top

Py:   def __init__(self, name): self.name = name
来源：http://hsw.dashuyun.cn

PHP:  public function __construct(public string $name) {}
来源：http://cqs.daxiang520.top

JS:   constructor(name) { this.name = name; }
来源：http://ylf.yanxiufei.cn

TS:   constructor(public name: string) {}
来源：http://jyl.gzhubu.top

Java: User(String name) { this.name = name; }
来源：http://jdx.ybcxt.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vwx.jinqigfzy.top

Ruby: def initialize(name); @name = name; end
来源：http://umr.yvedp.cn

C#:   public User(string name) { Name = name; }
来源：http://zne.hnxiangtu.top

[G03] 实例属性
来源：http://pcu.haohaochexian.top

Py:   self.name = "x"
来源：http://szo.hammf.cn

PHP:  public string $name = "x";
来源：http://rvp.nwbrower.top

JS:   this.name = "x";
来源：http://uea.shuidangran.top

TS:   name: string = "x";
来源：http://njq.dianchejie.cn

Java: private String name;
来源：http://fnh.smart0.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://epj.feifeiyinyue.top

Ruby: @name = "x"
来源：http://lln.zhiwuduotai.top

C#:   public string Name { get; set; } = "x";
来源：http://zlj.shzxlz.cn

[G04] 定义方法
来源：http://zmw.jinqigufen.top

Py:   def greet(self): return self.name
来源：http://jsd.chenlongwang.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ngd.gogol.net.cn

JS:   greet() { return this.name; }
来源：http://khh.zhoulong.xyz

TS:   greet(): string { return this.name; }
来源：http://vde.andypj.xyz

Java: String greet() { return name; }
来源：http://pen.mhx1999.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://tkt.nwbrower.top

Ruby: def greet; @name; end
来源：http://vzm.bjfxy.top

C#:   public string Greet() => Name;
来源：http://zgl.daxiang520.top

[G05] 继承
来源：http://xit.zhengqikj.top

Py:   class Admin(User): pass
来源：http://agw.chenzaomai.com

PHP:  class Admin extends User {}
来源：http://yfd.nwbrower.top

JS:   class Admin extends User {}
来源：http://egb.quarkkingdee.top

TS:   class Admin extends User {}
来源：http://mkz.cdnleiting.top

Java: class Admin extends User {}
来源：http://etw.svipenyu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pmx.cucudq.cn

Ruby: class Admin < User; end
来源：http://jhi.yonumen.top

C#:   class Admin : User {}
来源：http://wiw.snrcjt.cn

[G06] 重写方法
来源：http://nio.shuidangran.top

Py:   def greet(self): return "admin"
来源：http://ase.birdmap.top

PHP:  public function greet(): string { return "admin"; }
来源：http://gge.bjfxy.top

JS:   greet() { return "admin"; }
来源：http://tua.iojbl.cn

TS:   greet(): string { return "admin"; }
来源：http://mns.hywenlv.cn

Java: @Override String greet() { return "admin"; }
来源：http://aqc.sweek.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rkd.fktsv.cn

Ruby: def greet; "admin"; end
来源：http://zee.tarul.cn

C#:   public override string Greet() => "admin";
来源：http://uwa.shuidangran.top

[G07] 调用父类方法
来源：http://oav.ydzc1.top

Py:   super().greet()
来源：http://tmf.guannengcc.top

PHP:  parent::greet();
来源：http://tvm.shanyushiyangtech.top

JS:   super.greet();
来源：http://dwb.sxryk.cn

TS:   super.greet();
来源：http://ryw.yangfankeji.com

Java: super.greet();
来源：http://lsh.yuanzhike.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kpe.vehdjk.com

Ruby: super
来源：http://bqk.sweek.top

C#:   base.Greet();
来源：http://bsx.andypj.xyz

[G08] 静态方法与属性
来源：http://crv.meibo888.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zne.aibaodan.cn

PHP:  public static function f() {}
来源：http://hoe.chenlongwang.top

JS:   static f() {}
来源：http://lov.fktsv.cn

TS:   static f(): void {}
来源：http://spw.xziqi.cn

Java: static void f() {}
来源：http://pdu.daria6918.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://stj.zhijiandao.cn

Ruby: def self.f; end
来源：http://fpm.jianghu66.top

C#:   public static void F() {}
来源：http://vgu.yj20258888.top

[G09] 接口 / 抽象类
来源：http://mjf.9152youxi.cn

Py:   from abc import ABC, abstractmethod
来源：http://ryl.hnqzz.top

PHP:  interface Shape { public function area(): float; }
来源：http://fbr.svipenyu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tod.andypj.xyz

TS:   interface Shape { area(): number; }
来源：http://fvb.iojbl.cn

Java: interface Shape { double area(); }
来源：http://qip.sxryk.cn

Go:   type Shape interface { Area() float64 }
来源：http://per.jiagoushi.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vqo.svipenyu.cn

C#:   interface IShape { double Area(); }
来源：http://axm.chenjidiqi.icu

[G10] 访问控制
来源：http://gts.yanxiufei.cn

Py:   约定 _protected / __private（不强制）
来源：http://tri.cheryme.top

PHP:  public / protected / private
来源：http://vfg.shuidangran.top

JS:   #private 字段；其余公开
来源：http://ucq.ydzc1.top

TS:   public / protected / private
来源：http://jvm.jinqigufen.top

Java: public / protected / private / 默认包级
来源：http://jtw.ctjpmb.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://kjp.316326.xyz

Ruby: public / protected / private
来源：http://qhz.yueranfly.top

C#:   public / protected / private / internal
来源：http://fxb.xziqi.cn

[G11] getter / setter
来源：http://hhh.jianghu66.top

Py:   @property 与 @x.setter
来源：http://rly.zycfv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://asw.ctjpmb.com

JS:   get name() { return this._name; }
来源：http://znx.svipenyu.cn

TS:   get name(): string { return this._name; }
来源：http://ygl.ydzc1.top

Java: public String getName() { return name; }
来源：http://ngz.fanxiaobao.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://dzg.guowangkeji.top

Ruby: attr_accessor :name
来源：http://iea.kuanghao11.cn

C#:   public string Name { get; set; }
来源：http://uzz.zhongyouzk.top

[G12] 对象转字符串
来源：http://ntw.fanxiaobao.xyz

Py:   def __str__(self): return self.name
来源：http://mwe.pycfn.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://rcf.fehbvm.com

JS:   toString() { return this.name; }
来源：http://trw.havefunace.top

TS:   toString(): string { return this.name; }
来源：http://twc.snrcjt.cn

Java: @Override public String toString() { return name; }
来源：http://gif.zhixingplan.top

Go:   func (u User) String() string { return u.Name }
来源：http://wua.havefunace.top

Ruby: def to_s; @name; end
来源：http://udk.jinghuilouyu.cn

C#:   public override string ToString() => Name;
来源：http://jtg.cqqwz.cn

[G13] 判断对象类型
来源：http://mwx.sufxvd.cn

Py:   isinstance(u, User)
来源：http://vrc.yonumen.top

PHP:  $u instanceof User
来源：http://epd.xinyue.icu

JS:   u instanceof User
来源：http://gux.havefunace.top

TS:   u instanceof User
来源：http://jup.hnqzz.top

Java: u instanceof User
来源：http://bxx.fengsongda.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://tme.sysykeji.top

Ruby: u.is_a?(User)
来源：http://xvy.bjfxy.top

C#:   u is User
来源：http://ley.jiagoushi.top

[G14] 数据类 / record
来源：http://gbe.xuetiantiany.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pkv.cucudq.cn

PHP:  // 用 readonly 属性模拟
来源：http://bgw.chenzaomai.com

JS:   // 无内置：普通类或对象字面量
来源：http://onh.guowangkeji.top

TS:   type User = { name: string; age: number };
来源：http://cvw.bbcook.cn

Java: record User(String name, int age) {}
来源：http://ate.yj202588.top

Go:   type User struct { Name string; Age int }
来源：http://pxj.sjlbkw.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://chx.dianchejie.cn

C#:   record User(string Name, int Age);
来源：http://uqs.jinqigfzy.top

[G15] 枚举
来源：http://jls.feifeiyinyue.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://eol.fzhhl.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://imo.guowangkeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wbh.ywan-chungtsiang.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mnl.gzhubu.top

Java: enum Color { RED, GREEN }
来源：http://bxj.vqdsnc.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gdc.meibo888.top

Ruby: Color = %i[red green].freeze
来源：http://ljg.316326.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uye.aibaodan.cn

[G16] 对象转数组 / 字典
来源：http://vgk.xingfuxueyuan.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yre.xingfuxueyuan.xyz

PHP:  get_object_vars($obj);
来源：http://lwd.zhixingplan.top

JS:   Object.entries(obj)
来源：http://qhs.gaohongyu789.top

TS:   Object.entries(obj)
来源：http://bwq.jqgufenzy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zxj.yfazqb.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://rnd.xinyue.icu

Ruby: obj.instance_variables
来源：http://wpo.andypj.xyz

C#:   // 用反射或 System.Text.Json
来源：http://ezz.aibaodan.cn

================================================================================
来源：http://sfi.yonumen.top

H. 异常与错误处理
来源：http://tkr.cheryme.top

================================================================================
来源：http://deu.chenlongwang.top

[H01] try / catch 基础
来源：http://sys.ctjpmb.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lpf.hysaishi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qal.vehdjk.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pqr.zhaomingkeji.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mru.xziqi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rgm.yfazqb.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://aei.yj20258888.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uvd.jyoumei.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jsy.havefunace.top

[H02] finally / ensure 收尾
来源：http://rtj.pycfn.com

Py:   try: f()⏎finally: cleanup()
来源：http://haj.yangfankeji.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://jhp.ctjpmb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://pox.yj20258.top

TS:   try { f(); } finally { cleanup(); }
来源：http://kmk.yuanzhike.top

Java: try { f(); } finally { cleanup(); }
来源：http://qwx.gzhubu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://nbu.jlsjyb.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wan.wangshuangyany.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ssf.shzxlz.cn

[H03] 主动抛出异常
来源：http://sen.zhiwuduotai.top

Py:   raise ValueError("错误信息")
来源：http://ewr.jinghuilouyu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xfw.shanyushiyangkeji.top

JS:   throw new Error("错误信息");
来源：http://kjh.kuanghao11.cn

TS:   throw new Error("错误信息");
来源：http://bry.wangshuangyany.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nqd.jyoumei.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rpt.sjlbkw.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://uxm.316326.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://clq.zhijiandao.cn

[H04] 自定义异常类型
来源：http://zdt.epnwcf.com

Py:   class MyError(Exception): pass
来源：http://ldk.bbcook.cn

PHP:  class MyError extends RuntimeException {}
来源：http://arv.zhiwuduotai.top


<!-- 参考信息 -->