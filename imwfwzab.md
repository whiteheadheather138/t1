代发 wailian999

[E22] 字节长度与字符长度
来源：http://mqq.nwbrower.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://plf.zhijiandao.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fhu.xinyue.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sim.jqgfzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fbn.316326.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oky.vehdjk.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dfv.jinqigfzy.top

Ruby: s.bytesize;  s.length
来源：http://fpe.jyoumei.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wrs.zhongyouzk.top

================================================================================
来源：http://klo.guowangkeji.top

F. 文件与目录
来源：http://zhh.chenzaomai.com

================================================================================
来源：http://ivt.ybcxt.top

[F01] 读取整个文件
来源：http://fei.yuxming.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://esq.nanxinkj.top

PHP:  file_get_contents("a.txt");
来源：http://xly.xuetiantiany.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://has.hnxiangtu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gbi.sweek.top

Java: Files.readString(Path.of("a.txt"))
来源：http://pmp.hysaishi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qkr.sxryk.cn

Ruby: File.read("a.txt")
来源：http://skb.fengsongda.top

C#:   File.ReadAllText("a.txt");
来源：http://nwo.hywenlv.cn

[F02] 逐行读取文件
来源：http://oen.birdmap.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vnr.cqqwz.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dmh.cdnleiting.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ywc.zdbjq.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fpn.hnqzz.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pdu.hongshengwenyu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kuf.mhx1999.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ihi.zdbjq.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xbe.cdnleiting.top

[F03] 写入文件（覆盖）
来源：http://wpw.xziqi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ths.hesvh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rbc.sysykeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blz.uphjek.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://itc.sxryk.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://egm.jlsjyb.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://aax.nanxuanxn.top

Ruby: File.write("a.txt", "hi")
来源：http://ngl.jyoumei.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bkb.cdnleiting.top

[F04] 追加写入文件
来源：http://qaf.cucudq.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xta.shanyushiyangkeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wcl.gzhubu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nja.316326.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wxu.aibaodan.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://aox.yfazqb.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mjd.cucudq.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kiz.52xcode.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fdd.xziqi.cn

[F05] 判断文件或目录是否存在
来源：http://wyp.ybcxt.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://faw.uphjek.com

PHP:  file_exists("a.txt");
来源：http://yer.svipenyu.cn

JS:   fs.existsSync("a.txt")
来源：http://tlj.shuidangran.top

TS:   fs.existsSync("a.txt")
来源：http://qfu.cdnleiting.top

Java: Files.exists(Path.of("a.txt"))
来源：http://mjp.zhengqikj.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bnq.vehdjk.com

Ruby: File.exist?("a.txt")
来源：http://zle.hesvh.cn

C#:   File.Exists("a.txt")
来源：http://jnp.ctjpmb.com

[F06] 删除文件
来源：http://cjf.guowangkeji.top

Py:   os.remove("a.txt")
来源：http://fhj.aibaodan.cn

PHP:  unlink("a.txt");
来源：http://dcy.shuidangran.top

JS:   fs.unlinkSync("a.txt")
来源：http://osq.vqdsnc.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gwg.ppjwa.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nbx.jinyuanbaomall.cn

Go:   os.Remove("a.txt")
来源：http://raj.hcnkem.com

Ruby: File.delete("a.txt")
来源：http://fii.zycfv.cn

C#:   File.Delete("a.txt");
来源：http://nul.bbcook.cn

[F07] 创建目录（含多级）
来源：http://fah.cdnleiting.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nyf.cdnleiting.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mdp.iojbl.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eod.vehdjk.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://exf.xziqi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lni.birdmap.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://exe.shangyingyoupin.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rum.iojbl.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ggi.shzxlz.cn

[F08] 遍历目录
来源：http://lvk.tian-w.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bhf.cqqwz.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pgf.fehbvm.com

JS:   fs.readdirSync("dir")
来源：http://dyn.cucudq.cn

TS:   fs.readdirSync("dir")
来源：http://ddd.chenjidiqi.icu

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://spp.tianlin.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://mss.xuetiantiany.cn

Ruby: Dir.children("dir")
来源：http://vlu.hnxiangtu.top

C#:   Directory.GetFiles("dir")
来源：http://kyl.hesvh.cn

[F09] 获取文件大小
来源：http://pab.c1oappe.top

Py:   os.path.getsize("a.txt")
来源：http://pfa.daria6918.cn

PHP:  filesize("a.txt");
来源：http://hjo.hongshengwenyu.top

JS:   fs.statSync("a.txt").size
来源：http://rwz.xziqi.cn

TS:   fs.statSync("a.txt").size
来源：http://xmi.wangshuangyany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ttt.nanxinkj.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://svc.sufxvd.cn

Ruby: File.size("a.txt")
来源：http://vld.zhongyouzk.top

C#:   new FileInfo("a.txt").Length
来源：http://bca.sysykeji.top

[F10] 取文件扩展名 / 文件名
来源：http://ggj.tarul.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hca.meibo888.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tms.ctjpmb.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kli.wangshuangyany.cn

TS:   path.extname("a.txt")
来源：http://jgo.haohaochexian.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lvy.jianghu66.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mkc.yanxiufei.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qsc.meibo888.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zdt.guowangkeji.top

[F11] 复制与移动文件
来源：http://fyp.pycfn.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://iby.daria6918.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lqt.zdqjudy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ndx.jinyuanbaomall.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://afw.havefunace.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ytl.dianchejie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://iun.xziqi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://osf.feifeiyinyue.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nqj.zhijiandao.cn

[F12] CSV 读写
来源：http://ggg.xuanzx.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sqk.zycfv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pwo.jqgfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gnm.52xcode.cn

TS:   // 同上
来源：http://tte.dashuyun.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uym.gogol.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qhc.yfazqb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qhb.tianlin.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://zlr.ydjk.org.cn

================================================================================
来源：http://ysq.wangdashe.top

G. 面向对象
来源：http://spe.nanxuanxn.top

================================================================================
来源：http://ocz.0kj1m.cn

[G01] 定义类
来源：http://jnh.zhongyouzk.top

Py:   class User: pass
来源：http://wrg.cdnleiting.top

PHP:  class User {}
来源：http://kto.redwolf501.top

JS:   class User {}
来源：http://gix.hnxiangtu.top

TS:   class User { name: string = ""; }
来源：http://tkt.cqqwz.cn

Java: class User {}
来源：http://mjs.hywenlv.cn

Go:   type User struct { Name string }
来源：http://ksm.cheryme.top

Ruby: class User; end
来源：http://wgn.ydjk.org.cn

C#:   class User {}
来源：http://qyy.mhx1999.top

[G02] 构造函数
来源：http://www.zhijiandao.cn

Py:   def __init__(self, name): self.name = name
来源：http://nkv.vehdjk.com

PHP:  public function __construct(public string $name) {}
来源：http://jli.wangdashe.top

JS:   constructor(name) { this.name = name; }
来源：http://kwi.ybcxt.top

TS:   constructor(public name: string) {}
来源：http://fux.zdbjq.cn

Java: User(String name) { this.name = name; }
来源：http://wve.quarkkingdee.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zqt.feifeiyinyue.top

Ruby: def initialize(name); @name = name; end
来源：http://pjx.yangfankeji.com

C#:   public User(string name) { Name = name; }
来源：http://ltr.smart0.xyz

[G03] 实例属性
来源：http://hxg.jyoumei.cn

Py:   self.name = "x"
来源：http://cen.xuanzx.com

PHP:  public string $name = "x";
来源：http://wxj.52xcode.cn

JS:   this.name = "x";
来源：http://sfv.jinyuanbaomall.cn

TS:   name: string = "x";
来源：http://cso.shuidangran.top

Java: private String name;
来源：http://kwp.uphjek.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zuq.zycfv.cn

Ruby: @name = "x"
来源：http://gez.quarkkingdee.top

C#:   public string Name { get; set; } = "x";
来源：http://tat.yvedp.cn

[G04] 定义方法
来源：http://hcf.guowangkeji.top

Py:   def greet(self): return self.name
来源：http://pcg.zhaomingkeji.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://ulf.hcnkem.com

JS:   greet() { return this.name; }
来源：http://jrg.ybcxt.top

TS:   greet(): string { return this.name; }
来源：http://aok.nanxuanxn.top

Java: String greet() { return name; }
来源：http://yld.yangfankeji.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://vak.cqqwz.cn

Ruby: def greet; @name; end
来源：http://qsh.xuetiantiany.cn

C#:   public string Greet() => Name;
来源：http://ong.tanke756.top

[G05] 继承
来源：http://sfv.aizwys.cn

Py:   class Admin(User): pass
来源：http://yph.havefunace.top

PHP:  class Admin extends User {}
来源：http://bfe.zdbjq.cn

JS:   class Admin extends User {}
来源：http://ppc.havefunace.top

TS:   class Admin extends User {}
来源：http://pna.chenzaomai.com

Java: class Admin extends User {}
来源：http://syi.cheryme.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hdu.ctjpmb.com

Ruby: class Admin < User; end
来源：http://zlu.0kj1m.cn

C#:   class Admin : User {}
来源：http://hmd.nwbrower.top

[G06] 重写方法
来源：http://dgu.uphjek.com

Py:   def greet(self): return "admin"
来源：http://anc.sufxvd.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bwj.sjlbkw.cn

JS:   greet() { return "admin"; }
来源：http://enx.xuanzx.com

TS:   greet(): string { return "admin"; }
来源：http://qed.pycfn.com

Java: @Override String greet() { return "admin"; }
来源：http://ict.yongpay.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uzw.pengpengdd.cyou

Ruby: def greet; "admin"; end
来源：http://wjo.sjlbkw.cn

C#:   public override string Greet() => "admin";
来源：http://vtq.jiagoushi.top

[G07] 调用父类方法
来源：http://qzz.shanyushiyangkeji.top

Py:   super().greet()
来源：http://hxs.xziqi.cn

PHP:  parent::greet();
来源：http://izw.daria6918.cn

JS:   super.greet();
来源：http://mcj.chenlongwang.top

TS:   super.greet();
来源：http://pra.sweek.top

Java: super.greet();
来源：http://qpz.quarkkingdee.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://iph.tanke756.top

Ruby: super
来源：http://yis.yangfankeji.com

C#:   base.Greet();
来源：http://faq.gotoacloud.top

[G08] 静态方法与属性
来源：http://nbn.epnwcf.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jex.sxryk.cn

PHP:  public static function f() {}
来源：http://hcm.andypj.xyz

JS:   static f() {}
来源：http://jna.shanyushiyangkeji.top

TS:   static f(): void {}
来源：http://pol.dianchejie.cn

Java: static void f() {}
来源：http://xxf.aibaodan.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ygq.52xcode.cn

Ruby: def self.f; end
来源：http://cdb.meibo888.top

C#:   public static void F() {}
来源：http://ftk.cqqwz.cn

[G09] 接口 / 抽象类
来源：http://rup.guowangkeji.top

Py:   from abc import ABC, abstractmethod
来源：http://edi.cucudq.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hwt.fktsv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://onf.hfpthk.cn

TS:   interface Shape { area(): number; }
来源：http://emb.gaohongyu789.top

Java: interface Shape { double area(); }
来源：http://ekg.chenjidiqi.icu

Go:   type Shape interface { Area() float64 }
来源：http://ryl.hysaishi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fhc.fengsongda.top

C#:   interface IShape { double Area(); }
来源：http://ayv.haohaochexian.top

[G10] 访问控制
来源：http://loy.cqqwz.cn

Py:   约定 _protected / __private（不强制）
来源：http://jqu.ctjpmb.com

PHP:  public / protected / private
来源：http://gcf.chenlongwang.top

JS:   #private 字段；其余公开
来源：http://fen.redwolf501.top

TS:   public / protected / private
来源：http://mna.yonumen.top

Java: public / protected / private / 默认包级
来源：http://jqv.hesvh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ajs.vehdjk.com

Ruby: public / protected / private
来源：http://nyn.jqgufenzy.top

C#:   public / protected / private / internal
来源：http://grr.ybcxt.top

[G11] getter / setter
来源：http://ali.aibaodan.cn

Py:   @property 与 @x.setter
来源：http://wpq.zdbjq.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hzb.svipenyu.cn

JS:   get name() { return this._name; }
来源：http://cll.redwolf501.top

TS:   get name(): string { return this._name; }
来源：http://kqp.dashuyun.cn

Java: public String getName() { return name; }
来源：http://vrf.cqqwz.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://lvv.nanxuanxn.top

Ruby: attr_accessor :name
来源：http://pvq.snrcjt.cn

C#:   public string Name { get; set; }
来源：http://aah.ctjpmb.com

[G12] 对象转字符串
来源：http://uiv.jinghuilouyu.cn

Py:   def __str__(self): return self.name
来源：http://wbc.xylfe.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://itc.xinyue.icu

JS:   toString() { return this.name; }
来源：http://kbn.zhiwuduotai.top

TS:   toString(): string { return this.name; }
来源：http://kcj.ppjwa.cn

Java: @Override public String toString() { return name; }
来源：http://qde.hnqzz.top

Go:   func (u User) String() string { return u.Name }
来源：http://lwm.zhoulong.xyz

Ruby: def to_s; @name; end
来源：http://gtz.yuxming.cn

C#:   public override string ToString() => Name;
来源：http://ezc.jinqigufen.top

[G13] 判断对象类型
来源：http://ptb.hfpthk.cn

Py:   isinstance(u, User)
来源：http://ver.xuetiantiany.cn

PHP:  $u instanceof User
来源：http://fpc.shuidangran.top

JS:   u instanceof User
来源：http://url.zhiwuduotai.top

TS:   u instanceof User
来源：http://jwh.hammf.cn

Java: u instanceof User
来源：http://vhn.0kj1m.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://baa.chenjidiqi.icu

Ruby: u.is_a?(User)
来源：http://haw.tarul.cn

C#:   u is User
来源：http://jng.hywenlv.cn

[G14] 数据类 / record
来源：http://kuo.vehdjk.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mme.snrcjt.cn

PHP:  // 用 readonly 属性模拟
来源：http://xzh.ywan-chungtsiang.top

JS:   // 无内置：普通类或对象字面量
来源：http://bbr.wangdashe.top

TS:   type User = { name: string; age: number };
来源：http://kgb.shangyingyoupin.top

Java: record User(String name, int age) {}
来源：http://uvi.zdbjq.cn

Go:   type User struct { Name string; Age int }
来源：http://qoe.yueranfly.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mws.smart0.xyz

C#:   record User(string Name, int Age);
来源：http://eca.jlsjyb.cn

[G15] 枚举
来源：http://hek.hfpthk.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://aql.ybcxt.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://jyt.cheryme.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cvt.xingfuxueyuan.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ilr.snrcjt.cn

Java: enum Color { RED, GREEN }
来源：http://mmd.jqgfzy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ymw.yfazqb.com

Ruby: Color = %i[red green].freeze
来源：http://xka.zycfv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iop.pengpengdd.cyou

[G16] 对象转数组 / 字典
来源：http://okk.hongshengwenyu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ylx.jiagoushi.top

PHP:  get_object_vars($obj);
来源：http://jzt.xuanzx.com

JS:   Object.entries(obj)
来源：http://gwp.9152youxi.cn

TS:   Object.entries(obj)
来源：http://zoy.uphjek.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rrn.nanxinkj.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ado.sjlbkw.cn

Ruby: obj.instance_variables
来源：http://vwp.xuanzx.com

C#:   // 用反射或 System.Text.Json
来源：http://upa.shuidangran.top

================================================================================
来源：http://qpc.nwbrower.top

H. 异常与错误处理
来源：http://tuq.zdqjudy.top

================================================================================
来源：http://xsh.smart0.xyz

[H01] try / catch 基础
来源：http://upw.fengsongda.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uhv.vqdsnc.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bcn.zhixingplan.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ijp.yuxming.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wtr.ivvv.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ped.wangshuangyany.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://krl.iojbl.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jzg.meibo888.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fby.zhoulong.xyz

[H02] finally / ensure 收尾
来源：http://otj.pycfn.com

Py:   try: f()⏎finally: cleanup()
来源：http://iri.nwbrower.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ojo.cdnleiting.top

JS:   try { f(); } finally { cleanup(); }
来源：http://bhc.chenzaomai.com

TS:   try { f(); } finally { cleanup(); }
来源：http://bcy.xuanzx.com

Java: try { f(); } finally { cleanup(); }
来源：http://eyd.hnxiangtu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://rww.uphjek.com

Ruby: begin; f; ensure; cleanup; end
来源：http://uch.pengpengdd.cyou

C#:   try { F(); } finally { Cleanup(); }
来源：http://ojc.fzhhl.top

[H03] 主动抛出异常
来源：http://izz.yj20258.top

Py:   raise ValueError("错误信息")
来源：http://drj.cashguo.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rpn.shangyingyoupin.top

JS:   throw new Error("错误信息");
来源：http://adu.ybcxt.top

TS:   throw new Error("错误信息");
来源：http://xrj.shangyingyoupin.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://wbj.yvedp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yyc.yj202588.top

Ruby: raise ArgumentError, "错误信息"
来源：http://vhk.ppjwa.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rba.guannengcc.top

[H04] 自定义异常类型
来源：http://zlj.zdqjudy.top

Py:   class MyError(Exception): pass
来源：http://bxb.cucudq.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gvi.9152youxi.cn


<!-- 参考信息 -->