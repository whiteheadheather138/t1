代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vvm.dianchejie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://viv.316326.xyz

TS:   if (s === "") {}
来源：http://mrb.bbcook.cn

Java: if (s.isEmpty()) {}
来源：http://lvj.tian-w.cn

Go:   if s == "" {}
来源：http://gle.fktsv.cn

Ruby: if s.empty?
来源：http://kpr.shuidangran.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jvp.yj20258.top

[E21] 超长截断加省略号
来源：http://kut.316326.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rnp.smart0.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://phf.hfpthk.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dmc.chenzaomai.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yyo.zhengqikj.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sqv.epnwcf.com

Go:   // 按 rune 判断长度后截断
来源：http://vpm.yfazqb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kyc.ybcxt.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jtx.ctjpmb.com

[E22] 字节长度与字符长度
来源：http://kop.tarul.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://htc.mhx1999.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yql.xuanzx.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://okm.tarul.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kvn.uphjek.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ecv.ehwqpu.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dwv.meibo888.top

Ruby: s.bytesize;  s.length
来源：http://mro.mhx1999.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://iga.ivvv.top

================================================================================
来源：http://ymn.redwolf501.top

F. 文件与目录
来源：http://hyi.ehwqpu.com

================================================================================
来源：http://vjj.yfazqb.com

[F01] 读取整个文件
来源：http://dmu.jinghuilouyu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sua.yuxming.cn

PHP:  file_get_contents("a.txt");
来源：http://kwo.snrcjt.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lsv.guannengcc.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pqr.snrcjt.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hce.ydzc1.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wsd.nwbrower.top

Ruby: File.read("a.txt")
来源：http://rke.ivvv.top

C#:   File.ReadAllText("a.txt");
来源：http://wpo.jinqigufen.top

[F02] 逐行读取文件
来源：http://tvr.xuetiantiany.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://upe.hnxiangtu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rug.gaohongyu789.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qbg.guowangkeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rnh.52xcode.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xuf.hnxiangtu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://peo.pycfn.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://urv.snrcjt.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rlx.zhengqikj.top

[F03] 写入文件（覆盖）
来源：http://dno.epnwcf.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rpn.chenjidiqi.icu

PHP:  file_put_contents("a.txt", "hi");
来源：http://zes.jyoumei.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nyz.hfpthk.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iqq.daria6918.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ecu.guowangkeji.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gva.ivvv.top

Ruby: File.write("a.txt", "hi")
来源：http://nos.meibo888.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://iyv.zhengqikj.top

[F04] 追加写入文件
来源：http://auc.jqgufenzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gmm.ywan-chungtsiang.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rmj.vqdsnc.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mrk.jqgfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qyx.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sxt.jyoumei.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://awx.shzxlz.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wos.jlsjyb.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cnq.jqgfzy.top

[F05] 判断文件或目录是否存在
来源：http://vbc.shanyushiyangkeji.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wez.yuxming.cn

PHP:  file_exists("a.txt");
来源：http://bnw.nanxinkj.top

JS:   fs.existsSync("a.txt")
来源：http://oka.aibaodan.cn

TS:   fs.existsSync("a.txt")
来源：http://mcu.wangdashe.top

Java: Files.exists(Path.of("a.txt"))
来源：http://vwh.c1oappe.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qat.shanyushiyangtech.top

Ruby: File.exist?("a.txt")
来源：http://mpn.nwbrower.top

C#:   File.Exists("a.txt")
来源：http://vsb.redwolf501.top

[F06] 删除文件
来源：http://fto.chenzaomai.com

Py:   os.remove("a.txt")
来源：http://wiy.shuidangran.top

PHP:  unlink("a.txt");
来源：http://jko.gogol.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nkd.hesvh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://owm.nwbrower.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ktd.yangfankeji.com

Go:   os.Remove("a.txt")
来源：http://tuv.yonumen.top

Ruby: File.delete("a.txt")
来源：http://kmd.bjfxy.top

C#:   File.Delete("a.txt");
来源：http://zvt.aibaodan.cn

[F07] 创建目录（含多级）
来源：http://zib.xuetiantiany.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vmf.ppjwa.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sac.jiagoushi.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://djg.ywan-chungtsiang.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ggc.yongpay.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://isp.aibaodan.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yly.shuidangran.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vkh.hongshengwenyu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://czm.bjfxy.top

[F08] 遍历目录
来源：http://gxx.52xcode.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mox.tanke756.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ksm.xuanzx.com

JS:   fs.readdirSync("dir")
来源：http://hfq.nanxinkj.top

TS:   fs.readdirSync("dir")
来源：http://hoa.chenjidiqi.icu

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bim.jinqigfzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://iia.gogol.net.cn

Ruby: Dir.children("dir")
来源：http://ypi.jyoumei.cn

C#:   Directory.GetFiles("dir")
来源：http://pxw.dianchejie.cn

[F09] 获取文件大小
来源：http://pzb.hammf.cn

Py:   os.path.getsize("a.txt")
来源：http://rwu.yuxming.cn

PHP:  filesize("a.txt");
来源：http://fvx.yj202588.top

JS:   fs.statSync("a.txt").size
来源：http://dip.fktsv.cn

TS:   fs.statSync("a.txt").size
来源：http://kfk.zhixingplan.top

Java: Files.size(Path.of("a.txt"))
来源：http://onu.uphjek.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lat.feifeiyinyue.top

Ruby: File.size("a.txt")
来源：http://cia.zdbjq.cn

C#:   new FileInfo("a.txt").Length
来源：http://rkj.jiagoushi.top

[F10] 取文件扩展名 / 文件名
来源：http://pmh.nanxuanxn.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xgs.snrcjt.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://oec.snrcjt.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nac.shzxlz.cn

TS:   path.extname("a.txt")
来源：http://xmb.52xcode.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bia.yuxming.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://exs.aibaodan.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://shg.shangyingyoupin.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vwu.pengpengdd.cyou

[F11] 复制与移动文件
来源：http://uht.pycfn.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ydn.aibaodan.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zlc.jinyuanbaomall.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fxo.mhx1999.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://soy.sysykeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://eve.jinqigfzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dwe.guowangkeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wwc.chenjidiqi.icu

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kpl.svipenyu.cn

[F12] CSV 读写
来源：http://qpe.cashguo.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ioc.andypj.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ytd.sjlbkw.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ssd.uphjek.com

TS:   // 同上
来源：http://jyk.cheryme.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ttn.fzhhl.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cqg.yueranfly.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://iyw.kuanghao11.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://txt.sweek.top

================================================================================
来源：http://lkr.chenjidiqi.icu

G. 面向对象
来源：http://ulu.tianlin.xyz

================================================================================
来源：http://auz.gaohongyu789.top

[G01] 定义类
来源：http://bud.hnxiangtu.top

Py:   class User: pass
来源：http://njq.nanxuanxn.top

PHP:  class User {}
来源：http://ijx.ydzc1.top

JS:   class User {}
来源：http://dot.ydzc1.top

TS:   class User { name: string = ""; }
来源：http://xtp.sufxvd.cn

Java: class User {}
来源：http://elr.andypj.xyz

Go:   type User struct { Name string }
来源：http://nvd.mhx1999.top

Ruby: class User; end
来源：http://liy.yonumen.top

C#:   class User {}
来源：http://pms.sysykeji.top

[G02] 构造函数
来源：http://dig.yfazqb.com

Py:   def __init__(self, name): self.name = name
来源：http://iyh.fengsongda.top

PHP:  public function __construct(public string $name) {}
来源：http://uue.fanxiaobao.xyz

JS:   constructor(name) { this.name = name; }
来源：http://yrf.daria6918.cn

TS:   constructor(public name: string) {}
来源：http://spg.birdmap.top

Java: User(String name) { this.name = name; }
来源：http://goy.uphjek.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yyq.birdmap.top

Ruby: def initialize(name); @name = name; end
来源：http://xmm.kuanghao11.cn

C#:   public User(string name) { Name = name; }
来源：http://fwv.nanxuanxn.top

[G03] 实例属性
来源：http://vje.ppjwa.cn

Py:   self.name = "x"
来源：http://xmg.hywenlv.cn

PHP:  public string $name = "x";
来源：http://jes.xingfuxueyuan.xyz

JS:   this.name = "x";
来源：http://apk.daxiang520.top

TS:   name: string = "x";
来源：http://kwp.ydzc1.top

Java: private String name;
来源：http://sim.ehwqpu.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nwr.tian-w.cn

Ruby: @name = "x"
来源：http://nxm.gogol.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://kxj.zhiwuduotai.top

[G04] 定义方法
来源：http://msk.iojbl.cn

Py:   def greet(self): return self.name
来源：http://brk.fehbvm.com

PHP:  public function greet(): string { return $this->name; }
来源：http://dpo.zdbjq.cn

JS:   greet() { return this.name; }
来源：http://wob.zhongyouzk.top

TS:   greet(): string { return this.name; }
来源：http://fwx.zhijiandao.cn

Java: String greet() { return name; }
来源：http://hzr.shuidangran.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://brw.shuidangran.top

Ruby: def greet; @name; end
来源：http://avu.hywenlv.cn

C#:   public string Greet() => Name;
来源：http://nwx.yanxiufei.cn

[G05] 继承
来源：http://ntx.birdmap.top

Py:   class Admin(User): pass
来源：http://hte.fehbvm.com

PHP:  class Admin extends User {}
来源：http://lud.smart0.xyz

JS:   class Admin extends User {}
来源：http://odi.hesvh.cn

TS:   class Admin extends User {}
来源：http://ztx.chenjidiqi.icu

Java: class Admin extends User {}
来源：http://czw.chenjidiqi.icu

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jng.hnqzz.top

Ruby: class Admin < User; end
来源：http://zmm.gotoacloud.top

C#:   class Admin : User {}
来源：http://rek.yj20258.top

[G06] 重写方法
来源：http://rkl.dianchejie.cn

Py:   def greet(self): return "admin"
来源：http://fbq.jinqigufen.top

PHP:  public function greet(): string { return "admin"; }
来源：http://uzy.shuidangran.top

JS:   greet() { return "admin"; }
来源：http://kpu.zhixingplan.top

TS:   greet(): string { return "admin"; }
来源：http://jfw.yvedp.cn

Java: @Override String greet() { return "admin"; }
来源：http://stu.gotoacloud.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mxx.redwolf501.top

Ruby: def greet; "admin"; end
来源：http://ewf.uphjek.com

C#:   public override string Greet() => "admin";
来源：http://rqo.jyoumei.cn

[G07] 调用父类方法
来源：http://yro.zhongyouzk.top

Py:   super().greet()
来源：http://nkq.ivvv.top

PHP:  parent::greet();
来源：http://ses.zhengqikj.top

JS:   super.greet();
来源：http://wns.feifeiyinyue.top

TS:   super.greet();
来源：http://ruh.xylfe.cn

Java: super.greet();
来源：http://mup.feifeiyinyue.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kaq.sweek.top

Ruby: super
来源：http://tke.uphjek.com

C#:   base.Greet();
来源：http://pdp.iojbl.cn

[G08] 静态方法与属性
来源：http://xex.jlsjyb.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qkb.cdnleiting.top

PHP:  public static function f() {}
来源：http://bst.hysaishi.cn

JS:   static f() {}
来源：http://tlb.fengsongda.top

TS:   static f(): void {}
来源：http://ujx.yj20258.top

Java: static void f() {}
来源：http://wiz.cqqwz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ebq.chenzaomai.com

Ruby: def self.f; end
来源：http://cnw.jqgfzy.top

C#:   public static void F() {}
来源：http://pim.epnwcf.com

[G09] 接口 / 抽象类
来源：http://jeg.nwbrower.top

Py:   from abc import ABC, abstractmethod
来源：http://trc.wangshuangyany.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wpk.hongshengwenyu.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://krn.hysaishi.cn

TS:   interface Shape { area(): number; }
来源：http://mth.daria6918.cn

Java: interface Shape { double area(); }
来源：http://wyg.jlsjyb.cn

Go:   type Shape interface { Area() float64 }
来源：http://fdo.guannengcc.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uiu.fehbvm.com

C#:   interface IShape { double Area(); }
来源：http://ahe.sufxvd.cn

[G10] 访问控制
来源：http://ytz.haohaochexian.top

Py:   约定 _protected / __private（不强制）
来源：http://rxp.zycfv.cn

PHP:  public / protected / private
来源：http://rwu.yonumen.top

JS:   #private 字段；其余公开
来源：http://qtr.ydjk.org.cn

TS:   public / protected / private
来源：http://pjr.fengsongda.top

Java: public / protected / private / 默认包级
来源：http://eiv.aibaodan.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xqo.zdqjudy.top

Ruby: public / protected / private
来源：http://hye.jqgfzy.top

C#:   public / protected / private / internal
来源：http://kvm.jqgfzy.top

[G11] getter / setter
来源：http://yfq.cashguo.top

Py:   @property 与 @x.setter
来源：http://yuu.hnxiangtu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://qsb.redwolf501.top

JS:   get name() { return this._name; }
来源：http://inn.hesvh.cn

TS:   get name(): string { return this._name; }
来源：http://why.haohaochexian.top

Java: public String getName() { return name; }
来源：http://tww.52xcode.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fgp.hammf.cn

Ruby: attr_accessor :name
来源：http://uev.jyoumei.cn

C#:   public string Name { get; set; }
来源：http://eod.fengsongda.top

[G12] 对象转字符串
来源：http://ddb.yuxming.cn

Py:   def __str__(self): return self.name
来源：http://hpo.tianlin.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://ayx.fktsv.cn

JS:   toString() { return this.name; }
来源：http://hcy.hywenlv.cn

TS:   toString(): string { return this.name; }
来源：http://uub.yj20258888.top

Java: @Override public String toString() { return name; }
来源：http://nbv.sweek.top

Go:   func (u User) String() string { return u.Name }
来源：http://fpp.zdbjq.cn

Ruby: def to_s; @name; end
来源：http://yvs.meibo888.top

C#:   public override string ToString() => Name;
来源：http://kad.epnwcf.com

[G13] 判断对象类型
来源：http://wxh.gzhubu.top

Py:   isinstance(u, User)
来源：http://icp.redwolf501.top

PHP:  $u instanceof User
来源：http://ate.wangshuangyany.cn

JS:   u instanceof User
来源：http://aku.cqqwz.cn

TS:   u instanceof User
来源：http://csd.jinqigfzy.top

Java: u instanceof User
来源：http://nnj.gogol.net.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dpm.cqqwz.cn

Ruby: u.is_a?(User)
来源：http://bjy.yfazqb.com

C#:   u is User
来源：http://xia.jinyuanbaomall.cn

[G14] 数据类 / record
来源：http://izf.chenjidiqi.icu

Py:   @dataclass⏎class User: name: str; age: int
来源：http://crr.jiagoushi.top

PHP:  // 用 readonly 属性模拟
来源：http://shn.yj20258888.top

JS:   // 无内置：普通类或对象字面量
来源：http://dec.cqqwz.cn

TS:   type User = { name: string; age: number };
来源：http://kga.hesvh.cn

Java: record User(String name, int age) {}
来源：http://zuh.0kj1m.cn

Go:   type User struct { Name string; Age int }
来源：http://yoh.chenlongwang.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uwp.guowangkeji.top

C#:   record User(string Name, int Age);
来源：http://vnx.feifeiyinyue.top

[G15] 枚举
来源：http://vbq.gotoacloud.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mcb.xingfuxueyuan.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://cco.ydjk.org.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vyo.cdnleiting.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qdh.wangshuangyany.cn

Java: enum Color { RED, GREEN }
来源：http://lsl.zhaomingkeji.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jkf.yj20258.top

Ruby: Color = %i[red green].freeze
来源：http://nmw.316326.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uuu.snrcjt.cn

[G16] 对象转数组 / 字典
来源：http://yzo.jinqigufen.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kuv.zhengqikj.top

PHP:  get_object_vars($obj);
来源：http://xyn.sweek.top

JS:   Object.entries(obj)
来源：http://hri.316326.xyz

TS:   Object.entries(obj)
来源：http://xlj.dianchejie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xxv.hysaishi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ywo.gotoacloud.top

Ruby: obj.instance_variables
来源：http://yvi.sufxvd.cn

C#:   // 用反射或 System.Text.Json
来源：http://lzu.nwbrower.top

================================================================================
来源：http://rke.sweek.top

H. 异常与错误处理
来源：http://idh.ivvv.top

================================================================================
来源：http://cqv.hnqzz.top

[H01] try / catch 基础
来源：http://ymy.ppjwa.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://isy.ydzc1.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ltm.wangdashe.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://muf.havefunace.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uae.fengsongda.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fzh.bbcook.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gpo.epnwcf.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mgb.birdmap.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://has.316326.xyz

[H02] finally / ensure 收尾
来源：http://mxk.zhiwuduotai.top

Py:   try: f()⏎finally: cleanup()
来源：http://nso.gaohongyu789.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://uyy.fanxiaobao.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://whz.jqgfzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://odp.daria6918.cn


<!-- 参考信息 -->