代发 wailian999

PHP:  number_format(1234567);
来源：http://yya.316326.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://vgl.nwbrower.top

TS:   (1234567).toLocaleString("en-US")
来源：http://hhx.fanxiaobao.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yqi.zycfv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vnq.zhoulong.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dvj.shzxlz.cn

C#:   1234567.ToString("N0")
来源：http://sad.xuetiantiany.cn

[E17] 首字母大写
来源：http://lgj.zhiwuduotai.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uut.gaohongyu789.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://icz.hnqzz.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wnn.nanxinkj.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qae.hfpthk.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uxw.yj202588.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ria.snrcjt.cn

Ruby: s.capitalize
来源：http://jal.yj20258888.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tln.316326.xyz

[E18] 模板占位符替换
来源：http://sfy.jlsjyb.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mcm.redwolf501.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kib.yanxiufei.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ntk.yangfankeji.com

TS:   tpl.replaceAll("{name}", name)
来源：http://umj.c1oappe.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sha.zhijiandao.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jrj.yj20258.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gjl.chenzaomai.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nhj.52xcode.cn

[E19] 多行文本按行拆分
来源：http://nqu.fzhhl.top

Py:   s.splitlines()
来源：http://mgh.hnqzz.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hmh.jiagoushi.top

JS:   s.split(/\r?\n/)
来源：http://fqp.zdqjudy.top

TS:   s.split(/\r?\n/)
来源：http://idf.ybcxt.top

Java: s.lines().toList()
来源：http://kej.quarkkingdee.top

Go:   strings.Split(s, "\n")
来源：http://rpj.gzhubu.top

Ruby: s.lines
来源：http://giv.guannengcc.top

C#:   s.Split('\n')
来源：http://iko.tian-w.cn

[E20] 判断字符串是否为空
来源：http://esc.fzhhl.top

Py:   if not s:
来源：http://tkg.tian-w.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pqc.yvedp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://exk.birdmap.top

TS:   if (s === "") {}
来源：http://bdj.tianlin.xyz

Java: if (s.isEmpty()) {}
来源：http://kxn.quarkkingdee.top

Go:   if s == "" {}
来源：http://ryg.jinghuilouyu.cn

Ruby: if s.empty?
来源：http://elz.meibo888.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tta.chenzaomai.com

[E21] 超长截断加省略号
来源：http://bpw.wangdashe.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xoq.ivvv.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tln.cucudq.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dis.chenzaomai.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vrp.sweek.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://unh.hesvh.cn

Go:   // 按 rune 判断长度后截断
来源：http://eha.jiagoushi.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tnx.dashuyun.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ano.52xcode.cn

[E22] 字节长度与字符长度
来源：http://slx.fzhhl.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sbf.zycfv.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uyb.cucudq.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://izl.hnqzz.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yhg.yueranfly.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hpe.ehwqpu.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rqb.yanxiufei.cn

Ruby: s.bytesize;  s.length
来源：http://uuy.cqqwz.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wfd.iojbl.cn

================================================================================
来源：http://dah.yuxming.cn

F. 文件与目录
来源：http://tbc.chenlongwang.top

================================================================================
来源：http://zfv.zhiwuduotai.top

[F01] 读取整个文件
来源：http://ovs.kuanghao11.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bma.gaohongyu789.top

PHP:  file_get_contents("a.txt");
来源：http://apw.tianlin.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rpc.pycfn.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jmo.vehdjk.com

Java: Files.readString(Path.of("a.txt"))
来源：http://xrp.9152youxi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cbt.hnxiangtu.top

Ruby: File.read("a.txt")
来源：http://qgh.redwolf501.top

C#:   File.ReadAllText("a.txt");
来源：http://qbd.sweek.top

[F02] 逐行读取文件
来源：http://nbd.shangyingyoupin.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gnh.sjlbkw.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://djt.daxiang520.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yqu.jianghu66.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://egs.hesvh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yby.redwolf501.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dav.cheryme.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tvy.epnwcf.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zdv.zhiwuduotai.top

[F03] 写入文件（覆盖）
来源：http://cqi.zhijiandao.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://twg.xingfuxueyuan.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://oyq.zhijiandao.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uwy.guowangkeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kal.kuanghao11.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qqf.epnwcf.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zhp.fzhhl.top

Ruby: File.write("a.txt", "hi")
来源：http://dlg.yfazqb.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qnu.haohaochexian.top

[F04] 追加写入文件
来源：http://noj.gotoacloud.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bum.cashguo.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lhb.shzxlz.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zbt.iojbl.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hhl.tian-w.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kxl.yfazqb.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nha.ctjpmb.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cjc.jlsjyb.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tqc.sxryk.cn

[F05] 判断文件或目录是否存在
来源：http://cji.cheryme.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gpx.fengsongda.top

PHP:  file_exists("a.txt");
来源：http://isj.snrcjt.cn

JS:   fs.existsSync("a.txt")
来源：http://nlz.vqdsnc.cn

TS:   fs.existsSync("a.txt")
来源：http://xmq.nanxinkj.top

Java: Files.exists(Path.of("a.txt"))
来源：http://hwp.gogol.net.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://izs.jiagoushi.top

Ruby: File.exist?("a.txt")
来源：http://enc.bjfxy.top

C#:   File.Exists("a.txt")
来源：http://qdp.hcnkem.com

[F06] 删除文件
来源：http://szo.jlsjyb.cn

Py:   os.remove("a.txt")
来源：http://hrx.meibo888.top

PHP:  unlink("a.txt");
来源：http://sne.hnxiangtu.top

JS:   fs.unlinkSync("a.txt")
来源：http://uft.havefunace.top

TS:   fs.unlinkSync("a.txt")
来源：http://tfc.0kj1m.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tbf.gzhubu.top

Go:   os.Remove("a.txt")
来源：http://snv.jiagoushi.top

Ruby: File.delete("a.txt")
来源：http://qni.svipenyu.cn

C#:   File.Delete("a.txt");
来源：http://ycy.hywenlv.cn

[F07] 创建目录（含多级）
来源：http://hem.hcnkem.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zwk.yangfankeji.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lho.ivvv.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ngr.sweek.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://smr.sweek.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qly.sxryk.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wql.sjlbkw.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zii.daxiang520.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kpy.snrcjt.cn

[F08] 遍历目录
来源：http://kap.gzhubu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hwe.shangyingyoupin.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kek.nanxuanxn.top

JS:   fs.readdirSync("dir")
来源：http://hio.fehbvm.com

TS:   fs.readdirSync("dir")
来源：http://ksa.pengpengdd.cyou

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://aqj.vqdsnc.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fnw.wangdashe.top

Ruby: Dir.children("dir")
来源：http://bwq.cqqwz.cn

C#:   Directory.GetFiles("dir")
来源：http://cjw.xuetiantiany.cn

[F09] 获取文件大小
来源：http://lla.shuidangran.top

Py:   os.path.getsize("a.txt")
来源：http://rld.9152youxi.cn

PHP:  filesize("a.txt");
来源：http://amr.ppjwa.cn

JS:   fs.statSync("a.txt").size
来源：http://var.chenjidiqi.icu

TS:   fs.statSync("a.txt").size
来源：http://wls.yj20258.top

Java: Files.size(Path.of("a.txt"))
来源：http://gee.shanyushiyangkeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sbt.jinghuilouyu.cn

Ruby: File.size("a.txt")
来源：http://owm.mhx1999.top

C#:   new FileInfo("a.txt").Length
来源：http://wko.nanxinkj.top

[F10] 取文件扩展名 / 文件名
来源：http://vzg.andypj.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://eqi.guannengcc.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://byc.bjfxy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ooe.vqdsnc.cn

TS:   path.extname("a.txt")
来源：http://ish.gzhubu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mua.fengsongda.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://woy.hammf.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uzr.gogol.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://huq.cashguo.top

[F11] 复制与移动文件
来源：http://kll.cheryme.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kkm.yfazqb.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://too.birdmap.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mei.yvedp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ahk.zhixingplan.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kfi.smart0.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xjb.guowangkeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kyi.vehdjk.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://smj.jinyuanbaomall.cn

[F12] CSV 读写
来源：http://uqd.shuidangran.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gto.xingfuxueyuan.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://idc.fengsongda.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hfy.xuanzx.com

TS:   // 同上
来源：http://nak.shangyingyoupin.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hwk.zhoulong.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ucu.zhengqikj.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nuz.0kj1m.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dre.bbcook.cn

================================================================================
来源：http://srl.yanxiufei.cn

G. 面向对象
来源：http://xrm.jqgfzy.top

================================================================================
来源：http://ytw.guannengcc.top

[G01] 定义类
来源：http://dgn.zycfv.cn

Py:   class User: pass
来源：http://hyl.jqgufenzy.top

PHP:  class User {}
来源：http://awx.nanxuanxn.top

JS:   class User {}
来源：http://mdv.chenjidiqi.icu

TS:   class User { name: string = ""; }
来源：http://whu.aizwys.cn

Java: class User {}
来源：http://ldc.hywenlv.cn

Go:   type User struct { Name string }
来源：http://ggn.yfazqb.com

Ruby: class User; end
来源：http://iqu.yuanzhike.top

C#:   class User {}
来源：http://lsn.pengpengdd.cyou

[G02] 构造函数
来源：http://tvv.yj20258888.top

Py:   def __init__(self, name): self.name = name
来源：http://skk.jyoumei.cn

PHP:  public function __construct(public string $name) {}
来源：http://agm.hnqzz.top

JS:   constructor(name) { this.name = name; }
来源：http://ena.hesvh.cn

TS:   constructor(public name: string) {}
来源：http://gqw.ydzc1.top

Java: User(String name) { this.name = name; }
来源：http://gud.52xcode.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xul.316326.xyz

Ruby: def initialize(name); @name = name; end
来源：http://jfy.snrcjt.cn

C#:   public User(string name) { Name = name; }
来源：http://oxn.xylfe.cn

[G03] 实例属性
来源：http://jlu.xuetiantiany.cn

Py:   self.name = "x"
来源：http://xah.jqgufenzy.top

PHP:  public string $name = "x";
来源：http://ydk.xuetiantiany.cn

JS:   this.name = "x";
来源：http://pqs.wangshuangyany.cn

TS:   name: string = "x";
来源：http://phf.ydjk.org.cn

Java: private String name;
来源：http://dht.havefunace.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rde.nwbrower.top

Ruby: @name = "x"
来源：http://cmv.aibaodan.cn

C#:   public string Name { get; set; } = "x";
来源：http://far.tianlin.xyz

[G04] 定义方法
来源：http://zfo.havefunace.top

Py:   def greet(self): return self.name
来源：http://dsl.chenjidiqi.icu

PHP:  public function greet(): string { return $this->name; }
来源：http://oai.zdqjudy.top

JS:   greet() { return this.name; }
来源：http://usu.ydjk.org.cn

TS:   greet(): string { return this.name; }
来源：http://jfy.cdnleiting.top

Java: String greet() { return name; }
来源：http://xwq.sjlbkw.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nkb.fengsongda.top

Ruby: def greet; @name; end
来源：http://rfq.zhaomingkeji.xyz

C#:   public string Greet() => Name;
来源：http://esv.tian-w.cn

[G05] 继承
来源：http://man.sysykeji.top

Py:   class Admin(User): pass
来源：http://cjx.zdbjq.cn

PHP:  class Admin extends User {}
来源：http://rsg.dashuyun.cn

JS:   class Admin extends User {}
来源：http://jln.chenzaomai.com

TS:   class Admin extends User {}
来源：http://ycy.gotoacloud.top

Java: class Admin extends User {}
来源：http://utm.zhaomingkeji.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ynr.gaohongyu789.top

Ruby: class Admin < User; end
来源：http://vup.sysykeji.top

C#:   class Admin : User {}
来源：http://anj.yongpay.top

[G06] 重写方法
来源：http://edd.cheryme.top

Py:   def greet(self): return "admin"
来源：http://ngl.jinqigfzy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://nie.sysykeji.top

JS:   greet() { return "admin"; }
来源：http://oqn.shanyushiyangkeji.top

TS:   greet(): string { return "admin"; }
来源：http://iew.feifeiyinyue.top

Java: @Override String greet() { return "admin"; }
来源：http://jju.gotoacloud.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rxt.52xcode.cn

Ruby: def greet; "admin"; end
来源：http://pko.smart0.xyz

C#:   public override string Greet() => "admin";
来源：http://uum.ywan-chungtsiang.top

[G07] 调用父类方法
来源：http://igh.zhoulong.xyz

Py:   super().greet()
来源：http://okc.gotoacloud.top

PHP:  parent::greet();
来源：http://pkh.ivvv.top

JS:   super.greet();
来源：http://iaz.vehdjk.com

TS:   super.greet();
来源：http://izv.yueranfly.top

Java: super.greet();
来源：http://jps.xziqi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tkq.zhengqikj.top

Ruby: super
来源：http://wkb.jinqigfzy.top

C#:   base.Greet();
来源：http://ysb.zhixingplan.top

[G08] 静态方法与属性
来源：http://ril.yvedp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jiw.zhijiandao.cn

PHP:  public static function f() {}
来源：http://juo.chenjidiqi.icu

JS:   static f() {}
来源：http://vvq.mhx1999.top

TS:   static f(): void {}
来源：http://nfr.xinyue.icu

Java: static void f() {}
来源：http://srn.sufxvd.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hod.nanxinkj.top

Ruby: def self.f; end
来源：http://ide.fzhhl.top

C#:   public static void F() {}
来源：http://awg.nanxuanxn.top

[G09] 接口 / 抽象类
来源：http://gjm.yonumen.top

Py:   from abc import ABC, abstractmethod
来源：http://hyb.tian-w.cn

PHP:  interface Shape { public function area(): float; }
来源：http://tkm.nwbrower.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://cgw.52xcode.cn

TS:   interface Shape { area(): number; }
来源：http://rgi.fehbvm.com

Java: interface Shape { double area(); }
来源：http://hpr.iojbl.cn

Go:   type Shape interface { Area() float64 }
来源：http://cin.vehdjk.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://omh.ctjpmb.com

C#:   interface IShape { double Area(); }
来源：http://utm.0kj1m.cn

[G10] 访问控制
来源：http://ztd.cheryme.top

Py:   约定 _protected / __private（不强制）
来源：http://psr.pycfn.com

PHP:  public / protected / private
来源：http://zoo.dianchejie.cn

JS:   #private 字段；其余公开
来源：http://dhl.hammf.cn

TS:   public / protected / private
来源：http://icw.yanxiufei.cn

Java: public / protected / private / 默认包级
来源：http://lgk.zhixingplan.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://zwk.jiagoushi.top

Ruby: public / protected / private
来源：http://lic.vqdsnc.cn

C#:   public / protected / private / internal
来源：http://xkz.cdnleiting.top

[G11] getter / setter
来源：http://rgi.epnwcf.com

Py:   @property 与 @x.setter
来源：http://xle.cucudq.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vsv.vehdjk.com

JS:   get name() { return this._name; }
来源：http://xst.zhongyouzk.top

TS:   get name(): string { return this._name; }
来源：http://oij.haohaochexian.top

Java: public String getName() { return name; }
来源：http://hjk.bbcook.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fig.fktsv.cn

Ruby: attr_accessor :name
来源：http://gej.epnwcf.com

C#:   public string Name { get; set; }
来源：http://fhk.daria6918.cn

[G12] 对象转字符串
来源：http://wvx.tianlin.xyz

Py:   def __str__(self): return self.name
来源：http://zmp.jinyuanbaomall.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jko.zdbjq.cn

JS:   toString() { return this.name; }
来源：http://yso.sufxvd.cn

TS:   toString(): string { return this.name; }
来源：http://wcu.shzxlz.cn

Java: @Override public String toString() { return name; }
来源：http://qlm.zycfv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zqr.jiagoushi.top

Ruby: def to_s; @name; end
来源：http://ftw.yj20258888.top

C#:   public override string ToString() => Name;
来源：http://ntn.ctjpmb.com

[G13] 判断对象类型
来源：http://sds.zhaomingkeji.xyz

Py:   isinstance(u, User)
来源：http://tju.wangdashe.top

PHP:  $u instanceof User
来源：http://ghu.jinyuanbaomall.cn

JS:   u instanceof User
来源：http://kxo.shanyushiyangtech.top

TS:   u instanceof User
来源：http://xlb.jqgfzy.top

Java: u instanceof User
来源：http://fgd.zdbjq.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pvu.quarkkingdee.top

Ruby: u.is_a?(User)
来源：http://nyn.hesvh.cn

C#:   u is User
来源：http://zkx.sufxvd.cn

[G14] 数据类 / record
来源：http://vds.jianghu66.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kkk.aizwys.cn

PHP:  // 用 readonly 属性模拟
来源：http://hsz.epnwcf.com

JS:   // 无内置：普通类或对象字面量
来源：http://yha.daxiang520.top

TS:   type User = { name: string; age: number };
来源：http://szf.hfpthk.cn

Java: record User(String name, int age) {}
来源：http://tye.yj20258.top

Go:   type User struct { Name string; Age int }
来源：http://ukd.guannengcc.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ngu.yueranfly.top


<!-- 参考信息 -->