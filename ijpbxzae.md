代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fjl.ybcxt.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tkn.tianlin.xyz

[E16] 数字千分位
来源：http://gcy.daxiang520.top

Py:   f"{1234567:,}"
来源：http://oso.hnxiangtu.top

PHP:  number_format(1234567);
来源：http://coo.gaohongyu789.top

JS:   (1234567).toLocaleString("en-US")
来源：http://plz.shanyushiyangtech.top

TS:   (1234567).toLocaleString("en-US")
来源：http://dyu.zhixingplan.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wlr.pengpengdd.cyou

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://opo.hfpthk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bpm.tarul.cn

C#:   1234567.ToString("N0")
来源：http://tdb.zhaomingkeji.xyz

[E17] 首字母大写
来源：http://nch.zhoulong.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nzw.hysaishi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://kjw.zycfv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://epg.jinyuanbaomall.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://smr.wangshuangyany.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lsb.fktsv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://orq.sjlbkw.cn

Ruby: s.capitalize
来源：http://kpw.shzxlz.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dfk.zhixingplan.top

[E18] 模板占位符替换
来源：http://rwl.daxiang520.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hir.zdqjudy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nag.smart0.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://abf.yfazqb.com

TS:   tpl.replaceAll("{name}", name)
来源：http://fun.andypj.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pvc.316326.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nno.vehdjk.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gyq.haohaochexian.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://skz.smart0.xyz

[E19] 多行文本按行拆分
来源：http://tgv.chenlongwang.top

Py:   s.splitlines()
来源：http://hqp.cqqwz.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uza.tianlin.xyz

JS:   s.split(/\r?\n/)
来源：http://eej.yj20258.top

TS:   s.split(/\r?\n/)
来源：http://hfu.zycfv.cn

Java: s.lines().toList()
来源：http://fqb.zhiwuduotai.top

Go:   strings.Split(s, "\n")
来源：http://stl.xylfe.cn

Ruby: s.lines
来源：http://bhf.dashuyun.cn

C#:   s.Split('\n')
来源：http://wtk.xuetiantiany.cn

[E20] 判断字符串是否为空
来源：http://sui.fengsongda.top

Py:   if not s:
来源：http://eii.hywenlv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jnn.yfazqb.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hku.yuanzhike.top

TS:   if (s === "") {}
来源：http://eqi.zhijiandao.cn

Java: if (s.isEmpty()) {}
来源：http://uvd.chenjidiqi.icu

Go:   if s == "" {}
来源：http://nqd.tanke756.top

Ruby: if s.empty?
来源：http://ffe.jqgfzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nkl.nanxinkj.top

[E21] 超长截断加省略号
来源：http://rlv.nanxuanxn.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://del.guowangkeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cog.c1oappe.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://feh.vehdjk.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uud.fanxiaobao.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hln.zdqjudy.top

Go:   // 按 rune 判断长度后截断
来源：http://exu.xylfe.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://shx.ybcxt.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://csu.chenjidiqi.icu

[E22] 字节长度与字符长度
来源：http://pvj.andypj.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mar.svipenyu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ash.jiagoushi.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hum.dianchejie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hug.guowangkeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yqs.sxryk.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zmn.hongshengwenyu.top

Ruby: s.bytesize;  s.length
来源：http://srd.hammf.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fca.shangyingyoupin.top

================================================================================
来源：http://etb.hfpthk.cn

F. 文件与目录
来源：http://kxv.zhoulong.xyz

================================================================================
来源：http://jxz.aizwys.cn

[F01] 读取整个文件
来源：http://mpp.chenlongwang.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://beg.xylfe.cn

PHP:  file_get_contents("a.txt");
来源：http://hto.yonumen.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jby.shangyingyoupin.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jki.chenlongwang.top

Java: Files.readString(Path.of("a.txt"))
来源：http://uwr.iojbl.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vdh.zhoulong.xyz

Ruby: File.read("a.txt")
来源：http://xso.yuanzhike.top

C#:   File.ReadAllText("a.txt");
来源：http://ole.sxryk.cn

[F02] 逐行读取文件
来源：http://iqo.chenlongwang.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wsg.zhongyouzk.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mdi.xylfe.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kpe.jiagoushi.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yvp.tian-w.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wfl.hywenlv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qtl.cashguo.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dth.yfazqb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fed.havefunace.top

[F03] 写入文件（覆盖）
来源：http://mjv.snrcjt.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mzi.jinqigfzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://bgn.redwolf501.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ysf.cdnleiting.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bap.nwbrower.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ghs.shuidangran.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://buv.smart0.xyz

Ruby: File.write("a.txt", "hi")
来源：http://vab.yonumen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://znu.hnqzz.top

[F04] 追加写入文件
来源：http://mqj.zhengqikj.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uci.yvedp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fzd.feifeiyinyue.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oac.9152youxi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://six.shuidangran.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://opo.gzhubu.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qja.wangdashe.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vrn.tian-w.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gqq.zycfv.cn

[F05] 判断文件或目录是否存在
来源：http://pgr.sxryk.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mbh.daria6918.cn

PHP:  file_exists("a.txt");
来源：http://uxh.316326.xyz

JS:   fs.existsSync("a.txt")
来源：http://luw.shanyushiyangkeji.top

TS:   fs.existsSync("a.txt")
来源：http://ysi.ydjk.org.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pdm.vehdjk.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mrz.aizwys.cn

Ruby: File.exist?("a.txt")
来源：http://mqu.yfazqb.com

C#:   File.Exists("a.txt")
来源：http://esn.svipenyu.cn

[F06] 删除文件
来源：http://vla.tianlin.xyz

Py:   os.remove("a.txt")
来源：http://pzb.jinghuilouyu.cn

PHP:  unlink("a.txt");
来源：http://lyr.9152youxi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ila.jinyuanbaomall.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bwf.sxryk.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://luv.yonumen.top

Go:   os.Remove("a.txt")
来源：http://nsn.jianghu66.top

Ruby: File.delete("a.txt")
来源：http://pkd.daxiang520.top

C#:   File.Delete("a.txt");
来源：http://unl.jyoumei.cn

[F07] 创建目录（含多级）
来源：http://qqv.smart0.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://edn.ywan-chungtsiang.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lmz.gotoacloud.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nue.yj20258.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hds.fengsongda.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xsb.jinyuanbaomall.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ynw.0kj1m.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mvy.cashguo.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ofs.iojbl.cn

[F08] 遍历目录
来源：http://wzp.epnwcf.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://ihl.zhaomingkeji.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vma.zhoulong.xyz

JS:   fs.readdirSync("dir")
来源：http://uzc.xuetiantiany.cn

TS:   fs.readdirSync("dir")
来源：http://jtr.chenlongwang.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tpr.zdqjudy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ivm.shuidangran.top

Ruby: Dir.children("dir")
来源：http://xmn.gaohongyu789.top

C#:   Directory.GetFiles("dir")
来源：http://ayn.fzhhl.top

[F09] 获取文件大小
来源：http://qkf.ybcxt.top

Py:   os.path.getsize("a.txt")
来源：http://ijv.guannengcc.top

PHP:  filesize("a.txt");
来源：http://aon.shanyushiyangkeji.top

JS:   fs.statSync("a.txt").size
来源：http://hjv.jqgfzy.top

TS:   fs.statSync("a.txt").size
来源：http://wpx.sweek.top

Java: Files.size(Path.of("a.txt"))
来源：http://ybz.jqgufenzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wnn.yangfankeji.com

Ruby: File.size("a.txt")
来源：http://xzz.yj20258.top

C#:   new FileInfo("a.txt").Length
来源：http://lrs.meibo888.top

[F10] 取文件扩展名 / 文件名
来源：http://xct.ppjwa.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ivu.yj20258.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://loa.kuanghao11.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ixy.daxiang520.top

TS:   path.extname("a.txt")
来源：http://psi.meibo888.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://poa.vehdjk.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ykz.chenzaomai.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://syr.zhongyouzk.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://txi.zhoulong.xyz

[F11] 复制与移动文件
来源：http://wtq.hfpthk.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pde.sxryk.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qdv.hammf.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pky.cqqwz.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jpf.wangdashe.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jlu.ehwqpu.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hbk.chenjidiqi.icu

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qoq.zycfv.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wdc.zhoulong.xyz

[F12] CSV 读写
来源：http://jbn.yonumen.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cmk.jianghu66.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tps.daria6918.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://iak.hammf.cn

TS:   // 同上
来源：http://uny.jinyuanbaomall.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qon.sysykeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://uej.xingfuxueyuan.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uvb.tian-w.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://meg.wangshuangyany.cn

================================================================================
来源：http://klt.guannengcc.top

G. 面向对象
来源：http://nhn.jlsjyb.cn

================================================================================
来源：http://nai.yongpay.top

[G01] 定义类
来源：http://qbd.yvedp.cn

Py:   class User: pass
来源：http://mrp.zhongyouzk.top

PHP:  class User {}
来源：http://hkz.xziqi.cn

JS:   class User {}
来源：http://tsp.jyoumei.cn

TS:   class User { name: string = ""; }
来源：http://trd.ehwqpu.com

Java: class User {}
来源：http://hnn.jinqigufen.top

Go:   type User struct { Name string }
来源：http://ttw.gzhubu.top

Ruby: class User; end
来源：http://nqp.cashguo.top

C#:   class User {}
来源：http://odb.xylfe.cn

[G02] 构造函数
来源：http://fdz.cqqwz.cn

Py:   def __init__(self, name): self.name = name
来源：http://dbd.birdmap.top

PHP:  public function __construct(public string $name) {}
来源：http://mue.snrcjt.cn

JS:   constructor(name) { this.name = name; }
来源：http://rik.gaohongyu789.top

TS:   constructor(public name: string) {}
来源：http://rnt.yj20258.top

Java: User(String name) { this.name = name; }
来源：http://krh.ivvv.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qml.dianchejie.cn

Ruby: def initialize(name); @name = name; end
来源：http://zdj.tarul.cn

C#:   public User(string name) { Name = name; }
来源：http://hby.xziqi.cn

[G03] 实例属性
来源：http://dtw.hammf.cn

Py:   self.name = "x"
来源：http://vbx.shanyushiyangtech.top

PHP:  public string $name = "x";
来源：http://aru.yonumen.top

JS:   this.name = "x";
来源：http://ysi.316326.xyz

TS:   name: string = "x";
来源：http://qrv.xylfe.cn

Java: private String name;
来源：http://rxo.wangdashe.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fdk.chenzaomai.com

Ruby: @name = "x"
来源：http://muz.yj20258.top

C#:   public string Name { get; set; } = "x";
来源：http://yue.zdqjudy.top

[G04] 定义方法
来源：http://pex.tanke756.top

Py:   def greet(self): return self.name
来源：http://itw.yj20258.top

PHP:  public function greet(): string { return $this->name; }
来源：http://pio.zdbjq.cn

JS:   greet() { return this.name; }
来源：http://hjz.daria6918.cn

TS:   greet(): string { return this.name; }
来源：http://msa.shangyingyoupin.top

Java: String greet() { return name; }
来源：http://yxw.cqqwz.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://not.sjlbkw.cn

Ruby: def greet; @name; end
来源：http://oza.zhixingplan.top

C#:   public string Greet() => Name;
来源：http://tve.gaohongyu789.top

[G05] 继承
来源：http://jfv.cheryme.top

Py:   class Admin(User): pass
来源：http://kcl.shzxlz.cn

PHP:  class Admin extends User {}
来源：http://xeb.zycfv.cn

JS:   class Admin extends User {}
来源：http://zte.cdnleiting.top

TS:   class Admin extends User {}
来源：http://zyj.yuanzhike.top

Java: class Admin extends User {}
来源：http://hmt.zhijiandao.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zby.yuanzhike.top

Ruby: class Admin < User; end
来源：http://ery.sufxvd.cn

C#:   class Admin : User {}
来源：http://zel.xuetiantiany.cn

[G06] 重写方法
来源：http://jlb.aibaodan.cn

Py:   def greet(self): return "admin"
来源：http://ybl.52xcode.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qzd.pengpengdd.cyou

JS:   greet() { return "admin"; }
来源：http://klg.shuidangran.top

TS:   greet(): string { return "admin"; }
来源：http://tys.meibo888.top

Java: @Override String greet() { return "admin"; }
来源：http://wqi.jyoumei.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dao.chenlongwang.top

Ruby: def greet; "admin"; end
来源：http://fnw.wangdashe.top

C#:   public override string Greet() => "admin";
来源：http://nzx.pengpengdd.cyou

[G07] 调用父类方法
来源：http://moy.jyoumei.cn

Py:   super().greet()
来源：http://fnl.gogol.net.cn

PHP:  parent::greet();
来源：http://mpk.ivvv.top

JS:   super.greet();
来源：http://wrb.zhongyouzk.top

TS:   super.greet();
来源：http://yuh.vqdsnc.cn

Java: super.greet();
来源：http://yuo.dashuyun.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://iek.jianghu66.top

Ruby: super
来源：http://jrw.jqgufenzy.top

C#:   base.Greet();
来源：http://oio.yj202588.top

[G08] 静态方法与属性
来源：http://rzx.aibaodan.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://npi.zhiwuduotai.top

PHP:  public static function f() {}
来源：http://clg.cashguo.top

JS:   static f() {}
来源：http://fhs.yuxming.cn

TS:   static f(): void {}
来源：http://uaw.birdmap.top

Java: static void f() {}
来源：http://bnc.hesvh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zkt.shzxlz.cn

Ruby: def self.f; end
来源：http://kpk.zhongyouzk.top

C#:   public static void F() {}
来源：http://ajr.fzhhl.top

[G09] 接口 / 抽象类
来源：http://wxr.chenjidiqi.icu

Py:   from abc import ABC, abstractmethod
来源：http://aei.meibo888.top

PHP:  interface Shape { public function area(): float; }
来源：http://fbx.hfpthk.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jtt.mhx1999.top

TS:   interface Shape { area(): number; }
来源：http://xtj.redwolf501.top

Java: interface Shape { double area(); }
来源：http://sem.cheryme.top

Go:   type Shape interface { Area() float64 }
来源：http://fxs.ivvv.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qyu.jinqigufen.top

C#:   interface IShape { double Area(); }
来源：http://sss.hnqzz.top

[G10] 访问控制
来源：http://uva.316326.xyz

Py:   约定 _protected / __private（不强制）
来源：http://jtm.wangdashe.top

PHP:  public / protected / private
来源：http://fix.feifeiyinyue.top

JS:   #private 字段；其余公开
来源：http://aug.iojbl.cn

TS:   public / protected / private
来源：http://ygo.yangfankeji.com

Java: public / protected / private / 默认包级
来源：http://hws.kuanghao11.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ihx.haohaochexian.top

Ruby: public / protected / private
来源：http://hwp.fehbvm.com

C#:   public / protected / private / internal
来源：http://ttx.zhongyouzk.top

[G11] getter / setter
来源：http://fxx.tian-w.cn

Py:   @property 与 @x.setter
来源：http://xuf.xingfuxueyuan.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://cfk.uphjek.com

JS:   get name() { return this._name; }
来源：http://gyn.cashguo.top

TS:   get name(): string { return this._name; }
来源：http://gvf.jqgufenzy.top

Java: public String getName() { return name; }
来源：http://xhv.zhiwuduotai.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://mru.zhaomingkeji.xyz

Ruby: attr_accessor :name
来源：http://keo.yj20258888.top

C#:   public string Name { get; set; }
来源：http://ctp.fzhhl.top

[G12] 对象转字符串
来源：http://fbt.sxryk.cn

Py:   def __str__(self): return self.name
来源：http://qfh.52xcode.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qqh.0kj1m.cn

JS:   toString() { return this.name; }
来源：http://gwg.sweek.top

TS:   toString(): string { return this.name; }
来源：http://lye.uphjek.com

Java: @Override public String toString() { return name; }
来源：http://rpe.kuanghao11.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zmj.316326.xyz

Ruby: def to_s; @name; end
来源：http://obt.ctjpmb.com

C#:   public override string ToString() => Name;
来源：http://cym.daxiang520.top

[G13] 判断对象类型
来源：http://lxm.gogol.net.cn

Py:   isinstance(u, User)
来源：http://gjs.chenlongwang.top

PHP:  $u instanceof User
来源：http://owg.epnwcf.com

JS:   u instanceof User
来源：http://mgn.epnwcf.com

TS:   u instanceof User
来源：http://knj.andypj.xyz

Java: u instanceof User
来源：http://xlc.jinqigufen.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://zsg.jqgufenzy.top

Ruby: u.is_a?(User)
来源：http://hji.cucudq.cn

C#:   u is User
来源：http://dms.gotoacloud.top

[G14] 数据类 / record
来源：http://xcj.jinqigufen.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zmk.iojbl.cn

PHP:  // 用 readonly 属性模拟
来源：http://kdh.bbcook.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wnx.pycfn.com


<!-- 参考信息 -->