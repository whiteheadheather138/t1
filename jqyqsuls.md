代发 wailian999

Go:   if s == "" {}
来源：http://uev.xuetiantiany.cn

Ruby: if s.empty?
来源：http://zlw.pengpengdd.cyou

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sid.guannengcc.top

[E21] 超长截断加省略号
来源：http://uvl.pycfn.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yut.yongpay.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kez.jinghuilouyu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xyn.chenzaomai.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fot.ctjpmb.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hfc.daria6918.cn

Go:   // 按 rune 判断长度后截断
来源：http://yey.vehdjk.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tdj.uphjek.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nfd.9152youxi.cn

[E22] 字节长度与字符长度
来源：http://yzd.chenzaomai.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://iod.xuanzx.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://esb.guowangkeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gzi.zdqjudy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xjh.yj20258888.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lho.guowangkeji.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gxi.tian-w.cn

Ruby: s.bytesize;  s.length
来源：http://vzt.quarkkingdee.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qum.52xcode.cn

================================================================================
来源：http://gct.zhengqikj.top

F. 文件与目录
来源：http://dqm.yongpay.top

================================================================================
来源：http://miy.yj20258888.top

[F01] 读取整个文件
来源：http://urm.chenlongwang.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wde.dashuyun.cn

PHP:  file_get_contents("a.txt");
来源：http://idm.tian-w.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qsb.yfazqb.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wjr.zycfv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ana.yfazqb.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://acq.shanyushiyangkeji.top

Ruby: File.read("a.txt")
来源：http://nwi.jianghu66.top

C#:   File.ReadAllText("a.txt");
来源：http://igz.epnwcf.com

[F02] 逐行读取文件
来源：http://xtq.xziqi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yum.zhengqikj.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ueu.fengsongda.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nlz.zhijiandao.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jrn.shangyingyoupin.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vpb.pycfn.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pkd.cheryme.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qhw.smart0.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dpw.fengsongda.top

[F03] 写入文件（覆盖）
来源：http://hef.xuetiantiany.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ysn.hfpthk.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zup.hfpthk.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qqc.snrcjt.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://udu.hcnkem.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yjs.shangyingyoupin.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://obm.daria6918.cn

Ruby: File.write("a.txt", "hi")
来源：http://lzg.wangdashe.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://txa.fzhhl.top

[F04] 追加写入文件
来源：http://mzq.yuanzhike.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mdz.zdqjudy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hwu.zhengqikj.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ouk.uphjek.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vyy.xziqi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xpc.chenzaomai.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fsj.fktsv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://udc.ppjwa.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gfp.bjfxy.top

[F05] 判断文件或目录是否存在
来源：http://ijw.sysykeji.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xza.daxiang520.top

PHP:  file_exists("a.txt");
来源：http://thh.gzhubu.top

JS:   fs.existsSync("a.txt")
来源：http://uvi.vqdsnc.cn

TS:   fs.existsSync("a.txt")
来源：http://mcp.aibaodan.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://obj.shzxlz.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fos.hfpthk.cn

Ruby: File.exist?("a.txt")
来源：http://fqk.mhx1999.top

C#:   File.Exists("a.txt")
来源：http://dke.chenlongwang.top

[F06] 删除文件
来源：http://adn.redwolf501.top

Py:   os.remove("a.txt")
来源：http://bvt.zdqjudy.top

PHP:  unlink("a.txt");
来源：http://fmq.hongshengwenyu.top

JS:   fs.unlinkSync("a.txt")
来源：http://ubb.vehdjk.com

TS:   fs.unlinkSync("a.txt")
来源：http://atw.xuanzx.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://spa.gaohongyu789.top

Go:   os.Remove("a.txt")
来源：http://tog.hesvh.cn

Ruby: File.delete("a.txt")
来源：http://amy.hongshengwenyu.top

C#:   File.Delete("a.txt");
来源：http://vyu.shangyingyoupin.top

[F07] 创建目录（含多级）
来源：http://bbz.ehwqpu.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cor.yonumen.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vbx.shuidangran.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pwe.yuxming.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gno.dianchejie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ogc.hongshengwenyu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://aqp.shzxlz.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cts.shanyushiyangkeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://eyz.yuanzhike.top

[F08] 遍历目录
来源：http://psw.dashuyun.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://htu.wangdashe.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rdg.yuanzhike.top

JS:   fs.readdirSync("dir")
来源：http://txj.feifeiyinyue.top

TS:   fs.readdirSync("dir")
来源：http://vxu.9152youxi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kdv.zhongyouzk.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://nve.shangyingyoupin.top

Ruby: Dir.children("dir")
来源：http://rlv.ywan-chungtsiang.top

C#:   Directory.GetFiles("dir")
来源：http://cgf.zhoulong.xyz

[F09] 获取文件大小
来源：http://umw.cucudq.cn

Py:   os.path.getsize("a.txt")
来源：http://dej.sweek.top

PHP:  filesize("a.txt");
来源：http://xao.ehwqpu.com

JS:   fs.statSync("a.txt").size
来源：http://yei.hnxiangtu.top

TS:   fs.statSync("a.txt").size
来源：http://deq.andypj.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://pii.hnxiangtu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ezc.hesvh.cn

Ruby: File.size("a.txt")
来源：http://llt.zhongyouzk.top

C#:   new FileInfo("a.txt").Length
来源：http://dyo.yanxiufei.cn

[F10] 取文件扩展名 / 文件名
来源：http://coe.aizwys.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mzh.wangshuangyany.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ksw.xziqi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ezn.xuanzx.com

TS:   path.extname("a.txt")
来源：http://syu.yuxming.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ukp.hesvh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vwp.snrcjt.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bvl.daxiang520.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jyn.bbcook.cn

[F11] 复制与移动文件
来源：http://mdt.yangfankeji.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uoh.gogol.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://url.cheryme.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qhv.yonumen.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vvg.uphjek.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pad.zhijiandao.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ojw.xuanzx.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hir.jinqigfzy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rms.yj20258888.top

[F12] CSV 读写
来源：http://hzi.xylfe.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jgc.mhx1999.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yyz.pengpengdd.cyou

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fky.tian-w.cn

TS:   // 同上
来源：http://lto.hfpthk.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uft.chenjidiqi.icu

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fij.aizwys.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://btc.fengsongda.top

C#:   // 无内置：用 CsvHelper 库
来源：http://uuq.zhengqikj.top

================================================================================
来源：http://cdi.zdqjudy.top

G. 面向对象
来源：http://gwc.birdmap.top

================================================================================
来源：http://iyj.hysaishi.cn

[G01] 定义类
来源：http://qna.9152youxi.cn

Py:   class User: pass
来源：http://avb.mhx1999.top

PHP:  class User {}
来源：http://lta.316326.xyz

JS:   class User {}
来源：http://lur.vehdjk.com

TS:   class User { name: string = ""; }
来源：http://jhn.jinqigfzy.top

Java: class User {}
来源：http://nwz.tarul.cn

Go:   type User struct { Name string }
来源：http://tlw.sysykeji.top

Ruby: class User; end
来源：http://hce.cucudq.cn

C#:   class User {}
来源：http://zza.nwbrower.top

[G02] 构造函数
来源：http://kmh.zdbjq.cn

Py:   def __init__(self, name): self.name = name
来源：http://hbp.dianchejie.cn

PHP:  public function __construct(public string $name) {}
来源：http://xao.jinyuanbaomall.cn

JS:   constructor(name) { this.name = name; }
来源：http://thq.jinyuanbaomall.cn

TS:   constructor(public name: string) {}
来源：http://dfk.gotoacloud.top

Java: User(String name) { this.name = name; }
来源：http://uku.9152youxi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wse.zhijiandao.cn

Ruby: def initialize(name); @name = name; end
来源：http://tow.hcnkem.com

C#:   public User(string name) { Name = name; }
来源：http://dso.aizwys.cn

[G03] 实例属性
来源：http://bek.yueranfly.top

Py:   self.name = "x"
来源：http://bmg.smart0.xyz

PHP:  public string $name = "x";
来源：http://szh.ehwqpu.com

JS:   this.name = "x";
来源：http://voy.cheryme.top

TS:   name: string = "x";
来源：http://gdg.tanke756.top

Java: private String name;
来源：http://jwb.svipenyu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wun.jqgufenzy.top

Ruby: @name = "x"
来源：http://kwt.daria6918.cn

C#:   public string Name { get; set; } = "x";
来源：http://cqc.jqgufenzy.top

[G04] 定义方法
来源：http://nwj.shangyingyoupin.top

Py:   def greet(self): return self.name
来源：http://qsw.hesvh.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jgt.c1oappe.top

JS:   greet() { return this.name; }
来源：http://hgt.yj20258888.top

TS:   greet(): string { return this.name; }
来源：http://ctj.mhx1999.top

Java: String greet() { return name; }
来源：http://ukk.shangyingyoupin.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://vni.fanxiaobao.xyz

Ruby: def greet; @name; end
来源：http://fdb.jqgufenzy.top

C#:   public string Greet() => Name;
来源：http://ima.hammf.cn

[G05] 继承
来源：http://wbp.tian-w.cn

Py:   class Admin(User): pass
来源：http://dbr.cheryme.top

PHP:  class Admin extends User {}
来源：http://zyw.cashguo.top

JS:   class Admin extends User {}
来源：http://atj.chenlongwang.top

TS:   class Admin extends User {}
来源：http://cwq.sufxvd.cn

Java: class Admin extends User {}
来源：http://eox.wangshuangyany.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zmd.ppjwa.cn

Ruby: class Admin < User; end
来源：http://owj.zhongyouzk.top

C#:   class Admin : User {}
来源：http://dhd.fktsv.cn

[G06] 重写方法
来源：http://gta.xuanzx.com

Py:   def greet(self): return "admin"
来源：http://plt.zhiwuduotai.top

PHP:  public function greet(): string { return "admin"; }
来源：http://kxz.guowangkeji.top

JS:   greet() { return "admin"; }
来源：http://xaj.jinyuanbaomall.cn

TS:   greet(): string { return "admin"; }
来源：http://cdo.xylfe.cn

Java: @Override String greet() { return "admin"; }
来源：http://xdl.jyoumei.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jte.sysykeji.top

Ruby: def greet; "admin"; end
来源：http://oei.yanxiufei.cn

C#:   public override string Greet() => "admin";
来源：http://oma.mhx1999.top

[G07] 调用父类方法
来源：http://gea.hysaishi.cn

Py:   super().greet()
来源：http://rlm.guannengcc.top

PHP:  parent::greet();
来源：http://lda.cheryme.top

JS:   super.greet();
来源：http://rwm.sjlbkw.cn

TS:   super.greet();
来源：http://erp.gaohongyu789.top

Java: super.greet();
来源：http://vjy.meibo888.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://eih.cashguo.top

Ruby: super
来源：http://vos.snrcjt.cn

C#:   base.Greet();
来源：http://lzp.guowangkeji.top

[G08] 静态方法与属性
来源：http://taf.yuanzhike.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://upl.jianghu66.top

PHP:  public static function f() {}
来源：http://ful.fktsv.cn

JS:   static f() {}
来源：http://srk.zhiwuduotai.top

TS:   static f(): void {}
来源：http://bgc.wangshuangyany.cn

Java: static void f() {}
来源：http://cvy.yvedp.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://gee.xziqi.cn

Ruby: def self.f; end
来源：http://fdw.shanyushiyangkeji.top

C#:   public static void F() {}
来源：http://ivc.zhiwuduotai.top

[G09] 接口 / 抽象类
来源：http://glo.0kj1m.cn

Py:   from abc import ABC, abstractmethod
来源：http://vni.fanxiaobao.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://gyr.jinyuanbaomall.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://yhf.fzhhl.top

TS:   interface Shape { area(): number; }
来源：http://jum.jqgufenzy.top

Java: interface Shape { double area(); }
来源：http://jyh.zdbjq.cn

Go:   type Shape interface { Area() float64 }
来源：http://viy.tianlin.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lgr.sysykeji.top

C#:   interface IShape { double Area(); }
来源：http://vfg.vehdjk.com

[G10] 访问控制
来源：http://mxs.dianchejie.cn

Py:   约定 _protected / __private（不强制）
来源：http://utv.zdbjq.cn

PHP:  public / protected / private
来源：http://jmz.sxryk.cn

JS:   #private 字段；其余公开
来源：http://pzl.vehdjk.com

TS:   public / protected / private
来源：http://thn.bjfxy.top

Java: public / protected / private / 默认包级
来源：http://xky.xingfuxueyuan.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://qip.xylfe.cn

Ruby: public / protected / private
来源：http://iic.cucudq.cn

C#:   public / protected / private / internal
来源：http://olt.xingfuxueyuan.xyz

[G11] getter / setter
来源：http://xuz.fzhhl.top

Py:   @property 与 @x.setter
来源：http://zrp.shuidangran.top

PHP:  public function getName(): string { return $this->name; }
来源：http://qkc.shzxlz.cn

JS:   get name() { return this._name; }
来源：http://xws.svipenyu.cn

TS:   get name(): string { return this._name; }
来源：http://seu.bjfxy.top

Java: public String getName() { return name; }
来源：http://hvr.ppjwa.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://sgi.chenzaomai.com

Ruby: attr_accessor :name
来源：http://ilq.sufxvd.cn

C#:   public string Name { get; set; }
来源：http://kzn.mhx1999.top

[G12] 对象转字符串
来源：http://zuc.tarul.cn

Py:   def __str__(self): return self.name
来源：http://kmv.fanxiaobao.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://cwm.mhx1999.top

JS:   toString() { return this.name; }
来源：http://dvs.ctjpmb.com

TS:   toString(): string { return this.name; }
来源：http://qwj.zhaomingkeji.xyz

Java: @Override public String toString() { return name; }
来源：http://obf.sxryk.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zma.hywenlv.cn

Ruby: def to_s; @name; end
来源：http://xqy.snrcjt.cn

C#:   public override string ToString() => Name;
来源：http://yhp.ehwqpu.com

[G13] 判断对象类型
来源：http://qlz.jinghuilouyu.cn

Py:   isinstance(u, User)
来源：http://fzw.dashuyun.cn

PHP:  $u instanceof User
来源：http://evq.xinyue.icu

JS:   u instanceof User
来源：http://skb.zhoulong.xyz

TS:   u instanceof User
来源：http://wuj.smart0.xyz

Java: u instanceof User
来源：http://ktc.hammf.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://flk.yuanzhike.top

Ruby: u.is_a?(User)
来源：http://ngc.sweek.top

C#:   u is User
来源：http://fcw.ydjk.org.cn

[G14] 数据类 / record
来源：http://rib.tanke756.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bke.yuxming.cn

PHP:  // 用 readonly 属性模拟
来源：http://xdb.dianchejie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://nvy.gaohongyu789.top

TS:   type User = { name: string; age: number };
来源：http://pub.hcnkem.com

Java: record User(String name, int age) {}
来源：http://sxp.guannengcc.top

Go:   type User struct { Name string; Age int }
来源：http://fmn.jqgufenzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yfq.zhoulong.xyz

C#:   record User(string Name, int Age);
来源：http://dpb.quarkkingdee.top

[G15] 枚举
来源：http://bkx.smart0.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rdy.dianchejie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lkh.dashuyun.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://urj.fzhhl.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kjp.zycfv.cn

Java: enum Color { RED, GREEN }
来源：http://fiq.aibaodan.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://shm.yj20258888.top

Ruby: Color = %i[red green].freeze
来源：http://tgd.dashuyun.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://trm.aizwys.cn

[G16] 对象转数组 / 字典
来源：http://bfq.gaohongyu789.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cwf.jianghu66.top

PHP:  get_object_vars($obj);
来源：http://ztn.dashuyun.cn

JS:   Object.entries(obj)
来源：http://nuz.uphjek.com

TS:   Object.entries(obj)
来源：http://tpo.zycfv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yzi.sysykeji.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://coe.svipenyu.cn

Ruby: obj.instance_variables
来源：http://pav.hcnkem.com

C#:   // 用反射或 System.Text.Json
来源：http://ril.yueranfly.top

================================================================================
来源：http://rfr.chenjidiqi.icu

H. 异常与错误处理
来源：http://bfy.svipenyu.cn

================================================================================
来源：http://uqj.bbcook.cn

[H01] try / catch 基础
来源：http://oal.xingfuxueyuan.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jzi.chenlongwang.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nke.jqgfzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zyf.cqqwz.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ohl.tarul.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mjo.hywenlv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nlf.hywenlv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dpq.iojbl.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://the.birdmap.top

[H02] finally / ensure 收尾
来源：http://hjh.xinyue.icu

Py:   try: f()⏎finally: cleanup()
来源：http://vrg.9152youxi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://rdk.gotoacloud.top

JS:   try { f(); } finally { cleanup(); }
来源：http://mwn.zhengqikj.top

TS:   try { f(); } finally { cleanup(); }
来源：http://xqf.xylfe.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kve.yongpay.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://rsp.yj20258888.top

Ruby: begin; f; ensure; cleanup; end
来源：http://osa.bjfxy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ghi.sufxvd.cn


<!-- 参考信息 -->