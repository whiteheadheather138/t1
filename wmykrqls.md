代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://duo.xziqi.cn

Go:   // 按 rune 判断长度后截断
来源：http://mxc.zhengqikj.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://foq.meibo888.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zji.ybcxt.top

[E22] 字节长度与字符长度
来源：http://yuw.shanyushiyangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pfi.haohaochexian.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ycd.sxryk.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vxk.yongpay.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dyx.haohaochexian.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lxh.zhiwuduotai.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://msf.redwolf501.top

Ruby: s.bytesize;  s.length
来源：http://ehx.hnxiangtu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dpa.jiagoushi.top

================================================================================
来源：http://agx.c1oappe.top

F. 文件与目录
来源：http://kdr.kuanghao11.cn

================================================================================
来源：http://jct.nwbrower.top

[F01] 读取整个文件
来源：http://rzi.zhengqikj.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ovp.cdnleiting.top

PHP:  file_get_contents("a.txt");
来源：http://vyk.havefunace.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ddo.nanxuanxn.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ljo.ctjpmb.com

Java: Files.readString(Path.of("a.txt"))
来源：http://zvl.hywenlv.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://avn.xingfuxueyuan.xyz

Ruby: File.read("a.txt")
来源：http://nfh.yfazqb.com

C#:   File.ReadAllText("a.txt");
来源：http://jsb.ydzc1.top

[F02] 逐行读取文件
来源：http://ehm.yuxming.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ddj.0kj1m.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xry.fehbvm.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ebe.ydzc1.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bpp.mhx1999.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kai.chenjidiqi.icu

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oqt.meibo888.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lrs.pycfn.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pyh.hysaishi.cn

[F03] 写入文件（覆盖）
来源：http://pqd.gzhubu.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rel.jianghu66.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://cit.dashuyun.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vla.nanxuanxn.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sbx.xuetiantiany.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fpr.ctjpmb.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ute.ybcxt.top

Ruby: File.write("a.txt", "hi")
来源：http://tiv.aizwys.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hrn.9152youxi.cn

[F04] 追加写入文件
来源：http://rdp.gzhubu.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://irh.jinghuilouyu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zne.snrcjt.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gtk.feifeiyinyue.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ufo.ehwqpu.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vur.shzxlz.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fbp.fengsongda.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ups.feifeiyinyue.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://djl.xylfe.cn

[F05] 判断文件或目录是否存在
来源：http://jsv.cashguo.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://alf.daxiang520.top

PHP:  file_exists("a.txt");
来源：http://xfo.shangyingyoupin.top

JS:   fs.existsSync("a.txt")
来源：http://gmc.ehwqpu.com

TS:   fs.existsSync("a.txt")
来源：http://erx.shangyingyoupin.top

Java: Files.exists(Path.of("a.txt"))
来源：http://fgb.shuidangran.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uyt.yuxming.cn

Ruby: File.exist?("a.txt")
来源：http://cxg.meibo888.top

C#:   File.Exists("a.txt")
来源：http://pax.gaohongyu789.top

[F06] 删除文件
来源：http://ljh.jyoumei.cn

Py:   os.remove("a.txt")
来源：http://oxz.ehwqpu.com

PHP:  unlink("a.txt");
来源：http://cvf.xingfuxueyuan.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://gbb.zhiwuduotai.top

TS:   fs.unlinkSync("a.txt")
来源：http://sbc.fktsv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kep.jianghu66.top

Go:   os.Remove("a.txt")
来源：http://juu.uphjek.com

Ruby: File.delete("a.txt")
来源：http://lnq.andypj.xyz

C#:   File.Delete("a.txt");
来源：http://hrc.hysaishi.cn

[F07] 创建目录（含多级）
来源：http://uja.aibaodan.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://msn.zhijiandao.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qyd.aizwys.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jfm.316326.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iua.hesvh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bwy.hongshengwenyu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qcy.zhaomingkeji.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pem.sysykeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://esi.iojbl.cn

[F08] 遍历目录
来源：http://kda.cheryme.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://csa.zhoulong.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yep.guowangkeji.top

JS:   fs.readdirSync("dir")
来源：http://jif.epnwcf.com

TS:   fs.readdirSync("dir")
来源：http://yzi.havefunace.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vyo.zhengqikj.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ymd.fzhhl.top

Ruby: Dir.children("dir")
来源：http://dsl.shanyushiyangtech.top

C#:   Directory.GetFiles("dir")
来源：http://rrv.sjlbkw.cn

[F09] 获取文件大小
来源：http://nxz.jyoumei.cn

Py:   os.path.getsize("a.txt")
来源：http://rxo.zhengqikj.top

PHP:  filesize("a.txt");
来源：http://exn.ivvv.top

JS:   fs.statSync("a.txt").size
来源：http://xbp.jinyuanbaomall.cn

TS:   fs.statSync("a.txt").size
来源：http://szd.zdbjq.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vhe.hnqzz.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xeh.tian-w.cn

Ruby: File.size("a.txt")
来源：http://ndt.xylfe.cn

C#:   new FileInfo("a.txt").Length
来源：http://emi.hfpthk.cn

[F10] 取文件扩展名 / 文件名
来源：http://opm.jyoumei.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cqo.tianlin.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kvh.jinyuanbaomall.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mvn.hesvh.cn

TS:   path.extname("a.txt")
来源：http://uew.quarkkingdee.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://let.ybcxt.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mhc.jqgfzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kjr.cheryme.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lwd.jyoumei.cn

[F11] 复制与移动文件
来源：http://eeg.yj20258.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://whm.fehbvm.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sbc.316326.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xyl.smart0.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qou.hcnkem.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://okd.zhengqikj.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cxo.cucudq.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gaj.yongpay.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jxp.yj202588.top

[F12] CSV 读写
来源：http://zkb.yvedp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kge.c1oappe.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://meq.ywan-chungtsiang.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sur.zhijiandao.cn

TS:   // 同上
来源：http://rsb.jinghuilouyu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ggu.xuetiantiany.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jhi.9152youxi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dzc.ydzc1.top

C#:   // 无内置：用 CsvHelper 库
来源：http://tgv.quarkkingdee.top

================================================================================
来源：http://ixs.fktsv.cn

G. 面向对象
来源：http://ixg.jlsjyb.cn

================================================================================
来源：http://tth.xinyue.icu

[G01] 定义类
来源：http://dfc.ydzc1.top

Py:   class User: pass
来源：http://hji.tanke756.top

PHP:  class User {}
来源：http://mvw.andypj.xyz

JS:   class User {}
来源：http://ush.pengpengdd.cyou

TS:   class User { name: string = ""; }
来源：http://chf.ctjpmb.com

Java: class User {}
来源：http://odj.aizwys.cn

Go:   type User struct { Name string }
来源：http://jvq.yj20258.top

Ruby: class User; end
来源：http://pnj.zhongyouzk.top

C#:   class User {}
来源：http://tzv.gaohongyu789.top

[G02] 构造函数
来源：http://nrr.cqqwz.cn

Py:   def __init__(self, name): self.name = name
来源：http://nad.xuanzx.com

PHP:  public function __construct(public string $name) {}
来源：http://mxm.yanxiufei.cn

JS:   constructor(name) { this.name = name; }
来源：http://fwm.hysaishi.cn

TS:   constructor(public name: string) {}
来源：http://nlj.zycfv.cn

Java: User(String name) { this.name = name; }
来源：http://qmz.meibo888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nyq.zdbjq.cn

Ruby: def initialize(name); @name = name; end
来源：http://vxn.nanxinkj.top

C#:   public User(string name) { Name = name; }
来源：http://vsh.shangyingyoupin.top

[G03] 实例属性
来源：http://vnu.zhengqikj.top

Py:   self.name = "x"
来源：http://osa.xuanzx.com

PHP:  public string $name = "x";
来源：http://qad.andypj.xyz

JS:   this.name = "x";
来源：http://mjy.feifeiyinyue.top

TS:   name: string = "x";
来源：http://qxa.snrcjt.cn

Java: private String name;
来源：http://vkb.hfpthk.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xlx.jiagoushi.top

Ruby: @name = "x"
来源：http://kna.xziqi.cn

C#:   public string Name { get; set; } = "x";
来源：http://uce.hnxiangtu.top

[G04] 定义方法
来源：http://adb.316326.xyz

Py:   def greet(self): return self.name
来源：http://hsl.nanxuanxn.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hrv.guowangkeji.top

JS:   greet() { return this.name; }
来源：http://zbu.fehbvm.com

TS:   greet(): string { return this.name; }
来源：http://vzg.gogol.net.cn

Java: String greet() { return name; }
来源：http://uju.zhiwuduotai.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ogr.pycfn.com

Ruby: def greet; @name; end
来源：http://cmq.hesvh.cn

C#:   public string Greet() => Name;
来源：http://hii.sysykeji.top

[G05] 继承
来源：http://wok.zhixingplan.top

Py:   class Admin(User): pass
来源：http://xwz.dianchejie.cn

PHP:  class Admin extends User {}
来源：http://ugh.snrcjt.cn

JS:   class Admin extends User {}
来源：http://cfz.0kj1m.cn

TS:   class Admin extends User {}
来源：http://jwa.yuxming.cn

Java: class Admin extends User {}
来源：http://rva.chenzaomai.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mrx.yueranfly.top

Ruby: class Admin < User; end
来源：http://hnc.yj20258.top

C#:   class Admin : User {}
来源：http://hin.nanxuanxn.top

[G06] 重写方法
来源：http://kkc.tarul.cn

Py:   def greet(self): return "admin"
来源：http://iqu.xuanzx.com

PHP:  public function greet(): string { return "admin"; }
来源：http://bhl.fanxiaobao.xyz

JS:   greet() { return "admin"; }
来源：http://mhl.yfazqb.com

TS:   greet(): string { return "admin"; }
来源：http://txh.yuxming.cn

Java: @Override String greet() { return "admin"; }
来源：http://fqm.fanxiaobao.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dnk.zhiwuduotai.top

Ruby: def greet; "admin"; end
来源：http://rfx.tarul.cn

C#:   public override string Greet() => "admin";
来源：http://mcg.zhaomingkeji.xyz

[G07] 调用父类方法
来源：http://kxm.xuetiantiany.cn

Py:   super().greet()
来源：http://xqo.uphjek.com

PHP:  parent::greet();
来源：http://wnt.hfpthk.cn

JS:   super.greet();
来源：http://ywk.bbcook.cn

TS:   super.greet();
来源：http://szf.nanxuanxn.top

Java: super.greet();
来源：http://wvm.yj202588.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mvv.xinyue.icu

Ruby: super
来源：http://rck.haohaochexian.top

C#:   base.Greet();
来源：http://hvs.yuanzhike.top

[G08] 静态方法与属性
来源：http://gdd.hnqzz.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://klq.zhaomingkeji.xyz

PHP:  public static function f() {}
来源：http://lnz.ppjwa.cn

JS:   static f() {}
来源：http://bxc.zhongyouzk.top

TS:   static f(): void {}
来源：http://gdf.guowangkeji.top

Java: static void f() {}
来源：http://rzm.hcnkem.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://gbo.snrcjt.cn

Ruby: def self.f; end
来源：http://zga.ybcxt.top

C#:   public static void F() {}
来源：http://zdc.yj202588.top

[G09] 接口 / 抽象类
来源：http://vlm.gogol.net.cn

Py:   from abc import ABC, abstractmethod
来源：http://tip.xziqi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ffa.wangdashe.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://exc.feifeiyinyue.top

TS:   interface Shape { area(): number; }
来源：http://ytr.zhijiandao.cn

Java: interface Shape { double area(); }
来源：http://vgj.hammf.cn

Go:   type Shape interface { Area() float64 }
来源：http://jqk.sjlbkw.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://aku.xziqi.cn

C#:   interface IShape { double Area(); }
来源：http://zsg.gogol.net.cn

[G10] 访问控制
来源：http://isn.zycfv.cn

Py:   约定 _protected / __private（不强制）
来源：http://btg.jyoumei.cn

PHP:  public / protected / private
来源：http://mgz.zhoulong.xyz

JS:   #private 字段；其余公开
来源：http://wxy.daria6918.cn

TS:   public / protected / private
来源：http://hch.haohaochexian.top

Java: public / protected / private / 默认包级
来源：http://feb.zhoulong.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://hom.nwbrower.top

Ruby: public / protected / private
来源：http://wdv.ydzc1.top

C#:   public / protected / private / internal
来源：http://wtv.guowangkeji.top

[G11] getter / setter
来源：http://xqt.cashguo.top

Py:   @property 与 @x.setter
来源：http://few.quarkkingdee.top

PHP:  public function getName(): string { return $this->name; }
来源：http://vjc.nanxinkj.top

JS:   get name() { return this._name; }
来源：http://psi.hfpthk.cn

TS:   get name(): string { return this._name; }
来源：http://iuj.cashguo.top

Java: public String getName() { return name; }
来源：http://fus.bbcook.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://nwm.xziqi.cn

Ruby: attr_accessor :name
来源：http://wja.zdqjudy.top

C#:   public string Name { get; set; }
来源：http://jxt.vqdsnc.cn

[G12] 对象转字符串
来源：http://sxx.jinghuilouyu.cn

Py:   def __str__(self): return self.name
来源：http://mlq.c1oappe.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://rfv.yfazqb.com

JS:   toString() { return this.name; }
来源：http://fcb.gzhubu.top

TS:   toString(): string { return this.name; }
来源：http://gwh.zhaomingkeji.xyz

Java: @Override public String toString() { return name; }
来源：http://mgc.aizwys.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ivp.fengsongda.top

Ruby: def to_s; @name; end
来源：http://lil.jyoumei.cn

C#:   public override string ToString() => Name;
来源：http://ytk.chenjidiqi.icu

[G13] 判断对象类型
来源：http://iih.zycfv.cn

Py:   isinstance(u, User)
来源：http://lin.shzxlz.cn

PHP:  $u instanceof User
来源：http://gfz.fktsv.cn

JS:   u instanceof User
来源：http://sbd.svipenyu.cn

TS:   u instanceof User
来源：http://ocj.tianlin.xyz

Java: u instanceof User
来源：http://taf.yonumen.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://vha.hnqzz.top

Ruby: u.is_a?(User)
来源：http://dge.tianlin.xyz

C#:   u is User
来源：http://gir.ydjk.org.cn

[G14] 数据类 / record
来源：http://ccf.sjlbkw.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ras.andypj.xyz

PHP:  // 用 readonly 属性模拟
来源：http://tmk.zhaomingkeji.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://lbi.hesvh.cn

TS:   type User = { name: string; age: number };
来源：http://vyl.yj202588.top

Java: record User(String name, int age) {}
来源：http://yav.jinghuilouyu.cn

Go:   type User struct { Name string; Age int }
来源：http://vwp.zhixingplan.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jwi.jiagoushi.top

C#:   record User(string Name, int Age);
来源：http://ayf.hcnkem.com

[G15] 枚举
来源：http://tvt.sufxvd.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mkr.fzhhl.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://rrv.gogol.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pmq.xinyue.icu

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mrh.jinghuilouyu.cn

Java: enum Color { RED, GREEN }
来源：http://kwi.xuanzx.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tng.c1oappe.top

Ruby: Color = %i[red green].freeze
来源：http://lnq.yfazqb.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ppg.andypj.xyz

[G16] 对象转数组 / 字典
来源：http://bko.yueranfly.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zed.tianlin.xyz

PHP:  get_object_vars($obj);
来源：http://pnb.gogol.net.cn

JS:   Object.entries(obj)
来源：http://osw.zycfv.cn

TS:   Object.entries(obj)
来源：http://sqh.chenjidiqi.icu

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jlu.fehbvm.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://fds.daxiang520.top

Ruby: obj.instance_variables
来源：http://cod.epnwcf.com

C#:   // 用反射或 System.Text.Json
来源：http://phq.ehwqpu.com

================================================================================
来源：http://ucp.zhaomingkeji.xyz

H. 异常与错误处理
来源：http://yde.zdbjq.cn

================================================================================
来源：http://cdl.dianchejie.cn

[H01] try / catch 基础
来源：http://mml.c1oappe.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cme.fengsongda.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://oac.zhoulong.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://trq.fzhhl.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://adl.guowangkeji.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dtp.tanke756.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xnb.yueranfly.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zbu.iojbl.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vwd.hnxiangtu.top

[H02] finally / ensure 收尾
来源：http://pch.yongpay.top

Py:   try: f()⏎finally: cleanup()
来源：http://qnj.bbcook.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://eof.daria6918.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gfj.nanxuanxn.top

TS:   try { f(); } finally { cleanup(); }
来源：http://usu.nwbrower.top

Java: try { f(); } finally { cleanup(); }
来源：http://fpi.zdbjq.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zkv.birdmap.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ubt.jinqigufen.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://gai.jinqigufen.top

[H03] 主动抛出异常
来源：http://zwr.c1oappe.top

Py:   raise ValueError("错误信息")
来源：http://bjp.ehwqpu.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zxo.sysykeji.top

JS:   throw new Error("错误信息");
来源：http://ckj.havefunace.top

TS:   throw new Error("错误信息");
来源：http://yce.fktsv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://byn.sjlbkw.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jbw.zhiwuduotai.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ise.tarul.cn


<!-- 参考信息 -->