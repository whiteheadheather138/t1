代发 wailian999

Go:   if s == "" {}
来源：http://sje.vehdjk.com

Ruby: if s.empty?
来源：http://kmw.gotoacloud.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gla.yongpay.top

[E21] 超长截断加省略号
来源：http://jay.kuanghao11.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://esy.sxryk.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pgh.yonumen.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hsl.zhijiandao.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pdu.ywan-chungtsiang.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://aej.316326.xyz

Go:   // 按 rune 判断长度后截断
来源：http://akz.birdmap.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ckq.yj202588.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://krk.bbcook.cn

[E22] 字节长度与字符长度
来源：http://nte.bjfxy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ena.gzhubu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://let.bbcook.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tsh.jyoumei.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://aut.zhoulong.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wst.mhx1999.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hkb.yanxiufei.cn

Ruby: s.bytesize;  s.length
来源：http://aya.zhoulong.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dhm.yuxming.cn

================================================================================
来源：http://dah.ctjpmb.com

F. 文件与目录
来源：http://thn.shanyushiyangkeji.top

================================================================================
来源：http://akk.ydjk.org.cn

[F01] 读取整个文件
来源：http://suv.daxiang520.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uey.yj202588.top

PHP:  file_get_contents("a.txt");
来源：http://pvi.hywenlv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mmv.tanke756.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://udh.ydzc1.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ycz.tarul.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mpn.zhengqikj.top

Ruby: File.read("a.txt")
来源：http://uwg.xylfe.cn

C#:   File.ReadAllText("a.txt");
来源：http://efa.vehdjk.com

[F02] 逐行读取文件
来源：http://noe.guowangkeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lur.snrcjt.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gjd.gogol.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yju.xinyue.icu

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://poq.guowangkeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dsz.zhongyouzk.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://npt.hongshengwenyu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://njh.guannengcc.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mfn.gaohongyu789.top

[F03] 写入文件（覆盖）
来源：http://vgx.yj20258888.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://utm.cqqwz.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mks.sjlbkw.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nqj.dashuyun.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fdz.9152youxi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dnj.bjfxy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://npx.hfpthk.cn

Ruby: File.write("a.txt", "hi")
来源：http://ujv.jqgufenzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nwp.gaohongyu789.top

[F04] 追加写入文件
来源：http://end.dashuyun.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://awr.jiagoushi.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dgq.fanxiaobao.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tlh.jiagoushi.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hal.dianchejie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fog.hysaishi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://exn.gogol.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wym.jinqigufen.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jps.tarul.cn

[F05] 判断文件或目录是否存在
来源：http://qmv.jiagoushi.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bnv.xylfe.cn

PHP:  file_exists("a.txt");
来源：http://qgi.yuanzhike.top

JS:   fs.existsSync("a.txt")
来源：http://fbu.quarkkingdee.top

TS:   fs.existsSync("a.txt")
来源：http://fkt.gzhubu.top

Java: Files.exists(Path.of("a.txt"))
来源：http://imn.daxiang520.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://oqd.jinyuanbaomall.cn

Ruby: File.exist?("a.txt")
来源：http://biy.chenjidiqi.icu

C#:   File.Exists("a.txt")
来源：http://mwv.yonumen.top

[F06] 删除文件
来源：http://rzs.c1oappe.top

Py:   os.remove("a.txt")
来源：http://mvy.ywan-chungtsiang.top

PHP:  unlink("a.txt");
来源：http://omi.ppjwa.cn

JS:   fs.unlinkSync("a.txt")
来源：http://izj.birdmap.top

TS:   fs.unlinkSync("a.txt")
来源：http://cyi.dianchejie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nrv.tarul.cn

Go:   os.Remove("a.txt")
来源：http://wdo.chenzaomai.com

Ruby: File.delete("a.txt")
来源：http://xey.tanke756.top

C#:   File.Delete("a.txt");
来源：http://jpy.c1oappe.top

[F07] 创建目录（含多级）
来源：http://iok.fktsv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dbk.cashguo.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://iyt.fehbvm.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qpe.c1oappe.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cti.c1oappe.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://soj.ydjk.org.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jff.tarul.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qdg.fehbvm.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yyd.mhx1999.top

[F08] 遍历目录
来源：http://sso.jiagoushi.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://fcl.jlsjyb.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sjp.fehbvm.com

JS:   fs.readdirSync("dir")
来源：http://mkx.fzhhl.top

TS:   fs.readdirSync("dir")
来源：http://lpx.hysaishi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://afy.pycfn.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://xmm.xziqi.cn

Ruby: Dir.children("dir")
来源：http://jns.0kj1m.cn

C#:   Directory.GetFiles("dir")
来源：http://izo.fengsongda.top

[F09] 获取文件大小
来源：http://ozy.9152youxi.cn

Py:   os.path.getsize("a.txt")
来源：http://aho.cucudq.cn

PHP:  filesize("a.txt");
来源：http://vak.shzxlz.cn

JS:   fs.statSync("a.txt").size
来源：http://hmz.ivvv.top

TS:   fs.statSync("a.txt").size
来源：http://dqp.aibaodan.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hkx.gaohongyu789.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://niq.shzxlz.cn

Ruby: File.size("a.txt")
来源：http://tai.hfpthk.cn

C#:   new FileInfo("a.txt").Length
来源：http://qtt.zhoulong.xyz

[F10] 取文件扩展名 / 文件名
来源：http://qnh.shanyushiyangtech.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rev.52xcode.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mhr.snrcjt.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zvk.nanxinkj.top

TS:   path.extname("a.txt")
来源：http://ulf.wangdashe.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ajv.xuetiantiany.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rxv.zhixingplan.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ype.gogol.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hfp.316326.xyz

[F11] 复制与移动文件
来源：http://omm.zhixingplan.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fuy.fktsv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vih.fzhhl.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zjm.sjlbkw.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ghl.fehbvm.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bot.shangyingyoupin.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hqj.zhijiandao.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://auy.shuidangran.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ety.smart0.xyz

[F12] CSV 读写
来源：http://vwn.shuidangran.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fwp.hnqzz.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rxj.guowangkeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vjl.zhaomingkeji.xyz

TS:   // 同上
来源：http://wsm.yangfankeji.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qmr.shanyushiyangkeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://icz.jianghu66.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://roi.jqgufenzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://vuf.zhoulong.xyz

================================================================================
来源：http://uog.shanyushiyangtech.top

G. 面向对象
来源：http://alc.smart0.xyz

================================================================================
来源：http://swg.gogol.net.cn

[G01] 定义类
来源：http://qmc.sufxvd.cn

Py:   class User: pass
来源：http://agy.mhx1999.top

PHP:  class User {}
来源：http://kve.jinqigfzy.top

JS:   class User {}
来源：http://lnj.epnwcf.com

TS:   class User { name: string = ""; }
来源：http://ven.iojbl.cn

Java: class User {}
来源：http://olx.redwolf501.top

Go:   type User struct { Name string }
来源：http://zlp.ctjpmb.com

Ruby: class User; end
来源：http://ohg.jqgfzy.top

C#:   class User {}
来源：http://cru.ydzc1.top

[G02] 构造函数
来源：http://byk.zhongyouzk.top

Py:   def __init__(self, name): self.name = name
来源：http://fgl.zhengqikj.top

PHP:  public function __construct(public string $name) {}
来源：http://ioi.sysykeji.top

JS:   constructor(name) { this.name = name; }
来源：http://qwc.yfazqb.com

TS:   constructor(public name: string) {}
来源：http://cni.fktsv.cn

Java: User(String name) { this.name = name; }
来源：http://ion.guowangkeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://edx.zycfv.cn

Ruby: def initialize(name); @name = name; end
来源：http://ola.ybcxt.top

C#:   public User(string name) { Name = name; }
来源：http://cft.guannengcc.top

[G03] 实例属性
来源：http://skf.yvedp.cn

Py:   self.name = "x"
来源：http://amz.hcnkem.com

PHP:  public string $name = "x";
来源：http://tmg.0kj1m.cn

JS:   this.name = "x";
来源：http://vfc.zhijiandao.cn

TS:   name: string = "x";
来源：http://mmz.jinqigufen.top

Java: private String name;
来源：http://xoc.zhaomingkeji.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wqg.yvedp.cn

Ruby: @name = "x"
来源：http://oeu.sufxvd.cn

C#:   public string Name { get; set; } = "x";
来源：http://dfq.aizwys.cn

[G04] 定义方法
来源：http://nfu.xinyue.icu

Py:   def greet(self): return self.name
来源：http://piw.andypj.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://fum.guowangkeji.top

JS:   greet() { return this.name; }
来源：http://nvk.zdbjq.cn

TS:   greet(): string { return this.name; }
来源：http://vbx.316326.xyz

Java: String greet() { return name; }
来源：http://xbb.nwbrower.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://qqb.gzhubu.top

Ruby: def greet; @name; end
来源：http://vyj.0kj1m.cn

C#:   public string Greet() => Name;
来源：http://hrv.fengsongda.top

[G05] 继承
来源：http://rhc.ydjk.org.cn

Py:   class Admin(User): pass
来源：http://tig.zdqjudy.top

PHP:  class Admin extends User {}
来源：http://nxx.jyoumei.cn

JS:   class Admin extends User {}
来源：http://qpf.svipenyu.cn

TS:   class Admin extends User {}
来源：http://poj.gotoacloud.top

Java: class Admin extends User {}
来源：http://vqb.chenzaomai.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ozf.sweek.top

Ruby: class Admin < User; end
来源：http://oqy.jianghu66.top

C#:   class Admin : User {}
来源：http://rvq.haohaochexian.top

[G06] 重写方法
来源：http://mls.shanyushiyangtech.top

Py:   def greet(self): return "admin"
来源：http://bhd.yfazqb.com

PHP:  public function greet(): string { return "admin"; }
来源：http://gxp.sjlbkw.cn

JS:   greet() { return "admin"; }
来源：http://nxe.jiagoushi.top

TS:   greet(): string { return "admin"; }
来源：http://ekq.zhongyouzk.top

Java: @Override String greet() { return "admin"; }
来源：http://fco.xziqi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rqw.ctjpmb.com

Ruby: def greet; "admin"; end
来源：http://kfi.nwbrower.top

C#:   public override string Greet() => "admin";
来源：http://znq.nanxinkj.top

[G07] 调用父类方法
来源：http://iod.dianchejie.cn

Py:   super().greet()
来源：http://cdt.nanxinkj.top

PHP:  parent::greet();
来源：http://usn.hysaishi.cn

JS:   super.greet();
来源：http://iud.hnxiangtu.top

TS:   super.greet();
来源：http://kox.havefunace.top

Java: super.greet();
来源：http://sat.wangshuangyany.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cqa.sufxvd.cn

Ruby: super
来源：http://urp.xinyue.icu

C#:   base.Greet();
来源：http://asr.yanxiufei.cn

[G08] 静态方法与属性
来源：http://nud.mhx1999.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://soj.xinyue.icu

PHP:  public static function f() {}
来源：http://zqb.dashuyun.cn

JS:   static f() {}
来源：http://nmb.haohaochexian.top

TS:   static f(): void {}
来源：http://twn.aizwys.cn

Java: static void f() {}
来源：http://hui.yueranfly.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://zcv.pycfn.com

Ruby: def self.f; end
来源：http://wyn.tarul.cn

C#:   public static void F() {}
来源：http://fwf.9152youxi.cn

[G09] 接口 / 抽象类
来源：http://hqa.chenjidiqi.icu

Py:   from abc import ABC, abstractmethod
来源：http://yym.nanxuanxn.top

PHP:  interface Shape { public function area(): float; }
来源：http://lbp.zhoulong.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://uah.sxryk.cn

TS:   interface Shape { area(): number; }
来源：http://ozy.zhaomingkeji.xyz

Java: interface Shape { double area(); }
来源：http://xkj.yonumen.top

Go:   type Shape interface { Area() float64 }
来源：http://rnt.cucudq.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wom.mhx1999.top

C#:   interface IShape { double Area(); }
来源：http://cmv.xingfuxueyuan.xyz

[G10] 访问控制
来源：http://uhq.mhx1999.top

Py:   约定 _protected / __private（不强制）
来源：http://lxd.hfpthk.cn

PHP:  public / protected / private
来源：http://qvm.wangshuangyany.cn

JS:   #private 字段；其余公开
来源：http://zvx.chenjidiqi.icu

TS:   public / protected / private
来源：http://xrf.ywan-chungtsiang.top

Java: public / protected / private / 默认包级
来源：http://xer.gogol.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qhi.xziqi.cn

Ruby: public / protected / private
来源：http://pna.fanxiaobao.xyz

C#:   public / protected / private / internal
来源：http://fei.xingfuxueyuan.xyz

[G11] getter / setter
来源：http://fxs.cqqwz.cn

Py:   @property 与 @x.setter
来源：http://riv.zhengqikj.top

PHP:  public function getName(): string { return $this->name; }
来源：http://hpy.fktsv.cn

JS:   get name() { return this._name; }
来源：http://jpq.shuidangran.top

TS:   get name(): string { return this._name; }
来源：http://eyg.zhengqikj.top

Java: public String getName() { return name; }
来源：http://tap.chenlongwang.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://evq.ppjwa.cn

Ruby: attr_accessor :name
来源：http://eun.aibaodan.cn

C#:   public string Name { get; set; }
来源：http://mod.feifeiyinyue.top

[G12] 对象转字符串
来源：http://ddg.hfpthk.cn

Py:   def __str__(self): return self.name
来源：http://gdu.gzhubu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://coe.iojbl.cn

JS:   toString() { return this.name; }
来源：http://zlh.hcnkem.com

TS:   toString(): string { return this.name; }
来源：http://mtt.guannengcc.top

Java: @Override public String toString() { return name; }
来源：http://yra.fzhhl.top

Go:   func (u User) String() string { return u.Name }
来源：http://nms.yj20258888.top

Ruby: def to_s; @name; end
来源：http://zom.hywenlv.cn

C#:   public override string ToString() => Name;
来源：http://xjp.gotoacloud.top

[G13] 判断对象类型
来源：http://wtp.tian-w.cn

Py:   isinstance(u, User)
来源：http://jqb.yvedp.cn

PHP:  $u instanceof User
来源：http://zgv.jinghuilouyu.cn

JS:   u instanceof User
来源：http://oku.zhoulong.xyz

TS:   u instanceof User
来源：http://tmc.redwolf501.top

Java: u instanceof User
来源：http://ssb.ctjpmb.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://juz.xylfe.cn

Ruby: u.is_a?(User)
来源：http://son.ppjwa.cn

C#:   u is User
来源：http://okj.bbcook.cn

[G14] 数据类 / record
来源：http://mpa.zhaomingkeji.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://foa.fzhhl.top

PHP:  // 用 readonly 属性模拟
来源：http://zke.jinqigfzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://kxn.dianchejie.cn

TS:   type User = { name: string; age: number };
来源：http://nqu.316326.xyz

Java: record User(String name, int age) {}
来源：http://emh.redwolf501.top

Go:   type User struct { Name string; Age int }
来源：http://yaw.dianchejie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ulo.wangshuangyany.cn

C#:   record User(string Name, int Age);
来源：http://vyx.chenjidiqi.icu

[G15] 枚举
来源：http://auj.nanxinkj.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wkw.zycfv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://efk.nwbrower.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sqw.9152youxi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hnp.yongpay.top

Java: enum Color { RED, GREEN }
来源：http://igw.hysaishi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rys.daria6918.cn

Ruby: Color = %i[red green].freeze
来源：http://ywe.hesvh.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kzr.sufxvd.cn

[G16] 对象转数组 / 字典
来源：http://fin.sjlbkw.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://omq.cheryme.top

PHP:  get_object_vars($obj);
来源：http://hhn.chenjidiqi.icu

JS:   Object.entries(obj)
来源：http://wxg.wangdashe.top

TS:   Object.entries(obj)
来源：http://axr.cashguo.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vvo.pengpengdd.cyou

Go:   // 手写转换，或用 mapstructure 库
来源：http://xgu.xuetiantiany.cn

Ruby: obj.instance_variables
来源：http://uvo.svipenyu.cn

C#:   // 用反射或 System.Text.Json
来源：http://jzh.ctjpmb.com

================================================================================
来源：http://aot.jlsjyb.cn

H. 异常与错误处理
来源：http://lhd.sxryk.cn

================================================================================
来源：http://wne.cdnleiting.top

[H01] try / catch 基础
来源：http://mdu.havefunace.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gck.iojbl.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jte.nwbrower.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pnr.fengsongda.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ive.zhijiandao.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qix.jqgfzy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qls.hnqzz.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rxg.jinyuanbaomall.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://axy.yuanzhike.top

[H02] finally / ensure 收尾
来源：http://dey.shangyingyoupin.top

Py:   try: f()⏎finally: cleanup()
来源：http://yjh.zdqjudy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ucn.sjlbkw.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://dzv.yonumen.top

TS:   try { f(); } finally { cleanup(); }
来源：http://bes.aizwys.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ikg.cqqwz.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qvh.chenjidiqi.icu

Ruby: begin; f; ensure; cleanup; end
来源：http://kmw.cdnleiting.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://auj.fengsongda.top


<!-- 参考信息 -->