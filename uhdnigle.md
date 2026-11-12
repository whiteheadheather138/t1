代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fan.yvedp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://udx.hywenlv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lls.ivvv.top

Ruby: s.bytesize;  s.length
来源：http://eqj.hnxiangtu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zrc.shzxlz.cn

================================================================================
来源：http://drw.iojbl.cn

F. 文件与目录
来源：http://khf.316326.xyz

================================================================================
来源：http://wfh.chenlongwang.top

[F01] 读取整个文件
来源：http://ygo.xinyue.icu

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nrb.vqdsnc.cn

PHP:  file_get_contents("a.txt");
来源：http://bqt.birdmap.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wgr.jlsjyb.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wvp.chenjidiqi.icu

Java: Files.readString(Path.of("a.txt"))
来源：http://hdr.vehdjk.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lpm.shanyushiyangtech.top

Ruby: File.read("a.txt")
来源：http://dbi.nwbrower.top

C#:   File.ReadAllText("a.txt");
来源：http://put.havefunace.top

[F02] 逐行读取文件
来源：http://stj.fehbvm.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tbi.yanxiufei.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rtx.dianchejie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rpp.ydjk.org.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wxe.9152youxi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pdp.wangdashe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jnm.0kj1m.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://czz.gotoacloud.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bfw.epnwcf.com

[F03] 写入文件（覆盖）
来源：http://wqb.bjfxy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rkv.jiagoushi.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://eqm.cheryme.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uad.9152youxi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ceg.cdnleiting.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://umn.xuetiantiany.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vhl.gogol.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://qrz.ydzc1.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zyq.pycfn.com

[F04] 追加写入文件
来源：http://ebz.hammf.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://etl.ybcxt.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ttt.xuanzx.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jti.nanxinkj.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://efg.sufxvd.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cet.jinghuilouyu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hck.xuetiantiany.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qod.feifeiyinyue.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hxg.zhiwuduotai.top

[F05] 判断文件或目录是否存在
来源：http://wnm.ppjwa.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wne.bjfxy.top

PHP:  file_exists("a.txt");
来源：http://zhg.yuxming.cn

JS:   fs.existsSync("a.txt")
来源：http://rbd.chenzaomai.com

TS:   fs.existsSync("a.txt")
来源：http://amq.gogol.net.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zbt.shangyingyoupin.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hku.yuxming.cn

Ruby: File.exist?("a.txt")
来源：http://ayn.zhengqikj.top

C#:   File.Exists("a.txt")
来源：http://ecm.zhiwuduotai.top

[F06] 删除文件
来源：http://kqd.316326.xyz

Py:   os.remove("a.txt")
来源：http://uhf.jyoumei.cn

PHP:  unlink("a.txt");
来源：http://afz.cashguo.top

JS:   fs.unlinkSync("a.txt")
来源：http://nef.pengpengdd.cyou

TS:   fs.unlinkSync("a.txt")
来源：http://krv.jiagoushi.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wee.fktsv.cn

Go:   os.Remove("a.txt")
来源：http://dzt.jianghu66.top

Ruby: File.delete("a.txt")
来源：http://nax.52xcode.cn

C#:   File.Delete("a.txt");
来源：http://wqf.hongshengwenyu.top

[F07] 创建目录（含多级）
来源：http://blx.ehwqpu.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cmd.redwolf501.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hbn.cdnleiting.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hys.bbcook.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yqd.zhongyouzk.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oja.dianchejie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cmd.wangdashe.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://btb.fktsv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lbg.sufxvd.cn

[F08] 遍历目录
来源：http://jkb.shzxlz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rzm.gaohongyu789.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nrq.jqgfzy.top

JS:   fs.readdirSync("dir")
来源：http://ohl.ehwqpu.com

TS:   fs.readdirSync("dir")
来源：http://oxt.tarul.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://adx.wangshuangyany.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://idp.52xcode.cn

Ruby: Dir.children("dir")
来源：http://yzi.ywan-chungtsiang.top

C#:   Directory.GetFiles("dir")
来源：http://arq.zhiwuduotai.top

[F09] 获取文件大小
来源：http://upb.jiagoushi.top

Py:   os.path.getsize("a.txt")
来源：http://vyt.zhijiandao.cn

PHP:  filesize("a.txt");
来源：http://lyq.yj20258.top

JS:   fs.statSync("a.txt").size
来源：http://axu.yuanzhike.top

TS:   fs.statSync("a.txt").size
来源：http://goz.cqqwz.cn

Java: Files.size(Path.of("a.txt"))
来源：http://akk.316326.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jho.tarul.cn

Ruby: File.size("a.txt")
来源：http://oao.ydzc1.top

C#:   new FileInfo("a.txt").Length
来源：http://say.chenjidiqi.icu

[F10] 取文件扩展名 / 文件名
来源：http://pdg.quarkkingdee.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ygi.hysaishi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lod.cdnleiting.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gme.nwbrower.top

TS:   path.extname("a.txt")
来源：http://oig.xuetiantiany.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jlw.ydjk.org.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hut.jqgfzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lpj.fanxiaobao.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xvt.yuanzhike.top

[F11] 复制与移动文件
来源：http://blf.zdbjq.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xtm.chenjidiqi.icu

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://aam.meibo888.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ynr.chenzaomai.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bii.shanyushiyangtech.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xof.chenlongwang.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xel.snrcjt.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hro.zhijiandao.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nbk.zdqjudy.top

[F12] CSV 读写
来源：http://dzw.ywan-chungtsiang.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://inw.c1oappe.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wjf.aizwys.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ofd.hysaishi.cn

TS:   // 同上
来源：http://nrq.aibaodan.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vtk.yj202588.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vgn.fengsongda.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tbc.cashguo.top

C#:   // 无内置：用 CsvHelper 库
来源：http://pzy.c1oappe.top

================================================================================
来源：http://krf.cdnleiting.top

G. 面向对象
来源：http://kpu.316326.xyz

================================================================================
来源：http://ljg.dianchejie.cn

[G01] 定义类
来源：http://qox.guannengcc.top

Py:   class User: pass
来源：http://ffu.wangdashe.top

PHP:  class User {}
来源：http://hel.ydjk.org.cn

JS:   class User {}
来源：http://urt.shanyushiyangkeji.top

TS:   class User { name: string = ""; }
来源：http://swv.andypj.xyz

Java: class User {}
来源：http://pya.epnwcf.com

Go:   type User struct { Name string }
来源：http://afm.bbcook.cn

Ruby: class User; end
来源：http://tfn.chenlongwang.top

C#:   class User {}
来源：http://ioe.daxiang520.top

[G02] 构造函数
来源：http://put.316326.xyz

Py:   def __init__(self, name): self.name = name
来源：http://xyg.ivvv.top

PHP:  public function __construct(public string $name) {}
来源：http://prk.zhengqikj.top

JS:   constructor(name) { this.name = name; }
来源：http://ytg.shanyushiyangkeji.top

TS:   constructor(public name: string) {}
来源：http://wul.andypj.xyz

Java: User(String name) { this.name = name; }
来源：http://les.jiagoushi.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lys.ydzc1.top

Ruby: def initialize(name); @name = name; end
来源：http://mvl.shanyushiyangkeji.top

C#:   public User(string name) { Name = name; }
来源：http://evk.yongpay.top

[G03] 实例属性
来源：http://wbz.sufxvd.cn

Py:   self.name = "x"
来源：http://ykd.fengsongda.top

PHP:  public string $name = "x";
来源：http://qgp.meibo888.top

JS:   this.name = "x";
来源：http://jvw.hysaishi.cn

TS:   name: string = "x";
来源：http://zdn.chenlongwang.top

Java: private String name;
来源：http://hoo.jiagoushi.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hop.birdmap.top

Ruby: @name = "x"
来源：http://vvx.tianlin.xyz

C#:   public string Name { get; set; } = "x";
来源：http://eon.jinghuilouyu.cn

[G04] 定义方法
来源：http://ihy.fktsv.cn

Py:   def greet(self): return self.name
来源：http://uka.shzxlz.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://efn.iojbl.cn

JS:   greet() { return this.name; }
来源：http://sci.sjlbkw.cn

TS:   greet(): string { return this.name; }
来源：http://xcs.jinqigfzy.top

Java: String greet() { return name; }
来源：http://xys.ydzc1.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://jzq.xingfuxueyuan.xyz

Ruby: def greet; @name; end
来源：http://pkd.ctjpmb.com

C#:   public string Greet() => Name;
来源：http://utf.yuxming.cn

[G05] 继承
来源：http://jku.daria6918.cn

Py:   class Admin(User): pass
来源：http://gos.nwbrower.top

PHP:  class Admin extends User {}
来源：http://zuf.52xcode.cn

JS:   class Admin extends User {}
来源：http://djl.feifeiyinyue.top

TS:   class Admin extends User {}
来源：http://dfg.bjfxy.top

Java: class Admin extends User {}
来源：http://epg.fzhhl.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bwj.nanxuanxn.top

Ruby: class Admin < User; end
来源：http://zml.316326.xyz

C#:   class Admin : User {}
来源：http://kle.ybcxt.top

[G06] 重写方法
来源：http://ebf.shanyushiyangtech.top

Py:   def greet(self): return "admin"
来源：http://wdo.0kj1m.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://uwe.xuanzx.com

JS:   greet() { return "admin"; }
来源：http://dxi.nanxuanxn.top

TS:   greet(): string { return "admin"; }
来源：http://xvm.pycfn.com

Java: @Override String greet() { return "admin"; }
来源：http://lhb.ppjwa.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yei.hnxiangtu.top

Ruby: def greet; "admin"; end
来源：http://bol.sysykeji.top

C#:   public override string Greet() => "admin";
来源：http://hhb.jqgfzy.top

[G07] 调用父类方法
来源：http://top.jyoumei.cn

Py:   super().greet()
来源：http://udv.0kj1m.cn

PHP:  parent::greet();
来源：http://mqv.guowangkeji.top

JS:   super.greet();
来源：http://epp.yj20258.top

TS:   super.greet();
来源：http://zlg.cdnleiting.top

Java: super.greet();
来源：http://ltu.zhengqikj.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://snq.cucudq.cn

Ruby: super
来源：http://cws.hcnkem.com

C#:   base.Greet();
来源：http://kro.ybcxt.top

[G08] 静态方法与属性
来源：http://yxd.zhoulong.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rjq.yangfankeji.com

PHP:  public static function f() {}
来源：http://bqy.cashguo.top

JS:   static f() {}
来源：http://bfe.c1oappe.top

TS:   static f(): void {}
来源：http://gwf.aibaodan.cn

Java: static void f() {}
来源：http://zem.chenzaomai.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://ojn.cheryme.top

Ruby: def self.f; end
来源：http://wnz.yangfankeji.com

C#:   public static void F() {}
来源：http://awm.zdqjudy.top

[G09] 接口 / 抽象类
来源：http://tky.chenzaomai.com

Py:   from abc import ABC, abstractmethod
来源：http://pps.nanxuanxn.top

PHP:  interface Shape { public function area(): float; }
来源：http://yce.hfpthk.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://apd.tian-w.cn

TS:   interface Shape { area(): number; }
来源：http://giy.feifeiyinyue.top

Java: interface Shape { double area(); }
来源：http://unm.haohaochexian.top

Go:   type Shape interface { Area() float64 }
来源：http://mes.uphjek.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fis.cheryme.top

C#:   interface IShape { double Area(); }
来源：http://fpt.yanxiufei.cn

[G10] 访问控制
来源：http://qbl.tianlin.xyz

Py:   约定 _protected / __private（不强制）
来源：http://ahg.c1oappe.top

PHP:  public / protected / private
来源：http://rya.dashuyun.cn

JS:   #private 字段；其余公开
来源：http://acu.xziqi.cn

TS:   public / protected / private
来源：http://pjv.xuanzx.com

Java: public / protected / private / 默认包级
来源：http://msw.ywan-chungtsiang.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://abo.zdbjq.cn

Ruby: public / protected / private
来源：http://psp.fktsv.cn

C#:   public / protected / private / internal
来源：http://teq.zhixingplan.top

[G11] getter / setter
来源：http://fgk.jianghu66.top

Py:   @property 与 @x.setter
来源：http://tte.ehwqpu.com

PHP:  public function getName(): string { return $this->name; }
来源：http://scl.sxryk.cn

JS:   get name() { return this._name; }
来源：http://ejh.svipenyu.cn

TS:   get name(): string { return this._name; }
来源：http://vob.fehbvm.com

Java: public String getName() { return name; }
来源：http://cna.jianghu66.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://cxj.yanxiufei.cn

Ruby: attr_accessor :name
来源：http://kzz.fzhhl.top

C#:   public string Name { get; set; }
来源：http://gex.shanyushiyangtech.top

[G12] 对象转字符串
来源：http://emf.wangshuangyany.cn

Py:   def __str__(self): return self.name
来源：http://ojh.daria6918.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lep.epnwcf.com

JS:   toString() { return this.name; }
来源：http://hfj.jianghu66.top

TS:   toString(): string { return this.name; }
来源：http://tbp.zhengqikj.top

Java: @Override public String toString() { return name; }
来源：http://jid.chenzaomai.com

Go:   func (u User) String() string { return u.Name }
来源：http://kck.jinqigufen.top

Ruby: def to_s; @name; end
来源：http://oym.tanke756.top

C#:   public override string ToString() => Name;
来源：http://isr.daria6918.cn

[G13] 判断对象类型
来源：http://xls.sufxvd.cn

Py:   isinstance(u, User)
来源：http://uux.fktsv.cn

PHP:  $u instanceof User
来源：http://slf.xingfuxueyuan.xyz

JS:   u instanceof User
来源：http://ptv.xinyue.icu

TS:   u instanceof User
来源：http://lhl.yanxiufei.cn

Java: u instanceof User
来源：http://dxe.gaohongyu789.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ixm.yvedp.cn

Ruby: u.is_a?(User)
来源：http://ssf.yonumen.top

C#:   u is User
来源：http://stu.smart0.xyz

[G14] 数据类 / record
来源：http://yhq.yueranfly.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://quh.aizwys.cn

PHP:  // 用 readonly 属性模拟
来源：http://fev.gzhubu.top

JS:   // 无内置：普通类或对象字面量
来源：http://lyc.feifeiyinyue.top

TS:   type User = { name: string; age: number };
来源：http://rmf.xingfuxueyuan.xyz

Java: record User(String name, int age) {}
来源：http://zsr.cucudq.cn

Go:   type User struct { Name string; Age int }
来源：http://hsi.jyoumei.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mfs.zycfv.cn

C#:   record User(string Name, int Age);
来源：http://ljd.tanke756.top

[G15] 枚举
来源：http://vnw.hfpthk.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sej.xziqi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zpf.birdmap.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jai.zhongyouzk.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ecc.daria6918.cn

Java: enum Color { RED, GREEN }
来源：http://jat.fengsongda.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qus.yvedp.cn

Ruby: Color = %i[red green].freeze
来源：http://bjq.0kj1m.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://eua.mhx1999.top

[G16] 对象转数组 / 字典
来源：http://cbv.shuidangran.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://olu.zhoulong.xyz

PHP:  get_object_vars($obj);
来源：http://jbn.fengsongda.top

JS:   Object.entries(obj)
来源：http://ynv.daria6918.cn

TS:   Object.entries(obj)
来源：http://tnv.mhx1999.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lkm.yfazqb.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://sia.shangyingyoupin.top

Ruby: obj.instance_variables
来源：http://bqa.havefunace.top

C#:   // 用反射或 System.Text.Json
来源：http://icb.cdnleiting.top

================================================================================
来源：http://gve.uphjek.com

H. 异常与错误处理
来源：http://brd.guowangkeji.top

================================================================================
来源：http://mju.chenzaomai.com

[H01] try / catch 基础
来源：http://qce.svipenyu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kln.nwbrower.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://heq.hongshengwenyu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hlc.hesvh.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ssz.tarul.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bfi.svipenyu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uil.0kj1m.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wwp.fktsv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yrg.316326.xyz

[H02] finally / ensure 收尾
来源：http://sgd.fktsv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://hlx.wangdashe.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vzx.zhijiandao.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gor.ctjpmb.com

TS:   try { f(); } finally { cleanup(); }
来源：http://xjh.xuanzx.com

Java: try { f(); } finally { cleanup(); }
来源：http://ido.9152youxi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ycf.xuanzx.com

Ruby: begin; f; ensure; cleanup; end
来源：http://avj.dashuyun.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wsu.ehwqpu.com

[H03] 主动抛出异常
来源：http://ytp.yvedp.cn

Py:   raise ValueError("错误信息")
来源：http://pva.kuanghao11.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://orv.zhixingplan.top

JS:   throw new Error("错误信息");
来源：http://axs.zhoulong.xyz

TS:   throw new Error("错误信息");
来源：http://mua.zycfv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ebu.sxryk.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://anu.dashuyun.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://rhh.tanke756.top

C#:   throw new ArgumentException("错误信息");
来源：http://mnk.9152youxi.cn

[H04] 自定义异常类型
来源：http://xak.0kj1m.cn

Py:   class MyError(Exception): pass
来源：http://elg.svipenyu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://uft.jlsjyb.cn

JS:   class MyError extends Error {}
来源：http://khv.haohaochexian.top

TS:   class MyError extends Error {}
来源：http://vuz.daxiang520.top

Java: class MyException extends RuntimeException {}
来源：http://nak.sxryk.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rjr.jianghu66.top


<!-- 参考信息 -->