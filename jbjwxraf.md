代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://imu.shuidangran.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kyb.fzhhl.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://twf.yj20258888.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zsb.uphjek.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://efj.cqqwz.cn

Go:   // 按 rune 判断长度后截断
来源：http://lmo.sjlbkw.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://icd.jqgufenzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ryc.mhx1999.top

[E22] 字节长度与字符长度
来源：http://sjw.nanxuanxn.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vou.ivvv.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fty.hywenlv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vhk.ybcxt.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cqs.bjfxy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qjb.xingfuxueyuan.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pqx.yuxming.cn

Ruby: s.bytesize;  s.length
来源：http://bwk.fktsv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ryv.316326.xyz

================================================================================
来源：http://hvb.quarkkingdee.top

F. 文件与目录
来源：http://kvx.nanxuanxn.top

================================================================================
来源：http://tgt.guowangkeji.top

[F01] 读取整个文件
来源：http://msd.guowangkeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zhg.andypj.xyz

PHP:  file_get_contents("a.txt");
来源：http://ezi.fzhhl.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xob.guowangkeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://guf.aibaodan.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jee.dashuyun.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://emw.0kj1m.cn

Ruby: File.read("a.txt")
来源：http://qfy.ivvv.top

C#:   File.ReadAllText("a.txt");
来源：http://ymx.nwbrower.top

[F02] 逐行读取文件
来源：http://ofl.guowangkeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kmo.jinqigfzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://use.yj20258.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qmg.hnxiangtu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wwn.kuanghao11.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gnr.gzhubu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kui.vqdsnc.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nls.nwbrower.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mpr.dashuyun.cn

[F03] 写入文件（覆盖）
来源：http://hle.smart0.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://krb.svipenyu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://byj.sufxvd.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lfg.fehbvm.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jmv.wangshuangyany.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vbe.yuxming.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rxn.tian-w.cn

Ruby: File.write("a.txt", "hi")
来源：http://bid.ywan-chungtsiang.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://esd.guannengcc.top

[F04] 追加写入文件
来源：http://zzm.gotoacloud.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://abz.gotoacloud.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xrl.yj202588.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dfp.jinghuilouyu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zhz.uphjek.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lfb.hnqzz.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tpq.ctjpmb.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kbb.feifeiyinyue.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xqt.chenlongwang.top

[F05] 判断文件或目录是否存在
来源：http://kbj.ydjk.org.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pxz.gotoacloud.top

PHP:  file_exists("a.txt");
来源：http://kyx.kuanghao11.cn

JS:   fs.existsSync("a.txt")
来源：http://lew.yuanzhike.top

TS:   fs.existsSync("a.txt")
来源：http://drs.yj20258888.top

Java: Files.exists(Path.of("a.txt"))
来源：http://mcc.aibaodan.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fqc.uphjek.com

Ruby: File.exist?("a.txt")
来源：http://ace.havefunace.top

C#:   File.Exists("a.txt")
来源：http://dvv.vehdjk.com

[F06] 删除文件
来源：http://gzb.svipenyu.cn

Py:   os.remove("a.txt")
来源：http://bmk.ywan-chungtsiang.top

PHP:  unlink("a.txt");
来源：http://jtu.ywan-chungtsiang.top

JS:   fs.unlinkSync("a.txt")
来源：http://uah.jinqigufen.top

TS:   fs.unlinkSync("a.txt")
来源：http://tkk.shanyushiyangkeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pcd.nanxuanxn.top

Go:   os.Remove("a.txt")
来源：http://taz.xziqi.cn

Ruby: File.delete("a.txt")
来源：http://cwr.zhoulong.xyz

C#:   File.Delete("a.txt");
来源：http://vgz.gaohongyu789.top

[F07] 创建目录（含多级）
来源：http://ndg.xinyue.icu

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://eha.haohaochexian.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bgz.sysykeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cke.iojbl.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wtt.wangshuangyany.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://noo.zdqjudy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fzm.jinyuanbaomall.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ler.gotoacloud.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xpc.yvedp.cn

[F08] 遍历目录
来源：http://wro.jinyuanbaomall.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://isv.zhaomingkeji.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://epg.ppjwa.cn

JS:   fs.readdirSync("dir")
来源：http://eok.fanxiaobao.xyz

TS:   fs.readdirSync("dir")
来源：http://pdt.yueranfly.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ozd.nanxinkj.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://nyf.iojbl.cn

Ruby: Dir.children("dir")
来源：http://wym.epnwcf.com

C#:   Directory.GetFiles("dir")
来源：http://utk.ywan-chungtsiang.top

[F09] 获取文件大小
来源：http://gls.chenlongwang.top

Py:   os.path.getsize("a.txt")
来源：http://kxj.52xcode.cn

PHP:  filesize("a.txt");
来源：http://ofl.yonumen.top

JS:   fs.statSync("a.txt").size
来源：http://mnp.zycfv.cn

TS:   fs.statSync("a.txt").size
来源：http://omr.ppjwa.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xvt.jianghu66.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lik.meibo888.top

Ruby: File.size("a.txt")
来源：http://qpx.jlsjyb.cn

C#:   new FileInfo("a.txt").Length
来源：http://hug.wangshuangyany.cn

[F10] 取文件扩展名 / 文件名
来源：http://aqu.jinqigufen.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tay.quarkkingdee.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://usr.ctjpmb.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vix.epnwcf.com

TS:   path.extname("a.txt")
来源：http://jrs.jinghuilouyu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vfq.gzhubu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nhd.vqdsnc.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xeu.ctjpmb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wiv.ydjk.org.cn

[F11] 复制与移动文件
来源：http://wab.sysykeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hgr.tian-w.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lqp.shuidangran.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nse.pengpengdd.cyou

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cri.fehbvm.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lql.vehdjk.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://djl.fehbvm.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kdi.9152youxi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://boa.yuanzhike.top

[F12] CSV 读写
来源：http://syv.ybcxt.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zas.meibo888.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bdn.xziqi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qzm.vehdjk.com

TS:   // 同上
来源：http://tew.yangfankeji.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nig.yongpay.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gsj.guannengcc.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hmx.hywenlv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fii.meibo888.top

================================================================================
来源：http://zsp.jinghuilouyu.cn

G. 面向对象
来源：http://hsp.uphjek.com

================================================================================
来源：http://dgw.sysykeji.top

[G01] 定义类
来源：http://tet.andypj.xyz

Py:   class User: pass
来源：http://gyl.vqdsnc.cn

PHP:  class User {}
来源：http://hvx.ywan-chungtsiang.top

JS:   class User {}
来源：http://ykr.pengpengdd.cyou

TS:   class User { name: string = ""; }
来源：http://xgv.chenlongwang.top

Java: class User {}
来源：http://skd.hywenlv.cn

Go:   type User struct { Name string }
来源：http://xvq.meibo888.top

Ruby: class User; end
来源：http://zxh.fehbvm.com

C#:   class User {}
来源：http://ixa.yonumen.top

[G02] 构造函数
来源：http://kvc.yj202588.top

Py:   def __init__(self, name): self.name = name
来源：http://hpy.ydzc1.top

PHP:  public function __construct(public string $name) {}
来源：http://egd.zycfv.cn

JS:   constructor(name) { this.name = name; }
来源：http://svz.vehdjk.com

TS:   constructor(public name: string) {}
来源：http://uqf.redwolf501.top

Java: User(String name) { this.name = name; }
来源：http://ema.hammf.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pnp.guowangkeji.top

Ruby: def initialize(name); @name = name; end
来源：http://fwd.ivvv.top

C#:   public User(string name) { Name = name; }
来源：http://fbo.daxiang520.top

[G03] 实例属性
来源：http://nbh.hywenlv.cn

Py:   self.name = "x"
来源：http://amc.wangshuangyany.cn

PHP:  public string $name = "x";
来源：http://lof.jianghu66.top

JS:   this.name = "x";
来源：http://llc.ctjpmb.com

TS:   name: string = "x";
来源：http://hbw.shzxlz.cn

Java: private String name;
来源：http://bca.shanyushiyangtech.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://eps.cdnleiting.top

Ruby: @name = "x"
来源：http://uyt.zhixingplan.top

C#:   public string Name { get; set; } = "x";
来源：http://sqo.shzxlz.cn

[G04] 定义方法
来源：http://fbt.fehbvm.com

Py:   def greet(self): return self.name
来源：http://ndy.jlsjyb.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pgw.epnwcf.com

JS:   greet() { return this.name; }
来源：http://gwq.vqdsnc.cn

TS:   greet(): string { return this.name; }
来源：http://vra.xingfuxueyuan.xyz

Java: String greet() { return name; }
来源：http://qzc.hnqzz.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xkh.zhengqikj.top

Ruby: def greet; @name; end
来源：http://nio.bbcook.cn

C#:   public string Greet() => Name;
来源：http://zxj.chenzaomai.com

[G05] 继承
来源：http://ino.redwolf501.top

Py:   class Admin(User): pass
来源：http://pts.hongshengwenyu.top

PHP:  class Admin extends User {}
来源：http://epu.jinghuilouyu.cn

JS:   class Admin extends User {}
来源：http://ztl.tianlin.xyz

TS:   class Admin extends User {}
来源：http://kfy.yj20258.top

Java: class Admin extends User {}
来源：http://qen.vehdjk.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://igm.sufxvd.cn

Ruby: class Admin < User; end
来源：http://ovi.hongshengwenyu.top

C#:   class Admin : User {}
来源：http://dkt.zdbjq.cn

[G06] 重写方法
来源：http://jyj.zycfv.cn

Py:   def greet(self): return "admin"
来源：http://wmc.vehdjk.com

PHP:  public function greet(): string { return "admin"; }
来源：http://mhf.sxryk.cn

JS:   greet() { return "admin"; }
来源：http://prr.xinyue.icu

TS:   greet(): string { return "admin"; }
来源：http://wzh.shanyushiyangtech.top

Java: @Override String greet() { return "admin"; }
来源：http://kyc.shanyushiyangkeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zxa.shangyingyoupin.top

Ruby: def greet; "admin"; end
来源：http://gph.uphjek.com

C#:   public override string Greet() => "admin";
来源：http://ces.aibaodan.cn

[G07] 调用父类方法
来源：http://lpl.hnqzz.top

Py:   super().greet()
来源：http://mjj.pengpengdd.cyou

PHP:  parent::greet();
来源：http://vgz.yfazqb.com

JS:   super.greet();
来源：http://scp.ydjk.org.cn

TS:   super.greet();
来源：http://bvp.dashuyun.cn

Java: super.greet();
来源：http://wqg.ivvv.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dkt.316326.xyz

Ruby: super
来源：http://qjp.andypj.xyz

C#:   base.Greet();
来源：http://xdq.sufxvd.cn

[G08] 静态方法与属性
来源：http://han.316326.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qjr.ydzc1.top

PHP:  public static function f() {}
来源：http://viv.yvedp.cn

JS:   static f() {}
来源：http://pus.jyoumei.cn

TS:   static f(): void {}
来源：http://lfe.guannengcc.top

Java: static void f() {}
来源：http://dye.c1oappe.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://zrx.hnxiangtu.top

Ruby: def self.f; end
来源：http://aaa.guowangkeji.top

C#:   public static void F() {}
来源：http://qlk.gaohongyu789.top

[G09] 接口 / 抽象类
来源：http://luu.fehbvm.com

Py:   from abc import ABC, abstractmethod
来源：http://doa.xylfe.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ere.yj20258888.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://zzv.snrcjt.cn

TS:   interface Shape { area(): number; }
来源：http://wog.jinghuilouyu.cn

Java: interface Shape { double area(); }
来源：http://uuy.gaohongyu789.top

Go:   type Shape interface { Area() float64 }
来源：http://yen.tian-w.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lrq.aibaodan.cn

C#:   interface IShape { double Area(); }
来源：http://lzw.wangdashe.top

[G10] 访问控制
来源：http://tut.tarul.cn

Py:   约定 _protected / __private（不强制）
来源：http://yek.yj202588.top

PHP:  public / protected / private
来源：http://xun.shangyingyoupin.top

JS:   #private 字段；其余公开
来源：http://bgc.c1oappe.top

TS:   public / protected / private
来源：http://xek.hnxiangtu.top

Java: public / protected / private / 默认包级
来源：http://jgk.zhijiandao.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://eph.fzhhl.top

Ruby: public / protected / private
来源：http://qdb.zdbjq.cn

C#:   public / protected / private / internal
来源：http://gyb.jqgufenzy.top

[G11] getter / setter
来源：http://pkw.yuanzhike.top

Py:   @property 与 @x.setter
来源：http://xiz.cdnleiting.top

PHP:  public function getName(): string { return $this->name; }
来源：http://omc.yvedp.cn

JS:   get name() { return this._name; }
来源：http://vlq.ydzc1.top

TS:   get name(): string { return this._name; }
来源：http://ytc.aibaodan.cn

Java: public String getName() { return name; }
来源：http://awf.yangfankeji.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://jrw.aibaodan.cn

Ruby: attr_accessor :name
来源：http://eid.cucudq.cn

C#:   public string Name { get; set; }
来源：http://gmg.sufxvd.cn

[G12] 对象转字符串
来源：http://ozf.hfpthk.cn

Py:   def __str__(self): return self.name
来源：http://scr.sufxvd.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ajv.sjlbkw.cn

JS:   toString() { return this.name; }
来源：http://kmm.bbcook.cn

TS:   toString(): string { return this.name; }
来源：http://hie.yfazqb.com

Java: @Override public String toString() { return name; }
来源：http://mht.xuanzx.com

Go:   func (u User) String() string { return u.Name }
来源：http://sxf.jinqigufen.top

Ruby: def to_s; @name; end
来源：http://fuw.zhixingplan.top

C#:   public override string ToString() => Name;
来源：http://lzk.ywan-chungtsiang.top

[G13] 判断对象类型
来源：http://hsu.yongpay.top

Py:   isinstance(u, User)
来源：http://hji.jinqigufen.top

PHP:  $u instanceof User
来源：http://htn.52xcode.cn

JS:   u instanceof User
来源：http://woc.fanxiaobao.xyz

TS:   u instanceof User
来源：http://xyj.hesvh.cn

Java: u instanceof User
来源：http://cot.zhijiandao.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kvh.tarul.cn

Ruby: u.is_a?(User)
来源：http://mdq.yueranfly.top

C#:   u is User
来源：http://jkw.zhongyouzk.top

[G14] 数据类 / record
来源：http://hpd.sufxvd.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xid.guannengcc.top

PHP:  // 用 readonly 属性模拟
来源：http://elm.fanxiaobao.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://zff.aibaodan.cn

TS:   type User = { name: string; age: number };
来源：http://bwg.svipenyu.cn

Java: record User(String name, int age) {}
来源：http://fnj.vqdsnc.cn

Go:   type User struct { Name string; Age int }
来源：http://rzi.yj20258888.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tee.fanxiaobao.xyz

C#:   record User(string Name, int Age);
来源：http://ezn.dashuyun.cn

[G15] 枚举
来源：http://ncd.jinqigufen.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gia.yongpay.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://tnh.gzhubu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bon.hnxiangtu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://awq.tanke756.top

Java: enum Color { RED, GREEN }
来源：http://fki.ppjwa.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xgv.dashuyun.cn

Ruby: Color = %i[red green].freeze
来源：http://uww.meibo888.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xsa.jinqigufen.top

[G16] 对象转数组 / 字典
来源：http://vgv.yonumen.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bmi.redwolf501.top

PHP:  get_object_vars($obj);
来源：http://jys.epnwcf.com

JS:   Object.entries(obj)
来源：http://evd.xuanzx.com

TS:   Object.entries(obj)
来源：http://ejj.daria6918.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ycz.jlsjyb.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vqs.ppjwa.cn

Ruby: obj.instance_variables
来源：http://dma.nanxinkj.top

C#:   // 用反射或 System.Text.Json
来源：http://dsi.ctjpmb.com

================================================================================
来源：http://mtp.sxryk.cn

H. 异常与错误处理
来源：http://mcn.hfpthk.cn

================================================================================
来源：http://one.vqdsnc.cn

[H01] try / catch 基础
来源：http://xdx.shanyushiyangkeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lth.hnqzz.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mju.shuidangran.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jww.jinghuilouyu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rkd.cdnleiting.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qlp.yj20258.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bbm.daria6918.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dwm.gotoacloud.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pmr.cucudq.cn

[H02] finally / ensure 收尾
来源：http://sgo.bbcook.cn

Py:   try: f()⏎finally: cleanup()
来源：http://fkd.quarkkingdee.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://xli.aibaodan.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://nzz.xziqi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xsl.jinqigufen.top

Java: try { f(); } finally { cleanup(); }
来源：http://lqo.yvedp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tyf.zhengqikj.top

Ruby: begin; f; ensure; cleanup; end
来源：http://hyc.fktsv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zaw.ivvv.top

[H03] 主动抛出异常
来源：http://zuq.dashuyun.cn

Py:   raise ValueError("错误信息")
来源：http://gun.tarul.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hsg.shuidangran.top

JS:   throw new Error("错误信息");
来源：http://txo.jlsjyb.cn


<!-- 参考信息 -->