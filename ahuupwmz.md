代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://vyq.pengpengdd.cyou

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hxs.smart0.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ewo.xingfuxueyuan.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://euw.aizwys.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://brn.birdmap.top

[E19] 多行文本按行拆分
来源：http://oet.tanke756.top

Py:   s.splitlines()
来源：http://svk.yongpay.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fnf.daria6918.cn

JS:   s.split(/\r?\n/)
来源：http://bun.0kj1m.cn

TS:   s.split(/\r?\n/)
来源：http://ttv.zhengqikj.top

Java: s.lines().toList()
来源：http://ujf.vqdsnc.cn

Go:   strings.Split(s, "\n")
来源：http://soo.tanke756.top

Ruby: s.lines
来源：http://soa.sufxvd.cn

C#:   s.Split('\n')
来源：http://oyd.havefunace.top

[E20] 判断字符串是否为空
来源：http://qeb.hnqzz.top

Py:   if not s:
来源：http://rat.ehwqpu.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://myb.shzxlz.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wkn.zhengqikj.top

TS:   if (s === "") {}
来源：http://twf.ctjpmb.com

Java: if (s.isEmpty()) {}
来源：http://qdr.cdnleiting.top

Go:   if s == "" {}
来源：http://spy.tarul.cn

Ruby: if s.empty?
来源：http://ldg.ivvv.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mvb.redwolf501.top

[E21] 超长截断加省略号
来源：http://zlx.jinghuilouyu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yhi.chenjidiqi.icu

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hgh.fengsongda.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pvx.jinqigfzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://luq.yj202588.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://aiv.jqgfzy.top

Go:   // 按 rune 判断长度后截断
来源：http://lez.zhengqikj.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tle.dashuyun.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ifm.hongshengwenyu.top

[E22] 字节长度与字符长度
来源：http://hnf.hcnkem.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yjz.shanyushiyangkeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kqv.yueranfly.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://juj.fzhhl.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jte.jqgufenzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cgo.yj20258.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hji.wangdashe.top

Ruby: s.bytesize;  s.length
来源：http://rjj.jiagoushi.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ksw.yuxming.cn

================================================================================
来源：http://yly.redwolf501.top

F. 文件与目录
来源：http://xvu.xinyue.icu

================================================================================
来源：http://shb.sjlbkw.cn

[F01] 读取整个文件
来源：http://fdm.yonumen.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bbr.pycfn.com

PHP:  file_get_contents("a.txt");
来源：http://fsk.ctjpmb.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tzs.ywan-chungtsiang.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qbg.yongpay.top

Java: Files.readString(Path.of("a.txt"))
来源：http://cpf.fengsongda.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hza.jinyuanbaomall.cn

Ruby: File.read("a.txt")
来源：http://qvq.sufxvd.cn

C#:   File.ReadAllText("a.txt");
来源：http://rbu.ehwqpu.com

[F02] 逐行读取文件
来源：http://zij.andypj.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gzu.hammf.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://udl.zhixingplan.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nqi.yanxiufei.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ldz.yongpay.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vrj.birdmap.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bmo.zhengqikj.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hbk.aizwys.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gub.uphjek.com

[F03] 写入文件（覆盖）
来源：http://zwm.sjlbkw.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://goz.sysykeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://nkn.yuanzhike.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qln.yuxming.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vnv.tanke756.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rdn.nanxinkj.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nbn.tianlin.xyz

Ruby: File.write("a.txt", "hi")
来源：http://qez.redwolf501.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wbh.aizwys.cn

[F04] 追加写入文件
来源：http://cbx.zhiwuduotai.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fct.guannengcc.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dld.uphjek.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://thj.sjlbkw.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fow.c1oappe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hpm.wangshuangyany.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qwg.chenjidiqi.icu

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://egr.tarul.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cjf.vqdsnc.cn

[F05] 判断文件或目录是否存在
来源：http://znh.zhengqikj.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qdv.nwbrower.top

PHP:  file_exists("a.txt");
来源：http://dce.vehdjk.com

JS:   fs.existsSync("a.txt")
来源：http://vkx.sysykeji.top

TS:   fs.existsSync("a.txt")
来源：http://ath.redwolf501.top

Java: Files.exists(Path.of("a.txt"))
来源：http://val.shanyushiyangtech.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vzd.fktsv.cn

Ruby: File.exist?("a.txt")
来源：http://qnp.shanyushiyangtech.top

C#:   File.Exists("a.txt")
来源：http://bew.pycfn.com

[F06] 删除文件
来源：http://imv.yongpay.top

Py:   os.remove("a.txt")
来源：http://dce.yj202588.top

PHP:  unlink("a.txt");
来源：http://yzf.shzxlz.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hxz.smart0.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://txi.sjlbkw.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qaj.jqgufenzy.top

Go:   os.Remove("a.txt")
来源：http://xzx.xuetiantiany.cn

Ruby: File.delete("a.txt")
来源：http://xpw.aibaodan.cn

C#:   File.Delete("a.txt");
来源：http://vnn.shanyushiyangtech.top

[F07] 创建目录（含多级）
来源：http://znm.yanxiufei.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://arm.xylfe.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nnn.haohaochexian.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hbw.zhixingplan.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://akm.cheryme.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ltz.smart0.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://juv.hnxiangtu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ztv.xingfuxueyuan.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zpb.gotoacloud.top

[F08] 遍历目录
来源：http://vgg.jianghu66.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://kbo.snrcjt.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dts.yongpay.top

JS:   fs.readdirSync("dir")
来源：http://diy.cdnleiting.top

TS:   fs.readdirSync("dir")
来源：http://uct.fzhhl.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hiw.smart0.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://twz.yongpay.top

Ruby: Dir.children("dir")
来源：http://jig.fanxiaobao.xyz

C#:   Directory.GetFiles("dir")
来源：http://elp.aizwys.cn

[F09] 获取文件大小
来源：http://ogq.cucudq.cn

Py:   os.path.getsize("a.txt")
来源：http://igq.yanxiufei.cn

PHP:  filesize("a.txt");
来源：http://ufz.vqdsnc.cn

JS:   fs.statSync("a.txt").size
来源：http://tdq.epnwcf.com

TS:   fs.statSync("a.txt").size
来源：http://kgw.andypj.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://dfc.xinyue.icu

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nun.jqgfzy.top

Ruby: File.size("a.txt")
来源：http://fel.fengsongda.top

C#:   new FileInfo("a.txt").Length
来源：http://ans.xuetiantiany.cn

[F10] 取文件扩展名 / 文件名
来源：http://vyu.zhijiandao.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fgw.chenjidiqi.icu

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tkq.xuetiantiany.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sts.zhaomingkeji.xyz

TS:   path.extname("a.txt")
来源：http://bvm.shanyushiyangtech.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jae.ybcxt.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://too.daxiang520.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rke.havefunace.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rov.ctjpmb.com

[F11] 复制与移动文件
来源：http://leb.jqgufenzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cti.cucudq.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vnq.cucudq.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wil.ctjpmb.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uyj.c1oappe.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vae.sufxvd.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pto.guowangkeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rox.sxryk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ulh.meibo888.top

[F12] CSV 读写
来源：http://hjs.shangyingyoupin.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nma.zhoulong.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bdv.sjlbkw.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yke.vqdsnc.cn

TS:   // 同上
来源：http://eaa.xinyue.icu

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ipp.havefunace.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lmj.wangdashe.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fjg.dashuyun.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ymy.vehdjk.com

================================================================================
来源：http://gqq.ppjwa.cn

G. 面向对象
来源：http://jrc.vehdjk.com

================================================================================
来源：http://adg.ydzc1.top

[G01] 定义类
来源：http://ims.hammf.cn

Py:   class User: pass
来源：http://mhx.yanxiufei.cn

PHP:  class User {}
来源：http://gzc.cucudq.cn

JS:   class User {}
来源：http://pej.zhijiandao.cn

TS:   class User { name: string = ""; }
来源：http://awx.gaohongyu789.top

Java: class User {}
来源：http://pfp.nanxinkj.top

Go:   type User struct { Name string }
来源：http://gte.gotoacloud.top

Ruby: class User; end
来源：http://pub.yfazqb.com

C#:   class User {}
来源：http://qoj.zhijiandao.cn

[G02] 构造函数
来源：http://wjr.ivvv.top

Py:   def __init__(self, name): self.name = name
来源：http://ojm.shuidangran.top

PHP:  public function __construct(public string $name) {}
来源：http://hwn.cashguo.top

JS:   constructor(name) { this.name = name; }
来源：http://ppd.316326.xyz

TS:   constructor(public name: string) {}
来源：http://gqn.shzxlz.cn

Java: User(String name) { this.name = name; }
来源：http://kvk.9152youxi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nrl.pycfn.com

Ruby: def initialize(name); @name = name; end
来源：http://krs.zhoulong.xyz

C#:   public User(string name) { Name = name; }
来源：http://tlw.bjfxy.top

[G03] 实例属性
来源：http://ebe.hywenlv.cn

Py:   self.name = "x"
来源：http://upu.yj202588.top

PHP:  public string $name = "x";
来源：http://dvr.zdqjudy.top

JS:   this.name = "x";
来源：http://gdg.hysaishi.cn

TS:   name: string = "x";
来源：http://kva.jlsjyb.cn

Java: private String name;
来源：http://jfv.jlsjyb.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uic.havefunace.top

Ruby: @name = "x"
来源：http://txt.fehbvm.com

C#:   public string Name { get; set; } = "x";
来源：http://giz.kuanghao11.cn

[G04] 定义方法
来源：http://xij.zhoulong.xyz

Py:   def greet(self): return self.name
来源：http://rfy.tanke756.top

PHP:  public function greet(): string { return $this->name; }
来源：http://xuz.cucudq.cn

JS:   greet() { return this.name; }
来源：http://rsh.yj202588.top

TS:   greet(): string { return this.name; }
来源：http://uxm.xinyue.icu

Java: String greet() { return name; }
来源：http://clc.shanyushiyangkeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://jik.sufxvd.cn

Ruby: def greet; @name; end
来源：http://zwm.cqqwz.cn

C#:   public string Greet() => Name;
来源：http://xzd.smart0.xyz

[G05] 继承
来源：http://wxh.zhijiandao.cn

Py:   class Admin(User): pass
来源：http://ceq.yongpay.top

PHP:  class Admin extends User {}
来源：http://ayf.hnxiangtu.top

JS:   class Admin extends User {}
来源：http://cap.nanxuanxn.top

TS:   class Admin extends User {}
来源：http://nyy.fanxiaobao.xyz

Java: class Admin extends User {}
来源：http://wij.fktsv.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jej.sxryk.cn

Ruby: class Admin < User; end
来源：http://sjb.jqgufenzy.top

C#:   class Admin : User {}
来源：http://jnb.tarul.cn

[G06] 重写方法
来源：http://yiz.shangyingyoupin.top

Py:   def greet(self): return "admin"
来源：http://iwz.jyoumei.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://eyd.tian-w.cn

JS:   greet() { return "admin"; }
来源：http://iyt.jqgfzy.top

TS:   greet(): string { return "admin"; }
来源：http://idq.xziqi.cn

Java: @Override String greet() { return "admin"; }
来源：http://ruv.zhoulong.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fxj.nanxinkj.top

Ruby: def greet; "admin"; end
来源：http://old.sysykeji.top

C#:   public override string Greet() => "admin";
来源：http://jhd.kuanghao11.cn

[G07] 调用父类方法
来源：http://qcy.xziqi.cn

Py:   super().greet()
来源：http://ixn.chenzaomai.com

PHP:  parent::greet();
来源：http://nml.zycfv.cn

JS:   super.greet();
来源：http://itv.jyoumei.cn

TS:   super.greet();
来源：http://aaj.epnwcf.com

Java: super.greet();
来源：http://zbb.svipenyu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pmv.aizwys.cn

Ruby: super
来源：http://rfu.xuanzx.com

C#:   base.Greet();
来源：http://lfg.jianghu66.top

[G08] 静态方法与属性
来源：http://trs.yonumen.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kdl.nwbrower.top

PHP:  public static function f() {}
来源：http://fhu.jinqigfzy.top

JS:   static f() {}
来源：http://gmo.birdmap.top

TS:   static f(): void {}
来源：http://nim.xinyue.icu

Java: static void f() {}
来源：http://tlh.haohaochexian.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://say.cashguo.top

Ruby: def self.f; end
来源：http://elb.havefunace.top

C#:   public static void F() {}
来源：http://sdn.mhx1999.top

[G09] 接口 / 抽象类
来源：http://pnz.guowangkeji.top

Py:   from abc import ABC, abstractmethod
来源：http://sec.fehbvm.com

PHP:  interface Shape { public function area(): float; }
来源：http://cey.fehbvm.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://dgd.fktsv.cn

TS:   interface Shape { area(): number; }
来源：http://ubz.aibaodan.cn

Java: interface Shape { double area(); }
来源：http://lwn.ehwqpu.com

Go:   type Shape interface { Area() float64 }
来源：http://wse.zhongyouzk.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dfl.smart0.xyz

C#:   interface IShape { double Area(); }
来源：http://poz.fktsv.cn

[G10] 访问控制
来源：http://fho.yongpay.top

Py:   约定 _protected / __private（不强制）
来源：http://rrp.cdnleiting.top

PHP:  public / protected / private
来源：http://aov.shanyushiyangtech.top

JS:   #private 字段；其余公开
来源：http://tcf.sxryk.cn

TS:   public / protected / private
来源：http://hmy.xylfe.cn

Java: public / protected / private / 默认包级
来源：http://tnr.chenlongwang.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://vum.yj20258888.top

Ruby: public / protected / private
来源：http://oqg.iojbl.cn

C#:   public / protected / private / internal
来源：http://teo.cashguo.top

[G11] getter / setter
来源：http://ftg.zhiwuduotai.top

Py:   @property 与 @x.setter
来源：http://adn.cqqwz.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qwa.zhengqikj.top

JS:   get name() { return this._name; }
来源：http://kdd.jinghuilouyu.cn

TS:   get name(): string { return this._name; }
来源：http://lac.jinqigfzy.top

Java: public String getName() { return name; }
来源：http://ktx.yvedp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://lnq.yvedp.cn

Ruby: attr_accessor :name
来源：http://rxs.zhixingplan.top

C#:   public string Name { get; set; }
来源：http://jxj.quarkkingdee.top

[G12] 对象转字符串
来源：http://reh.jyoumei.cn

Py:   def __str__(self): return self.name
来源：http://pkt.9152youxi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://iep.nwbrower.top

JS:   toString() { return this.name; }
来源：http://smg.ybcxt.top

TS:   toString(): string { return this.name; }
来源：http://mnx.wangdashe.top

Java: @Override public String toString() { return name; }
来源：http://pjr.jinqigufen.top

Go:   func (u User) String() string { return u.Name }
来源：http://llt.jqgfzy.top

Ruby: def to_s; @name; end
来源：http://pvm.smart0.xyz

C#:   public override string ToString() => Name;
来源：http://fxc.ydjk.org.cn

[G13] 判断对象类型
来源：http://qzc.hammf.cn

Py:   isinstance(u, User)
来源：http://xir.xziqi.cn

PHP:  $u instanceof User
来源：http://qtm.fktsv.cn

JS:   u instanceof User
来源：http://krk.chenzaomai.com

TS:   u instanceof User
来源：http://qgr.nanxinkj.top

Java: u instanceof User
来源：http://wfr.zhiwuduotai.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://fjc.sysykeji.top

Ruby: u.is_a?(User)
来源：http://nqe.jqgufenzy.top

C#:   u is User
来源：http://ojp.svipenyu.cn

[G14] 数据类 / record
来源：http://whq.zycfv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tph.ppjwa.cn

PHP:  // 用 readonly 属性模拟
来源：http://wuq.aibaodan.cn

JS:   // 无内置：普通类或对象字面量
来源：http://eej.hongshengwenyu.top

TS:   type User = { name: string; age: number };
来源：http://pkr.wangdashe.top

Java: record User(String name, int age) {}
来源：http://fps.yuxming.cn

Go:   type User struct { Name string; Age int }
来源：http://oes.zhiwuduotai.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mbj.fktsv.cn

C#:   record User(string Name, int Age);
来源：http://zpj.316326.xyz

[G15] 枚举
来源：http://nqu.vehdjk.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cji.pengpengdd.cyou

PHP:  enum Color: string { case Red = "red"; }
来源：http://pgr.iojbl.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fzc.jinyuanbaomall.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ifm.smart0.xyz

Java: enum Color { RED, GREEN }
来源：http://ajd.ppjwa.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qmt.shangyingyoupin.top

Ruby: Color = %i[red green].freeze
来源：http://cht.hfpthk.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://syo.xylfe.cn

[G16] 对象转数组 / 字典
来源：http://ggp.yj20258888.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tir.ivvv.top

PHP:  get_object_vars($obj);
来源：http://sjv.zhijiandao.cn

JS:   Object.entries(obj)
来源：http://gjk.yj20258888.top

TS:   Object.entries(obj)
来源：http://mvr.bjfxy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fbs.zycfv.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://khu.xuanzx.com

Ruby: obj.instance_variables
来源：http://szg.ehwqpu.com

C#:   // 用反射或 System.Text.Json
来源：http://gxt.fengsongda.top

================================================================================
来源：http://lld.vehdjk.com


<!-- 参考信息 -->