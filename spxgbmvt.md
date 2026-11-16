代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://aye.dashuyun.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vvq.hfpthk.cn

TS:   if (s === "") {}
来源：http://ynv.pengpengdd.cyou

Java: if (s.isEmpty()) {}
来源：http://hed.meibo888.top

Go:   if s == "" {}
来源：http://jkv.yj202588.top

Ruby: if s.empty?
来源：http://ksj.ydjk.org.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jlm.aibaodan.cn

[E21] 超长截断加省略号
来源：http://qcg.fanxiaobao.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fix.zdqjudy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uet.9152youxi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bmi.nwbrower.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zku.hcnkem.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ych.xuetiantiany.cn

Go:   // 按 rune 判断长度后截断
来源：http://scs.sysykeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://coy.ywan-chungtsiang.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rvg.daxiang520.top

[E22] 字节长度与字符长度
来源：http://jzx.tian-w.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zap.xuetiantiany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dhl.ydjk.org.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dmv.yuxming.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qqm.hywenlv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wcb.daxiang520.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ytn.cdnleiting.top

Ruby: s.bytesize;  s.length
来源：http://eif.hywenlv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://var.haohaochexian.top

================================================================================
来源：http://itt.c1oappe.top

F. 文件与目录
来源：http://phf.zhijiandao.cn

================================================================================
来源：http://hum.xingfuxueyuan.xyz

[F01] 读取整个文件
来源：http://vmb.sjlbkw.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ntm.wangdashe.top

PHP:  file_get_contents("a.txt");
来源：http://osq.fzhhl.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fux.vqdsnc.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qcy.guowangkeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://uue.fehbvm.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tdb.redwolf501.top

Ruby: File.read("a.txt")
来源：http://ehq.jiagoushi.top

C#:   File.ReadAllText("a.txt");
来源：http://tyt.cdnleiting.top

[F02] 逐行读取文件
来源：http://agt.fzhhl.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xyg.tianlin.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jqp.gaohongyu789.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uup.haohaochexian.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qbl.meibo888.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zcj.quarkkingdee.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dvp.mhx1999.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kyb.jinghuilouyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nci.nanxinkj.top

[F03] 写入文件（覆盖）
来源：http://npn.xuetiantiany.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ake.aibaodan.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://awx.ybcxt.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cjs.hywenlv.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kga.zhoulong.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vpo.xuetiantiany.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ntb.jqgufenzy.top

Ruby: File.write("a.txt", "hi")
来源：http://kop.vqdsnc.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vbq.chenzaomai.com

[F04] 追加写入文件
来源：http://pev.jinyuanbaomall.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://myg.cashguo.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ipi.xuetiantiany.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bzt.zhongyouzk.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qcc.fanxiaobao.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lyl.meibo888.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ktx.fktsv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bii.shangyingyoupin.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lvw.shangyingyoupin.top

[F05] 判断文件或目录是否存在
来源：http://llu.9152youxi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nkg.yonumen.top

PHP:  file_exists("a.txt");
来源：http://vhj.snrcjt.cn

JS:   fs.existsSync("a.txt")
来源：http://kmv.jinqigufen.top

TS:   fs.existsSync("a.txt")
来源：http://hcb.xylfe.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://alg.zhoulong.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fff.jqgfzy.top

Ruby: File.exist?("a.txt")
来源：http://tlw.hnqzz.top

C#:   File.Exists("a.txt")
来源：http://hzm.chenjidiqi.icu

[F06] 删除文件
来源：http://vkg.ivvv.top

Py:   os.remove("a.txt")
来源：http://rlp.yj202588.top

PHP:  unlink("a.txt");
来源：http://bau.hcnkem.com

JS:   fs.unlinkSync("a.txt")
来源：http://aje.svipenyu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rpg.pengpengdd.cyou

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://irg.ppjwa.cn

Go:   os.Remove("a.txt")
来源：http://gku.yfazqb.com

Ruby: File.delete("a.txt")
来源：http://asc.52xcode.cn

C#:   File.Delete("a.txt");
来源：http://uis.nanxuanxn.top

[F07] 创建目录（含多级）
来源：http://ncz.wangshuangyany.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://oql.smart0.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mwk.316326.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vjs.svipenyu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vri.yueranfly.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cdw.hysaishi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gjc.nwbrower.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mqm.316326.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fun.dianchejie.cn

[F08] 遍历目录
来源：http://xcx.yonumen.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ljx.yj202588.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://miw.yanxiufei.cn

JS:   fs.readdirSync("dir")
来源：http://bel.fktsv.cn

TS:   fs.readdirSync("dir")
来源：http://oqo.cdnleiting.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wpk.gzhubu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://qrk.xingfuxueyuan.xyz

Ruby: Dir.children("dir")
来源：http://zpa.cheryme.top

C#:   Directory.GetFiles("dir")
来源：http://mpb.quarkkingdee.top

[F09] 获取文件大小
来源：http://mjq.iojbl.cn

Py:   os.path.getsize("a.txt")
来源：http://two.daxiang520.top

PHP:  filesize("a.txt");
来源：http://wtq.chenlongwang.top

JS:   fs.statSync("a.txt").size
来源：http://zbj.andypj.xyz

TS:   fs.statSync("a.txt").size
来源：http://qjg.tarul.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xsd.0kj1m.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://eui.yonumen.top

Ruby: File.size("a.txt")
来源：http://iit.yangfankeji.com

C#:   new FileInfo("a.txt").Length
来源：http://oea.cheryme.top

[F10] 取文件扩展名 / 文件名
来源：http://nee.zhijiandao.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xmv.guannengcc.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yvr.fanxiaobao.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://die.fehbvm.com

TS:   path.extname("a.txt")
来源：http://dja.shanyushiyangkeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qae.cdnleiting.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gzt.iojbl.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jmi.tianlin.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kgf.nanxuanxn.top

[F11] 复制与移动文件
来源：http://ljr.guannengcc.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sno.yangfankeji.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oeb.tian-w.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tgc.shangyingyoupin.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vrd.hesvh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mpa.daria6918.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ada.xziqi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lie.dashuyun.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hsd.ydjk.org.cn

[F12] CSV 读写
来源：http://ltq.sxryk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://twz.ppjwa.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vyt.vqdsnc.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://stt.gaohongyu789.top

TS:   // 同上
来源：http://opj.zhongyouzk.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://eff.zycfv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yfo.snrcjt.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uzx.daria6918.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xbf.hnxiangtu.top

================================================================================
来源：http://tee.hnqzz.top

G. 面向对象
来源：http://cad.daxiang520.top

================================================================================
来源：http://hlz.redwolf501.top

[G01] 定义类
来源：http://cls.jyoumei.cn

Py:   class User: pass
来源：http://duw.sufxvd.cn

PHP:  class User {}
来源：http://lav.yueranfly.top

JS:   class User {}
来源：http://qgq.guowangkeji.top

TS:   class User { name: string = ""; }
来源：http://ujy.yj202588.top

Java: class User {}
来源：http://kuh.zdbjq.cn

Go:   type User struct { Name string }
来源：http://imb.hysaishi.cn

Ruby: class User; end
来源：http://qrp.shzxlz.cn

C#:   class User {}
来源：http://gub.ydzc1.top

[G02] 构造函数
来源：http://fgj.hnxiangtu.top

Py:   def __init__(self, name): self.name = name
来源：http://dbo.snrcjt.cn

PHP:  public function __construct(public string $name) {}
来源：http://ctc.shangyingyoupin.top

JS:   constructor(name) { this.name = name; }
来源：http://xyn.fanxiaobao.xyz

TS:   constructor(public name: string) {}
来源：http://pov.9152youxi.cn

Java: User(String name) { this.name = name; }
来源：http://usu.zycfv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gdc.jinqigfzy.top

Ruby: def initialize(name); @name = name; end
来源：http://jrg.hywenlv.cn

C#:   public User(string name) { Name = name; }
来源：http://ypz.52xcode.cn

[G03] 实例属性
来源：http://nfd.jlsjyb.cn

Py:   self.name = "x"
来源：http://nyj.chenlongwang.top

PHP:  public string $name = "x";
来源：http://rju.316326.xyz

JS:   this.name = "x";
来源：http://pqy.jinqigufen.top

TS:   name: string = "x";
来源：http://lbt.vqdsnc.cn

Java: private String name;
来源：http://shw.quarkkingdee.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sid.daxiang520.top

Ruby: @name = "x"
来源：http://adc.hongshengwenyu.top

C#:   public string Name { get; set; } = "x";
来源：http://rqg.hnqzz.top

[G04] 定义方法
来源：http://qgg.dashuyun.cn

Py:   def greet(self): return self.name
来源：http://acg.dianchejie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wgz.jinqigfzy.top

JS:   greet() { return this.name; }
来源：http://kxa.shangyingyoupin.top

TS:   greet(): string { return this.name; }
来源：http://hma.bbcook.cn

Java: String greet() { return name; }
来源：http://mav.zhaomingkeji.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://hcr.jianghu66.top

Ruby: def greet; @name; end
来源：http://hoy.ehwqpu.com

C#:   public string Greet() => Name;
来源：http://cbz.gotoacloud.top

[G05] 继承
来源：http://unt.zhixingplan.top

Py:   class Admin(User): pass
来源：http://nzo.xylfe.cn

PHP:  class Admin extends User {}
来源：http://yhz.daria6918.cn

JS:   class Admin extends User {}
来源：http://orz.snrcjt.cn

TS:   class Admin extends User {}
来源：http://jyb.yongpay.top

Java: class Admin extends User {}
来源：http://mah.birdmap.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rzp.ctjpmb.com

Ruby: class Admin < User; end
来源：http://bbg.zdbjq.cn

C#:   class Admin : User {}
来源：http://qce.xuanzx.com

[G06] 重写方法
来源：http://uyg.gaohongyu789.top

Py:   def greet(self): return "admin"
来源：http://mfh.yj20258.top

PHP:  public function greet(): string { return "admin"; }
来源：http://qhe.chenjidiqi.icu

JS:   greet() { return "admin"; }
来源：http://tfi.hesvh.cn

TS:   greet(): string { return "admin"; }
来源：http://cok.ydzc1.top

Java: @Override String greet() { return "admin"; }
来源：http://fau.hesvh.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kad.yj202588.top

Ruby: def greet; "admin"; end
来源：http://wwp.iojbl.cn

C#:   public override string Greet() => "admin";
来源：http://ozk.jinqigufen.top

[G07] 调用父类方法
来源：http://dzq.yj20258.top

Py:   super().greet()
来源：http://jjz.pycfn.com

PHP:  parent::greet();
来源：http://gxe.chenzaomai.com

JS:   super.greet();
来源：http://ozt.gaohongyu789.top

TS:   super.greet();
来源：http://hxu.aibaodan.cn

Java: super.greet();
来源：http://yjh.zhongyouzk.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wmc.xinyue.icu

Ruby: super
来源：http://dfw.tarul.cn

C#:   base.Greet();
来源：http://ykh.gzhubu.top

[G08] 静态方法与属性
来源：http://pgi.hcnkem.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fso.sxryk.cn

PHP:  public static function f() {}
来源：http://zfp.gzhubu.top

JS:   static f() {}
来源：http://opc.ehwqpu.com

TS:   static f(): void {}
来源：http://onm.xuetiantiany.cn

Java: static void f() {}
来源：http://yrt.cqqwz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://yvc.haohaochexian.top

Ruby: def self.f; end
来源：http://frx.hesvh.cn

C#:   public static void F() {}
来源：http://uog.jinqigufen.top

[G09] 接口 / 抽象类
来源：http://fap.daxiang520.top

Py:   from abc import ABC, abstractmethod
来源：http://csp.gogol.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pkn.zycfv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cym.havefunace.top

TS:   interface Shape { area(): number; }
来源：http://dgt.yangfankeji.com

Java: interface Shape { double area(); }
来源：http://wmc.hongshengwenyu.top

Go:   type Shape interface { Area() float64 }
来源：http://pgs.cheryme.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ltr.ivvv.top

C#:   interface IShape { double Area(); }
来源：http://qna.yangfankeji.com

[G10] 访问控制
来源：http://clk.sufxvd.cn

Py:   约定 _protected / __private（不强制）
来源：http://pow.gzhubu.top

PHP:  public / protected / private
来源：http://nne.cdnleiting.top

JS:   #private 字段；其余公开
来源：http://pkc.pengpengdd.cyou

TS:   public / protected / private
来源：http://fjz.shanyushiyangkeji.top

Java: public / protected / private / 默认包级
来源：http://qab.shanyushiyangkeji.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://fpx.hywenlv.cn

Ruby: public / protected / private
来源：http://rzq.zdbjq.cn

C#:   public / protected / private / internal
来源：http://tkw.0kj1m.cn

[G11] getter / setter
来源：http://sur.nanxuanxn.top

Py:   @property 与 @x.setter
来源：http://tab.0kj1m.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://tpc.meibo888.top

JS:   get name() { return this._name; }
来源：http://fpu.ydzc1.top

TS:   get name(): string { return this._name; }
来源：http://gwp.jlsjyb.cn

Java: public String getName() { return name; }
来源：http://qdk.yvedp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://okn.shzxlz.cn

Ruby: attr_accessor :name
来源：http://ytz.meibo888.top

C#:   public string Name { get; set; }
来源：http://dvp.yanxiufei.cn

[G12] 对象转字符串
来源：http://nki.gzhubu.top

Py:   def __str__(self): return self.name
来源：http://juz.gaohongyu789.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://qxc.bbcook.cn

JS:   toString() { return this.name; }
来源：http://ncq.zhengqikj.top

TS:   toString(): string { return this.name; }
来源：http://uiq.xuetiantiany.cn

Java: @Override public String toString() { return name; }
来源：http://xrx.aibaodan.cn

Go:   func (u User) String() string { return u.Name }
来源：http://rrs.snrcjt.cn

Ruby: def to_s; @name; end
来源：http://qij.svipenyu.cn

C#:   public override string ToString() => Name;
来源：http://dwy.aizwys.cn

[G13] 判断对象类型
来源：http://qmk.shanyushiyangtech.top

Py:   isinstance(u, User)
来源：http://nmv.shangyingyoupin.top

PHP:  $u instanceof User
来源：http://qub.zhiwuduotai.top

JS:   u instanceof User
来源：http://zgu.guannengcc.top

TS:   u instanceof User
来源：http://udb.yanxiufei.cn

Java: u instanceof User
来源：http://mgg.cucudq.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://okc.cqqwz.cn

Ruby: u.is_a?(User)
来源：http://qrq.zycfv.cn

C#:   u is User
来源：http://ebf.jinqigfzy.top

[G14] 数据类 / record
来源：http://eeu.dianchejie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rzg.ivvv.top

PHP:  // 用 readonly 属性模拟
来源：http://brb.shzxlz.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bhb.yongpay.top

TS:   type User = { name: string; age: number };
来源：http://miw.hnxiangtu.top

Java: record User(String name, int age) {}
来源：http://biu.cqqwz.cn

Go:   type User struct { Name string; Age int }
来源：http://wjp.zhijiandao.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dhy.0kj1m.cn

C#:   record User(string Name, int Age);
来源：http://naf.tanke756.top

[G15] 枚举
来源：http://jlj.yj20258.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kjk.svipenyu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lbs.dashuyun.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iei.fehbvm.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mdq.dashuyun.cn

Java: enum Color { RED, GREEN }
来源：http://aky.yvedp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ayc.zhongyouzk.top

Ruby: Color = %i[red green].freeze
来源：http://nwl.havefunace.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fei.vehdjk.com

[G16] 对象转数组 / 字典
来源：http://ibt.hfpthk.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nix.cheryme.top

PHP:  get_object_vars($obj);
来源：http://fdc.yuxming.cn

JS:   Object.entries(obj)
来源：http://knw.zycfv.cn

TS:   Object.entries(obj)
来源：http://eps.tarul.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hym.jinyuanbaomall.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://nis.yuxming.cn

Ruby: obj.instance_variables
来源：http://jfr.jinghuilouyu.cn

C#:   // 用反射或 System.Text.Json
来源：http://kyj.wangdashe.top

================================================================================
来源：http://ddy.9152youxi.cn

H. 异常与错误处理
来源：http://dte.hammf.cn

================================================================================
来源：http://gfo.jianghu66.top

[H01] try / catch 基础
来源：http://nia.jinyuanbaomall.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vem.hnxiangtu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qjd.smart0.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nus.ehwqpu.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xke.zhengqikj.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gkx.snrcjt.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hzm.meibo888.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mab.aibaodan.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wug.sweek.top

[H02] finally / ensure 收尾
来源：http://vkn.chenjidiqi.icu

Py:   try: f()⏎finally: cleanup()
来源：http://hjk.yonumen.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://fkm.hywenlv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hep.jinyuanbaomall.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lsn.0kj1m.cn


<!-- 参考信息 -->