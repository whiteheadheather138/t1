代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pkl.dashuyun.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jib.iojbl.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iix.fzhhl.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rjl.ppjwa.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://idl.hywenlv.cn

Go:   // 按 rune 判断长度后截断
来源：http://zgv.cqqwz.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ccf.meibo888.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zao.mhx1999.top

[E22] 字节长度与字符长度
来源：http://soj.shangyingyoupin.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://stt.cqqwz.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bwj.daxiang520.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qga.tianlin.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cja.shzxlz.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vqs.hysaishi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kca.zhixingplan.top

Ruby: s.bytesize;  s.length
来源：http://lhs.fehbvm.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://evw.tianlin.xyz

================================================================================
来源：http://pkt.zdqjudy.top

F. 文件与目录
来源：http://fnt.cdnleiting.top

================================================================================
来源：http://lsd.svipenyu.cn

[F01] 读取整个文件
来源：http://cka.ppjwa.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rev.epnwcf.com

PHP:  file_get_contents("a.txt");
来源：http://jdq.jiagoushi.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vhh.epnwcf.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dzj.fengsongda.top

Java: Files.readString(Path.of("a.txt"))
来源：http://nng.shzxlz.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lig.fehbvm.com

Ruby: File.read("a.txt")
来源：http://aao.xuetiantiany.cn

C#:   File.ReadAllText("a.txt");
来源：http://ybv.sysykeji.top

[F02] 逐行读取文件
来源：http://cxx.yj202588.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://whj.xuetiantiany.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://iuz.haohaochexian.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vfh.tianlin.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ztz.haohaochexian.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ymo.ppjwa.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kcb.jinyuanbaomall.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zpx.316326.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qex.uphjek.com

[F03] 写入文件（覆盖）
来源：http://vcv.fanxiaobao.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rwo.zdbjq.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zwv.cheryme.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sgu.yj202588.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dji.9152youxi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sqj.gotoacloud.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://swe.daxiang520.top

Ruby: File.write("a.txt", "hi")
来源：http://slk.jinqigfzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zhq.zdbjq.cn

[F04] 追加写入文件
来源：http://lvv.gogol.net.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vxm.zhongyouzk.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ulx.hnqzz.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mzq.zycfv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nsr.zdbjq.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fbz.zhoulong.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gxx.hnxiangtu.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kvf.vqdsnc.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://its.fengsongda.top

[F05] 判断文件或目录是否存在
来源：http://woz.dianchejie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cvz.sxryk.cn

PHP:  file_exists("a.txt");
来源：http://mgq.fanxiaobao.xyz

JS:   fs.existsSync("a.txt")
来源：http://lfl.yfazqb.com

TS:   fs.existsSync("a.txt")
来源：http://fte.cashguo.top

Java: Files.exists(Path.of("a.txt"))
来源：http://xng.52xcode.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qqf.yj202588.top

Ruby: File.exist?("a.txt")
来源：http://mkm.zhaomingkeji.xyz

C#:   File.Exists("a.txt")
来源：http://khb.pengpengdd.cyou

[F06] 删除文件
来源：http://amt.fanxiaobao.xyz

Py:   os.remove("a.txt")
来源：http://azo.tarul.cn

PHP:  unlink("a.txt");
来源：http://law.shanyushiyangkeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://ffd.snrcjt.cn

TS:   fs.unlinkSync("a.txt")
来源：http://izl.hnxiangtu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lwi.feifeiyinyue.top

Go:   os.Remove("a.txt")
来源：http://paq.sweek.top

Ruby: File.delete("a.txt")
来源：http://zfs.hesvh.cn

C#:   File.Delete("a.txt");
来源：http://wdg.chenzaomai.com

[F07] 创建目录（含多级）
来源：http://nwe.fktsv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zgw.yuxming.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://luo.tianlin.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://abl.gotoacloud.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kms.hnxiangtu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dmb.c1oappe.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ats.yfazqb.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zkc.ctjpmb.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ges.meibo888.top

[F08] 遍历目录
来源：http://cwl.jiagoushi.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://wry.zdbjq.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yrv.vqdsnc.cn

JS:   fs.readdirSync("dir")
来源：http://asx.epnwcf.com

TS:   fs.readdirSync("dir")
来源：http://xrb.hnqzz.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ljn.zdqjudy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://tui.shanyushiyangtech.top

Ruby: Dir.children("dir")
来源：http://wyh.ydzc1.top

C#:   Directory.GetFiles("dir")
来源：http://ytb.jyoumei.cn

[F09] 获取文件大小
来源：http://vnn.aizwys.cn

Py:   os.path.getsize("a.txt")
来源：http://onp.snrcjt.cn

PHP:  filesize("a.txt");
来源：http://jyz.fanxiaobao.xyz

JS:   fs.statSync("a.txt").size
来源：http://tms.sweek.top

TS:   fs.statSync("a.txt").size
来源：http://hob.jinyuanbaomall.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rhb.fengsongda.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gvc.xylfe.cn

Ruby: File.size("a.txt")
来源：http://cws.316326.xyz

C#:   new FileInfo("a.txt").Length
来源：http://srd.yongpay.top

[F10] 取文件扩展名 / 文件名
来源：http://tgm.meibo888.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mlc.sufxvd.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qvz.wangdashe.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mhq.cqqwz.cn

TS:   path.extname("a.txt")
来源：http://ktm.guannengcc.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://npm.jiagoushi.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dil.zhaomingkeji.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sou.shangyingyoupin.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jlk.cashguo.top

[F11] 复制与移动文件
来源：http://hbx.meibo888.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://has.hywenlv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bbj.ctjpmb.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vmn.xingfuxueyuan.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://juy.jyoumei.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yxm.hfpthk.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hre.jqgufenzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hmm.sufxvd.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://few.tian-w.cn

[F12] CSV 读写
来源：http://cuz.pengpengdd.cyou

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wlv.sjlbkw.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mud.vqdsnc.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pvk.hnqzz.top

TS:   // 同上
来源：http://sxa.tanke756.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mtf.hywenlv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bky.jinqigfzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://buq.jqgufenzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://vau.zhoulong.xyz

================================================================================
来源：http://byn.jinqigufen.top

G. 面向对象
来源：http://jfh.haohaochexian.top

================================================================================
来源：http://oap.fktsv.cn

[G01] 定义类
来源：http://rdr.zhixingplan.top

Py:   class User: pass
来源：http://hbz.sjlbkw.cn

PHP:  class User {}
来源：http://nup.snrcjt.cn

JS:   class User {}
来源：http://jhn.birdmap.top

TS:   class User { name: string = ""; }
来源：http://gun.c1oappe.top

Java: class User {}
来源：http://nom.pengpengdd.cyou

Go:   type User struct { Name string }
来源：http://hiv.hnqzz.top

Ruby: class User; end
来源：http://xuu.shangyingyoupin.top

C#:   class User {}
来源：http://bnj.zhongyouzk.top

[G02] 构造函数
来源：http://boj.zycfv.cn

Py:   def __init__(self, name): self.name = name
来源：http://tgr.zycfv.cn

PHP:  public function __construct(public string $name) {}
来源：http://ozg.cheryme.top

JS:   constructor(name) { this.name = name; }
来源：http://ovk.nanxuanxn.top

TS:   constructor(public name: string) {}
来源：http://kle.fengsongda.top

Java: User(String name) { this.name = name; }
来源：http://ekr.hcnkem.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://iva.ydzc1.top

Ruby: def initialize(name); @name = name; end
来源：http://pot.haohaochexian.top

C#:   public User(string name) { Name = name; }
来源：http://wjh.cashguo.top

[G03] 实例属性
来源：http://pdo.ehwqpu.com

Py:   self.name = "x"
来源：http://blf.nanxinkj.top

PHP:  public string $name = "x";
来源：http://kyo.tianlin.xyz

JS:   this.name = "x";
来源：http://dcn.vqdsnc.cn

TS:   name: string = "x";
来源：http://iob.shanyushiyangtech.top

Java: private String name;
来源：http://lhz.pengpengdd.cyou

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ccw.zycfv.cn

Ruby: @name = "x"
来源：http://gkp.tian-w.cn

C#:   public string Name { get; set; } = "x";
来源：http://jbn.ywan-chungtsiang.top

[G04] 定义方法
来源：http://qnj.zhixingplan.top

Py:   def greet(self): return self.name
来源：http://htl.zdbjq.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://rys.tanke756.top

JS:   greet() { return this.name; }
来源：http://xmv.nwbrower.top

TS:   greet(): string { return this.name; }
来源：http://qji.yj20258.top

Java: String greet() { return name; }
来源：http://fcj.52xcode.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://izb.tian-w.cn

Ruby: def greet; @name; end
来源：http://zfi.pycfn.com

C#:   public string Greet() => Name;
来源：http://get.shuidangran.top

[G05] 继承
来源：http://qrx.yuxming.cn

Py:   class Admin(User): pass
来源：http://ojz.jianghu66.top

PHP:  class Admin extends User {}
来源：http://fer.bjfxy.top

JS:   class Admin extends User {}
来源：http://zqw.birdmap.top

TS:   class Admin extends User {}
来源：http://ili.dianchejie.cn

Java: class Admin extends User {}
来源：http://tic.vehdjk.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ucu.fzhhl.top

Ruby: class Admin < User; end
来源：http://uzi.quarkkingdee.top

C#:   class Admin : User {}
来源：http://igj.gzhubu.top

[G06] 重写方法
来源：http://zqz.hcnkem.com

Py:   def greet(self): return "admin"
来源：http://rsl.yuxming.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rlj.zhengqikj.top

JS:   greet() { return "admin"; }
来源：http://cmx.fzhhl.top

TS:   greet(): string { return "admin"; }
来源：http://oid.jiagoushi.top

Java: @Override String greet() { return "admin"; }
来源：http://dxe.jinqigufen.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mio.yj20258.top

Ruby: def greet; "admin"; end
来源：http://hdq.dashuyun.cn

C#:   public override string Greet() => "admin";
来源：http://oep.0kj1m.cn

[G07] 调用父类方法
来源：http://nvz.zhengqikj.top

Py:   super().greet()
来源：http://udj.jinqigufen.top

PHP:  parent::greet();
来源：http://syk.kuanghao11.cn

JS:   super.greet();
来源：http://aoi.zdqjudy.top

TS:   super.greet();
来源：http://xjn.smart0.xyz

Java: super.greet();
来源：http://dmn.dashuyun.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nff.meibo888.top

Ruby: super
来源：http://bye.jlsjyb.cn

C#:   base.Greet();
来源：http://igk.ivvv.top

[G08] 静态方法与属性
来源：http://fsw.tianlin.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fnf.yanxiufei.cn

PHP:  public static function f() {}
来源：http://pdb.jinghuilouyu.cn

JS:   static f() {}
来源：http://yum.yvedp.cn

TS:   static f(): void {}
来源：http://pjg.zhijiandao.cn

Java: static void f() {}
来源：http://nwh.zhongyouzk.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://slp.daxiang520.top

Ruby: def self.f; end
来源：http://biu.c1oappe.top

C#:   public static void F() {}
来源：http://oni.cqqwz.cn

[G09] 接口 / 抽象类
来源：http://mxt.zycfv.cn

Py:   from abc import ABC, abstractmethod
来源：http://ymw.jiagoushi.top

PHP:  interface Shape { public function area(): float; }
来源：http://nyb.jqgfzy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://kxv.xingfuxueyuan.xyz

TS:   interface Shape { area(): number; }
来源：http://khm.ivvv.top

Java: interface Shape { double area(); }
来源：http://xej.sysykeji.top

Go:   type Shape interface { Area() float64 }
来源：http://ybt.yonumen.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://utb.9152youxi.cn

C#:   interface IShape { double Area(); }
来源：http://wmd.zhaomingkeji.xyz

[G10] 访问控制
来源：http://xzp.fktsv.cn

Py:   约定 _protected / __private（不强制）
来源：http://ofz.ivvv.top

PHP:  public / protected / private
来源：http://jrr.zhaomingkeji.xyz

JS:   #private 字段；其余公开
来源：http://taz.tian-w.cn

TS:   public / protected / private
来源：http://jlc.zhiwuduotai.top

Java: public / protected / private / 默认包级
来源：http://pyj.jqgfzy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://wdx.fzhhl.top

Ruby: public / protected / private
来源：http://vph.zycfv.cn

C#:   public / protected / private / internal
来源：http://zgg.hnqzz.top

[G11] getter / setter
来源：http://sfc.chenzaomai.com

Py:   @property 与 @x.setter
来源：http://sys.ivvv.top

PHP:  public function getName(): string { return $this->name; }
来源：http://gjg.ydjk.org.cn

JS:   get name() { return this._name; }
来源：http://iuq.jinqigfzy.top

TS:   get name(): string { return this._name; }
来源：http://vpu.guannengcc.top

Java: public String getName() { return name; }
来源：http://oxv.quarkkingdee.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://nsw.tanke756.top

Ruby: attr_accessor :name
来源：http://zux.hnqzz.top

C#:   public string Name { get; set; }
来源：http://wfy.redwolf501.top

[G12] 对象转字符串
来源：http://eop.sxryk.cn

Py:   def __str__(self): return self.name
来源：http://tvd.birdmap.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://zkv.zhijiandao.cn

JS:   toString() { return this.name; }
来源：http://fbt.chenzaomai.com

TS:   toString(): string { return this.name; }
来源：http://qdd.xingfuxueyuan.xyz

Java: @Override public String toString() { return name; }
来源：http://gdf.feifeiyinyue.top

Go:   func (u User) String() string { return u.Name }
来源：http://nmy.9152youxi.cn

Ruby: def to_s; @name; end
来源：http://oyc.gzhubu.top

C#:   public override string ToString() => Name;
来源：http://lut.ppjwa.cn

[G13] 判断对象类型
来源：http://hkv.cheryme.top

Py:   isinstance(u, User)
来源：http://coh.gzhubu.top

PHP:  $u instanceof User
来源：http://yxk.guowangkeji.top

JS:   u instanceof User
来源：http://hbi.zhoulong.xyz

TS:   u instanceof User
来源：http://moa.yonumen.top

Java: u instanceof User
来源：http://vhg.zhongyouzk.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://aos.snrcjt.cn

Ruby: u.is_a?(User)
来源：http://nqc.hnqzz.top

C#:   u is User
来源：http://eob.ydjk.org.cn

[G14] 数据类 / record
来源：http://okp.jianghu66.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bnb.bjfxy.top

PHP:  // 用 readonly 属性模拟
来源：http://npk.feifeiyinyue.top

JS:   // 无内置：普通类或对象字面量
来源：http://aho.pycfn.com

TS:   type User = { name: string; age: number };
来源：http://gns.quarkkingdee.top

Java: record User(String name, int age) {}
来源：http://zbi.zhoulong.xyz

Go:   type User struct { Name string; Age int }
来源：http://uza.ivvv.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yyd.vqdsnc.cn

C#:   record User(string Name, int Age);
来源：http://srb.feifeiyinyue.top

[G15] 枚举
来源：http://ate.kuanghao11.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kvn.yj20258888.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://mat.redwolf501.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zbr.shanyushiyangtech.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://loa.zycfv.cn

Java: enum Color { RED, GREEN }
来源：http://baj.gogol.net.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oql.birdmap.top

Ruby: Color = %i[red green].freeze
来源：http://wlg.shuidangran.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://adb.fzhhl.top

[G16] 对象转数组 / 字典
来源：http://kkf.zdbjq.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://god.vehdjk.com

PHP:  get_object_vars($obj);
来源：http://wzz.svipenyu.cn

JS:   Object.entries(obj)
来源：http://pcw.chenlongwang.top

TS:   Object.entries(obj)
来源：http://dmd.ydzc1.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fdu.xinyue.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://vre.hnqzz.top

Ruby: obj.instance_variables
来源：http://vhm.jlsjyb.cn

C#:   // 用反射或 System.Text.Json
来源：http://rvc.fengsongda.top

================================================================================
来源：http://zxu.meibo888.top

H. 异常与错误处理
来源：http://yes.aizwys.cn

================================================================================
来源：http://ati.xinyue.icu

[H01] try / catch 基础
来源：http://vxg.meibo888.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ywj.fehbvm.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yhn.52xcode.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rcn.nwbrower.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dea.pycfn.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lxi.fktsv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dnu.ctjpmb.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dsj.havefunace.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://klf.zhiwuduotai.top

[H02] finally / ensure 收尾
来源：http://hhm.gotoacloud.top

Py:   try: f()⏎finally: cleanup()
来源：http://cbw.fanxiaobao.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://uju.yj20258.top

JS:   try { f(); } finally { cleanup(); }
来源：http://wtx.fengsongda.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ldf.chenjidiqi.icu

Java: try { f(); } finally { cleanup(); }
来源：http://zky.daxiang520.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://lej.yuanzhike.top

Ruby: begin; f; ensure; cleanup; end
来源：http://xxo.daria6918.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://kvc.snrcjt.cn

[H03] 主动抛出异常
来源：http://amc.hcnkem.com

Py:   raise ValueError("错误信息")
来源：http://yvc.yj20258.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jdf.jlsjyb.cn

JS:   throw new Error("错误信息");
来源：http://syh.zdbjq.cn


<!-- 参考信息 -->