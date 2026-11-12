代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://siv.tanke756.top

TS:   // 同上，务必做 XSS 过滤
来源：http://xkv.nanxinkj.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vhn.9152youxi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://slc.0kj1m.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ryr.hfpthk.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vft.fanxiaobao.xyz

[E16] 数字千分位
来源：http://cbh.yj20258.top

Py:   f"{1234567:,}"
来源：http://kff.fehbvm.com

PHP:  number_format(1234567);
来源：http://ses.xuanzx.com

JS:   (1234567).toLocaleString("en-US")
来源：http://loi.hysaishi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://otm.sjlbkw.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://eyd.ehwqpu.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dqw.ehwqpu.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fnz.jinghuilouyu.cn

C#:   1234567.ToString("N0")
来源：http://lyz.iojbl.cn

[E17] 首字母大写
来源：http://svw.daxiang520.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xyx.feifeiyinyue.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://rub.shanyushiyangkeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bky.zycfv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ors.fzhhl.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xab.xylfe.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vju.hysaishi.cn

Ruby: s.capitalize
来源：http://shv.yvedp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ztx.chenzaomai.com

[E18] 模板占位符替换
来源：http://ged.fehbvm.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sur.dashuyun.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wga.mhx1999.top

JS:   tpl.replaceAll("{name}", name)
来源：http://odx.yfazqb.com

TS:   tpl.replaceAll("{name}", name)
来源：http://vti.xuanzx.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fkd.aizwys.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://oix.yvedp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hxu.birdmap.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hbw.shanyushiyangkeji.top

[E19] 多行文本按行拆分
来源：http://zex.ywan-chungtsiang.top

Py:   s.splitlines()
来源：http://ikl.aizwys.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qlv.jinyuanbaomall.cn

JS:   s.split(/\r?\n/)
来源：http://kcz.316326.xyz

TS:   s.split(/\r?\n/)
来源：http://huj.pengpengdd.cyou

Java: s.lines().toList()
来源：http://bvi.shuidangran.top

Go:   strings.Split(s, "\n")
来源：http://jqc.pycfn.com

Ruby: s.lines
来源：http://wla.hnxiangtu.top

C#:   s.Split('\n')
来源：http://gvq.meibo888.top

[E20] 判断字符串是否为空
来源：http://adv.hnqzz.top

Py:   if not s:
来源：http://xet.wangdashe.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rzu.aizwys.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ydk.haohaochexian.top

TS:   if (s === "") {}
来源：http://qbc.ybcxt.top

Java: if (s.isEmpty()) {}
来源：http://cvk.ywan-chungtsiang.top

Go:   if s == "" {}
来源：http://khw.zhengqikj.top

Ruby: if s.empty?
来源：http://mfn.cqqwz.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wku.aizwys.cn

[E21] 超长截断加省略号
来源：http://lci.fktsv.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nmi.andypj.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cbx.hnxiangtu.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eet.yonumen.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qqg.zhiwuduotai.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://voz.fengsongda.top

Go:   // 按 rune 判断长度后截断
来源：http://xhc.haohaochexian.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qhx.yuxming.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://izy.xinyue.icu

[E22] 字节长度与字符长度
来源：http://dzp.gogol.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kzo.fengsongda.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hcv.yueranfly.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nhe.ctjpmb.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yii.52xcode.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qxx.0kj1m.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qvi.fzhhl.top

Ruby: s.bytesize;  s.length
来源：http://ezv.birdmap.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cqz.hammf.cn

================================================================================
来源：http://flh.zycfv.cn

F. 文件与目录
来源：http://iws.pengpengdd.cyou

================================================================================
来源：http://jwd.haohaochexian.top

[F01] 读取整个文件
来源：http://sxw.ydjk.org.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bzr.shzxlz.cn

PHP:  file_get_contents("a.txt");
来源：http://bti.sxryk.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rly.hesvh.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://goq.tianlin.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://axv.fehbvm.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mly.kuanghao11.cn

Ruby: File.read("a.txt")
来源：http://qma.meibo888.top

C#:   File.ReadAllText("a.txt");
来源：http://taw.hysaishi.cn

[F02] 逐行读取文件
来源：http://pwm.nwbrower.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fhr.aibaodan.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sbj.jinghuilouyu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oqu.hnqzz.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tkn.bjfxy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vzf.fehbvm.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hah.sufxvd.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qec.sxryk.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://oxh.redwolf501.top

[F03] 写入文件（覆盖）
来源：http://nxj.jinyuanbaomall.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mox.shanyushiyangkeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://bsn.yueranfly.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tsa.ehwqpu.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lkn.xuanzx.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://iuq.guannengcc.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bxf.0kj1m.cn

Ruby: File.write("a.txt", "hi")
来源：http://zmc.hongshengwenyu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zba.xziqi.cn

[F04] 追加写入文件
来源：http://qnq.xuanzx.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wmh.zycfv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zbv.bjfxy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qvl.gogol.net.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://env.tarul.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vej.tian-w.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://spm.ctjpmb.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xif.zdbjq.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yas.jlsjyb.cn

[F05] 判断文件或目录是否存在
来源：http://iam.svipenyu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fsl.dashuyun.cn

PHP:  file_exists("a.txt");
来源：http://lqq.zhaomingkeji.xyz

JS:   fs.existsSync("a.txt")
来源：http://ojd.zhongyouzk.top

TS:   fs.existsSync("a.txt")
来源：http://njv.sweek.top

Java: Files.exists(Path.of("a.txt"))
来源：http://rwh.yvedp.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ceg.yj202588.top

Ruby: File.exist?("a.txt")
来源：http://iec.gogol.net.cn

C#:   File.Exists("a.txt")
来源：http://pvn.zhijiandao.cn

[F06] 删除文件
来源：http://erx.hfpthk.cn

Py:   os.remove("a.txt")
来源：http://ifu.jinghuilouyu.cn

PHP:  unlink("a.txt");
来源：http://mdb.zhijiandao.cn

JS:   fs.unlinkSync("a.txt")
来源：http://you.yueranfly.top

TS:   fs.unlinkSync("a.txt")
来源：http://kba.shanyushiyangtech.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tfl.fzhhl.top

Go:   os.Remove("a.txt")
来源：http://nos.guannengcc.top

Ruby: File.delete("a.txt")
来源：http://ctr.guannengcc.top

C#:   File.Delete("a.txt");
来源：http://qxx.vehdjk.com

[F07] 创建目录（含多级）
来源：http://doz.shangyingyoupin.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lbx.xingfuxueyuan.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yra.dashuyun.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ikp.wangshuangyany.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ekr.gzhubu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xhy.ydzc1.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tkn.gogol.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wwj.cashguo.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pzv.svipenyu.cn

[F08] 遍历目录
来源：http://jev.hcnkem.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://fte.hammf.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://buw.kuanghao11.cn

JS:   fs.readdirSync("dir")
来源：http://kab.pycfn.com

TS:   fs.readdirSync("dir")
来源：http://dpx.yj202588.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gnu.sweek.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://lvo.yangfankeji.com

Ruby: Dir.children("dir")
来源：http://ubc.jinqigfzy.top

C#:   Directory.GetFiles("dir")
来源：http://nvj.pycfn.com

[F09] 获取文件大小
来源：http://zvw.jlsjyb.cn

Py:   os.path.getsize("a.txt")
来源：http://dlo.ydjk.org.cn

PHP:  filesize("a.txt");
来源：http://ibe.meibo888.top

JS:   fs.statSync("a.txt").size
来源：http://hxd.guowangkeji.top

TS:   fs.statSync("a.txt").size
来源：http://cbb.sufxvd.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ttt.zdqjudy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://iqa.fanxiaobao.xyz

Ruby: File.size("a.txt")
来源：http://wgw.gotoacloud.top

C#:   new FileInfo("a.txt").Length
来源：http://lma.fzhhl.top

[F10] 取文件扩展名 / 文件名
来源：http://vxo.gotoacloud.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tmc.feifeiyinyue.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xkw.hnqzz.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://apd.fktsv.cn

TS:   path.extname("a.txt")
来源：http://gyt.tianlin.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://til.xuetiantiany.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kga.tarul.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ubr.yangfankeji.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jhb.xinyue.icu

[F11] 复制与移动文件
来源：http://jtr.shzxlz.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://iuu.jlsjyb.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ton.xziqi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ghg.nanxuanxn.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wjj.ydzc1.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://snu.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uuw.xziqi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fyp.hcnkem.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bkf.cucudq.cn

[F12] CSV 读写
来源：http://xwq.mhx1999.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gvz.tanke756.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gwd.uphjek.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qtd.fehbvm.com

TS:   // 同上
来源：http://uqa.bjfxy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ocd.zhaomingkeji.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://skk.sysykeji.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://klh.52xcode.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://afz.jinyuanbaomall.cn

================================================================================
来源：http://zdk.gotoacloud.top

G. 面向对象
来源：http://ays.zhiwuduotai.top

================================================================================
来源：http://kon.yonumen.top

[G01] 定义类
来源：http://sws.redwolf501.top

Py:   class User: pass
来源：http://hqg.zhongyouzk.top

PHP:  class User {}
来源：http://mei.yj20258.top

JS:   class User {}
来源：http://wfi.sufxvd.cn

TS:   class User { name: string = ""; }
来源：http://qyv.hammf.cn

Java: class User {}
来源：http://czx.cucudq.cn

Go:   type User struct { Name string }
来源：http://zjo.tarul.cn

Ruby: class User; end
来源：http://zwe.9152youxi.cn

C#:   class User {}
来源：http://djv.andypj.xyz

[G02] 构造函数
来源：http://rfb.zhaomingkeji.xyz

Py:   def __init__(self, name): self.name = name
来源：http://iip.yuanzhike.top

PHP:  public function __construct(public string $name) {}
来源：http://uaz.zhaomingkeji.xyz

JS:   constructor(name) { this.name = name; }
来源：http://tay.snrcjt.cn

TS:   constructor(public name: string) {}
来源：http://nad.quarkkingdee.top

Java: User(String name) { this.name = name; }
来源：http://vuw.ctjpmb.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kat.epnwcf.com

Ruby: def initialize(name); @name = name; end
来源：http://mlp.uphjek.com

C#:   public User(string name) { Name = name; }
来源：http://jsl.ehwqpu.com

[G03] 实例属性
来源：http://ydg.yangfankeji.com

Py:   self.name = "x"
来源：http://evu.chenjidiqi.icu

PHP:  public string $name = "x";
来源：http://zdr.iojbl.cn

JS:   this.name = "x";
来源：http://frw.yangfankeji.com

TS:   name: string = "x";
来源：http://ujn.dianchejie.cn

Java: private String name;
来源：http://pel.fehbvm.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://irr.jinyuanbaomall.cn

Ruby: @name = "x"
来源：http://prh.jinyuanbaomall.cn

C#:   public string Name { get; set; } = "x";
来源：http://jiu.sxryk.cn

[G04] 定义方法
来源：http://vfw.havefunace.top

Py:   def greet(self): return self.name
来源：http://dkk.sweek.top

PHP:  public function greet(): string { return $this->name; }
来源：http://tkj.havefunace.top

JS:   greet() { return this.name; }
来源：http://dcc.gzhubu.top

TS:   greet(): string { return this.name; }
来源：http://ywf.jlsjyb.cn

Java: String greet() { return name; }
来源：http://twr.haohaochexian.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://omf.uphjek.com

Ruby: def greet; @name; end
来源：http://hkd.wangshuangyany.cn

C#:   public string Greet() => Name;
来源：http://ybk.jyoumei.cn

[G05] 继承
来源：http://yuh.uphjek.com

Py:   class Admin(User): pass
来源：http://xlg.xylfe.cn

PHP:  class Admin extends User {}
来源：http://yrb.aizwys.cn

JS:   class Admin extends User {}
来源：http://jnl.hnxiangtu.top

TS:   class Admin extends User {}
来源：http://jiz.chenlongwang.top

Java: class Admin extends User {}
来源：http://wpb.sxryk.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ggi.cheryme.top

Ruby: class Admin < User; end
来源：http://lct.tian-w.cn

C#:   class Admin : User {}
来源：http://pht.cdnleiting.top

[G06] 重写方法
来源：http://xsq.sysykeji.top

Py:   def greet(self): return "admin"
来源：http://vwf.hywenlv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rkz.uphjek.com

JS:   greet() { return "admin"; }
来源：http://epn.guowangkeji.top

TS:   greet(): string { return "admin"; }
来源：http://rxp.cashguo.top

Java: @Override String greet() { return "admin"; }
来源：http://mgv.ybcxt.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wvw.gotoacloud.top

Ruby: def greet; "admin"; end
来源：http://ybr.xylfe.cn

C#:   public override string Greet() => "admin";
来源：http://gch.hysaishi.cn

[G07] 调用父类方法
来源：http://lhf.birdmap.top

Py:   super().greet()
来源：http://ywn.bjfxy.top

PHP:  parent::greet();
来源：http://gzh.kuanghao11.cn

JS:   super.greet();
来源：http://yfj.guowangkeji.top

TS:   super.greet();
来源：http://rxl.gogol.net.cn

Java: super.greet();
来源：http://kht.fehbvm.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://css.jianghu66.top

Ruby: super
来源：http://zax.hcnkem.com

C#:   base.Greet();
来源：http://xhn.yuxming.cn

[G08] 静态方法与属性
来源：http://hjv.jqgufenzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zqn.zhiwuduotai.top

PHP:  public static function f() {}
来源：http://mmu.shzxlz.cn

JS:   static f() {}
来源：http://lej.cdnleiting.top

TS:   static f(): void {}
来源：http://fwt.ydzc1.top

Java: static void f() {}
来源：http://dvu.snrcjt.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bmo.ydjk.org.cn

Ruby: def self.f; end
来源：http://zru.hnqzz.top

C#:   public static void F() {}
来源：http://nal.gaohongyu789.top

[G09] 接口 / 抽象类
来源：http://fei.hnqzz.top

Py:   from abc import ABC, abstractmethod
来源：http://iys.aibaodan.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nwv.guannengcc.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://fhs.cucudq.cn

TS:   interface Shape { area(): number; }
来源：http://jti.ydjk.org.cn

Java: interface Shape { double area(); }
来源：http://udi.yj20258.top

Go:   type Shape interface { Area() float64 }
来源：http://irz.kuanghao11.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://czt.9152youxi.cn

C#:   interface IShape { double Area(); }
来源：http://scz.aibaodan.cn

[G10] 访问控制
来源：http://dob.guannengcc.top

Py:   约定 _protected / __private（不强制）
来源：http://tsb.ivvv.top

PHP:  public / protected / private
来源：http://pcw.guannengcc.top

JS:   #private 字段；其余公开
来源：http://kkq.fktsv.cn

TS:   public / protected / private
来源：http://ojf.xingfuxueyuan.xyz

Java: public / protected / private / 默认包级
来源：http://fpk.jyoumei.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xea.ctjpmb.com

Ruby: public / protected / private
来源：http://plv.fengsongda.top

C#:   public / protected / private / internal
来源：http://brh.fzhhl.top

[G11] getter / setter
来源：http://mez.vqdsnc.cn

Py:   @property 与 @x.setter
来源：http://hmk.gzhubu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ndd.nanxinkj.top

JS:   get name() { return this._name; }
来源：http://dqh.fanxiaobao.xyz

TS:   get name(): string { return this._name; }
来源：http://pll.iojbl.cn

Java: public String getName() { return name; }
来源：http://vhk.fanxiaobao.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://gaw.hammf.cn

Ruby: attr_accessor :name
来源：http://trt.fanxiaobao.xyz

C#:   public string Name { get; set; }
来源：http://lqd.cheryme.top

[G12] 对象转字符串
来源：http://hls.guannengcc.top

Py:   def __str__(self): return self.name
来源：http://hoh.yonumen.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://rqj.hnqzz.top

JS:   toString() { return this.name; }
来源：http://roh.xuetiantiany.cn

TS:   toString(): string { return this.name; }
来源：http://doj.snrcjt.cn

Java: @Override public String toString() { return name; }
来源：http://xcc.ydjk.org.cn

Go:   func (u User) String() string { return u.Name }
来源：http://pfk.gaohongyu789.top

Ruby: def to_s; @name; end
来源：http://txz.tianlin.xyz

C#:   public override string ToString() => Name;
来源：http://yka.gzhubu.top

[G13] 判断对象类型
来源：http://uvd.zhixingplan.top

Py:   isinstance(u, User)
来源：http://meq.zhijiandao.cn

PHP:  $u instanceof User
来源：http://wxe.jqgfzy.top

JS:   u instanceof User
来源：http://jop.ctjpmb.com

TS:   u instanceof User
来源：http://euv.yuxming.cn

Java: u instanceof User
来源：http://xae.cashguo.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://elj.shanyushiyangkeji.top

Ruby: u.is_a?(User)
来源：http://uar.zhengqikj.top

C#:   u is User
来源：http://hhc.316326.xyz


<!-- 参考信息 -->